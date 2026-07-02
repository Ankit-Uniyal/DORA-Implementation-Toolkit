# Related Standards and Frameworks: How They Map to DORA

A structured, in-depth guide to the standards and frameworks that pair well with DORA (Regulation (EU) 2022/2554), and exactly how each one helps you meet each pillar. Plain English, no em dashes.

DORA tells you what outcomes to achieve, but it does not hand you a full control library or test method. These standards fill that gap. If you already run one or more of them well, most of your DORA evidence already exists. Your job is to link that existing work to DORA's pillars and prove it.

Important: DORA is the law. Standards are helpers. Being certified to a standard does not make you DORA compliant on its own, and DORA can ask for more than a standard does. Use standards to build and evidence controls, then check the result against DORA and its RTS and ITS.

## 1. The shortlist (start here)

If you adopt only a handful, these give the best coverage in a European setting:

- ISO/IEC 27001 and 27002: information security management and controls.
- ISO/IEC 22301: business continuity.
- ISO/IEC 27017 and 27018: cloud security and personal data in the cloud.
- EBA Guidelines on ICT and security risk management, and on outsourcing.
- TIBER-EU: threat-led red team testing (the base for DORA's TLPT).
- NIST Cybersecurity Framework: a clean way to organise the whole programme.

The rest of this page explains each one and maps it to the pillars.

## 2. Standard-by-standard profiles

Each profile covers what it is, who issues it, how it helps DORA, and where it stops.

### ISO/IEC 27001 (ISMS) and ISO/IEC 27002 (controls)

- What it is: a management system for information security (27001) and a catalogue of security controls (27002).
- Who issues it: ISO and IEC.
- How it helps DORA: it is the backbone for Pillar 1 protect and much of detect. Its controls cover access control, cryptography, operations security, logging, supplier relationships, and incident handling. A certified ISMS gives strong, audited evidence.
- Where it stops: it does not cover DORA's specific incident reporting deadlines, the register of information format, or TLPT. It is risk-managed and flexible, so you must show the controls actually cover your critical functions.

### ISO/IEC 27005 (information security risk management)

- What it is: guidance on how to run information security risk assessments.
- How it helps DORA: gives you a repeatable risk method for Pillar 1 (RM-03) and feeds the risk register.
- Where it stops: it is method only, not a control set.

### ISO/IEC 22301 (business continuity) and ISO/IEC 27031 (ICT readiness for continuity)

- What they are: a management system for business continuity (22301) and guidance on ICT readiness for it (27031).
- How they help DORA: directly support Pillar 1 respond and recover (RM-06), including impact analysis, recovery strategies, RTO and RPO, and continuity testing.
- Where they stop: they do not set DORA's incident classification or reporting duties.

### ISO/IEC 27017 (cloud security) and ISO/IEC 27018 (personal data in the cloud)

- What they are: cloud-specific control guidance (27017) and protection of personal data in public cloud (27018).
- How they help DORA: strengthen Pillar 4 third-party work and Pillar 1 protect where you run in the cloud. Useful when assessing cloud providers and their shared-responsibility split.
- Where they stop: they help you assess providers but do not replace DORA's contract terms, register, or exit-testing duties.

### ISO/IEC 27036 (supplier relationships security)

- What it is: guidance on information security in supplier relationships.
- How it helps DORA: supports Pillar 4 due diligence and ongoing monitoring of providers.
- Where it stops: it is security-focused and does not cover the register format or the oversight framework for CTPPs.

### EBA Guidelines on ICT and security risk management

- What they are: supervisory guidelines from the European Banking Authority on managing ICT and security risk.
- How they help DORA: they shaped much of DORA's thinking and remain a good source of expected practice across Pillars 0, 1, and 2. Good for calibrating "what good looks like" for supervisors.
- Where they stop: DORA now takes precedence where they overlap; use the guidelines for depth, not as the primary rule.

### EBA Guidelines on outsourcing arrangements

- What they are: supervisory guidelines on outsourcing, including to the cloud.
- How they help DORA: strong support for Pillar 4, especially due diligence, contract content, concentration risk, sub-outsourcing, and exit planning.
- Where they stop: DORA's Art. 28 to 44 and the register ITS are the binding rules; use these guidelines to enrich your process.

### TIBER-EU (threat intelligence-based ethical red teaming)

- What it is: the European framework for running intelligence-led red team tests, published by the ECB.
- How it helps DORA: it is the base that DORA's TLPT rules (Pillar 3, Art. 26 and 27) are built on. If you are named for TLPT, you will run a TIBER-style test.
- Where it stops: it applies only to advanced testing, not baseline testing, and only to firms named for TLPT.

### NIS2 Directive

- What it is: the EU directive on network and information security for essential and important entities.
- How it helps DORA: it sits alongside DORA in the EU cyber landscape. For groups with mixed entities, understanding both avoids double work and gaps. DORA is the specific law for the financial sector (lex specialis), so it takes priority for in-scope financial entities.
- Where it stops: it is a directive transposed by each Member State, so detail varies by country.

### GDPR (General Data Protection Regulation)

- What it is: the EU law on personal data.
- How it helps DORA: unavoidable across incident handling (Pillar 2 client notices), third-party data locations (Pillar 4), and information sharing (Pillar 5 safeguards). Your DPO should review these areas.
- Where it stops: it governs personal data, not operational resilience as a whole.

### NIST Cybersecurity Framework (CSF)

- What it is: a widely used framework organised around Identify, Protect, Detect, Respond, and Recover.
- How it helps DORA: it lines up almost one-to-one with DORA's five jobs in Pillar 1, so it is a clean way to structure and communicate the whole programme.
- Where it stops: it is US-origin and outcome-based, so it does not carry EU-specific duties like the register or TLPT.

### COBIT

- What it is: a framework for the governance and management of enterprise IT (ISACA).
- How it helps DORA: supports Pillar 0 governance, roles, and oversight, and links IT activity to board accountability.
- Where it stops: it is governance-focused, not a technical control set.

### OWASP resources and PTES

- What they are: the OWASP Testing Guide and Application Security Verification Standard, and the Penetration Testing Execution Standard.
- How they help DORA: concrete method and depth for Pillar 3 baseline testing, especially for applications and penetration tests.
- Where they stop: they are testing methods, not management systems.

### MITRE ATT&CK

- What it is: a knowledge base of real attacker tactics and techniques.
- How it helps DORA: a common language for describing threats. Useful for Pillar 3 TLPT scenario design and Pillar 5 threat sharing.
- Where it stops: it is a reference, not a control or process framework.

### SOC 2 and ISAE 3402 (assurance reports)

- What they are: independent assurance reports on a service provider's controls.
- How they help DORA: key evidence for Pillar 4 when you assess and monitor providers, especially where direct audit is hard.
- Where they stop: they describe the provider's own controls, so you still need DORA contract terms, audit rights, and exit tests.

## 3. Pillar-by-pillar mapping

This table shows which standards do the most work for each DORA pillar.

| DORA pillar | Primary standards | Supporting standards |
|---|---|---|
| Pillar 0 Governance (Art. 5, 6) | COBIT; EBA ICT guidelines | NIST CSF (Identify); ISO/IEC 27001 (leadership clauses) |
| Pillar 1 ICT risk management (Art. 5 to 16) | ISO/IEC 27001 and 27002; ISO/IEC 22301 | ISO/IEC 27005; 27031; 27017; 27018; NIST CSF |
| Pillar 2 Incident management (Art. 17 to 23) | ISO/IEC 27035 (incident management); EBA ICT guidelines | NIST CSF (Respond, Recover); GDPR (for personal-data breaches) |
| Pillar 3 Resilience testing (Art. 24 to 27) | TIBER-EU (for TLPT); OWASP; PTES | MITRE ATT&CK; ISO/IEC 27001 (test controls) |
| Pillar 4 Third-party risk (Art. 28 to 44) | EBA outsourcing guidelines; ISO/IEC 27036 | ISO/IEC 27017 and 27018; SOC 2; ISAE 3402 |
| Pillar 5 Information sharing (Art. 45) | Traffic Light Protocol (handling); MITRE ATT&CK | GDPR (safeguards); sector sharing community rules |

## 4. Control-family cross-reference

A deeper view: common control families, the DORA controls they support (from this toolkit), and where the standards help.

| Control family | This toolkit's controls | Best-fit standards |
|---|---|---|
| Governance and oversight | GOV-01 to GOV-07 | COBIT; EBA ICT guidelines; ISO/IEC 27001 clauses 5 and 9 |
| Asset and dependency management | RM-02 | ISO/IEC 27002 (asset controls); NIST CSF (Identify) |
| Risk assessment | RM-03 | ISO/IEC 27005; NIST CSF |
| Access control and authentication | RM-04 | ISO/IEC 27002; ISO/IEC 27017 (cloud) |
| Cryptography | RM-04 | ISO/IEC 27002 |
| Change and patch management | RM-04 | ISO/IEC 27002 |
| Logging and detection | RM-05 | ISO/IEC 27002; NIST CSF (Detect); MITRE ATT&CK |
| Continuity and recovery | RM-06 | ISO/IEC 22301; ISO/IEC 27031 |
| Backup and restore | RM-07 | ISO/IEC 27002; ISO/IEC 22301 |
| Incident handling | INC-01 to INC-09 | ISO/IEC 27035; NIST CSF (Respond) |
| Testing (baseline) | TST-01 to TST-05 | OWASP; PTES; ISO/IEC 27002 |
| Testing (advanced) | TST-06 to TST-08 | TIBER-EU; MITRE ATT&CK |
| Supplier management | TPP-01 to TPP-09 | EBA outsourcing guidelines; ISO/IEC 27036; SOC 2; ISAE 3402 |
| Threat intelligence sharing | ISH-01 to ISH-05 | Traffic Light Protocol; MITRE ATT&CK |

## 5. How to use standards without doubling your work

1. Start from what you already run. List your current certifications and frameworks.
2. Map them to the pillars using the tables above. Mark the DORA controls they already cover.
3. Find the gaps. These are usually the DORA-specific items no general standard covers: the register of information, incident reporting deadlines, exit testing, and TLPT.
4. Reuse the evidence. An ISO/IEC 27001 audit report, a 22301 continuity test, or a provider SOC 2 report can all be DORA evidence when you link them to a control.
5. Do not assume certification equals compliance. Always check the result against DORA and the current RTS and ITS.

## 6. A note on versions and sources

Standards and guidelines are updated over time (for example ISO revisions, EBA guideline updates, and TIBER-EU releases). Always confirm the current version and read DORA and its RTS and ITS on EUR-Lex and the ESA websites before relying on any mapping for a real compliance or audit job. This page is guidance, not legal advice.
