- You could run a nessus scan.
- nmap
- github search 'SMB Signing Check'

This is the NMAP way

On Kali:

```
nmap --script=smb2-security-mode.nse -p445 <network_address_CIDR>
```

