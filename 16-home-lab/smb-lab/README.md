# Windows 10 SMB Lab

## Purpose

Build a simple SMB server/share on Windows 10 Pro and understand the protocol before moving into more advanced enumeration.

## SMB in Simple Terms

SMB (Server Message Block) is a Windows-oriented network protocol used for sharing resources such as:

- Files and folders
- Printers
- Named pipes
- Other Windows network services

A Windows computer can act as both an SMB client and an SMB server.

## Typical Flow

```
Kali Linux
   │
   │ TCP 445
   ▼
Windows 10 Pro
   │
   ├── SMB Server
   ├── Shared Folder
   └── Access Control
```

## Lab Exercises

### Exercise 1 — Create a test share

Create a dedicated folder such as `C:\LabShare`, share it through Windows, and use a dedicated lab account.

### Exercise 2 — Discover the share from Kali

Use:

```bash
smbclient -L //<TARGET-IP> -U <LAB-USER>
```

### Exercise 3 — Connect to the share

```bash
smbclient //<TARGET-IP>/<SHARE-NAME> -U <LAB-USER>
```

### Exercise 4 — Compare permissions

Test read-only and read/write permissions with separate lab accounts.

### Exercise 5 — Observe traffic

Capture the authorized lab traffic in Wireshark and identify SMB negotiation, session setup, and tree-connect operations.

## Security Notes

Avoid enabling legacy SMB protocols simply to make a lab easier. Prefer modern SMB configurations and keep this environment isolated.

## Status

**In progress — foundational SMB lab**
