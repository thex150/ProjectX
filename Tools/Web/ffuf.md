# Overview

Web Fuzzer

# Resources

https://github.com/ffuf/ffuf
https://github.com/thex150/Seclists
https://github.com/danielmiessler/SecLists

# Usage

Help
```bash
ffuf -h
```

Directory Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://domain.name/FUZZ
```

Extension Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://domain.name/indexFUZZ
```

Page Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://domain.name/FUZZ.php
```

Sub-domain Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://FUZZ.domain.name/
```

Vhost Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://domain.name/ -H 'Host: FUZZ.domain.name'
```

Recursive Scanning
```bash
ffuf -w wordlist.txt:FUZZ -u https://domain.name/FUZZ -recursion -recursion-depth 1 -e .php -v
```

GET Request Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://sub.domain.name/admin/admin.php?FUZZ=key
```

POST Request Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://sub.domain.name/admin/admin.php -X POST -d 'FUZZ=key' -H 'Content-Type: application/x-www-form-urlencoded'
```

Value Fuzzing
```bash
ffuf -w wordlist.txt:FUZZ -u https://sub.domain.name/admin/admin.php -X POST -d 'id=FUZZ' -H 'Content-Type: application/x-www-form-urlencoded'
```

Change number of threads
```bash
-t 200
```

Filter Size
```bash
-fs 500
```

Specify Extension
```bash
-e .php
```

Output full url
```bash
-v
```
