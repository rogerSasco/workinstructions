
---

### 📋 Document Overview

| **Field** | **Details** |
|-----------|-------------|
| **Title** | Resigned Staff Offboarding |
| **Document No.** | WI-IT-08 |
| **Effective Date** | 14 April 2024 |
| **Process Owner** | Alicia Png, IT Executive |
| **Approver** | Maria Leong, Head of IT |
| **Purpose** | Guidelines for removal of access rights when staff resigns or during re-org |
| **Revision No.** | 00 |

---

### 🧾 Definitions

| **Term** | **Definition** |
|----------|----------------|
| **SASCO** | SASCO Senior Citizens’ Home |
| **Information Resources** | All SASCO-generated data (hardcopy, electronic, magnetic) |
| **IT Facilities** | Devices provided for official duties (laptop, desktop, tablet, phone, storage) |
| **User** | IT Department Staff |

---

### 🛠️ Offboarding Procedure

| **Step** | **Action** |
|---------|------------|
| **1. HR Confirmation** | - At 3pm on last day, confirm with HR to proceed |
| **2. O365 Admin Portal** | - Locate user<br>- Reset password<br>- Sign out of all accounts<br>- Block sign-in |
| **3. OneDrive Backup** | - Create OneDrive link<br>- Select all files and download<br>- Rename with “[ResignedStaffName]-” prefix<br> e.g., `FionaDevi-OneDrive_1_7-2-2024` |
| **4. SharePoint Backup (OneDrive)** | - Go to SharePoint > IT Resigned Staff Backup > Documents<br>- Create folder named after staff<br>- Save OneDrive download |
| **5. Mailbox Permissions** | - Under Mail tab, add `SascoO365backup@sasco.org.sg` to “Read and manage permissions” |
| **6. Mailbox Export (Pikachu PC)** | - Use Action1 device `NALITJHHKVP3`<br>- Export mailbox as `.pst`<br>- Verify folders are up to date |
| **7. Export Steps** | - File > Open & Export > Import/Export<br>- Choose: Export to a file → Outlook Data File (.pst)<br>- Select mailbox folder<br>- Save as `[StaffName][DateOfExport]`<br> e.g., `FionaDevi20240701` |
| **8. SharePoint Backup (Email)** | - Go to SharePoint > IT Resigned Staff Backup > Email<br>- Create folder named after staff<br>- Save `.pst` file |
| **9. Profile Review** | - Check for SharePoint sites, shared mailboxes, distribution lists<br>- Remove or reassign access |
| **10. Delete User** | - Remove from “Active users” in O365<br>- Consult supervisor<br>- Convert email to alias for replacement staff |

---

### 🔒 Access Removal Checklist

| **System / Group** | **Action** |
|--------------------|------------|
| **Email Group** | Remove from `sascoAll` |
| **Applications** | Remove from CARES, infoCARE |
| **Security Tools** | Remove from Checkpoint |
| **Endpoint Protection** | - Locate endpoint<br>- Disable Tamper Protection<br>- Delete endpoint |
| **VPN Access** | - Remove from CCK Firewall<br>- Delete VPN folder from IT SharePoint |
| **Action1** | - Locate endpoint<br>- Click 3 dots → Remove endpoint |
| **Barracuda** | Remove from Phishing Campaign Address Book |

---

Let me know if you'd like this turned into a reusable checklist or embedded into a SharePoint workflow. I can also help automate parts of this with Power Automate or Action1 scripting if you're streamlining offboarding.