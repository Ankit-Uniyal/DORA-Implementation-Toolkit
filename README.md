# DORA Implementation and Self-Assessment Toolkit

An end-to-end toolkit for the **Digital Operational Resilience Act (DORA)**, Regulation (EU) 2022/2554. It supports three uses, with equal weight:

- **Implement:** build a DORA-compliant resilience programme from scratch.
- **Gap-assess:** measure where you are against DORA and prioritise the fixes.
- **Audit:** independently check compliance against DORA controls.

New to DORA? Start with the **[Glossary](docs/glossary.md)**, then the **[Proportionality guide](docs/proportionality-guide.md)** to see how much applies to you.

> **Regulatory note.** DORA came into force on 16 January 2023 and applied from 17 January 2025. Its detail sits in Regulatory Technical Standards (RTS) and Implementing Technical Standards (ITS) from the ESAs (EBA, EIOPA, ESMA). This toolkit reflects the main regulation and the RTS/ITS package as understood at the time of writing. **Always check the current official text on EUR-Lex and the ESA websites before using this for a real compliance or audit job.** This is guidance, not legal advice.

---

## Start here

| If you want to... | Read this first |
|-------------------|-----------------|
| Understand the words | [Glossary](docs/glossary.md) |
| Know how much applies to you | [Proportionality guide](docs/proportionality-guide.md) |
| Plan the build | [Implementation roadmap](docs/implementation-roadmap.md) |

## Who is in scope?

DORA applies to a wide set of **financial entities** (banks, payment and e-money firms, investment firms, crypto firms, central securities depositories, central counterparties, trading venues, insurers and intermediaries, crowdfunding providers, credit rating agencies, and more) and to **critical ICT third-party providers (CTPPs)**, which the EU oversees directly. A **proportionality principle** means the rules scale to your size, risk, and complexity. Some smaller firms can use a lighter "simplified framework". See the [Proportionality guide](docs/proportionality-guide.md).

## The five pillars (plus governance)

| # | Pillar | DORA articles | Guide |
|---|--------|---------------|-------|
| 0 | Governance and proportionality | Art. 5 to 6 | [governance](docs/implementation/00-governance-and-proportionality.md) |
| 1 | ICT risk management | Art. 5 to 16 | [ict-risk-management](docs/implementation/01-ict-risk-management.md) |
| 2 | Incident management, classification and reporting | Art. 17 to 23 | [incident-management](docs/implementation/02-incident-management-and-reporting.md) |
| 3 | Resilience testing (including TLPT) | Art. 24 to 27 | [resilience-testing](docs/implementation/03-resilience-testing.md) |
| 4 | ICT third-party risk management | Art. 28 to 44 | [third-party-risk](docs/implementation/04-third-party-risk-management.md) |
| 5 | Information and intelligence sharing | Art. 45 | [information-sharing](docs/implementation/05-information-sharing.md) |

Each guide follows the same shape: what it is really about, the requirements in plain English, what good and weak look like, control objectives, an ordered how-to, sample filled-in artifacts, evidence to keep, common mistakes, and a quick self-check.

## How to use this toolkit

### If you are IMPLEMENTING
1. Read the [Glossary](docs/glossary.md) and [Proportionality guide](docs/proportionality-guide.md).
2. Follow the [Implementation roadmap](docs/implementation-roadmap.md) phase by phase.
3. Work through each pillar guide in `docs/implementation/`.
4. Fill in the artifacts in `templates/`.
5. Track progress with the [maturity model](docs/gap-assessment/maturity-model.md).

### If you are GAP-ASSESSING
1. Answer the [self-assessment questionnaire](docs/gap-assessment/self-assessment-questionnaire.md). Each control has small, testable sub-questions.
2. Score with the [maturity model](docs/gap-assessment/maturity-model.md). Watch the legal-breach flags, which matter more than the average score.
3. Use the [control mapping](docs/gap-assessment/control-mapping.md) to prove coverage and find gaps.
4. Build a prioritised fix list.

### If you are AUDITING
1. Scope and test with the [audit test procedures](docs/audit/test-procedures.md), which cover all 48 controls with clear pass lines.
2. Size samples with the [sampling and evidence guidance](docs/audit/sampling-and-evidence.md).
3. Record results and reach an opinion using the [findings and report template](docs/audit/findings-template.md).

## Repository structure

```
DORA-Implementation-Toolkit/
├── README.md
├── docs/
│   ├── glossary.md
│   ├── proportionality-guide.md
│   ├── implementation-roadmap.md
│   ├── implementation/      # In-depth guide per pillar plus governance
│   ├── gap-assessment/      # Maturity model, questionnaire, control mapping
│   └── audit/               # Test procedures, sampling, findings template
└── templates/               # Reusable registers and working templates
```

## A note on legal duties versus maturity

Some DORA duties are hard legal lines (for example, reporting a major incident on time). The toolkit marks these clearly. A maturity score tells you how healthy a control is. A legal flag tells you if you are breaking a rule today. Fix the legal breaches first. This idea runs through the maturity model, the questionnaire, and the audit opinion guide.

## Disclaimer

Provided under the MIT License for information only. It is not legal, regulatory, or professional advice. Financial entities remain responsible for their own compliance with DORA and national law.
