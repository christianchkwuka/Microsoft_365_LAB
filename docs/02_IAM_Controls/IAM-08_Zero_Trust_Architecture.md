# IAM-08 – Zero Trust Conditional Access

## 🎯 Objective
Implement Zero Trust security by enforcing access controls based on identity, device compliance, and location.

---

## 🔐 Controls Implemented

### 1. Location-Based Access Control
- Block access from unknown locations
- Allow only trusted regions
<img width="1895" height="905" alt="Block-Unknown-Locations" src="https://github.com/user-attachments/assets/25f0d1be-5d5c-4d7a-af75-83e0438fbb9d" />

<img width="1852" height="862" alt="Block-Unknown-Locations_2" src="https://github.com/user-attachments/assets/ec06bfb6-c14b-45b5-bc10-b7f9600d6858" />


- 

### 2. Risk-Based Authentication
- Detect risky sign-ins
- Enforce MFA on suspicious activity

- <img width="1912" height="852" alt="Risky-SignIn-MFA_1" src="https://github.com/user-attachments/assets/cbfe12dd-a6f2-4338-9398-81acbd54adde" />

<img width="1898" height="888" alt="Risky-SignIn-MFA_2" src="https://github.com/user-attachments/assets/3eb28332-2518-4d86-9f8a-d43ff44cbeaa" />



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
