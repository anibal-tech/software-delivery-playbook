# Incident RCA Template

## Purpose

This template helps teams document the root cause analysis of an incident in a structured, practical, and improvement-oriented way.

Root Cause Analysis, also known as RCA, is used to understand what happened, why it happened, how it was resolved, and what actions should be taken to prevent recurrence.

The goal is not to assign blame. The goal is to improve systems, processes, communication, monitoring, controls, and operational readiness.

## When to Use This Template

Use this template after:

- Production incidents
- Major service interruptions
- Failed deployments
- Integration failures
- Data quality incidents
- Security or access-related issues
- Customer-impacting defects
- Business process disruptions
- Regulatory or operational risk events
- Repeated incidents with similar symptoms

## Incident RCA Overview

```text
Incident detected
      ↓
Impact assessed
      ↓
Containment or mitigation applied
      ↓
Service restored
      ↓
Root cause investigated
      ↓
Corrective actions defined
      ↓
Preventive actions implemented
      ↓
Lessons learned captured
```

## 1. Incident Summary

Provide a short summary of the incident.

```text
Incident ID:
Incident title:
Date detected:
Date resolved:
System or application:
Business area:
Severity:
Incident owner:
Technical owner:
Business owner:
```

## 2. Executive Summary

Write a concise summary for leadership or stakeholders.

The executive summary should explain:

- What happened
- Who or what was impacted
- How long the impact lasted
- What was done to restore service
- What caused the incident
- What actions will prevent recurrence

Example format:

```text
On [date], [system/process] experienced [issue], affecting [users/process/business area].
The incident caused [business impact] for approximately [duration].
The team mitigated the issue by [action].
The root cause was identified as [root cause].
Corrective and preventive actions have been defined to reduce recurrence.
```

## 3. Incident Classification

Classify the incident clearly.

| Field | Value |
|---|---|
| Severity | Critical / High / Medium / Low |
| Impact type | Availability / Performance / Data / Security / Integration / Process |
| Business impact | Critical / High / Medium / Low |
| Customer impact | Yes / No |
| Regulatory impact | Yes / No / Under Review |
| Financial impact | Yes / No / Under Review |
| Recurrence | First occurrence / Repeated issue |
| Status | Open / Under Review / Resolved / Closed |

## 4. Business Impact

Describe the impact from a business perspective.

Useful questions:

- Which users, customers, teams, or processes were affected?
- Was revenue, billing, fulfillment, reporting, compliance, or customer experience impacted?
- Were any SLAs or operational commitments missed?
- Was there any manual workaround?
- Was executive or regulatory communication required?

Impact summary:

```text
Affected users or teams:
Affected business process:
Start of impact:
End of impact:
Total duration:
Workaround available:
Business impact:
```

## 5. Timeline

Document the incident timeline.

| Time | Event | Owner | Notes |
|---|---|---|---|
|  | Incident detected |  |  |
|  | Initial triage started |  |  |
|  | Business impact confirmed |  |  |
|  | Mitigation started |  |  |
|  | Service restored |  |  |
|  | Root cause investigation started |  |  |
|  | RCA completed |  |  |
|  | Corrective actions defined |  |  |

## 6. Detection

Explain how the incident was detected.

Possible detection sources:

- Monitoring alert
- User report
- Business team notification
- Support ticket
- Log review
- Failed job
- Integration error
- Data reconciliation
- Vendor notification
- Security alert

Detection details:

```text
How was the incident detected?
Was detection automatic or manual?
Was the alert timely?
Was the alert clear?
Could detection have happened earlier?
```

## 7. Immediate Response

Describe the initial response.

- [ ] Incident owner assigned
- [ ] Severity confirmed
- [ ] Business impact assessed
- [ ] Technical triage started
- [ ] Communication channel created
- [ ] Stakeholders informed
- [ ] Mitigation options reviewed
- [ ] Workaround identified, if applicable
- [ ] Escalation triggered, if needed

## 8. Mitigation and Resolution

Document what was done to contain, mitigate, or resolve the incident.

| Action | Owner | Time | Result |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |

Key questions:

- What action restored service?
- Was the fix temporary or permanent?
- Was a workaround used?
- Were any rollback steps executed?
- Was vendor support required?
- Was business validation completed after resolution?

## 9. Root Cause Analysis

Describe the root cause of the incident.

A root cause should explain why the incident happened, not only what symptom was observed.

Avoid vague statements like:

```text
Human error
System failure
Process issue
```

Prefer specific statements like:

```text
The deployment checklist did not include validation of the integration configuration, so an incorrect endpoint was promoted to production.
```

## 10. Five Whys Analysis

Use the Five Whys technique to go deeper.

| Question | Answer |
|---|---|
| Why did the incident happen? |  |
| Why did that condition exist? |  |
| Why was it not detected earlier? |  |
| Why did the process or control fail? |  |
| What is the underlying root cause? |  |

## 11. Contributing Factors

Identify factors that contributed to the incident.

Examples:

- Missing validation step
- Incomplete test coverage
- Monitoring gap
- Configuration drift
- Manual deployment step
- Unclear ownership
- Incomplete documentation
- Environment difference
- Integration dependency
- Insufficient rollback plan
- Late stakeholder communication

Contributing factors:

- Factor 1:
- Factor 2:
- Factor 3:

## 12. Corrective Actions

Corrective actions fix the current issue.

| ID | Corrective Action | Owner | Due Date | Status | Validation Method |
|---|---|---|---|---|---|
| CA-001 |  |  |  | Not Started |  |
| CA-002 |  |  |  | Not Started |  |

## 13. Preventive Actions

Preventive actions reduce the chance of recurrence.

| ID | Preventive Action | Owner | Due Date | Status | Expected Outcome |
|---|---|---|---|---|---|
| PA-001 |  |  |  | Not Started |  |
| PA-002 |  |  |  | Not Started |  |

Examples of preventive actions:

- Add monitoring alert
- Update release checklist
- Add automated validation
- Improve test coverage
- Document operational runbook
- Add approval gate
- Improve rollback plan
- Update access control process
- Add integration health check
- Define clearer ownership

## 14. Communication Review

Review communication effectiveness.

- [ ] Incident communication started on time
- [ ] Stakeholders were identified correctly
- [ ] Business impact was communicated clearly
- [ ] Executive updates were concise
- [ ] Status updates had a defined cadence
- [ ] Resolution communication was sent
- [ ] Post-incident summary was shared

Communication notes:

```text
What communication worked well?
What communication should improve?
Were the right people involved at the right time?
Was the business impact clear?
```

## 15. Operational and Control Gaps

Identify gaps in process, controls, monitoring, documentation, or ownership.

| Gap | Impact | Improvement Needed | Owner |
|---|---|---|---|
|  |  |  |  |

Possible gap areas:

- Monitoring
- Alerting
- Testing
- Deployment process
- Access management
- Data validation
- Integration validation
- Documentation
- Incident escalation
- Business validation
- Vendor coordination
- Change management

## 16. Validation After Fix

Confirm that the fix or mitigation was validated.

- [ ] Technical validation completed
- [ ] Business validation completed
- [ ] Logs reviewed
- [ ] Monitoring reviewed
- [ ] Integration flow validated
- [ ] Data accuracy confirmed, if applicable
- [ ] Users confirmed recovery, if applicable
- [ ] No recurring errors observed
- [ ] Support team informed

Validation evidence:

```text
Validation performed:
Validation owner:
Validation date:
Evidence:
```

## 17. Remediation Tracking

Track all remediation items until closure.

| ID | Remediation Item | Type | Owner | Due Date | Status | Evidence |
|---|---|---|---|---|---|---|
| REM-001 |  | Corrective / Preventive |  |  | Open |  |
| REM-002 |  | Corrective / Preventive |  |  | Open |  |

## 18. Lessons Learned

Capture lessons that can improve future delivery and operations.

Questions:

- What went well?
- What slowed the response?
- What could have detected the incident earlier?
- What control failed?
- What documentation was missing?
- What should be automated?
- What should be added to release, cutover, or hypercare processes?

## 19. Closure Criteria

The incident RCA can be closed when:

- [ ] Incident impact is documented.
- [ ] Timeline is completed.
- [ ] Root cause is identified.
- [ ] Corrective actions are defined.
- [ ] Preventive actions are defined.
- [ ] Owners and due dates are assigned.
- [ ] Business validation is completed.
- [ ] Communication summary is documented.
- [ ] Remediation tracking is active.
- [ ] Closure is approved by accountable owner.

## 20. Final Approval

| Name | Role | Decision | Date | Comments |
|---|---|---|---|---|
|  | Incident Owner | Approved / Not Approved |  |  |
|  | Technical Owner | Approved / Not Approved |  |  |
|  | Business Owner | Approved / Not Approved |  |  |
|  | Support Lead | Approved / Not Approved |  |  |

## Privacy Notice

This template should not include private customer data, passwords, credentials, access tokens, API keys, confidential financial information, network details, security vulnerabilities, or sensitive personal information.

Use sanitized or fictional data when sharing incident documentation publicly.
