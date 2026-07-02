# DORA Audit Test Procedures

A full audit programme to check DORA compliance, whether by internal audit or an outside reviewer. It covers **all 48 controls**, so nothing is missed by accident. For each control there is a test step, the evidence to look at, and a clear **pass line** (what "Effective" looks like). Record results in the [findings template](findings-template.md) and size samples using the [sampling and evidence guidance](sampling-and-evidence.md).

**Read first:** [Glossary](../glossary.md).

---

## How to use this programme

1. Scope the engagement (see the checklist below).
2. For every in-scope control, do the test and compare what you find to the **pass line**.
3. Give each control a rating: **Effective**, **Partially effective**, or **Not effective**.
4. Turn every "Partially" or "Not effective" into a finding.
5. Roll the ratings up into an overall opinion using Section "Reaching an opinion".

Where a control is not applicable (for example TLPT for a firm not named), write "N/A" and the reason. Do not leave it blank.

## Engagement scoping checklist

- Confirm the firm's DORA scope, type, and proportionality tier.
- Confirm whether the simplified framework (Art. 16) applies.
- Confirm whether the firm is named for TLPT (Art. 26).
- Identify critical or important functions and the systems and third parties behind them.
- Agree the audit period, the populations (incidents, tests, contracts), and materiality.
- Confirm which RTS and ITS were in force during the period.

---

## Pillar 0 - Governance

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-GOV-01 | Inspect board minutes for approval and last annual review of the framework. | Minutes, framework doc | Approval and a review within the period, both dated. |
| A-GOV-02 | Inspect the RACI and org chart; interview the ICT risk owner. | RACI, interview notes | Every key activity has one accountable owner who knows the role. |
| A-GOV-03 | Sample board reporting packs across the period. | Board packs, minutes | Regular reporting with recorded challenge and decisions. |
| A-GOV-04 | Inspect board training records. | Training log | Board members completed role-suitable training. |
| A-GOV-05 | Inspect budget approval showing a resilience line. | Budget papers | Budget set and reviewed at least yearly. |
| A-GOV-06 | Inspect the proportionality assessment. | Assessment doc | Written, reasoned, states full or simplified, and current. |
| A-GOV-07 | Inspect the internal audit plan and three-lines model. | Audit plan, ToR | ICT risk covered independently on a plan. |

## Pillar 1 - ICT Risk Management

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-RM-01 | Inspect the resilience strategy and its approval. | Strategy doc | Board-approved, with risk appetite and objectives. |
| A-RM-02 | Reconcile the inventory to a sample of live systems and third-party services; test for shadow IT. | Inventory, system lists | Inventory complete, current, classified, linked to functions and third parties. |
| A-RM-03 | Inspect the risk method and register; check reassessment on a recent major change. | Method, register | Repeatable method, current register, reassessed on change. |
| A-RM-04 | Test a sample of access, MFA, patching, change, and encryption controls. | Control logs, configs | Controls operate as the policy says. |
| A-RM-05 | Inspect logging and alerting on a sample of critical systems. | Alert configs, tickets | Logging on, thresholds set, alerts acted on. |
| A-RM-06 | Inspect RTO and RPO and the latest continuity or recovery test for critical functions. | Plans, test report | RTO and RPO defined and a test proved recovery within them. |
| A-RM-07 | Inspect backup policy; inspect or re-perform a restore test; check segregation. | Policy, restore report | Backups segregated and a restore was verified in the period. |
| A-RM-08 | Sample post-incident reviews; trace actions to closure; check threat-intel use. | Reviews, action log | Root cause found, actions closed, intel used. |
| A-RM-09 | Inspect training records for staff and board. | Training log | Role-based training completed and recorded. |
| A-RM-10 | Inspect evidence the framework was reviewed in the period. | Review minutes | Reviewed at least yearly and after any major incident. |

## Pillar 2 - Incident Management and Reporting

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-INC-01 | Inspect the incident process end to end. | Process doc | Covers detection, logging, severity, escalation, closure. |
| A-INC-02 | Re-perform classification on a sample of incidents using the RTS criteria. | Classification aid, incident records | Classifications consistent and correct against the RTS. |
| A-INC-03 | Inspect the on-call and escalation matrix and any exercise. | Matrix, exercise report | Defined and tested. |
| A-INC-04 | For every major incident in the period, trace initial, intermediate, and final reports to the deadlines. | Reports, timestamps | All reports made inside the ITS deadlines. Test the whole population, not a sample. |
| A-INC-05 | Compare submitted reports to the ITS template fields. | Submitted forms | Complete and accurate. |
| A-INC-06 | Inspect client notices where clients were affected. | Client notices | Sent without undue delay, with protective advice. |
| A-INC-07 | Inspect the process for assessing cyber threats for voluntary notification. | Triage records | A working process exists. |
| A-INC-08 | Sample post-incident reviews; trace to closure. | Reviews | RCA done and actions closed. |
| A-INC-09 | Check payment-related incidents are captured under the same regime. | Incident register | Payment incidents included where applicable. |

## Pillar 3 - Resilience Testing

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-TST-01 | Inspect the testing programme and its review. | Programme doc | Documented, risk-based, reviewed. |
| A-TST-02 | Reconcile the population of critical systems to tests done in the period. | Calendar, test reports | Every critical system tested at least yearly. Test the whole population. |
| A-TST-03 | Inspect the mix of test methods against system risk. | Method catalogue | Suitable mix for the risk. |
| A-TST-04 | Inspect tester qualifications, independence, and insurance. | Tester records | Independent, qualified, insured where external. |
| A-TST-05 | Sample findings; trace to fix and re-test. | Findings tracker | Prioritised, fixed, and re-verified. |
| A-TST-06 | If in scope, inspect TLPT scope, reports, validation, and attestation. | TLPT pack | TLPT done per RTS at required frequency; attestation held. |
| A-TST-07 | Check in-scope third parties were included in TLPT or pooled tests. | TLPT scope | Third parties covered. |
| A-TST-08 | Inspect TLPT method against RTS and TIBER-EU, and regulator validation. | Method, validation | Followed the RTS and TIBER-EU. |

## Pillar 4 - Third-Party Risk

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-TPP-01 | Inspect the third-party strategy and critical-function policy. | Strategy, policy | Board-approved and current. |
| A-TPP-02 | Reconcile the register to procurement, AP, and cloud or SaaS inventory. | Register, AP data | Complete; critical functions flagged. Test completeness hard. |
| A-TPP-03 | Sample new contracts; inspect due-diligence records. | DD files | DD covers risk, criticality, concentration, conflicts. |
| A-TPP-04 | Sample contracts, including critical-function ones; check required and enhanced terms. | Contracts | All required terms present; enhanced terms for critical functions. Test all critical-function contracts. |
| A-TPP-05 | Verify audit and access rights exist and were used on a risk basis. | Contracts, audit reports | Rights secured and exercised. |
| A-TPP-06 | Inspect concentration and sub-outsourcing assessments. | Assessments | Assessed and monitored. |
| A-TPP-07 | Inspect exit strategies and their feasibility tests for critical functions. | Exit docs, test | Written and tested exit plans exist. |
| A-TPP-08 | Check CTPP status is tracked and reflected in risk. | Register, risk notes | Tracked and used. |
| A-TPP-09 | Inspect the yearly register submission to the regulator. | Submission record | Register reported in the period. |

## Pillar 5 - Information Sharing (voluntary)

| Ref | Test step | Evidence | Pass line (Effective) |
|-----|-----------|----------|------------------------|
| A-ISH-01 | Inspect the participation decision. | Decision doc | Written and risk-based. |
| A-ISH-02 | Check sharing is under a formal trusted-community arrangement. | Membership, arrangement | Formal arrangement in place. |
| A-ISH-03 | Inspect the arrangement and legal or DPO review. | Arrangement, review | Confidentiality, GDPR, competition safeguards present. |
| A-ISH-04 | Inspect notifications of joining or leaving. | Notifications | Regulator told where applicable. |
| A-ISH-05 | Check received intelligence is used in detection. | Intake records | Intelligence fed into defences. |

> If the firm chose not to take part in information sharing, mark A-ISH controls "N/A" and note that Art. 45 is voluntary. This is not a finding on its own.

---

## Rating each control

- **Effective:** the control is well designed and worked with no exception in your sample, meeting the pass line.
- **Partially effective:** a design or operating weakness with limited impact, or exceptions within tolerance.
- **Not effective:** the control is missing, poorly designed, or exceptions show it does not do its job.

## Reaching an overall opinion

Roll the control ratings up into one entity-level opinion using this guide. Adjust to your own audit methodology, but state the rule you used.

| Overall opinion | When to give it |
|-----------------|-----------------|
| Compliant / Effective | All or almost all controls Effective. No legal breaches. Any weaknesses are minor (P3 to P4). |
| Partially compliant | Several Partially effective controls, or one or two Not effective controls that are not legal breaches, with a credible fix plan. |
| Non-compliant / Not effective | Any confirmed legal breach (for example a late or missing major-incident report, or an incomplete register), OR many Not effective controls, OR a Not effective control behind a critical or important function. |

**Legal breaches override the maths.** A single confirmed breach of a hard duty (the items marked "(legal)" in the questionnaire) should pull the overall opinion down to at least Partially compliant, and usually Non-compliant, no matter how good the other controls are. Say this plainly in the report.

## Linking to priorities

Give every finding a priority using the [maturity model](../1-gap-assessment/maturity-model.md) priority table. Legal breaches are always P1.
