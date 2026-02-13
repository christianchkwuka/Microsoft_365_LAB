# Conditional Access Configuration Evidence

## 🔹 MFA Registration

![MFA Setup](../../evidence/screenshots/iam/IAM01_Authenticator_App_Added.png)

---

## 🔹 MFA Challenge

![MFA Challenge](../../evidence/screenshots/iam/MFA_Act2.png)

---

## 🔹 Password Reset (Admin Action)

![Password Reset](../../evidence/screenshots/iam/45_Admin_Password_Reset.png)

---

## 🔹 Sign-In Logs Validation

![Logs](../../evidence/screenshots/iam/Sign-in logs_conditional_access.png)

---

## 🔹 Analysis

- backup.admin → Conditional Access: **Success**
- Christian → Conditional Access: **Not Applied**

### Explanation:
The policy targets only privileged accounts, therefore normal users are excluded.

---

## 🔹 Conclusion
Conditional Access policy successfully enforced MFA for administrators and validated via sign-in logs.
