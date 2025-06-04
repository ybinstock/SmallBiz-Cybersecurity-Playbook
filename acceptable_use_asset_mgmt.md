Acceptable Use & Asset Management Policy
1. Purpose
Define acceptable use of company‑owned (and BYOD) assets and establish baseline controls for hardware, software, cloud services, and data.

2. Scope
All employees, contractors, interns, vendors, and any device—company‑owned or personal—that processes or stores COMPANY data.

3. Roles & Responsibilities
CISO / Security Lead – owns this policy, reviews annually.

IT / DevOps – enforces endpoint management, MDM, patching.

People Ops – includes policy in onboarding / off‑boarding.

All Users – acknowledge and comply; report violations within 24 h.

4. Policy Statements
Authorized Assets Only – Devices must be inventoried in the CMDB and enrolled in MDM before accessing Prod or sensitive data.

Least‑Privilege SaaS Access – SaaS tools approved by IT; shadow SaaS is prohibited.

Software Installation – End‑users may install software only via approved app catalog; Devs may request exceptions via Change‑Management ticket.

Data Handling – No PII or customer data on local drives; use encrypted cloud storage.

Prohibited Activities – Personal crypto‑mining, torrenting, offensive content, or unlicensed media on company networks.

Remote Work Security – VPN or ZTNA required off‑prem; no public Wi‑Fi without VPN tunnel.

Device Hardening – OS auto‑patching within 72 h of critical CVE release; full‑disk encryption mandatory.

5. Monitoring & Metrics
100 % asset inventory in CMDB (weekly audit).

≥95 % endpoints on latest security patch (monthly).

Quarterly shadow‑IT scan → 0 critical findings.

6. Exceptions
Submit Jira ticket with business justification; CISO approves ≤30 days, renewable.

7. Revision History
Date	Version	Author	Notes
2025‑06‑04	1.0	Y. Binstock	Initial draft

| Framework              | Relevant controls                                                                                                                      |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **NIST CSF 1.1**       | ID.AM‑1, ID.AM‑2, PR.AC‑1, PR.AC‑3, PR.DS‑1                                                                                            |
| **CIS Controls v8**    | 1.1 – 1.4 (Asset Inventory), 2.1 – 2.3 (Software Inventory), 4.2 (Restrict Admin Priv), 5.1 (Secure Config), 8.2 (Data Classification) |
| **ISO/IEC 27001:2022** | 5.9 (Acceptable Use), 5.10 (Return of Assets), 5.11 (Access Control), 8.9 (Configuration Mgmt), 8.12 (Data Leakage Prevention)         |
