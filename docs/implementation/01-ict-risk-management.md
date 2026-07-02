# Pillar 1 — ICT Risk Management

**DORA articles:** Art. 5–16 (ICT risk management framework and its components). Supplemented by RTS on ICT risk management framework and the simplified ICT risk management framework.

---

## 1. Purpose

The ICT risk management framework is the foundation of DORA. It requires financial entities to identify, protect, detect, respond to, and recover from ICT risks across their entire technology estate, on a continuous basis, and to learn and evolve.

## 2. Structure of the framework (Art. 6)

The framework must be documented, reviewed **at least once a year** (and after major incidents or following supervisory instructions), and continuously improved. It must include the strategies, policies, procedures, ICT protocols and tools needed to protect all information and ICT assets. Entities must maintain a **digital operational resilience strategy** setting how the framework is implemented, including risk tolerance levels, objectives, and a reference architecture.

## 3. Framework components (Art. 7–13)

### 3.1 ICT systems, protocols and tools (Art. 7)
Use and maintain ICT systems that are reliable, resilient, with sufficient capacity, and technologically resilient to handle peak conditions and adverse scenarios.

### 3.2 Identification (Art. 8)
- Identify, classify and adequately document all ICT-supported business functions, roles and responsibilities, the information assets and ICT assets supporting them, and their interdependencies.
- Maintain an inventory and update it periodically and after major changes.
- Identify all sources of ICT risk, and assess cyber threats and vulnerabilities relevant to functions/assets.
- Perform a risk assessment upon each major change.
- Map dependencies on ICT third-party service providers.

### 3.3 Protection and prevention (Art. 9)
- Continuously monitor and control the security and functioning of ICT systems and tools.
- Minimise the impact of ICT risk through appropriate strategies, policies, procedures and tools.
- Design and implement an information security policy defining rules to protect confidentiality, integrity, availability and authenticity of data.
- Implement identity and access management, strong authentication, network security, encryption/cryptographic controls, secure configuration, change management, and patching.

### 3.4 Detection (Art. 10)
- Have mechanisms to promptly detect anomalous activities, ICT network performance issues and ICT-related incidents.
- Define multiple layers of control, alert thresholds and criteria to trigger incident detection/response.

### 3.5 Response and recovery (Art. 11)
- Put in place an **ICT business continuity policy**, including plans, response and recovery measures, and communication.
- Set recovery objectives (RTO/RPO) so that recovery is possible with minimal disruption.
- Ensure at least one set of restoration capabilities and redundancy.
- Test the plans periodically.

### 3.6 Backup and restoration (Art. 12)
- Develop backup policies and procedures specifying scope and minimum frequency based on criticality.
- Keep backup systems physically and logically segregated from source systems.
- Maintain redundant ICT capacity with adequate resources and functions.

### 3.7 Learning and evolving (Art. 13)
- Gather information on vulnerabilities, cyber threats, incidents (especially cyber-attacks) and analyse likely impacts.
- Conduct post-incident reviews after significant disruptions.
- Continuously develop ICT security awareness programmes and digital operational resilience training for staff and management.

### 3.8 Communication (Art. 14)
- Have crisis communication plans for disclosing incidents/vulnerabilities to clients, counterparts and the public as appropriate.

## 4. Control objectives

| ID | Control objective |
|----|-------------------|
| RM-01 | A board-approved digital operational resilience strategy defines risk tolerance and objectives. |
| RM-02 | A complete, current inventory of business functions, information assets, ICT assets and interdependencies is maintained. |
| RM-03 | ICT risks are identified and assessed on a continuous basis and upon major change. |
| RM-04 | An information security policy and supporting controls (IAM, encryption, network, change, patch) are implemented and enforced. |
| RM-05 | Detection mechanisms with defined thresholds identify anomalies and incidents promptly. |
| RM-06 | ICT business continuity and response/recovery plans exist, with defined RTO/RPO, and are tested. |
| RM-07 | Backups are policy-driven, segregated, and restoration is periodically tested. |
| RM-08 | Post-incident reviews and threat intelligence feed continuous improvement. |
| RM-09 | Security awareness and resilience training programmes operate for all staff and the management body. |
| RM-10 | The framework is reviewed at least annually and after major incidents. |

## 5. Implementation steps

1. **Draft the resilience strategy** with explicit risk tolerance/appetite statements and objectives; obtain board approval.
2. **Build the asset & dependency inventory** (link to the ICT asset register template). Classify by criticality and map to business functions and third parties.
3. **Run the initial risk assessment** across the estate; establish a repeatable methodology and register.
4. **Codify the information security policy** and the underlying control standards (IAM, cryptography, network segmentation, secure configuration, vulnerability & patch management, change management).
5. **Stand up detection & monitoring** (logging, SIEM/monitoring, alerting thresholds, use cases).
6. **Build BC/DR capability**: define RTO/RPO per critical function, document response & recovery plans, establish redundancy, and schedule tests.
7. **Implement backup regime**: policy, frequency by criticality, segregation, and periodic restore testing.
8. **Establish the learning loop**: threat-intel intake, post-incident reviews, lessons-learned tracking, and metrics.
9. **Roll out awareness & training** with role-based content and completion tracking.
10. **Institutionalise annual review** and event-driven updates of the whole framework.

## 6. Evidence to retain

- Approved resilience strategy and ICT risk framework document (versioned).
- Asset/dependency inventory extract and classification methodology.
- Risk assessment methodology and current risk register.
- Information security policy and control standards.
- Monitoring/alerting configuration and sample alerts.
- BC/DR plans, RTO/RPO definitions, and test reports.
- Backup policy and restore-test evidence.
- Post-incident review reports and lessons-learned log.
- Training completion records.
- Annual review minutes/change history.

## 7. Common pitfalls

- Incomplete asset inventory (shadow IT, undocumented dependencies, missing third-party links).
- RTO/RPO defined on paper but never validated by testing.
- Backups not segregated (vulnerable to the same ransomware event as production).
- "Annual review" that is a rubber stamp rather than a genuine reassessment.
- Training that is generic rather than role-based and risk-relevant.
