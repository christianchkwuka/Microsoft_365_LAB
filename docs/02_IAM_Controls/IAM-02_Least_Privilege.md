# IAM-02 — Least Privilege & Administrative Access Control

## Control Objective
Ensure administrative permissions follow the **principle of least privilege** and are clearly separated from standard user accounts.

---

## Scope
- Global Administrators
- Department administrators
- Standard users

---

## Implementation Summary

### Security Groups Created
- SG-DEPT-IT
- SG-DEPT-HR
- SG-DEPT-FIN
- SG-DEPT-SALES
- SG-DEPT-MGMT
- SG-Global-Admin

---

## Privilege Model
- Admin privileges assigned only to dedicated admin accounts
- Standard users have no administrative permissions
- Group-based access control is enforced

---

## Evidence
- Security group creation screenshots
- Group membership assignments
- Admin password reset activity
- Admin sign-in logs

---

## Verification
- Entra ID → Groups → Security Groups
- Entra ID → Roles & Administrators
- Sign-in logs filtered by admin accounts

---

## Risk Addressed
- Privilege escalation
- Insider threats
- Unauthorized configuration changes

---

## Compliance Mapping
- ISO/IEC 27001: A.5.18
- NIST SP 800-53: AC-6
- BSI IT-Grundschutz: ORP.4.A9

---

## Control Status
✅ Implemented  
✅ Auditable



Step:
Assigned Global Administrator role via Microsoft Entra PIM

Control:
Role-based access control (RBAC)

Finding:
Privileged access restricted to authorized account (backup.admin)

Risk:
Excessive privilege assignment could lead to full tenant compromise

Mitigation:
Least privilege enforced and monitored



<img width="1567" height="837" alt="Privileged_Identity_Magt_1" src="https://github.com/user-attachments/assets/588d01a2-f002-4c73-94e2-17736a9cb27d" />



<img width="1908" height="862" alt="Privileged_Identity_Magt_2" src="https://github.com/user-attachments/assets/62af5c7a-b6da-4650-8b23-f3601cd6a23d" />


<img width="1892" height="883" alt="Privileged_Identity_Magt_3" src="https://github.com/user-attachments/assets/554e1377-56d0-4050-a52b-344e9cfc355a" />


