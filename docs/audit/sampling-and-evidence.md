# Sampling & Evidence Guidance

Guidance for sizing samples, selecting items, and evaluating evidence when executing the [audit test procedures](test-procedures.md). Adapt to your organisation's audit methodology and risk appetite; this is a pragmatic default, not a prescriptive standard.

---

## 1. Types of testing

- **Inquiry** — interviews and walkthroughs. Corroborate; never rely on inquiry alone.
- **Inspection** — examine documents, configurations, records.
- **Observation** — watch a process being performed.
- **Re-performance** — independently re-execute the control (strongest evidence).

Prefer re-performance and inspection for high-risk controls; inquiry plus observation may suffice for low-risk ones.

## 2. Full-population vs sample

Some DORA controls should be tested on the **whole population**, not a sample, because each item carries regulatory weight:

- **All major incidents** in the period (reporting timeliness and completeness — INC-04/05).
- **All critical/important functions** for BC/DR, RTO/RPO and testing coverage.
- **All contracts supporting critical/important functions** for mandatory/enhanced clauses.
- **All TLPT engagements** in the cycle (if in scope).

For higher-volume, lower-individual-risk populations (e.g. change tickets, patch records, access reviews), use sampling.

## 3. Indicative sample sizes for attribute testing

| Control frequency | Population | Indicative sample |
|-------------------|-----------|-------------------|
| Annual | 1 | 1 (the instance) |
| Quarterly | 4 | 2 |
| Monthly | 12 | 2-4 |
| Weekly | ~52 | 5-8 |
| Daily | ~250 | 15-25 |
| Many times per day / continuous | large | 25-40 |

These are typical internal-audit defaults; increase the sample if the control is high-risk, if you expect exceptions, or if prior testing found issues.

## 4. Selection method

- Prefer **random or systematic** selection for representativeness.
- Add **risk-based / judgmental** selections for the highest-criticality items (e.g. the largest third parties, the most critical systems, the highest-severity incidents).
- Document the population source, its completeness check, the selection method, and the seed/criteria.

## 5. Evaluating exceptions

1. Determine whether each exception is a **control exception** (control did not operate) or a data/documentation issue.
2. Assess whether it is **isolated** or **systemic** (extend testing if systemic).
3. Consider the **regulatory consequence** — a single missed major-incident reporting deadline is a significant finding regardless of sample rate.
4. Project the exception rate where appropriate and conclude on operating effectiveness.

## 6. Evidence quality & retention

- Prefer evidence that is **objective, dated, and independently generated** (system logs, timestamps, authority acknowledgements) over management assertions.
- Record for each test: control ref, procedure performed, population, sample, items examined, results, exceptions, conclusion, preparer, reviewer, date.
- Retain workpapers and source evidence in line with your audit methodology and DORA record-keeping expectations.

## 7. Completeness of populations

The reliability of sampling depends on population completeness. For each population, perform an independent completeness check, e.g.:
- **Incidents** — reconcile the incident register to monitoring/alerting logs and service-desk tickets.
- **Third parties** — reconcile the register of information to accounts-payable and cloud/SaaS inventories.
- **Critical systems** — reconcile to the ICT asset inventory and business-function mapping.
