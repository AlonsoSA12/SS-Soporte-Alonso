# Support Case — Client Profile Displayed as Talent

## Date

2026-03-05

---

## Overview

A user reported that one of their clients was unable to see the **Pre Work Authorization** section in the platform.

After reviewing the case, it was identified that the client account was being interpreted by the system as a **Talent profile instead of a Client profile**, which caused the interface to display the incorrect view.

---

## Issue Description

The affected user logged into the platform but was seeing the interface corresponding to a **Talent user**, not a **Client user**.

Because of this, the user could not access certain sections that are only available to clients, including the **Pre Work Authorization** functionality.

<img width="1359" height="588" alt="image" src="https://github.com/user-attachments/assets/59da5e4d-543c-445f-8c30-80fa0163113e" />

---

## Root Cause

The issue was caused by an incorrect role assignment in the **database**.

The user's email address was registered with the **Talent role** instead of the **Client role**, which caused the system to load the wrong permissions and interface.

---

## Resolution

The database record for the affected user was reviewed and updated.

The role associated with the user's email was corrected from **Talent** to **Client**.

After updating the role in the database, the user was able to access the platform with the correct permissions and interface.

<img width="1519" height="461" alt="image" src="https://github.com/user-attachments/assets/e8a69cb2-9b3e-4bd0-a9fa-51eb28309096" />



---

## Result

The client account now displays the correct **Client interface**, and the user can access the **Pre Work Authorization** section without issues.

---

## Time Spent

0.25 hours
