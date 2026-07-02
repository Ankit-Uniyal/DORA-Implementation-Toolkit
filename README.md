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
| 0 | Governance and proportionality | Art. 5 to 6 | [governance](docs/2-implementation/00-governance-and-proportionality.md) |
| 1 | ICT risk management | Art. 5 to 16 | [ict-risk-management](docs/2-implementation/01-ict-risk-management.md) |
| 2 | Incident management, classification and reporting | Art. 17 to 23 | [incident-management](docs/2-implementation/02-incident-management-and-reporting.md) |
| 3 | Resilience testing (including TLPT) | Art. 24 to 27 | [resilience-testing](docs/2-implementation/03-resilience-testing.md) |
| 4 | ICT third-party risk management | Art. 28 to 44 | [third-party-risk](docs/2-implementation/04-third-party-risk-management.md) |
| 5 | Information and intelligence sharing | Art. 45 | [information-sharing](docs/2-implementation/05-information-sharing.md) |


Each guide follows the same shape: what it is really about, the requirements in plain English, what good and weak look like, control objectives, an ordered how-to, sample filled-in artifacts, evidence to keep, common mistakes, and a quick self-check.


## Repository structure

```
DORA-Implementation-Toolkit/
├── README.md
├── docs/
│   ├── 1-gap-assessment/      # Start here: questionnaire, maturity model,
│   │                          #   control mapping (also holds the standards-to-DORA mapping)
│   ├── 2-implementation/      # In-depth playbook per pillar plus governance
│   ├── 3-audit/               # Test procedures, sampling, findings template
│   ├── glossary.md
│   ├── proportionality-guide.md
│   └── implementation-roadmap.md
└── templates/                 # Reusable registers and working templates
```

Related standards and frameworks (ISO/IEC 27001, 22301, 27017, EBA guidelines, TIBER-EU, NIST CSF, and more) and how they map to each DORA pillar are covered at the end of [docs/1-gap-assessment/control-mapping.md](docs/1-gap-assessment/control-mapping.md).
