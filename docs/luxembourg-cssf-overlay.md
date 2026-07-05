# Luxembourg Overlay: DORA Through the CSSF Lens

**Last verified against CSSF published guidance: 5 July 2026.** This overlay sits
on top of the pan-EU toolkit. DORA is an EU Regulation and applies directly, but
*how* you report, *whom* you notify, and *which* national circulars bind you
depend on your Member State. This file captures the Luxembourg specifics for
entities supervised by the **CSSF**. Insurance and reinsurance undertakings and
their intermediaries are instead supervised by the **Commissariat aux Assurances
(CAA)** and should read the CAA's own DORA guidance.

> This is orientation, not legal advice. Always confirm the live text on the CSSF
> website (https://www.cssf.lu) and EUR-Lex, and speak to qualified Luxembourg
> regulatory counsel before you rely on any point for a real filing.

---

## 1. Who supervises you, and since when

DORA (Regulation (EU) 2022/2554) has applied to in-scope financial entities
across the EU **since 17 January 2025**. The accompanying Directive (EU) 2022/2556
was transposed into Luxembourg law on **1 July 2024** (the "DORA Law"), which
designates the **CSSF** and the **CAA** as the competent authorities responsible
for supervising and enforcing DORA over their respective entities.

If the CSSF authorises or registers you, the CSSF is your DORA competent
authority. Credit institutions that are **significant institutions under direct
ECB supervision** have an additional ECB reporting channel for some processes
(see section 4).

General ICT-risk supervision contact: **ictrisksupervision@cssf.lu**.

---

## 2. The CSSF circulars that turn DORA into local obligations

DORA's Level 1 text and its RTS/ITS are directly applicable, but the CSSF has
issued circulars that specify local modalities. The ones most likely to bind a
CSSF-supervised entity:

| Circular | Subject | Why it matters |
|---|---|---|
| CSSF 25/893 | Reporting of major ICT-related incidents and significant cyber threats under DORA | Sets the modalities for how you notify major incidents / cyber threats to the CSSF |
| CSSF 25/892 | Adoption of the ESA Joint Guidelines (JC GL 2024 34) on estimating aggregated annual costs and losses | Applies when the CSSF requests your Art. 11(10) cost/loss estimate |
| CSSF 25/882 | Requirements on the use of ICT third-party services for financial entities subject to DORA | Local rules on which providers you may use, cloud-officer designation, backup of accounting data / client positions, and the notification timeline for planned ICT arrangements |
| CSSF 25/880 | Relationship management of payment service users and PSP ICT assessment | PSP-specific; the ICT assessment is submitted via the CSSF eDesk portal |
| CSSF 23/834 | Mandatory use of the IMAS portal for certain supervisory processes | Relevant for ECB-supervised significant institutions |
| CSSF 21/769 | Governance and security for telework / ICT outsourcing substance | Central-administration and substance expectations that intersect with ICT risk |

Always open the CSSF "ICT and cyber risk - for DORA entities" page for the
current list, as circulars are added and amended over time.

---

## 3. Incident classification and reporting: the Luxembourg route

Classify against the **Classification RTS (EU) 2024/1772** and report within the
time limits of the **Reporting RTS (EU) 2025/301** using the forms of the
**Reporting ITS (EU) 2025/302**. All three are in the toolkit's
[regulatory-references.md](regulatory-references.md).

In Luxembourg the notification of a major ICT-related incident (and, optionally, a
significant cyber threat) goes **to the CSSF**, following the modalities in
**Circular CSSF 25/893**. Build the CSSF channel and the exact deadline clock into
your incident runbook rather than a generic "notify the regulator" step.

On request, you must also provide an estimate of **aggregated annual costs and
losses** from major incidents (DORA Art. 11(10)); Luxembourg adopts the ESA Joint
Guidelines via **Circular CSSF 25/892**.

---

## 4. ICT third-party arrangements: who to notify, and when

Under DORA Art. 28(3) you must inform your competent authority in good time about
any **planned** contractual arrangement for ICT services supporting a critical or
important function, and when a function *becomes* critical or important. In
Luxembourg the route depends on your supervision:

- **Significant institutions under direct ECB supervision** notify the **ECB**
  directly via the **IMAS portal** (see Circular CSSF 23/834 on mandatory IMAS
  use).
- **All other CSSF-supervised DORA entities** notify the **CSSF** using the
  form *Notification of an ICT third-party arrangement supporting a critical or
  important function*, submitted to the agent in charge of your supervision via
  the agreed channels. Under **Circular CSSF 25/882** this notification is due at
  least **three (3) months** before the arrangement takes effect. Where you use a
  **Luxembourg support PFS governed by Article 29-3 LFS**, the notice period is
  reduced to **one (1) month**.

---

## 5. Register of information: submission to the CSSF

Maintain the register per the **Register ITS (EU) 2024/2956** (toolkit templates
cover the structure). In Luxembourg the register is submitted to the **CSSF via
the eDesk portal**. The CSSF has published guidance tables to help you determine
**whether** you must submit an RoI, at **what level of consolidation**, and to
which National Competent Authority, plus guidance on resolving ESA and CSSF
validation error messages. The EBA reporting framework (data point model,
taxonomy, validation rules) and the ESAs' RoI FAQ are the technical references to
monitor before each submission window.

---

## 6. Resilience testing and TLPT

Basic resilience testing follows DORA Arts. 24-25. For advanced testing, the
**CSSF is the TLPT authority for the financial sector under its supervision**
(DORA Art. 46). Threat-led penetration testing in Luxembourg runs under
**TIBER-LU**, jointly adopted by the **Banque centrale du Luxembourg (BCL)** and
the CSSF and updated after DORA's entry into force, in line with the RTS on TLPT
((EU) 2025/1190) and the TIBER-EU framework. Only entities meeting the RTS
identification criteria are in the mandatory TLPT population.

---

## 7. Information sharing (voluntary)

If you join or leave a cyber-threat information-sharing arrangement under DORA
Chapter VI (Art. 45), notify the **CSSF** upon validation of your membership or,
as applicable, once your departure takes effect. Participation is voluntary.

---

## 8. Quick Luxembourg checklist

- [ ] Confirmed which authority supervises you (CSSF vs CAA; and whether you are an ECB-supervised significant institution).
- [ ] Incident runbook cites the CSSF channel and Circular CSSF 25/893, with the 4h / 24h / 72h / 1-month clock built in.
- [ ] ICT third-party notification route chosen (IMAS vs CSSF form) with the correct lead time (3 months, or 1 month for Art. 29-3 LFS support PFS).
- [ ] Register of information submission tested against the CSSF eDesk portal and the CSSF guidance tables.
- [ ] Checked whether you fall in the mandatory TLPT population and, if so, engaged with TIBER-LU (CSSF/BCL).
- [ ] Information-sharing membership changes notified to the CSSF.

---

## 9. Primary sources

- CSSF "ICT and cyber risk - for DORA entities": https://www.cssf.lu/en/ict-and-cyber-risk-for-dora-entities/
- CSSF DORA contact: ictrisksupervision@cssf.lu
- DORA and all RTS/ITS numbers: see [regulatory-references.md](regulatory-references.md)
- EUR-Lex: https://eur-lex.europa.eu
