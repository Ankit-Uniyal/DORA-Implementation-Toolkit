# Template: Incident Classification Aid

Supports DORA Art. 18 and the Classification RTS (Commission Delegated Regulation
(EU) 2024/1772). Use this aid to decide, in a consistent way, whether an
ICT-related incident is **major** (which triggers mandatory reporting) and to help
classify **significant cyber threats**.

> The thresholds below are the **real figures from Classification RTS 2024/1772**,
> verified 3 July 2026. They are maintained centrally in
> docs/regulatory-references.md — if the law changes, update them there. Always
> confirm against the current Official Journal text before relying on them.

## 1. The "major" test (RTS Art. 8)

An incident is **major** when it **has affected critical services** (criterion 6
below) **AND** either:

- the **data-losses** threshold (criterion 5, limb b) is met, **or**
- **two or more** of the other materiality thresholds (criteria 1 to 7) are met.

In other words: criticality of services is the gate. Once through the gate, one
serious data-loss trigger, or any two other triggers, makes it major.

## 2. Classification criteria and real thresholds (RTS Art. 1 to 9)

| # | Criterion | RTS threshold that counts as "met" | Value observed | Met? |
|---|---|---|---|---|
| 1 | Clients, counterparts, transactions | Affected clients > 10% of all clients using the service; OR > 100 000 clients; OR affected financial counterparts > 30%; OR affected transactions > 10% of daily average number; OR affected transaction value > 10% of daily average value; OR a "relevant" client/counterpart affected | | |
| 2 | Reputational impact | Any of: reflected in the media; repetitive client/counterpart complaints; likely regulatory breach; likely material client loss | | |
| 3 | Duration and downtime | Incident duration > 24 hours; OR service downtime > 2 hours for ICT services supporting critical/important functions | | |
| 4 | Geographical spread | Impact in 2 or more Member States | | |
| 5 | Data losses | (a) any impact on availability, authenticity, integrity or confidentiality harming business objectives or regulatory compliance; OR (b) any successful malicious unauthorised access that may lead to data loss | | |
| 6 | Criticality of services (the gate) | Affects ICT/systems behind critical or important functions; OR supervised/authorised financial services; OR a successful malicious unauthorised access | | |
| 7 | Economic impact | Direct + indirect costs and losses exceed, or are likely to exceed, EUR 100 000 | | |

**Determination:** [ Major / Not major ]. Record which criteria were met and which
were the deciding ones.

**Recurring incidents (RTS Art. 8(2)):** individually non-major incidents count as
one major incident if they happen at least twice in 6 months, share the same
apparent root cause, and together meet the major test. Assess monthly. (Not for
microenterprises or Art. 16 simplified-framework entities.)

## 3. Worked example (fictional)

*NovaPay, a small e-money institution.* At 09:40 it confirms unauthorised access
to a client-facing wallet system that supports a critical function.

| # | Criterion | Assessment for this incident | Met? |
|---|---|---|---|
| 6 | Criticality (gate) | Successful malicious unauthorised access to a system behind a critical function | YES (gate passed) |
| 5 | Data losses | Unauthorised access that may lead to data loss — Art. 9(5)(b) | YES |
| 3 | Duration/downtime | Wallet unavailable 2h20m (> 2h for a critical-function service) | YES |
| 1 | Clients | ~4% of clients affected (< 10%, < 100 000) | No |
| 2 | Reputational | No media yet, few complaints | No |
| 4 | Geographical | Single Member State | No |
| 7 | Economic | Estimated EUR 30 000 (< 100 000) | No |

**Result: MAJOR.** The gate (criterion 6) is passed and the data-losses trigger
(criterion 5b) alone is enough under Art. 8. Even without it, criteria 5 and 3 are
two triggers. Start the reporting clock at 10:15 when "major" is declared.

## 4. Significant cyber threat (voluntary) — RTS Art. 10

Notify voluntarily where all of these hold: the threat could affect
critical/important functions or other entities; it has a **high probability** of
materialising; and if it materialised it could meet the criticality criterion (6)
or the thresholds in criterion 1 or 4.

## 5. Reporting deadlines once "major" is declared (Reporting RTS 2025/301, Art. 5)

| Report | Deadline |
|---|---|
| Initial notification | Within 4 hours of classifying as major, and no later than 24 hours from awareness |
| Intermediate report | Within 72 hours of the initial notification |
| Final report | Within 1 month of the intermediate report |

If you cannot meet a deadline, tell the competent authority **before** it passes
and explain why (Art. 5(3)). Weekend/bank-holiday relief may apply to some firms
but not to credit institutions, CCPs, trading venues, or NIS2 essential/important
entities. See docs/regulatory-references.md, section 3.

## 6. Incident record fields

| Field | Value |
|---|---|
| Incident ID | |
| Detected (date and time) | |
| Aware (date and time) | |
| Classified major (date and time) | |
| Description | |
| Affected functions or assets | |
| Criteria met | |
| Classification decision | Major / Not major |
| Decision maker | |
| Initial report due / sent | |
| Intermediate report(s) due / sent | |
| Final report due / sent | |
| Root cause | |
| Clients notified? | Yes / No / N/A |
| Lessons-learned reference | |

## 7. Reminders

- Classification can change. Re-check it as impact becomes clearer; an incident
  can become major later, and the 4-hour clock then runs from that moment.
- Keep the full evidence trail (timeline, inputs, decision reasoning) for audit
  and for the final report.
