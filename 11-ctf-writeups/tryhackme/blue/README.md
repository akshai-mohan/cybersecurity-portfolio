# TryHackMe — Blue

**Platform:** TryHackMe  
**Type:** CTF / training lab  
**Status:** Completed lab

## Skills Practiced

- Windows service enumeration
- SMB-focused reconnaissance
- Vulnerability research
- Controlled exploitation
- Windows post-exploitation concepts

## Learning Notes

This lab reinforced a core assessment workflow:

```
Discover → Identify → Research → Validate → Exploit in Scope → Document → Remediate
```

The important lesson is that an exposed service should be investigated in context: version, configuration, authentication, network exposure, and patch level all matter.

## Defensive Takeaways

- Keep Windows systems patched
- Restrict unnecessary SMB exposure
- Segment sensitive systems
- Monitor unusual SMB activity
- Disable legacy protocols where operationally possible
