# Full vs Simplified Framework: What Actually Changes

The [proportionality guide](proportionality-guide.md) tells you *whether* you can
use the simplified ICT risk management framework (DORA Art. 16). This file answers
the next question a practitioner always asks: **so what actually changes,
control by control?**

The key idea, repeated because people get it wrong: the simplified framework
reduces **formality and depth**, not the **goal**. You still protect, detect,
respond, recover, and report. And the **hard legal duties apply to everyone** -
major-incident reporting, the register of information, and baseline testing do not
get lighter just because you are small.

> Confirm your eligibility for the simplified framework in writing before relying
> on this. If unsure, apply the full framework. This is guidance, not legal advice.

## 1. What is identical under both (do not lighten these)

- **Incident classification and major-incident reporting** on the 4h/72h/1-month
  clock (see [regulatory-references.md](regulatory-references.md)). Pass/fail duty.
- **Register of information** kept and submitted at least yearly.
- **Baseline resilience testing** of your systems.
- **Management-body ownership** of ICT risk.
- **Third-party rules** for critical or important functions (contract terms, exit).
- **Written proportionality reasoning** on file.

## 2. Control-by-control delta

"Full" = the complete framework (Art. 5-16 in depth). "Simplified" = the lighter
Art. 16 framework. This is a practical reading; the binding detail is in the ICT
risk RTS (EU) 2024/1774, which contains a dedicated simplified-framework section.

| Control | Full framework | Simplified framework (Art. 16) |
|---|---|---|
| Governance (GOV) | Formal framework, RACI, board committee, training plan, budget line, three lines of defence | Management body still owns and approves ICT risk; lighter documentation and structure; roles still clear |
| Strategy & risk appetite (RM-01) | Written resilience strategy with quantified appetite, board-approved | A documented, proportionate ICT risk framework; appetite stated more simply |
| Asset inventory (RM-02) | Full inventory linking assets to functions, owners, RTO/RPO, third parties, reconciled for shadow IT | Inventory of key ICT systems and dependencies; still complete for critical functions |
| Risk assessment (RM-03) | Repeatable methodology, reassessed on change, full register | Continuous monitoring of security/functioning; proportionate assessment |
| Security controls (RM-04) | Full documented control standards, enforced and evidenced | Controls that reduce ICT risk impact; the essentials (access, MFA, encryption, patching) still expected |
| Detection (RM-05) | Logging + thresholds + named team + evidence alerts are actioned | A way to detect anomalous activity and incidents promptly |
| Continuity & recovery (RM-06) | RTO/RPO per critical function, plans, proven restore inside RTO | Business continuity and recovery arrangements; periodic testing (lighter) |
| Backups (RM-07) | Segregated, tiered, restore-tested with reports | Backups and restoration arrangements that work; test them |
| Learning (RM-08/09) | Post-incident reviews, threat intel, role-based training incl. board | Lessons learned and awareness, proportionate |
| Testing (Pillar 3) | Risk-based programme across methods; TLPT if named | Periodic testing of key systems and arrangements; TLPT only if named (rare for simplified-eligible firms) |
| Third-party (Pillar 4) | Full strategy, register, due diligence, Art. 30 terms, tested exit, concentration/sub-outsourcing analysis | Same register and reporting duty; proportionate due diligence; enhanced terms still apply for critical-function providers |
| Information sharing (Pillar 5) | Voluntary; formal arrangement if you join | Voluntary; same |

## 3. How to use this with the questionnaire

Run the [self-assessment questionnaire](1-gap-assessment/self-assessment-questionnaire.md)
as normal. If you are simplified-framework, set the **target maturity lower** on
depth-heavy controls (aim for solid Level 3 rather than 4-5), but keep the
**(legal)** items at full strength - they never scale down. Record next to each
control that you are applying the simplified reading and why.

## 4. Common mistakes

- Reading "simplified" as "optional". It is lighter, not absent.
- Lightening a **(legal)** duty (reporting, register, baseline testing). Never do this.
- Claiming simplified eligibility without written legal confirmation.
- Forgetting that critical-or-important-function rules apply regardless of size.

Pairs with the [proportionality guide](proportionality-guide.md) and the
[CIF determination worksheet](../templates/critical-function-determination-worksheet.md).
