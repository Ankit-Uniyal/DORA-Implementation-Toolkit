# Worked Example: NovaPay Major-Incident Reports (Initial, Intermediate, Final)

**Fully worked, fictional example.** This shows what the three regulatory reports
for a major incident actually look like when filled in, using the NovaPay scenario
from [model-startup-novapay.md](model-startup-novapay.md) and the
[incident classification aid](../templates/incident-classification-aid.md). The
field sets follow the **Reporting RTS (EU) 2025/301, Art. 1 to 4** and are submitted
on the forms of the **Reporting ITS (EU) 2025/302**; the exact deadlines live in
[regulatory-references.md](../docs/regulatory-references.md).

> Everything below is invented for teaching. In a real filing, use your NCA's
> current portal and the official ITS forms, and confirm every field. This is a
> teaching aid, not evidence of compliance.

## Scenario recap

NovaPay (fictional EU e-money institution, authorised in Ireland, LEI
5493001NOVAPAY0EXAMPLE). At 09:12 an alert fires on failed logins; at 09:40
unauthorised access to the client wallet system (a critical function) is confirmed;
at 10:15 the incident is classified **major** and the reporting clock starts.
Wallet is unavailable 09:40 to 12:00 (2h20m).

Why it is major (from the classification aid): criticality gate passed (successful
malicious unauthorised access to a critical-function system); data-losses trigger
met (Art. 9(5)(b)); downtime > 2h. Any one of the last two, with the gate, is enough.

---

## 1. Initial notification (Art. 2) - due within 4h of classification

Submitted 12:05 (classified 10:15, so ~1h50m in, well inside the 4-hour limit and
inside 24h of awareness).

| Field (RTS 2025/301) | NovaPay entry |
|---|---|
| Submission type | Initial notification |
| Entity name / LEI / type | NovaPay Ltd / 5493001NOVAPAY0EXAMPLE / E-money institution |
| Submitting entity | NovaPay Ltd (on its own behalf) |
| Contact person(s) | [Reporting Owner name], [phone], [email]; backup [name] |
| Parent undertaking | [None / name + LEI] |
| Currency for monetary figures | EUR |
| Incident reference code (internal) | NP-INC-2026-014 |
| Detection date/time | 2026-03-10 09:12 (WET) |
| Classification date/time | 2026-03-10 10:15 (WET) |
| Description | Unauthorised access to the client wallet system following a credential-based attack; wallet access disrupted |
| Classification criteria met | Criticality (malicious unauthorised access to a critical-function system); Data losses (Art. 9(5)(b)); Duration/downtime (> 2h) |
| Member States impacted | Ireland |
| How discovered | SIEM alert on a spike in failed logins, then confirmed unauthorised access |
| Origin (if known) | External; credential-based, under investigation |
| Business continuity plan activated? | Yes - wallet failover and forced credential reset |
| Reclassified to non-major? | No |
| Other relevant info | Law enforcement notification under consideration |

---

## 2. Intermediate report (Art. 3) - due within 72h of the initial

Submitted next day (Day 2), inside the 72-hour window.

| Field | NovaPay entry |
|---|---|
| Authority-assigned reference code | [as issued by the NCA on receipt of the initial] |
| Occurrence date/time | 2026-03-10 09:40 (first confirmed unauthorised access) |
| Recovery date/time | 2026-03-10 12:00 (wallet service restored) |
| How the criteria were met | Malicious access to a critical-function system; access that may cause data loss; wallet downtime 2h20m |
| Incident type | Malicious / cyber (credential compromise) |
| Threats / techniques used | Credential stuffing leading to account takeover of an admin session (under confirmation) |
| Affected functional areas / processes | Client wallet access and authentication |
| Affected infrastructure | Wallet application and its authentication service (single region) |
| Impact on clients' financial interests | No confirmed loss of client funds; ~4% of clients temporarily unable to access wallet |
| Reporting to other authorities | Data protection authority assessment initiated (possible personal-data impact) |
| Temporary / planned recovery measures | Forced password reset, session invalidation, MFA enforcement tightened, blocklist updated |
| Indicators of compromise | Source IP ranges and user-agent strings shared with the SOC (list attached) |

---

## 3. Final report (Art. 4) - due within 1 month of the intermediate

Submitted ~Day 20.

| Field | NovaPay entry |
|---|---|
| Root cause(s) | An admin account without phishing-resistant MFA was taken over via credential stuffing; alerting caught it but session controls were weak |
| Resolution date/time | 2026-03-10 12:00 service restored; remediation completed 2026-03-24 |
| How it was resolved | Compromised sessions killed; credentials reset; phishing-resistant MFA enforced for all admin access; rate-limiting and anomaly detection improved |
| Info for resolution authorities | [If applicable to the entity type; otherwise N/A] |
| Direct/indirect costs, losses, recoveries | Direct response cost ~EUR 30 000; no client-fund loss; no financial recovery claimed |
| Recurring-incident information | Not a recurring incident under Art. 8(2) |
| Lessons learned / actions | MFA policy hardened; tabletop scheduled; detection thresholds tuned; findings tracked to closure |

---

## What this example teaches

- The **classification decision and the clock are explicit and owned** before the
  crisis, so the initial notification lands comfortably inside 4 hours.
- Each report **adds detail** as it becomes known: initial = what/when/why-major;
  intermediate = impact and handling; final = root cause and actual cost.
- The fields come straight from **RTS 2025/301**; the **forms** come from **ITS
  2025/302**; the **deadlines** come from **regulatory-references.md**. Keep the
  numbers in one place.
- NovaPay is an EMI handling payments, so it must check whether the
  weekend/bank-holiday relief is switched off for it (Art. 5(5)-(6)).

Pairs with [playbook 02](../docs/2-implementation/02-incident-management-and-reporting.md),
the [classification aid](../templates/incident-classification-aid.md), and
[competent-authorities.md](../docs/competent-authorities.md).
