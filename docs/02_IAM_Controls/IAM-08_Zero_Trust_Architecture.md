# IAM-08 – Zero Trust Conditional Access

## 🎯 Objective
Implement Zero Trust security by enforcing access controls based on identity, device compliance, and location.

---

## 🔐 Controls Implemented

### 1. Location-Based Access Control
- Block access from unknown locations
- Allow only trusted regions

### 2. Risk-Based Authentication
- Detect risky sign-ins
- Enforce MFA on suspicious activity

### 3. Device Compliance Enforcement
- Allow access only from compliant devices

---

## 📊 Policy Logic

Access is granted only if:

- User identity is verified
- Device is compliant
- Location is trusted

Otherwise, access is denied.

---

## 🛡️ Risk Addressed

- Account takeover attacks
- Unauthorized remote access
- Compromised credentials

---

## 📚 Framework Mapping

| Framework | Control |
|----------|--------|
| ISO 27001 | A.8 / A.9 |
| NIST | AC-3 / IA-2 |
| BSI | OPS.1.1.4 Network Access Control |

---

## ✅ Conclusion

Zero Trust model ensures continuous verification of identity, device, and context before granting access.
