# Support Case — New Project Unable to Create OKRs

## Date

2026-03-04

---

## Overview

Jossy Solano reported that they were unable to create OKRs for a newly created project named **J2 Academy**.  
The issue occurred when accessing the **Objectives section**, where an error message appeared instead of allowing the creation of the first objective.

<img width="1045" height="461" alt="image" src="https://github.com/user-attachments/assets/9cfc107c-03de-4aac-80cf-70ed60de25d8" />

---

## Issue Description

When the user accessed the **Objectives** page for the new project, the system displayed an error message.

This occurred because the project was newly created and **did not yet have any objectives**, but the system attempted to load objective data that did not exist.

Instead of showing the initial state for creating the first objective, the interface displayed an error message.

---

## Root Cause

The Objectives page assumed that at least one objective already existed for the project.

When the project was new and contained **no objectives**, the system attempted to retrieve data that was not yet available, resulting in an error message being displayed.

---

## Resolution

The logic handling the Objectives page was adjusted so that when a project has **no existing objectives**, the system displays the initial interface to create the first objective instead of attempting to load non-existent data.

After implementing the change, the application was redeployed.

<img width="1918" height="879" alt="image" src="https://github.com/user-attachments/assets/18838636-45a8-4a41-a968-b284d7876d7c" />

---

## Result

New projects without objectives now correctly display the **initial objective creation screen**, without showing an error message.

If a user still encounters the error, it may be caused by browser caching. In such cases, opening the page in a new session or incognito window should resolve the issue.

<img width="1916" height="1017" alt="image" src="https://github.com/user-attachments/assets/92353100-04d7-4724-b833-be1aad453513" />

---

## Time Spent

0.5 hours
