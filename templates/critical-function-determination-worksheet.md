# Template: Critical or Important Function (CIF) Determination Worksheet

Deciding which of your functions are **critical or important** is one of the first
and most consequential judgments in a DORA programme. The strongest requirements
(enhanced contract terms, tested exit, TLPT if named, whole-population audit
testing) attach to these functions no matter your size. Get this wrong and you
either over-build everywhere or, worse, under-protect a function that mattered.

DORA defines a critical or important function as one where a disruption would
**materially impair** your financial performance, the soundness/continuity of your
services, or your ability to meet regulatory obligations (see DORA Art. 3(22) and
the related definitions). This worksheet turns that into a repeatable, evidenced
decision. It is a working aid, not legal advice.

> Write down the reasoning, not just the answer. Assessors want the "why". Keep
> this worksheet with your framework documents and revisit it on material change.

## 1. Method in one line

List every business function, score it against clear impact dimensions, apply a
transparent threshold, then sanity-check the result against regulatory duties and
client harm.

## 2. Scoring dimensions

Score each function 1 (low) to 5 (high) on each dimension. Set your own anchors;
examples given.

| Dimension | What it measures | Example anchor for a "5" |
|---|---|---|
| Client impact | Harm to clients if the function fails | Clients cannot access funds or transact |
| Financial impact | Direct/indirect loss from failure | Loss likely to exceed [materiality figure] |
| Regulatory/legal impact | Breach of a duty if it fails | A missed regulatory deadline or a licence condition |
| Market/systemic impact | Effect beyond your firm | Disruption spreads to counterparties or the market |
| Substitutability | How hard to work around | No manual or alternative process; hard to replace |
| Recovery difficulty | How hard/slow to restore | Very low tolerable downtime (tight RTO) |

## 3. Threshold rule (set and record yours)

A function is **critical or important** if **any** of the following holds (example
rule - tailor and record it):

- Client, financial, regulatory, or market impact scores **4 or 5**, **or**
- Substitutability scores **4 or 5** (you are effectively locked in), **or**
- Its failure would, on its own, breach a hard DORA duty (for example, prevent
  timely major-incident reporting or register submission).

Everything else is a standard function. Borderline cases: default to
critical/important and note why. It is safer to over-protect than to miss one.

## 4. The worksheet (fill one row per function)

| Function | Client | Financial | Regulatory | Market | Substitutability | Recovery diff. | CIF? (Y/N) | Reason / evidence |
|---|---|---|---|---|---|---|---|---|
| [e.g. Payments processing] | 5 | 5 | 5 | 4 | 5 | 5 | Y | Core to the licence; clients cannot transact; no manual fallback |
| [e.g. Customer wallet access] | 5 | 4 | 4 | 2 | 4 | 5 | Y | Direct client harm; tight RTO |
| [e.g. Client onboarding / KYC] | 3 | 3 | 5 | 2 | 3 | 3 | Y | Regulatory duty (AML/KYC) breached if it fails |
| [e.g. Internal HR portal] | 1 | 2 | 1 | 1 | 2 | 2 | N | No client, market, or regulatory impact |

## 5. Sanity checks before you sign off

- Does every function that touches client money, client data, or a regulatory
  deadline come out as critical/important? If not, re-examine it.
- Have you included **shared/enabling** functions (identity/access, core network,
  primary database)? Their failure can take down several critical functions at once.
- Have you cross-checked against the asset register so every CIF has its systems,
  owner, RTO/RPO, and third parties mapped?
- Did the business owner and second line agree the list? Record it.

## 6. What being a CIF triggers downstream

| Area | Extra requirement for CIFs |
|---|---|
| Third-party contracts | Enhanced Art. 30 terms (audit/access, TLPT cooperation, exit) |
| Register of information | Flagged as supporting a critical or important function |
| Exit strategy | Written **and tested** |
| Testing | Included in risk-based testing; in TLPT scope if you are named |
| Audit | Tested on the **whole population**, not a sample |
| Regulator notification | Planned ICT arrangements notified in advance (Art. 28(3)) |

## 7. Record and review

| Field | Value |
|---|---|
| Prepared by / date | |
| Reviewed by (2nd line) | |
| Approved by | |
| Next review / trigger | Yearly and on material change (new product, restructuring, major outsourcing) |

Pairs with the [proportionality guide](../docs/proportionality-guide.md), the
[asset register](ict-asset-register.md), and playbook 04.
