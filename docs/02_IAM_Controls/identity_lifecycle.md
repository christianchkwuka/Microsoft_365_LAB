# 👤 Identity Lifecycle Management

## 🟢 Joiner Process

### Objective
Ensure new users receive appropriate access.

### Steps
1. Created new user: john.hr
2. Assigned to HR security group
3. Access granted via group-based RBAC

### Result
- User successfully onboarded
- Access limited to HR resources

### Risk Mitigated
- Unauthorized access

<img width="1837" height="873" alt="Joiner_Process" src="https://github.com/user-attachments/assets/d1d619e0-dc22-4be8-95fa-6267112362f2" />



## 🟡 Mover Process

### Scenario
User transferred from HR → IT

### Steps
1. Removed user from HR group
2. Assigned user to IT group

### Result
- Access updated correctly
- No privilege overlap

### Risk Mitigated
- Privilege escalation

### Before Moving process

### After Moving Process
<img width="1533" height="852" alt="After_Move" src="https://github.com/user-attachments/assets/2c68bd16-ca2e-49cb-8e3b-9b7e518f6dc3" />


- ## 🔴 Leaver Process

### Scenario
User leaves organization

### Steps
1. Account disabled
2. Removed from all groups
3. Access revoked

### Result
- No system access
- Identity secured

### Risk Mitigated
- Unauthorized access after exit

- ### Before Account Enabled
- 
- <img width="1582" height="848" alt="Accoubt_Enabled" src="https://github.com/user-attachments/assets/72c660e8-cb8e-44de-bae0-904b54c7a2ac" />

### After Account Disabled
- <img width="1467" height="747" alt="image" src="https://github.com/user-attachments/assets/739e8e0c-8108-4642-9c98-be143f01c17f" />


## 🔐 Lifecycle Control Mapping

| Stage | Control | Framework |
|------|--------|----------|
| Joiner | Access provisioning | ISO 27001 A.9 |
| Mover | Access review | ISO 27001 A.9.2 |
| Leaver | Access revocation | ISO 27001 A.9.2.6 |

