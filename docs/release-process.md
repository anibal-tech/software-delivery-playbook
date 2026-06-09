# Release Process

## Purpose

This document describes a simple release process for software teams that need control, traceability, and confidence when moving changes to production.

The goal is to reduce release risk and make the delivery process visible to the team and stakeholders.

## Release Flow

```text
develop → release/* → main → production
```

## Release Preparation

Before creating a release, the team should confirm:

- Planned changes are complete.
- Pull requests were reviewed and approved.
- Critical defects were addressed.
- Documentation was updated.
- Testing was completed.
- Known risks were identified.
- Stakeholders were informed if needed.

## Release Branch

A release branch can be created from `develop`.

Example:

```text
release/1.0.0
```

The release branch should be used only for:

- Final validation
- Minor fixes
- Release notes
- Version updates
- Deployment preparation

## Release Validation

Before merging into `main`, validate:

- Main workflows
- Critical business scenarios
- Configuration changes
- Security considerations
- Data or migration impacts
- Rollback plan, if applicable

## Release Notes

Each release should include:

- Version or release name
- Release date
- Summary of changes
- New features
- Fixes
- Known issues
- Deployment notes
- Rollback considerations

## Production Deployment

Production deployment should happen only after:

- Release approval
- Validation completed
- Required communication sent
- Deployment plan confirmed
- Rollback strategy understood

## After Deployment

After deployment, the team should verify:

- Application is available.
- Critical flows work as expected.
- Logs or monitoring do not show unexpected errors.
- Stakeholders are informed.
- Release notes are updated if needed.

## Rollback Considerations

A rollback plan should be considered when:

- The release affects critical business processes.
- There are database changes.
- There are configuration changes.
- There is high operational risk.
- The deployment cannot be easily reversed.

## Release Principles

- Release small and often when possible.
- Keep the process visible.
- Avoid last-minute uncontrolled changes.
- Document what changed.
- Validate before and after deployment.
- Learn from each release.
