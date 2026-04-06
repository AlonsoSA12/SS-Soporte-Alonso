# SS Soporte Alonso

This repository stores support documentation and automation references used to track operational work across Singular-related systems.

It is a documentation repository, not an application codebase.

---

## Repository Scope

This repo currently tracks two main areas:

- `automations/`
  Documentation for automation flows and technical references such as `n8n`, `Airtable`, `Make`, `Firebase`, and `Pipedream`.

- `support-cases/`
  Support case documentation organized by sprint, including case logs, summaries, and templates.

---

## Repository Structure

```text
.
├── automations/
│   └── README.md
├── support-cases/
│   ├── README.md
│   ├── plantilla-caso-soporte.md
│   ├── sprint-99-support-cases/
│   ├── sprint-100-support-cases/
│   └── sprint-101-support-cases/
└── README.md
```

---

## How to Read This Repo

- Use [automations/README.md](./automations/README.md) to understand the automation documentation area.
- Use [support-cases/README.md](./support-cases/README.md) to understand how support cases are organized by sprint.

The root `README.md` describes the repository as a whole.  
Each internal `README.md` describes the rules and structure for its own folder.

---

## What Is Expected to Be Versioned

This repository is intended to store:

- Markdown documentation
- Sprint support records
- Templates used to create support documentation
- Supporting documentation indexes

It is not intended to store:

- application source code
- local exports or temporary files
- screenshots kept only for local reference unless intentionally documented

---

## Notes

- The support documentation can evolve by sprint without changing the overall repository structure.
- Folder-level conventions may differ slightly between sections, but the root repo should stay focused on documentation only.
