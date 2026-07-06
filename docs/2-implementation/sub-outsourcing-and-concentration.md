# Sub-Outsourcing Chains and Concentration Risk (Method)

Two of the hardest practical tasks in Pillar 4 are (1) seeing and controlling the
**sub-outsourcing chain** beneath your direct providers, and (2) honestly measuring
**concentration** risk. This companion to
[playbook 04](04-third-party-risk-management.md) gives a repeatable method for both.

DORA basis: Art. 28 to 30, and specifically the **Subcontracting RTS (Commission
Delegated Regulation (EU) 2025/532)** on what to assess when subcontracting ICT
services that support critical or important functions, plus the **Policy RTS (EU)
2024/1773)**. Numbers and instruments: see
[regulatory-references.md](../regulatory-references.md). Guidance, not legal advice.

---

## Part A: Sub-outsourcing chain assessment

### A1. Why it matters

Your provider can pass work down the chain (a "fourth party" and beyond). The risk
is still yours to manage, but it is now further from your sight, sometimes in a
different country and legal regime. A failure two links down can still take out
your critical function.

### A2. Map the chain (steps)

1. For each provider behind a critical or important function, ask for and record
   the **full sub-outsourcing chain** for that specific service (not the provider
   in general).
2. For each sub-provider capture: legal name, what part of the service they
   provide, country of provision and of data storage, and whether they are
   themselves substitutable.
3. Mark any link that is **material** to the critical function (its failure would
   disrupt the function) versus incidental.
4. Record whether the contract requires the provider to **notify you before**
   material sub-outsourcing changes, and gives you the right to **object or exit**.

### A3. What to assess (per the Subcontracting RTS)

| Question | Why it matters |
|---|---|
| Does sub-outsourcing cover the *whole* or only part of the critical function? | Whole-function sub-outsourcing is higher risk |
| Is the chain length reasonable and transparent? | Long, opaque chains are hard to oversee |
| Are audit/access rights preserved **down the chain**? | You need reach beyond the first party |
| Is data location and applicable law acceptable at each link? | Third-country links add legal/access risk |
| Can the direct provider still meet its obligations if a sub-provider fails? | Tests real resilience |
| Are sub-outsourcing changes notified in advance, with a right to object/exit? | Keeps you in control |

### A4. Chain worksheet (fill per critical-function service)

| Link | Party | Role in the service | Country (service / data) | Material? | Audit reach? | Notify/object right? | Residual risk |
|---|---|---|---|---|---|---|---|
| 1 (direct) | [Provider] | | | | | | |
| 2 (sub) | [Sub-provider] | | | | | | |
| 3 (sub-sub) | | | | | | | |

Decision: is the chain acceptable as-is, acceptable with mitigations, or not
acceptable for a critical function? Record the reasoning and who approved it.

---

## Part B: Concentration risk (make it measurable)

### B1. The idea

Concentration is the risk that too much depends on one provider (or one group, or
one region), so a single failure hits many critical functions at once. "We use one
cloud for everything" is the classic case.

### B2. Dimensions to measure

| Dimension | How to measure it | Red flag |
|---|---|---|
| Provider concentration | Count of critical/important functions per provider or group | One provider behind [3+] critical functions |
| Substitutability | Time/cost/feasibility to move each critical function | Not substitutable within its RTO |
| Geographic concentration | Share of critical processing/data in one region | Single region with no tested failover |
| Sub-provider concentration | Same sub-provider under several direct providers | Hidden common dependency |
| Sector-wide concentration | Whether peers rely on the same CTPP | Systemic single point of failure |

### B3. A simple concentration score

For each provider/group, score: (a) number of critical functions supported, (b)
substitutability (1 easy - 5 locked in), (c) single-region dependency (Y/N). Flag
as **high concentration** if it supports 2+ critical functions **and** scores 4-5
on substitutability, **or** everything sits in one region with no tested failover.

### B4. What to do with a high-concentration finding

You often cannot remove concentration by contract, so manage it deliberately:

- **Reduce lock-in technically** (portable formats, infrastructure-as-code,
  independent segregated backups you control, multi-region or multi-provider where
  feasible for the most critical functions).
- **Record it as an accepted, monitored residual risk** with **board sign-off**
  and named mitigations. An honest, evidenced concentration decision is defensible;
  a silent one is not.
- **Track CTPP status**: if the provider is (or becomes) a designated critical ICT
  third-party provider, factor the EU oversight into your risk view.

---

## Part C: How CTPP oversight fits (what you actually do)

The ESAs directly oversee the most systemically important providers (**CTPPs**),
each with a Lead Overseer. As a normal financial entity you do **not** run this
oversight - the ESAs do. Your job is narrow and concrete: know **whether** any of
your providers are CTPPs, reflect that in your risk assessment and register, and be
ready to act if a CTPP does not follow oversight recommendations (for example, by
revisiting your reliance or exit plan). You do not need to build CTPP-oversight
machinery yourself.

---

## Evidence to keep

Chain maps per critical-function service, sub-outsourcing assessments, provider
notifications of chain changes, the concentration analysis and scores, board
sign-off on accepted concentration risk, and CTPP-status tracking in the register.

Pairs with the [third-party register](../../templates/third-party-register.md),
the [third-party risk policy](../../templates/model-policies/third-party-risk-policy.md),
and playbook 04.
