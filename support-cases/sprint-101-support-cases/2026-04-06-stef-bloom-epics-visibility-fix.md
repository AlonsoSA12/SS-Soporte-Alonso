# Stef Bloom Epics Visibility Fix

## Date
2026-04-06

## Context

Silvia reported that client `Stef Bloom` from the `Parabellum` project could not visualize content inside `Singular Stories`.

The issue required deeper review because the client view was failing due to project-specific data conditions.

---

## Actions Taken

- Reviewed the report for the affected client
- Analyzed the error returned by the project when loading the client view
- Identified that some banned epics were returning an empty value
- Corrected the behavior that was breaking the visualization
- Confirmed the fix with the team

---

## Result

The client view was restored successfully and the project loaded correctly again in `Singular Stories`.

---

## Time Spent

2 hours
