## Privileged Identity Management (PIM)

### Objective
Ensure privileged roles are not permanently assigned but activated on-demand (Just-in-Time access).

### Implementation

- Global Administrator role assigned as **Eligible**
- Access requires manual activation
- Time-bound access enforced (e.g., 4–8 hours)
- Permanent assignments avoided

### Evidence

- PIM role assignment configuration
- Eligible role listing
- Assignment duration enforcement error (policy validation)

### Verification

- Entra ID → Privileged Identity Management → Roles
- Confirm role = Eligible
- Confirm activation required before use

### Risk Addressed

- Standing privilege abuse
- Credential compromise impact
- Insider threat escalation

### Framework Mapping

- ISO 27001 A.9.2.3 – Privileged Access
- NIST AC-2 / AC-6
- CIS Control 6


## Control Validation Test

### Scenario
Attempted to assign Global Administrator role for 1 year.

### Result
Assignment blocked due to maximum duration policy.

### Evidence
Screenshot showing:
"Time duration specified exceeds maximum allowed"

### Conclusion
PIM successfully enforces time-bound privileged access.


## Evidence

### Identity & Access Control
- Security group creation (SG-DEPT-*)
- User-to-group assignment (HR, IT, Finance)

### Privileged Access
- Global Admin role assignment (backup.admin)
- PIM Eligible role configuration
- Assignment duration enforcement

### Authentication & Activity
- Admin sign-in logs (Entra ID)
- Password reset activity

### Policy Enforcement
- Conditional Access (if enabled)
- MFA enforcement (if configured)

## Audit Conclusion

Privileged access is effectively controlled using RBAC and PIM.

Administrative privileges are:
- Restricted to authorized accounts
- Time-bound (Just-in-Time)
- Monitored through Entra ID logs

No excessive or permanent privileged access identified.

Overall Risk Level: LOW

Privileged roles are assigned as eligible and activated only when required, reducing attack surface and enforcing Zero Trust principles.
