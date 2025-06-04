# SmallBiz-Cybersecurity-Playbook

*A lightweight, framework‑mapped policy pack and IR toolkit for tech startups (<200 staff)*  

**Author:** Yoni Binstock • CISSP (Candidate) • Security+  
**Version:** 1.0 • 2025‑06‑04  

---



## 📄 Policy overview

| # | Policy | Primary CSF Fn | One‑liner |
|---|---|---|---|
| 1 | `acceptable_use_asset_mgmt.md` | Identify / Protect | Defines device & data rules; kills shadow‑IT. |
| 2 | `access_control_IAM.md` | Protect | SSO + MFA + JML lifecycle. |
| 3 | `secure_dev_change_mgmt.md` | Protect / Detect | SDLC gates, SAST/SCA, IaC guardrails. |
| 4 | `incident_response_playbook.md` | Detect / Respond / Recover | 6‑phase IR with SLAs & comms matrix. |
| 5 | `backup_disaster_recovery.md` | Recover | RTO/RPO targets, immutable backups, quarterly restores. |

*Each policy: purpose → scope → roles → statements → **control mapping** (NIST CSF, CIS v8, ISO 27001) → metrics → exceptions → revision log.*

---

## 🚀 Quick‑start (adapt for your org)

1. **Fork** or clone the repo.  
2. Update company‑specific names, roles, and tool references inside `/docs/policies/`.  
3. Replace RTO/RPO values in **Backup & DR** with your tiering.  
4. Export each Markdown file to PDF (e.g., `pandoc acceptable_use_asset_mgmt.md -o AUP.pdf`) if you need a board‑ready bundle.  
5. Publish on your internal wiki or attach to onboarding packets.  

---

## 🔗 Framework coverage snapshot

| Framework | Controls touched by this pack |
|---|---|
| **NIST CSF 1.1** | **ID.AM, PR.AC/DS/IP, DE.CM, RS.RP/CO/MI, RC.IM** |
| **CIS Controls v8** | **1–6, 11–12, 16–18** (core sub‑controls) |
| **ISO/IEC 27001 (2022)** | **5.9 – 5.15, 5.24 – 5.30, 8.5, 8.9, 8.26** |

*(See individual policies for line‑item mappings.)*

---

## 📈 Metrics you can track from day 1
* 100 % asset inventory in CMDB  
* ≥95 % endpoints on latest security patch  
* 0 dormant accounts >30 days  
* Mean Time to Detect (MTTD) <1 h | Mean Time to Recover (MTTR) <2 h  
* Quarterly restore success = 100 %  

---

## 🙋 FAQ  

**Q : Can I add more policies (e.g., Vendor Risk, DLP)?**  
A : Yes—duplicate any file in `/docs/policies/`, keep the template header, and add new control mappings.

**Q : We use Azure AD, not Okta—what should I tweak?**  
A : Search for “Okta” inside `access_control_IAM.md`; swap with your IdP and update MFA wording.

**Q : May I commercialize a fork?**  
A : The MIT license permits it—just retain attribution.

---

> **Enjoy!** If this playbook saves your team time or helps you pass an audit, drop a ⭐ on the repo or tag me on LinkedIn.
