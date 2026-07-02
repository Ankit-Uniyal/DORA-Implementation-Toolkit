# Control-to-Requirement Mapping


This matrix links each toolkit control to the relevant DORA articles and, where useful, the supplementing RTS or ITS. Use it to show coverage, to check evidence is complete, and to plan audit sampling.


Article numbers are indicative, based on Regulation (EU) 2022/2554 as published. RTS and ITS references are described in plain terms because their final numbering and dates should be confirmed on EUR-Lex and the ESA websites.


## Pillar 0: Governance and Proportionality


| Control | DORA article(s) | Supplementing standards | Primary evidence |
|---|---|---|---|
| GOV-01 | Art. 5, 6(1) to (3) | RTS on ICT risk management framework | Board minutes; approved framework |
| GOV-02 | Art. 5(2) | | RACI; org chart |
| GOV-03 | Art. 5(2)(f), 6(5) | | Board reporting pack |
| GOV-04 | Art. 5(4) | | Training records |
| GOV-05 | Art. 5(3) | | Budget approvals |
| GOV-06 | Art. 4, 16 | RTS on simplified ICT risk management framework | Proportionality assessment |
| GOV-07 | Art. 6(4), 5(2) | | Audit plan; terms of reference |


## Pillar 1: ICT Risk Management


| Control | DORA article(s) | Supplementing standards | Primary evidence |
|---|---|---|---|
| RM-01 | Art. 6(8) | RTS on ICT risk management framework | Resilience strategy |
| RM-02 | Art. 8 | RTS on ICT risk management framework | Asset and dependency inventory |
| RM-03 | Art. 8(2) to (7) | | Risk assessment; register |
| RM-04 | Art. 9 | RTS on ICT risk management framework | InfoSec policy; control standards |
| RM-05 | Art. 10 | | Monitoring and alert config |
| RM-06 | Art. 11 | | BC and DR plans; RTO and RPO; test reports |
| RM-07 | Art. 12 | | Backup policy; restore-test evidence |
| RM-08 | Art. 13 | | Post-incident reviews; lessons log |
| RM-09 | Art. 13(6) | | Training completion records |
| RM-10 | Art. 6(5) | | Annual review minutes |


## Pillar 2: Incident Management, Classification and Reporting


| Control | DORA article(s) | Supplementing standards | Primary evidence |
|---|---|---|---|
| INC-01 | Art. 17 | | Incident process; RACI |
| INC-02 | Art. 18 | RTS on classification | Classification decision aid |
| INC-03 | Art. 17(3) | | Escalation matrix; exercise reports |
| INC-04 | Art. 19(1) to (4) | ITS on reporting (timelines) | Regulatory submissions |
| INC-05 | Art. 20 | ITS on reporting content and templates | Submitted report forms |
| INC-06 | Art. 19(3) | | Client notification records |
| INC-07 | Art. 19(2) | | Threat-notification triage records |


## Related standards and frameworks: how they map to DORA

DORA tells you what outcomes to achieve, but it does not hand you a full control library or test method. The standards below fill that gap. If you already run one or more of them well, most of your DORA evidence already exists. Your job is to link that existing work to DORA's pillars and prove it.

Important: DORA is the law and standards are helpers. Being certified to a standard does not make you DORA compliant on its own, and DORA can ask for more than a standard does. Use standards to build and evidence controls, then check the result against DORA and its RTS and ITS. Standards get revised over time, so confirm the current version before you rely on any mapping.

### The shortlist (best coverage in a European setting)

- ISO/IEC 27001 and 27002: information security management and controls.
- ISO/IEC 22301: business continuity.
- ISO/IEC 27017 and 27018: cloud security and personal data in the cloud.
- EBA Guidelines on ICT and security risk management, and on outsourcing.
- TIBER-EU: threat-led red team testing (the base for DORA's TLPT).
- NIST Cybersecurity Framework: a clean way to organise the whole programme.

### Standard profiles (what it is, how it helps DORA, where it stops)

| Standard | What it is | How it helps DORA | Where it stops |
|---|---|---|---|
| ISO/IEC 27001 and 27002 | ISMS and security control catalogue | Backbone for Pillar 1 protect and much of detect | No incident deadlines, register format, or TLPT |
| ISO/IEC 27005 | Information security risk method | Repeatable risk method for Pillar 1 (RM-03) | Method only, not a control set |
| ISO/IEC 22301 and 27031 | Business continuity and ICT readiness | Pillar 1 respond and recover, RTO and RPO (RM-06) | Not DORA classification or reporting duties |
| ISO/IEC 27017 and 27018 | Cloud security and cloud personal data | Pillar 4 provider assessment; Pillar 1 protect in cloud | Not contract terms, register, or exit testing |
| ISO/IEC 27036 | Supplier relationship security | Pillar 4 due diligence and monitoring | Not the register format or CTPP oversight |
| ISO/IEC 27035 | Incident management | Pillar 2 incident handling process | Not the DORA reporting deadlines |
| EBA ICT and security risk guidelines | Supervisory guidance | Depth for Pillars 0, 1, and 2 | DORA takes precedence where they overlap |
| EBA outsourcing guidelines | Supervisory guidance | Strong support for Pillar 4 | DORA Art. 28 to 44 and the register ITS are binding |
| TIBER-EU | EU threat-led red team framework | The base for DORA TLPT (Pillar 3, Art. 26 and 27) | Advanced testing only, only for named firms |
| NIS2 | EU network and information security directive | Sits next to DORA in the EU cyber landscape | DORA is lex specialis for financial entities |
| GDPR | EU personal data law | Pillar 2 client notices, Pillar 4 data locations, Pillar 5 safeguards | Governs personal data, not resilience overall |
| NIST CSF | Identify, Protect, Detect, Respond, Recover | Lines up with DORA's five jobs in Pillar 1 | US-origin, no EU-specific duties |
| COBIT | IT governance framework | Pillar 0 governance, roles, and oversight | Governance-focused, not a control set |
| OWASP and PTES | Testing method and standards | Pillar 3 baseline testing depth | Testing methods, not management systems |
| MITRE ATT&CK | Attacker tactics knowledge base | Pillar 3 TLPT scenarios; Pillar 5 threat sharing | A reference, not a process framework |
| SOC 2 and ISAE 3402 | Independent assurance reports | Pillar 4 provider evidence where direct audit is hard | You still need DORA terms, audit rights, exit tests |

### Pillar-by-pillar mapping

| DORA pillar | Primary standards | Supporting standards |
|---|---|---|
| Pillar 0 Governance (Art. 5, 6) | COBIT; EBA ICT guidelines | NIST CSF (Identify); ISO/IEC 27001 leadership clauses |
| Pillar 1 ICT risk management (Art. 5 to 16) | ISO/IEC 27001 and 27002; ISO/IEC 22301 | ISO/IEC 27005; 27031; 27017; 27018; NIST CSF |
| Pillar 2 Incident management (Art. 17 to 23) | ISO/IEC 27035; EBA ICT guidelines | NIST CSF (Respond, Recover); GDPR |
| Pillar 3 Resilience testing (Art. 24 to 27) | TIBER-EU; OWASP; PTES | MITRE ATT&CK; ISO/IEC 27001 |
| Pillar 4 Third-party risk (Art. 28 to 44) | EBA outsourcing guidelines; ISO/IEC 27036 | ISO/IEC 27017 and 27018; SOC 2; ISAE 3402 |
| Pillar 5 Information sharing (Art. 45) | Traffic Light Protocol; MITRE ATT&CK | GDPR; sector sharing community rules |

### Control-family cross-reference

| Control family | Toolkit controls | Best-fit standards |
|---|---|---|
| Governance and oversight | GOV-01 to GOV-07 | COBIT; EBA ICT guidelines; ISO/IEC 27001 clauses 5 and 9 |
| Asset and dependency management | RM-02 | ISO/IEC 27002; NIST CSF (Identify) |
| Risk assessment | RM-03 | ISO/IEC 27005; NIST CSF |
| Access control and authentication | RM-04 | ISO/IEC 27002; ISO/IEC 27017 |
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

### How to use standards without doubling your work

1. Start from what you already run. List your current certifications and frameworks.
2. Map them to the pillars using the tables above. Mark the DORA controls they already cover.
3. Find the gaps. These are usually the DORA-specific items no general standard covers: the register of information, incident reporting deadlines, exit testing, and TLPT.
4. Reuse the evidence. An ISO/IEC 27001 audit report, a 22301 continuity test, or a provider SOC 2 report can all be DORA evidence when you link them to a control.
5. Do not assume certification equals compliance. Always check the result against DORA and the current RTS and ITS.
