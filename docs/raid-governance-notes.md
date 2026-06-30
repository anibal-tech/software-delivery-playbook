# RAID Governance Notes

## Purpose

This document provides practical notes for managing a RAID log in software delivery, transformation, migration, automation, or technology implementation initiatives.

A RAID log helps teams track and govern:

- Risks
- Actions
- Issues
- Dependencies

The goal is to improve visibility, ownership, escalation, and decision-making across technical and business teams.

## What RAID Means

## Risks

Risks are uncertain events that may happen in the future and could affect delivery, quality, cost, scope, timeline, operations, or business outcomes.

Example:

```text
There is a risk that business users may not be available for UAT during the planned execution window.
```

## Actions

Actions are tasks or follow-up items assigned to a specific owner.

Example:

```text
Confirm test data availability with the business owner by Friday.
```

## Issues

Issues are problems that are already happening and require attention, resolution, or escalation.

Example:

```text
The UAT environment is unavailable, blocking business validation.
```

## Dependencies

Dependencies are items that rely on another team, system, vendor, decision, approval, or external activity.

Example:

```text
The release depends on infrastructure team approval for firewall changes.
```

## RAID Lifecycle

A RAID item should move through a clear lifecycle.

```text
Identify
      ↓
Assess
      ↓
Assign owner
      ↓
Track progress
      ↓
Escalate when needed
      ↓
Resolve or close
      ↓
Capture lessons learned
```

## Why RAID Governance Matters

RAID governance helps teams:

- Make risks visible before they become issues
- Assign clear ownership
- Track decisions and follow-up actions
- Manage blockers and dependencies
- Improve executive reporting
- Reduce delivery surprises
- Support go-live, cutover, UAT, and hypercare readiness
- Improve stakeholder alignment

## When to Use a RAID Log

Use a RAID log for:

- Software delivery projects
- ERP or business application implementations
- Cloud migration initiatives
- Integration projects
- Process automation initiatives
- UAT execution
- Cutover planning
- Hypercare stabilization
- Vendor-managed work
- Transformation programs
- PMO governance routines

## RAID Governance Cadence

A RAID log should be reviewed regularly.

Recommended cadence:

| Project Stage | Suggested Review Frequency |
|---|---|
| Planning | Weekly |
| Development | Weekly |
| UAT | Two or three times per week |
| Cutover preparation | Daily or every checkpoint |
| Go-live | Multiple times per day |
| Hypercare | Daily |
| Stabilized BAU | As needed |

## Roles and Responsibilities

| Role | Responsibility |
|---|---|
| Project Manager / Delivery Lead | Owns the RAID process and ensures regular review |
| Technical Lead | Provides technical assessment, ownership, and mitigation plans |
| Business Owner | Confirms business impact, priority, and acceptance |
| PMO Lead | Supports governance, reporting, and escalation |
| Risk Owner | Owns mitigation or response actions |
| Action Owner | Completes assigned action items |
| Issue Owner | Drives issue resolution |
| Dependency Owner | Coordinates dependency completion |
| Executive Sponsor | Supports decisions and escalations when needed |

## Risk Assessment

Risks should be assessed based on probability and impact.

## Probability

| Level | Description |
|---|---|
| Low | Unlikely to happen |
| Medium | Could happen |
| High | Likely to happen |

## Impact

| Level | Description |
|---|---|
| Low | Minor impact, manageable within the team |
| Medium | Noticeable impact on timeline, quality, cost, or scope |
| High | Significant impact requiring leadership attention |

## Risk Priority

A simple priority model can be used:

| Probability | Impact | Priority |
|---|---|---|
| High | High | Critical |
| High | Medium | High |
| Medium | High | High |
| Medium | Medium | Medium |
| Low | High | Medium |
| Low | Medium | Low |
| Low | Low | Low |

## Issue Severity

Issues should be classified based on business or delivery impact.

| Severity | Description | Escalation |
|---|---|---|
| Critical | Blocks a critical business or delivery activity | Immediate escalation |
| High | Significant impact, but workaround may exist | Same day escalation |
| Medium | Partial impact or manageable delay | Track in regular checkpoint |
| Low | Minor impact or informational item | Normal follow-up |

## Dependency Management

Dependencies should be tracked clearly because they often create hidden delivery risk.

Each dependency should include:

- Dependency description
- Owning team or person
- Required date
- Impact if delayed
- Current status
- Escalation path
- Related risk or issue

## Escalation Principles

Escalation should not be treated as blame.

It is a mechanism to make decisions, remove blockers, and protect delivery outcomes.

Escalate when:

- A risk becomes likely or critical
- An issue blocks progress
- A dependency is delayed
- Ownership is unclear
- A decision is required
- The timeline, quality, or business outcome is at risk
- The team cannot resolve the item within the expected timeframe

## Executive Reporting

A RAID log should support executive visibility.

A good executive summary should include:

- Top risks
- Critical issues
- Overdue actions
- Blocked dependencies
- Decisions required
- Business impact
- Mitigation plan
- Owner and due date

Example format:

```text
Status:
Top risk:
Critical issue:
Blocked dependency:
Decision required:
Owner:
Target date:
```

## Common RAID Mistakes

Common mistakes include:

- Tracking items without owners
- Keeping old items open without updates
- Mixing risks and issues
- Not defining due dates
- Not escalating blocked dependencies
- Using vague descriptions
- Reporting too much detail to executives
- Not capturing business impact
- Closing items without evidence
- Reviewing the RAID log only when there is a crisis

## Good RAID Practices

Good practices include:

- Use clear descriptions
- Assign one accountable owner per item
- Define due dates
- Update status regularly
- Capture business impact
- Escalate early
- Link risks, issues, and dependencies when related
- Review critical items first
- Keep executive summaries concise
- Close items only when resolution is confirmed

## Recommended Fields

A RAID log should usually include:

- ID
- Type
- Description
- Impact
- Probability or severity
- Priority
- Owner
- Due date
- Status
- Mitigation or action plan
- Escalation required
- Last update
- Resolution notes

## Status Values

Recommended status values:

```text
New
Open
In Progress
Blocked
Escalated
Resolved
Closed
Deferred
```

## Final Principle

A RAID log is not an administrative artifact.

It is a management tool that helps teams protect delivery, improve visibility, and make better decisions before risks become surprises.
