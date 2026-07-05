# DORA Self-Assessment Questionnaire

A deeper questionnaire for gahp analysis. Each control is broken into small, testable sub-questions so the score is based on real evidence, not a gut feel. Read the [maturity model](maturity-model.md) first, then follow the scoring rule below.

**Read first:** [Glossary](../glossary.md).

---

## How to score (the rule)

For each control:

1. Answer every sub-question with **Yes**, **Partly**, or **No**, and note the evidence.
2. Turn the answers into a 0 to 5 maturity score using this rule:

- **0** = No to all sub-questions. Nothing exists.
- **1** = Yes or Partly to only the "is it documented" type question. It exists on paper only.
- **2** = The control is documented and partly working, but not consistent or complete.
- **3** = Yes to all "documented", "owned", and "operating" sub-questions, with evidence. This is the minimum to call the control compliant.
- **4** = Level 3 plus it is measured (metrics or KPIs) and reviewed regularly.
- **5** = Level 4 plus it is continuously improved using data, threat intelligence, and lessons learned.

3. If any sub-question marked **(legal)** is answered No or Partly, flag the control as a **breach risk**, not just a low score. See the note below.

> **Maturity is not the same as legal compliance.** Some duties are hard legal lines, not a maturity journey. Reporting a major incident late, or not reporting it, is a breach even if your process is otherwise mature. Sub-questions marked **(legal)** are pass or fail duties. A No there means "act now", regardless of the overall score.

---

## Pillar 0 - Governance

### GOV-01 Framework approved and reviewed
- Is the ICT risk framework written down?
- Did the board formally approve it, with minutes? **(legal)**
- Was it reviewed in the last 12 months, or after the last major incident?
- Score (0-5): ___  Evidence: ___

### GOV-02 Roles and accountability
- Are ICT risk roles and accountability documented (for example a RACI)?
- Does every key activity have exactly one accountable owner?
- Do the named people know and accept their role (confirmed by interview)?
- Score (0-5): ___  Evidence: ___

### GOV-03 Board oversight
- Does the board get ICT risk reporting on a regular schedule?
- Does the reporting show real challenge and decisions, not just "noted"?
- Are actions from the board tracked to closure?
- Score (0-5): ___  Evidence: ___

### GOV-04 Board training
- Is there a training plan for the board on ICT resilience?
- Have board members actually completed it, with records?
- Score (0-5): ___  Evidence: ___

### GOV-05 Resilience budget
- Is there a defined budget for resilience?
- Does the board review it at least yearly?
- Score (0-5): ___  Evidence: ___

### GOV-06 Proportionality assessed
- Is there a written proportionality assessment?
- Does it state whether the full or simplified framework applies, and why?
- Is it reviewed when the firm changes materially?
- Score (0-5): ___  Evidence: ___

### GOV-07 Three lines and audit
- Is a three-lines-of-defence model defined?
- Does internal audit cover ICT risk independently, on a plan?
- Score (0-5): ___  Evidence: ___

## Pillar 1 - ICT Risk Management

### RM-01 Resilience strategy
- Is there a written resilience strategy with risk appetite and objectives?
- Did the board approve it?
- Score (0-5): ___  Evidence: ___

### RM-02 Asset and dependency inventory
- Is there an inventory of functions, information assets, and ICT assets?
- Are dependencies and third-party links recorded?
- Is it reconciled to reality regularly (to catch shadow IT)?
- Is each critical asset linked to its function, owner, and recovery targets?
- Score (0-5): ___  Evidence: ___

### RM-03 Risk assessment
- Is there a repeatable risk assessment method?
- Is a current risk register maintained?
- Are risks reassessed on major change?
- Score (0-5): ___  Evidence: ___

### RM-04 Information security controls
- Is there an information security policy and control standards?
- Are key controls (access, MFA, encryption, patching, change) actually operating?
- Is operation checked, not just assumed?
- Score (0-5): ___  Evidence: ___

### RM-05 Detection
- Is logging in place on critical systems?
- Are there defined alert thresholds and a named team that acts on alerts?
- Score (0-5): ___  Evidence: ___

### RM-06 Continuity and recovery
- Do critical functions have agreed RTO and RPO?
- Do response and recovery plans name who does what?
- Has a real test proven recovery inside the RTO?
- Score (0-5): ___  Evidence: ___

### RM-07 Backups
- Is there a backup policy with frequency by criticality?
- Are backups kept separate from live systems?
- Has a real restore been tested in the period?
- Score (0-5): ___  Evidence: ___

### RM-08 Learning
- Are post-incident reviews done for significant incidents?
- Are actions tracked to closure and fed back into controls?
- Is threat intelligence taken in and used?
- Score (0-5): ___  Evidence: ___

### RM-09 Training
- Is there role-based ICT resilience training for staff?
- Is completion recorded, including for the board?
- Score (0-5): ___  Evidence: ___

### RM-10 Framework review
- Was the framework reviewed in the last 12 months?
- Was it also reviewed after any major incident?
- Score (0-5): ___  Evidence: ___

## Pillar 2 - Incident Management and Reporting

### INC-01 Incident process
- Is there a documented end-to-end incident process?
- Does it define severity levels, escalation, and closure?
- Score (0-5): ___  Evidence: ___

### INC-02 Classification
- Is there a classification aid using the DORA and RTS criteria?
- Are the current RTS thresholds filled in? **(legal)**
- Is classification applied consistently, shown by worked examples?
- Score (0-5): ___  Evidence: ___

### INC-03 Roles and escalation
- Is there an on-call and escalation matrix?
- Has it been tested (for example by an exercise)?
- Score (0-5): ___  Evidence: ___

### INC-04 Reporting timeliness
- Is the reporting owner pre-assigned, with a backup?
- Are the current Reporting RTS deadlines built into the runbook? **(legal)**
- For every major incident in the period, were initial, intermediate, and final reports on time? **(legal)**
- Has a timed exercise proven you can meet the first deadline?
- Score (0-5): ___  Evidence: ___

### INC-05 Reporting content
- Do reports match the Reporting RTS template fields? **(legal)**
- Are they complete and accurate?
- Score (0-5): ___  Evidence: ___

### INC-06 Client notification
- Are affected clients told without undue delay? **(legal)**
- Are they given protective advice?
- Score (0-5): ___  Evidence: ___

### INC-07 Threat notification
- Is there a process to assess significant cyber threats for voluntary notification?
- Score (0-5): ___  Evidence: ___

### INC-08 Lessons learned
- Is root-cause analysis done and tracked to closure?
- Score (0-5): ___  Evidence: ___

### INC-09 Payment incidents
- Are payment-related operational and security incidents captured under the same regime? **(legal, if applicable)**
- Score (0-5): ___  Evidence: ___

## Pillar 3 - Resilience Testing

### TST-01 Testing programme
- Is there a documented, risk-based testing programme?
- Is it reviewed periodically?
- Score (0-5): ___  Evidence: ___

### TST-02 Critical systems tested
- Is there a test calendar covering all critical systems?
- Was every critical system tested in the last 12 months? **(legal)**
- Score (0-5): ___  Evidence: ___

### TST-03 Mix of methods
- Does testing use a suitable mix of methods for each system's risk?
- Score (0-5): ___  Evidence: ___

### TST-04 Tester independence
- Are testers independent of those who built the systems?
- Are they qualified, and (if external) insured?
- Score (0-5): ___  Evidence: ___

### TST-05 Findings fixed
- Are findings prioritised and assigned owners and deadlines?
- Are fixes re-tested and verified?
- Score (0-5): ___  Evidence: ___

### TST-06 TLPT (if named)
- If named, is TLPT run at least every three years on production critical functions? **(legal, if in scope)**
- Score (0-5): ___  Evidence: ___

### TST-07 Third parties in TLPT
- Are in-scope third parties included in TLPT, or via pooled testing?
- Score (0-5): ___  Evidence: ___

### TST-08 TLPT method and attestation
- Does TLPT follow the RTS and TIBER-EU, with regulator validation?
- Is the attestation held? **(legal, if in scope)**
- Score (0-5): ___  Evidence: ___

## Pillar 4 - Third-Party Risk

### TPP-01 Strategy and policy
- Is there a board-approved third-party strategy?
- Is there a policy for services supporting critical functions?
- Score (0-5): ___  Evidence: ___

### TPP-02 Register of information
- Does a register of information exist?
- Is it reconciled to actual spend, cloud, and SaaS (completeness)?
- Are critical or important functions flagged?
- Score (0-5): ___  Evidence: ___

### TPP-03 Due diligence
- Is pre-contract due diligence done?
- Does it cover risk, criticality, concentration, and conflicts?
- Score (0-5): ___  Evidence: ___

### TPP-04 Contract terms
- Do contracts hold all required base terms? **(legal)**
- Do critical-function contracts hold the enhanced terms (audit rights, TLPT cooperation, exit)? **(legal)**
- Score (0-5): ___  Evidence: ___

### TPP-05 Audit rights
- Are audit, access, and inspection rights secured in contracts?
- Are they used on a risk basis?
- Score (0-5): ___  Evidence: ___

### TPP-06 Concentration and sub-outsourcing
- Is concentration risk assessed?
- Are sub-outsourcing chains identified and monitored?
- Score (0-5): ___  Evidence: ___

### TPP-07 Exit strategies
- Do critical functions have written exit strategies?
- Have they been tested for feasibility?
- Score (0-5): ___  Evidence: ___

### TPP-08 CTPP tracking
- Is it tracked whether providers are CTPPs?
- Is that reflected in risk management?
- Score (0-5): ___  Evidence: ___

### TPP-09 Regulatory reporting
- Is the register reported to the regulator at least yearly? **(legal)**
- Score (0-5): ___  Evidence: ___

## Pillar 5 - Information Sharing

### ISH-01 Participation decision
- Is the decision to take part (or not) written down and risk-based?
- Score (0-5): ___  Evidence: ___

### ISH-02 Trusted communities
- Does sharing happen in trusted communities under a formal arrangement?
- Score (0-5): ___  Evidence: ___

### ISH-03 Safeguards
- Does the arrangement protect confidentiality, personal data (GDPR), and competition rules?
- Was it reviewed by legal and the DPO?
- Score (0-5): ___  Evidence: ___

### ISH-04 Regulator notified
- Is the regulator told when you join or leave? **(legal, if participating)**
- Score (0-5): ___  Evidence: ___

### ISH-05 Intelligence used
- Is received intelligence fed into detection and response?
- Score (0-5): ___  Evidence: ___

---

## Scoring summary

| Pillar | Controls | Average score | Target | Any breach-risk flags? |
|--------|----------|---------------|--------|------------------------|
| 0 - Governance | 7 | | 3.0 | |
| 1 - ICT risk management | 10 | | 3.0 | |
| 2 - Incident management | 9 | | 3.0 | |
| 3 - Resilience testing | 8 | | 3.0 | |
| 4 - Third-party risk | 9 | | 3.0 | |
| 5 - Information sharing | 5 | | 3.0 | |
| **Overall** | **48** | | **3.0** | |

**How to read the summary.** The average score shows overall maturity. The breach-risk column matters more: any control with a **(legal)** sub-question failing must go straight to the top of the remediation list, even if its number looks acceptable.
