# Branching Strategy

## Purpose

This document describes a simple branching strategy for software teams that need clarity, traceability, and controlled releases.

The goal is to help teams work in parallel while protecting the stability of production-ready code.

## Recommended Branches

```text
main
develop
feature/*
hotfix/*
release/*
```

## Branch Roles

### main

The `main` branch contains stable production-ready code.

Code should only reach this branch after review, validation, and release preparation.

### develop

The `develop` branch is used as the integration branch for upcoming changes.

It allows the team to combine completed features before preparing a release.

### feature/*

Feature branches are used for new features, improvements, or planned changes.

Example:

```text
feature/email-priority-classification
```

### hotfix/*

Hotfix branches are used for urgent production fixes.

Example:

```text
hotfix/fix-login-error
```

### release/*

Release branches are used to prepare a production release.

Example:

```text
release/1.0.0
```

## Basic Flow

```text
feature/* → develop → release/* → main
```

## Principles

- Do not commit directly to `main`.
- Use pull requests for review.
- Keep branches focused and short-lived.
- Merge only after validation and approval.
- Use meaningful branch names.
- Delete branches after they are merged.
- Keep the release process visible to the team.

## Suggested Naming Convention

```text
feature/short-description
hotfix/short-description
release/version-number
bugfix/short-description
chore/short-description
```

Examples:

```text
feature/add-email-summary
bugfix/fix-priority-label
chore/update-documentation
release/1.1.0
```

## Benefits

- Better traceability
- Safer releases
- Cleaner collaboration
- Reduced production risk
- Clearer separation between development and production-ready code
