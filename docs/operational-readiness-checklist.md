# Operational Readiness Checklist

## Purpose

This checklist helps teams confirm whether a solution, system, application, automation, integration, or business process change is ready to transition from project delivery into operational support.

Operational readiness ensures that the solution can be supported, monitored, maintained, escalated, documented, and handed over to Business As Usual, also known as BAU.

The goal is to avoid a common delivery problem: going live successfully but leaving support teams, users, and operations without enough ownership, documentation, visibility, or process clarity.

## When to Use This Checklist

Use this checklist before or after:

- Production release
- Go-live
- ERP migration
- Cloud migration
- System implementation
- Integration deployment
- Automation rollout
- Business process transition
- Hypercare exit
- BAU support handover
- Service transition
- Post-implementation stabilization

## Operational Readiness Overview

```text
Solution delivered
      ↓
Support model defined
      ↓
Monitoring and alerts prepared
      ↓
Known issues documented
      ↓
Access and roles validated
      ↓
Runbooks prepared
      ↓
Training completed
      ↓
SLA / KPI impact reviewed
      ↓
BAU handover completed
```

## 1. Operational Scope

Confirm what is included in the operational readiness review.

- [ ] System, application, or process is identified.
- [ ] Business area is documented.
- [ ] Support scope is defined.
- [ ] In-scope modules, components, or processes are listed.
- [ ] Out-of-scope items are documented.
- [ ] Critical business processes are identified.
- [ ] Operational dependencies are listed.
- [ ] Support ownership is confirmed.
- [ ] Business ownership is confirmed.
- [ ] Technical ownership is confirmed.
- [ ] Operational risks are documented.

Example scope:

```text
System or application:
Business area:
Release or implementation:
Go-live date:
Hypercare period:
Operational support start date:
In-scope processes:
Out-of-scope items:
```

## 2. Support Model

Confirm how the solution will be supported after go-live or hypercare.

- [ ] Support model is documented.
- [ ] Support team is identified.
- [ ] Support levels are defined.
- [ ] First-level support responsibilities are clear.
- [ ] Second-level support responsibilities are clear.
- [ ] Third-level support or engineering responsibilities are clear.
- [ ] Vendor support responsibilities are documented, if applicable.
- [ ] Business support responsibilities are documented.
- [ ] Support hours are defined.
- [ ] Support channels are documented.
- [ ] Ticket intake process is defined.
- [ ] Support ownership is formally accepted.

Recommended support model table:

| Support Level | Responsibility | Owner | Channel | Hours |
|---|---|---|---|---|
| Level 1 | Initial intake and basic triage |  |  |  |
| Level 2 | Application or functional support |  |  |  |
| Level 3 | Technical deep-dive or engineering support |  |  |  |
| Vendor | Third-party support, if applicable |  |  |  |
| Business | Process validation and business decisions |  |  |  |

Key questions:

- Who receives the first support request?
- Who triages incidents?
- Who owns functional issues?
- Who owns technical issues?
- Who approves business workarounds?
- Who supports after business hours?
- What happens when the issue requires escalation?

## 3. Monitoring and Alerting

Confirm that the solution can be monitored effectively.

- [ ] Monitoring scope is documented.
- [ ] Critical components are monitored.
- [ ] Application availability is monitored.
- [ ] Infrastructure or platform health is monitored.
- [ ] Integration health is monitored.
- [ ] Batch jobs or scheduled processes are monitored.
- [ ] Error logs are available.
- [ ] Alerts are defined.
- [ ] Alert recipients are assigned.
- [ ] Alert severity is documented.
- [ ] Dashboards are available, if applicable.
- [ ] Monitoring ownership is defined.
- [ ] Support team knows how to interpret alerts.

Monitoring examples:

| Monitoring Area | Example |
|---|---|
| Availability | Application is reachable |
| Performance | Response time is within expected threshold |
| Integrations | Files, APIs, or messages are processing |
| Batch jobs | Scheduled process completed successfully |
| Errors | Critical exceptions are logged and reviewed |
| Data quality | Expected records, totals, or reconciliation checks pass |
| Security | Unusual access or failed authentication is visible |

Alerting questions:

- Which alerts require immediate action?
- Which alerts are informational?
- Who receives alerts?
- What is the expected response time?
- How are false positives handled?
- What runbook should be followed for each alert?

## 4. Known Issues

Known issues should be documented before operational handover.

- [ ] Known issues are listed.
- [ ] Business impact is documented.
- [ ] Workarounds are documented.
- [ ] Owners are assigned.
- [ ] Target resolution dates are defined.
- [ ] Accepted risks are documented.
- [ ] Business owner has accepted known limitations.
- [ ] Support team understands known issues.
- [ ] Known issues are transferred to BAU tracking.

Recommended known issues table:

| ID | Known Issue | Business Impact | Workaround | Owner | Target Date | Accepted By |
|---|---|---|---|---|---|---|
| KI-001 |  |  |  |  |  |  |
| KI-002 |  |  |  |  |  |  |

A known issue is acceptable only when:

- Impact is understood.
- Owner is assigned.
- Workaround exists or risk is accepted.
- Target resolution is documented.
- Business stakeholder accepts the limitation.
- Support team knows how to handle it.

## 5. Access and Security Readiness

Confirm that users and support teams have the access required to operate and support the solution.

- [ ] User roles are documented.
- [ ] Support roles are documented.
- [ ] Administrative access is controlled.
- [ ] Access request process is defined.
- [ ] Access approval process is defined.
- [ ] Role changes are documented.
- [ ] Privileged access is reviewed.
- [ ] Segregation of duties is reviewed, if applicable.
- [ ] Support team has required access.
- [ ] Business users have required access.
- [ ] Access issues are tracked.
- [ ] Security owner has reviewed access model.

Access readiness table:

| Role | Access Needed | Owner | Approved | Validated |
|---|---|---|---|---|
| Business User |  |  | Yes / No | Yes / No |
| Support Analyst |  |  | Yes / No | Yes / No |
| Application Owner |  |  | Yes / No | Yes / No |
| Technical Support |  |  | Yes / No | Yes / No |
| Vendor Support |  |  | Yes / No | Yes / No |

Key questions:

- Can users access what they need?
- Can support teams troubleshoot issues?
- Is privileged access controlled?
- Is there a process to request or revoke access?
- Are access risks documented?

## 6. Runbooks and Support Procedures

Runbooks help support teams respond consistently.

- [ ] Operational runbooks are prepared.
- [ ] Incident handling procedure is documented.
- [ ] Restart procedure is documented, if applicable.
- [ ] Reprocessing procedure is documented, if applicable.
- [ ] Data correction process is documented, if applicable.
- [ ] Backup and restore process is documented, if applicable.
- [ ] Monitoring response procedure is documented.
- [ ] Escalation process is documented.
- [ ] Known issue workarounds are documented.
- [ ] Support team has reviewed the runbooks.
- [ ] Runbooks are stored in an accessible location.

Recommended runbooks:

| Runbook | Purpose |
|---|---|
| Incident response runbook | Steps to triage and resolve incidents |
| Integration reprocessing runbook | Steps to correct and reprocess failed transactions |
| Batch job runbook | Steps to validate and restart scheduled jobs |
| Access support runbook | Steps to resolve access-related issues |
| Monitoring alert runbook | Steps to respond to alerts |
| Data reconciliation runbook | Steps to validate and reconcile data |
| Rollback runbook | Steps to restore previous state when needed |

## 7. Escalation Path

Confirm that escalation is clear before operational transition.

- [ ] Escalation matrix is documented.
- [ ] Severity levels are defined.
- [ ] Business escalation contacts are listed.
- [ ] Technical escalation contacts are listed.
- [ ] Vendor escalation contacts are listed, if applicable.
- [ ] Executive escalation path is documented.
- [ ] Escalation response expectations are defined.
- [ ] Support team understands when to escalate.
- [ ] Business team understands how issues will be escalated.

Severity example:

| Severity | Description | Escalation |
|---|---|---|
| Critical | Business-critical process is blocked | Immediate escalation |
| High | Major business function degraded | Same business day |
| Medium | Partial impact or workaround available | Regular support cadence |
| Low | Minor issue, question, or enhancement | Normal support queue |

Escalation questions:

- Who owns critical incidents?
- Who communicates business impact?
- Who decides on workaround acceptance?
- Who contacts the vendor?
- Who informs leadership?
- What is the expected response time?

## 8. Training and Knowledge Transfer

Confirm that users and support teams are prepared.

- [ ] Business users received training.
- [ ] Support team received knowledge transfer.
- [ ] Training materials are available.
- [ ] Frequently asked questions are documented.
- [ ] Support team understands common issues.
- [ ] Business users understand how to request support.
- [ ] Process changes are communicated.
- [ ] New roles or responsibilities are explained.
- [ ] Training gaps are identified.
- [ ] Adoption risks are documented.

Training areas:

| Audience | Training Focus |
|---|---|
| Business users | How to use the solution or process |
| Support team | How to triage and resolve issues |
| Technical team | How to monitor and maintain the solution |
| Business owners | How to validate outcomes and make decisions |
| Operations team | How to operate the solution in BAU |

Knowledge transfer should include:

- Process overview
- System overview
- Known issues
- Common support requests
- Escalation path
- Runbooks
- Monitoring
- Access model
- Reporting
- Business validation steps

## 9. Documentation Readiness

Confirm that required documentation is available and accessible.

- [ ] Solution overview is documented.
- [ ] Architecture notes are available.
- [ ] Support model is documented.
- [ ] Runbooks are available.
- [ ] Monitoring documentation is available.
- [ ] Access model is documented.
- [ ] Known issues are documented.
- [ ] Integration documentation is available, if applicable.
- [ ] Data flow documentation is available, if applicable.
- [ ] User guides are available, if applicable.
- [ ] Training material is available.
- [ ] BAU handover package is prepared.

Recommended documentation package:

| Document | Owner | Status |
|---|---|---|
| Solution overview |  | Pending / Complete |
| Support model |  | Pending / Complete |
| Architecture notes |  | Pending / Complete |
| Runbooks |  | Pending / Complete |
| Monitoring notes |  | Pending / Complete |
| Known issues log |  | Pending / Complete |
| User guide |  | Pending / Complete |
| BAU handover document |  | Pending / Complete |

## 10. SLA and KPI Impact

Review whether the solution affects service levels or operational metrics.

- [ ] SLA impact is assessed.
- [ ] KPI impact is assessed.
- [ ] Operational metrics are defined.
- [ ] Reporting owner is assigned.
- [ ] Support response targets are reviewed.
- [ ] Resolution targets are reviewed.
- [ ] Availability expectations are documented.
- [ ] Performance expectations are documented.
- [ ] Business process metrics are documented.
- [ ] Baseline metrics are known, if applicable.
- [ ] Measurement frequency is defined.

Examples of operational KPIs:

| KPI | Description |
|---|---|
| Availability | Percentage of time the service is available |
| Incident volume | Number of incidents reported |
| Mean time to resolution | Average time to resolve incidents |
| Failed transactions | Number of failed integrations or processes |
| Reprocessing volume | Number of items requiring reprocessing |
| User access issues | Number of access-related incidents |
| Business process completion | Success rate of critical business flows |
| Report refresh success | Reports updated within expected window |

Key questions:

- Does this solution affect existing SLAs?
- Are new KPIs required?
- Who reports operational performance?
- How often are KPIs reviewed?
- What threshold requires escalation?

## 11. Business Validation

Business validation confirms that the solution works in real operational conditions.

- [ ] Critical business flows are validated.
- [ ] Business owner confirms readiness.
- [ ] Users confirm they can execute required steps.
- [ ] Reports or outputs are trusted.
- [ ] Known limitations are accepted.
- [ ] Workarounds are documented.
- [ ] Open risks are understood.
- [ ] Business sign-off is captured.

Business validation table:

| Business Process | Owner | Validation Status | Open Issues | Sign-Off |
|---|---|---|---:|---|
|  |  | Pending / Passed / Failed |  | Yes / No |
|  |  | Pending / Passed / Failed |  | Yes / No |

## 12. BAU Handover

BAU handover confirms that the solution is ready to move into normal support operations.

- [ ] BAU owner is identified.
- [ ] Support team accepts ownership.
- [ ] Business owner confirms operational readiness.
- [ ] Final issue log is shared.
- [ ] Known issues are transferred.
- [ ] Open actions are assigned.
- [ ] Runbooks are handed over.
- [ ] Monitoring documentation is shared.
- [ ] Access support process is confirmed.
- [ ] Escalation path is confirmed.
- [ ] Training material is shared.
- [ ] SLA or KPI impact is documented.
- [ ] Handover approval is captured.

BAU handover package:

- Support model
- Known issues log
- Open actions
- Runbooks
- Monitoring notes
- Access model
- Escalation matrix
- Training materials
- User guides
- Operational KPIs
- Lessons learned
- Business acceptance summary

## Operational Readiness Decision

Use this section to summarize readiness.

```text
Readiness decision:
Ready for BAU / Ready with conditions / Not ready

Key conditions:
Decision owner:
Decision date:
Next review:
```

## Operational Readiness Exit Criteria

The solution can be considered operationally ready when:

- [ ] Support model is documented and accepted.
- [ ] Monitoring and alerts are ready.
- [ ] Known issues are documented and owned.
- [ ] Access model is validated.
- [ ] Runbooks are available.
- [ ] Escalation path is confirmed.
- [ ] Support team received knowledge transfer.
- [ ] Business users received required training.
- [ ] Required documentation is available.
- [ ] SLA or KPI impact is understood.
- [ ] Business validation is completed.
- [ ] BAU handover is approved.

## Common Operational Readiness Risks

Common risks include:

- Support team is not involved early enough.
- Runbooks are missing or incomplete.
- Monitoring is not configured.
- Known issues are not transferred.
- Business users do not know how to request support.
- Access process is unclear.
- SLA or KPI impact is not understood.
- Escalation path is incomplete.
- Training is rushed.
- Documentation is stored in the wrong place.
- BAU ownership is assumed but not confirmed.

## Recommended Artifacts

Useful artifacts for operational readiness include:

- Operational readiness checklist
- Support model
- Monitoring and alerting guide
- Known issues log
- Access matrix
- Runbooks
- Escalation matrix
- Training material
- User guide
- SLA or KPI impact summary
- BAU handover document
- Lessons learned summary

## Final Principle

Operational readiness is not an afterthought.

A solution is not truly delivered until it can be supported, monitored, maintained, escalated, documented, and owned by the teams responsible for keeping it running.
