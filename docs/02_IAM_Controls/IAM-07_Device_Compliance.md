# IAM-07 – Device-Based Conditional Access

## 🎯 Objective
Restrict access to cloud resources based on device compliance status.

---

## 🔐 Description
Conditional Access policy enforcing access only from compliant and managed devices.

---

## ⚙️ Configuration

- Policy Name: CA-02-Require-Compliant-Device
- Users: All users (excluding emergency account)
- Target: All cloud apps
- Condition: Device compliance
- Grant: Require device to be marked as compliant

---

## 📊 Expected Behavior

| Device Type | Access |
|------------|-------|
| Corporate compliant device | ✅ Allowed |
| Personal device | ❌ Blocked |
| Unknown device | ❌ Blocked |

---

## ⚠️ Limitation

Full enforcement requires Microsoft Intune for device compliance evaluation.

---

## 🛡️ Risk Addressed

- Unauthorized device access
- Data leakage
- Malware-infected endpoints

---

## 📚 Control Mapping

| Framework           | Control |
|--------------------|--------|
| ISO 27001          | A.8.1 / A.8.2 |
| NIST               | AC-3 / IA-2 |
| BSI IT-Grundschutz | OPS.1.1.2 Endpoint Security |

---

## ✅ Conclusion

Device-based access control enhances Zero Trust architecture by ensuring only secure endpoints can access corporate resources.
