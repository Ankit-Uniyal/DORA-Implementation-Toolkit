# Pillar 1: ICT Risk Management (Playbook)

DORA articles: Art. 5 to 16. Supplemented by the RTS on the ICT risk management framework and the RTS on the simplified framework.

Read first: Glossary and Proportionality guide. Use with: ICT asset register template, Policy register template.

This is a playbook. It gives you the steps, the order, the owner for each step, ready-to-copy artifacts, and worked examples so you can build ICT risk management from scratch. Plain English, no em dashes.

## At a glance

| Item | Detail |
|---|---|
| Goal | Know your technology, protect it, detect trouble, recover fast, and keep improving. |
| Who leads | CISO or Head of ICT Risk, sponsored by the accountable board member. |
| Typical time | 20 to 24 weeks to build the core; then ongoing. |
| Main outputs | Framework doc, asset inventory, risk register, security standards, detection setup, recovery plans with RTO and RPO, tested backups. |
| Done when | You can list critical functions and systems in an hour, and you have proven a restore inside its RTO. |

## 1. What this pillar is really about

This pillar is the foundation. Everything else in DORA sits on top of it. It asks one question: do you know what technology you depend on, and can you protect it, spot trouble, and recover when something breaks?

DORA breaks that into five jobs that repeat forever in a loop: Identify, Protect, Detect, Respond and recover, and Learn. If you can show you do all five, consistently, with evidence, you are most of the way to meeting this pillar.

## 2. Before you start (prerequisites)

- Governance in place from Pillar 0 (a named owner and a way to get board approval).
- A list of your top business functions (start rough, refine as you go).
- Access to procurement, cloud, and IT asset data so your inventory can be complete.
- A copy of the ICT asset register template and the policy register template.

## 3. Step-by-step build

Step 1: Draft the framework and risk appetite. Owner: CISO. Write one short, version-controlled framework document. State risk appetite, name the owner, and list the policies underneath it. Output: a draft framework for board approval.

Step 2: Build the asset and dependency inventory. Owner: IT asset owner. Start with critical functions. For each function, record the systems, data, and outside providers it needs. Reconcile against procurement and cloud bills to catch shadow IT. Output: a live inventory (use the template).

Step 3: Run the first risk assessment. Owner: Risk. Use one repeatable method (see the worked register below). Score likelihood and impact, list current controls, and record a rating and an owner for each risk. Output: a current risk register.

Step 4: Write the security control standards. Owner: CISO. Turn your security policy into clear standards people can follow (see the ready-to-use list below). Output: approved control standards.

Step 5: Set up detection. Owner: SOC or IT Ops. Turn on logging for critical systems, set alert thresholds, and name the team that acts on alerts. Output: logging and alerting live, with sample alerts.

Step 6: Define recovery targets and plans. Owner: Continuity lead. Agree RTO and RPO per critical function with the business. Write response and recovery plans that name who does what. Output: signed RTO and RPO and recovery plans.

Step 7: Set up and test backups. Owner: IT Ops. Back up by criticality, keep backups separate from live systems, and run a real restore test. Output: a restore-test report proving recovery inside the RTO.

Step 8: Close the loop with learning. Owner: CISO. Set up post-incident reviews, take in threat intelligence, and run role-based training. Output: a lessons-learned process and training records.

## 4. The five jobs, with what good looks like

Identify (Art. 8). Keep a live inventory linking each critical system to its function, owner, recovery targets, and third parties. Risk assessments are repeatable and recorded, not from memory. Concrete first step: list your top 10 business functions and, for each, the systems, data, and providers it needs. That one table exposes most of your real risk on day one.

Protect (Art. 9). Written control standards that say exactly what is expected, enforced and checked. DORA does not invent new security controls. If you already run a recognised security standard well, most of your protection work is done. The gap is usually proving it and linking it to critical functions.

Detect (Art. 10). Logging on critical systems, alerts to a named team, defined thresholds, and evidence that alerts are acted on.

Respond and recover (Art. 11 and 12). Each critical function has an agreed RTO and RPO, plans that name who does what, and test reports proving a real restore worked inside the target time. Backups are isolated so one ransomware attack cannot destroy both live data and backups.

Learn (Art. 13 and 14). Every significant incident has a written review with actions tracked to closure. Training completion is recorded, including for the board. A crisis communication plan is ready.

## 5. Ready-to-use artifact: security control standards (starter list)

Copy this list and set your own numbers where brackets appear. These are common, sensible defaults, not legal minimums.

- Access control: least privilege; access reviewed every [90] days; joiners, movers, and leavers processed within [1] business day.
- Strong authentication: multi-factor authentication required for all remote and administrative access.
- Encryption: data encrypted in transit; sensitive data encrypted at rest.
- Patching: critical security patches applied within [14] days; high within [30] days.
- Change management: all production changes recorded and approved; emergency changes reviewed after the fact.
- Secure configuration: systems built from hardened baselines; default credentials removed.
- Logging: security logs kept for at least [12] months and protected from tampering.
- Backup: backups run by criticality, kept separate, and restore-tested at least [yearly].

## 6. Worked example: RTO and RPO tiering

| Tier | Example functions | RTO (max downtime) | RPO (max data loss) |
|---|---|---|---|
| 1 Critical | Payments, trading, customer access | 2 hours | 15 minutes |
| 2 Important | Reporting, reconciliation | 8 hours | 4 hours |
| 3 Standard | Internal admin tools | 48 hours | 24 hours |

These numbers are examples. Set your own from real business impact, then prove them by testing.

## 7. Worked example: restore-test drill (steps to copy)

1. Pick a Tier 1 system and its latest backup.
2. Restore it to an isolated environment. Start a timer.
3. Check the data is complete and correct against the RPO.
4. Confirm the system works (a short function test).
5. Stop the timer. Compare the elapsed time to the RTO.
6. Record the result, any gaps, and fixes. Re-test after fixes.

Pass line: the restore completed inside the RTO and lost no more than the RPO allows, with a report to prove it.

## 8. Worked example: a filled-in risk register row

| Risk ID | Risk | Affected function | Likelihood | Impact | Current controls | Rating | Owner | Action |
|---|---|---|---|---|---|---|---|---|
| R-011 | Ransomware encrypts core banking data | Customer accounts | Medium | Severe | Segregated backups, EDR, MFA | High | CISO | Test restore quarterly; run a tabletop |

## 9. Control objectives

| ID | Control objective |
|---|---|
| RM-01 | A board-approved resilience strategy defines risk appetite and objectives. |
| RM-02 | A complete, current inventory of functions, assets, and dependencies is maintained. |
| RM-03 | ICT risks are assessed regularly and on major change. |
| RM-04 | An information security policy and supporting controls are implemented and enforced. |
| RM-05 | Detection with defined thresholds identifies anomalies and incidents promptly. |
| RM-06 | Continuity and recovery plans exist with tested RTO and RPO. |
| RM-07 | Backups are segregated and restoration is tested. |
| RM-08 | Post-incident reviews and threat intelligence drive improvement. |
| RM-09 | Awareness and resilience training runs for all staff and the board. |
| RM-10 | The framework is reviewed at least yearly and after major incidents. |

## 10. Acceptance checklist (done when)

- [ ] The board has approved the framework and risk appetite.
- [ ] The inventory covers all critical functions and links each to owner, recovery targets, and third parties.
- [ ] A current risk register exists from a repeatable method.
- [ ] Control standards are approved and enforced, with checks.
- [ ] Logging and alerting are live on critical systems.
- [ ] RTO and RPO are agreed for every critical function and a real restore was tested inside the RTO.
- [ ] Backups are segregated and a restore report exists.
- [ ] Post-incident reviews and role-based training are running.

## 11. Evidence to keep

Approved strategy and framework (with version history), asset inventory extract, risk method and register, security policy and standards, alert configuration and sample alerts, continuity plans with RTO and RPO, restore-test reports, post-incident reviews, training records, and the annual review minutes.

## 12. Common mistakes

- An asset inventory that misses shadow IT, hidden dependencies, or third-party links.
- RTO and RPO written on paper but never proven by a real restore test.
- Backups that sit on the same network as production, so one attack destroys both.
- An "annual review" that is a rubber stamp, not a real reassessment.
- Generic training instead of role-based training that matches real risk.

## 13. Quick self-check

- Can you produce, in one hour, a list of your critical functions and the systems behind them? If not, start with the inventory.
- Have you ever proven, with a report, that you can restore a critical system inside its RTO? If not, that is your top priority.
- Did the board approve the framework this year, with minutes to show it? If not, fix the governance gap first.
