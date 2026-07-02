# Template — TLPT Scoping Worksheet

Supports DORA Art. 26-27 and the RTS on TLPT (aligned to TIBER-EU). Use only if your entity is **identified by the competent authority as in scope** for threat-led penetration testing. Confirm applicability with your authority before proceeding.

> TLPT is performed on **live production** systems and covers **critical or important functions**. It must follow the RTS/TIBER-EU methodology, with authority validation of scope and a final attestation.

---

## 1. Applicability

| Question | Answer |
|----------|--------|
| Has the competent authority identified the entity as in scope for TLPT? | Yes / No |
| Date of identification / reference | |
| Required frequency (default: at least every 3 years) | |
| Last TLPT completed (date) | |
| Next TLPT due | |

## 2. Scope definition

| Item | Detail |
|------|--------|
| Critical/important functions in scope | |
| Underlying systems, applications, infrastructure | |
| Data flows and external interfaces | |
| In-scope ICT third-party providers | |
| Pooled testing arrangement? (shared providers) | Yes / No |
| Out-of-scope items & rationale | |
| Authority scope validation date | |

## 3. Roles

| Role | Party | Notes |
|------|-------|-------|
| Control team (internal) | | Oversees the test, manages risk to production |
| Threat intelligence provider | | Produces targeted threat intel |
| Red team provider | | Conducts the attack simulation |
| Internal tester (if used) | | Additional Art. 27 conditions apply |
| Authority / TLPT cyber team | | Validation & oversight |

## 4. Tester requirements checklist (Art. 27)

- [ ] Highest suitability and reputation.
- [ ] Technical/organisational capability; expertise in threat intel, pen testing, red teaming.
- [ ] Certification or adherence to a formal code of conduct/framework.
- [ ] (External) professional indemnity insurance in place.
- [ ] Conflicts of interest assessed and managed (especially for internal testers).
- [ ] Authority approval obtained where internal testers are used.

## 5. TIBER-EU phase plan

| Phase | Key activities | Owner | Target dates | Status |
|-------|----------------|-------|--------------|--------|
| Preparation | Scoping, procurement, risk management, authority engagement | | | |
| Threat intelligence | Targeted threat intelligence report; scenario design | | | |
| Red teaming | Attack simulation on production against scenarios | | | |
| Closure | Findings, remediation planning, replay/purple teaming, reporting | | | |

## 6. Deliverables & attestation

- [ ] Threat intelligence report.
- [ ] Red team test report (findings, evidence).
- [ ] Remediation plan with owners and dates.
- [ ] Summary provided to the authority.
- [ ] **Authority attestation** received confirming the test met requirements.

## 7. Risk management during testing

Document safeguards to protect production: pre-agreed rules of engagement, "legs-up" procedures, real-time control-team monitoring, escalation and abort criteria, and post-test clean-up verification.
