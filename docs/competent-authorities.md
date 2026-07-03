docs/competent-authorities.md# Who Supervises You: National Competent Authorities and Incident Reporting

**Last reviewed: 3 July 2026.** This appendix helps you answer two practical
questions a first-timer always hits: *which authority supervises us*, and
*where do we actually send a major-incident report*. It is a signpost, not a
substitute for confirming your own supervisor. Confirm your NCA and its live
reporting channel before you need it, not during an incident.

---

## 1. How to find your competent authority

Your supervisor depends on **your entity type** and **the Member State that
authorised you**. In several countries more than one authority is involved (for
example a central bank for prudential matters and a separate markets authority),
so a single country can have different NCAs for different firm types.

Five-step method:

1. **Confirm your entity type** (bank, payment/e-money institution, investment
   firm, crypto-asset service provider (MiCA), insurer/intermediary, fund
   manager, etc.). See docs/proportionality-guide.md.
2. **Confirm your home Member State** (where you are authorised/registered).
3. **Match type + country** to the authority in the table below.
4. **Verify on the ESA registers** (these are the authoritative, always-current
   lists — bookmark them):
   - EBA credit-institutions and payments registers: https://euclid.eba.europa.eu/register/
   - ESMA registers (investment firms, CASPs, trading venues, funds): https://registers.esma.europa.eu/
   - EIOPA insurance register: https://register.eiopa.europa.eu/
5. **Confirm the incident-reporting channel** on your NCA's own DORA page (each
   NCA publishes its own portal, form, or secure email).

---

## 2. National competent authorities (quick directory)

Authority abbreviations and remits change; treat this as a starting map and verify
via the ESA registers above.

| Member State | Typical NCA(s) for DORA-relevant firms | Authority website |
|---|---|---|
| Austria | FMA | https://www.fma.gv.at |
| Belgium | NBB (prudential); FSMA (markets/conduct) | https://www.nbb.be / https://www.fsma.be |
| Bulgaria | BNB (banks); FSC (non-bank) | https://www.bnb.bg / https://www.fsc.bg |
| Croatia | CNB (HNB); HANFA | https://www.hnb.hr / https://www.hanfa.hr |
| Cyprus | CBC; CySEC | https://www.centralbank.cy / https://www.cysec.gov.cy |
| Czechia | CNB | https://www.cnb.cz |
| Denmark | DFSA (Finanstilsynet) | https://www.finanstilsynet.dk |
| Estonia | Finantsinspektsioon | https://www.fi.ee |
| Finland | FIN-FSA (Finanssivalvonta) | https://www.finanssivalvonta.fi |
| France | ACPR (banking/insurance); AMF (markets) | https://acpr.banque-france.fr / https://www.amf-france.org |
| Germany | BaFin | https://www.bafin.de |
| Greece | Bank of Greece; HCMC | https://www.bankofgreece.gr / https://www.hcmc.gr |
| Hungary | MNB | https://www.mnb.hu |
| Ireland | Central Bank of Ireland | https://www.centralbank.ie |
| Italy | Banca d'Italia; CONSOB; IVASS | https://www.bancaditalia.it / https://www.consob.it / https://www.ivass.it |
| Latvia | Latvijas Banka | https://www.bank.lv |
| Lithuania | Bank of Lithuania | https://www.lb.lt |
| Luxembourg | CSSF; CAA (insurance) | https://www.cssf.lu / https://www.caa.lu |
| Malta | MFSA | https://www.mfsa.mt |
| Netherlands | DNB (prudential); AFM (conduct) | https://www.dnb.nl / https://www.afm.nl |
| Poland | KNF (UKNF) | https://www.knf.gov.pl |
| Portugal | Banco de Portugal; CMVM; ASF | https://www.bportugal.pt / https://www.cmvm.pt / https://www.asf.com.pt |
| Romania | BNR; ASF | https://www.bnr.ro / https://www.asfromania.ro |
| Slovakia | NBS | https://www.nbs.sk |
| Slovenia | Banka Slovenije; ATVP; AZN | https://www.bsi.si / https://www.a-tvp.si |
| Spain | Banco de España; CNMV; DGSFP | https://www.bde.es / https://www.cnmv.es |
| Sweden | Finansinspektionen | https://www.fi.se |
| EEA — Iceland | FME (Central Bank of Iceland) | https://www.sedlabanki.is |
| EEA — Liechtenstein | FMA Liechtenstein | https://www.fma-li.li |
| EEA — Norway | Finanstilsynet | https://www.finanstilsynet.no |

Significant banks in the euro area are also prudentially supervised by the
**ECB** under the Single Supervisory Mechanism, working with the national
authority. For DORA incident reporting you still use the channel your NCA tells
you to use.

---

## 3. Reporting a major incident: prepare the channel in advance

Do this **now**, not mid-incident:

1. On your NCA's website, find the **DORA incident-reporting page** and record
   the exact submission method (secure portal, structured form, or email).
2. **Register/onboard** to that portal ahead of time if pre-registration is
   required (many are).
3. Note the **format** they expect — most NCAs align to the EU reporting template
   fields set in Reporting RTS (EU) 2025/301 (see docs/regulatory-references.md).
4. Record **who in your firm is authorised** to submit, plus a named backup.
5. Store the portal URL, credentials location, and a filled dry-run in your
   incident reporting runbook (docs/2-implementation/02-incident-management-and-reporting.md).

### The deadlines you are reporting against (from Reporting RTS 2025/301)

- **Initial notification:** within **4 hours** of classifying as major, and no
  later than **24 hours** from awareness.
- **Intermediate report:** within **72 hours** of the initial notification.
- **Final report:** within **1 month** of the intermediate report.

Weekend/bank-holiday relief (submit by noon next working day) applies to some
firms but **not** to credit institutions, CCPs, trading-venue operators, or
NIS2 essential/important entities. See docs/regulatory-references.md, section 3.

---

## 4. Keep this current

Authority names, mergers, and portals change. Re-check your own NCA's DORA page at
least yearly and whenever you are notified of a supervisory change, and update the
"Last reviewed" date above.

> Signpost only, not legal advice. The ESA registers and your NCA's own site are
> the authoritative sources.
