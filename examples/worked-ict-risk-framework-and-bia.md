# Worked Example: NovaPay ICT Risk Management Framework and BIA

**Fully worked, fictional example.** A first-timer can copy a policy skeleton but
still not know what a *filled* ICT risk framework or a business impact analysis
(BIA) actually looks like. This shows both, using NovaPay from
[model-startup-novapay.md](model-startup-novapay.md). Replace with your real facts.
Teaching aid, not legal advice or evidence of compliance.

Pairs with the [ICT risk management policy](../templates/model-policies/ict-risk-management-policy.md)
and [playbook 01](../docs/2-implementation/01-ict-risk-management.md).

---

## Part 1: The ICT risk management framework (worked)

A framework document does not need to be long. NovaPay's is about three pages. Here
is the shape, filled in.

### 1.1 Purpose and scope

NovaPay manages ICT risk to keep its critical functions (payments processing,
client wallet, onboarding/KYC, access management) running. Scope: all systems, data,
and providers behind those functions, including its single hyperscale cloud.

### 1.2 Risk appetite (quantified)

| Statement | NovaPay's appetite |
|---|---|
| Unplanned downtime, Tier 1 | Zero tolerance beyond the RTO (2h) |
| Known critical vulnerabilities, internet-facing | None older than 14 days |
| Data loss, Tier 1 | None beyond the RPO (15 min) |
| Unreviewed privileged access | Zero |
| Major incidents reported late | Zero (legal duty) |

### 1.3 Governance

The board's Risk Committee owns ICT risk (minute 2026-01). The CISO runs the
framework. Three lines of defence: engineering (1st), risk/compliance (2nd),
outsourced internal audit (3rd).

### 1.4 The five jobs, mapped to NovaPay's controls

| Job (DORA Art.) | What NovaPay does | Evidence |
|---|---|---|
| Identify (8) | Asset register linking each critical function to systems, owner, RTO/RPO, providers | ict-asset-register.csv |
| Protect (9) | Security control standards (MFA, encryption, patching, least privilege) | Information Security Policy + configs |
| Detect (10) | Cloud-native logging + SIEM alerts to the on-call SOC | Alert config, sample tickets |
| Respond/recover (11,12) | RTO/RPO per function, recovery runbooks, segregated backups | BC/DR Policy + restore-test report |
| Learn (13) | Post-incident reviews, threat intel feed, role-based training | Reviews, training log |

### 1.5 Review

Reviewed yearly and after any major incident; re-approved by the Risk Committee.

---

## Part 2: The Business Impact Analysis (worked)

The BIA is how you *derive* RTO and RPO from real impact, instead of guessing.
NovaPay's method: for each function, estimate how impact grows with outage duration,
then set the RTO where impact becomes unacceptable, and the RPO from how much data
loss the business can absorb.

### 2.1 Impact-over-time (one function shown: client wallet)

| Outage duration | Impact on NovaPay | Severity |
|---|---|---|
| 0-30 min | Minor client friction; few complaints | Low |
| 30 min - 2h | Rising complaints; some failed transactions; reputational risk | Medium |
| 2h - 4h | Widespread client harm; likely media; possible regulatory attention | High |
| > 4h | Serious client harm; likely regulatory breach territory | Severe |

**RTO decision:** set at **2h** - the point just before impact becomes High.
**RPO decision:** wallet balances must be near-exact, so **15 min** maximum data loss.

### 2.2 BIA table (all critical functions)

| Function | Max tolerable outage -> RTO | Max tolerable data loss -> RPO | Key dependencies | Tier |
|---|---|---|---|---|
| Payments processing | 2h | 15 min | Cloud region A, payments DB, KYC | 1 |
| Client wallet | 2h | 15 min | Cloud region A, wallet DB, auth | 1 |
| Onboarding / KYC | 8h | 4h | KYC SaaS, identity provider | 2 |
| Access management | 2h | 15 min | Identity provider (shared dependency) | 1 |
| Internal reporting | 24h | 24h | Data warehouse | 3 |

Note how **access management** is Tier 1 even though it is "internal": it is a
**shared dependency** whose failure takes down payments and wallet at once. The BIA
surfaces that; a naive function list would miss it.

### 2.3 From BIA to action

- RTO/RPO feed the recovery plans and the restore-test pass lines (playbook 01).
- The shared-dependency finding drives extra resilience on the identity provider.
- The single-region dependency is recorded as a concentration risk (see the
  [sub-outsourcing and concentration method](../docs/2-implementation/sub-outsourcing-and-concentration.md)).

### 2.4 Method notes (so you can repeat it)

1. List functions from the [CIF worksheet](../templates/critical-function-determination-worksheet.md).
2. For each, agree impact-over-time with the business owner (not IT alone).
3. Set RTO at the last duration before impact turns High; set RPO from tolerable data loss.
4. Capture dependencies (including shared/enabling ones).
5. Prove the numbers by testing; adjust if a restore cannot meet the RTO.

**Lesson:** RTO and RPO are **outputs of the BIA**, agreed with the business and
proven by testing - not numbers invented by IT and never checked.
