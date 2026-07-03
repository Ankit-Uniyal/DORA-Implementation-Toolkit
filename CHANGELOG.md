# Changelog

All notable changes to the DORA Implementation and Self-Assessment Toolkit.
Because this toolkit summarises binding EU law, every content change should note
**which RTS/ITS version it reflects** and **when it was last verified**, so users
can detect regulatory drift.

Format loosely follows Keep a Changelog. Dates are ISO 8601.

## [Unreleased]

### Added
- "docs/regulatory-references.md" — single source of truth for the real RTS/ITS
  figures (classification thresholds, reporting deadlines) with EUR-Lex links and
  a "last verified" date.
- "docs/faq.md" — debunks the "DORA certification/accreditation" myth and
  explains the supervisory model.
- "docs/competent-authorities.md" — per-Member-State NCA directory and how to
  find your incident-reporting channel.
- "templates/third-party-register.csv", "templates/ict-asset-register.csv",
  "templates/policy-register.csv" — fillable CSV registers with worked example
  rows.
- "templates/maturity-scoring-calculator.csv" — all 48 controls with score,
  legal-flag, gap and priority columns.
- "examples/model-startup-novapay.md" — a fully worked, fictional walkthrough
  across all pillars.
- "CONTRIBUTING.md" — how to keep the toolkit current with regulatory change.

### Changed
- "templates/incident-classification-aid.md" — placeholders replaced with the
  real thresholds from Classification RTS (EU) 2024/1772 and deadlines from
  Reporting RTS (EU) 2025/301; added a worked example.
- "docs/2-implementation/02-incident-management-and-reporting.md" — filled the
  [from RTS]/[from ITS] placeholders with the real classification thresholds and
  the 4h / 72h / 1-month reporting deadlines, with citations.
- "docs/2-implementation/04-third-party-risk-management.md" — added guidance for
  small firms with no negotiating leverage against hyperscalers (DORA addenda,
  audit substitutes, anti-lock-in, board-approved residual risk).
- "README.md" — linked the new documents and artifacts.
- "docs/regulatory-references.md" — added the verified Official Journal (OJ)
  references and permanent ELI links for all seven core standards (previously four
  were shown only as "see ESA page"); refreshed the verification note.
- "templates/ict-asset-register.csv" — fixed a column-alignment defect where the
  header had 17 columns but the example rows had 16, which shifted every value
  after hosting_location and dropped the notes column. All rows now have 17 columns.
- "templates/maturity-scoring-calculator.csv" — fixed a column-count defect where
  the header had 15 columns but all 48 control rows had 14, which stopped GitHub
  rendering the table and misaligned the final column. Added the missing trailing
  field so every row now has 15 columns. (Note: this fix was committed with an
  inaccurate auto-generated commit message; this CHANGELOG entry is the accurate
  description of that change.)

### Regulatory basis (verified 2026-07-03 against EUR-Lex)
- DORA: Regulation (EU) 2022/2554 — OJ L 333, 27.12.2022.
- ICT risk RTS: Commission Delegated Regulation (EU) 2024/1774 — OJ L, 2024/1774, 25.6.2024.
- Classification RTS: Commission Delegated Regulation (EU) 2024/1772 — OJ L, 2024/1772, 25.6.2024.
- Register of information ITS: Commission Implementing Regulation (EU) 2024/2956 — OJ L, 2024/2956, 2.12.2024.
- Reporting RTS (content and time limits): Commission Delegated Regulation (EU) 2025/301 — OJ L, 2025/301, 20.2.2025.
- Subcontracting RTS: Commission Delegated Regulation (EU) 2025/532 — OJ L, 2025/532, 2.7.2025.
- TLPT RTS: Commission Delegated Regulation (EU) 2025/1190 — OJ L, 2025/1190, 18.6.2025.

> Reminder: re-verify all figures against EUR-Lex at least yearly and after any
> ESA announcement of amended standards, then update the "last verified" dates.
