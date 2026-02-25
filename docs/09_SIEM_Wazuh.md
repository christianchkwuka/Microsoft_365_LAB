# 📡 SIEM Detection – Wazuh Integration

## 🎯 Objective
Detect identity-based attacks using SIEM monitoring.

---

## 🔍 Log Source
- Microsoft Entra ID Sign-in Logs

---

## 🚨 Detection Use Case

### Scenario:
Multiple failed login attempts

---

## 📊 Detection Logic

- Event: Failed authentication
- Threshold: 5 attempts
- Time window: 5 minutes

---

## ⚙️ Wazuh Rule Example

```xml
<rule id="100001" level="10">
  <if_sid>authentication_failed</if_sid>
  <description>Multiple failed login attempts detected</description>
</rule>
