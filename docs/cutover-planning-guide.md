# Cutover Planning Guide

## Purpose

This guide helps teams plan and execute a controlled cutover from a current state to a new solution, system version, process, or production release.

A cutover is the coordinated set of activities required to move from an existing operating model to a new one with minimum disruption, clear ownership, and controlled risk.

## When to Use This Guide

Use this guide for:

- Production releases
- System migrations
- ERP or business application deployments
- Integration go-lives
- Cloud migration events
- Major configuration changes
- Data migration activities
- Business process transitions
- Operational handovers

## Cutover Objective

The objective of a cutover is to move a validated solution into production or operational use in a controlled, traceable, and coordinated way.

A good cutover plan should answer:

- What will change?
- When will it change?
- Who is responsible?
- What activities must happen before, during, and after the cutover?
- How will success be validated?
- What happens if something goes wrong?
- Who needs to be informed?

## Cutover Overview

```text
Pre-cutover preparation
      ↓
Go / No-Go decision
      ↓
Cutover execution
      ↓
Production validation
      ↓
Business confirmation
      ↓
Hypercare / stabilization
      ↓
Handover to operations
```

## 1. Scope and Objectives

Before planning the cutover, confirm the scope.

- [ ] Cutover objective is documented.
- [ ] In-scope systems are identified.
- [ ] In-scope business processes are identified.
- [ ] In-scope integrations are identified.
- [ ] Out-of-scope items are documented.
- [ ] Dependencies are listed.
- [ ] Expected business impact is understood.
- [ ] Success criteria are defined.

## 2. Roles and Responsibilities

A cutover requires clear ownership. Every activity should have an accountable owner.

Common roles include:

| Role | Responsibility |
|---|---|
| Cutover Lead | Coordinates the full cutover plan and execution |
| Business Owner | Confirms business readiness and validates outcome |
| Technical Lead | Coordinates technical execution and troubleshooting |
| Release Manager | Manages release governance and approvals |
| Application Owner | Validates application readiness |
| Infrastructure Owner | Supports servers, cloud, network, or platform dependencies |
| Integration Owner | Validates integrations and interfaces |
| Data Owner | Validates data migration, data quality, and reconciliation |
| Support Lead | Prepares support model and hypercare readiness |
| Communications Lead | Coordinates stakeholder communication |

## 3. Execution Windows

The execution window defines when cutover activities will take place.

Consider:

- Business operating hours
- Low-impact execution periods
- System availability windows
- Vendor availability
- Support team availability
- Time zone dependencies
- Backup and rollback windows
- Validation time
- Communication timing

Example:

```text
Cutover window:
Start: Friday 22:00
End: Saturday 04:00

Validation window:
Start: Saturday 04:00
End: Saturday 08:00

Business confirmation:
Saturday 09:00
```

## 4. Pre-Cutover Checklist

Before starting cutover execution, confirm readiness.

- [ ] Release scope is approved.
- [ ] UAT sign-off is completed.
- [ ] Open critical defects are resolved or accepted.
- [ ] Cutover plan is reviewed.
- [ ] Roles and responsibilities are confirmed.
- [ ] Communication plan is approved.
- [ ] Deployment package is ready.
- [ ] Configuration changes are documented.
- [ ] Data migration plan is ready, if applicable.
- [ ] Backup plan is confirmed.
- [ ] Rollback plan is documented.
- [ ] Support team is available.
- [ ] Vendors are available, if applicable.
- [ ] Monitoring or logging is available.
- [ ] Business validation plan is ready.
- [ ] Go / No-Go meeting is scheduled.

## 5. Go / No-Go Decision

A Go / No-Go decision should happen before cutover execution.

Review:

- Business readiness
- Technical readiness
- Environment readiness
- Data readiness
- Support readiness
- Risk status
- Open defects
- Rollback feasibility
- Stakeholder alignment

Possible decisions:

```text
Go
Go with conditions
No-Go
```

A `Go with conditions` decision should include clear ownership, risk acceptance, and mitigation actions.

## 6. Cutover Execution Activities

During cutover, all activities should be tracked and time-boxed.

Examples of cutover activities:

- Freeze business transactions, if required
- Take system backup
- Stop scheduled jobs
- Disable or pause integrations
- Deploy application changes
- Apply configuration changes
- Execute data migration
- Validate migrated data
- Restart required services
- Enable integrations
- Run smoke tests
- Validate core business flows
- Confirm system access
- Monitor logs and errors
- Communicate progress

## 7. Activity Tracking

Each cutover activity should include:

- Activity ID
- Description
- Owner
- Planned start time
- Planned end time
- Actual start time
- Actual end time
- Status
- Comments or issues

Recommended activity statuses:

```text
Not Started
In Progress
Completed
Blocked
Failed
Skipped
```

## 8. Post-Cutover Validation

After execution, validate that the solution is working as expected.

Validation should include:

- Application availability
- User access
- Critical business flows
- Integration status
- Data accuracy
- Report availability
- Performance checks
- Error logs
- Monitoring alerts
- Business confirmation

## 9. Business Validation

Business users should validate the most critical operational scenarios.

Examples:

- Can users access the system?
- Can users complete critical transactions?
- Are reports showing expected data?
- Are integrations working?
- Are business rules behaving as expected?
- Are there any blocking issues?

## 10. Rollback Plan

A rollback plan defines how to return to the previous state if the cutover fails or creates unacceptable business risk.

The rollback plan should include:

- Rollback decision criteria
- Rollback owner
- Technical rollback steps
- Data rollback considerations
- Communication steps
- Validation after rollback
- Maximum rollback decision time
- Business impact of rollback

Rollback decision examples:

```text
Rollback if critical business process cannot be executed.
Rollback if data migration fails validation.
Rollback if integration failures block operations.
Rollback if production stability cannot be confirmed within the agreed window.
```

## 11. Executive Communication

Cutover communication should be clear, concise, and timely.

Executive updates should include:

- Current status
- Key milestones completed
- Open risks or issues
- Business impact
- Decision required, if any
- Next update timing

Example update:

```text
Status: In progress
Completed: Deployment package applied and services restarted
In progress: Business validation
Risk: One integration delay under review
Next update: 30 minutes
Decision required: None at this time
```

## 12. Hypercare and Stabilization

After cutover, teams should enter a stabilization or hypercare period.

Hypercare should include:

- Dedicated support window
- Daily checkpoints
- Issue triage
- Business feedback tracking
- Known issue management
- Escalation process
- Operational handover criteria

## 13. Cutover Exit Criteria

Cutover can be considered complete when:

- Critical technical activities are completed.
- Critical business flows are validated.
- Data validation is completed.
- Integrations are confirmed.
- No critical blockers remain open.
- Business owner confirms acceptance.
- Support team is ready.
- Hypercare process is active.
- Stakeholders are informed.

## Common Risks

- Activities do not have clear owners.
- Execution window is too short.
- Rollback plan is incomplete.
- Business validation is not clearly defined.
- Dependencies are discovered too late.
- Communication is delayed or unclear.
- Critical defects are accepted without risk understanding.
- Support team is not prepared.
- Data reconciliation is not completed.

## Recommended Artifacts

Useful artifacts for cutover planning include:

- Cutover plan
- Activity tracker
- Go / No-Go checklist
- Rollback plan
- Communication plan
- Business validation checklist
- Risk and issue log
- Hypercare plan
- Executive status update

## Final Principle

Cutover is not just a technical deployment.

It is a coordinated business transition that requires planning, ownership, communication, validation, and risk control.
