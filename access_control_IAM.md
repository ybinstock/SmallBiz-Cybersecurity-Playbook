Access Control & Identity Management Policy
1. Purpose
Ensure only authorized individuals gain access to COMPANY systems and data through robust identity lifecycle management and MFA enforcement.

2. Scope
All production systems, SaaS apps, CI/CD pipelines, and physical facilities.

3. Roles & Responsibilities
Security Lead – defines IAM standards.

IT – manages SSO, MFA, off‑boarding.

Engineering Managers – review access lists monthly.

4. Policy Statements
SSO‑first – All apps integrated with Okta (or other IdP).

MFA – Hardware token or push‑based MFA for all privileged roles; SMS allowed only for low‑risk accounts.

Role‑Based Access Control – Access mapped to job role; reviewed quarterly.

Just‑in‑Time Privilege – Admin rights granted for ≤8 hours via approval workflow.

Joiner‑Mover‑Leaver – HR triggers automatic provisioning / de‑provisioning via HRIS webhook.

Service Accounts – No shared passwords; rotate secrets every 90 days through vault.

5. Monitoring & Metrics
0 dormant accounts >30 days.

100 % MFA coverage on privileged accounts.

Quarterly access recertification completion rate ≥98 %.

6. Exceptions
Documented in access‑review tool; Security Lead signs off.

7. Revision History
2025‑06‑04 v1.0 – Initial.


| Framework     | Relevant controls                                                                     |
| ------------- | ------------------------------------------------------------------------------------- |
| **NIST CSF**  | PR.AC‑1 → PR.AC‑6 (Access), PR.AC‑7 (Least Priv), PR.PT‑3 (CUI), DE.CM‑1 (Monitoring) |
| **CIS v8**    | 4.1 – 4.12 (Account Mgmt), 6.3 (MFA), 6.7 (SSO), 6.8 (Just‑in‑Time)                   |
| **ISO 27001** | 5.11 (Access Control), 5.15 (Identity Mgmt), 8.8 (User Endpoints)                     |

