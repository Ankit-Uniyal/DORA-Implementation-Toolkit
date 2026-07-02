# Template — Incident Classification Aid

Supports DORA Art. 18 and the RTS on classification. Use this aid to consistently assess whether an ICT-related incident is **major** (triggering mandatory reporting) and to classify significant cyber threats.

> **Materiality thresholds are defined in the RTS on classification.** The exact numeric thresholds (e.g. numbers/percentages of clients or transactions affected, downtime hours, economic-impact amounts) must be taken from the current official RTS. This aid provides the criteria structure and a worksheet; **populate the thresholds from the RTS in force** before operational use.

---

## 1. Classification criteria (Art. 18)

Assess the incident against each criterion, then apply the RTS thresholds/logic to decide "major".

| # | Criterion | What to measure | RTS threshold (fill in) | Value observed | Met? |
|---|-----------|-----------------|-------------------------|----------------|------|
| 1 | Clients / counterparts / transactions affected | Number and/or relevance | _[from RTS]_ | | |
| 2 | Reputational impact | Media coverage, complaints, regulatory attention | _[from RTS]_ | | |
| 3 | Duration & service downtime | Elapsed time of disruption | _[from RTS]_ | | |
| 4 | Geographical spread | Areas/Member States affected | _[from RTS]_ | | |
| 5 | Data losses | Impact on availability, authenticity, integrity, confidentiality | _[from RTS]_ | | |
| 6 | Criticality of services affected | Critical/important functions impacted | _[from RTS]_ | | |
| 7 | Economic impact | Direct + indirect costs, absolute & relative | _[from RTS]_ | | |

**Determination:** _[Major / Not major]_ — record the reasoning and which criteria/thresholds were decisive.

## 2. Decision workflow

1. Log the incident and capture the seven criteria inputs as early data allows.
2. Apply the RTS logic (primary/secondary criteria and thresholds) to decide "major".
3. If **major**, trigger the [reporting runbook](../docs/implementation/02-incident-management-and-reporting.md): initial, intermediate, final reports.
4. Re-evaluate classification as new information emerges (an incident can escalate to major).
5. If a **significant cyber threat** (not an incident), assess criticality of services at risk, number of affected parties, and geographical spread for voluntary notification.

## 3. Incident record fields

| Field | Value |
|-------|-------|
| Incident ID | |
| Detected (date/time) | |
| Description | |
| Affected functions/assets | |
| Classification decision | Major / Not major |
| Decision maker / time | |
| Initial report due / sent | |
| Intermediate report(s) | |
| Final report due / sent | |
| Root cause | |
| Clients notified? | Yes / No / N/A |
| Lessons learned ref | |

## 4. Reminders

- Classification is **dynamic** — re-check as impact becomes clearer.
- The initial-notification clock is tight; pre-assign ownership and escalation.
- Keep the evidence trail (timeline, inputs, decision rationale) for audit and the final report.
