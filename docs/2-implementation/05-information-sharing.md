# Pillar 5: Information and Intelligence Sharing (Playbook)

DORA article: Art. 45.

Read first: Glossary.

This is a playbook. It gives you a decision path, a joining checklist, a safeguards checklist, and a way to turn intelligence into action. Plain English, no em dashes. This is the one voluntary pillar, but it is worth doing well.

## At a glance

| Item | Detail |
|---|---|
| Goal | Get early warning of attacks by sharing threat information safely with trusted peers. |
| Who leads | CISO or Threat Intelligence lead, with Legal and the Data Protection Officer. |
| Typical time | 8 weeks to join and wire in; then ongoing. |
| Main outputs | A written participation decision, a signed arrangement, a regulator notification, and intel feeding your defences. |
| Done when | You belong to a trusted community under a reviewed arrangement, and the intel you receive changes what your defences block. |

## 1. What this pillar is really about

Attackers often reuse the same tricks against many firms. If firms share what they see, everyone defends faster. DORA encourages this but does not force it. Even though it is optional, it is worth doing, because good threat sharing gives early warning of attacks heading your way.

The plain idea: if your neighbour's house was just burgled using a new trick, you would want to know tonight, not next month.

## 2. Before you start (prerequisites)

- A working detection setup from Pillar 1, so received intelligence has somewhere to go.
- Legal and Data Protection Officer support for the arrangement.
- A view of which trusted communities fit your sector.

## 3. What DORA allows (Art. 45)

Firms may share cyber threat information and intelligence: indicators of compromise (technical signs of an attack), attacker tactics and techniques, alerts, and tools. The sharing must aim to improve resilience, happen inside trusted communities of financial firms, and run under proper arrangements that protect sensitive information, respect data protection law (the GDPR), and follow competition rules. If you join or leave such an arrangement, you tell your regulator.

## 4. Decision path: should you take part?

1. Assess the benefit: would earlier warning of sector threats reduce your real risk? For most firms, yes.
2. Assess the cost and risk: can you handle the intel, and can you meet the confidentiality, data protection, and competition rules?
3. Decide and write it down, with the reasoning. This written decision is itself evidence.
4. If yes, go to the joining steps. If no, record why and revisit later.

## 5. Step-by-step: joining and using a community

Step 1: Choose the community. Owner: CISO. Pick a trusted community (for example a sector sharing group). Check its governance and handling rules, including the traffic-light protocol for how information can be passed on. Output: a shortlisted community.

Step 2: Put the arrangement in place. Owner: Legal and DPO. Sign an arrangement with confidentiality, data protection, and competition safeguards. Output: a signed, reviewed arrangement.

Step 3: Notify the regulator. Owner: Compliance. Tell your regulator that you have joined. Tell them again if you leave. Output: a notification record.

Step 4: Wire intel into detection. Owner: SOC. Feed received indicators into your blocklists and monitoring tools. Output: intel that actually changes what you block.

Step 5: Contribute back. Owner: SOC. Share what you safely can, following the handling rules. Output: a two-way relationship.

## 6. Ready-to-use artifact: safeguards checklist

- Confidentiality: the arrangement limits who can see shared data and how it is stored.
- Data protection: personal data is handled per the GDPR; the DPO has reviewed it.
- Competition: the arrangement avoids sharing anything that could breach competition law.
- Handling rules: a clear protocol (for example traffic-light) for onward sharing.
- Legal review: signed off by legal before joining.

## 7. Worked example: intelligence intake row

| Date | Source community | Type | Summary | Action taken | Owner |
|---|---|---|---|---|---|
| 2025-07-01 | Sector sharing group | Indicators of compromise | New phishing domains | Added to email blocklist and SIEM | SOC lead |

## 8. Control objectives

| ID | Control objective |
|---|---|
| ISH-01 | The decision to take part is written down and based on risk. |
| ISH-02 | Sharing happens in trusted communities under a formal arrangement. |
| ISH-03 | The arrangement protects confidentiality, personal data, and competition rules. |
| ISH-04 | The regulator is told when you join or leave. |
| ISH-05 | Shared intelligence is actually used in detection and response. |

## 9. Acceptance checklist (done when)

- [ ] A written, risk-based participation decision exists.
- [ ] You belong to a trusted community under a signed arrangement.
- [ ] Legal and the DPO have reviewed the arrangement.
- [ ] The regulator has been told you joined (and will be told if you leave).
- [ ] Received intelligence is wired into your detection tools.

## 10. Evidence to keep

The written participation decision and risk assessment, the signed sharing arrangement and its handling rules, the legal and DPO review, the notifications to your regulator, and records showing the intelligence was actually used.

## 11. Common mistakes

- Sharing outside a formal arrangement, creating legal risk.
- Receiving intelligence but never wiring it into detection.
- Forgetting to tell the regulator when membership changes.

## 12. Quick self-check

- If you take part, is there a signed arrangement with legal and data protection review? If not, formalise it.
- Does the threat intelligence you receive actually change what your defences block? If not, close the loop between intake and action.
