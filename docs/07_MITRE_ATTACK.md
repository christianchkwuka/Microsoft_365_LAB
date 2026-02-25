# 🔥 MITRE ATT&CK Mapping – IAM Controls

## 🎯 Objective
Map implemented IAM security controls to known attacker techniques.

---

## 🧠 Attack Scenarios

| Technique | ID | Description | Mitigation |
|----------|----|------------|-----------|
| Credential Access | T1078 | Valid account misuse | MFA + Conditional Access |
| Brute Force | T1110 | Password guessing | Account lockout + MFA |
| Privilege Escalation | T1068 | Admin abuse | PIM + Least Privilege |
| Initial Access | T1078 | External login | Conditional Access (Location) |
| Persistence | T1098 | Account misuse | Access Reviews |

---

## 🛡️ Controls Implemented

- MFA enforcement
- Conditional Access
- PIM (Just-In-Time)
- Access Reviews
- Device compliance

---

## ✅ Conclusion

IAM controls effectively mitigate common identity-based attack techniques.
