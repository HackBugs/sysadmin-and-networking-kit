Bilkul. Main **Q1 se Q12 tak poori chat ko ek hi “Final Revision Notes”** mein arrange kar raha hoon, taaki interview se pehle aap isi ko revise kar sako. Isme **simple Hinglish explanation + important technical points + interview mein bolne layak English lines** hain.

<hr>

# IT Technical Interview Questions – Gulf Horses

1. Network Connectivity Between Branches
2. Network Troubleshooting
3. Server and Backup
4. Hikvision CCTV System
5. Computer Troubleshooting
6. Microsoft 365 / Email
7. ERP / Odoo
8. Cybersecurity Incident
9. Hikvision Attendance System
10. First 7 Days
11. Real IT Experience
12. IT Infrastructure Assessment

<hr>

IT Technical Interview Questions – Gulf Horses

1. Network Connectivity Between Branches
    We have our Head Office in Al-Murgab, Wafra Hospital, Kabd Hospital, and several pharmacies. We need to connect all locations securely and reliably.
    How would you design the network? What devices and solutions would you use?
2. Network Troubleshooting
    An employee at Kabd Hospital says that the internet works on his mobile phone, but his computer cannot access the system.
    How would you troubleshoot this issue step by step?
3. Server and Backup
    Suppose we have a server containing important company data, and at 10:00 AM the hard disk fails.
    What would you do, and how would you make sure that no important data is lost?
4. Hikvision CCTV System
    We have Hikvision CCTV cameras installed at several locations, and we want to monitor them from the Head Office.
    If the cameras at one branch suddenly stop appearing on the central monitoring system, how would you identify and troubleshoot the problem?
5. Computer Troubleshooting
    A user’s computer has become extremely slow, and the user is unable to open some files and applications.
    How would you diagnose and troubleshoot the problem?
6. Microsoft 365 / Email
    An employee says that his email works correctly on his mobile phone but does not work on his computer.
    How would you troubleshoot this issue?
7. ERP / Odoo
    A user can log in to the ERP system but cannot access a specific function or screen.
    How would you determine whether the problem is technical, related to user permissions, or related to system configuration?
8. Cybersecurity Incident
    An employee receives a suspicious email and clicks on a link. After that, his computer starts behaving abnormally.
    What are the first five actions you would take?
9. Hikvision Attendance System
    We have Hikvision attendance machines at several locations, and we need the attendance data to reach the central administration.
    If one branch’s attendance device suddenly stops sending data, how would you identify and resolve the problem?
10. First 7 Days
    Imagine that you join our company tomorrow and become responsible for all IT systems, including the Head Office, hospitals, pharmacies, computers, printers, CCTV, attendance machines, network, email, ERP, and shared data.
    What would you do during your first seven days? Please give us a practical step-by-step plan.
11. Real IT Experience
    Please describe one real IT problem that you personally solved. What was the problem, how did you identify the cause, what tools did you use, and how did you solve it?
12. IT Infrastructure Assessment
    If you were asked to assess our entire IT infrastructure on your first day, what would you check first, and why?
<hr>


# GULF HORSES – IT TECHNICAL INTERVIEW

## COMPLETE REVISION NOTES — Q1 to Q12

---

# 1. NETWORK CONNECTIVITY BETWEEN BRANCHES

### Question:

Head Office Al-Murgab mein hai aur Wafra Hospital, Kabd Hospital aur pharmacies different locations par hain. In sabko securely aur reliably kaise connect karoge?

### Simple Understanding:

Sab branches ko ek secure network se connect karna hai.

### Recommended Structure:

Internet
↓
Head Office Firewall
↓
Core Switch
↓
Head Office LAN

Har branch:

Branch Internet
↓
Branch Firewall
↓
Switch
↓
PC / CCTV / Attendance / Printers

Head Office aur branches ke beech:

**Site-to-Site IPsec VPN**

### Important Technologies:

* Firewall
* Site-to-Site IPsec VPN
* Managed Switch
* VLAN
* Routing
* Backup Internet
* UPS

### Example VLAN:

* Office PCs
* Servers
* CCTV
* Attendance
* Printers
* Guest Wi-Fi

### Example IP Scheme:

* HQ → 10.10.0.0/24
* Wafra → 10.20.0.0/24
* Kabd → 10.30.0.0/24
* Pharmacy → 10.40.0.0/24

### Interview Answer:

“I would connect the Head Office and branches using site-to-site IPsec VPNs through business-grade firewalls. I would use managed switches and VLANs to separate office users, servers, CCTV, attendance and guest traffic. I would also configure proper firewall rules, routing and backup internet connectivity for critical locations. Finally, I would document the IP addressing, VLANs, VPNs and network topology.”

### Remember:

**Firewall + IPsec VPN + VLAN + Security + Redundancy + Documentation**

---

# 2. NETWORK TROUBLESHOOTING

### Question:

Kabd Hospital mein employee ke mobile par internet chal raha hai, lekin computer company system access nahi kar raha. Kya check karoge?

### Troubleshooting Order:

**Physical → IP → Gateway → Internet → DNS → VPN → Server → Application → Permission**

### Step 1 – Physical:

* LAN cable
* Wi-Fi
* Switch port
* Link light
* Network adapter

### Step 2 – IP:

Run:

`ipconfig /all`

Check:

* IP address
* Subnet mask
* Default gateway
* DNS

### Step 3 – Gateway:

`ping <default-gateway>`

Agar gateway ping nahi ho raha:

* Cable
* PC
* Switch
* VLAN
* Local network

### Step 4 – Internet:

`ping 8.8.8.8`

Agar gateway working hai but internet nahi:

* Firewall
* Router
* ISP
* Routing

### Step 5 – DNS:

`nslookup google.com`

DNS problem ho sakti hai agar IP se internet chale but domain name se nahi.

### Step 6 – Company System:

`ping <server-IP>`

Then:

`tracert <server-IP>`

Check:

* VPN
* Routing
* Firewall
* Server
* Application

### Important:

Ek working computer se compare karna bahut useful hai.

### Interview Answer:

“First, I would check the physical connection and then verify the IP configuration using ipconfig. I would ping the default gateway, then test internet connectivity and DNS. If internet is working but the company system is not accessible, I would check the VPN, routing, firewall rules, server connectivity and application status. I would also compare the affected computer with a working computer to identify whether the issue is local or network-wide.”

### Remember:

**Cable → IP → Gateway → Internet → DNS → VPN → Server → Application**

---

# 3. SERVER FAILURE & BACKUP

### Question:

Important company data wale server ka hard disk 10 AM par fail ho gaya. Kya karoge?

### First:

Panic nahi karna.

Server ko unnecessarily:

* Format
* Reinstall
* Reboot

nahi karna.

### Step 1:

Confirm hardware failure.

Check:

* RAID controller
* Disk status
* SMART
* Server hardware logs
* OS logs

### If RAID:

Agar ek disk fail hui aur RAID healthy hai:

**Failed disk replace → RAID rebuild → Monitor**

### If Server Down:

Latest verified backup identify karo.

Check:

* Backup date/time
* Full/incremental backup
* Database backup
* Offsite/cloud backup
* Backup integrity
* Restore possibility

### RPO:

**Recovery Point Objective**

Kitna maximum data loss acceptable hai.

Example:
RPO = 1 hour
→ Maximum 1 hour ka data loss acceptable.

### RTO:

**Recovery Time Objective**

System ko kitne time mein restore karna hai.

Example:
RTO = 4 hours
→ System 4 hours ke andar restore hona chahiye.

### 3-2-1 Backup:

* 3 copies of data
* 2 different storage/media
* 1 offsite copy

### Important:

**RAID is NOT backup.**

RAID hardware failure se availability improve karta hai, backup data recovery ke liye hota hai.

### Database:

Aapke Oracle/PostgreSQL knowledge ka use ho sakta hai.

PostgreSQL:

* Database backup
* WAL archiving, if configured
* Point-in-time recovery

Oracle:

* Database backup
* Archived redo logs, if configured
* Recovery/PITR

### After Recovery:

Verify:

* OS
* Storage
* Database
* Application
* Network
* User access
* Backup

### Interview Answer:

“First, I would confirm the disk failure through the server or RAID management tools and check whether the server is protected by RAID. If only one disk has failed, I would replace it and monitor the RAID rebuild. If the server is unavailable, I would use the latest verified backup and restore the system to replacement hardware, a VM or a temporary recovery environment. I would also verify the database, application, network connectivity and user access after recovery. I would follow the company’s RPO, RTO and backup policy.”

### Remember:

**Detect → Protect → Backup → Restore → Verify**

---

# 4. HIKVISION CCTV TROUBLESHOOTING

### Question:

Ek branch ke CCTV cameras Head Office monitoring mein show nahi ho rahe. Kya check karoge?

### First Question:

**One camera affected or all cameras?**

### One Camera:

Check:

* Camera power
* PoE port
* Cable
* Camera IP
* IP conflict

### All Cameras:

Likely:

* PoE switch
* Branch network
* Internet
* VPN
* Firewall
* Routing
* NVR/VMS

### Basic Test:

`ping <camera-IP>`

HQ se camera ko ping karo.

### Troubleshooting Chain:

**Power → PoE → Camera → IP → LAN → Internet → VPN → Firewall/Routing → NVR/VMS**

### Check NVR/VMS:

* Camera online/offline
* IP
* Authentication
* Recording
* Storage
* Service status

### Final:

Live view + recording verify karo.

### Interview Answer:

“First, I would determine whether one camera or all cameras are affected. For a single camera, I would check power, PoE, cable and IP connectivity. If all cameras are offline, I would check the branch switch, internet connection, site-to-site VPN, routing and firewall. From the Head Office, I would test connectivity to the camera IP and then check the Hikvision NVR or VMS. Finally, I would verify live view and recording.”

---

# 5. COMPUTER TROUBLESHOOTING

### Question:

Employee ka computer bahut slow hai aur kuch files/applications open nahi ho rahe. Kya karoge?

### First:

User se ask:

* Problem kab start hui?
* Sab applications slow hain ya kuch?
* Specific files open nahi ho rahi?
* Koi error message?
* Recently software install/update hua?
* Problem suddenly hui ya gradually?

### Task Manager:

`Ctrl + Shift + Esc`

Check:

* CPU
* RAM
* Disk
* Network

### Storage:

Check:

* Free space
* HDD/SSD health
* Disk errors

### Startup:

Unnecessary startup applications disable/check karo.

### Security:

* Antivirus
* Malware scan
* Endpoint protection

### Windows:

`eventvwr.msc`

System/Application logs check karo.

Possible commands:

`sfc /scannow`

DISM where appropriate.

`chkdsk` where appropriate.

### Hardware:

* RAM
* SSD/HDD
* Overheating
* Fan
* CPU

### Important:

Immediately Windows format/reinstall mat karo.

Pehle **root cause identify** karo.

### Interview Answer:

“First, I would understand when the issue started and whether it affects all applications or only specific files. I would check Task Manager for CPU, RAM and disk usage, then check storage health and free space. I would also check startup applications, malware protection and Windows event logs. If specific files are affected, I would test them on another computer to determine whether it is a file or application issue. I would check hardware and system integrity before considering a reinstall.”

### Remember:

**User Problem → Task Manager → CPU/RAM/Disk → Storage → Startup → Security → Logs → Hardware**

---

# 6. MICROSOFT 365 / EMAIL TROUBLESHOOTING

### Question:

Employee ka email mobile par chal raha hai but computer par nahi. Kya karoge?

### Step 1:

Check internet.

### Step 2:

Browser mein Microsoft 365 webmail open karo.

Agar webmail works:
→ Problem likely Outlook/application side.

Agar webmail also fails:
→ Network/DNS/account side check karo.

### Outlook:

Check:

* Offline/Disconnected status
* Send/Receive errors
* Outlook profile
* Account
* Password
* MFA
* Sync
* Outbox
* Mailbox quota
* Office activation

### Network/DNS:

`ipconfig /all`

`nslookup outlook.office.com`

### Multiple Users:

Agar multiple users affected hain:
→ Microsoft 365 service status/health check karo.

### Office Repair:

Settings → Apps → Microsoft 365 → Modify

Try:

* Quick Repair
* Online Repair

### Important:

User se password kabhi mat maango.

### Interview Answer:

“First, I would check the internet connection and test the user's Microsoft 365 webmail in a browser. If webmail works, I would focus on Outlook, including its connection status, account configuration, profile, synchronization and Office activation. If webmail also fails, I would check DNS, network, firewall and account-related issues. I would also check MFA and mailbox status without asking the user to share their password. Finally, I would test sending and receiving email.”

### Remember:

**Internet → Webmail → Account/MFA → Outlook → Profile → Sync → DNS/Network → Repair → Test**

---

# 7. ODOO ERP TROUBLESHOOTING

### Question:

User Odoo ERP login kar raha hai but ek specific function/screen access nahi kar pa raha. Kya check karoge?

### First:

Ask:

* Exact screen?
* Exact error?
* Pehle kaam karta tha?
* Same role wale doosre user ke liye working hai?

### Best Test:

Affected user vs working user compare karo.

### If Other User Works:

Likely:
**Permission/Access Issue**

Check:

* User active?
* Groups
* Access rights
* Record rules
* Company assignment
* Role
* Branch/warehouse access

### If Multiple Users Affected:

Likely technical/configuration issue.

Check:

* Odoo service
* Server
* PostgreSQL
* Database
* Network/VPN
* Reverse proxy
* Web server
* Odoo logs
* Browser cache/session
* JavaScript errors using F12

### Configuration:

* Module installed?
* Module updated?
* Company configuration
* Warehouse
* Workflow
* Accounting/Sales configuration

### Important:

Odoo commonly uses **PostgreSQL**.

Aapka PostgreSQL knowledge yahan useful hai.

Production database mein direct SQL changes **without authorization** nahi karne chahiye.

### Interview Answer:

“First, I would reproduce the issue and check the exact error. I would compare the affected user with another user who has the same role. If the other user can access the function, I would check user groups, access rights, record rules and company or branch assignment. If multiple users are affected, I would investigate the Odoo server, PostgreSQL database, network, reverse proxy and application logs. I would avoid making direct database changes in production unless they are properly authorized.”

### Remember:

**Reproduce → Compare User → Permission → Configuration → Server → PostgreSQL → Logs**

---

# 8. CYBERSECURITY INCIDENT / PHISHING

### Question:

Employee ne suspicious email ka link click kar diya aur computer abnormal behave kar raha hai. First 5 steps?

## 1. ISOLATE

Computer ko network se isolate karo.

* LAN disconnect
* Wi-Fi disable
* Endpoint quarantine if available

## 2. PRESERVE

Immediately format/reboot/delete evidence mat karo.

## 3. REPORT

Incident ko proper IT/security procedure ke according report/document karo.

## 4. SECURE ACCOUNT

Agar employee ne credentials enter kiye:

* Password reset
* Active sessions revoke where supported
* MFA verify
* Suspicious sign-ins check

## 5. INVESTIGATE / REMEDIATE

* Antivirus/EDR
* Processes
* Logs
* Suspicious files
* Network connections
* Malware investigation
* Rebuild/restore if required

### Shortcut:

**ISOLATE → PRESERVE → REPORT → SECURE ACCOUNT → INVESTIGATE**

### Interview Answer:

“First, I would isolate the affected computer from the network to prevent possible spread. I would avoid immediately formatting or rebooting it because evidence may be needed. I would report and document the incident according to the security procedure. If credentials were entered, I would secure the account by resetting the password, revoking sessions where possible and verifying MFA. Then I would investigate using endpoint security tools, logs and malware analysis and remediate or rebuild the system if necessary.”

### Golden Rule:

**Do not say: “I will immediately format the computer.”**

---

# 9. HIKVISION ATTENDANCE SYSTEM

### Question:

Branch ka attendance machine local punching kar raha hai but central administration ko data nahi bhej raha. Kya check karoge?

### First:

Determine:
**One device or whole branch?**

### Device:

Check:

* Power
* LAN cable
* Network status
* IP
* Subnet
* Gateway
* Date/time

### Test:

`ping <device-IP>`

### If Device Reachable:

Check:

* Internet
* VPN
* Routing
* Firewall
* Central server

### Central Software:

Check:

* Device online/offline
* Last communication
* IP
* Authentication
* Server/service
* Sync status

### Time:

Check:

* Date/time
* NTP/time synchronization

### Important:

Local attendance data ko preserve karo.

Device ko unnecessarily reset/delete mat karo.

### Final Test:

New attendance punch → central system mein receive hua ya nahi.

### Interview Answer:

“First, I would check whether the attendance device is powered on and whether it is still recording attendance locally. Then I would verify the LAN connection, IP address, gateway and network connectivity using ping. If the device is reachable, I would check the internet, VPN, routing and firewall connectivity to the central server. I would then check the Hikvision attendance management software and synchronization status. I would also verify the device time and make sure existing attendance records are preserved before making any reset.”

### Remember:

**Power → Network → IP → Ping → Internet/VPN → Firewall → Software → Sync → Verify**

---

# 10. FIRST 7 DAYS AS IT ADMINISTRATOR

### Question:

Company join karne ke first 7 days mein kya karoge?

## DAY 1 – IT INVENTORY

Check:

* PCs
* Laptops
* Servers
* Printers
* Network devices
* Wi-Fi
* CCTV
* Attendance
* Microsoft 365
* Email
* Odoo
* Shared data

Document:

* Device
* Location
* IP
* Serial number
* OS
* Purpose
* Status

Also check immediate:

* Backup risks
* Security risks

---

## DAY 2 – NETWORK

Check:

* ISP
* Internet
* Public IP
* Internal IP
* DHCP
* DNS
* VLAN
* Firewall
* VPN
* Switches
* Branch connectivity
* Backup ISP

Create network map.

---

## DAY 3 – SERVER & BACKUP

Check:

* CPU
* RAM
* Disk
* RAID
* Storage
* UPS
* Server logs
* Database
* Backup
* Restore capability

Oracle/PostgreSQL backup and recovery verify karo.

---

## DAY 4 – MICROSOFT 365 & SECURITY

Check:

* User accounts
* Licenses
* Email
* Outlook
* MFA
* Admin accounts
* Former employee accounts
* Endpoint protection
* Updates
* Security risks

---

## DAY 5 – ODOO + CCTV + ATTENDANCE

### Odoo:

* Server
* Database
* Permissions
* Application

### CCTV:

* Cameras
* NVR
* Recording
* Storage
* Remote monitoring

### Attendance:

* Devices
* Connectivity
* Synchronization

---

## DAY 6 – PRIORITY FIXES

### P1 – Critical

* Server down
* ERP unavailable
* Hospital network failure
* Major security issue
* Backup failure

### P2 – Important

* CCTV
* Attendance
* Email
* Major user issue

### P3 – Normal

* PC issue
* Printer
* Minor software issue

Also create:

* Network diagram
* IP list
* Asset list
* Backup schedule
* VPN list
* CCTV list
* Attendance list
* Vendor contacts
* Issue list

---

## DAY 7 – IT HEALTH REPORT

Prepare:

### Current Status

What is working?

### Risks

What can cause major problems?

### Backup

Is data protected?

### Security

Any major security gaps?

### Hardware

What needs replacement?

### Pending Issues

What needs attention?

### 30/60/90-Day Plan

What should be improved next?

### Strong Interview Line:

“Before making major changes, I would first understand and document the existing environment, because in a hospital and multi-branch environment, an unnecessary change can affect critical operations.”

---

# 11. REAL IT PROBLEM YOU PERSONALLY SOLVED

### Question:

“Please describe one real IT problem that you personally solved. What was the problem, how did you identify the cause, what tools did you use, and how did you solve it?”

### Interviewer Wants:

They want a real incident in this format:

**Problem → Investigation → Tools → Root Cause → Solution → Result**

### Example Structure – Database Connectivity

Problem:
Application database server se connect nahi ho raha tha.

Investigation:

* User/application error check
* Network connectivity
* Server reachability
* Database service
* Connection configuration
* Port
* Firewall
* Application logs
* Database logs

Tools:

* Windows/Linux
* ping
* Network configuration
* Database administration tools
* System/application logs

Root Cause:
Actual cause jo aapne real incident mein identify kiya ho.

Solution:
Configuration/service/firewall/network issue ko correct kiya.

Result:
Application successfully database se connect hua aur users ka work resume hua.

### Important:

**Fake experience claim mat karna.**

Agar interviewer detailed follow-up karega:

* Which server?
* Which port?
* Which database?
* What exact error?
* What configuration?
* What did you change?

Isliye sirf wahi details bolo jo aapne actually handle ki hain.

### Interview Formula:

**Problem**
↓
**How I investigated**
↓
**Tools used**
↓
**Root Cause**
↓
**Solution**
↓
**Result**

### Natural Opening:

“One real IT problem I handled was a database connectivity issue where an application was unable to connect to the database server…”

Iske baad apna **actual experience** explain karo.

---

# 12. IT INFRASTRUCTURE ASSESSMENT

### Question:

“If you were asked to assess our entire IT infrastructure on your first day, what would you check first, and why?”

### Most Important Point:

**First critical systems + backup/data protection + security.**

Kyunki infrastructure mein changes karne se pehle pata hona chahiye ki company ka important data aur critical services protected hain ya nahi.

---

## STEP 1 – CRITICAL SYSTEMS

Identify:

* ERP/Odoo
* Servers
* Databases
* Network
* Internet
* Email/Microsoft 365
* Shared data
* Hospital IT systems
* CCTV
* Attendance

---

## STEP 2 – BACKUP

Check:

* Last successful backup
* Backup location
* Cloud/offsite copy
* Database backup
* Backup frequency
* Backup integrity
* Restore test

---

## STEP 3 – NETWORK

Check:

* ISP
* Firewall
* Router
* Switch
* IP addressing
* DHCP
* DNS
* VLAN
* VPN
* Branch connectivity

---

## STEP 4 – SECURITY

Check:

* Firewall
* Antivirus/EDR
* Updates
* Admin accounts
* User permissions
* MFA
* Remote access
* Security policies

---

## STEP 5 – SERVERS & DATABASE

Check:

* CPU
* RAM
* Storage
* RAID
* Disk health
* UPS
* Logs
* Services
* Database health
* Oracle/PostgreSQL

---

## STEP 6 – CCTV & ATTENDANCE

Check:

* Hikvision cameras
* NVR
* Recording
* Storage
* Attendance devices
* Synchronization
* Connectivity

---

## STEP 7 – END USERS

Check:

* PCs
* Laptops
* Printers
* Software
* Windows
* Antivirus
* Hardware problems

---

## STEP 8 – DOCUMENTATION

Create:

* Asset Inventory
* Network Diagram
* IP Address List
* Server List
* Backup Plan
* Software List
* User/Access List
* CCTV List
* Attendance List
* IT Issues
* Security Risks

Then make a prioritized action plan.

### Interview Answer:

“On my first day, I would not start by changing or configuring systems immediately. First, I would understand the existing environment and identify the systems that are critical to business operations.

My first priority would be the critical systems, especially the ERP, servers, databases, network connectivity, email and shared company data. I would then verify the backup situation because protecting existing data is one of the most important responsibilities of an IT administrator. I would check when the last successful backup was taken, where it is stored, whether there is an offsite copy, and whether a restore has been tested.

Next, I would assess the network infrastructure at the Head Office and branches, including internet connections, firewalls, routers, switches, IP addressing, DHCP, DNS, VLANs and site-to-site VPN connectivity.

After that, I would review cybersecurity controls such as endpoint protection, firewall rules, administrator accounts, MFA, software updates and remote access.

I would then check the servers and databases, including storage health, RAID, CPU, memory, disk space, system logs, services and database health. My experience with Oracle and PostgreSQL would also help me assess the database side.

I would also assess the Hikvision CCTV and attendance systems, followed by user computers, printers and other endpoint devices.

Finally, I would document the complete infrastructure, identify critical risks and prepare a prioritized action plan. My approach would be to first understand, protect and document the environment, and then make controlled improvements without unnecessarily disrupting business operations.”

---

# 🔥 ULTRA-FAST REVISION SHEET

Interview se just pehle ye keywords revise karo:

## Q1 – Branch Network

**Firewall + IPsec VPN + VLAN + Routing + Backup ISP**

## Q2 – Network Issue

**Cable → IP → Gateway → Internet → DNS → VPN → Server**

## Q3 – Server Failure

**RAID + Backup + RPO + RTO + 3-2-1 + Restore**

## Q4 – CCTV

**Power → PoE → IP → Network → VPN → Firewall → NVR**

## Q5 – Slow PC

**Task Manager → CPU/RAM/Disk → Storage → Startup → Malware → Logs**

## Q6 – Email

**Internet → Webmail → MFA → Outlook → Profile → Sync → DNS**

## Q7 – Odoo

**Reproduce → Compare User → Permission → Configuration → Server → PostgreSQL**

## Q8 – Cyber Incident

**ISOLATE → PRESERVE → REPORT → SECURE ACCOUNT → INVESTIGATE**

## Q9 – Attendance

**Power → LAN → IP → Ping → VPN → Firewall → Software → Sync**

## Q10 – First 7 Days

**Inventory → Network → Server/Backup → M365/Security → Odoo/CCTV/Attendance → Fix → Report**

## Q11 – Real Experience

**Problem → Investigation → Tools → Root Cause → Solution → Result**

## Q12 – Infrastructure Assessment

**Critical Systems → Backup → Network → Security → Servers/DB → CCTV/Attendance → Endpoints → Documentation**

---

# ⭐ 10 GOLDEN LINES FOR INTERVIEW

1. “First, I would understand the existing environment before making major changes.”

2. “I would identify whether the issue is local to one device or affecting the entire network.”

3. “I would troubleshoot step by step instead of making assumptions.”

4. “I would always verify the backup before performing major recovery or maintenance.”

5. “RAID improves availability, but RAID is not a backup.”

6. “I would compare the affected user or device with a known working one.”

7. “I would avoid unnecessary formatting or resetting because it can cause data loss or destroy useful evidence.”

8. “Security and data protection would be one of my first priorities.”

9. “After fixing an issue, I would verify the service from the user's point of view.”

10. “I would document the infrastructure and the changes I make so that future troubleshooting becomes easier.”

---

# 🧠 MASTER TROUBLESHOOTING FORMULA

Almost kisi bhi IT problem mein:

**1. Understand the problem**
↓
**2. Identify the scope**
↓
**3. Check physical layer**
↓
**4. Check IP/network**
↓
**5. Check service/server**
↓
**6. Check application**
↓
**7. Check permissions/security**
↓
**8. Identify root cause**
↓
**9. Fix**
↓
**10. Test**
↓
**11. Document**

---

# 🎯 YOUR MAIN TECHNICAL AREAS

Interview mein aapko in areas par confident rehna chahiye:

### Networking

* TCP/IP
* IP Address
* Subnet
* Gateway
* DNS
* DHCP
* VLAN
* VPN
* Firewall
* Routing
* Ping
* Tracert
* Nslookup

### System Administration

* Windows
* Linux
* Users/permissions
* Services
* Logs
* Updates
* Hardware
* Storage
* RAID
* UPS

### Database

* Oracle
* PostgreSQL
* Backup
* Restore
* Connectivity
* Database service
* Logs
* Basic troubleshooting

### Applications

* Odoo ERP
* Microsoft 365
* Outlook
* Browser-based applications

### Security

* Firewall
* Antivirus/EDR
* MFA
* Password/account security
* Phishing
* Incident response
* Backup security

### Physical IT

* CCTV
* Hikvision NVR/VMS
* Attendance machines
* Printers
* PCs
* Switches
* Wi-Fi

---

# FINAL INTERVIEW MINDSET

Interviewer ko ye feel hona chahiye ki:

**“This person does not randomly change things. He first understands the problem, checks the scope, protects the data, troubleshoots systematically, fixes the root cause, verifies the result and documents the solution.”**

Ye mindset ek **IT Support + System Administrator + Infrastructure** role ke liye bahut important hai.
