# Pillar 2 — ICT-Related Incident Management, Classification & Reporting

**DORA articles:** Art. 17 (incident management process), Art. 18 (classification of incidents and cyber threats), Art. 19 (reporting of major ICT-related incidents and voluntary notification of significant cyber threats), Art. 20 (harmonised reporting content and templates), Art. 21 (centralisation / single EU Hub — feasibility), Art. 22 (supervisory feedback), Art. 23 (operational or security payment-related incidents). Supplemented by the RTS/ITS on classification and on reporting content, templates and timelines.

---

## 1. Purpose

DORA requires a consistent, documented process to detect, manage, log and report ICT-related incidents, plus a harmonised approach to classifying their severity and reporting **major** incidents to the competent authority within strict deadlines.

## 2. Incident management process (Art. 17)

Establish and implement an ICT-related incident management process to detect, manage and notify incidents. Requirements include:
- Procedures to identify, track, log, categorise and classify incidents by priority, severity and criticality of affected services.
- Assigned roles and responsibilities for different incident types and scenarios.
- Plans for communication to staff, external stakeholders, media, and (where relevant) clients, and for internal escalation including complaints.
- Ensuring at least major incidents are reported to relevant senior management, with impact, response and additional controls to be established.
- Response procedures to mitigate impacts and ensure services become operational and secure.

## 3. Classification (Art. 18)

Classify incidents and determine their impact using criteria set out in DORA and detailed in the RTS. The primary classification criteria include:
- Number and/or relevance of **clients, financial counterparts and transactions** affected.
- **Reputational impact**.
- **Duration** of the incident, including service downtime.
- **Geographical spread** (areas affected, especially cross-border).
- **Data losses** — impact on availability, authenticity, integrity or confidentiality of data.
- **Criticality of services affected**, including the entity's critical/important functions.
- **Economic impact** in absolute and relative terms.

An incident is classified as **major** when it meets the materiality thresholds defined in the RTS across these criteria. **Significant cyber threats** are classified using criticality of services at risk, number of affected parties, and geographical spread.

## 4. Reporting of major incidents (Art. 19)

Report major ICT-related incidents to the relevant competent authority. Reporting is staged:
- **Initial notification** — submitted within the early deadline after classification as major.
- **Intermediate report** — when the status of the original incident has changed significantly or handling has changed based on new information, and thereafter on updates.
- **Final report** — when the root-cause analysis is complete (regardless of whether mitigation measures are implemented) and actual impact figures are available.

> **Deadlines are defined in the ITS on reporting.** Exact hour-based timelines for initial, intermediate and final reports must be confirmed against the current official ITS text before relying on them operationally. Build your runbook around the confirmed timelines.

Entities **may**, on a voluntary basis, notify **significant cyber threats** to the competent authority when they deem the threat relevant to the financial system, service users or clients. Where an incident affects clients, the entity must inform them without undue delay and communicate protective measures.

## 5. Harmonised content & templates (Art. 20)

The ESAs develop standard forms, templates and procedures for reporting. Align your reporting fields to the ITS template so submissions are complete and machine-consumable.

## 6. Payment-related operational/security incidents (Art. 23)

The incident-management and reporting requirements also apply to **operational or security payment-related incidents** and to major ones concerning credit institutions, payment institutions, account information service providers and e-money institutions.

## 7. Control objectives

| ID | Control objective |
|----|-------------------|
| INC-01 | A documented incident management process defines detection, logging, categorisation, escalation and closure. |
| INC-02 | Incident classification applies the DORA/RTS criteria and thresholds consistently. |
| INC-03 | Roles, responsibilities and an on-call/escalation matrix are defined and tested. |
| INC-04 | Major incidents are reported to the competent authority within the mandated initial/intermediate/final deadlines. |
| INC-05 | Reporting content aligns to the ITS templates and is complete and accurate. |
| INC-06 | Clients are informed without undue delay where they are affected, with protective guidance. |
| INC-07 | Significant cyber threats are assessed for voluntary notification. |
| INC-08 | Post-incident root-cause analysis feeds lessons learned and framework updates. |
| INC-09 | Payment-related operational/security incidents are captured under the same regime where applicable. |

## 8. Implementation steps

1. Document the process end to end (detect, triage, classify, contain, eradicate, recover, report, review) with a RACI.
2. Codify classification as a decision aid encoding the RTS criteria and thresholds (see the incident classification template).
3. Build the regulatory reporting runbook with the confirmed initial/intermediate/final deadlines and the ITS template fields.
4. Set up tooling and logging to capture incident timeline, evidence and classification inputs.
5. Define client and stakeholder communications templates and approval paths.
6. Establish threat-notification triage to decide on voluntary cyber-threat notification.
7. Run exercises (tabletop and technical) to validate detection, escalation and reporting within deadlines.
8. Integrate lessons learned into the ICT risk framework and controls.

## 9. Evidence to retain

- Incident management policy/procedure and RACI.
- Classification decision aid and worked examples.
- Incident register with timelines, classifications and evidence.
- Copies of initial/intermediate/final regulatory submissions and acknowledgements.
- Client notification records where applicable.
- Post-incident review reports.
- Exercise reports demonstrating deadline adherence.

## 10. Common pitfalls

- No pre-agreed classification thresholds, leading to inconsistent or late "major" determinations.
- Reporting runbook that cannot meet the initial-notification deadline due to unclear ownership or slow internal escalation.
- Incomplete incident logging, so the final report lacks accurate impact figures and root cause.
- Forgetting that payment-related security incidents fall within scope.
