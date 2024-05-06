# Overview



# Resources

https://github.com/vanhauser-thc/thc-hydra \
https://github.com/thex150/Seclists \
https://github.com/danielmiessler/SecLists

# Usage

Help
```bash
hydra -h
```

Bruteforce SSH
```bash
hydra -L user.list -P password.list ssh://10.129.42.197
```

Bruteforce RDP
```bash
hydra -L user.list -P password.list rdp://10.129.42.197
```

Bruteforce SMB
```bash
hydra -L user.list -P password.list smb://10.129.42.197
```
