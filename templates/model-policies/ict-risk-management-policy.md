# Model Policy: ICT Risk Management Policy

> **Skeleton draft, not legal advice.** Fill the [brackets], delete what does not apply, and have the management body approve the final version. Keep all regulatory figures pointing to [docs/regulatory-references.md](../../docs/regulatory-references.md). Pairs with playbook `docs/2-implementation/01-ict-risk-management.md`.

| Field | Value |
|---|---|
| Document owner | [CISO / Head of ICT Risk] |
| Approved by | [Board / Risk Committee], minute ref [___] |
| Version / date | [v1.0] / [YYYY-MM-DD] |
| Next review | [YYYY-MM-DD] (at least yearly and after any major incident) |
| Applies to | All staff, contractors, and systems of [Entity] |

## 1. Purpose

This policy sets out how [Entity] identifies, protects against, detects, responds to, recovers from, and learns from ICT risk, so that the firm can keep delivering its critical or important functions. It gives effect to DORA (Regulation (EU) 2022/2554) Art. 5 to 13 and the ICT risk RTS (EU) 2024/1774.

## 2. Scope

All ICT systems, information assets, services, and third-party arrangements that support [Entity]'s business functions, including cloud, SaaS, and intra-group services. State whether the simplified framework under Art. 16 applies and why (see the proportionality assessment).

## 3. Governance and accountability

- The management body owns ICT risk and cannot delegate that accountability (Art. 5). [Name the accountable board member or committee.]
- [Owner role] runs the framework day to day.
- Roles follow the three lines of defence and the RACI in the governance playbook.
- The board approves this policy, sets risk appetite, and reviews reporting at [monthly / quarterly] intervals.

## 4. Risk appetite

[Entity] will state its appetite in plain terms, for example: tolerate no unplanned downtime beyond the RTO for Tier 1 functions; accept no known critical vulnerability on internet-facing critical systems beyond [X] days. Risks outside appetite are escalated to [the board / risk committee] for a decision to mitigate, transfer, or accept.

## 5. The five jobs (Art. 8 to 13)

**Identify (Art. 8).** Maintain a live inventory linking each critical function to its systems, data, owners, recovery targets, and third parties. Run repeatable, recorded risk assessments at least [yearly] and on major change.

**Protect (Art. 9).** Enforce documented security control standards covering at least: access control and least privilege, multi-factor authentication, encryption in transit and at rest, patching within defined windows, change management, secure configuration, and logging. See the Information Security Policy.

**Detect (Art. 10).** Log critical systems, set alert thresholds, and route alerts to a named team that acts on them.

**Respond and recover (Art. 11, 12).** Every critical function has an agreed RTO and RPO, response and recovery plans that name who does what, and segregated backups that are restore-tested. See the BC/DR Policy.

**Learn (Art. 13).** Run post-incident reviews, take in threat intelligence, and deliver role-based training, including for the board.

## 6. Legal duties that override maturity

Some duties are pass/fail, not a maturity journey. [Entity] will always: report major incidents inside the deadlines in docs/regulatory-references.md; keep and submit the register of information; and run TLPT if named. A failure here is a breach, not a low score.

## 7. Roles and responsibilities

| Role | Responsibility |
|---|---|
| Management body | Owns ICT risk; approves this policy and risk appetite |
| [CISO / Head of ICT Risk] | Runs the framework; maintains standards and reporting |
| IT Operations | Runs day-to-day controls, detection, backups |
| Risk / Compliance | Second-line oversight and challenge |
| Internal Audit | Independent third-line assurance |

## 8. Related documents

Information Security Policy; BC/DR Policy; Incident Management & Reporting Policy; Third-Party Risk Policy; the proportionality assessment; docs/regulatory-references.md.

## 9. Review and version control

Reviewed at least yearly and after any major incident. Changes are version-controlled and re-approved by the management body. Approval is recorded in board minutes (evidence for control GOV-01 and RM-10).
