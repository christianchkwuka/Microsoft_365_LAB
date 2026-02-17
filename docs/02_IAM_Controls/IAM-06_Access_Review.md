# IAM-06 – Access Review (Identity Governance)

## 📌 Control Objective
Ensure that user access to critical resources is **periodically reviewed** and remains appropriate, enforcing the **principle of least privilege** and reducing unauthorized access risks.

---

## 🧩 Scope
- Azure / Microsoft Entra ID
- Security Group: SG-APP-FINANCE
- User Type: Guest Users
- Reviewer: backup.admin

---

## ⚙️ Configuration Details

| Parameter              | Value                          |
|----------------------|--------------------------------|
| Review Name          | FINANCE_Group_Access_Review_Monthly |
| Resource Type        | Teams + Groups                 |
| Group Reviewed       | SG-APP-FINANCE                 |
| Scope                | Guest users                    |
| Reviewer             | backup.admin                   |
| Duration             | 3 days                         |
| Frequency            | Monthly                        |
| Start Date           | 17/02/2026                     |

---

## 🔐 Implementation Steps

1. Navigate to:
   - Microsoft Entra ID → Identity Governance → Access Reviews

2. Click:
   - **New Access Review**

3. Configure Review Type:
   - Select **Teams + Groups**
   - Choose **Specific Group (SG-APP-FINANCE)**

4. Define Scope:
   - Guest users only

5. Assign Reviewer:
   - backup.admin

6. Configure Recurrence:
   - Monthly
   - Duration: 3 days

7. Provide:
   - Review Name
   - Description (compliance-based justification)

8. Review and Create

---

## 🎯 Objective

The access review ensures that:
- Only **authorized users** retain access
- **Inactive or unnecessary accounts** are removed
- Access aligns with **business roles and responsibilities**

---

## 🔍 Verification Steps

- Navigate to:
  - Entra ID → Identity Governance → Access Reviews

- Validate:
  - Review configuration
  - Assigned reviewer
  - Scope and recurrence settings

- Confirm:
  - Group membership aligns with job roles

---

## 📸 Evidence

- Access Review configuration screen
- Reviewer assignment (backup.admin)
- Group selection (SG-APP-FINANCE)
- Review schedule configuration
- Azure subscription limitation message

---

## ⚠️ Limitation

Due to **Azure subscription requirements**, full execution of the access review workflow could not be completed.  
However, the **design, configuration, and governance controls were successfully implemented and validated**.

---

## 🛡️ Risk Addressed

- Unauthorized access to sensitive financial data
- Excessive permissions (privilege creep)
- Insider threats
- Compliance violations

---

## 🔧 Mitigation

- Periodic access validation
- Reviewer accountability
- Removal of unnecessary access rights
- Enforcement of least privilege

---




## 📚 Control Mapping

| Framework              | Control ID                     | Description                              |
|-----------------------|--------------------------------|------------------------------------------|
| ISO 27001:2022        | A.5.18 / A.9.2.5               | Access rights review                     |
| NIST SP 800-53        | AC-2                           | Account Management                      |
| CIS Controls v8       | Control 6                      | Access Control Management               |
| GDPR (DSGVO)          | Art. 32                        | Security of processing                  |
| BSI IT-Grundschutz    | ORP.4.A8 / CON.2.A10           | Benutzer- und Berechtigungsverwaltung   |

---

## 🧠 Auditor Insight

Access reviews are a **critical identity governance mechanism** that ensures continuous validation of access rights.  
Failure to perform regular reviews may result in **privilege accumulation and increased attack surface**.

---

## ✅ Conclusion

The implementation of access reviews demonstrates:
- Strong **identity governance practices**
- Alignment with **security frameworks**
- Proactive **risk management**

This control enhances organizational security by ensuring that access rights remain **appropriate, justified, and auditable**.
