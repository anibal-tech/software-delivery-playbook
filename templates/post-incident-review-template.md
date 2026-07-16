# Post-Incident Review Template

## Purpose

This template helps teams conduct a structured post-incident review after a production, operational, integration, data, or business process incident.

The review should be blameless, factual, and focused on improvement.

## Incident Information

```text
Incident ID:
Incident title:
System or application:
Business area:
Severity:
Date detected:
Date resolved:
Duration:
Incident owner:
Review date:
Review facilitator:
```

## Review Participants

| Name | Role | Area | Responsibility |
|---|---|---|---|
|  | Incident Owner |  | Overall incident accountability |
|  | Technical Lead |  | Technical analysis |
|  | Business Owner |  | Business impact validation |
|  | Support Lead |  | Support process review |
|  | Release Manager |  | Change or deployment context |
|  | Communications Lead |  | Stakeholder communication review |

## 1. What Happened?

Summarize the incident in plain language.

```text
Summary:
```

Useful questions:

- What service, process, or system was affected?
- What symptoms were observed?
- Who detected the issue?
- What business process was impacted?
- How was the issue resolved?

## 2. Impact Assessment

| Impact Area | Description |
|---|---|
| Users impacted |  |
| Business process impacted |  |
| Customer impact |  |
| Operational impact |  |
| Financial impact |  |
| Regulatory impact |  |
| SLA impact |  |
| Workaround available | Yes / No |

## 3. Timeline Review

| Time | Event | Owner | Notes |
|---|---|---|---|
|  | Incident detected |  |  |
|  | Triage started |  |  |
|  | Stakeholders informed |  |  |
|  | Mitigation started |  |  |
|  | Service restored |  |  |
|  | Business validation completed |  |  |
|  | Incident closed |  |  |

## 4. Root Cause

Document the confirmed root cause.

```text
Root cause:
```

Distinguish between:

| Type | Description |
|---|---|
| Symptom | What was visible or experienced |
| Trigger | What started the incident |
| Root cause | The underlying reason the incident happened |
| Contributing factor | Something that made the incident more likely or harder to resolve |

## 5. Five Whys

| Why | Answer |
|---|---|
| Why 1 |  |
| Why 2 |  |
| Why 3 |  |
| Why 4 |  |
| Why 5 |  |

## 6. What Went Well?

Capture strengths in the response.

- Item 1
- Item 2
- Item 3

Examples:

- Monitoring detected the issue quickly.
- Support team escalated correctly.
- Business owner was available for validation.
- Rollback plan was clear.
- Communication was timely.

## 7. What Did Not Go Well?

Capture improvement areas.

- Item 1
- Item 2
- Item 3

Examples:

- Alert did not include enough context.
- Ownership was unclear.
- Runbook was outdated.
- Business impact was not assessed early.
- Communication cadence was not defined.

## 8. Where Did We Get Lucky?

Identify areas where the impact could have been worse.

- Item 1
- Item 2
- Item 3

This section helps teams avoid relying on luck as a control.

## 9. Corrective Actions

| ID | Action | Owner | Due Date | Status | Evidence Required |
|---|---|---|---|---|---|
| CA-001 |  |  |  | Not Started |  |
| CA-002 |  |  |  | Not Started |  |

## 10. Preventive Actions

| ID | Action | Owner | Due Date | Status | Expected Outcome |
|---|---|---|---|---|---|
| PA-001 |  |  |  | Not Started |  |
| PA-002 |  |  |  | Not Started |  |

## 11. Communication Review

| Communication Item | Result | Notes |
|---|---|---|
| Initial stakeholder notification sent | Yes / No |  |
| Executive update sent | Yes / No |  |
| Business impact explained clearly | Yes / No |  |
| Resolution update sent | Yes / No |  |
| Final incident summary shared | Yes / No |  |

## 12. Monitoring and Detection Review

| Question | Answer |
|---|---|
| Was the incident detected automatically? |  |
| Was the alert actionable? |  |
| Was detection delayed? |  |
| What monitoring should be added or improved? |  |
| What logs or metrics were useful? |  |

## 13. Process and Control Review

Review whether process or control gaps contributed to the incident.

- [ ] Change management gap
- [ ] Deployment validation gap
- [ ] Testing gap
- [ ] Monitoring gap
- [ ] Access control gap
- [ ] Documentation gap
- [ ] Support handover gap
- [ ] Vendor coordination gap
- [ ] Business validation gap

Notes:

```text
Process or control gaps:
```

## 14. Follow-Up Tracking

| ID | Follow-Up Item | Owner | Due Date | Status | Related Action |
|---|---|---|---|---|---|
| F-001 |  |  |  | Open |  |
| F-002 |  |  |  | Open |  |

## 15. Closure Decision

Select one:

```text
Ready to close
Keep open for remediation tracking
Escalate to governance forum
```

## 16. Approval

| Name | Role | Decision | Date | Comments |
|---|---|---|---|---|
|  | Incident Owner | Approved / Not Approved |  |  |
|  | Technical Lead | Approved / Not Approved |  |  |
|  | Business Owner | Approved / Not Approved |  |  |
|  | Support Lead | Approved / Not Approved |  |  |

## Privacy Notice

Do not include private customer data, passwords, credentials, access tokens, API keys, network details, confidential vulnerabilities, or sensitive personal information.

Use sanitized or fictional data when sharing incident review examples publicly.
