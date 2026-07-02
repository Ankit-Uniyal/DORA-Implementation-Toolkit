# DORA Maturity Model and Scoring Guide

This model gives every control a score from 0 to 5. Use it with the [self-assessment questionnaire](self-assessment-questionnaire.md) to measure where you are, and to turn gaps into a clear to-do list. It works for implementing, gap-assessing, and audit rating.

**Read first:** [Glossary](../glossary.md).

---

## 1. The five-level scale

| Level | Name | Plain meaning |
|-------|------|---------------|
| 0 | Absent | Nothing exists. The requirement is not addressed at all. |
| 1 | On paper only | It is written down, but not really working. Or it happens informally, depending on one person. |
| 2 | Partly working | Documented and running in some places, but not consistent or complete. |
| 3 | Working | Documented, owned, and running consistently, with evidence. This is the minimum to call a control compliant. |
| 4 | Measured | Level 3, plus you measure it (metrics or KPIs) and review it regularly. |
| 5 | Improving | Level 4, plus you keep improving it using data, threat intelligence, and lessons learned. |

**Target.** Aim for Level 3 or higher on every control. Aim for Level 4 or higher on the most important ones (for example, incident reporting, backups, and TLPT if you are in scope). Levels 0 to 2 are gaps.

## 2. Maturity is not the same as legal compliance

This is the most important point in this guide, so read it carefully.

The 0 to 5 scale measures **how well a control is built and running**. But some DORA duties are **hard legal lines**, not a slow journey. You either did them or you did not. Examples:

- Reporting a major incident inside the deadline.
- Keeping and reporting the register of information.
- Running TLPT if the regulator named you.

For these, a "Level 2" is not a mild improvement item. It means you are **breaching a legal duty right now**. In the questionnaire, these are marked **(legal)**. If a **(legal)** item fails, treat it as a top priority, no matter what the average score says.

Simple way to hold both ideas at once: the score tells you how healthy a control is; the legal flags tell you if you are breaking the law today. Fix the law-breaking first.

## 3. How to score, step by step

1. For each control, answer its sub-questions in the questionnaire (Yes, Partly, No), with evidence.
2. Pick the 0 to 5 level that matches, using the scale above.
3. Score only on evidence you can show, not on good intentions.
4. Write the evidence reference next to the score.
5. Mark the control as a gap if it is below Level 3.
6. Mark the control as a **breach risk** if any **(legal)** sub-question failed.

## 4. Turning scores into priorities

Use both the score and the risk to set priority:

| Priority | When to use it |
|----------|----------------|
| P1 - Critical | Any failed **(legal)** duty, OR a Level 0 to 1 control behind a critical or important function. Fix now. |
| P2 - High | A mandatory control at Level 0 to 2 with real risk. |
| P3 - Medium | A control at Level 2 to 3 that needs to be more consistent or measured. |
| P4 - Low | A control at Level 3 or above with only minor polish left. |

## 5. Your remediation to-do list

For each gap, record: control ID, current level, target level, priority, whether it is a legal breach, the root cause, the fix, the owner, the due date, and the re-check date.

## 6. Reporting to the board

Show the board four simple things:

- The overall maturity score and the score per pillar (a colour heat map works well).
- The number of gaps by priority.
- Any legal breach flags, called out clearly and separately.
- The top P1 and P2 fixes, with owners and dates.

This is the kind of clear, honest view the board needs to meet its duty under Art. 5.

## 7. Worked examples

| Control | What you found | Level | Legal breach? | Priority |
|---------|----------------|-------|---------------|----------|
| INC-04 (report major incidents on time) | Runbook exists, but no test proves you can hit the first deadline, and ownership is unclear | 2 | Yes, if a real incident was late | P1 |
| RM-07 (backups and restore) | Backups run, are kept separate, and a restore was tested this year with a report | 4 | No | P4 |
| TPP-02 (register of information) | Register exists but misses SaaS and intra-group services | 2 | Yes, register is incomplete | P1 |
| ISH-05 (use of shared intelligence) | You receive threat intel but do not feed it into detection | 1 | No (this pillar is voluntary) | P3 |

Notice how two controls at the same Level 2 can have very different priorities, because one involves a legal breach and one does not.
