# Changelog

All notable changes to the DORA Implementation and Self-Assessment Toolkit.
Because this toolkit summarises binding EU law, every content change should note
**which RTS/ITS version it reflects** and **when it was last verified**, so users
can detect regulatory drift.

Format loosely follows Keep a Changelog. Dates are ISO 8601.

## [Unreleased]

## [2026-07-05]

### Added
- "templates/dora-workbook.xlsx" — native Excel version of the combined workbook with live formulas: auto-scoring, per-pillar averages, and RAG status; a 0-5 score data-validation dropdown; and conditional formatting on scores and RAG cells. Mirrors the HTML workbook's structure and logic so the two stay consistent. README updated with a download link.
- GitHub Pages enabled (deploy from main) so the combined workbook has a live, clickable URL: https://ankit-uniyal.github.io/DORA-Implementation-Toolkit/templates/dora-workbook.html — it runs in the browser with no download. README updated with this link.
- "templates/dora-workbook.html" — single-file, offline-capable combined workbook: linked tabs for the asset, third-party and policy registers plus maturity scoring, an auto-calculating maturity heat map and overall-readiness gauge, and per-tab CSV export. Loads the source CSVs from main on open.
- "docs/luxembourg-cssf-overlay.md" — Luxembourg overlay covering CSSF/CAA competent-authority split, the binding CSSF circulars (25/893, 25/892, 25/882, 25/880, 23/834, 21/769), incident reporting to the CSSF, the ICT third-party notification routes (IMAS vs CSSF form; 3-month / 1-month lead times), register-of-information submission via the CSSF eDesk portal, and TLPT under TIBER-LU.
- "templates/master-traceability-matrix.csv" — audit-navigable matrix linking each of the 48 controls to its DORA article, supplementing RTS/ITS, questionnaire item, audit test (A-*), primary evidence, and an evidence-location/status column to fill in.
- "docs/regulatory-references.md" — added the Reporting ITS (EU) 2025/302 (forms, templates, procedures) as a distinct row alongside the Reporting RTS 2025/301.

### Fixed
- "templates/dora-workbook.html" — sticky table headers were offset by 52px and overlapped the first data row (hiding Pillar 1 on the heat map and the first control on each register). Header offset corrected to the top of each scroll container, and the dashboard heat-map header set to static. Verified live on GitHub Pages: 48 controls load, entering a score recomputes the pillar rollup, dashboard tiles and RAG colour instantly.
- "templates/dora-workbook.html" — removed a duplicate CSS/HTML block that had been accidentally appended after the closing </html>; it was overriding the corrected header rule and reintroducing the overlap. File is now a single well-formed document (126 lines) and verified live on GitHub Pages.

### Changed
- "docs/regulatory-references.md" — every instrument number, OJ citation, in-force status, incident-classification threshold, and reporting deadline re-verified against the authentic Official Journal text on EUR-Lex; "last verified" note updated accordingly.

### Regulatory basis (verified 2026-07-05 against EUR-Lex authentic OJ text)
- DORA 2022/2554; ICT risk RTS 2024/1774; Classification RTS 2024/1772; Register ITS 2024/2956; Reporting RTS 2025/301; Reporting ITS 2025/302; Subcontracting RTS 2025/532; TLPT RTS 2025/1190 — all confirmed "In force".


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
