# 16 — Home Lab

My cybersecurity home lab is used to safely develop practical skills without testing third-party systems.

## Current Lab

```
┌─────────────────────┐
│      Kali Linux     │
│ Recon / Security    │
│ Tools / Analysis    │
└──────────┬──────────┘
           │
      Private Lab LAN
           │
┌──────────▼──────────┐
│   Windows 10 Pro    │
│   Target / Server   │
└─────────────────────┘
```

## Current Focus

- Windows administration
- SMB fundamentals
- SMB share configuration
- Enumeration from Kali
- Impacket fundamentals
- PowerShell
- Network traffic analysis
- Windows security hardening

## Lab Principles

1. Keep vulnerable configurations isolated.
2. Use private virtual networking where possible.
3. Never expose intentionally vulnerable services to the public Internet.
4. Record both offensive findings and defensive remediation.
5. Reset/rebuild targets when a lab becomes unstable.
