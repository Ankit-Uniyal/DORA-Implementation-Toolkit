# Template: Incident Classification Aid

Supports DORA Art. 18 and the RTS on classification. Use this aid to decide, in a consistent way, whether an ICT-related incident is major (which triggers mandatory reporting) and to help classify significant cyber threats.

Important: the exact thresholds are set in the RTS on classification. The numbers (for example, how many clients or transactions are affected, how many hours of downtime, or the money amounts) must be taken from the current official RTS. This aid gives you the structure and a worksheet. Fill in the thresholds from the RTS in force before you use it for real.

## 1. Classification criteria (Art. 18)

Assess the incident against each criterion, then apply the RTS thresholds and logic to decide if it is major.

| # | Criterion | What to measure | RTS threshold (fill in) | Value observed | Met? |
|---|---|---|---|---|---|
| 1 | Clients, counterparts, transactions affected | Number and importance | [from RTS] | | |
| 2 | Reputational impact | Media, complaints, regulator attention | [from RTS] | | |
| 3 | Duration and downtime | How long the disruption lasts | [from RTS] | | |
| 4 | Geographical spread | Areas or Member States affected | [from RTS] | | |
| 5 | Data losses | Impact on availability, authenticity, integrity, confidentiality | [from RTS] | | |
| 6 | Criticality of services affected | Critical or important functions hit | [from RTS] | | |
| 7 | Economic impact | Direct and indirect costs, absolute and relative | [from RTS] | | |

Determination: [Major / Not major]. Record the reasoning and which criteria and thresholds were the deciding ones.

## 2. Decision workflow

- Log the incident and capture the seven criteria inputs as soon as the data allows.
- Apply the RTS logic (which criteria and thresholds count) to decide if it is major.
- If it is major, start the reporting runbook: initial, intermediate, and final reports.
- Re-check the classification as new facts come in. An incident can become major later.
- If this is a significant cyber threat and not an incident, assess how critical the services at risk are, how many parties are affected, and how wide the spread is, then decide on voluntary notification.

## 3. Incident record fields

| Field | Value |
|---|---|
| Incident ID | |
| Detected (date and time) | |
| Description | |
| Affected functions or assets | |
| Classification decision | Major / Not major |
| Decision maker and time | |
| Initial report due and sent | |
| Intermediate report(s) | |
| Final report due and sent | |
| Root cause | |
| Clients notified? | Yes / No / N/A |
| Lessons-learned reference | |

## 4. Reminders

- Classification can change. Re-check it as the impact becomes clearer.
- The initial-notification clock is tight. Pre-assign ownership and escalation.
- Keep the evidence trail (timeline, inputs, decision reasoning) for audit and for the final report.
