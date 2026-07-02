# Pillar 2: ICT Incident Management, Classification and Reporting (Playbook)

DORA articles: Art. 17 to 23. Supplemented by the RTS on classification and the ITS on reporting content, templates, and timelines.

Read first: Glossary. Use with: Incident classification aid.

This is a playbook. It gives you a ready-to-use incident runbook, a RACI, comms templates, a worked timeline, and a tabletop script. Plain English, no em dashes. The one thing you must confirm yourself: the RTS thresholds for "major" and the ITS reporting deadlines in hours. Those are set in official text. Fill them into the brackets marked [from RTS] and [from ITS] before you go live.

## At a glance

| Item | Detail |
|---|---|
| Goal | Detect, handle, and report incidents well, and hit the reporting deadlines for major ones. |
| Who leads | Incident Manager, with a pre-named Reporting Owner. |
| Typical time | 12 weeks to stand up; then always ready. |
| Main outputs | Incident runbook, classification aid, reporting runbook, comms templates, tested on-call rota. |
| Done when | You can name who classifies, who reports, and by when, and a timed exercise proves you can hit the first deadline. |

## 1. What this pillar is really about

Things will go wrong. DORA does not punish you for having incidents. It expects you to handle them well and, when they are serious, to tell your regulator quickly and honestly. The two hard parts are deciding when an incident is "major" (classification) and reporting it inside tight deadlines. Both must be worked out in advance, because in a real crisis you will not have time to figure them out from scratch.

The plain flow is: detect, log, classify, contain, recover, report, review.

Important. Reporting a major incident on time is a hard legal duty, not a nice-to-have. If you miss the deadline you have breached DORA, even if everything else was handled well. Treat the reporting clock as the single most time-critical thing in this pillar.

## 2. Before you start (prerequisites)

- Detection and logging from Pillar 1 (so you can see incidents and build a timeline).
- A named Incident Manager and a named Reporting Owner, each with a backup.
- The current RTS classification thresholds and ITS reporting deadlines confirmed from official text.
- The Incident classification aid template.

## 3. Ready-to-use incident runbook (copy and fill)

Anyone on call should be able to follow this at 3am.

Step 1: Detect and open. Whoever spots it opens a ticket and pages the on-call lead. Capture time, what is affected, and first symptoms.

Step 2: Triage and set severity. On-call lead sets an initial severity (for example Sev1 to Sev3) and pages the Incident Manager for high severities.

Step 3: Classify (is it major?). Incident Manager runs the classification aid against the seven criteria and the RTS thresholds. If it crosses the line, declare "major" and start the reporting clock. Write down the exact time you declared it.

Step 4: Contain and recover. The technical team contains the issue and starts recovery using the Pillar 1 recovery plans. Keep a running timeline.

Step 5: Report (if major). The Reporting Owner submits the initial, intermediate, and final reports inside the ITS deadlines, using the ITS template fields.

Step 6: Notify clients (if affected). Send the client notice without undue delay, with protective advice, using the pre-approved template.

Step 7: Close and review. Confirm recovery, close the incident, and run a post-incident review. Feed actions back into controls.

## 4. Ready-to-use artifact: incident RACI

| Activity | On-call lead | Incident Manager | Reporting Owner | Tech team | Comms | Board |
|---|---|---|---|---|---|---|
| Open and triage | R | A | I | C | I | I |
| Classify as major | C | A/R | C | C | I | I |
| Contain and recover | I | A | I | R | I | I |
| Report to regulator | I | C | A/R | C | C | I |
| Notify clients | I | A | C | I | R | I |
| Post-incident review | C | A/R | C | C | C | I |

## 5. Classification: is it "major"? (Art. 18)

This decision triggers mandatory reporting. DORA gives you seven things to look at. The exact thresholds live in the RTS, so fill them in.

The seven criteria: clients, counterparts, and transactions affected; reputational impact; duration and downtime; geographical spread; data losses; criticality of services affected; economic impact.

An incident is "major" when it crosses the RTS thresholds across these criteria. Use the classification aid so the decision is consistent every time.

## 6. Reporting a major incident (Art. 19 and 20)

Reporting happens in three stages, each with a deadline set in the ITS. Fill in the confirmed numbers and hard-code them into your runbook and on-call rota.

| Stage | What it is | Deadline (fill in) |
|---|---|---|
| Initial notification | First alert soon after you classify it as major | [from ITS] |
| Intermediate report | Update when the situation changes meaningfully | [from ITS] |
| Final report | Once root cause and actual impact are known | [from ITS] |

Use the standard ITS forms. Line up your reporting fields to those forms so nothing is missing when the clock is running. If clients are affected, tell them without undue delay and tell them how to protect themselves.

## 7. Voluntary threat notification (Art. 19) and payment incidents (Art. 23)

You may, if you choose, tell your regulator about a significant cyber threat before it causes an incident. Decide in advance who assesses threats and who makes that call. Also remember that operational or security incidents linked to payments (for banks, payment firms, account information service providers, and e-money firms) are covered by the same regime. Do not let payment incidents fall through a separate crack.

## 8. Ready-to-use artifact: client notification template (outline)

- What happened, in plain words, and when.
- What it means for you (the client).
- What we are doing about it.
- What you should do now to protect yourself (for example, watch for phishing, reset a password).
- Where to get help (contact details).
- We will update you by [time or channel].

Get this template pre-approved by legal and comms so it can go out fast.

## 9. Worked example: incident timeline

| Time | Event | Action | Owner |
|---|---|---|---|
| 09:12 | Alert on a spike in failed logins | Triage opened | SOC analyst |
| 09:40 | Confirmed unauthorised access to a client system | Severity raised, Incident Manager paged | Incident Manager |
| 10:15 | Classification aid run, crosses "major" | Reporting clock started | Incident Manager |
| 10:55 | Initial notification submitted | Filed and acknowledged | Reporting Owner |
| Day 2 | Situation update | Intermediate report submitted | Reporting Owner |
| Day 9 | Root cause confirmed, impact quantified | Final report submitted | Reporting Owner |

Times are examples. The point is that the classification decision and the reporting clock are explicit and owned.

## 10. Ready-to-use artifact: tabletop exercise script

Run this at least yearly, timed against the real deadlines.

1. Set the scene: read out a realistic scenario (for example ransomware on a payment system).
2. Inject facts every few minutes so the picture changes.
3. Ask the team to classify: is it major? Time how long the decision takes.
4. Start the reporting clock at the moment they declare "major".
5. Have the Reporting Owner draft the initial notification against the real deadline.
6. Debrief: did you hit the first deadline? Where was the slow point? Assign fixes with owners and dates.

## 11. Control objectives

| ID | Control objective |
|---|---|
| INC-01 | A documented process covers detection, logging, categorising, escalation, and closure. |
| INC-02 | Classification applies the DORA and RTS criteria and thresholds consistently. |
| INC-03 | Roles and an escalation and on-call matrix are defined and tested. |
| INC-04 | Major incidents are reported inside the initial, intermediate, and final deadlines. |
| INC-05 | Report content matches the ITS templates and is complete and accurate. |
| INC-06 | Affected clients are told without undue delay, with protective advice. |
| INC-07 | Significant cyber threats are assessed for voluntary notification. |
| INC-08 | Root-cause analysis feeds lessons learned and framework updates. |
| INC-09 | Payment-related incidents are captured under the same regime where relevant. |

## 12. Acceptance checklist (done when)

- [ ] The incident runbook exists with a RACI and severity levels.
- [ ] The classification aid has the current RTS thresholds filled in.
- [ ] The reporting runbook has the confirmed ITS deadlines and a pre-named Reporting Owner with a backup.
- [ ] Logging captures a full incident timeline automatically.
- [ ] Client and stakeholder comms templates are pre-approved.
- [ ] A timed tabletop has proven you can meet the first deadline.

## 13. Evidence to keep

Incident process and RACI, the classification aid with worked examples, an incident register with full timelines, copies of initial, intermediate, and final reports plus regulator acknowledgements, client notices, post-incident reviews, and exercise reports that prove you can hit the deadlines.

## 14. Common mistakes

- No agreed thresholds, so "major" is decided late or inconsistently.
- A reporting runbook that cannot meet the first deadline because ownership or escalation is slow.
- Poor logging, so the final report lacks accurate impact and root cause.
- Forgetting that payment security incidents are in scope.

## 15. Quick self-check

- If a major incident happened right now, do you know exactly who classifies it, who reports it, and by when? If any answer is "not sure", fix that before anything else.
- Have you ever run a timed exercise against the real reporting deadline? If not, do one soon. It is the fastest way to find the weak link.
