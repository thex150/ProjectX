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

Bruteforce Web Login (username:password)
```bash
hydra -C wordlist.txt <ip> -s <port> http-get /
```

Bruteforce Username
```bash
hydra -L user.list -p password -f <ip> -s <port> http-get /
```

Bruteforce Password
```bash
hydra -l username -P password.list -f <ip> -s <port> http-get /
```

Bruteforce SSH
```bash
hydra -L user.list -P password.list ssh://<ip>
```

Bruteforce RDP
```bash
hydra -L user.list -P password.list rdp://<ip>
```

Bruteforce SMB
```bash
hydra -L user.list -P password.list smb://<ip>
```

Stop after successful login
```bash
-f
```

Try all users on each password
```bash
-u
```

Set username
```bash
-l test
```

Set password
```bash
-p test
```
