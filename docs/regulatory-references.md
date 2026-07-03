# Regulatory References: Real Figures Behind the Placeholders

**Last verified against official sources: 3 July 2026.** Always re-check the live
text on EUR-Lex before relying on any figure for a real compliance or audit job.
Regulatory technical standards (RTS) and implementing technical standards (ITS)
are amended over time; this file records the version the toolkit was written
against so you can spot drift.

This file is the single source of truth for the numbers that other documents in
this toolkit refer to. Where a guide previously said `[from RTS]` or
`[from ITS]`, it now points here. If a figure changes in law, change it here
once and every guide stays correct.

---

## 1. The core legal instruments

| Short name | Full instrument | Covers | Official link (ELI) |
|---|---|---|---|
| DORA | Regulation (EU) 2022/2554 | The main law, all five pillars | http://data.europa.eu/eli/reg/2022/2554/oj |
| Classification RTS | Commission Delegated Regulation (EU) 2024/1772 (13 Mar 2024) | Incident classification criteria and materiality thresholds | http://data.europa.eu/eli/reg_del/2024/1772/oj |
| Reporting RTS | Commission Delegated Regulation (EU) 2025/301 (23 Oct 2024) | Content and time limits for initial / intermediate / final reports and voluntary threat notifications | http://data.europa.eu/eli/reg_del/2025/301/oj |
| ICT risk RTS | RTS on ICT risk management framework and simplified framework | Pillar 1 detail | See ESA DORA page (indexed below) |
| Register ITS | ITS on the templates for the register of information | Pillar 4 register format | See ESA DORA page |
| Subcontracting RTS | Joint RTS on subcontracting ICT services supporting critical or important functions | Pillar 4 | See ESA DORA page |
| TLPT RTS | Joint RTS specifying elements related to threat-led penetration testing | Pillar 3 (TLPT) | See ESA DORA page |
| Oversight RTS | Joint RTS on harmonisation of conditions enabling oversight activities | CTPP oversight | See ESA DORA page |

Authoritative index of all DORA technical standards (bookmark this):
EBA DORA page — https://www.eba.europa.eu/activities/direct-supervision-and-oversight/digital-operational-resilience-act

---

## 2. Incident classification thresholds (Classification RTS 2024/1772)

An incident is **major** (RTS Art. 8) when it **has affected critical services**
(Art. 6) **AND** either:

- the **data-losses** threshold in Art. 9(5)(b) is met, **or**
- **two or more** of the other materiality thresholds in Art. 9(1) to (6) are met.

The seven criteria and their exact thresholds:

| Criterion (RTS Art.) | Threshold that counts as "met" |
|---|---|
| Clients, counterparts, transactions (Art. 9(1)) | Affected clients > **10%** of all clients using the service; **or** > **100 000** clients; **or** affected financial counterparts > **30%**; **or** affected transactions > **10%** of daily average number; **or** affected transaction value > **10%** of daily average value; **or** a client/counterpart identified as "relevant" is affected |
| Reputational impact (Art. 9(2), Art. 2) | Any of: reflected in the media; repetitive client/counterpart complaints; likely regulatory breach; likely material client loss |
| Duration and downtime (Art. 9(3)) | Incident duration > **24 hours**; **or** service downtime > **2 hours** for ICT services supporting critical or important functions |
| Geographical spread (Art. 9(4), Art. 4) | Impact in **two or more Member States** |
| Data losses (Art. 9(5)) | Any impact on availability, authenticity, integrity or confidentiality that harms business objectives or regulatory compliance (a); or any successful malicious unauthorised access that may lead to data loss (b) |
| Criticality of services (Art. 6) | Affects ICT/systems behind critical or important functions; or supervised/authorised financial services; or a successful malicious unauthorised access. **This is the gating criterion in Art. 8.** |
| Economic impact (Art. 9(6)) | Direct + indirect costs and losses have exceeded or are likely to exceed **EUR 100 000** |

**Recurring incidents** (Art. 8(2)): individually non-major incidents count as one
major incident if they occur at least **twice within 6 months**, share the same
apparent root cause, and together meet the major test. Assess monthly. (Does not
apply to microenterprises or Art. 16 simplified-framework entities.)

**Significant cyber threat** (Art. 10): voluntary notification test — the threat
could affect critical/important functions, has a **high probability** of
materialising, and if it materialised could meet the criticality criterion or the
thresholds in Art. 9(1) or 9(4).

---

## 3. Incident reporting time limits (Reporting RTS 2025/301, Art. 5)

| Report | Deadline |
|---|---|
| **Initial notification** | As early as possible, and **within 4 hours** of classifying the incident as major, **and no later than 24 hours** from becoming aware of it |
| **Intermediate report** | **Within 72 hours** of the initial notification (even if nothing changed); update without undue delay, and in any case once regular activities are recovered |
| **Final report** | **No later than 1 month** after the intermediate report (or the latest updated intermediate report) |

Extra rules that a runbook must build in:

- **Late classification (Art. 5(2)).** If you do not classify within 24 hours of
  awareness but classify later, the 4-hour initial-notification clock still runs
  from the moment of classification.
- **Cannot meet a deadline (Art. 5(3)).** You must tell the competent authority
  before the deadline passes and explain the delay. Silence is the worst option.
- **Weekends and bank holidays (Art. 5(4)).** If a deadline falls on a weekend or
  a national bank holiday, you may submit by **noon of the next working day**.
- **Exception (Art. 5(5)).** The weekend/holiday relief does **not** apply to the
  initial notification or intermediate report for credit institutions, CCPs,
  trading-venue operators, and entities that are "essential or important" under
  NIS2 (Directive (EU) 2022/2555).
- **Exception (Art. 5(6)).** A competent authority may also switch off the relief
  for other significant or systemic entities, by notifying them.

---

## 4. Report content (Reporting RTS 2025/301, Art. 1 to 4)

General info in every submission (Art. 1): submission type; entity name, LEI and
type; submitting entity; aggregated entities where relevant; contact person(s);
parent undertaking; currency for monetary figures.

- **Initial notification (Art. 2):** incident reference code; detection date/time
  and classification; description; the classification criteria met; impacted
  Member States; how it was discovered; origin if known; whether a BCP was
  activated; any reclassification to non-major; other relevant info.
- **Intermediate report (Art. 3):** authority-assigned reference code;
  occurrence date/time; recovery date/time; how the criteria were met; incident
  type; threats/techniques used; affected functional areas and processes;
  affected infrastructure; impact on clients' financial interests; reporting to
  other authorities; temporary/planned recovery measures; indicators of
  compromise.
- **Final report (Art. 4):** root causes; resolution date/time; how it was
  resolved; info for resolution authorities; direct/indirect costs, losses and
  financial recoveries; recurring-incident information.
- **Voluntary threat notification (Art. 6):** general info; detection timing;
  description; potential impact; the classification criteria that would have
  triggered a major report; threat status/changes; preventive actions;
  notifications to others; indicators of compromise.

---

## 5. How to keep this file honest

1. Re-verify every figure against EUR-Lex at least once a year and after any ESA
   announcement of amended standards.
2. Update the "Last verified" date at the top when you do.
3. If a figure changes, change it **here** and check that the incident playbook
   and the incident-classification aid still point here rather than repeating a
   hard-coded number.
4. Record the RTS/ITS versions in force during any audit in your findings report
   (see docs/3-audit/findings-template.md, Parts A and F).

> This document summarises binding EU law in plain English for working use. It is
> not legal advice and is not a substitute for the official text. Where this
> summary and the Official Journal differ, the Official Journal governs.
