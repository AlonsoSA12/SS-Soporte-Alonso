# Stef Bloom Epics Visibility Fix

## Date
2026-04-06

## Context

Silvia reported that client `Stef Bloom` from the `Parabellum` project could not visualize content inside `Singular Stories`.

The issue was reproduced in the client authorization flow under `/ClientPendingApprovalStories/:clientEmail/:apiKey`, where the page loaded but remained in an empty state because the sprint selector was not being populated.

The problem was project-specific and tied to the data returned by the backend for Parabellum, not to a general frontend outage.

---

## Actions Taken

- Reviewed the report and reproduced the issue for the affected client in the `ClientPendingApprovalStories` flow.
- Confirmed that the backend call defined in `lib/backend/api_requests/api_calls.dart` was returning sprint data from `loadSprintsFromEmail`.
- Traced the frontend parsing flow through `lib/backend/schema/structs/sprint_struct.dart` and `lib/backend/schema/util/schema_util.dart`.
- Identified that the backend response included `keyProjectsBanned` values with `null`, for example `[null, "Data foundations"]`.
- Verified that `SprintStruct.fromMap` was calling `getDataList(data['keyProjectsBanned'])`, and that `getDataList` was failing on `null` values because it uses `castToType<T>(e)!`.
- Confirmed that this prevented the sprint list from being parsed correctly, which left the dropdown empty in `lib/components/sprint_component_widget.dart` and forced the empty placeholder state in `lib/pre_work_auth/client_pending_approval_stories/client_pending_approval_stories_widget.dart`.
- Downloaded the deployed source for the backend function `loadSprintsFromEmail` from production for direct inspection.
- Located the transformation logic in `cloud functions SS creation stories/loadSprintsFromEmail/LoadSprintsFromEmail/step2-transformSprintsByEmail.js`.
- Updated the function so `keyProjectsBanned` only returns non-empty string values, filtering out `null` and blank entries before sending the response back to the app.
- Deployed the updated `loadSprintsFromEmail` function to the Firebase project `singular-stories-f-f-lr5b73`.
- Re-tested the flow and confirmed with the team that the client view was restored.

---

## Result

The issue was resolved in the backend by sanitizing `keyProjectsBanned` before the response reached the FlutterFlow client.

After deployment, the sprint data parsed correctly, the sprint selector populated as expected, and Stef Bloom's client view loaded successfully again in `Singular Stories`.

This fix did not require changes to the Airtable structure or to the visible UI logic. The root cause was the presence of invalid `null` values inside the banned epics array returned by the backend.

---

## Time Spent

2 hours
