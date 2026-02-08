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
