# helpdesk-lab
This project simulates a real-world IT Help Desk environment using Spiceworks Cloud Help Desk integrated with a Windows Server 2019 Active Directory domain.   It demonstrates how tickets are created, categorized, and resolved using industry-standard workflows, with real troubleshooting tasks completed inside a virtual lab.

# 🧰 Help Desk Ticketing System Home Lab

### Created by Emanuel Reyes  
**Certifications:** CompTIA Security+, CySA+, CASP+  
**Goal:** Entry-Level IT Help Desk | Junior System Administrator | SOC Analyst  

---

## 🗒️ Overview
This project simulates a real-world **IT Help Desk environment** using **Spiceworks Cloud Help Desk** integrated with a **Windows Server 2019 Active Directory** domain.  
It demonstrates how support tickets are received, categorized, and resolved following ITIL-style workflows, using real troubleshooting tasks performed in a virtualized lab environment.

---

## 🖥️ Lab Setup

| Component | Description |
|------------|--------------|
| **Domain Controller** | Windows Server 2019 running Active Directory Domain Services |
| **Client Machine** | Windows 10 Pro joined to the domain |
| **Ticketing Platform** | Spiceworks Cloud Help Desk |
| **Tools Used** | PowerShell, Active Directory Users & Computers (ADUC), Group Policy, Windows Event Viewer |

---

## 🎯 Objectives
- Simulate realistic **help desk tickets** covering common IT support issues  
- Practice **Active Directory account management** and **group membership troubleshooting**  
- Demonstrate use of **GUI and PowerShell** for administration tasks  
- Document ticket workflows clearly and professionally  

---

## 🧾 Tickets Completed

| Ticket ID | Category | Description | Tools Used | Status |
|------------|-----------|--------------|-------------|---------|
| #001 | Account | Password reset requested | ADUC GUI | ✅ Resolved |
| #002 | Software | User requested additional software installation *(simulated)* | Documentation only | ✅ Resolved |
| #003 | Account | Account locked; reset password, unlocked, required password change | ADUC GUI | ✅ Resolved |
| #004 | Access | User unable to access shared “Finance” folder; added to group using PowerShell | PowerShell, AD | ✅ Resolved |
| #005 | Performance | User reported slow computer performance *(simulated)* | Documentation only | ✅ Resolved |

Detailed write-ups for each ticket can be found in the [`/tickets`](./tickets) folder.

---

## 🧰 Example Ticket Walkthrough

### Ticket #004 – Finance Shared Folder Access

**Requester:** j.doe@domain.local  
**Category:** File Access  
**Priority:** Medium  

**Problem:**  
User reported being unable to access the shared Finance folder located on the file server.

**Troubleshooting Steps:**
1. Verified permissions in Active Directory using PowerShell:
   ```powershell
   Get-ADUser -Identity "j.doe" -Properties MemberOf
2. Confirmed user was not a member of the Finance_Users group.

3. Added user to the correct group:
   ```powershell
   Add-ADGroupMember -Identity "Finance_Users" -Members "j.doe"
4. Confirmed group update replicated successfully.

Had user log off and back in to reauthenticate group membership.

Resolution:
User regained access to Finance folder. Confirmed with user and documented resolution in Spiceworks.
