# ATAK — GitHub Organization Profile

This repository contains the public GitHub organization profile and organization-level GitHub governance documentation for **ATAK**.

## Purpose

The `profile/README.md` file is rendered on the public `atak-official` organization page and serves as the organization-level introduction to ATAK, its working model and engineering culture.

The documents under `docs/` define high-level GitHub governance and security conventions without imposing repository-specific workflows on existing projects.

## Scope

This repository is intentionally kept conservative.

Shared community-health files, issue templates, pull-request templates, workflows, or repository-wide defaults are **not** placed here unless ATAK explicitly decides that they should apply across repositories.

Project-specific policies belong in their respective repositories.

## Structure

```text
.github/
├── README.md
├── profile/
│   └── README.md
└── docs/
    ├── GOVERNANCE.md
    ├── REPOSITORY-STANDARDS.md
    └── SECURITY-BASELINE.md
```

## Organization documentation

- [GitHub Governance](./docs/GOVERNANCE.md)
- [Repository Standards](./docs/REPOSITORY-STANDARDS.md)
- [Security Baseline](./docs/SECURITY-BASELINE.md)

## Maintenance

Changes to organization-level documentation should remain concise, deliberate, and consistent with ATAK's current structure and public identity.
