# Pillar 2: ICT Incident Management, Classification and Reporting (Playbook)

DORA articles: Art. 17 to 23. Supplemented by the **Classification RTS
(Commission Delegated Regulation (EU) 2024/1772)** and the **Reporting RTS
(Commission Delegated Regulation (EU) 2025/301)** on report content and time
limits.

Read first: Glossary. Use with: Incident classification aid and
docs/regulatory-references.md (the real thresholds and deadlines live there).

This is a playbook. It gives you a ready-to-use incident runbook, a RACI, comms
templates, a worked timeline, and a tabletop script. The RTS thresholds for
"major" and the reporting deadlines are now **filled in from the official text**
(verified 3 July 2026); confirm them against EUR-Lex before you go live and keep
docs/regulatory-references.md as the single source of truth.

## At a glance
| Item | Detail |
|---|---|
| Goal | Detect, handle, and report incidents well, and hit the reporting deadlines for major ones. |
| Who leads | Incident Manager, with a pre-named Reporting Owner. |
| Typical time | 12 weeks to stand up; then always ready. |
| Main outputs | Incident runbook, classification aid, reporting runbook, comms templates, tested on-call rota. |
| Done when | You can name who classifies, who reports, and by when, and a timed exercise proves you can hit the first deadline. |

## 1. What this pillar is really about

Things will go wrong. DORA does not punish you for having incidents. It expects
you to handle them well and, when they are serious, to tell your regulator
quickly and honestly. The two hard parts are deciding when an incident is "major"
(classification) and reporting it inside tight deadlines. Both must be worked out
in advance, because in a real crisis you will not have time to figure them out
from scratch.

The plain flow is: detect, log, classify, contain, recover, report, review.

**Important.** Reporting a major incident on time is a hard legal duty. If you
miss the deadline you have breached DORA, even if everything else was handled
well. Treat the reporting clock as the single most time-critical thing here.

## 2. Before you start (prerequisites)
- Detection and logging from Pillar 1 (so you can see incidents and build a timeline).
- A named Incident Manager and a named Reporting Owner, each with a backup.
- The classification thresholds (RTS 2024/1772) and reporting deadlines (RTS 2025/301) — already summarised in docs/regulatory-references.md.
- The Incident classification aid template (now pre-filled with the real thresholds).

## 3. Ready-to-use incident runbook (copy and fill)

Anyone on call should be able to follow this at 3am.

**Step 1: Detect and open.** Whoever spots it opens a ticket and pages the on-call
lead. Capture time, what is affected, and first symptoms.

**Step 2: Triage and set severity.** On-call lead sets an initial severity (for
example Sev1 to Sev3) and pages the Incident Manager for high severities.

**Step 3: Classify (is it major?).** Incident Manager runs the classification aid
against the seven criteria and the RTS thresholds. If it crosses the line, declare
"major" and start the reporting clock. Write down the exact time you declared it.

**Step 4: Contain and recover.** The technical team contains the issue and starts
recovery using the Pillar 1 recovery plans. Keep a running timeline.

**Step 5: Report (if major).** The Reporting Owner submits the initial,
intermediate, and final reports inside the deadlines in section 6, using the
report content fields from Reporting RTS 2025/301.

**Step 6: Notify clients (if affected).** Send the client notice without undue
delay, with protective advice, using the pre-approved template.

**Step 7: Close and review.** Confirm recovery, close the incident, and run a
post-incident review. Feed actions back into controls.

## 4. Ready-to-use artifact: incident RACI
| Activity | On-call lead | Incident Manager | Reporting Owner | Tech team | Comms | Board |
|---|---|---|---|---|---|---|
| Open and triage | R | A | I | C | I | I |
| Classify as major | C | A/R | C | C | I | I |
| Contain and recover | I | A | I | R | I | I |
| Report to regulator | I | C | A/R | C | C | I |
| Notify clients | I | A | C | I | R | I |
| Post-incident review | C | A/R | C | C | C | I |

## 5. Classification: is it "major"? (Art. 18, RTS 2024/1772)

This decision triggers mandatory reporting. An incident is **major** when it
**has affected critical services** AND either the **data-losses** trigger is met,
or **two or more** of the other thresholds are met (RTS Art. 8).

The seven criteria and their **real thresholds**:

| # | Criterion | Threshold that counts as "met" |
|---|---|---|
| 1 | Clients, counterparts, transactions | > 10% of clients, or > 100 000 clients; or > 30% of counterparts; or > 10% of daily transaction number or value; or a "relevant" client/counterpart |
| 2 | Reputational impact | media coverage; repeat complaints; likely regulatory breach; likely material client loss |
| 3 | Duration and downtime | duration > 24 hours; or downtime > 2 hours for critical-function services |
| 4 | Geographical spread | impact in 2 or more Member States |
| 5 | Data losses | impact on availability/authenticity/integrity/confidentiality harming objectives or compliance; or successful malicious unauthorised access that may cause data loss |
| 6 | Criticality of services (the gate) | affects systems behind critical/important functions; or supervised services; or a successful malicious unauthorised access |
| 7 | Economic impact | costs and losses exceed, or are likely to exceed, EUR 100 000 |

Use the classification aid so the decision is consistent every time. Full detail
and citations in docs/regulatory-references.md.

## 6. Reporting a major incident (Art. 19 and 20, RTS 2025/301)

Reporting happens in three stages with **binding deadlines**:

| Stage | What it is | Deadline |
|---|---|---|
| Initial notification | First alert after you classify it as major | Within **4 hours** of classifying as major, and no later than **24 hours** from awareness |
| Intermediate report | Update on the situation | Within **72 hours** of the initial notification (update again once regular activities recover) |
| Final report | Root cause and actual impact known | Within **1 month** of the intermediate report |

Build these rules into the runbook too:

- **Late classification:** if you classify as major more than 24 hours after
  awareness, the 4-hour initial clock runs from the moment of classification.
- **Cannot meet a deadline:** tell the competent authority **before** it passes
  and explain the delay (RTS 2025/301 Art. 5(3)). Do not go silent.
- **Weekends/bank holidays:** you may submit by noon of the next working day —
  but **not** if you are a credit institution, CCP, trading-venue operator, or a
  NIS2 essential/important entity (Art. 5(4) to (6)).

Use the report content fields set out in RTS 2025/301 Art. 1 to 4 (summarised in
docs/regulatory-references.md, section 4). If clients are affected, tell them
without undue delay and how to protect themselves.

## 7. Voluntary threat notification (Art. 19) and payment incidents (Art. 23)

You may voluntarily tell your regulator about a **significant cyber threat**
before it causes an incident (see the RTS Art. 10 test in the classification aid).
Decide in advance who assesses threats and who makes that call. Also remember that
operational or security incidents linked to **payments** (for banks, payment
firms, account information service providers, and e-money firms) are covered by
the same regime. Do not let payment incidents fall through a separate crack.

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
| 12:30 | Initial notification submitted (well inside the 4-hour window) | Filed and acknowledged | Reporting Owner |
| Day 2 | Situation update | Intermediate report submitted (within 72h) | Reporting Owner |
| Day 20 | Root cause confirmed, impact quantified | Final report submitted (within 1 month) | Reporting Owner |

Times are examples. The point is that the classification decision and the
reporting clock are explicit, owned, and comfortably inside the legal deadlines.

## 10. Ready-to-use artifact: tabletop exercise script

Run this at least yearly, timed against the real deadlines.

- Set the scene: read out a realistic scenario (for example ransomware on a payment system).
- Inject facts every few minutes so the picture changes.
- Ask the team to classify: is it major? Time how long the decision takes.
- Start the reporting clock at the moment they declare "major".
- Have the Reporting Owner draft the initial notification against the real 4-hour deadline.
- Debrief: did you hit the first deadline? Where was the slow point? Assign fixes with owners and dates.

## 11. Control objectives
| ID | Control objective |
|---|---|
| INC-01 | A documented process covers detection, logging, categorising, escalation, and closure. |
| INC-02 | Classification applies the DORA and RTS 2024/1772 criteria and thresholds consistently. |
| INC-03 | Roles and an escalation and on-call matrix are defined and tested. |
| INC-04 | Major incidents are reported inside the 4h / 72h / 1-month deadlines (RTS 2025/301). |
| INC-05 | Report content matches the RTS 2025/301 fields and is complete and accurate. |
| INC-06 | Affected clients are told without undue delay, with protective advice. |
| INC-07 | Significant cyber threats are assessed for voluntary notification. |
| INC-08 | Root-cause analysis feeds lessons learned and framework updates. |
| INC-09 | Payment-related incidents are captured under the same regime where relevant. |

## 12. Acceptance checklist (done when)
- The incident runbook exists with a RACI and severity levels.
- The classification aid has the RTS 2024/1772 thresholds (it now does).
- The reporting runbook has the 4h / 72h / 1-month deadlines and a pre-named Reporting Owner with a backup.
- Logging captures a full incident timeline automatically.
- Client and stakeholder comms templates are pre-approved.
- A timed tabletop has proven you can meet the first deadline.

## 13. Evidence to keep

Incident process and RACI, the classification aid with worked examples, an
incident register with full timelines, copies of initial, intermediate, and final
reports plus regulator acknowledgements, client notices, post-incident reviews,
and exercise reports that prove you can hit the deadlines.

## 14. Common mistakes
- No agreed thresholds, so "major" is decided late or inconsistently. (The aid now fixes this.)
- A reporting runbook that cannot meet the 4-hour first deadline because ownership or escalation is slow.
- Poor logging, so the final report lacks accurate impact and root cause.
- Forgetting that payment security incidents are in scope.
- Going silent when a deadline will be missed instead of notifying the authority first (Art. 5(3)).

## 15. Quick self-check
- If a major incident happened right now, do you know exactly who classifies it, who reports it, and by when? If any answer is "not sure", fix that before anything else.
- Have you ever run a timed exercise against the real 4-hour deadline? If not, do one soon. It is the fastest way to find the weak link.
