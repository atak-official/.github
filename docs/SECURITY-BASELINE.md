# ROTA GitHub Security Baseline

This document defines the organization-level security baseline for the **ROTA** GitHub organization.

It does not replace repository-specific security documentation.

## Account security

All organization members with access to private resources should use GitHub two-factor authentication.

Preferred secure methods include passkeys, hardware security keys, authenticator applications, and GitHub Mobile. SMS should not be relied upon as the primary security method where a stronger option is available.

Organization Owners should keep independent recovery methods and recovery codes in secure personal storage.

## Owner security

ROTA should maintain at least two trusted Organization Owners to avoid a single point of administrative failure.

Owner access must remain exceptional. A person should not receive Owner solely because they hold an official club title.

## Base access

Organization-wide base repository permission should be kept at the lowest practical level. Private repository access should be granted intentionally through Teams or explicit repository access.

## Applications and integrations

GitHub Apps and OAuth applications with organization access should be installed only when there is a defined operational need.

Before approving an integration, review requested permissions, repository scope, whether write access is necessary, and who owns and maintains the integration.

Unused integrations should be removed.

## Personal access tokens

Prefer GitHub Apps or fine-grained personal access tokens over classic personal access tokens for organization automation.

Fine-grained tokens should request only the repositories and permissions they need, have a finite lifetime, and be reviewed before organization access is granted when supported by organization policy.

## Secrets

Secrets must not be committed to repositories.

If a secret is committed, rotate or revoke it immediately.

## Audit and review

Organization Owners should periodically review GitHub's organization audit log, especially after Owner or membership changes, GitHub App changes, repository lifecycle changes, security incidents, and leadership transitions.

## Offboarding

When a privileged member leaves a project or ROTA, promptly remove unnecessary Team/direct repository access, review Owner access, revoke relevant tokens or application access, reassign open work, and transfer infrastructure ownership where applicable.
