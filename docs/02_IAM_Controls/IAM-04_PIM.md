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
