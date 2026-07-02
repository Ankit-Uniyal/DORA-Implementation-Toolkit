# Pillar 2 - ICT Incident Management, Classification and Reporting

**DORA articles:** Art. 17 to 23. Supplemented by the RTS on classification and the ITS on reporting content, templates and timelines.

**Read first:** [Glossary](../glossary.md). **Use with:** [Incident classification aid](../../templates/incident-classification-aid.md).

---

## 1. What this pillar is really about

Things will go wrong. DORA does not punish you for having incidents. It expects you to handle them well and, when they are serious, to tell your regulator quickly and honestly. The two hard parts are: deciding when an incident is "major" (classification), and reporting it inside tight deadlines. Both need to be worked out in advance, because in a real crisis you will not have time to figure them out from scratch.

The plain flow is: detect, log, classify, contain, recover, report, review.

## 2. The incident process (Art. 17)

You need one documented process to find, manage, and notify incidents. It must set roles, define severity levels, define escalation, and make sure serious incidents reach senior management.

**What good looks like:** a single runbook that anyone on call can follow at 3am. It names who classifies, who decides, who reports, and who talks to clients. It has clear severity levels and a clock that starts the moment an incident is called "major".

**What weak looks like:** an incident process that lives in someone's head, with no agreed way to decide severity and no pre-assigned reporting owner.

## 3. Classification: is it "major"? (Art. 18)

This is the decision that triggers mandatory reporting. DORA gives you seven things to look at. The exact thresholds live in the RTS and you must fill them in from the current official text.

The seven criteria:

1. **Clients, counterparts and transactions affected:** how many, and how important.
2. **Reputational impact:** media, complaints, regulator attention.
3. **Duration and downtime:** how long the disruption lasts.
4. **Geographical spread:** how many areas or countries are hit.
5. **Data losses:** harm to the availability, authenticity, integrity, or confidentiality of data.
6. **Criticality of services affected:** whether critical or important functions are hit.
7. **Economic impact:** direct and indirect costs.

An incident is "major" when it crosses the thresholds set in the RTS across these criteria. Use the [classification aid](../../templates/incident-classification-aid.md) so the decision is consistent every time.

> **Important warning about how to think about this.** Reporting a major incident on time is a hard legal duty, not a "nice to have". If you miss the deadline, you have breached DORA, even if everything else was handled well. Treat the reporting clock as the single most time-critical thing in this whole pillar.

## 4. Reporting a major incident (Art. 19 and 20)

Reporting happens in three stages:

1. **Initial notification:** a first alert soon after you classify the incident as major.
2. **Intermediate report:** an update when the situation changes in a meaningful way, and on further updates.
3. **Final report:** once you know the root cause and the actual impact.

> **The exact deadlines are set in the ITS.** They are measured in hours from set trigger points. You must take the current numbers from the official ITS and build your runbook around them. Do not guess. Confirm, then hard-code the deadlines into your process and your on-call rota.

You use standard forms and templates from the ITS. Line up your reporting fields to those forms so nothing is missing when the clock is running.

If clients are affected, tell them without undue delay and tell them what to do to protect themselves.

## 5. Voluntary threat notification (Art. 19)

You can, if you choose, tell your regulator about a significant cyber threat, even before it causes an incident. This is optional. Decide in advance who assesses threats and who makes that call.

## 6. Payment incidents (Art. 23)

The same rules also cover operational or security incidents linked to payments, for banks, payment firms, account information service providers, and e-money firms. Do not let payment incidents fall through a separate crack.

## 7. Control objectives

| ID | Control objective |
|----|-------------------|
| INC-01 | A documented process covers detection, logging, categorising, escalation and closure. |
| INC-02 | Classification applies the DORA and RTS criteria and thresholds consistently. |
| INC-03 | Roles and an escalation and on-call matrix are defined and tested. |
| INC-04 | Major incidents are reported inside the initial, intermediate and final deadlines. |
| INC-05 | Report content matches the ITS templates and is complete and accurate. |
| INC-06 | Affected clients are told without undue delay, with protective advice. |
| INC-07 | Significant cyber threats are assessed for voluntary notification. |
| INC-08 | Root-cause analysis feeds lessons learned and framework updates. |
| INC-09 | Payment-related incidents are captured under the same regime where relevant. |

## 8. How to implement, in order

1. **Weeks 1 to 3:** Write the incident process end to end, with a RACI and severity levels.
2. **Weeks 2 to 5:** Build the classification aid with the RTS criteria and thresholds filled in.
3. **Weeks 3 to 6:** Build the reporting runbook with the confirmed ITS deadlines and template fields. Pre-assign the reporting owner and backups.
4. **Weeks 4 to 8:** Set up logging and tooling so you can capture the incident timeline and evidence automatically.
5. **Weeks 5 to 9:** Write client and stakeholder communication templates with pre-agreed approvers.
6. **Weeks 8 to 12:** Run a tabletop exercise of a major incident, timed against the real deadlines. Fix whatever slows you down.
7. **Ongoing:** Post-incident reviews, and feed lessons back into controls.

## 9. Sample artifact: incident timeline (worked example)

| Time | Event | Action | Owner |
|------|-------|--------|-------|
| 09:12 | Monitoring alerts on failed logins spike | Triage opened | SOC analyst |
| 09:40 | Confirmed unauthorised access to a client system | Severity raised, incident manager paged | Incident manager |
| 10:15 | Classification aid run: crosses "major" threshold | Reporting clock started | Incident manager |
| 10:55 | Initial notification submitted to regulator | Filed and acknowledged | Reporting owner |
| Day 2 | Situation update | Intermediate report submitted | Reporting owner |
| Day 9 | Root cause confirmed, impact quantified | Final report submitted | Reporting owner |

Times are examples. The point is that the classification decision and the reporting clock are explicit and owned.

## 10. Evidence to keep

Incident process and RACI, the classification aid with worked examples, an incident register with full timelines, copies of initial, intermediate and final reports plus regulator acknowledgements, client notices, post-incident reviews, and exercise reports that prove you can hit the deadlines.

## 11. Common mistakes

- No agreed thresholds, so "major" is decided late or inconsistently.
- A reporting runbook that cannot meet the first deadline because ownership or escalation is slow.
- Poor logging, so the final report lacks accurate impact and root cause.
- Forgetting that payment security incidents are in scope.

## 12. Quick self-check

- If a major incident happened right now, do you know exactly who classifies it, who reports it, and by when? If any answer is "not sure", fix that before anything else.
- Have you ever run a timed exercise against the real reporting deadline? If not, do one soon. It is the fastest way to find the weak link.
