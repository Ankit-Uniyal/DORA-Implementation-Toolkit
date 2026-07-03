# DORA Implementation and Self-Assessment Toolkit

An end-to-end toolkit for the **Digital Operational Resilience Act (DORA)**, Regulation (EU) 2022/2554. It supports three uses, with equal weight:

- **Implement:** build a DORA-compliant resilience programme from scratch.
- **Gap-assess:** measure where you are against DORA and prioritise the fixes.
- **Audit:** independently check compliance against DORA controls.

**New to DORA? Start with the [FAQ](docs/faq.md)** (it explains that there is **no
DORA certification or accreditation** — a common and costly misunderstanding),
then the [Glossary](docs/glossary.md) and the
[Proportionality guide](docs/proportionality-guide.md).

**Last reviewed: 3 July 2026.** This toolkit reflects the main regulation and the
RTS/ITS package as understood at the time of writing. The real regulatory figures
(incident thresholds and reporting deadlines) are kept in one place:
[docs/regulatory-references.md](docs/regulatory-references.md). Always check the
current official text on EUR-Lex and the ESA websites before using this for a real
compliance or audit job. **This is guidance, not legal advice.**

## Start here

| If you want to... | Read this first |
|---|---|
| Understand what "compliant" even means (and why there's no certificate) | [FAQ](docs/faq.md) |
| Understand the words | [Glossary](docs/glossary.md) |
| Know how much applies to you | [Proportionality guide](docs/proportionality-guide.md) |
| See the real thresholds and deadlines | [Regulatory references](docs/regulatory-references.md) |
| Find your supervisor and reporting channel | [Competent authorities](docs/competent-authorities.md) |
| Plan the build | [Implementation roadmap](docs/implementation-roadmap.md) |
| See a fully worked example | [Model startup: NovaPay](examples/model-startup-novapay.md) |

## Who is in scope?

DORA applies to a wide set of financial entities (banks, payment and e-money firms,
investment firms, crypto firms, central securities depositories, central
counterparties, trading venues, insurers and intermediaries, crowdfunding
providers, credit rating agencies, and more) and to **critical ICT third-party
providers (CTPPs)**, which the EU oversees directly. A proportionality principle
means the rules scale to your size, risk, and complexity. Some smaller firms can
use a lighter "simplified framework". See the
[Proportionality guide](docs/proportionality-guide.md).

## The five pillars (plus governance)

| # | Pillar | DORA articles | Guide |
|---|---|---|---|
| 0 | Governance and proportionality | Art. 5 to 6 | [governance](docs/2-implementation/00-governance-and-proportionality.md) |
| 1 | ICT risk management | Art. 6 to 16 | [ict-risk-management](docs/2-implementation/01-ict-risk-management.md) |
| 2 | Incident management, classification and reporting | Art. 17 to 23 | [incident-management](docs/2-implementation/02-incident-management-and-reporting.md) |
| 3 | Resilience testing (including TLPT) | Art. 24 to 27 | [resilience-testing](docs/2-implementation/03-resilience-testing.md) |
| 4 | ICT third-party risk management | Art. 28 to 44 | [third-party-risk](docs/2-implementation/04-third-party-risk-management.md) |
| 5 | Information and intelligence sharing | Art. 45 | [information-sharing](docs/2-implementation/05-information-sharing.md) |

Each guide follows the same shape: what it is really about, the requirements in
plain English, what good and weak look like, control objectives, an ordered
how-to, sample filled-in artifacts, evidence to keep, common mistakes, and a quick
self-check.

## Reference documents

- **[FAQ](docs/faq.md)** — what compliance means, who supervises you, and why there is no "DORA certificate".
- **[Regulatory references](docs/regulatory-references.md)** — the real RTS/ITS thresholds and reporting deadlines, with EUR-Lex links and a "last verified" date. Single source of truth for every number.
- **[Competent authorities](docs/competent-authorities.md)** — per-Member-State supervisor directory and how to set up your incident-reporting channel.

## Fillable templates and calculators

Markdown templates and ready-to-use CSVs you can open in any spreadsheet:

- [ICT asset and dependency register](templates/ict-asset-register.md) · [CSV](templates/ict-asset-register.csv)
- [ICT third-party register of information](templates/third-party-register.md) · [CSV](templates/third-party-register.csv)
- [Policy register](templates/policy-register.md) · [CSV](templates/policy-register.csv)
- [Incident classification aid](templates/incident-classification-aid.md) (pre-filled with the real RTS thresholds)
- [TLPT scoping worksheet](templates/tlpt-scoping-worksheet.md)
- [Maturity scoring calculator (CSV)](templates/maturity-scoring-calculator.csv) — all 48 controls with score, legal-flag, gap and priority columns.

## Worked example

- [Model startup: NovaPay](examples/model-startup-novapay.md) — a fully worked, fictional walkthrough from scoping to audit-ready across all pillars.

## Repository structure
```
DORA-Implementation-Toolkit/
├── README.md
├── CHANGELOG.md            # what changed and which RTS/ITS version it reflects
├── CONTRIBUTING.md         # how to keep the toolkit current with regulatory change
├── docs/
│   ├── faq.md              # compliance vs certification, supervision model
│   ├── regulatory-references.md   # the real RTS/ITS figures (single source of truth)
│   ├── competent-authorities.md   # NCA directory and reporting channels
│   ├── 1-gap-assessment/   # questionnaire, maturity model, control mapping
│   ├── 2-implementation/   # in-depth playbook per pillar plus governance
│   ├── 3-audit/            # test procedures, sampling, findings template
│   ├── glossary.md
│   ├── proportionality-guide.md
│   └── implementation-roadmap.md
├── templates/              # reusable registers (md + csv) and worksheets
└── examples/               # fully worked, fictional model-company walkthrough
```

Related standards and frameworks (ISO/IEC 27001, 22301, 27017, EBA guidelines,
TIBER-EU, NIST CSF, and more) and how they map to each DORA pillar are covered at
the end of [docs/1-gap-assessment/control-mapping.md](docs/1-gap-assessment/control-mapping.md).

## Keeping it current

Because this toolkit summarises binding EU law, it must be maintained. See
[CONTRIBUTING.md](CONTRIBUTING.md) for how to re-verify figures against EUR-Lex,
update the "last verified" dates, and record changes in
[CHANGELOG.md](CHANGELOG.md). Re-check at least yearly and after any ESA
announcement of amended standards.
