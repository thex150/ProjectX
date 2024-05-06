# Overview



# Resources

https://github.com/vanhauser-thc/thc-hydra \
https://github.com/thex150/Seclists \
https://github.com/danielmiessler/SecLists

# Usage

Help
```sh
hydra -h
```

Bruteforce HTTP-Get (username:password)
```sh
hydra -C <wordlist> <ip> -s <port> http-get /
```

Bruteforce Username HTTP-Get
```sh
hydra -L <username-list> -p <password> -f <ip> -s <port> http-get /
```

Bruteforce Password HTTP-Get
```sh
hydra -l <username> -P <password-list> -f <ip> -s <port> http-get /
```

Bruteforce POST form
```sh
hydra -l <username -P <password-list> <ip> -s <port> http-post-form "/<page>:<username-post-data>=^USER^&<password-post-data>=^PASS^:F=<string-logged-out>"
```

Bruteforce SSH
```sh
hydra -L <username-list> -P <password-list> ssh://<ip> -t 4
```

Bruteforce FTP
```sh
hydra -l <username> -P <password-list> ftp://<ip>
```

Bruteforce RDP
```sh
hydra -L <username-list> -P <password-list> rdp://<ip>
```

Bruteforce SMB
```sh
hydra -L <username-list> -P <password-list> smb://<ip>
```

Stop after successful login
```sh
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
