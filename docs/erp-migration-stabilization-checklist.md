# ERP Migration Stabilization Checklist

## Purpose

This checklist helps teams stabilize an ERP migration after go-live.

It is designed for complex ERP transitions where business processes, master data, transactional data, integrations, reports, users, and operational support must be validated after moving from a legacy ERP to a new ERP platform.

The focus is not only technical stabilization. The goal is to confirm that business operations can continue with confidence after migration.

## When to Use This Checklist

Use this checklist after:

- ERP go-live
- Legacy ERP to new ERP migration
- JD Edwards to SAP migration
- SAP implementation or rollout
- ERP module migration
- Finance or supply chain system migration
- Data migration and cutover execution
- Integration-heavy ERP deployment
- Post-go-live hypercare
- Business process stabilization
- Transition to Business As Usual, also known as BAU

## Stabilization Overview

```text
Go-live completed
      ↓
Hypercare activated
      ↓
Critical process validation
      ↓
Data reconciliation
      ↓
Integration monitoring
      ↓
Issue triage and resolution
      ↓
Business acceptance
      ↓
BAU handover
```

## 1. Stabilization Scope

Confirm what is included in the stabilization period.

- [ ] ERP system or platform is identified.
- [ ] Migration scope is documented.
- [ ] Business areas included are confirmed.
- [ ] In-scope modules are listed.
- [ ] Out-of-scope processes are documented.
- [ ] Critical business processes are identified.
- [ ] Support period is defined.
- [ ] Hypercare team is assigned.
- [ ] BAU support team is identified.
- [ ] Business owners are confirmed.
- [ ] Technical owners are confirmed.
- [ ] Integration owners are confirmed.

Example scope:

```text
Legacy ERP:
Target ERP:
Go-live date:
Hypercare start:
Hypercare end:
Business areas:
In-scope modules:
Out-of-scope items:
```

## 2. ERP Business Process Coverage

Confirm that core business processes are included in stabilization review.

Common ERP process areas:

| Process Area | Example Validation Focus |
|---|---|
| Procurement | Purchase orders, goods receipts, vendor master, approvals |
| Inventory | Stock balances, movements, adjustments, valuation |
| Warehouse | Receiving, picking, packing, transfers, cycle counts |
| Production | Work orders, production confirmations, material consumption |
| Costing | Standard cost, actual cost, cost rollups, variances |
| Sales | Customer orders, pricing, availability, delivery creation |
| Billing | Invoice generation, tax calculation, invoice posting |
| Collections | Open items, customer balances, payment application |
| Finance | GL postings, AP, AR, cost centers, profit centers |
| Commissions | Commission rules, sales crediting, payout calculations |
| Reporting | Operational reports, financial reports, reconciliation reports |

## 3. Business Criticality

Classify each process by business criticality.

- [ ] Critical processes are identified.
- [ ] High-impact processes are documented.
- [ ] Manual workaround is defined where needed.
- [ ] Business process owner is assigned.
- [ ] Stabilization priority is agreed.
- [ ] Business impact of failures is documented.

Suggested criticality levels:

| Level | Description |
|---|---|
| Critical | Business operation is blocked if unavailable |
| High | Major process is degraded or delayed |
| Medium | Noticeable impact, but workaround may exist |
| Low | Limited operational impact |

Recommended table:

| Process | Criticality | Business Owner | Workaround Available | Notes |
|---|---|---|---|---|
| Procurement | Critical / High / Medium / Low |  | Yes / No |  |
| Inventory | Critical / High / Medium / Low |  | Yes / No |  |
| Warehouse | Critical / High / Medium / Low |  | Yes / No |  |
| Production | Critical / High / Medium / Low |  | Yes / No |  |
| Costing | Critical / High / Medium / Low |  | Yes / No |  |
| Sales | Critical / High / Medium / Low |  | Yes / No |  |
| Billing | Critical / High / Medium / Low |  | Yes / No |  |
| Collections | Critical / High / Medium / Low |  | Yes / No |  |

## 4. Master Data Stabilization

Master data quality is one of the most important stabilization areas after an ERP migration.

- [ ] Customer master data is validated.
- [ ] Vendor master data is validated.
- [ ] Material or item master data is validated.
- [ ] Pricing master data is validated.
- [ ] Tax configuration is reviewed.
- [ ] Payment terms are validated.
- [ ] Units of measure are validated.
- [ ] Plant, warehouse, and storage locations are reviewed.
- [ ] Cost centers and profit centers are validated.
- [ ] Chart of accounts mapping is reviewed.
- [ ] Master data ownership is assigned.
- [ ] Master data correction process is defined.

Recommended validation table:

| Master Data Object | Owner | Validation Status | Issues Found | Resolution Owner |
|---|---|---|---|---|
| Customer master |  | Pending / Passed / Failed |  |  |
| Vendor master |  | Pending / Passed / Failed |  |  |
| Material master |  | Pending / Passed / Failed |  |  |
| Pricing records |  | Pending / Passed / Failed |  |  |
| Tax setup |  | Pending / Passed / Failed |  |  |
| Cost centers |  | Pending / Passed / Failed |  |  |

## 5. Transactional Data Validation

Validate that migrated transactional data is complete, accurate, and usable.

- [ ] Open purchase orders are validated.
- [ ] Open sales orders are validated.
- [ ] Inventory balances are reconciled.
- [ ] Open invoices are validated.
- [ ] Open AR items are validated.
- [ ] Open AP items are validated.
- [ ] Production orders are validated.
- [ ] Warehouse tasks or movements are reviewed.
- [ ] Historical balances required for operations are available.
- [ ] Transaction cutover timing is documented.
- [ ] Data reconciliation evidence is captured.

Recommended reconciliation areas:

| Data Area | Source Count | Target Count | Difference | Status | Owner |
|---|---:|---:|---:|---|---|
| Open purchase orders |  |  |  | Pending / Passed / Failed |  |
| Open sales orders |  |  |  | Pending / Passed / Failed |  |
| Inventory balances |  |  |  | Pending / Passed / Failed |  |
| Open invoices |  |  |  | Pending / Passed / Failed |  |
| Customer balances |  |  |  | Pending / Passed / Failed |  |
| Vendor balances |  |  |  | Pending / Passed / Failed |  |

## 6. Procurement Stabilization

Validate procurement-related processes after go-live.

- [ ] Purchase requisitions can be created.
- [ ] Purchase orders can be created.
- [ ] Approval workflow works as expected.
- [ ] Goods receipts can be posted.
- [ ] Vendor data is correct.
- [ ] Pricing and purchasing conditions are valid.
- [ ] Open purchase orders migrated correctly.
- [ ] Three-way match process works, if applicable.
- [ ] Procurement reports are available.
- [ ] Procurement users have correct access.
- [ ] Procurement issues are tracked.

Key questions:

- Can users create and approve purchase orders?
- Are vendor records correct?
- Can goods receipts be posted?
- Are migrated open purchase orders usable?
- Are approval workflows working?
- Are integration points working?

## 7. Inventory and Warehouse Stabilization

Validate inventory and warehouse operations.

- [ ] Inventory balances are reconciled.
- [ ] Stock movements can be posted.
- [ ] Goods receipts work correctly.
- [ ] Goods issues work correctly.
- [ ] Warehouse locations are correct.
- [ ] Transfer processes are validated.
- [ ] Cycle count process is available.
- [ ] Inventory valuation is reviewed.
- [ ] Warehouse users have correct access.
- [ ] Inventory reports match expected balances.
- [ ] Inventory discrepancies are tracked.

Key questions:

- Do inventory balances match expected values?
- Can users complete receiving and issuing processes?
- Are storage locations and warehouses correctly configured?
- Are material movements posting correctly?
- Are inventory reports trusted by the business?

## 8. Production Stabilization

Validate production-related processes.

- [ ] Production orders can be created.
- [ ] Production orders can be released.
- [ ] Material consumption can be posted.
- [ ] Production confirmations can be completed.
- [ ] Finished goods receipt can be posted.
- [ ] Bill of materials are validated.
- [ ] Routings or recipes are validated.
- [ ] Work centers are validated.
- [ ] Production variances are reviewed.
- [ ] Production users have correct access.
- [ ] Production reports are available.

Key questions:

- Can production execute critical shop floor processes?
- Are BOMs and routings correct?
- Are material consumption postings accurate?
- Are production confirmations working?
- Are production cost impacts understood?

## 9. Costing Stabilization

Validate costing and valuation after migration.

- [ ] Standard costs are loaded or calculated.
- [ ] Material valuation is reviewed.
- [ ] Costing variants or rules are validated.
- [ ] Cost centers are mapped correctly.
- [ ] Profit centers are mapped correctly.
- [ ] Production variances are reviewed.
- [ ] Inventory valuation is reviewed.
- [ ] Cost reports are validated.
- [ ] Finance and controlling teams confirm results.
- [ ] Costing issues are tracked.

Key questions:

- Are costs correctly reflected in the new ERP?
- Are cost centers and profit centers correct?
- Are inventory values aligned?
- Are production variances reasonable?
- Are finance users comfortable with the outputs?

## 10. Sales Stabilization

Validate sales processes after go-live.

- [ ] Customer orders can be created.
- [ ] Customer master data is correct.
- [ ] Pricing is correct.
- [ ] Discounts and conditions are validated.
- [ ] Availability check works, if applicable.
- [ ] Delivery creation works.
- [ ] Sales order status is correct.
- [ ] Open sales orders migrated correctly.
- [ ] Sales users have correct access.
- [ ] Sales reports are available.

Key questions:

- Can users create customer orders?
- Are prices and conditions correct?
- Are customer records accurate?
- Can deliveries be created?
- Are migrated orders usable?

## 11. Billing and Collections Stabilization

Validate billing, accounts receivable, and collections processes.

- [ ] Billing documents can be created.
- [ ] Tax calculation is validated.
- [ ] Invoice output is correct.
- [ ] Invoice posting works.
- [ ] Customer open items are validated.
- [ ] Payment application process works.
- [ ] Credit and collections process is available.
- [ ] Customer balances are reconciled.
- [ ] Billing users have correct access.
- [ ] AR and collections reports are validated.
- [ ] Billing issues are tracked.

Key questions:

- Can invoices be generated and posted?
- Are taxes and totals correct?
- Are customer balances accurate?
- Can payments be applied?
- Can collections users operate normally?

## 12. Commissions Stabilization

If commissions are part of the migration scope, validate commission flows.

- [ ] Commission rules are documented.
- [ ] Sales crediting logic is validated.
- [ ] Commission-relevant transactions are identified.
- [ ] Commission calculations are tested.
- [ ] Exception scenarios are reviewed.
- [ ] Payout reports are validated.
- [ ] Commission owners confirm results.
- [ ] Open commission issues are tracked.

Key questions:

- Are eligible sales transactions captured?
- Are commission rates or rules correct?
- Are exceptions handled correctly?
- Are reports trusted by business owners?
- Is sign-off required before payout?

## 13. Integration Stabilization

Validate ERP integrations after migration.

- [ ] Customer integrations are monitored.
- [ ] Supplier integrations are monitored.
- [ ] EDI interfaces are validated.
- [ ] Middleware queues are reviewed.
- [ ] API integrations are checked.
- [ ] File-based integrations are validated.
- [ ] Failed messages are tracked.
- [ ] Reprocessing process is defined.
- [ ] Integration owners are assigned.
- [ ] Business impact of failed integrations is understood.

Recommended integration table:

| Integration | Direction | Owner | Status | Failed Transactions | Action |
|---|---|---|---|---:|---|
|  | Inbound / Outbound |  | Healthy / Degraded / Failed |  |  |

## 14. Reporting Stabilization

Validate operational and executive reporting.

- [ ] Critical operational reports are available.
- [ ] Finance reports are validated.
- [ ] Inventory reports are validated.
- [ ] Sales reports are validated.
- [ ] Procurement reports are validated.
- [ ] Production reports are validated.
- [ ] Report totals are reconciled with expected values.
- [ ] Report access is confirmed.
- [ ] Report refresh schedules are working.
- [ ] Business owners trust report outputs.

Key questions:

- Are reports available when business users need them?
- Are totals accurate?
- Are filters, dates, and business dimensions correct?
- Are users able to access the reports?
- Are reporting delays impacting decisions?

## 15. User Access Stabilization

Validate that users can operate in the new ERP.

- [ ] Critical users can log in.
- [ ] Business roles are assigned correctly.
- [ ] Segregation of duties is reviewed, if applicable.
- [ ] Approval roles are working.
- [ ] Emergency access process is available.
- [ ] Access issues are tracked.
- [ ] Users know how to request support.
- [ ] User training gaps are identified.
- [ ] Security owner is involved in access issues.

Common access issues:

- Missing role
- Incorrect authorization
- User assigned to wrong organization
- Approval workflow not routing correctly
- Report access missing
- Transaction access blocked

## 16. Incident and Defect Triage

During stabilization, issues should be triaged consistently.

- [ ] Issue intake process is defined.
- [ ] Severity model is agreed.
- [ ] Business impact is captured.
- [ ] Owners are assigned.
- [ ] Daily triage is scheduled.
- [ ] Escalation path is documented.
- [ ] Critical issues are prioritized.
- [ ] Workarounds are documented.
- [ ] Known issues are tracked.
- [ ] Resolution evidence is captured.

Suggested severity model:

| Severity | Description | Response |
|---|---|---|
| Critical | Business-critical process blocked | Immediate escalation |
| High | Major process degraded | Same-day resolution focus |
| Medium | Partial impact or workaround available | Track in daily triage |
| Low | Minor issue or question | Normal support queue |

## 17. Daily Stabilization Checkpoints

Daily checkpoints help maintain visibility during hypercare.

Recommended agenda:

- Review critical and high issues.
- Review business process status.
- Review integration failures.
- Review data reconciliation concerns.
- Review access issues.
- Review reporting issues.
- Confirm owners and due dates.
- Identify executive decisions needed.
- Confirm communication updates.
- Review exit criteria progress.

Executive update format:

```text
Overall status:
Critical issues:
High priority issues:
Business impact:
Actions in progress:
Decisions required:
Next update:
```

## 18. Business Validation

Business owners should validate real operational readiness.

- [ ] Procurement owner confirms readiness.
- [ ] Inventory owner confirms readiness.
- [ ] Warehouse owner confirms readiness.
- [ ] Production owner confirms readiness.
- [ ] Costing or finance owner confirms readiness.
- [ ] Sales owner confirms readiness.
- [ ] Billing owner confirms readiness.
- [ ] Collections owner confirms readiness.
- [ ] Commission owner confirms readiness, if applicable.
- [ ] Reporting owner confirms readiness.
- [ ] Known issues are accepted or assigned.

Business validation table:

| Business Area | Owner | Status | Open Issues | Sign-Off |
|---|---|---|---:|---|
| Procurement |  | Pending / Accepted / Blocked |  | Yes / No |
| Inventory |  | Pending / Accepted / Blocked |  | Yes / No |
| Warehouse |  | Pending / Accepted / Blocked |  | Yes / No |
| Production |  | Pending / Accepted / Blocked |  | Yes / No |
| Costing |  | Pending / Accepted / Blocked |  | Yes / No |
| Sales |  | Pending / Accepted / Blocked |  | Yes / No |
| Billing |  | Pending / Accepted / Blocked |  | Yes / No |
| Collections |  | Pending / Accepted / Blocked |  | Yes / No |

## 19. Hypercare Exit Criteria

ERP stabilization should not end only because the calendar says so.

Recommended exit criteria:

- [ ] No critical business process remains blocked.
- [ ] High severity issues are resolved or formally accepted.
- [ ] Core business processes are validated.
- [ ] Data reconciliation is completed or exceptions are accepted.
- [ ] Critical integrations are stable.
- [ ] Users can execute required transactions.
- [ ] Reporting outputs are trusted by business owners.
- [ ] Known issues are documented.
- [ ] Workarounds are documented.
- [ ] BAU support team is ready.
- [ ] Business owners approve transition.
- [ ] Hypercare closure communication is sent.

## 20. BAU Handover

BAU means Business As Usual. It represents the normal support and operating model after migration and stabilization.

BAU handover should include:

- [ ] Final issue log
- [ ] Known issues list
- [ ] Open actions
- [ ] Support ownership matrix
- [ ] Escalation path
- [ ] Process documentation
- [ ] Integration monitoring notes
- [ ] Reprocessing procedures
- [ ] Access support process
- [ ] Reporting support notes
- [ ] Data reconciliation summary
- [ ] Lessons learned
- [ ] Business acceptance summary

Recommended handover table:

| Handover Item | Owner | Status | Notes |
|---|---|---|---|
| Final issue log |  | Pending / Completed |  |
| Known issues |  | Pending / Completed |  |
| Support model |  | Pending / Completed |  |
| Escalation path |  | Pending / Completed |  |
| Runbooks |  | Pending / Completed |  |
| Integration monitoring |  | Pending / Completed |  |
| Business acceptance |  | Pending / Completed |  |

## 21. Common Stabilization Risks

Common risks after ERP migration include:

- Data reconciliation issues
- Missing master data
- Incorrect roles or authorizations
- Integration failures
- Reporting discrepancies
- Incomplete training
- Business users reverting to offline workarounds
- Manual corrections without audit trail
- Unclear issue ownership
- Slow defect triage
- Incomplete BAU handover
- Hypercare closing too early
- Commission, billing, or costing exceptions discovered late

## 22. Recommended Artifacts

Useful artifacts for ERP migration stabilization include:

- Hypercare tracker
- Issue log
- Known issues log
- Data reconciliation report
- Integration monitoring report
- Business process validation checklist
- Access issue tracker
- Report validation list
- Daily status update
- Executive summary
- BAU handover checklist
- Lessons learned document

## Stabilization Decision

Use this section to summarize readiness to exit hypercare.

```text
Stabilization decision:
Ready for BAU handover / Ready with conditions / Not ready

Key conditions:
Decision owner:
Decision date:
Next review:
```

## Final Principle

An ERP migration is not complete at go-live.

It is complete when business operations are stable, data is trusted, integrations are working, users can execute critical processes, and support ownership has moved cleanly to BAU.
