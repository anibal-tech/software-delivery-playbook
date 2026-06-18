# Cutover Plan Template

## Purpose

This template documents the activities, responsibilities, timing, risks, validation steps, rollback plan, and communication approach required to execute a controlled cutover.

Use this template to coordinate production releases, migrations, go-live events, integration deployments, or major business system transitions.

## Project Information

```text
Project name:
Release name:
System or application:
Business area:
Cutover date:
Cutover window:
Prepared by:
Cutover lead:
Business owner:
Technical owner:
```

## Cutover Objective

Describe the main objective of the cutover.

```text
Objective:
```

Example:

```text
Move the validated release into production and confirm that critical business flows, integrations, and reports are working as expected.
```

## Scope

Describe what is included and excluded from the cutover.

### In Scope

- Item 1
- Item 2
- Item 3

### Out of Scope

- Item 1
- Item 2

## Assumptions

List assumptions that affect the cutover plan.

- Assumption 1
- Assumption 2
- Assumption 3

## Dependencies

List technical, business, vendor, environment, data, or integration dependencies.

| Dependency | Owner | Required By | Status | Comments |
|---|---|---|---|---|
|  |  |  | Not Started / In Progress / Completed / Blocked |  |

## Roles and Responsibilities

| Role | Name | Area | Responsibility | Contact |
|---|---|---|---|---|
| Cutover Lead |  |  | Overall coordination |  |
| Business Owner |  |  | Business approval and validation |  |
| Technical Lead |  |  | Technical execution |  |
| Release Manager |  |  | Release governance |  |
| Application Owner |  |  | Application validation |  |
| Data Owner |  |  | Data validation and reconciliation |  |
| Integration Owner |  |  | Integration validation |  |
| Support Lead |  |  | Hypercare and support readiness |  |
| Communications Lead |  |  | Stakeholder communication |  |

## Execution Window

Document the planned execution windows.

| Window | Start Date/Time | End Date/Time | Owner | Notes |
|---|---|---|---|---|
| Pre-cutover preparation |  |  |  |  |
| Cutover execution |  |  |  |  |
| Technical validation |  |  |  |  |
| Business validation |  |  |  |  |
| Hypercare start |  |  |  |  |

## Pre-Cutover Checklist

Complete before starting the cutover.

- [ ] Release scope approved
- [ ] UAT sign-off completed
- [ ] Critical defects resolved or accepted
- [ ] Cutover plan reviewed
- [ ] Roles and responsibilities confirmed
- [ ] Communication plan approved
- [ ] Deployment package ready
- [ ] Configuration changes documented
- [ ] Data migration plan ready, if applicable
- [ ] Backup plan confirmed
- [ ] Rollback plan documented
- [ ] Support team available
- [ ] Vendor support confirmed, if applicable
- [ ] Monitoring or logging available
- [ ] Business validation plan ready
- [ ] Go / No-Go meeting completed

## Go / No-Go Decision

Document the cutover decision.

```text
Decision:
Go / Go with conditions / No-Go

Decision date/time:
Decision owner:
Conditions or comments:
```

## Cutover Activity Plan

Track each activity required during the cutover.

| ID | Activity | Owner | Planned Start | Planned End | Actual Start | Actual End | Status | Comments |
|---|---|---|---|---|---|---|---|---|
| 1 | Confirm cutover start | Cutover Lead |  |  |  |  | Not Started |  |
| 2 | Execute backup | Technical Lead |  |  |  |  | Not Started |  |
| 3 | Pause scheduled jobs | Technical Lead |  |  |  |  | Not Started |  |
| 4 | Deploy release package | Technical Lead |  |  |  |  | Not Started |  |
| 5 | Apply configuration changes | Application Owner |  |  |  |  | Not Started |  |
| 6 | Execute data migration | Data Owner |  |  |  |  | Not Started |  |
| 7 | Validate data migration | Data Owner |  |  |  |  | Not Started |  |
| 8 | Enable integrations | Integration Owner |  |  |  |  | Not Started |  |
| 9 | Run technical smoke tests | Technical Lead |  |  |  |  | Not Started |  |
| 10 | Execute business validation | Business Owner |  |  |  |  | Not Started |  |
| 11 | Confirm go-live outcome | Cutover Lead |  |  |  |  | Not Started |  |
| 12 | Send completion communication | Communications Lead |  |  |  |  | Not Started |  |

Recommended status values:

```text
Not Started
In Progress
Completed
Blocked
Failed
Skipped
```

## Technical Validation

Document technical validation activities.

| Validation Item | Owner | Result | Evidence | Comments |
|---|---|---|---|---|
| Application is available |  | Passed / Failed |  |  |
| Services restarted correctly |  | Passed / Failed |  |  |
| Logs reviewed |  | Passed / Failed |  |  |
| Integrations active |  | Passed / Failed |  |  |
| Scheduled jobs confirmed |  | Passed / Failed |  |  |
| Monitoring checked |  | Passed / Failed |  |  |

## Business Validation

Document business validation activities.

| Business Scenario | Owner | Result | Evidence | Comments |
|---|---|---|---|---|
| User login and access |  | Passed / Failed |  |  |
| Critical transaction flow |  | Passed / Failed |  |  |
| Report validation |  | Passed / Failed |  |  |
| Integration business outcome |  | Passed / Failed |  |  |
| Data accuracy check |  | Passed / Failed |  |  |

## Post-Cutover Validation

Complete after technical and business validation.

- [ ] Critical business flows validated
- [ ] Integrations validated
- [ ] Data reconciliation completed
- [ ] Reports validated
- [ ] Monitoring reviewed
- [ ] No critical production blockers open
- [ ] Business owner confirms acceptance
- [ ] Support team confirms readiness
- [ ] Hypercare process activated
- [ ] Completion communication sent

## Rollback Plan

Document the rollback approach.

### Rollback Decision Criteria

Rollback should be considered if:

- Critical business process cannot be executed.
- Data migration fails validation.
- Integration failures block operations.
- Production stability cannot be confirmed.
- Critical defects cannot be resolved within the agreed window.
- Business owner does not accept the cutover outcome.

### Rollback Owner

```text
Rollback owner:
Decision deadline:
Required approvals:
```

### Rollback Steps

| Step | Activity | Owner | Estimated Duration | Status | Comments |
|---|---|---|---|---|---|
| 1 | Confirm rollback decision |  |  | Not Started |  |
| 2 | Notify stakeholders |  |  | Not Started |  |
| 3 | Disable new release components |  |  | Not Started |  |
| 4 | Restore backup or previous version |  |  | Not Started |  |
| 5 | Re-enable previous integrations |  |  | Not Started |  |
| 6 | Validate restored state |  |  | Not Started |  |
| 7 | Confirm business continuity |  |  | Not Started |  |
| 8 | Send rollback completion communication |  |  | Not Started |  |

## Risks and Issues

| ID | Risk or Issue | Impact | Owner | Mitigation | Status |
|---|---|---|---|---|---|
| R-001 |  | High / Medium / Low |  |  | Open |
| R-002 |  | High / Medium / Low |  |  | Open |

## Executive Communication Plan

Document key communications.

| Communication | Audience | Owner | Timing | Channel | Status |
|---|---|---|---|---|---|
| Cutover start notification |  |  |  | Email / Teams / Slack | Not Started |
| Progress update |  |  |  | Email / Teams / Slack | Not Started |
| Go-live confirmation |  |  |  | Email / Teams / Slack | Not Started |
| Issue escalation |  |  |  | Email / Teams / Slack | Not Started |
| Completion notification |  |  |  | Email / Teams / Slack | Not Started |

## Executive Status Update Format

Use this format for concise executive communication.

```text
Status:
Completed:
In progress:
Risks / Issues:
Business impact:
Decision required:
Next update:
```

## Hypercare Plan

Document the stabilization approach after cutover.

```text
Hypercare start:
Hypercare end:
Support hours:
Support channel:
Daily checkpoint time:
Escalation contact:
Exit criteria:
```

## Cutover Completion Criteria

The cutover can be considered complete when:

- [ ] Technical activities are completed.
- [ ] Critical business flows are validated.
- [ ] Data validation is completed.
- [ ] Integrations are confirmed.
- [ ] No critical blockers remain open.
- [ ] Business owner confirms acceptance.
- [ ] Support team is ready.
- [ ] Hypercare process is active.
- [ ] Stakeholders are informed.

## Final Approval

| Name | Role | Decision | Date | Comments |
|---|---|---|---|---|
|  | Business Owner | Approved / Not Approved |  |  |
|  | Technical Owner | Approved / Not Approved |  |  |
|  | Cutover Lead | Approved / Not Approved |  |  |
|  | Release Manager | Approved / Not Approved |  |  |

## Final Notes

```text
Final notes:
```

## Privacy Notice

This template should not include private customer data, passwords, credentials, access tokens, API keys, or sensitive personal information.

Use sanitized or fictional data when sharing this document publicly.
