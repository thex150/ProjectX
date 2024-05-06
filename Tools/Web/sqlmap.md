# Overview

Automatic SQL injection and database takeover tool

# Resources

https://github.com/sqlmapproject/sqlmap \
https://github.com/sqlmapproject/sqlmap/wiki/Usage

# Usage

Help
```sh
sqlmap -h
```

Advanced Help
```sh
sqlmap -hh
```

Basic Run
```sh
sqlmap -u "http://www.example.com/vuln.php?id=1" --batch
```

Skip Required user Input
```sh
--batch
```
