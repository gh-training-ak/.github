# Security policy

Organisation default. A repository with its own `.github/SECURITY.md` overrides this.

## Reporting a vulnerability

Use private vulnerability reporting on the repository in question. Do not open a public
issue.

We acknowledge within two working days and give a remediation plan within ten.

## Scope

These are **teaching repositories**. They are not deployed, they hold no real data, and
several of them contain deliberate problems used to demonstrate a point.

In scope: a dependency vulnerability reachable from the code, or a credential that has
genuinely leaked.

Out of scope: findings against demo environments, scanner output with no demonstrated
exploit path, and anything described in a repository as a known gap.

## If a secret leaks

Rotate it first, then tell the owners. Rewriting history does not revoke a credential,
and anybody who cloned the repository still has it.

Push protection is on across the organisation.
