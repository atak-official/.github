# ATAK GitHub Security Baseline

This document defines the organization-level security baseline for **atak-official**.

It does not replace repository-specific security documentation.

## Account security

All organization members with access to private resources should use GitHub two-factor authentication.

Preferred secure methods:

- passkeys;
- hardware security keys;
- authenticator applications;
- GitHub Mobile.

SMS should not be relied upon as the primary security method where a stronger option is available.

Organization Owners should keep independent recovery methods and recovery codes in secure personal storage.

## Owner security

ATAK should maintain at least two trusted Organization Owners to avoid a single point of administrative failure.

Owner access must remain exceptional. A person should not receive Owner solely because they hold an official club title.

## Base access

Organization-wide base repository permission should be kept at the lowest practical level.

Private repository access should be granted intentionally through Teams or explicit repository access.

## Applications and integrations

GitHub Apps and OAuth applications with organization access should be installed only when there is a defined operational need.

Before approving an integration, review:

- requested permissions;
- repositories it can access;
- whether write access is necessary;
- whether a narrower repository selection is possible;
- who owns and maintains the integration.

Unused integrations should be removed.

## Personal access tokens

Prefer GitHub Apps or fine-grained personal access tokens over classic personal access tokens for organization automation.

Fine-grained tokens should:

- request only the repositories they need;
- request only the permissions they need;
- have a finite lifetime;
- be reviewed before organization access is granted when the organization policy supports approval.

Long-lived unrestricted tokens should be avoided.

## Secrets

Secrets must not be committed to repositories.

Examples include:

- API keys;
- Telegram bot tokens;
- database passwords;
- private keys;
- deployment credentials;
- production environment files.

If a secret is committed, rotate or revoke it immediately.

## Audit and review

Organization Owners should periodically review GitHub's organization audit log, especially after:

- Owner or membership changes;
- GitHub App installation or removal;
- repository creation, transfer, deletion, or visibility changes;
- security incidents;
- leadership transitions.

## Offboarding

When a privileged member leaves a project or ATAK:

- remove unnecessary Team membership;
- remove direct repository access;
- review Owner access;
- revoke relevant tokens or application access;
- reassign open work;
- transfer infrastructure ownership where applicable.

Offboarding should happen promptly, not at the end of the semester.
