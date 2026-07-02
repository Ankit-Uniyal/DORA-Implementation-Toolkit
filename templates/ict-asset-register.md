# Template: ICT Asset and Dependency Register

Supports DORA Art. 8 (identification). Keep a complete, classified list of your information assets, ICT assets, and how they depend on each other, linked to the business functions they support and the third parties involved. Update it regularly and after major changes.

Copy this table into a spreadsheet for daily use, or keep it here in the repo. One row per asset.

| Field | Description |
|---|---|
| Asset ID | Unique identifier |
| Asset name | Name or label |
| Asset type | Information asset / application / system / infrastructure / data store |
| Description | Short purpose |
| Business function(s) supported | Linked function(s) |
| Critical or important function? | Yes / No |
| Confidentiality, integrity, availability rating | For example High, Medium, Low for each |
| Overall criticality | Critical / High / Medium / Low |
| Owner (business) | Accountable owner |
| Technical custodian | IT or ops owner |
| Hosting or location | On-premise / cloud / region |
| Data classification | Public / Internal / Confidential / Restricted |
| Personal data? | Yes / No (GDPR relevance) |
| Upstream dependencies | Assets or services it relies on |
| Downstream dependencies | Assets or services that rely on it |
| Supporting ICT third party | Provider (link to third-party register) |
| RTO and RPO | Recovery objectives |
| Last risk assessment | Date |
| Last review | Date |
| Notes | Free text |

## Example row

| Asset ID | Asset name | Type | Critical or important? | Overall criticality | Owner | Third party | RTO | RPO |
|---|---|---|---|---|---|---|---|---|
| APP-014 | Core payment processing | Application | Yes | Critical | Head of Payments | CloudProvider Ltd | 2h | 15m |

## Maintenance checklist

- Reconcile to production regularly to catch shadow IT.
- Re-classify criticality after major changes.
- Link each critical or important asset to its third-party arrangement.
- Confirm RTO and RPO match the BC and DR plans.
