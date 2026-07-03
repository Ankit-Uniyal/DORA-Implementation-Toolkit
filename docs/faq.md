docs/faq.md# DORA FAQ: What Compliance Really Means (and What It Does Not)

**Last reviewed: 3 July 2026.** Plain-English answers to the questions people ask
most when they start. This is guidance, not legal advice. Confirm anything that
affects your legal position with your competent authority and your lawyer.

---

## "How do we get DORA certified or accredited?"

**You do not, because there is no such thing.** This is the single biggest
misunderstanding, so read this carefully.

DORA is a **regulation you must comply with**, enforced by supervisors. It is
**not a certification scheme** like ISO/IEC 27001, where an accredited body
audits you and issues a certificate. There is:

- **no "DORA certificate",**
- **no accredited "DORA certification body",**
- **no official "DORA compliant" badge or logo you can earn or display.**

Any vendor selling you a "DORA certification" is selling you their own opinion,
not an official status. It may still be useful evidence, but it does not make you
compliant and it is not recognised in law.

### So what does "being compliant" actually look like?

Compliance under DORA is a **continuous, self-evidenced state**, checked through
**supervision**, not a one-off exam. In practice it means:

1. You **build and run** the controls DORA requires across the five pillars and
   governance (use the implementation playbooks).
2. You **hold evidence** that they work (use the control-mapping and the
   "evidence to keep" lists in each guide).
3. Your **management body owns and approves** the framework (DORA Art. 5).
4. Your **national competent authority (NCA) supervises** you, and can ask for
   information, inspect, and require fixes at any time.
5. Your **internal audit** (and, if you choose or your NCA expects it, an
   **external reviewer**) periodically tests the programme (use docs/3-audit).

The closest thing to a "result" is: a clean internal-audit or external-assurance
opinion, a complete evidence set, and no open regulatory findings. That is what
"audit-ready" means in this toolkit. It is not a certificate; it is a defensible,
evidenced position you can show a supervisor on demand.

---

## "Who actually checks us? Who is our regulator?"

Your **national competent authority (NCA)** — the supervisor for your entity type
in your Member State. Which authority depends on what kind of firm you are (bank,
payment/e-money firm, investment firm, crypto-asset service provider, insurer,
etc.) and where you are authorised. See docs/competent-authorities.md for the
list and links.

The three **European Supervisory Authorities (ESAs)** — EBA, ESMA, EIOPA — sit
above the NCAs, write the technical standards, and jointly run the **Lead
Overseer** role for **critical ICT third-party providers (CTPPs)**. As a normal
financial entity you deal with your NCA; you do not deal with the ESAs directly
unless you are a designated CTPP.

---

## "We are a small startup. Does DORA even apply to us?"

Almost certainly yes, if you are an authorised or registered financial entity
(see the list in docs/proportionality-guide.md). Being small does **not** exempt
you. What changes is **how much formality** is required:

- Some smaller/lower-risk firms may use the **simplified ICT risk management
  framework** (DORA Art. 16). It is lighter, not absent.
- The **hard legal duties still apply**: classify and report major incidents on
  time, keep and submit the register of information, and run baseline testing.

Work through the proportionality guide and **write down** your conclusion with
reasons — that record is itself evidence a supervisor will expect.

---

## "Does ISO 27001 (or SOC 2, or our cloud provider's certificates) make us DORA compliant?"

No, but they help a lot. Standards and provider attestations are **excellent
evidence** for many DORA controls, and you should reuse them (see
docs/1-gap-assessment/control-mapping.md). But:

- DORA asks for things **no general standard covers**: incident-reporting
  deadlines, the register of information, contractual exit testing, and TLPT.
- Being certified to a standard is **evidence of a control**, not proof of DORA
  compliance. You still have to link the evidence to DORA and fill the gaps.

---

## "What are the hard legal deadlines we absolutely cannot miss?"

See docs/regulatory-references.md for the exact figures and citations. In short:

- **Report a major incident** — initial notification within **4 hours** of
  classifying it as major (and no later than **24 hours** from awareness),
  intermediate within **72 hours**, final within **1 month**.
- **Submit the register of information** to your NCA at least **yearly**.
- **Run TLPT** if your authority names you for it.

Missing these is a breach **even if the rest of your programme is excellent**.
The toolkit marks these as `(legal)` items — treat them as top priority.

---

## "What happens if we get it wrong?"

DORA is supervised like other financial regulation. Consequences can include
requests for information, inspections, mandatory remediation, public statements,
and administrative penalties, applied under your NCA's national powers. The point
of this toolkit is to keep you demonstrably ahead of that: build the controls,
hold the evidence, fix the legal items first.

---

## "Where do we start?"

1. Read docs/glossary.md and docs/proportionality-guide.md.
2. Run the gap assessment (docs/1-gap-assessment/).
3. Follow docs/implementation-roadmap.md, fixing `(legal)` items first.
4. Keep docs/regulatory-references.md open for the real numbers.
5. Use docs/3-audit/ to check yourself the way a supervisor would.
