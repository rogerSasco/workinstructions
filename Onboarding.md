content by section and task category for clarity:

---

### 🖥️ Section 1 – IT Setup & Machine Preparation

| **Task Category** | **Steps / Notes** |
|------------------|-------------------|
| **IT Setup** | - Obtain email, license, VPN ID from IT/HOD<br>- Update One-Touch directory in photocopier<br>- Ensure ICTRequest SharePoint documentation (unless hardware refresh)<br>- Update asset tracking list<br>- Install CARE software (Nurse/Therapist)<br>- Reuse PC: 100% reset unless vendor-delivered<br>- WiFi:<br> • Staff: `SASCOxx` / `Teamwork#1`<br> • Guest: `SASCOxxG` / `Welcome2Sasco` |
| **Machine Prep** | - Boot up, join staff WiFi<br>- Join domain via Microsoft Entra<br>- Set login PIN: `01012000`<br>- Use ITSupport credentials for domain join<br>- Reboot and set local admin:<br> • Username: Administrator<br> • Password: `BigTicket8888`<br>- Sign in as staff: `Welcome2Sasco#168` |
| **Local Admin Setup** | - Add user via Settings > Accounts<br>- Create without Microsoft account<br>- Change account type to Administrator |
| **System Updates** | - Run Windows Updates<br>- Run `sfc /scannow` until clean<br>- If errors persist, run `DISM /Online /Cleanup-Image /RestoreHealth` |
| **PC Naming** | - Get serial number via `wmic bios get serialnumber` or PowerShell<br>- Rename PC: `[DeviceCode][ShortName][Serial]` (e.g., `LJohn4VLY8H2`) |
| **BitLocker** | - Ensure BitLocker is ON<br>- Backup recovery key to Azure AD |
| **Windows Security** | - Open Windows Security (blue shield icon)<br>- Resolve any warnings |
| **Basic Software Installation** | - Windows OS, Edge, Chrome, Office365, Adobe Suite, Autodesk, 7-Zip, Zoom (HOD only), Action1, Checkpoint, CARE software<br>- Uninstall bloatware (Winzip, McAfee, etc.)<br>- Set Chrome as default browser<br>- Install Adobe Reader and set as default for `.pdf`<br>- Install 7-Zip and set as default for `.zip` |

---

### 🔐 VPN Setup & Endpoint Configuration

| **Task Category** | **Steps / Notes** |
|------------------|-------------------|
| **Install Agents** | - Action1: `https://app.action1.com/login/`<br>- Checkpoint Infinity: `EndpointSetupHome.exe` |
| **VPN Account Creation** | - Username format: `<Name@HSsasc0>`<br>- Save credentials in IT Teams > Support > VPN folder |
| **VPN Client Setup** | - Connect via padlock icon<br>- Site: `203.125.130.202`<br>- Disable "Always-Connect"<br>- Test user login |
| **trac.defaults Edit** | - Modify line: `route_conflict_resolution_method STRING “modify” GLOBAL 1` |
| **trac.config Fix (if WiFi drops)** | - Disable encryption in `trac.defaults`<br>- Restart VPN service<br>- Edit `trac.config`:<br> • Add `<active_probing><enabled>true</enabled></active_probing>` |

---

### 🔧 System Optimization

| **Task Category** | **Steps / Notes** |
|------------------|-------------------|
| **Power Plan** | - Set sleep/display to “Never” (both battery & plugged in) |
| **Network Reset** | - Reset network settings if needed |

---

### 👤 Section 2 – User Onboarding

| **Task Category** | **Steps / Notes** |
|------------------|-------------------|
| **Email & Office Setup** | - Add user to `sascoAll` group<br>- Guide user to change password at `www.office.com`<br>- Install Office apps<br>- Configure Outlook:<br> • Download all emails<br> • Disable Focused Inbox<br> • Set up signature |
| **Calendar Setup** | - Share calendar with supervisor/team<br>- Add meeting room calendars:<br> • `ALBoard@sasco.org.sg`<br> • `ALMtgRoom@sasco.org.sg`<br> • `EPL1MtgRoom@sasco.org.sg` |
| **OneDrive & Teams** | - Sign in to OneDrive<br>- Install and test Microsoft Teams |
| **Taskbar Pinning** | - Pin Word, Excel, PowerPoint, Outlook, Teams |
| **Screensaver & Lock** | - Set to Mystify, 10 mins<br>- Enable “On resume, display logon screen”<br>- Teach `Windows + L` |
| **Startup Apps** | - Disable unnecessary startup apps |
| **Printer Setup** | - Download Canon UFR driver<br>- Rename printer appropriately<br>- Set default printer<br>- Configure secure print with Department ID<br>- Update Excel tracking |
| **Bookmarks Transfer** | - Export from old Chrome<br>- Save to OneDrive<br>- Import on new device |
| **Email Signature Setup** | - Copy template from email<br>- Configure in Outlook<br>- Can be done remotely via Action1 |

---

### ✅ Final Checklist

| **Category** | **Items to Confirm** |
|-------------|----------------------|
| **Laptop/PC Settings** | WiFi, SFC scan, PC name, Power plan, BitLocker, Windows Security |
| **Software** | Chrome, Office365, Adobe Reader, 7-Zip, Action1, Checkpoint VPN, CARE |
| **User Setup** | Email signature, OneDrive, Teams, Outlook, Calendar |
| **Hardware** | Printer setup, Inventory list updated |

---

