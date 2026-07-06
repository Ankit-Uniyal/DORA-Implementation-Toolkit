# Model Policy: Business Continuity and Disaster Recovery Policy

> **Skeleton draft, not legal advice.** Fill the [brackets], delete what does not apply, and have the management body approve the final version. Keep regulatory figures pointing to [docs/regulatory-references.md](../../docs/regulatory-references.md). Gives effect to DORA Art. 11 (response and recovery) and Art. 12 (backup, restoration, recovery).

| Field | Value |
|---|---|
| Document owner | [Continuity lead] |
| Approved by | [Board / Risk Committee], minute ref [___] |
| Version / date | [v1.0] / [YYYY-MM-DD] |
| Next review | [YYYY-MM-DD] (at least yearly and after any major incident or test) |
| Applies to | All critical or important functions of [Entity] |

## 1. Purpose

Ensure [Entity] can keep delivering, or quickly recover, its critical or important functions during and after an ICT disruption, and can restore data with minimal loss.

## 2. Recovery objectives

Each critical or important function has an agreed Recovery Time Objective (RTO, maximum downtime) and Recovery Point Objective (RPO, maximum data loss), set from business impact, approved by the business owner, and proven by testing. Example tiering (replace with your own):

| Tier | Example functions | RTO | RPO |
|---|---|---|---|
| 1 Critical | Payments, customer access | [2 hours] | [15 minutes] |
| 2 Important | Reporting, reconciliation | [8 hours] | [4 hours] |
| 3 Standard | Internal admin tools | [48 hours] | [24 hours] |

## 3. Continuity and recovery plans

For each critical function, [Entity] maintains a plan that names who does what, the recovery steps, dependencies, and communications. Plans are stored where they are reachable during an outage (including offline).

## 4. Backups (Art. 12)

- Backups run by criticality and cover data needed to restore critical functions.
- Backups are segregated from live systems so one attack cannot destroy both.
- Restores are tested at least [yearly] and results recorded, proving recovery inside the RTO and within the RPO.
- [State encryption and retention for backups.]

## 5. Crisis management and communications

A crisis-management approach names the decision-makers, escalation, and internal and external communications (including to clients and, where relevant, the regulator via the Incident Management & Reporting Policy).

## 6. Testing

Continuity and recovery arrangements are tested on a risk basis: at minimum a [yearly] restore test and a [yearly] scenario or tabletop exercise for critical functions. Findings are tracked to closure and fed back into the plans.

## 7. Roles

[Continuity lead] owns the policy and plans; system and function owners execute recovery; IT Operations runs backups and restores; the management body is informed and makes crisis decisions reserved to it.

## 8. Related documents

ICT Risk Management Policy; Incident Management & Reporting Policy; the recovery worked examples in playbook 01; docs/regulatory-references.md.

## 9. Review

Reviewed at least yearly and after any major incident or test; re-approved by the management body (evidence for RM-06 and RM-07).
