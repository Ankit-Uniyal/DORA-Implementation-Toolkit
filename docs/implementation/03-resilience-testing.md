# Pillar 3 — Digital Operational Resilience Testing

**DORA articles:** Art. 24 (general requirements for testing), Art. 25 (testing of ICT tools and systems), Art. 26 (advanced testing based on threat-led penetration testing — TLPT), Art. 27 (requirements for testers). Supplemented by the RTS on TLPT (aligned with the TIBER-EU framework).

---

## 1. Purpose

DORA requires a risk-based digital operational resilience testing programme to identify weaknesses, deficiencies and gaps, and to verify the readiness to respond to ICT-related incidents. Testing sits on two tiers: a **baseline** programme required of all in-scope entities, and **advanced threat-led penetration testing (TLPT)** required of a subset of significant entities identified by authorities.

## 2. General testing requirements (Art. 24)

- Establish, maintain and review a sound and comprehensive **digital operational resilience testing programme** as an integral part of the ICT risk management framework.
- Testing must be **risk-based**, follow a documented methodology, and be performed by independent parties (internal or external).
- Prioritise, classify and remediate all issues revealed during testing; establish counter-measures and validate their effectiveness.
- All **critical ICT systems and applications** must be tested at least yearly.

## 3. Baseline testing toolkit (Art. 25)

The programme should include, as appropriate: vulnerability assessments and scans, open-source analyses, network security assessments, gap analyses, physical security reviews, questionnaires and scanning software solutions, source-code reviews where feasible, scenario-based tests, compatibility testing, performance testing, end-to-end testing, and penetration testing. For microenterprises, tests are planned by combining a risk-based approach with the strategic evolution of ICT.

## 4. Advanced testing — TLPT (Art. 26)

Entities identified by competent authorities (based on impact on the financial sector, financial-stability concerns, and ICT risk profile) must carry out **TLPT at least every three years** (the authority may adjust the frequency). Key features:
- TLPT covers several or all **critical or important functions** and is performed on live production systems.
- The scope is validated by the authority (or the designated public body).
- Where ICT third-party providers are in scope, they are included in the TLPT; pooled testing arrangements are possible for shared providers.
- On completion, a summary of findings, remediation plans and documentation must be provided, and the authority issues an attestation confirming the test was performed in accordance with requirements.
- The RTS on TLPT is developed in line with the **TIBER-EU** framework (red-team testing driven by realistic threat intelligence).

## 5. Requirements for testers (Art. 27)

Testers must have: the highest suitability and reputation; technical and organisational capabilities and specific expertise in threat intelligence, penetration testing and red-team testing; certification or adherence to formal codes of conduct/frameworks; and (for external testers) professional indemnity insurance. Where internal testers are used, additional conditions apply (approval by the authority, no conflicts of interest, etc.).

## 6. Control objectives

| ID | Control objective |
|----|-------------------|
| TST-01 | A documented, risk-based resilience testing programme exists and is reviewed periodically. |
| TST-02 | All critical ICT systems and applications are tested at least annually. |
| TST-03 | Testing uses an appropriate mix of techniques proportionate to risk. |
| TST-04 | Testers are independent and appropriately qualified; conflicts of interest are managed. |
| TST-05 | Findings are prioritised, classified, remediated, and re-validated. |
| TST-06 | Entities in scope for TLPT conduct it at least every three years covering critical/important functions on production. |
| TST-07 | In-scope ICT third parties are included in TLPT (or via pooled testing). |
| TST-08 | TLPT is conducted per the RTS/TIBER-EU methodology, with authority validation and attestation. |

## 7. Implementation steps

1. **Design the testing programme**: inventory critical systems, define a risk-based test calendar, methods, and independence rules.
2. **Establish the baseline test suite** (vulnerability scanning, pen tests, scenario/end-to-end tests, etc.) with owners and cadence.
3. **Build a remediation workflow** linking findings to risk register, owners, deadlines and re-test.
4. **Determine TLPT applicability** with your competent authority and plan the multi-year cycle if in scope.
5. **Scope TLPT** around critical/important functions and relevant third parties; engage threat-intelligence and red-team providers meeting Art. 27 criteria.
6. **Run the TLPT** per TIBER-EU phases (preparation, threat intelligence & red teaming, closure), with control-team oversight and authority validation.
7. **Report and attest**: capture findings, remediation plans, and obtain the authority attestation.
8. **Feed results** into the ICT risk framework and continuous improvement loop.

## 8. Evidence to retain

- Testing programme document and annual test calendar.
- Test reports for critical systems (dated, with scope and methodology).
- Tester independence/qualification records and, for external testers, insurance.
- Findings register with prioritisation, remediation and re-test evidence.
- TLPT scoping documents, threat-intel and red-team reports, control-team logs.
- Authority validation and attestation for TLPT.

## 9. Common pitfalls

- Ad hoc testing with no documented, risk-based programme.
- Critical systems missed in the annual test cycle due to incomplete inventory.
- Findings identified but not tracked to closure or re-tested.
- Assuming baseline penetration testing satisfies the TLPT requirement (it does not — TLPT is threat-led red teaming on production).
- Overlooking in-scope third parties in TLPT scope.
