# DORA Maturity Model & Scoring Guide

Use this maturity model to score each control in the self-assessment questionnaires and to translate scores into a prioritised remediation backlog. It applies equally to implementation tracking, gap assessment, and audit rating.

---

## 1. Five-level maturity scale

| Level | Name | Definition |
|-------|------|------------|
| 0 | **Absent** | No process, control or documentation exists. The requirement is not addressed. |
| 1 | **Initial / Ad hoc** | The activity happens informally or reactively. Not documented, not repeatable, dependent on individuals. |
| 2 | **Developing / Defined** | A documented process/control exists but is inconsistently applied or not yet fully operational. |
| 3 | **Established / Implemented** | The control is documented, implemented consistently, and owned. Evidence of operation exists. |
| 4 | **Managed / Measured** | The control is measured with metrics/KPIs, reviewed regularly, and demonstrably effective. |
| 5 | **Optimised** | The control is continuously improved using metrics, threat intelligence and lessons learned; integrated and automated where appropriate. |

**Compliance threshold.** For DORA, a target of **Level 3 (Established)** or above is generally the minimum to evidence compliance for a given control, with Level 4+ expected for the most critical controls (e.g. incident reporting timeliness, backups, TLPT for in-scope entities). Levels 0–2 indicate a gap requiring remediation.

## 2. Scoring method

1. Score each control 0–5 using the scale above, based strictly on **observed evidence** (not intent).
2. Record the evidence reference and any notes for each score.
3. Compute a **pillar score** as the average (or weighted average) of its control scores.
4. Compute an **overall score** as the weighted average of pillar scores (weight by risk/criticality if desired).
5. Flag any control below the target level as a **gap**.

## 3. Gap rating & prioritisation

Combine the maturity gap with the risk of the underlying requirement to prioritise:

| Priority | Criteria |
|----------|----------|
| **P1 — Critical** | Control at Level 0–1 AND supports a critical/important function or a hard regulatory deadline (e.g. major-incident reporting, backups, TLPT). |
| **P2 — High** | Control at Level 0–2 with material risk, or a mandatory requirement not yet operational. |
| **P3 — Medium** | Control at Level 2–3 needing consistency or measurement improvements. |
| **P4 — Low** | Control at Level 3+ with minor optimisation opportunities. |

## 4. Remediation backlog fields

For each gap, capture: control ID, current level, target level, priority (P1–P4), root cause, remediation action, owner, due date, dependencies, and re-assessment date.

## 5. Reporting the results

Present results as: an overall maturity score, a per-pillar heat map (0–5), the count of gaps by priority, and the top P1/P2 remediation items with owners and dates. This view supports the board reporting expected under Art. 5.

## 6. Worked example

| Control | Evidence observed | Level | Gap? | Priority |
|---------|-------------------|-------|------|----------|
| INC-04 (report major incidents within deadline) | Runbook exists but no test proves the initial deadline can be met; ownership unclear | 2 | Yes | P1 |
| RM-07 (backup segregation & restore testing) | Backups run and are segregated; restore tested annually with report | 4 | No | P4 |
| TPP-02 (register of information) | Partial register; SaaS and intra-group arrangements missing | 2 | Yes | P2 |
