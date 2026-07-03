# Contributing and Keeping the Toolkit Current

Thanks for helping keep this toolkit accurate. Because it summarises **binding EU
law**, the most important contribution is keeping it **current and correct**, not
just adding content.

## Golden rules

1. **Law wins over convenience.** If a summary and the Official Journal differ,
   fix the summary. Never state a figure you have not checked against EUR-Lex.
2. **One source of truth for numbers.** All regulatory figures (thresholds,
   deadlines) live in "docs/regulatory-references.md". Do not hard-code a number
   in another file — point to that file. If a figure changes, change it there
   once.
3. **Always date your verification.** When you touch a regulatory figure, update
   the "Last verified" / "Last reviewed" date at the top of the file and add a
   note to "CHANGELOG.md" saying which RTS/ITS version it reflects.
4. **No legal advice.** Keep the tone practical and add the standard disclaimer to
   any new document.

## When the regulation changes

The ESAs and the Commission amend RTS/ITS over time. When that happens:

1. Open the amended instrument on EUR-Lex and read the changed articles.
2. Update the figures in "docs/regulatory-references.md" and its "Last verified"
   date.
3. Check the files that reference those figures still read correctly:
   - "templates/incident-classification-aid.md"
   - "docs/2-implementation/02-incident-management-and-reporting.md"
   - "docs/competent-authorities.md"
4. Add a "CHANGELOG.md" entry under Unreleased noting the instrument and date.

## Review checklist before you commit

- [ ] Every regulatory figure traced to an official source (ELI/EUR-Lex link).
- [ ] "Last verified"/"Last reviewed" date updated where figures changed.
- [ ] "CHANGELOG.md" updated with the RTS/ITS basis.
- [ ] No number hard-coded outside "docs/regulatory-references.md".
- [ ] Plain English; disclaimer present on new documents.
- [ ] Links between documents still resolve.

## Suggested review cadence

- **Yearly:** re-verify all figures against EUR-Lex; refresh the NCA directory.
- **On any ESA announcement:** check whether a standard you rely on changed.
- **After a real audit:** feed lessons back into the audit test procedures.

## Style

- ISO 8601 dates (YYYY-MM-DD).
- Prefer tables and short steps over long prose.
- Keep worked examples clearly marked as fictional.

> This document explains how to maintain the toolkit. It is not legal advice.
