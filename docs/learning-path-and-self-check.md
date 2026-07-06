# Learning Path and Self-Check: Zero to Working Competence

This toolkit is a reference library. This file turns it into a **learning path** so
a GRC professional new to DORA can go from zero to genuinely useful in a structured
way, and **test themselves** at each stage. Work the stages in order; do not skip
the self-checks. If you cannot answer a self-check from memory, re-read the linked
material before moving on.

> Honest expectation: finishing this path makes you competent to run a gap
> assessment, draft the core artifacts, and scope an audit. It does not make you a
> lawyer. For a live filing, always confirm the current text on EUR-Lex and get
> qualified counsel. "Competent" means "competent and knows when to escalate".

---

## Stage 0: Orientation (half a day)

Read: [FAQ](faq.md), [Glossary](glossary.md), [Proportionality guide](proportionality-guide.md).

**Self-check (answer before continuing):**

1. Is there such a thing as a "DORA certificate"? What does "compliant" actually mean?
2. Who supervises a normal financial entity - the ESAs or your NCA?
3. Does being a small firm exempt you from DORA? What changes with proportionality?
4. Name the two things that are always legal duties regardless of size.

## Stage 1: The shape of the law (half a day)

Read: [README](../README.md) pillar table, [regulatory-references](regulatory-references.md),
[full-vs-simplified framework](full-vs-simplified-framework.md).

**Self-check:**

1. List the five pillars plus governance, and one thing each is about.
2. What is the difference between an RTS and an ITS?
3. Where in this toolkit do the real thresholds and deadlines live, and why only there?
4. What are the three incident-reporting deadlines?

## Stage 2: Scoping your firm (1 day)

Do: the [proportionality decision](proportionality-guide.md) and the
[CIF determination worksheet](../templates/critical-function-determination-worksheet.md)
for a real or practice firm.

**Self-check:**

1. Is your practice firm full-framework or simplified? Write the reason.
2. List its critical or important functions, with a one-line justification each.
3. Which shared/enabling function did you almost miss?

## Stage 3: Gap assessment (2-3 days)

Read the [maturity model](1-gap-assessment/maturity-model.md); run the
[self-assessment questionnaire](1-gap-assessment/self-assessment-questionnaire.md);
use the [control mapping](1-gap-assessment/control-mapping.md).

**Self-check:**

1. What is the minimum maturity level that counts as "compliant" for a control?
2. Two controls both score Level 2. Why might one be P1 and the other P4?
3. What does a **(legal)** flag mean for prioritisation?

## Stage 4: Build the artifacts (1-2 weeks)

Do: draft the five [model policies](../templates/model-policies/); build a
[BIA](../examples/worked-ict-risk-framework-and-bia.md); populate the
[registers](../templates/); fill the [classification aid](../templates/incident-classification-aid.md).

**Self-check:**

1. How do you derive an RTO from a BIA rather than guessing it?
2. What must a critical-function contract contain that a normal one need not (Art. 30)?
3. Walk through classifying a sample incident. Is it major? Why?
4. Write a mock initial notification (compare to the
   [worked example](../examples/novapay-incident-reports.md)).

## Stage 5: Third parties and testing (1 week)

Read: [playbook 04](2-implementation/04-third-party-risk-management.md),
[sub-outsourcing and concentration](2-implementation/sub-outsourcing-and-concentration.md),
[playbook 03](2-implementation/03-resilience-testing.md),
[register ITS mapping](register-of-information-its-mapping.md).

**Self-check:**

1. A hyperscaler will not redline its terms. How do you comply anyway?
2. What is the difference between a normal pen test and TLPT, and who does TLPT?
3. Why is the toolkit's register a *subset*, and what must you add before submitting?

## Stage 6: Audit yourself (3-5 days)

Read/apply: [test procedures](3-audit/test-procedures.md),
[sampling and evidence](3-audit/sampling-and-evidence.md),
[findings template](3-audit/findings-template.md).

**Self-check:**

1. Which populations must be tested in full rather than sampled, and why?
2. A single major incident was reported late. What does that do to the overall opinion?
3. Write one finding using the Condition/Criteria/Cause/Consequence/Recommendation shape.

## Stage 7: Put it together

Read the two end-to-end examples: [NovaPay walkthrough](../examples/model-startup-novapay.md)
and the [worked framework and BIA](../examples/worked-ict-risk-framework-and-bia.md).

**You are ready when you can, from memory:**

- Explain what DORA compliance is (and is not) to a board member in two minutes.
- Run a proportionality and CIF assessment for a firm and defend the result.
- Produce a gap assessment with prioritised, legally-aware findings.
- Draft the core policy set and a BIA-derived RTO/RPO tiering.
- Classify an incident and write the three reports to deadline.
- Scope an audit and reach a defensible opinion.

If any of those is shaky, go back to that stage. That gap is exactly where a senior
reviewer would catch you.

---

## Answer notes (check yourself)

These are pointers, not full answers - the detail is in the linked docs.

- **Stage 0:** No certificate; compliance is a continuous, evidenced, supervised
  state. Your NCA supervises you. Small firms are in scope, just lighter. Always-on
  duties: report major incidents on time; keep/submit the register; baseline testing.
- **Stage 1:** RTS = binding detail (e.g. thresholds); ITS = forms/templates.
  Numbers live only in regulatory-references.md to avoid drift. Deadlines: 4h / 72h / 1 month.
- **Stage 3:** Level 3 is the compliance minimum. Priority depends on legal flags and
  whether the control sits behind a critical function, not just the score. A failed
  **(legal)** sub-question makes it P1.
- **Stage 4:** RTO = the last outage duration before impact turns unacceptable, agreed
  with the business and proven by test. Art. 30 enhanced terms: audit/access rights,
  TLPT cooperation, exit/transition, security requirements.
- **Stage 5:** Use the provider's DORA addendum + audit substitutes + technical
  anti-lock-in + board-approved residual risk. TLPT = intelligence-led red team on
  production, only if the regulator names you. The register subset lacks LEIs,
  taxonomies, consolidation scope, and linkage keys needed for validation.
- **Stage 6:** Test in full: all major incidents, all critical functions, all
  critical-function contracts, all TLPT engagements. A single late report pulls the
  opinion to at least Partially compliant, usually Non-compliant.
