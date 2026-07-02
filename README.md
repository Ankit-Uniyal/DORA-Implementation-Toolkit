# DORA Implementation & Self-Assessment Toolkit

An end-to-end toolkit for the **Digital Operational Resilience Act (DORA)** — Regulation (EU) 2022/2554. It is designed to support three complementary use cases with equal weight:

- **Implement** — stand up a DORA-compliant operational resilience programme from scratch.
- **Gap-assess** — measure your current state against DORA requirements and prioritise remediation.
- **Audit** — perform independent assurance / internal-audit testing against DORA controls.

> **Regulatory note.** DORA entered into force on 16 January 2023 and became applicable on **17 January 2025**. Its detailed requirements are supplemented by Regulatory Technical Standards (RTS) and Implementing Technical Standards (ITS) developed by the ESAs (EBA, EIOPA, ESMA). This toolkit reflects the Level 1 Regulation and the RTS/ITS package as understood at the time of writing. **Always verify the current, official text on EUR-Lex and the ESA websites before relying on this material for a live compliance or audit engagement.** This toolkit is guidance, not legal advice.

---

## Who is in scope?

DORA applies to a broad set of **financial entities** (credit institutions, payment and e-money institutions, investment firms, crypto-asset service providers, central securities depositories, central counterparties, trading venues, insurance and reinsurance undertakings, intermediaries, crowdfunding service providers, credit rating agencies, and more) and to **critical ICT third-party service providers (CTPPs)**, which fall under a direct EU Oversight Framework. A **proportionality principle** applies: requirements scale with the entity's size, risk profile, and the nature/scope/complexity of its services. A lighter "simplified ICT risk management framework" is available for certain smaller entities.

---

## The five pillars (plus governance)

| # | Pillar | DORA articles (indicative) | Guide |
|---|--------|----------------------------|-------|
| 0 | Governance & proportionality | Art. 5–6 | [governance](docs/implementation/00-governance-and-proportionality.md) |
| 1 | ICT risk management | Art. 5–16 | [ict-risk-management](docs/implementation/01-ict-risk-management.md) |
| 2 | ICT-related incident management, classification & reporting | Art. 17–23 | [incident-management](docs/implementation/02-incident-management-and-reporting.md) |
| 3 | Digital operational resilience testing (incl. TLPT) | Art. 24–27 | [resilience-testing](docs/implementation/03-resilience-testing.md) |
| 4 | ICT third-party risk management | Art. 28–44 | [third-party-risk](docs/implementation/04-third-party-risk-management.md) |
| 5 | Information & intelligence sharing | Art. 45 | [information-sharing](docs/implementation/05-information-sharing.md) |

---

## How to use this toolkit

### If you are IMPLEMENTING
1. Read [governance](docs/implementation/00-governance-and-proportionality.md) and confirm your proportionality tier.
2. Work through each pillar guide in `docs/implementation/`, using the **control objectives** and **implementation steps**.
3. Stand up the artefacts in `templates/` (policy register, ICT asset register, third-party register, incident classification aid, TLPT scoping).
4. Track progress with the [maturity model](docs/gap-assessment/maturity-model.md).

### If you are GAP-ASSESSING
1. Complete the per-pillar [self-assessment questionnaires](docs/gap-assessment/).
2. Score each control using the [maturity model](docs/gap-assessment/maturity-model.md).
3. Use the [control-to-requirement mapping](docs/gap-assessment/control-mapping.md) to evidence coverage and identify gaps.
4. Produce a prioritised remediation backlog.

### If you are AUDITING
1. Scope the engagement using the [audit test procedures](docs/audit/test-procedures.md).
2. Apply the [sampling & evidence guidance](docs/audit/sampling-and-evidence.md).
3. Record results in the [findings & report template](docs/audit/findings-template.md).

---

## Repository structure

```
DORA-Implementation-Toolkit/
├── README.md
├── docs/
│   ├── implementation/      # In-depth guide per pillar + governance
│   ├── gap-assessment/      # Maturity model, questionnaires, control mapping
│   └── audit/               # Test procedures, sampling, findings template
└── templates/               # Reusable registers and working templates
```

---

## Disclaimer

This toolkit is provided under the MIT License for informational purposes only. It does not constitute legal, regulatory, or professional advice. Financial entities remain responsible for their own compliance with DORA and applicable national law.
