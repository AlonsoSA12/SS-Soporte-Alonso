# Support Case — Incorrect Project Appearing in User Dashboard

## Date

2026-03-06

---

## Overview

Laura Aguirre reported during a call that **Jossy Solano** was seeing a project in her dashboard that did not belong to her.

The project **"Singular Reclutamiento y Selección"** was appearing across different sections of the platform, which affected the user's metrics and project visibility.

---

## Issue Description

According to Laura Aguirre, user **Jossy Solano** was seeing the project **"Singular Reclutamiento y Selección"** in all platform views where projects are displayed.

This project was not actually assigned to Jossy, but it was still appearing in her project lists and metrics.

Because of this, the user's metrics were being affected by a project that was not part of her actual assignments.

---

## Investigation

After receiving the report from **Laura**, an investigation was performed to determine the origin of the incorrect project association.

This required reviewing the relationships in the **database** and performing reverse analysis to identify where the project assignment was being generated.

The analysis revealed that the project **Singular Reclutamiento y Selección** was incorrectly associated with the user **Jossy Solano** in the database.

---

## Root Cause

The project **Singular Reclutamiento y Selección** had an incorrect association with the user **Jossy Solano** in the database records.

Because of this relationship, the system included the project when calculating the user's metrics and displaying project lists across the platform.

---

## Resolution

The database records were updated to remove the incorrect association between **Jossy Solano** and the project **Singular Reclutamiento y Selección**.

Once the association was removed, the project was no longer included in the user's project lists.

---

## Result

The project **Singular Reclutamiento y Selección** no longer appears in the dashboard or project lists for **Jossy Solano**, and the user's metrics now reflect the correct information.

---

## Time Spent

0.2 hours
