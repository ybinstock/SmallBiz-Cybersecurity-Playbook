Backup & Disaster Recovery Policy
1. Purpose
Ensure critical data and services can be restored to meet Recovery Time Objective (RTO) and Recovery Point Objective (RPO) targets.

2. Scope
Customer‑facing production systems, databases, and critical SaaS.

3. Roles & Responsibilities
Infrastructure Lead – owns backup tooling.

App Owners – define RTO/RPO.

Security – audits DR tests.

4. Policy Statements
Backup Cadence – Databases hourly; files daily; config snapshots pre‑deploy.

Immutable Storage – Off‑site, WORM storage for 30 days.

Encryption – Backups encrypted in transit & at rest (AES‑256).

DR Testing – Quarterly restore drills; log results.

RTO/RPO Targets – Tier 1 apps: RTO 2 h, RPO 15 min.

Retention – 1 year for operational backups; 7 years for compliance archives.

5. Monitoring & Metrics
Backup success rate ≥99 %.

Quarterly restore success 100 %.

Test drill report submitted within 7 days.

6. Exceptions
Temporary pauses require VP‑Engineering approval.

7. Revision History
2025‑06‑04 v1.0.


| Framework     | Relevant controls                                                                            |
| ------------- | -------------------------------------------------------------------------------------------- |
| **NIST CSF**  | PR.IP‑4 (Backup), PR.IP‑9 (Testing), PR.DS‑4 (Encrypt at Rest), RC.CO‑1 & RC.CO‑2 (Recovery) |
| **CIS v8**    | 11.1 – 11.5 (Data Recovery), 12.7 (Encrypted Storage), 12.10 (Immutable Backups)             |
| **ISO 27001** | 8.5 (Backup), 8.14 (Redundancy), 8.26 (BC/DR), 5.30 (ICT Readiness)                          |
