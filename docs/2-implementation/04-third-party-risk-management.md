# Pillar 4: ICT Third-Party Risk Management (Playbook)

DORA articles: Art. 28 to 44. Supplemented by the ITS on the register of information, the RTS on subcontracting, and the RTS on the policy for ICT services supporting critical or important functions.

Read first: Glossary. Use with: Third-party register template.

This is a playbook. It gives you the steps, a due-diligence checklist, a contract clause checklist, an exit-plan method, and worked examples.

## At a glance
| Item | Detail |
|---|---|
| Goal | Manage the risk from outside ICT providers as if it were your own, because it is. |
| Who leads | Head of Procurement or Third-Party Risk, with Legal and the CISO. |
| Typical time | 20 weeks to build the core; then ongoing. |
| Main outputs | Third-party strategy, register of information, due-diligence process, fixed contracts, tested exit plans. |
| Done when | The register matches real spend, your top provider has audit rights and a tested exit plan, and you report the register yearly. |

## 1. What this pillar is really about

Most firms depend heavily on outside technology: cloud platforms, software vendors, data centres, managed services. If one fails or is breached, your firm feels it directly. DORA treats this outside risk as your risk. You cannot outsource the responsibility, only the activity.

There are two parts: what you must do to manage your own providers, and the EU Oversight Framework, where regulators directly supervise the biggest providers (called CTPPs).

## 2. Before you start (prerequisites)
- The Pillar 1 inventory, so you know which providers sit behind critical functions.
- Access to procurement, accounts-payable, and cloud or SaaS data for a complete register.
- Legal support for contract review.
- The third-party register template.

## 3. Step-by-step build

**Step 1: Approve the strategy and policy.** Owner: Board. Get a third-party risk strategy and a specific policy for services behind critical functions approved.

**Step 2: Build the register of information.** Owner: Third-Party Risk lead. Use the template. Reconcile against accounts-payable and cloud or SaaS inventories so nothing is missing.

**Step 3: Flag critical or important arrangements.** Owner: Business owners. Mark each arrangement as supporting a critical function or not.

**Step 4: Set up due diligence for new contracts.** Owner: Procurement. Use the checklist below before signing anything.

**Step 5: Review existing contracts.** Owner: Legal with the CISO. Use the clause checklist below. Fix gaps, starting with audit rights and exit terms.

**Step 6: Write and test exit strategies.** Owner: Business owners. For each critical function, write an exit plan and then test it.

**Step 7: Monitor and report.** Owner: Third-Party Risk lead. Track service levels, incidents, sub-outsourcing changes, and CTPP status. Report the register to the regulator yearly.

## 4. Ready-to-use artifact: due-diligence checklist (before you sign)
- What service is it, and does it support a critical or important function?
- Financial and operational health of the provider.
- Security posture: certifications, past incidents, and how they handle breaches.
- Where is the data stored and processed, and under what law?
- Sub-outsourcing: who else is in the chain, and where?
- Concentration: do we already rely heavily on this provider or its group?
- Conflicts of interest.
- Can we get audit and access rights, and a workable exit?

## 5. Ready-to-use artifact: contract clause checklist

Every ICT contract needs a base set of terms. Contracts for critical or important functions need more.

| Clause | Needed for all? | Needed for critical? |
|---|---|---|
| Clear description of the service | Yes | Yes |
| Where the service runs and data is held | Yes | Yes |
| Data protection and data return on exit | Yes | Yes |
| Service levels | Basic | Full, with targets |
| Help during incidents | Yes | Yes |
| Cooperation with regulators | Yes | Yes |
| Termination rights | Yes | Yes |
| Duty to follow your security requirements | | Yes |
| Cooperation with your TLPT | | Yes |
| Full audit, access, and inspection rights | Basic | Full, for you and regulators |
| Exit and transition terms | Yes | Yes, with a transition period |

The most common gaps are missing audit and access rights and missing exit and transition terms. Check these first.

## 6. Ready-to-use artifact: exit-plan method (steps to copy)
- Name the critical function and its provider.
- Describe the target end state (another provider, in-house, or a mix).
- List what must move: data, configurations, integrations, and knowledge.
- Estimate the transition time and the resources needed.
- Identify the triggers that would make you exit (provider failure, price, risk).
- Test the plan: a tabletop at minimum, a partial live trial where possible.
- Record the test result and fix any gaps found.

Pass line: the plan is written, and a test shows you could leave without unacceptable disruption.

## 7. Concentration, sub-outsourcing, and CTPPs

Before relying on a provider for a critical function, ask: could we easily replace them, or are we locked in? Do many critical functions sit with the same provider or group? Does the provider pass work down a chain, especially outside the EU, and can we still see and control the risk?

The ESAs name the most systemically important providers as CTPPs and oversee them directly, each with a Lead Overseer. Your job is to know whether your providers are CTPPs, factor that into your risk view, and be ready to act if a CTPP ignores oversight recommendations.

## 8. Worked example: a register row (short form)
| Provider | Service | Supports critical function? | Substitutable? | Audit rights? | Exit tested? | CTPP? | Risk |
|---|---|---|---|---|---|---|---|
| CloudCo | Payments hosting | Yes | Hard to replace | Yes | Yes, tabletop 2025-11 | Unknown | High |

## 9. Worked example: a contract clause gap-check
| Clause | Required for all? | Required for critical? | Present? | Action |
|---|---|---|---|---|
| Data return on exit | Yes | Yes | No | Renegotiate at renewal |
| Audit and access rights | Base | Full and unrestricted | Partial | Add regulator access wording |
| TLPT cooperation | No | Yes | No | Add for critical-function contracts |
| Exit and transition period | Yes | Yes, with transition | No | Add a mandatory transition term |

## 10. Control objectives
| ID | Control objective |
|---|---|
| TPP-01 | A board-approved third-party strategy and critical-function policy exist. |
| TPP-02 | A complete register of information marks critical or important functions. |
| TPP-03 | Pre-contract due diligence covers risk, criticality, concentration, and conflicts. |
| TPP-04 | Contracts hold all required terms; enhanced terms apply to critical functions. |
| TPP-05 | Audit, access, and inspection rights are secured and used on a risk basis. |
| TPP-06 | Concentration and sub-outsourcing risks are assessed and monitored. |
| TPP-07 | Written, tested exit strategies exist for critical or important functions. |
| TPP-08 | CTPP status is tracked and reflected in risk management. |
| TPP-09 | The register is reported to the regulator at least once a year. |

## 11. Acceptance checklist (done when)
- The board has approved the third-party strategy and critical-function policy.
- The register is complete and reconciled to real spend, cloud, and SaaS.
- Each arrangement is flagged critical or not.
- Due diligence runs before any new contract.
- Existing contracts are reviewed and gaps (especially audit and exit) are being fixed.
- Exit plans for critical functions are written and tested.
- CTPP status is tracked and the register is submitted yearly.

## 12. Evidence to keep

The approved strategy and policy, the register (current and the versions sent to the regulator), due diligence records, contract gap analyses and signed contracts with the required terms, concentration and sub-outsourcing assessments, exit strategies and their test results, and records of the yearly register submission.

## 13. Common mistakes
- An incomplete register that misses SaaS, cloud, or intra-group services.
- Old contracts with no audit rights and no exit terms.
- Exit plans that were written but never tested, so they fail when needed.
- Ignoring concentration when many critical functions sit with one provider you cannot easily replace.

## 14. When you have no negotiating leverage (startups vs hyperscalers)

This is the part small firms find hardest and it is missing from most guidance.
DORA requires certain contract terms (audit rights, exit, regulator cooperation)
for critical-function providers — but a small startup often has near-zero
bargaining power against a hyperscale cloud provider or a large SaaS vendor who
will not edit their standard terms for a small customer. Here is how to comply
anyway.

**1. Use the provider's DORA package instead of bespoke redlines.** The major
cloud and SaaS providers publish a **DORA contractual addendum / financial
services amendment** that already contains the DORA-required clauses (audit and
access rights, sub-outsourcing transparency, incident cooperation, termination
and exit assistance, regulator access). You usually cannot rewrite their master
terms, but you **can** attach their DORA addendum. Ask for it by name; do not try
to draft your own from scratch.

**2. Accept "pooled" or third-party audit rights where direct audit is refused.**
DORA (Art. 30) allows audit and access rights to be exercised in proportionate
ways. Large providers rarely allow a small customer to send auditors on-site.
Acceptable substitutes to secure in the contract: pooled audits organised with
other customers, the provider's independent assurance reports (SOC 2 Type II,
ISO/IEC 27001, ISAE 3402), and third-party audit rights. Record in your file
**why** you relied on these (proportionality) rather than a direct audit.

**3. Manage what you cannot negotiate with architecture, not contract terms.**
If you cannot get strong exit terms, reduce lock-in technically: prefer portable
/ open formats, keep infrastructure-as-code, avoid single-provider proprietary
services for the most critical functions where a portable alternative exists, and
keep an independent, segregated backup you control. A tested technical exit is
worth more than an unenforceable contract clause.

**4. Treat concentration honestly.** A startup running everything on one
hyperscaler has real concentration risk it cannot fix by contract. Do not pretend
otherwise. Record it as an accepted, monitored risk with board sign-off, and
document your mitigations (multi-region, backups you control, a written exit
target even if slow).

**5. Escalate the residual gap to the board, do not hide it.** Where a required
term genuinely cannot be obtained, DORA expects you to assess the residual risk,
document it, and have the management body decide whether to accept it, mitigate
it, or not use the provider for that critical function. An honest, board-approved,
evidenced residual-risk decision is defensible; a silent gap is not.

**6. Time your leverage.** You have the most leverage at **renewal** and at
**new purchase**. Put the DORA addendum, exit terms, and audit-substitute wording
on the checklist **before** you sign or renew, not after. Track renewal dates in
the register so you never miss the one moment you can push.

Pass line for a small firm: for every critical-function provider you either hold
the DORA-required terms, or you hold a documented, proportionate substitute plus a
board-approved residual-risk decision, plus a technical mitigation for lock-in.

## 15. Quick self-check
- Does your register match your actual technology spend, including cloud and SaaS? If not, completeness is your first job.
- For your most important provider, do you have real audit rights (or a documented substitute) and a tested exit plan? If either is missing, that is a priority gap.
- Do you know which of your providers are CTPPs? If not, start tracking it.
- For any provider that refused your DORA terms, is there a board-approved residual-risk record and a technical lock-in mitigation? If not, that is your next task.
