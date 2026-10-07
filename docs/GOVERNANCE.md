# ATAK GitHub Governance

This document defines the organization-level governance model for the **ATAK** GitHub organization.

It applies to organization ownership, access management, teams, repository lifecycle, and continuity. Project-specific engineering rules remain the responsibility of each repository.

## 1. Principles

ATAK's GitHub organization follows five principles:

1. **Least privilege** — access is granted only to the level required for the work.
2. **Role separation** — university/club titles do not automatically imply GitHub administrative privileges.
3. **Team-based access** — repository permissions should be assigned to GitHub Teams instead of directly to individuals whenever practical.
4. **Continuity** — no critical repository, credential, or organization capability should depend on one individual.
5. **Traceability** — significant administrative changes should be reviewable through GitHub's audit trail and documented handover processes.

## 2. Organization ownership

The organization should maintain **at least two trusted Owners**.

Owner access is reserved for people who must administer the organization itself. Being a club president, board member, team lead, or project maintainer does not automatically require Owner access.

Owners are responsible for:

- organization security settings;
- membership and access governance;
- GitHub App and integration review;
- recovery and continuity;
- periodic audit-log review;
- transferring administrative responsibility when leadership changes.

Owner access should be reviewed at least once per academic term and immediately when an Owner leaves the organization.

## 3. Teams

GitHub Teams should represent technical responsibility, not permanent academic departments.

Recommended long-lived administrative team:

- **platform-maintainers** — maintains organization-level GitHub conventions and shared technical infrastructure.

Project teams should be created around real work, for example:

- `atak-hub`
- `website`
- `ctf-<event>-<year>`
- `project-<name>`

Permanent teams such as `cyber`, `ai`, or `cloud` should not be created merely to mirror areas of interest unless an ongoing operational need justifies them.

Teams should remain visible unless there is a legitimate security reason to make them secret.

## 4. Repository access model

Use the lowest repository role that satisfies the task:

| Role | Typical ATAK use |
| --- | --- |
| Read | Read-only access where needed |
| Triage | Issue/PR management without code changes |
| Write | Active contributors |
| Maintain | Project/team maintainers |
| Admin | Exceptional cases only |

Whenever practical, access should be granted to a Team rather than directly to an individual.

## 5. Repository lifecycle

Repositories should have a clear purpose before creation.

Recommended naming convention:

- lowercase;
- kebab-case;
- short and descriptive.

Examples:

- `website`
- `ctf-sunshine-2026`
- `network-monitor`

Avoid temporary names such as `final`, `new`, `test2`, or personal names.

A repository should normally be:

- **Private** while it contains internal, unreleased, or competition-sensitive work;
- **Public** when the project is intentionally released and suitable for public access;
- **Archived** when it is no longer actively maintained but should remain part of ATAK's technical history.

Repositories should be deleted only when there is a clear reason that archiving is insufficient.

## 6. Personal data and secrets

GitHub repositories are not a storage location for:

- passwords;
- API keys;
- bot tokens;
- private keys;
- production `.env` files;
- student records;
- personal identifiers that are not necessary for software development.

A committed secret must be treated as compromised and rotated; removing it from a later commit is not sufficient.

## 7. Administrative continuity

Critical organization resources must be transferable.

When an administrative member leaves:

1. review Owner status;
2. remove unnecessary Team and repository access;
3. transfer repository maintainership where necessary;
4. review GitHub Apps and tokens related to the member;
5. ensure open work is reassigned;
6. document anything required by the next maintainer.

## 8. Review cadence

At minimum, ATAK should perform an organization-access review:

- at the beginning of each academic term;
- after leadership changes;
- after a security incident;
- when a privileged member leaves.

The review should cover Owners, members, outside collaborators, Teams, installed GitHub Apps, token access, and recent administrative audit-log events.
