**GDPR & DPDP ACT**

**COMPLIANCE AUDIT**

**MEDINEST HEALTH TECHNOLOGIES PVT LTD**

**Data Processing Activities | Lawful Basis | Consent | Rights | Compliance Gaps | Remediation**

**By,**

**Aaruni Pandey**

**SCOPE & LEGAL STATUS NOTE**

This is a fictional compliance audit prepared for learning, portfolio and interview purposes. MediNest is a mock organisation, and the evidence described is simulated. The report is not legal advice. The DPDP Act 2023 and DPDP Rules 2025 have a phased commencement structure. This report distinguishes between requirements already in force and requirements used as a readiness benchmark.

The GDPR assessment treats MediNest's services to users in Germany and the Netherlands as falling within Article 3(2), subject to the facts assumed in this scenario.

Data processing activities, lawful basis, consent, data subject rights, and prioritised gap register

| **Item**          | **Detail**                                                                                                     |
| ----------------- | -------------------------------------------------------------------------------------------------------------- |
| Frameworks        | GDPR, Digital Personal Data Protection Act, 2023 (DPDP Act), DPDP Rules, 2025                                  |
| Prepared for      | Board and executive team, MediNest (fictional)                                                                 |
| Status of sources | DPDP Act: read from the official Gazette text (MeitY PDF), DPDP Rules, GDPR articles cited from the Regulation |
| Note              | This project is completely for training purpose.                                                               |

1. **EXECUTIVE SUMMARY**

MediNest is a telemedicine and health-tracking provider with about 1.8 million users in India and 90,000 in Germany and the Netherlands. The audit found 13 gaps: 3 critical, 5 high, 4 medium and 1 low. The pattern is consistent: consent is treated as a sign-up formality, health data reaches advertising vendors and governance (records, breach response) has not kept pace with the growth.

| **Severity** | **Count** | **Gaps**                                                       |
| ------------ | --------- | -------------------------------------------------------------- |
| Critical     | 3         | Consent and training; breach response, children and tracking   |
| High         | 5         | Records; DPIA; transfers; rights handling; processor contracts |
| Medium       | 4         | Retention; notices; governance rules; security                 |
| Low          | 1         | Training                                                       |

1. **SCOPE, METHOD AND LEGAL TIMELINE**

Method: Review of the simulated record of processing, privacy notice, consent screens, vendor list, incident log and request log. Each activity was tested for lawful basis, notice, consent quality, retention, security, processor control and transfer.

Severity

- Critical is a likely live breach with harm or regulator exposure.
- High is clear non-compliance
- Medium is a weak control
- Low is a good-practice gap

**Legal timeline**

| **Date**           | **Position**                                                                                                                                                                                       |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 25 May 2018 onward | Art 3(2) of GDPR applies to MediNest because it offers services to people in Germany and Netherlands.                                                                                              |
| 13 Nov 2025        | DPDP Rules notified. Rules 1, 2 and 17 to 21 (title, definitions, Board constitution and procedure) took effect on publication.                                                                    |
| 13 Nov 2025        | Rule 4 (Consent Manager registration) commences one year after the notification.                                                                                                                   |
| 13 May 2027        | Rules 3, 5 to 16, 22 and 23 commence; notice, safeguards, breach intimation, retention and erasure, contact information, children, Significant Data Fiduciary (SDF), rights mechanisms, transfers. |

1. **ORGANISATION PROFILE**

MediNest is a Bengaluru-headquartered private limited company with 240 staff and no EU establishment. It provides services such as video consultations, e-prescriptions, lab test booking through a partner lab, an AI symptom checker, paediatric consults, wearable sync and marketing newsletters. It is hosted with a US cloud provider (Mumbai and Frankfurt regions). Around seventeen vendors process personal data.

**Role classification:**

MediNest is a controller under GDPR Art. 4(7) and a Data fiduciary under DPDP Act sec 2(i). It is not yet notified as a Significant Data Fiduciary under sec. 10, but the volume and sensitivity of health data make notification a realistic risk.

1. **DATA PROCESSING ACTIVITIES**

Health data is a special category data under GDPR Art. 9, so each health activity needs both Art. 6 basis and Art. 9 condition. The DPDP Act has no special category tier and no legitimate-interest ground: processing must rest on consent (s.4(1)(a), s.6) or one of the listed certain legitimate uses (s.7).

| **Activity**                    | **Data**                               | **GDPR basis**                                                 | **DPDP basis**                                                                                                     | **Findings**                                                              |
| ------------------------------- | -------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------- |
| Account registration            | Name, phone, email, date of birth      | Art. 6(1)(b) contract                                          | Consent (sec. 6) after notice (Sec 5)                                                                              | Date of birth reused for marketing without separate consent               |
| Video consultations and records | Symptoms, diagnosis, notes, recordings | Art. 6(1)(b) with Art. 9(2)(h) professional secrecy under 9(3) | Consent sec. 7(f) only for medical emergencies                                                                     | Recordings retained with no stated purpose.                               |
| E-prescriptions, lab booking    | Medication, test orders, results       | Art. 6(1)(b) with 9(2)(h)                                      | Consent                                                                                                            | No processor agreement with the partner lab                               |
| AI symptom checker              | Symptoms, age, history, inferred risk  | Art 6(1)(a) with 9(2)(a)                                       | Consent                                                                                                            | No DPIA, no clinician review route.                                       |
| Paediatric consults             | Child health data, parent details      | Art 6(1)(b) with Art. 9(2)(h); Art 8 is consent based          | Parental consent Sec 9(1) Rule 10; healthcare exemption under Fourth Schedule may apply to the health service only | Self declared age. Ag SDK active in paediatric screens.                   |
| Wearable sync                   | Heart rate, sleep, steps               | Art. 6(1)(a) with Art 9(2)(a)                                  | Consent                                                                                                            | Consent bundled with terms of service.                                    |
| Analytics and ads SDK           | Device ID, usage, health-screen events | Art 6(1)(a)                                                    | Consent                                                                                                            | SDK fires before any choice , sends health screen events.                 |
| Marketing and newsletters       | Emails, interests                      | Art. 6(1)(a)                                                   | Consent                                                                                                            | Pre-ticked box                                                            |
| Security and fraud logs         | IP, device, login events               | Art. 6(1)(f) legitimate interests                              | No legitimate-interest ground; consent via notice and Rule 6 and 8 log duties.                                     | Logs kept for 6 months; Rule 8 says at least 1 year for specified purpose |
| Employee HR data                | ID, health leave                       | Art. 6(1)(b)(c) and Art. 9(2)(b)                               | Sec. 7 (i): processing employee's data without consent for employment purposes                                     | No in-depth audit.                                                        |

1. **CONSENT MECHANISMS**

GDPR requires consent that is freely given, specific, informed and unambiguous (Art. 4(11), 7), and explicit for health data relied on under Art. 9(2)(a). DPDP s.6(1) requires consent that is free, specific, informed, unconditional and unambiguous with a clear affirmative action, limited to data necessary for the specified purpose. The Act itself uses a telemedicine app as an example of what is not allowed: bundling consent for the service with access to the phone contact list.

| **Test**                 | **GDPR**                                                        | **DPDP Act and Rules**                                                                                                                             | **MediNest today**                                              |
| ------------------------ | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| Unbundled and specific   | Separate consent per purpose                                    | Sec. 6(1) specified purpose, necessary data only; Sec 6(2)                                                                                         | Fails: one checkbox for care, analytics, research and marketing |
| Explicit for health data | Art. 9(2)                                                       | Clear affirmative action                                                                                                                           | Fails for wearable and AI checker                               |
| Notice                   | Art. 13 content                                                 | Sec 5 and Rule 3: itemised data, specified purpose, specific goods or services, link to withdraw, exercise rights and complain to the Board.       | Partial: generic purposes, no complaint route.                  |
| Language                 | Clear and plain (Art. 12)                                       | Sec. 5(3). Sec 6 (3): English or any Eighth Schedule language                                                                                      | Partial: English only                                           |
| No pre-ticked boxes      | Yes (recital 32)                                                | Clear affirmative action                                                                                                                           | Fails; newsletter box pre-ticked                                |
| Withdrawal               | Art. 7(3): right to withdraw your consent as easy as giving it. | Sec. 6(4): withdraw consent at any time; sec. 6(6): stop processing within a reasonable time                                                       | Partial: one tap to give, email to withdraw                     |
| Proof                    | Art. 7(1) demonstrate consent                                   | Sec. 6(10) fiduciary must prove notice and consent                                                                                                 | Fails: no timestamped, versioned consent log.                   |
| Children                 | Art. 8 (16 in DE and NL for consent-based online services)      | Sec.9(1) verifiable parent consent under 18, Rule 10; sec.9(3) no tracking or targeted ads; Fourth Schedule exemptions for defined health purposes | Fails: self-declared age; tracking active.                      |
| Consent Managers         | Not applicable                                                  | s.6(7) to (9), Rule 4 from 13 Nov 2026                                                                                                             | Not ready to honour third-party consent requests                |

1. **DATA SUBJECT RIGHTS**

MediNest handles requests through a shared support mailbox. The simulated log shows 61 requests in 12 months, 19 answered after the GDPR deadline, and 8 with no identity check. GDPR requires a response within one month, extendable by two further months for complex or numerous requests with notice (Art. 12(3)). DPDP grievance responses must fall within a period the fiduciary publishes, which under Rule 14 cannot exceed 90 days.

| Right                          | GDPR                                                                                 | DPDP                                                                                                 | Status                                                 |
| ------------------------------ | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| Information                    | Art. 13, 14                                                                          | Sec. 5 Rule 3                                                                                        | Partial                                                |
| Access                         | Art. 15                                                                              | Sec.11: summary of data, processing, and identities of fiduciaries and processors it was shared with | Partial: consultation notes often omitted.             |
| Rectification                  | Art. 16                                                                              | Sec.12(2): correction, completion, updating                                                          | Working                                                |
| Erasure                        | Art. 17                                                                              | Sec.12(3), and Sec.8(7) erasure when purpose ends or consent is withdrawn                            | Broken: backups and processors not reached.            |
| Restriction, portability       | Art. 18, 20                                                                          | No equivalent right                                                                                  | Missing: no export tool (GDPR gap only).               |
| Objection, automated decisions | Art. 21, 22 (solely automated decisions with legal or similarly significant effects) | No equivalent right                                                                                  | Missing: no route to contest AI checker output.        |
| Grievance redressal            | Art. 77 complaint to authority                                                       | Sec.8(10), Sec.13: mechanism, response period, exhaust before the Board                              | Missing: no named grievance owner or published period. |
| Nominate a person              | Not provided                                                                         | Sec.14: death or incapacity                                                                          | Missing                                                |
| Withdraw consent               | Art. 7(3)                                                                            | Sec.6(4)                                                                                             | Partial                                                |
| Publish request channels       | Art. 12(1) transparent                                                               | Rule 14: publish means and particulars for requests; Rule 9: contact information                     | Missing                                                |

1. **COMPLIANCE GAP REGISTER  
   **

| **ID** | **Severity** | **Gap**                                                    | **GDPR**                       | **DPDP (Act and Rules)**              |
| ------ | ------------ | ---------------------------------------------------------- | ------------------------------ | ------------------------------------- |
| G1     | Critical     | Bundled consent and pre-consent tracking of health data    | Art. 5, 6, 7, 9; ePrivacy 5(3) | Sec. v4, 5, 6; Rule 3                 |
| G2     | Critical     | No tested breach response; past exposure not reported      | Art. 33, 34                    | Sec.8(6); Rule 7                      |
| G3     | Critical     | Children: no age assurance; tracking on paediatric screens | Art. 5, 8, 9                   | Sec.9(1), 9(3); Rule 10, 12           |
| G4     | High         | No complete record of processing                           | Art. 30                        | Sec 8(4)                              |
| G5     | High         | No DPIA for AI checker and large-scale health data         | Art. 35, 22                    | Sec.10 and Rule 13 if notified SDF    |
| G6     | High         | Onward transfers without a mechanism                       | Art. 44 to 46                  | Sec.16; Rule 15                       |
| G7     | High         | Rights handling slow, unverified, incomplete               | Art. 12 to 22                  | Sec.11 to 14; Rule 14                 |
| G8     | High         | Processors without contracts                               | Art. 28                        | Sec.8(1), 8(2); Rule 6                |
| G9     | Medium       | No retention schedule                                      | Art. 5(1)(e)                   | Sec. 8(7), 8(8); Rule 8               |
| G10    | Medium       | Generic, English-only notice                               | Art. 12 to 14                  | Sec.5; Rule 3                         |
| G11    | Medium       | No DPO, EU representative or grievance owner               | Art. 27, 37                    | Sec. 8(9), 8(10); Rule 9; s.10 if SDF |
| G12    | Medium       | Security governance evidence is thin                       | Art. 32                        | Sec. 8(5); Rule 6, 8                  |
| G13    | Low          | Training and awareness                                     | Art. 39, 32(4)                 | Sec. 8(4)                             |

1. **PRIORITISED REMEDIATION ROADMAP  
   **

| **Window**      | **Actions**                                                                                                                                                                                          |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Days 0 to 30    | Stop SDKs on health screens (G1). Review the past bucket incident with counsel (G2). Turn off tracking for minors (G3). Name an interim privacy lead and incident lead.                              |
| Days 31 to 90   | Rebuild consent flows and consent log (G1). Breach playbook and tabletop (G2). Age assurance and Fourth Schedule analysis (G3). Vendor agreements (G8). Full processing register (G4).               |
| Days 91 to 180  | DPIA and AI review path (G5). Transfer mapping, clauses and assessments (G6). Request portal and export tool (G7). Retention schedule and deletion (G9). Rewrite notices ahead of 13 May 2027 (G10). |
| Days 181 to 365 | DPO and EU representative (G11). Security controls (G12). Training programme (G13). Internal re-audit against GDPR and DPDP Rules 3 to 16.                                                           |

1. **PENALTY EXPOSURE  
   **

| **Regime**                                                                            | **Maximum**                                                            |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| GDPR Art. 83(5): principles, consent, rights, transfers                               | EUR 20 million or 4% of worldwide annual turnover, whichever is higher |
| GDPR Art. 83(4): controller duties such as Art. 25 to 39 (records, DPIA, breach, DPO) | EUR 10 million or 2% of worldwide annual turnover, whichever is higher |
| DPDP Schedule: reasonable security safeguards (s.8(5))                                | Up to INR 250 crore                                                    |
| DPDP Schedule: breach notice to Board or Data Principals (s.8(6))                     | Up to INR 200 crore                                                    |
| DPDP Schedule: children (s.9)                                                         | Up to INR 200 crore                                                    |
| DPDP Schedule: Significant Data Fiduciary duties (s.10)                               | Up to INR 150 crore                                                    |
| DPDP Schedule: any other provision of the Act or Rules                                | Up to INR 50 crore                                                     |

1. **SOURCES  
   **

- Digital Personal Data Protection Act, 2023 (official Gazette text): meity.gov.in/static/uploads/2024/02/Digital-Personal-Data-Protection-Act-2023.pdf
- Digital Personal Data Protection Rules, 2025, G.S.R. 846(E): official PDF via meity.gov.in (link listed in PrivacyTru Institute guide reviewed 5 September 2026)
- DPDP Act commencement notification, G.S.R. 843(E): meity.gov.in
- Summaries of the Rules reviewed: PrivacyTru Institute DPDP Rules guide; dpdpactindia.in; tsaaro.com; RuleExpert guide (Fourth Schedule healthcare exemption)
- Regulation (EU) 2016/679 (GDPR), Official Journal L 119, 4.5.2016
- EU-US Data Privacy Framework: Commission Implementing Decision (EU) 2023/1795; Latombe v Commission, T-553/23 (3 September 2025); appeal C-703/25 P pending