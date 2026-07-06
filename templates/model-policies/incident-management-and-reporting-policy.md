# Model Policy: ICT Incident Management and Reporting Policy

> **Skeleton draft, not legal advice.** Fill the [brackets], delete what does not apply, and have the management body approve the final version. All thresholds and deadlines live in [docs/regulatory-references.md](../../docs/regulatory-references.md) - do not hard-code them here. Gives effect to DORA Art. 17 to 23, the Classification RTS (EU) 2024/1772, and the Reporting RTS (EU) 2025/301.

| Field | Value |
|---|---|
| Document owner | [Incident Manager] |
| Reporting owner (pre-named) | [Name] / backup [Name] |
| Approved by | [Board / Risk Committee], minute ref [___] |
| Version / date | [v1.0] / [YYYY-MM-DD] |
| Next review | [YYYY-MM-DD] (at least yearly) |

## 1. Purpose

Ensure [Entity] detects, manages, and learns from ICT-related incidents, and reports major incidents to its competent authority accurately and inside the legal deadlines.

## 2. The flow

Detect - log - classify - contain - recover - report - review. Everyone on call can follow the incident runbook in playbook 02 at any hour.

## 3. Classification

Every incident is assessed against the DORA Art. 18 criteria and the thresholds in the Classification RTS (EU) 2024/1772, using the [incident classification aid](../incident-classification-aid.md). An incident is major when it affects critical services and either the data-losses trigger is met or two or more other thresholds are met. The exact thresholds are maintained in docs/regulatory-references.md.

## 4. Reporting a major incident (the legal clock)

The [Reporting owner] submits the initial, intermediate, and final reports inside the deadlines set in the Reporting RTS (EU) 2025/301 and recorded in docs/regulatory-references.md (section 3), using the report content fields in that file (section 4). Build these rules in:

- If a deadline cannot be met, tell the competent authority **before** it passes and explain why.
- Late classification: the initial-notification clock runs from the moment of classification.
- Confirm whether weekend/bank-holiday relief applies to [Entity] or is switched off.

Reporting a major incident late, or not at all, is a **breach**, regardless of how well the incident was otherwise handled.

## 5. Client and stakeholder notification

Where clients are affected, [Entity] tells them without undue delay, with protective advice, using the pre-approved client-notification template.

## 6. Voluntary threat notification and payment incidents

[Entity] assesses significant cyber threats for voluntary notification (Art. 19), and captures payment-related operational/security incidents under the same regime where applicable (Art. 23).

## 7. Roles

| Role | Responsibility |
|---|---|
| On-call lead | Detect, open, triage, escalate |
| Incident Manager | Own the incident; classify; drive recovery |
| Reporting owner | Submit regulator reports on time and complete |
| Tech team | Contain and recover |
| Comms | Client and stakeholder communications |
| Management body | Informed; makes reserved decisions |

## 8. Exercises

At least [yearly], [Entity] runs a timed tabletop against the real first-report deadline and fixes the weak points found.

## 9. Related documents

Incident classification aid; client-notification template; ICT Risk Management Policy; competent-authorities.md; docs/regulatory-references.md.

## 10. Review

Reviewed at least yearly and after any major incident; re-approved by the management body (evidence for INC-01 to INC-09).
