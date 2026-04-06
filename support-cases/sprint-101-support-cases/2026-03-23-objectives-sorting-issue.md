# Incorrect Sorting Logic in Objectives List

## Date
2026-03-23

## Context

During the initial QA review, an issue was identified in the Objectives list where archived or completed items were being prioritized over active work.

This affected the operational reading of the project because users had to scan older items before reaching objectives that still required attention.

---

## Actions Taken

- Reviewed the behavior of the Objectives list in the reported project
- Confirmed that `Achieved` items were appearing above active or pending-review objectives
- Documented the expected behavior versus the current behavior
- Registered the issue as a UI/UX problem in QA

---

## Result

The sorting issue was documented in the QA platform with clear evidence of the incorrect prioritization logic.

---

## Time Spent

0.5 hours
