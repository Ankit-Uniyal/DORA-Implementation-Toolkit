# Pillar 3 - Digital Operational Resilience Testing

**DORA articles:** Art. 24 to 27. Supplemented by the RTS on TLPT, which lines up with the TIBER-EU framework.

**Read first:** [Glossary](../glossary.md). **Use with:** [TLPT scoping worksheet](../../templates/tlpt-scoping-worksheet.md).

---

## 1. What this pillar is really about

You can write perfect policies and still fail in a real crisis. Testing is how you find out if your defences actually work before an attacker or an outage does. DORA asks for two levels of testing:

- **Baseline testing:** every in-scope firm does this. Regular, risk-based checks of your systems.
- **Advanced testing (TLPT):** only firms the regulator names do this. Skilled testers act like real attackers against your live systems.

The simple mental model: baseline testing checks the locks and alarms; TLPT hires an ethical burglar to actually try to break in.

## 2. Baseline testing (Art. 24 and 25)

You need a written testing programme that is part of your ICT risk framework, is based on risk, uses a clear method, and is run by people independent of those who built the systems. All critical systems and applications must be tested at least once a year. Every issue found must be prioritised, fixed, and re-checked.

The toolbox of test types includes: vulnerability scans, network security tests, gap analysis, source code review where possible, scenario-based tests, performance and load tests, end-to-end tests, and penetration tests. You pick the mix that fits each system's risk.

**What good looks like:** a test calendar that maps every critical system to a test in the year, a findings tracker where issues are fixed and re-tested, and testers who did not build the thing they are testing.

**What weak looks like:** occasional testing with no plan, findings that are noted but never fixed, and no proof that critical systems were all covered.

## 3. Advanced testing: TLPT (Art. 26)

TLPT is only for firms the regulator identifies, based on how important and risky they are. You do not opt in. If you are named:

- You run TLPT at least every three years (the regulator can change this).
- It covers several or all of your critical or important functions.
- It runs on live production systems, safely managed by a small control team.
- If outside providers support those functions, they are included, sometimes through shared "pooled" tests.
- The regulator validates the scope and, at the end, issues an attestation that the test met the rules.
- The method follows the RTS, which is built on TIBER-EU (threat-led red team testing driven by real threat intelligence).

**Plain-English warning:** a normal penetration test is not a TLPT. TLPT is a full, intelligence-led red team exercise on production, with regulator oversight. If you are in scope and you only do standard pen tests, you have a gap. Use the [TLPT scoping worksheet](../../templates/tlpt-scoping-worksheet.md).

## 4. Who can test (Art. 27)

Testers must be highly capable and reputable, with real expertise in threat intelligence, penetration testing, and red teaming. External testers need professional indemnity insurance. If you use internal testers, extra rules apply, including regulator approval and managing conflicts of interest.

## 5. Control objectives

| ID | Control objective |
|----|-------------------|
| TST-01 | A documented, risk-based testing programme exists and is reviewed. |
| TST-02 | All critical systems and applications are tested at least yearly. |
| TST-03 | Testing uses a suitable mix of methods for the risk. |
| TST-04 | Testers are independent and qualified, with conflicts managed. |
| TST-05 | Findings are prioritised, fixed, and re-checked. |
| TST-06 | If in scope, TLPT runs at least every three years on production critical functions. |
| TST-07 | In-scope third parties are included in TLPT, or via pooled testing. |
| TST-08 | TLPT follows the RTS and TIBER-EU, with regulator validation and attestation. |

## 6. How to implement, in order

1. **Weeks 1 to 4:** List critical systems and design a risk-based test calendar and method.
2. **Weeks 3 to 8:** Set up the baseline test suite (scans, pen tests, scenario tests) with owners and dates.
3. **Weeks 4 to 10:** Build a findings workflow that links each issue to an owner, a deadline, and a re-test.
4. **Weeks 6 to 12:** Check with your regulator whether you are named for TLPT.
5. **If in scope for TLPT:** plan the multi-year cycle, scope it around critical functions and third parties, and engage qualified providers. Use the scoping worksheet.
6. **Ongoing:** run tests to the calendar, fix findings, and feed results back into the risk framework.

## 7. Sample artifact: a test calendar row

| System | Function | Test type | Frequency | Last test | Result | Next test | Owner |
|--------|----------|-----------|-----------|-----------|--------|-----------|-------|
| Core payments | Payments (critical) | Penetration test | Annual | 2025-06 | 2 highs fixed and re-tested | 2026-06 | Head of Security |

## 8. Sample artifact: a findings tracker row

| Finding | Severity | System | Raised | Owner | Fix due | Status | Re-test date | Result |
|---------|----------|--------|--------|-------|---------|--------|--------------|--------|
| Unpatched web server | High | Core payments | 2025-06-10 | Platform team | 2025-06-24 | Closed | 2025-07-01 | Verified fixed |

## 9. Evidence to keep

The testing programme and calendar, dated test reports for critical systems, tester qualification and independence records (and insurance for external testers), the findings tracker showing fixes and re-tests, and, if in scope, TLPT scope documents, threat intelligence and red team reports, control-team logs, and the regulator attestation.

## 10. Common mistakes

- Ad hoc testing with no risk-based plan.
- A critical system missed because the inventory was incomplete.
- Findings that are logged but never fixed or re-tested.
- Assuming standard pen testing meets the TLPT duty. It does not.
- Leaving in-scope third parties out of TLPT scope.

## 11. Quick self-check

- Can you show that every critical system was tested in the last 12 months? If not, close the coverage gap.
- When you find a serious issue, can you prove it was fixed and re-tested? If not, fix the findings workflow.
- Do you know for certain whether you are named for TLPT? If not, ask your regulator before assuming you are out.
