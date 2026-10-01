# TryHackMe — Kenobi

**Platform:** TryHackMe  
**Type:** CTF / training lab  
**Status:** Completed lab

## Skills Practiced

- Nmap enumeration
- SMB/NFS-related service enumeration
- FTP/service investigation
- Linux privilege escalation
- Post-exploitation enumeration

## Methodology

```
Recon → Service Enumeration → Attack Surface Analysis → Initial Access → Local Enumeration → Privilege Escalation
```

## Learning Notes

This room helped reinforce the importance of correlating multiple network services instead of investigating each port in isolation.

Particular focus:

- Enumerating network services and versions
- Understanding file-sharing services
- Inspecting exposed data
- Moving from service-level findings to local privilege escalation

## Defensive Perspective

A defender should reduce unnecessary exposed services, restrict anonymous access, apply least privilege, and keep externally reachable software patched.
