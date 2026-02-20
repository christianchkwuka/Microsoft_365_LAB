
# IAM-10 – Federation (B2B / B2C)

## 🎯 Objective
Enable secure collaboration with external users while maintaining control over access and security policies.

---

## 🔐 Description
Federation allows external identities to access organizational resources using their own authentication systems.

---

## 🟢 B2B (Business-to-Business)

### Scenario
External users (partners, vendors, consultants) access internal resources.

### Implementation
- Guest users invited via Microsoft Entra ID
- Assigned to security groups
- Access controlled via RBAC and Conditional Access

---

## 🔵 B2C (Business-to-Consumer)

### Scenario
Public users access applications (e.g., customer portals)

### Authentication Methods
- Email/password
- Social identity providers (Google, Facebook)

---

## 🔐 Security Controls

- MFA enforcement
- Conditional Access policies
- Access Reviews (periodic validation)
- Least Privilege access

---

## 🛡️ Risk Addressed

- Unauthorized external access
- Privilege escalation
- Third-party compromise

---

## 📚 Control Mapping

| Framework | Control |
|----------|--------|
| ISO 27001 | A.5.17 / A.9 |
| NIST | IA-2 / AC-3 |
| BSI | ORP.4 Identity Management |

---

## ✅ Conclusion

Federation enables secure external collaboration while maintaining centralized identity control and enforcing Zero Trust principles.
