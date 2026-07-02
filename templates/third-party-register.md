# Template — ICT Third-Party Register of Information

Supports DORA Art. 28(3). Maintain a register of all contractual arrangements for the use of ICT services, distinguishing those supporting critical or important functions. This must be reported to the competent authority at least annually.

> **Align to the official ITS on the register of information.** The ESAs publish a detailed, structured template (multiple linked tables covering the entity, providers, contractual arrangements, functions, and assessments). The fields below are a practical working subset — confirm and expand against the current ITS before regulatory submission.

## Core fields (one row per contractual arrangement)

| Field | Description |
|-------|-------------|
| Arrangement ID | Unique reference |
| Provider legal name | ICT third-party service provider |
| Provider identifier | LEI or equivalent |
| Provider country | Country of establishment |
| Service description | Nature of ICT service |
| Service type | e.g. cloud, software, data centre, network, managed service |
| Supports critical/important function? | Yes / No |
| Function(s) supported | Linked business function(s) |
| Contract start / end | Dates |
| Notice period | For termination |
| Data locations | Where data is stored/processed |
| Sub-outsourcing? | Yes / No; if yes, chain and countries |
| Substitutability | Easy / Difficult / Not substitutable |
| Concentration flag | Multiple critical functions on this provider? |
| Audit/access rights secured? | Yes / No |
| TLPT cooperation clause (if C/I)? | Yes / No / N/A |
| Exit strategy documented? | Yes / No |
| Exit strategy tested? | Yes / No / date |
| CTPP designated? | Yes / No / Unknown |
| Risk rating | Critical / High / Medium / Low |
| Contract owner | Accountable owner |
| Last due diligence | Date |
| Last review | Date |

---

## Example row

| Arrangement ID | Provider | Country | Supports C/I? | Function | Substitutability | CTPP? | Exit tested? |
|----------------|----------|---------|---------------|----------|------------------|-------|--------------|
| TPA-007 | CloudProvider Ltd | IE | Yes | Core payments hosting | Not substitutable | Unknown | 2025-11 (tabletop) |

## Maintenance checklist

- [ ] Reconcile against accounts-payable and cloud/SaaS inventories for completeness.
- [ ] Include intra-group ICT arrangements.
- [ ] Flag and monitor concentration (single provider, many critical functions).
- [ ] Track sub-outsourcing changes and third-country exposure.
- [ ] Confirm annual submission to the competent authority is scheduled.
