# 📊 Risk Assessment  
## Microsoft 365 / Entra ID – Identity & Access Management (IAM)

---

## 1. Risk Assessment Methodology

This risk assessment follows a **qualitative, risk-based approach**, aligned with:

- ISO/IEC 27001 (Clause 6 – Planning & Risk Management)
- NIST SP 800-30 (Risk Assessment)
- BSI IT-Grundschutz (Risk analysis methodology)

### Risk Rating Criteria

| Factor | Scale |
|------|------|
| Likelihood | Low / Medium / High |
| Impact | Low / Medium / High |
| Risk Level | Likelihood × Impact |

---

## 2. IAM Risk Register

### 🔐 Identity & Authentication Risks

| Risk ID | Risk Description | Threat Scenario | Impact | Likelihood | Inherent Risk | Existing Controls | Residual Risk |
|------|----------------|----------------|--------|------------|--------------|------------------|--------------|
| IAM-R-01 | Compromised user credentials | Phishing or password reuse leads to account takeover | High | Medium | High | MFA enforced via Microsoft Authenticator | Low |
| IAM-R-02 | Weak authentication methods | SMS/voice MFA susceptible to SIM swap attacks | Medium | Medium | Medium | Weak MFA methods disabled | Low |
| IAM-R-03 | MFA bypass attempts | MFA fatigue or replay attacks | High | Low | Medium | Authenticator app + sign-in monitoring | Low |

---

### 🧑‍💼 Privileged Access Risks

| Risk ID | Risk Description | Threat Scenario | Impact | Likelihood | Inherent Risk | Existing Controls | Residual Risk |
|------|----------------|----------------|--------|------------|--------------|------------------|--------------|
| IAM-R-04 | Excessive admin privileges | Users assigned admin roles beyond job needs | High | Medium | High | Role separation & admin security groups | Low |
| IAM-R-05 | Privileged credential misuse | Admin account compromised or abused | High | Low | Medium | MFA + audit logs | Low |
| IAM-R-06 | Lack of privileged session control | Long-lived admin sessions abused | Medium | Medium | Medium | Session revocation & password reset | Medium |

---

### 📜 Logging & Monitoring Risks

| Risk ID | Risk Description | Threat Scenario | Impact | Likelihood | Inherent Risk | Existing Controls | Residual Risk |
|------|----------------|----------------|--------|------------|--------------|------------------|--------------|
| IAM-R-07 | Undetected malicious sign-ins | Attacker signs in without detection | High | Medium | High | Entra ID sign-in logs | Low |
| IAM-R-08 | Insufficient audit trail | Security incidents cannot be reconstructed | High | Low | Medium | Interactive & MFA logs enabled | Low |
| IAM-R-09 | Delayed incident response | Logs exist but alerts are not automated | Medium | Medium | Medium | Manual log review | Medium |

---

## 3. Risk Treatment Decisions

| Risk ID | Treatment | Justification |
|------|----------|--------------|
| IAM-R-01 | Mitigate | MFA significantly reduces credential compromise |
| IAM-R-02 | Mitigate | Weak MFA methods removed |
| IAM-R-04 | Mitigate | Least privilege enforced |
| IAM-R-06 | Improve | Recommend Privileged Identity Management (PIM) |
| IAM-R-09 | Improve | Recommend Conditional Access alerts |

---

## 4. Residual Risk Summary

| Risk Level | Count |
|----------|------|
| Low | 7 |
| Medium | 2 |
| High | 0 |

**Overall Risk Posture:** 🟢 **Low residual risk**

---

## 5. Recommendations (Risk-Based)

1. Implement Conditional Access policies for:
   - High-risk sign-ins
   - Administrative access
2. Enable Privileged Identity Management (PIM)
3. Integrate Entra ID logs with SIEM (e.g., Microsoft Sentinel / Wazuh)
4. Define formal IAM risk acceptance criteria
5. Schedule periodic access and log reviews

---

## 6. Framework Mapping

| Framework | Relevant Controls |
|--------|------------------|
| ISO/IEC 27001 | A.5.15, A.5.17, A.5.18, A.8.15 |
| NIST SP 800-53 | IA-2, AC-6, AU-2, AU-6 |
| BSI IT-Grundschutz | ORP.4, OPS.1.1 |

---

## 7. Conclusion

The Microsoft 365 IAM implementation demonstrates **effective risk mitigation** through:

- Strong MFA enforcement  
- Least privilege role design  
- Comprehensive audit logging  

Residual risks are **acceptable** and manageable with incremental security improvements.

---

**Risk Owner:** IT Security / IAM Team  
**Author:** Christian Chukwuka  
**Date:** February 2026
