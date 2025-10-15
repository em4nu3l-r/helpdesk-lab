# Ticket #004 – Access Denied to Finance Shared Folder

**Date:** 2025-10-06  
**Requester:** bsuber  
**Priority:** High  
**Category:** Permissions & Access Control  
**Status:** Resolved  

---

## Description
User unable to access shared network folder `\\server\finance`.

---

## Actions Taken
1. Verified user group membership in Active Directory using PowerShell:  
   ```powershell
   Get-ADUser -Identity "bsuber" -Properties memberOf
2. Confirmed user was not part of Finance_Group.
3. Added user to the group:
   ```powershell
   Add-ADGroupMember -Identity "Finance_Group" -Members "bsuber"
