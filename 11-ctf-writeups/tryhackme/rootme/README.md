# TryHackMe — RootMe

**Platform:** TryHackMe  
**Type:** CTF / training lab  
**Status:** Completed lab

## Skills Practiced

- Web enumeration
- Directory/content discovery
- File-upload security concepts
- Linux shell access
- Privilege escalation methodology

## Learning Notes

The lab demonstrates why file-upload functionality needs strong validation and why server-side controls must not rely only on client-side file extensions.

## Defensive Takeaways

- Validate uploaded files server-side
- Restrict executable content in upload directories
- Use allowlists where practical
- Store uploads outside executable web roots when possible
- Apply least privilege to the web-service account
