# Pillar 3: Digital Operational Resilience Testing (Playbook)

DORA articles: Art. 24 to 27. Supplemented by the RTS on TLPT, which lines up with the TIBER-EU framework.

Read first: Glossary. Use with: TLPT scoping worksheet.

This is a playbook. It gives you the steps, a method-selection table, a test calendar, a findings workflow, and a TLPT decision path. Plain English, no em dashes.

## At a glance

| Item | Detail |
|---|---|
| Goal | Prove your defences actually work before an attacker or an outage finds the gap. |
| Who leads | Head of Security or Test Manager, independent of the build teams. |
| Typical time | 12 weeks to set up baseline testing; TLPT runs on a multi-year cycle if you are in scope. |
| Main outputs | Testing programme, test calendar, findings tracker, and (if named) a TLPT plan. |
| Done when | Every critical system was tested in the last 12 months and serious findings are fixed and re-tested. |

## 1. What this pillar is really about

You can write perfect policies and still fail in a real crisis. Testing is how you find out if your defences work before an attacker or an outage does. DORA asks for two levels:

- Baseline testing: every in-scope firm does this. Regular, risk-based checks of your systems.
- Advanced testing (TLPT): only firms the regulator names do this. Skilled testers act like real attackers against your live systems.

The simple model: baseline testing checks the locks and alarms; TLPT hires an ethical burglar to actually try to break in.

## 2. Before you start (prerequisites)

- A complete inventory of critical systems from Pillar 1 (so nothing is missed).
- Independence: testers who did not build the thing they test.
- A findings process that can assign owners and deadlines.
- The TLPT scoping worksheet, in case you are in scope.

## 3. Step-by-step build (baseline)

Step 1: List critical systems. Owner: Test Manager. Pull the critical systems from the Pillar 1 inventory. Output: a scoped list.

Step 2: Choose methods per system. Owner: Test Manager. Use the method-selection table below to match test types to each system's risk. Output: a method plan.

Step 3: Build the test calendar. Owner: Test Manager. Map every critical system to at least one test in the next 12 months, with owners and dates. Output: a test calendar (see the sample row).

Step 4: Set up the findings workflow. Owner: Security. Every issue gets a severity, an owner, a fix deadline, and a re-test. Output: a findings tracker.

Step 5: Run the tests. Owner: Testers. Execute to the calendar. Keep dated reports. Output: test reports.

Step 6: Fix and re-test. Owner: System owners. Prioritise, fix, and re-verify. Output: closed findings with re-test evidence.

Step 7: Feed results back. Owner: CISO. Update the risk register and the framework with what testing found. Output: an updated risk view.

## 4. Ready-to-use artifact: method-selection table

Pick a mix that fits each system's risk. Higher risk means more, and deeper, testing.

| Test type | What it checks | Good for |
|---|---|---|
| Vulnerability scan | Known weaknesses | All systems, frequent |
| Patch and config review | Missing patches, weak settings | All critical systems |
| Penetration test | Whether weaknesses can be exploited | Internet-facing and critical systems |
| Scenario-based test | How you handle a specific event | Critical functions |
| Performance and load test | Behaviour under stress | High-volume systems |
| End-to-end test | Whether a full process holds up | Cross-system critical journeys |
| Source code review | Flaws in your own code | Systems you build |

## 5. Advanced testing: TLPT (Art. 26)

TLPT is only for firms the regulator identifies. You do not opt in. If you are named:

- You run TLPT at least every three years (the regulator can change this).
- It covers several or all of your critical or important functions.
- It runs on live production systems, safely managed by a small control team.
- In-scope outside providers are included, sometimes through shared "pooled" tests.
- The regulator validates the scope and, at the end, issues an attestation.
- The method follows the RTS, which is built on TIBER-EU.

Warning: a normal penetration test is not a TLPT. TLPT is a full, intelligence-led red team exercise on production, with regulator oversight. If you are in scope and only do standard pen tests, you have a gap. Use the TLPT scoping worksheet.

## 6. Decision path: are you in scope for TLPT?

1. Ask your competent authority whether they have named you. Do not assume.
2. If named: use the scoping worksheet, plan the multi-year cycle, engage qualified providers, and get scope validated.
3. If not named: you still do baseline testing, but not TLPT. Record that you checked.

## 7. Who can test (Art. 27)

Testers must be highly capable and reputable, with real expertise in threat intelligence, penetration testing, and red teaming. External testers need professional indemnity insurance. If you use internal testers, extra rules apply, including regulator approval and managing conflicts of interest.

## 8. Worked example: a test calendar row

| System | Function | Test type | Frequency | Last test | Result | Next test | Owner |
|---|---|---|---|---|---|---|---|
| Core payments | Payments (critical) | Penetration test | Annual | 2025-06 | 2 highs fixed and re-tested | 2026-06 | Head of Security |

## 9. Worked example: a findings tracker row

| Finding | Severity | System | Raised | Owner | Fix due | Status | Re-test date | Result |
|---|---|---|---|---|---|---|---|---|
| Unpatched web server | High | Core payments | 2025-06-10 | Platform team | 2025-06-24 | Closed | 2025-07-01 | Verified fixed |

## 10. Control objectives

| ID | Control objective |
|---|---|
| TST-01 | A documented, risk-based testing programme exists and is reviewed. |
| TST-02 | All critical systems and applications are tested at least yearly. |
| TST-03 | Testing uses a suitable mix of methods for the risk. |
| TST-04 | Testers are independent and qualified, with conflicts managed. |
| TST-05 | Findings are prioritised, fixed, and re-checked. |
| TST-06 | If in scope, TLPT runs at least every three years on production critical functions. |
| TST-07 | In-scope third parties are included in TLPT, or via pooled testing. |
| TST-08 | TLPT follows the RTS and TIBER-EU, with regulator validation and attestation. |

## 11. Acceptance checklist (done when)

- [ ] A risk-based testing programme and calendar exist and cover every critical system.
- [ ] Test methods match each system's risk.
- [ ] Testers are independent and qualified (and insured if external).
- [ ] A findings tracker shows fixes and re-tests.
- [ ] You have confirmed with the regulator whether you are named for TLPT.
- [ ] If in scope, a TLPT plan, scope validation, and provider engagement are in place.

## 12. Evidence to keep

The testing programme and calendar, dated test reports for critical systems, tester qualification and independence records (and insurance for external testers), the findings tracker showing fixes and re-tests, and, if in scope, TLPT scope documents, threat intelligence and red team reports, control-team logs, and the regulator attestation.

## 13. Common mistakes

- Ad hoc testing with no risk-based plan.
- A critical system missed because the inventory was incomplete.
- Findings that are logged but never fixed or re-tested.
- Assuming standard pen testing meets the TLPT duty. It does not.
- Leaving in-scope third parties out of TLPT scope.

## 14. Quick self-check

- Can you show that every critical system was tested in the last 12 months? If not, close the coverage gap.
- When you find a serious issue, can you prove it was fixed and re-tested? If not, fix the findings workflow.
- Do you know for certain whether you are named for TLPT? If not, ask your regulator before assuming you are out.
