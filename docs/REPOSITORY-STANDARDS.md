# ATAK Repository Standards

This document defines organization-level conventions for repositories under **atak-official**.

It intentionally avoids imposing repository-specific workflows on existing projects.

## Naming

Repository names should use lowercase kebab-case.

Good:

- `website`
- `ctf-sunshine-2026`
- `network-monitor`

Avoid:

- `ProjectFinal`
- `new_repo_2`
- `test123`
- personal names

## Repository purpose

Every repository should have one clearly defined purpose.

Before creating a repository, the team should be able to state:

- what the repository is for;
- who maintains it;
- whether it should be public or private;
- what outcome or project it belongs to.

## Visibility

Choose visibility deliberately.

### Private

Use for:

- unreleased work;
- internal infrastructure;
- active competition work;
- internal tools;
- projects containing operational configuration that should not be public.

### Public

Use when:

- the project is intentionally open-source;
- public release has been approved by its maintainers;
- competition rules allow publication;
- no sensitive data or secrets are present.

Private visibility is not permission to commit secrets.

## Repository metadata

Public repositories should, where practical, include:

- a clear description;
- relevant topics;
- a useful README;
- project status;
- maintainer/team information;
- license information when applicable.

Avoid decorative badges that do not communicate useful project information.

## Branches and changes

Projects should prefer short-lived task branches and reviewed pull requests over long-running personal branches.

Each repository may define its own exact review and CI requirements according to project maturity and GitHub plan capabilities.

## Ownership

Repository access should preferably be managed through GitHub Teams.

Direct individual access should be used only when there is a clear reason.

A repository should not become dependent on a single maintainer.

## Archiving

When a project is no longer maintained but remains useful as technical history, archive it instead of deleting it.

Archived repositories should, when useful, state their status in the README.

## Deletion

Repository deletion should be exceptional.

Before deletion, confirm that:

- the repository is not needed for historical or audit purposes;
- no useful releases, documentation, or technical artifacts would be lost;
- archiving is insufficient.

## Public release check

Before changing a repository from private to public:

1. review commit history for secrets;
2. review files for personal or confidential information;
3. verify third-party licenses;
4. confirm competition/event publication rules;
5. ensure README and repository metadata are appropriate for public viewing.
