# TryHackMe — Simple CTF

**Platform:** TryHackMe  
**Type:** CTF / training lab  
**Status:** Completed lab

## Learning Objectives

- Practice Nmap-based reconnaissance
- Enumerate exposed services
- Understand web-service attack surface
- Practice Linux privilege-escalation methodology

## Methodology

### 1. Reconnaissance

Start with a full TCP port scan and identify service versions.

```bash
nmap -sC -sV -p- <TARGET-IP>
```

### 2. Enumeration

For each discovered service:

- Identify the software and version
- Enumerate web content where applicable
- Check authentication boundaries
- Correlate versions with known weaknesses in the context of the lab

### 3. Exploitation

Use only the intended CTF attack path and keep evidence of the successful step.

### 4. Privilege Escalation

After obtaining a low-privileged shell, enumerate:

- Current user and groups
- SUID binaries
- Writable files/directories
- Scheduled tasks
- Interesting configuration files

## Key Lessons

- Enumeration quality strongly affects the rest of an assessment.
- Version information is useful for hypothesis generation, not proof of exploitability.
- Privilege escalation should be systematic rather than command guessing.

> Detailed flags/answers can be expanded as I continue improving this write-up.
