# IAM-01 — Multi-Factor Authentication (MFA)

## Control Objective
Ensure all users authenticate using **multi-factor authentication** to mitigate risks from stolen or compromised credentials.

---

## Scope
- All Microsoft 365 users
- Interactive cloud sign-ins
- Privileged and non-privileged accounts

---

## Implementation Summary
MFA is enforced using **modern authentication methods**:

### Enabled Methods
- Microsoft Authenticator App
- Software OATH Tokens
- Temporary Access Pass (TAP)

### Disabled / Restricted Methods
- SMS authentication
- Voice call MFA
- Legacy authentication protocols

---

## Configuration Location
Microsoft Entra Admin Center  
→ Security  
→ Authentication methods  
→ Policies

---

## Evidence
- Authentication methods policy configuration
- Authenticator app registration confirmation
- MFA-related sign-in events

---

## Verification Steps
1. Navigate to **Sign-in Logs**
2. Select a user sign-in event
3. Confirm MFA challenge was performed
4. Review authentication details

---

## Risk Addressed
- Phishing attacks
- Password reuse
- Credential stuffing
- Unauthorized access

---

## Compliance Mapping
- ISO/IEC 27001: A.5.17
- NIST SP 800-53: IA-2
- BSI IT-Grundschutz: ORP.4.A8

---

## Control Status
✅ Implemented  
✅ Verified via live sign-in logs
