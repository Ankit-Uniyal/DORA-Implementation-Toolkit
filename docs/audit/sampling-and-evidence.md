# Sampling and Evidence Guidance

How to size samples, pick items to test, and judge evidence when you run the audit test procedures. Adapt this to your own audit method and risk appetite. It is a sensible default, not a strict standard.

Version note: this file describes method only. It does not depend on any specific RTS or ITS numbers. Confirm the RTS and ITS versions in force for your audit period in the engagement scope.

## 1. Types of testing

There are four ways to get evidence, from weakest to strongest:

- Inquiry: interviews and walkthroughs. Always back it up with something else. Never rely on inquiry alone.
- Inspection: look at documents, settings, and records.
- Observation: watch a process being done.
- Re-performance: do the control again yourself. This is the strongest evidence.

Use re-performance and inspection for high-risk controls. Inquiry plus observation can be enough for low-risk ones.

## 2. Whole population or a sample

Some DORA controls should be tested on the whole population, not a sample, because each item carries regulatory weight:

- All major incidents in the period (reporting timeliness and content, controls INC-04 and INC-05).
- All critical or important functions for continuity, recovery, RTO, RPO, and test coverage.
- All contracts behind critical or important functions, for the required and enhanced clauses.
- All TLPT engagements in the cycle (if you are in scope).

For higher-volume, lower-risk populations (for example change tickets, patch records, access reviews), sampling is fine.

## 3. Suggested sample sizes for attribute testing

| Control frequency | Population | Suggested sample |
|---|---|---|
| Annual | 1 | 1 (the one instance) |
| Quarterly | 4 | 2 |
| Monthly | 12 | 2 to 4 |
| Weekly | about 52 | 5 to 8 |
| Daily | about 250 | 15 to 25 |
| Many times a day or continuous | large | 25 to 40 |

These are typical internal-audit defaults. Increase the sample if the control is high-risk, if you expect exceptions, or if past testing found problems.

## 4. How to pick the items

- Prefer random or systematic selection so the sample represents the population.
- Add some risk-based picks for the highest-risk items (for example the largest third parties, the most critical systems, the highest-severity incidents).
- Write down the population source, how you checked it was complete, how you selected items, and the criteria you used.

## 5. Judging exceptions

- Decide if each exception is a control failure (the control did not work) or just a paperwork issue.
- Decide if it is a one-off or a pattern. If it looks systemic, test more.
- Think about the regulatory effect. A single missed major-incident deadline is a serious finding no matter how small the sample rate looks.
- Where it helps, project the error rate across the population, then conclude on whether the control is effective.

## 6. Evidence quality and retention

- Prefer evidence that is objective, dated, and produced independently (system logs, timestamps, regulator acknowledgements) over what management simply tells you.
- For each test, record: the control reference, what you did, the population, the sample, the items you looked at, the results, any exceptions, your conclusion, who prepared it, who reviewed it, and the date.
- Keep your working papers and source evidence in line with your audit method and DORA record-keeping expectations.

## 7. Checking a population is complete

Sampling is only reliable if the population is complete. For each population, do an independent completeness check, for example:

- Incidents: reconcile the incident register to monitoring and alerting logs and to service-desk tickets.
- Third parties: reconcile the register of information to accounts-payable data and cloud or SaaS inventories.
- Critical systems: reconcile to the ICT asset inventory and the business-function map.
