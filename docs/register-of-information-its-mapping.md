# Register of Information: Mapping the Toolkit Subset to the Official ITS Tables

**Read this before you submit anything to a regulator.** The
[third-party register template](../templates/third-party-register.md) in this
toolkit is a **practical working subset** - great for building and maintaining your
register internally, but it is **not** the format a regulator ingests. The official
register of information is a set of **interlinked structured tables** defined by the
**Register ITS (Commission Implementing Regulation (EU) 2024/2956)** and submitted
through your national channel using the EBA reporting framework (data point model,
taxonomy, and validation rules).

This file maps the toolkit's working fields to the official table structure so you
know what you still have to add before submission, and where to confirm the exact
current specification. Instruments and dates: see
[regulatory-references.md](regulatory-references.md). Guidance, not legal advice.

> Always build against the **current** ITS templates, EBA data point model, and the
> ESAs' register-of-information FAQ for the applicable reporting window. Table codes
> and fields are amended over time; confirm before each submission.

## 1. The official structure (overview)

The ITS organises the register into linked tables, commonly referenced by codes in
the **B_01 to B_07** families. At a high level they cover:

| Table family | What it holds (plain English) |
|---|---|
| B_01.01 | The reporting entity and the scope/level of the register (solo, sub-consolidated, consolidated) |
| B_01.02 | The entities covered (LEIs, names, types) where the register is at group level |
| B_01.03 | The branches in scope |
| B_02.01 | The contractual arrangements (each ICT contract), with reference numbers |
| B_02.02 | Terms of each arrangement (dates, notice, governing law, links to functions) |
| B_02.03 | Intra-group arrangement links |
| B_03.01 to B_03.03 | The ICT third-party service providers (identifiers, type, country, parent) |
| B_04.01 | Which entity signs / uses each arrangement |
| B_05.01 to B_05.02 | The ICT services provided, and their links to functions |
| B_06.01 | The functions supported, with the criticality assessment |
| B_07.01 | The assessment of ICT services supporting critical or important functions (substitutability, exit, sub-outsourcing, etc.) |

The exact set, codes, and cardinalities are defined in the ITS Annexes - treat the
above as an orientation map, not the authoritative list.

## 2. Toolkit field -> official table (where each thing goes)

| Toolkit working field | Goes to (approx. official table) | Notes |
|---|---|---|
| Arrangement ID | B_02.01 (contractual arrangement reference) | Must be a stable unique reference |
| Provider legal name / identifier | B_03.01 (provider) | LEI required; EUID/other where no LEI |
| Provider country | B_03.01 | Country of registration/head office |
| Service description / type | B_05.01 (ICT service) | Uses the ITS service-type taxonomy |
| Supports critical/important function? | B_06.01 (function criticality) | Criticality assessment recorded here |
| Function(s) supported | B_05.02 / B_06.01 links | Service-to-function linkage |
| Contract start/end, notice period | B_02.02 (terms) | Dates in the required format |
| Data locations | B_02.02 / B_07.01 | Storage and processing locations |
| Sub-outsourcing chain | B_07.01 | Assessment for critical-function services |
| Substitutability | B_07.01 | Part of the critical-function assessment |
| Audit/access rights | B_02.02 / B_07.01 | Contract terms and assessment |
| Exit strategy documented/tested | B_07.01 | Exit assessment |
| CTPP designation | B_03.01 / B_03.03 | Provider-level flag |
| Contract owner, last review | Internal only | Not an ITS field; keep for your own management |

## 3. What the toolkit subset does NOT capture (add before submitting)

- **LEIs and standard identifiers** for every provider and covered entity (and the
  correct treatment where an LEI does not exist).
- The **service-type and function taxonomies** exactly as coded in the ITS.
- **Consolidation level** and which entities/branches are in scope (B_01 family).
- The **linkage keys** between tables (arrangement <-> provider <-> service <->
  function) that the validation engine checks.
- Formatting to the **data point model** so the file passes EBA/ESA validation.

## 4. Practical path to a submittable register

1. Build and maintain your register using the toolkit's working template (fast to fill).
2. When a submission window approaches, obtain the **current ITS templates** and the
   **EBA data point model / taxonomy** for that window.
3. Map your working fields into the official tables using section 2 as a starting point.
4. Add the missing identifiers, taxonomies, consolidation scope, and linkage keys (section 3).
5. Run the **ESA/EBA validation rules** and fix errors before you submit through your
   national channel (for example, in Luxembourg, the CSSF eDesk portal - see the
   [Luxembourg overlay](luxembourg-cssf-overlay.md)).
6. Keep the submitted version and the validation output as evidence (control TPP-09).

> Bottom line: use the toolkit subset to *think and maintain*; use the official ITS
> tables and validation to *submit*. Do not send the working subset to a regulator.
