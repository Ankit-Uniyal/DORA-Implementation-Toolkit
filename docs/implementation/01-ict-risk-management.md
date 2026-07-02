# Pillar 1 - ICT Risk Management

**DORA articles:** Art. 5 to 16. Supplemented by the RTS on the ICT risk management framework and the RTS on the simplified framework.

**Read first:** [Glossary](../glossary.md) and [Proportionality guide](../proportionality-guide.md).

---

## 1. What this pillar is really about

This pillar is the foundation. Everything else in DORA sits on top of it. In plain terms it asks one question: do you know what technology you depend on, and can you protect it, spot trouble, and recover when something breaks?

DORA breaks that into five simple jobs that repeat forever in a loop:

1. **Identify** what you have and what could go wrong.
2. **Protect** it.
3. **Detect** problems early.
4. **Respond and recover** when problems happen.
5. **Learn** and improve.

If you can show you do all five, consistently, with evidence, you are most of the way to meeting this pillar.

## 2. The framework document (Art. 6)

You need one written ICT risk management framework. The board approves it. You review it at least once a year, and also after any major incident or when the regulator tells you to.

**What good looks like:** a single, version-controlled document (or a small set of linked documents) that states your risk appetite, names the owner, lists the policies underneath it, and has a dated board approval. It is short enough that people actually read it and specific enough that it drives real decisions.

**What weak looks like:** a 90-page document written once, approved once, and never opened again. Or a pile of separate policies with no top-level framework tying them together.

## 3. The five jobs in detail

### 3.1 Identify (Art. 8)

Know your estate. Keep an inventory of your business functions, the information and ICT assets that support them, and how they depend on each other and on outside providers. Assess your risks, and reassess whenever something big changes.

**What good looks like:** a live asset inventory (see the [ICT asset register template](../../templates/ict-asset-register.md)) where every critical system is linked to the business function it supports, to its owner, to its recovery targets, and to any third party involved. Risk assessments are repeatable and recorded, not done from memory.

**Concrete first step:** list your top 10 business functions. For each, write down the systems it needs, the data it uses, and the outside providers it relies on. That single table exposes most of your real risk on day one.

### 3.2 Protect (Art. 9)

Reduce the chance and impact of harm. This is your information security. It includes access control, strong authentication, encryption, network security, secure configuration, change management, and patching.

**What good looks like:** written control standards that say exactly what is expected (for example, "multi-factor authentication is required for all remote and administrative access", "critical patches are applied within a defined number of days", "all changes to production go through recorded approval"). These are enforced and checked, not just written.

**Plain-English tip:** DORA does not invent new security controls. If you already run a recognised security standard well, most of your protection work is done. The gap is usually proving it and linking it to critical functions.

### 3.3 Detect (Art. 10)

Spot unusual activity and incidents quickly. Set thresholds and alerts so problems surface early.

**What good looks like:** logging on critical systems, alerts that go to a named team, defined thresholds for what triggers action, and evidence that alerts are actually reviewed and acted on.

### 3.4 Respond and recover (Art. 11 and 12)

Have a business continuity policy, response and recovery plans, and recovery targets (RTO and RPO) for your important functions. Back up your data, keep backups separate from the live systems, and test that you can actually restore.

**What good looks like:** each critical function has an agreed RTO and RPO signed off by the business, plans that name who does what, and test reports proving a real restore worked inside the target time. Backups are isolated so that one ransomware attack cannot destroy both the live data and the backup.

**Sample RTO and RPO tiering:**

| Tier | Example functions | RTO (max downtime) | RPO (max data loss) |
|------|-------------------|--------------------|---------------------|
| 1 - Critical | Payments, trading, customer access | 2 hours | 15 minutes |
| 2 - Important | Reporting, reconciliation | 8 hours | 4 hours |
| 3 - Standard | Internal admin tools | 48 hours | 24 hours |

These numbers are examples. Set your own based on real business impact, then prove them by testing.

### 3.5 Learn (Art. 13 and 14)

After incidents, find the root cause and fix the underlying weakness. Take in threat intelligence. Train your staff and your board. Have a crisis communication plan for telling clients, partners, and the public when needed.

**What good looks like:** every significant incident has a written review with actions that are tracked to closure, and training completion is recorded, including for the board.

## 4. Control objectives

| ID | Control objective |
|----|-------------------|
| RM-01 | A board-approved resilience strategy defines risk appetite and objectives. |
| RM-02 | A complete, current inventory of functions, assets and dependencies is maintained. |
| RM-03 | ICT risks are assessed regularly and on major change. |
| RM-04 | An information security policy and supporting controls are implemented and enforced. |
| RM-05 | Detection with defined thresholds identifies anomalies and incidents promptly. |
| RM-06 | Continuity and recovery plans exist with tested RTO and RPO. |
| RM-07 | Backups are segregated and restoration is tested. |
| RM-08 | Post-incident reviews and threat intelligence drive improvement. |
| RM-09 | Awareness and resilience training runs for all staff and the board. |
| RM-10 | The framework is reviewed at least yearly and after major incidents. |

## 5. How to implement, in order

This is a suggested sequence. Do the early steps first because later steps depend on them.

1. **Weeks 1 to 4:** Draft the resilience strategy and get the board to approve ownership and risk appetite.
2. **Weeks 2 to 8:** Build the asset and dependency inventory. Start with critical functions.
3. **Weeks 6 to 12:** Run the first risk assessment using a repeatable method.
4. **Weeks 8 to 16:** Write and roll out the information security control standards.
5. **Weeks 10 to 18:** Set up detection, logging, and alerting on critical systems.
6. **Weeks 12 to 20:** Define RTO and RPO, write recovery plans, and schedule a restore test.
7. **Weeks 16 to 24:** Set up the backup regime and run a real restore test.
8. **Ongoing:** Post-incident reviews, threat intelligence, training, and the yearly framework review.

## 6. Sample artifact: a filled-in risk register row

| Risk ID | Risk | Affected function | Likelihood | Impact | Current controls | Rating | Owner | Action |
|---------|------|-------------------|-----------|--------|------------------|--------|-------|--------|
| R-011 | Ransomware encrypts core banking data | Customer accounts | Medium | Severe | Segregated backups, EDR, MFA | High | CISO | Test restore quarterly; tabletop exercise |

## 7. Evidence to keep

Approved strategy and framework (with version history), asset inventory extract, risk method and register, security policy and standards, alert configuration and sample alerts, continuity plans with RTO and RPO, restore-test reports, post-incident reviews, training records, and the annual review minutes.

## 8. Common mistakes

- An asset inventory that misses shadow IT, hidden dependencies, or third-party links.
- RTO and RPO written on paper but never proven by a real restore test.
- Backups that sit on the same network as production, so one attack destroys both.
- An "annual review" that is a rubber stamp, not a real reassessment.
- Generic training instead of role-based training that matches real risk.

## 9. Quick self-check

- Can you produce, in one hour, a list of your critical functions and the systems behind them? If not, start with the inventory.
- Have you ever proven, with a report, that you can restore a critical system inside its RTO? If not, that is your top priority.
- Did the board approve the framework this year, with minutes to show it? If not, fix the governance gap first.
