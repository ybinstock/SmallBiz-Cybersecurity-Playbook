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

