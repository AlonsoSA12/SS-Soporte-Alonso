# Leads Sync Issue

## Date
2026-03-04

## Context

Some leads submitted through the website form were not appearing in the Slack channel.

The system uses an automation that retrieves lead data from an Excel file and sends it to Slack using an n8n workflow.

During the review, it was identified that several records had not been processed.

<img width="761" height="436" alt="image" src="https://github.com/user-attachments/assets/7d647230-d5d9-4998-a140-baa24f7dd351" />

---

## Actions Taken

- Reviewed the n8n automation workflow
- Identified records that had not been synchronized
- Implemented a date-based filter using the `createTime` field
- Normalized the date format for comparison
- Reprocessed the pending records

<img width="863" height="460" alt="image" src="https://github.com/user-attachments/assets/025fe378-ecca-4e73-a02a-4b76aa7f38dd" />

---

## Result

The automation successfully processed the valid records and sent the corresponding notifications to Slack.

<img width="1391" height="697" alt="image" src="https://github.com/user-attachments/assets/74b04fc0-694e-4607-8102-37fffc0a16fc" />


---

## Time Spent

Approximately 30 minutes.
