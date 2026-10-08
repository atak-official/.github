# ROTA Repository Standards

This document defines organization-level conventions for repositories belonging to **ROTA — Rekabet Odaklı Teknoloji ve Araştırma Kulübü**.

It intentionally avoids imposing repository-specific workflows on existing projects.

## Naming

Repository names should use lowercase kebab-case.

Good examples:

- `website`
- `ctf-sunshine-2026`
- `network-monitor`

Avoid temporary names such as `ProjectFinal`, `new_repo_2`, `test123`, or personal names.

## Repository purpose

Every repository should have one clearly defined purpose. Before creation, the team should be able to state what it is for, who maintains it, whether it should be public or private, and what outcome or project it belongs to.

## Visibility

Use private visibility for unreleased work, internal infrastructure, active competition work, and internal tools. Use public visibility only when the project is intentionally released and suitable for public access.

Private visibility is not permission to commit secrets.

## Repository metadata

Public repositories should, where practical, include a clear description, relevant topics, a useful README, project status, maintainer/team information, and license information when applicable.

Avoid decorative badges that do not communicate useful project information.

## Branches and changes

Projects should prefer short-lived task branches and reviewed pull requests over long-running personal branches. Each repository may define its own exact review and CI requirements according to project maturity and GitHub plan capabilities.

## Ownership

Repository access should preferably be managed through GitHub Teams. A repository should not become dependent on a single maintainer.

## Archiving and deletion

When a project is no longer maintained but remains useful as technical history, archive it instead of deleting it. Repository deletion should be exceptional.

## Public release check

Before changing a repository from private to public:

1. review commit history for secrets;
2. review files for personal or confidential information;
3. verify third-party licenses;
4. confirm competition/event publication rules;
5. ensure README and repository metadata are appropriate for public viewing.
