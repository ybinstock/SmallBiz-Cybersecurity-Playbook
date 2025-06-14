Secure Development & Change‑Management Policy
1. Purpose
Embed security controls into the entire SDLC, ensuring changes to code or infrastructure are peer‑reviewed, tested, and auditable.

2. Scope
All source code, IaC, CI/CD pipelines, infrastructure changes.

3. Roles & Responsibilities
Engineering – adhere to SDLC gates.

DevSecOps – maintain scanners and IaC policies.

Product – prioritize security defects.

4. Policy Statements
Code Review – Minimum 1 reviewer; security checklist item for OWASP Top 10.

Static / Dependency Scans – SAST and SCA run on every PR; blocking severity = High+

IaC Policy as Code – Terraform plans evaluated by OPA.

Secrets Management – No plaintext secrets in repo; use vault references.

Change Windows & Rollback – Prod deploys in maintenance windows with automated rollback on failure.

SBOM – Generate SBOM for every release; store 12 mos.

5. Monitoring & Metrics
100 % builds with passing SAST/SCA.

MTTR for High vulns ≤7 days.

Deployment failure rate <5 %.

6. Exceptions
Critical hotfixes may bypass certain gates with post‑mortem in 48 h.

7. Revision History
2025‑06‑04 v1.0.


| Framework     | Relevant controls                                                                           |
| ------------- | ------------------------------------------------------------------------------------------- |
| **NIST CSF**  | PR.IP‑3 (Config Mgmt), PR.IP‑8 (Dev Practices), PR.DS‑7 (Code Integrity), DE.CM‑8 (Logging) |
| **CIS v8**    | 4.4 (Review/Approve Code), 5.3 (Secure Config Baselines), 6.1 (Vuln Mgmt), 16.11 (SBOM)     |
| **ISO 27001** | 5.36 (Secure Coding), 8.9 (Config Mgmt), 8.28 (Change Mgmt), 8.25 (Secure Development)      |
