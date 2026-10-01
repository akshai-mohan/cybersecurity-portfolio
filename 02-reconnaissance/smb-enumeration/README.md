# SMB Enumeration — Home Lab

## Objective

Learn how Server Message Block (SMB) works and practice identifying exposed SMB services from Kali Linux against a Windows 10 Pro lab machine.

## Lab Context

- **Attacker:** Kali Linux
- **Target:** Windows 10 Pro home-lab VM
- **Network:** Private virtual/home-lab network
- **Authorization:** Personal lab

## What I Practiced

### Service discovery

I used network/service enumeration to identify SMB-related services on the target.

### SMB client enumeration

I used `smbclient` to interact with available SMB shares and inspect directory listings.

### SID enumeration

I also tested:

```bash
impacket-lookupsid <TARGET-IP>
```

The lab returned an RPC named-pipe binding similar to:

```
ncacn_np:<TARGET-IP>
```

This helped me understand that SMB/RPC can expose Windows security identifiers and account/group information when the target configuration permits it.

## What I Learned

- SMB is a network protocol used for file and printer sharing and Windows network services.
- SMB commonly operates through TCP 445.
- Windows RPC services can be exposed through SMB named pipes.
- Enumeration results depend heavily on Windows version, firewall rules, share permissions, and authentication settings.
- A successful enumeration result does not automatically mean a vulnerability exists.

## Next Steps

- Build a controlled Windows SMB server/share
- Compare anonymous vs authenticated access
- Document share permissions
- Capture and analyze SMB traffic in Wireshark
- Add remediation/hardening notes
