# Worked Example: "NovaPay" — a Model Startup End to End

**Last reviewed: 3 July 2026.** This is a **fully worked, fictional** example so a
first-timer can see what "done" looks like across the pillars, not just an empty
template. NovaPay is invented; every figure is illustrative. Use it as a shape to
copy, then replace with your real facts.

> Everything here must be backed by real evidence in a real programme. A filled
> example is a teaching aid, not evidence of compliance.

---

## The company (context)

**NovaPay** is a small EU e-money institution authorised in Ireland, ~40 staff,
running its stack on one hyperscale cloud provider. It offers a wallet and a
payments API to consumers and small merchants.

---

## 1. Scope and proportionality (see docs/proportionality-guide.md)

| Question | NovaPay's answer | Reason / evidence |
|---|---|---|
| Entity type | E-money institution | Central Bank of Ireland authorisation ref EMI-XXXX |
| In scope of DORA? | Yes | EMIs are listed financial entities |
| Excluded under Art. 2? | No | Not a listed exclusion |
| Eligible for simplified framework (Art. 16)? | No (chose full, conservatively) | Handles client funds and payments; treated as full-framework pending legal confirmation |
| Named for TLPT (Art. 26)? | No | Not identified by the NCA; runs baseline testing only |
| Critical/important functions identified? | Yes | Wallet, payments processing, client onboarding, auth |
| Date assessed / next review | 2025-01-10 / 2026-01-10 | Board minute 2025-01 |

**Lesson:** small and simple, but still full-framework by choice, and still bound
by every hard legal duty.

---

## 2. Critical functions and asset register (see templates/ict-asset-register.csv)

NovaPay's critical or important functions: **payments processing, wallet, client
onboarding (KYC), access management**. The filled asset register
(templates/ict-asset-register.csv) links each asset to its function, owner,
provider, RTO/RPO, and last restore test. Highlights:

- Core payments application and database: **Critical**, RTO 2h / RPO 15m,
  restore tested 2025-11.
- KYC API (external, SaaS): **Important**, SOC 2 relied on (no direct audit).
- Backup/DR environment: **Critical**, segregated, partial live failover tested.

**Lesson:** the register is only useful when each critical asset is tied to a
function, an owner, and a **tested** recovery target.

---

## 3. A classification decision (see templates/incident-classification-aid.md)

At 09:40 NovaPay confirms unauthorised access to the wallet system (a critical
function). Running the aid:

- **Criterion 6 (criticality gate):** successful malicious unauthorised access to
  a critical-function system → **gate passed**.
- **Criterion 5 (data losses):** access that may cause data loss (Art. 9(5)(b))
  → **met** (this alone makes it major under Art. 8).
- **Criterion 3 (downtime):** wallet down 2h20m (> 2h for a critical service)
  → **met**.
- Clients (~4%), reputational, geographical, economic (~EUR 30k) → not met.

**Result: MAJOR.** Reporting clock starts at 10:15 (declaration time).

### The reporting timeline NovaPay must hit (Reporting RTS 2025/301)

| Report | Deadline | NovaPay's plan |
|---|---|---|
| Initial notification | 4h from classification / 24h from awareness | Submit by ~12:30 (well inside 4h) |
| Intermediate report | 72h from initial | Submit Day 2 |
| Final report | 1 month from intermediate | Submit ~Day 20 |

NovaPay is an EMI handling payments, so it should confirm whether the
weekend/bank-holiday relief is switched off for it (Art. 5(5)-(6)).

**Lesson:** the decision and the clock are explicit and owned before the incident,
not improvised during it.

---

## 4. Third-party contracts, incl. the hyperscaler problem (see the third-party guide, section 15)

NovaPay runs on one hyperscaler that will not redline its master terms. What
NovaPay actually did:

| Provider | Approach | Result |
|---|---|---|
| Hyperscale cloud (Critical) | Attached the provider's published **DORA financial-services addendum**; relied on pooled audit + SOC 2 / ISO 27001; kept its own segregated backups | Required terms met via addendum + documented substitutes |
| KYC SaaS (Important) | Could not get direct audit; relied on SOC 2 Type II; recorded proportionality reasoning | Acceptable substitute, board-noted |
| Concentration | Everything on one cloud → recorded as an **accepted, board-approved residual risk** with multi-region + independent backups as mitigation | Honest, documented, mitigated |

The filled third-party register is templates/third-party-register.csv.

**Lesson:** a small firm complies through the provider's DORA addendum, documented
audit substitutes, technical anti-lock-in measures, and an honest board-approved
residual-risk record — not through redlines it cannot win.

---

## 5. Testing and TLPT scoping (see templates/tlpt-scoping-worksheet.md)

NovaPay is **not named for TLPT**, so it runs a **baseline** risk-based testing
programme: vulnerability scans, an annual penetration test of the payments API by
an independent tester, and continuity/restore tests. It still completes the TLPT
scoping worksheet once to record *why* TLPT does not currently apply and what
would change that (being named, or growth in systemic importance).

**Lesson:** "not in scope for TLPT" is a decision you **record with reasons**, not
a blank.

---

## 6. Governance and the honest board view

Quarterly, NovaPay's board sees: the maturity heat map per pillar (from
templates/maturity-scoring-calculator.csv), the count of gaps by priority, any
**legal-breach flags** called out separately, and the top P1/P2 fixes with owners
and dates. The board formally approved the ICT risk framework (GOV-01) — a hard
legal duty.

**Lesson:** the management body owning and approving the framework, on the record,
is what turns a pile of documents into a defensible programme.

---

## What NovaPay's "audit-ready" state looks like

- Every critical function mapped to assets, owners, and **tested** recovery targets.
- A classification aid with the real thresholds and a proven, timed reporting runbook.
- A complete register reconciled to real spend, with DORA addenda or documented substitutes for critical providers.
- Baseline testing done, findings fixed and re-tested; TLPT position recorded.
- Board approval and an honest quarterly view, with legal items green.

That is not a certificate (there isn't one — see docs/faq.md). It is a defensible,
evidenced position NovaPay can show its supervisor on demand.
