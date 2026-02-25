# 🚨 Incident Response Playbook – IAM Security

## 🎯 Objective
Define response actions for identity-based security incidents.

---

## 🧠 Scenario: Suspicious Login Detected

### Step 1: Detection
- Alert triggered (Wazuh / Entra logs)
- Multiple failed logins detected

---

### Step 2: Analysis
- Check sign-in logs
- Verify:
  - Location
  - Device
  - User behavior

---

### Step 3: Containment
- Block user account
- Revoke sessions
- Force password reset

---

### Step 4: Eradication
- Remove unauthorized access
- Review group memberships

---

### Step 5: Recovery
- Re-enable account
- Enforce MFA

---

### Step 6: Lessons Learned
- Improve Conditional Access
- Update detection rules

---

## ✅ Conclusion
Rapid response minimizes impact of identity-based attacks.
