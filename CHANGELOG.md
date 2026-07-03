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
- "templates/maturity-scoring-calculator.csv" — all 48 controls pre-listed with
  score, legal-flag, gap and priority columns.
- "examples/model-startup-novapay.md" — a fully worked, fictional end-to-end
  walkthrough across the pillars.
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

### Regulatory basis (verified 2026-07-03)
- DORA: Regulation (EU) 2022/2554.
- Classification RTS: Commission Delegated Regulation (EU) 2024/1772.
- Reporting RTS (content and time limits): Commission Delegated Regulation (EU) 2025/301.

> Reminder: re-verify all figures against EUR-Lex at least yearly and after any
> ESA announcement of amended standards, then update the "last verified" dates.
