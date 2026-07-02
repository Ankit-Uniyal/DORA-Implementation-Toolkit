# DORA Audit Test Procedures

Audit programme for independent assurance (internal audit or external review) over DORA compliance. Each procedure states the control objective, the test steps, and the expected result. Rate each control **Effective / Partially effective / Not effective** and record exceptions in the [findings template](findings-template.md).

> Scope the engagement first (see below), then execute the procedures relevant to the in-scope pillars. Use the [sampling & evidence guidance](sampling-and-evidence.md) to size samples.

---

## Engagement scoping checklist

1. Confirm the entity's DORA applicability, entity type and proportionality tier.
2. Confirm whether the simplified framework (Art. 16) applies.
3. Confirm whether the entity is designated in scope for TLPT (Art. 26).
4. Identify critical/important functions and the ICT assets/third parties supporting them.
5. Agree the audit period, populations (incidents, tests, contracts) and materiality.
6. Confirm the current RTS/ITS in force for the audit period.

---

## Pillar 0 — Governance

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-GOV-01 | Framework approved & reviewed | Inspect board minutes for approval and most recent annual review of the ICT risk framework. | Documented approval within the period; review at least annual. |
| A-GOV-02 | Accountability defined | Inspect RACI/org chart; interview the ICT risk owner. | Roles/accountability documented and understood. |
| A-GOV-03 | Board oversight | Sample board reporting packs; assess evidence of challenge. | Regular reporting with recorded challenge/decisions. |
| A-GOV-04 | Board training | Inspect training records for board members. | Role-appropriate training completed. |

## Pillar 1 — ICT Risk Management

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-RM-02 | Asset inventory complete | Reconcile inventory to a sample of live systems and third-party services; test for shadow IT. | Inventory complete, current, classified, links to functions/third parties. |
| A-RM-04 | InfoSec controls operating | Test a sample of IAM, patching, change and encryption controls for operating effectiveness. | Controls implemented and operating per policy. |
| A-RM-06 | BC/DR tested | Inspect RTO/RPO definitions and the latest BC/DR test report for critical functions. | RTO/RPO defined; test performed; results actioned. |
| A-RM-07 | Backup & restore | Inspect backup policy; re-perform or inspect a restore test; verify segregation. | Backups segregated; restore validated within period. |

## Pillar 2 — Incident Management & Reporting

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-INC-02 | Classification correct | Re-perform classification on a sample of incidents using the RTS criteria. | Classifications consistent and correct. |
| A-INC-04 | Reporting timeliness | For each major incident in the period, trace initial/intermediate/final reports to the deadlines. | All reports submitted within mandated deadlines. |
| A-INC-05 | Reporting completeness | Inspect submitted forms against the ITS template fields. | Reports complete and accurate. |
| A-INC-08 | Lessons learned | Sample post-incident reviews; trace actions to closure. | RCA performed; actions tracked and closed. |

## Pillar 3 — Resilience Testing

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-TST-02 | Critical systems tested | Reconcile the population of critical systems to tests performed in the period. | All critical systems tested at least annually. |
| A-TST-04 | Tester independence | Inspect tester qualifications, independence and (external) insurance. | Testers independent and qualified. |
| A-TST-05 | Findings remediated | Sample findings; trace to remediation and re-test. | Findings prioritised, remediated, re-validated. |
| A-TST-06 | TLPT (if in scope) | Inspect TLPT scope, reports, authority validation and attestation. | TLPT performed per RTS at required frequency; attestation held. |

## Pillar 4 — Third-Party Risk

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-TPP-02 | Register complete | Reconcile the register of information to procurement/AP records and cloud inventory. | Register complete; critical/important flagged. |
| A-TPP-04 | Contract clauses | Sample contracts (incl. critical/important) and check mandatory/enhanced clauses. | All required clauses present. |
| A-TPP-05 | Audit rights | Verify audit/access rights exist and have been exercised on a risk basis. | Rights secured and used appropriately. |
| A-TPP-07 | Exit strategies | Inspect exit strategies and evidence of feasibility testing for critical/important functions. | Documented, tested exit strategies exist. |
| A-TPP-09 | Regulatory reporting | Inspect the annual register submission to the competent authority. | Register reported within period. |

## Pillar 5 — Information Sharing

| Ref | Control objective | Test steps | Expected result |
|-----|-------------------|-----------|-----------------|
| A-ISH-03 | Safeguards in place | Inspect the sharing arrangement and DPO/legal review. | Confidentiality/GDPR/competition safeguards present. |
| A-ISH-04 | Authority notified | Inspect notifications of joining/leaving arrangements. | Notifications made where applicable. |

---

## Rating guidance

- **Effective** — control designed appropriately and operating without exception in the sample.
- **Partially effective** — design or operating deficiency with limited impact; exceptions within tolerance.
- **Not effective** — control absent, poorly designed, or exceptions indicate it does not achieve its objective.

Map every "Partially effective" or "Not effective" rating to a finding, with a priority per the [maturity model](../gap-assessment/maturity-model.md) prioritisation table.
