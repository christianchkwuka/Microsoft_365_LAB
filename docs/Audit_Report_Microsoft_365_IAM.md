# Audit Report  
## Microsoft 365 / Microsoft Entra ID – Identity & Access Management (IAM)

---

## 1. Executive Summary

An internal **Identity & Access Management (IAM) audit** was conducted on the Microsoft 365 / Microsoft Entra ID tenant to evaluate the effectiveness of identity security controls, administrative access, and authentication mechanisms.

The audit focused on:
- Multi-Factor Authentication (MFA)
- Least Privilege & administrative role management
- Logging, monitoring, and auditability of sign-in events

Overall, the IAM environment demonstrates a **strong security posture** aligned with industry best practices. Core IAM controls are implemented, enforced, and supported by audit evidence.

**Overall Assessment:**  
🟢 **Effective with minor improvement opportunities**

---

## 2. Audit Scope

### In Scope
- Microsoft Entra ID (Azure AD)
- Microsoft 365 authentication
- User and admin identity lifecycle
- Security groups and role assignments
- Sign-in and authentication logs

### Out of Scope
- Endpoint security
- Network security
- Third-party SaaS integrations

---

## 3. Audit Methodology

The audit was conducted using the following approach:

1. Review of Entra ID configuration
2. Validation of IAM controls against:
   - ISO/IEC 27001
   - NIST SP 800-53
   - BSI IT-Grundschutz
3. Inspection of:
   - Authentication method policies
   - Security group structures
   - Admin role assignments
4. Verification using:
   - Live sign-in logs
   - MFA authentication events
   - Administrative actions

Evidence was collected via screenshots and system logs.

---

## 4. Audit Findings Summary

| Control ID | Control Name | Result |
|----------|-------------|--------|
| IAM-01 | Multi-Factor Authentication | ✅ Effective |
| IAM-02 | Least Privilege & Admin Roles | ✅ Effective |
| IAM-03 | Logging & Monitoring | ✅ Effective |

---

## 5. Detailed Findings

---

### 5.1 IAM-01 — Multi-Factor Authentication (MFA)

**Objective:**  
Ensure users authenticate using more than one factor.

**Observation:**  
- Microsoft Authenticator App enabled
- Software OATH tokens enabled
- Temporary Access Pass configured
- Weak methods (SMS, voice) disabled
- MFA registration enforced during first sign-in

**Evidence Reviewed:**  
- Authentication methods policy
- Authenticator app registration confirmation
- MFA-related sign-in events

**Assessment:**  
MFA is correctly implemented and operational.

**Risk Rating:**  
🟢 Low

**Mapped Controls:**  
- ISO 27001: A.5.17  
- NIST 800-53: IA-2  
- BSI: ORP.4.A8

---

### 5.2 IAM-02 — Least Privilege & Administrative Access

**Objective:**  
Restrict administrative access to only authorized personnel.

**Observation:**  
- Department-based security groups implemented
- Dedicated admin groups defined
- Admin privileges separated from standard users
- Password reset and session revocation available for admins

**Security Groups Observed:**
- SG-DEPT-IT
- SG-DEPT-HR
- SG-DEPT-FIN
- SG-DEPT-SALES
- SG-Global-Admin

**Assessment:**  
Least privilege principle is enforced.

**Risk Rating:**  
🟢 Low

**Mapped Controls:**  
- ISO 27001: A.5.18  
- NIST 800-53: AC-6  
- BSI: ORP.4.A9

---

### 5.3 IAM-03 — Logging & Monitoring

**Objective:**  
Ensure security events are logged and reviewable.

**Observation:**  
- Interactive sign-in logs enabled
- MFA events visible in authentication details
- Admin and user activities traceable
- Location and IP address logging active

**Assessment:**  
Logging provides sufficient audit trail for investigations.

**Risk Rating:**  
🟢 Low

**Mapped Controls:**  
- ISO 27001: A.8.15  
- NIST 800-53: AU-2  
- BSI: OPS.1.1.5

---

## 6. Identified Risks & Impact

| Risk | Impact | Likelihood | Status |
|----|------|-----------|-------|
| Credential theft | High | Low | Mitigated by MFA |
| Privilege misuse | High | Low | Mitigated by role separation |
| Undetected access | Medium | Low | Mitigated by logging |

---

## 7. Recommendations

While the IAM implementation is strong, the following improvements are recommended:

1. Enforce Conditional Access policies for:
   - Location-based access
   - Device compliance
2. Implement Privileged Identity Management (PIM)
3. Define formal IAM policies and procedures
4. Enable alerting on high-risk sign-in events

---

## 8. Conclusion

The Microsoft 365 IAM environment is **well-designed, secure, and audit-ready**.  
Controls are effectively implemented and aligned with international security frameworks.

With minor enhancements, the environment would meet **enterprise and regulatory-grade IAM maturity**.

---

**Auditor:** Christian Chukwuka  
**Date:** February 2026  
**Environment:** Microsoft 365 / Entra ID
