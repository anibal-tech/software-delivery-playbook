# Sample Incident Review

## Purpose

This is a fictional and sanitized example of a post-incident review.

It is included for portfolio documentation purposes and does not represent a real company, real customer, real system, or real production incident.

## Incident Information

```text
Incident ID: INC-001
Incident title: Delayed executive reporting after deployment
System or application: Reporting Portal
Business area: Operations
Severity: High
Date detected: 2026-07-08 09:15
Date resolved: 2026-07-08 11:05
Duration: 1 hour 50 minutes
Incident owner: Support Lead
Review date: 2026-07-09
Review facilitator: Delivery Lead
```

## 1. What Happened?

After a scheduled release, the reporting portal showed delayed executive dashboard updates.

Business users could access the portal, but the latest operational metrics were not available. This affected the morning management review because stakeholders could not validate updated totals on time.

The issue was mitigated by manually triggering the reporting refresh job and validating the output with the business owner.

## 2. Impact Assessment

| Impact Area | Description |
|---|---|
| Users impacted | Operations leadership and reporting users |
| Business process impacted | Morning executive operations review |
| Customer impact | No direct customer impact |
| Operational impact | Management visibility delayed |
| Financial impact | No confirmed financial impact |
| Regulatory impact | No regulatory impact identified |
| SLA impact | Internal reporting SLA missed |
| Workaround available | Yes, manual refresh job execution |

## 3. Timeline Review

| Time | Event | Owner | Notes |
|---|---|---|---|
| 09:15 | Issue reported by business user | Business Owner | Dashboard data was not refreshed |
| 09:20 | Support ticket created | Support Lead | Classified as high severity |
| 09:30 | Technical triage started | Technical Lead | Reporting job logs reviewed |
| 09:45 | Root symptom identified | Technical Lead | Scheduled job did not trigger after deployment |
| 10:05 | Manual refresh executed | Technical Lead | Data refresh started successfully |
| 10:40 | Business validation completed | Business Owner | Dashboard totals confirmed |
| 11:05 | Incident marked resolved | Support Lead | Monitoring continued during the day |

## 4. Root Cause

The scheduled reporting refresh job was not re-enabled after deployment.

The deployment checklist included application validation but did not include validation of scheduled jobs after release execution.

## 5. Five Whys

| Why | Answer |
|---|---|
| Why did the dashboard data not refresh? | The scheduled reporting job did not run after deployment. |
| Why did the job not run? | The job was paused during deployment and not re-enabled. |
| Why was it not re-enabled? | The deployment checklist did not include that validation step. |
| Why was that step missing? | Scheduled jobs were not included in the release validation inventory. |
| What is the underlying root cause? | The release validation process did not account for scheduled job dependencies. |

## 6. What Went Well?

- Business users reported the issue quickly.
- Support team classified the incident correctly.
- Technical team identified the failed refresh path quickly.
- Manual workaround was available.
- Business owner validated the restored report output.

## 7. What Did Not Go Well?

- Scheduled job validation was missing from the deployment checklist.
- Monitoring did not alert that the job failed to run.
- The release notes did not list scheduled job dependencies.
- Executive reporting impact was not identified during release planning.

## 8. Where Did We Get Lucky?

- The issue happened during business hours when support was available.
- The refresh job could be triggered manually.
- No customer-facing process was impacted.
- No data correction was required after the refresh completed.

## 9. Corrective Actions

| ID | Action | Owner | Due Date | Status | Evidence Required |
|---|---|---|---|---|---|
| CA-001 | Add scheduled job validation to deployment checklist | Release Manager | 2026-07-12 | In Progress | Updated checklist |
| CA-002 | Add reporting job restart validation to release process | Technical Lead | 2026-07-12 | In Progress | Release validation evidence |
| CA-003 | Confirm all reporting jobs are listed in application dependency inventory | Application Owner | 2026-07-15 | Not Started | Updated dependency list |

## 10. Preventive Actions

| ID | Action | Owner | Due Date | Status | Expected Outcome |
|---|---|---|---|---|---|
| PA-001 | Add monitoring alert for missed scheduled reporting runs | Support Lead | 2026-07-18 | Not Started | Earlier detection |
| PA-002 | Include scheduled jobs in release readiness review | Release Manager | 2026-07-16 | Not Started | Lower deployment risk |
| PA-003 | Add post-deployment smoke test for executive dashboard refresh | Technical Lead | 2026-07-18 | Not Started | Faster validation |

## 11. Communication Review

| Communication Item | Result | Notes |
|---|---|---|
| Initial stakeholder notification sent | Yes | Sent after impact was confirmed |
| Executive update sent | Yes | Included expected resolution time |
| Business impact explained clearly | Yes | Reporting delay was clearly described |
| Resolution update sent | Yes | Sent after business validation |
| Final incident summary shared | Pending | To be shared after RCA approval |

## 12. Monitoring and Detection Review

| Question | Answer |
|---|---|
| Was the incident detected automatically? | No |
| Was the alert actionable? | Not applicable |
| Was detection delayed? | Yes, detection depended on business user report |
| What monitoring should be added or improved? | Alert when reporting job does not run within expected window |
| What logs or metrics were useful? | Job scheduler logs and dashboard refresh timestamp |

## 13. Process and Control Review

Identified gaps:

- Deployment validation gap
- Monitoring gap
- Documentation gap
- Release dependency inventory gap

Process or control notes:

```text
The release process should include scheduled jobs, batch processes, and reporting refresh dependencies as part of deployment validation.
```

## 14. Follow-Up Tracking

| ID | Follow-Up Item | Owner | Due Date | Status | Related Action |
|---|---|---|---|---|---|
| F-001 | Review all scheduled jobs for the reporting portal | Application Owner | 2026-07-15 | Open | CA-003 |
| F-002 | Add missed-job alert to monitoring backlog | Support Lead | 2026-07-18 | Open | PA-001 |
| F-003 | Update release checklist with job validation section | Release Manager | 2026-07-12 | Open | CA-001 |

## 15. Closure Decision

```text
Keep open for remediation tracking
```

## 16. Approval

| Name | Role | Decision | Date | Comments |
|---|---|---|---|---|
| Example Owner | Incident Owner | Approved | 2026-07-09 | RCA accepted |
| Example Lead | Technical Lead | Approved | 2026-07-09 | Actions defined |
| Example Business | Business Owner | Approved | 2026-07-09 | Business impact confirmed |
| Example Support | Support Lead | Approved | 2026-07-09 | Follow-up tracking required |

## Lessons Learned

- Scheduled jobs should be part of release dependency inventory.
- Post-deployment validation should include critical reporting flows.
- Monitoring should detect missed jobs before business users report them.
- Executive reporting processes should be treated as business-critical when they support decision-making routines.

## Privacy Notice

This example uses fictional data only.

It does not include private company data, customer information, real system names, credentials, financial data, network details, security vulnerabilities, or sensitive personal information.
