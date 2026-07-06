# Model Policy: Information Security Policy

> **Skeleton draft, not legal advice.** Fill the [brackets], delete what does not apply, and have the management body approve the final version. Keep regulatory figures pointing to [docs/regulatory-references.md](../../docs/regulatory-references.md). Gives effect mainly to DORA Art. 9 and the ICT risk RTS (EU) 2024/1774.

| Field | Value |
|---|---|
| Document owner | [CISO] |
| Approved by | [Board / Risk Committee], minute ref [___] |
| Version / date | [v1.0] / [YYYY-MM-DD] |
| Next review | [YYYY-MM-DD] (at least yearly) |
| Applies to | All staff, contractors, systems, and data of [Entity] |

## 1. Purpose

Protect the confidentiality, integrity, and availability of [Entity]'s information and ICT systems, in support of DORA Art. 9 (protection and prevention).

## 2. Principles

- Least privilege: people and systems get only the access they need.
- Defence in depth: no single control is relied on alone.
- Secure by default: systems are built from hardened baselines.
- Evidence: every control is not just set but checked, with records.

## 3. Control standards (minimum baseline)

These are sensible defaults. Set [Entity]'s own numbers and confirm they meet or exceed any regulatory or contractual minimum.

| Domain | Standard |
|---|---|
| Access control | Least privilege; access reviewed every [90] days; joiners/movers/leavers actioned within [1] business day |
| Authentication | Multi-factor authentication for all remote and administrative access |
| Encryption | Data encrypted in transit; sensitive data encrypted at rest |
| Patching | Critical patches within [14] days; high within [30] days |
| Change management | All production changes recorded and approved; emergency changes reviewed after the fact |
| Secure configuration | Hardened baselines; default credentials removed |
| Logging | Security logs kept [12] months and protected from tampering |
| Malware / endpoint | Endpoint protection on all managed devices, kept current |
| Vulnerability mgmt | Regular scanning; findings triaged and fixed to deadline |
| Data classification | Information classified and handled per its sensitivity |
| Physical / environmental | Access to facilities and data centres controlled |
| Secure development | Where [Entity] builds software: secure SDLC and code review |

## 4. Roles

[CISO] owns the standards; system owners implement them; Risk/Compliance oversees; Internal Audit tests independently.

## 5. Exceptions

Any deviation is risk-assessed, time-limited, approved by [role], recorded in an exceptions register, and reviewed at expiry.

## 6. Monitoring and enforcement

Control operation is checked, not assumed. Breaches of this policy are handled under [Entity]'s disciplinary and incident processes.

## 7. Related documents

ICT Risk Management Policy; Incident Management & Reporting Policy; BC/DR Policy; the security control standards in playbook 01; docs/regulatory-references.md.

## 8. Review

Reviewed at least yearly and after any major incident; re-approved by the management body; approval recorded in minutes (evidence for RM-04).
