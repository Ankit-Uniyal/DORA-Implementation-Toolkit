# Template — ICT Asset & Dependency Register

Supports DORA Art. 8 (identification). Maintain a complete, classified inventory of information assets, ICT assets and their interdependencies, linked to the business functions they support and the third parties involved. Update periodically and after major changes.

> Copy this table into a spreadsheet for day-to-day use, or maintain it here in the repo. One row per asset.

| Field | Description |
|-------|-------------|
| Asset ID | Unique identifier |
| Asset name | Name/label |
| Asset type | Information asset / application / system / infrastructure / data store |
| Description | Brief purpose |
| Business function(s) supported | Linked function(s) |
| Critical/important function? | Yes / No |
| Confidentiality / Integrity / Availability rating | e.g. High/Med/Low each |
| Overall criticality | Critical / High / Medium / Low |
| Owner (business) | Accountable owner |
| Technical custodian | IT/ops owner |
| Hosting / location | On-prem / cloud / region |
| Data classification | Public / Internal / Confidential / Restricted |
| Personal data? | Yes / No (GDPR relevance) |
| Upstream dependencies | Assets/services it relies on |
| Downstream dependencies | Assets/services relying on it |
| Supporting ICT third party | Provider (link to third-party register) |
| RTO / RPO | Recovery objectives |
| Last risk assessment | Date |
| Last review | Date |
| Notes | Free text |

---

## Example row

| Asset ID | Asset name | Type | Critical/important? | Overall criticality | Owner | Third party | RTO | RPO |
|----------|-----------|------|---------------------|---------------------|-------|-------------|-----|-----|
| APP-014 | Core payment processing | Application | Yes | Critical | Head of Payments | CloudProvider Ltd | 2h | 15m |

## Maintenance checklist

- [ ] Reconcile to production regularly (detect shadow IT).
- [ ] Re-classify criticality after major changes.
- [ ] Link each critical/important asset to its third-party arrangement.
- [ ] Confirm RTO/RPO are consistent with BC/DR plans.
