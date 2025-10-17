# Ticket #003 – Account Locked Out

**Date:** 2025-10-06  
**Requester:** ccorea  
**Priority:** Medium  
**Category:** Account Management  
**Status:** Resolved  

---

## Description
User was unable to log in due to multiple failed password attempts. Account was locked.

---

## Actions Taken
1. Located `ccorea` in Active Directory Users and Computers.  
2. Right-clicked → **Reset Password** and **Unlock Account**.  
3. Enabled **"User must change password at next logon"**.  
4. Informed user of the reset and confirmed login success.

---

## Resolution
Account unlocked and user able to log in successfully.

---

## Screenshots
<p align="center">
  <img src="../screenshots/ticket_003_locked_account.png" alt="ADUC User Properties Unlock Account" width="700"/><br/>
  <em>ADUC User Properties window showing “Unlock Account” and “User must change password at next logon” selected.</em>
</p>

<p align="center">
  <img src="../screenshots/ticket_003_locked_account2.png" alt="ADUC Reset Password Dialog" width="700"/><br/>
  <em>Password reset dialog confirming temporary password entry.</em>
</p>

<p align="center">
  <img src="../screenshots/ticket_003_locked_account3.png" alt="User changing password at next logon" width="700"/><br/>
  <em>User prompted to change password after signing in with temporary password.</em>
</p>

<p align="center">
  <img src="../screenshots/ticket_003_locked_account_sw.png" alt="Spiceworks message confirming account unlock" width="700"/><br/>
  <em>Spiceworks message confirming account unlock and providing temporary password to user.</em>
</p>

---

## Notes
Practiced **account lockout policy management** and **user communication** through ticket system.
