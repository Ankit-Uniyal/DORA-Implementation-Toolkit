# Pillar 5 - Information and Intelligence Sharing

**DORA article:** Art. 45.

**Read first:** [Glossary](../glossary.md).

---

## 1. What this pillar is really about

Attackers often reuse the same tricks against many firms. If firms share what they see, everyone can defend faster. DORA encourages this sharing but does not force it. This is the one voluntary pillar. Even though it is optional, it is worth doing, because good threat sharing gives you early warning of attacks heading your way.

The plain idea: if your neighbour's house was just burgled using a new trick, you would want to know tonight, not next month.

## 2. What DORA allows (Art. 45)

Firms may share cyber threat information and intelligence with each other. This can include indicators of compromise (technical signs of an attack), attacker tactics and techniques, alerts, and tools. The sharing must:

- Aim to improve resilience: raising awareness, stopping threats spreading, improving detection and defence, or helping response and recovery.
- Happen inside trusted communities of financial firms.
- Run under proper arrangements that protect sensitive information, respect data protection law (the GDPR), and follow competition rules.

If you join or leave such an arrangement, you tell your regulator.

**What good looks like:** you belong to a trusted sharing community (for example, a sector information sharing group), you have a signed arrangement reviewed by legal and data protection, and the intelligence you receive is actually fed into your detection tools, not just read and forgotten.

**What weak looks like:** informal sharing over personal channels with no arrangement, which creates confidentiality and competition-law risk; or receiving intelligence and doing nothing with it.

## 3. Control objectives

| ID | Control objective |
|----|-------------------|
| ISH-01 | The decision to take part is written down and based on risk. |
| ISH-02 | Sharing happens in trusted communities under a formal arrangement. |
| ISH-03 | The arrangement protects confidentiality, personal data and competition rules. |
| ISH-04 | The regulator is told when you join or leave. |
| ISH-05 | Shared intelligence is actually used in detection and response. |

## 4. How to implement, in order

1. **Weeks 1 to 3:** Decide, based on risk, whether to take part. Write down the decision.
2. **Weeks 2 to 6:** Choose trusted communities and check their governance and handling rules (for example, the traffic-light protocol for how information can be shared onward).
3. **Weeks 4 to 8:** Put the arrangement in place with data protection, confidentiality, and competition safeguards. Get legal and DPO review.
4. **On joining:** Tell your regulator. Tell them again if you leave.
5. **Ongoing:** Feed received intelligence into your detection tools and threat processes, and contribute back where you can.

## 5. Sample artifact: intelligence intake row

| Date | Source community | Type | Summary | Action taken | Owner |
|------|------------------|------|---------|--------------|-------|
| 2025-07-01 | Sector sharing group | Indicators of compromise | New phishing domains | Added to email blocklist and SIEM | SOC lead |

## 6. Evidence to keep

The written participation decision and risk assessment, the signed sharing arrangement and its handling rules, the legal and DPO review, the notifications to your regulator, and records showing the intelligence was actually used.

## 7. Common mistakes

- Sharing outside a formal arrangement, creating legal risk.
- Receiving intelligence but never wiring it into detection.
- Forgetting to tell the regulator when membership changes.

## 8. Quick self-check

- If you take part, is there a signed arrangement with legal and data protection review? If not, formalise it.
- Does the threat intelligence you receive actually change what your defences block? If not, close the loop between intake and action.
