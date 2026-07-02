# Pillar 4 - ICT Third-Party Risk Management

**DORA articles:** Art. 28 to 44. Supplemented by the ITS on the register of information, the RTS on subcontracting, and the RTS on the policy for ICT services supporting critical or important functions.

**Read first:** [Glossary](../glossary.md). **Use with:** [Third-party register template](../../templates/third-party-register.md).

---

## 1. What this pillar is really about

Most firms now depend heavily on outside technology providers: cloud platforms, software vendors, data centres, managed services. If one of them fails or is breached, your firm feels it directly. DORA treats this outside risk as your risk. You cannot outsource the responsibility, only the activity.

There are two parts to this pillar:

- **What you must do** to manage your own providers.
- **The EU Oversight Framework**, where regulators directly supervise the biggest providers (called CTPPs).

## 2. Manage your providers (Art. 28)

You must:

- Have a board-approved strategy for third-party risk, and a specific policy for services that support critical or important functions.
- Keep a **register of information**: a full, up-to-date list of all your ICT contracts, marking which ones support critical or important functions. You report this to your regulator at least once a year.
- Do due diligence before you sign: check the provider, decide if the service is critical, look at concentration and conflicts of interest.
- Think about **concentration risk** (too much reliance on one provider) and the risk hidden in **sub-outsourcing** chains.
- Have a written, tested **exit strategy** for critical or important functions, so you can leave without disruption if you must.

**What good looks like:** a complete register that matches your actual spend and cloud usage, a clear line between "supports a critical function" and "does not", and exit plans that have actually been tested, not just written.

**What weak looks like:** a register that misses cloud services, SaaS tools, and intra-group arrangements; and exit plans that look fine on paper but have never been tried.

## 3. Concentration and sub-outsourcing (Art. 29)

Before relying on a provider for a critical function, ask:

- Could we easily replace this provider, or are we locked in?
- Do we have many critical functions sitting with the same provider or a closely linked group?
- Does the provider pass work down a chain, especially outside the EU, and can we still see and control the risk?

## 4. Contracts (Art. 30)

Every ICT contract must be written and must include a base set of terms: what the service is, where it runs and where data is held, data protection and data return on exit, service levels, help during incidents, cooperation with regulators, and termination rights.

Contracts for **critical or important functions** must include more: full service levels with clear targets, notice periods, the duty to follow your security and contingency requirements, cooperation with your TLPT, full rights of access, inspection and audit (for you and for regulators), and clear exit and transition terms.

**Plain-English tip:** the most common contract gaps are missing audit and access rights, and missing exit and transition terms. Check these first when reviewing existing contracts.

## 5. The Oversight Framework for CTPPs (Art. 31 to 44)

The ESAs name the most systemically important providers as Critical ICT Third-Party Providers (CTPPs) and oversee them directly. Each gets a Lead Overseer with real powers. Your job as a firm is to know whether your providers are CTPPs, factor that into your risk view, and be ready to act (including suspending or ending a service) if a CTPP ignores the oversight recommendations.

## 6. Control objectives

| ID | Control objective |
|----|-------------------|
| TPP-01 | A board-approved third-party strategy and critical-function policy exist. |
| TPP-02 | A complete register of information marks critical or important functions. |
| TPP-03 | Pre-contract due diligence covers risk, criticality, concentration and conflicts. |
| TPP-04 | Contracts hold all required terms; enhanced terms apply to critical functions. |
| TPP-05 | Audit, access and inspection rights are secured and used on a risk basis. |
| TPP-06 | Concentration and sub-outsourcing risks are assessed and monitored. |
| TPP-07 | Written, tested exit strategies exist for critical or important functions. |
| TPP-08 | CTPP status is tracked and reflected in risk management. |
| TPP-09 | The register is reported to the regulator at least once a year. |

## 7. How to implement, in order

1. **Weeks 1 to 3:** Get the board to approve the third-party strategy and critical-function policy.
2. **Weeks 2 to 8:** Build the register of information using the template. Reconcile it against accounts payable and your cloud and SaaS inventory so nothing is missing.
3. **Weeks 4 to 10:** Mark each arrangement as supporting a critical function or not.
4. **Weeks 6 to 12:** Set up due diligence for new contracts.
5. **Weeks 8 to 16:** Review existing contracts against the required terms. Fix gaps, especially audit rights and exit terms.
6. **Weeks 12 to 20:** Write and then test exit strategies for critical functions.
7. **Ongoing:** Monitor SLAs, incidents, sub-outsourcing changes, and CTPP status. Report the register yearly.

## 8. Sample artifact: a register row (short form)

| Provider | Service | Supports critical function? | Substitutable? | Audit rights? | Exit tested? | CTPP? | Risk |
|----------|---------|-----------------------------|----------------|---------------|--------------|-------|------|
| CloudCo | Payments hosting | Yes | Hard to replace | Yes | Yes, tabletop 2025-11 | Unknown | High |

## 9. Sample artifact: a contract clause gap-check

| Clause | Required for all? | Required for critical? | Present? | Action |
|--------|-------------------|------------------------|----------|--------|
| Data return on exit | Yes | Yes | No | Renegotiate at renewal |
| Audit and access rights | Base | Full and unrestricted | Partial | Add regulator access wording |
| TLPT cooperation | No | Yes | No | Add for critical-function contracts |
| Exit and transition period | Yes | Yes, with transition | No | Add mandatory transition term |

## 10. Evidence to keep

The approved strategy and policy, the register (current and the versions sent to the regulator), due diligence records, contract gap analyses and signed contracts with the required terms, concentration and sub-outsourcing assessments, exit strategies and their test results, and records of the yearly register submission.

## 11. Common mistakes

- An incomplete register that misses SaaS, cloud, or intra-group services.
- Old contracts with no audit rights and no exit terms.
- Exit plans that were written but never tested, so they fail when needed.
- Ignoring concentration when many critical functions sit with one provider you cannot easily replace.

## 12. Quick self-check

- Does your register match your actual technology spend, including cloud and SaaS? If not, completeness is your first job.
- For your most important provider, do you have real audit rights and a tested exit plan? If either is missing, that is a priority gap.
- Do you know which of your providers are CTPPs? If not, start tracking it.
