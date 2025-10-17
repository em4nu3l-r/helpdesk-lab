# Screenshots Documentation

This folder contains supporting descriptions for the **Help Desk Simulation Lab Screenshots folder**, demonstrating ticket handling, user communication, and technical troubleshooting through Active Directory, PowerShell, and Spiceworks.

---

## Screenshot Index

### Ticket 001 – Password Reset Request
| Filename | Description |
|-----------|--------------|
| `ticket_001_password_reset_sw.png` | Spiceworks Help Desk message to user containing temporary password and notice to change it at next logon. |
| `ticket_001_reset_password.png` | Active Directory Users and Computers (ADUC) Reset Password dialog box with “User must change password at next logon” option selected. |

---

### Ticket 003 – Account Locked Out
| Filename | Description |
|-----------|--------------|
| `ticket_003_locked_account.png` | ADUC User Properties dialog showing “Unlock Account” and “User must change password at next logon” selected. |
| `ticket_003_locked_account2.png` | ADUC Reset Password window displaying temporary password entry. |
| `ticket_003_locked_account3.png` | Screenshot of user logging in and being prompted to change password after using the temporary one. |
| `ticket_003_locked_account_sw.png` | Spiceworks message sent to user providing temporary password and confirmation that account was unlocked. |

---

### Ticket 004 – Finance Folder Access Issue
| Filename | Description |
|-----------|--------------|
| `ticket_004_group_update.png` | PowerShell commands showing output of `Get-ADUser -Properties memberOf`, confirming user not part of Finance group, and command `Add-ADGroupMember` executed to add user to the Finance group.|
| `ticket_004_group_update2.png` | ADUC Finance folder “Members” tab showing the user now listed as part of the Finance group. |
| `ticket_004_group_update_sw.png` | Spiceworks message confirming the user was re-added to the Finance group and access restored. |
