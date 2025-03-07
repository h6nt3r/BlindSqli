## Installation
```
cd /opt/ && sudo git clone https://github.com/h6nt3r/BlindSqli.git && cd BlindSqli/
sudo chmod +x ./*.py
cd
sudo apt install dos2unix -y
sudo dos2unix /opt/BlindSqli/bsqli.py
sudo ln -sf /opt/BlindSqli/bsqli.py /usr/local/bin/bsqli
bsqli -h
```
### Options
```
usage: bsqli [-h] -u URLS -p PAYLOADS [-c COOKIE] [-t THREADS] [-o SAVE] [-v] [-V]

BSQLI Tool - One Line Command Tool

options:
  -h, --help            show this help message and exit
  -u URLS, --urls URLS  Path to URL list file or a single URL
  -p PAYLOADS, --payloads PAYLOADS
                        Path to the payload file
  -c COOKIE, --cookie COOKIE
                        Cookie to include in GET request
  -t THREADS, --threads THREADS
                        Number of concurrent threads (0-10)
  -o SAVE, --save SAVE  Filename to save vulnerable URLs
  -v, --verbose         Enable verbose mode
  -V, --version         show program's version number and exit
```
### Download sleep payload
```
wget https://raw.githubusercontent.com/h6nt3r/payloads/refs/heads/main/sqli/xor.txt
```
<a href="https://github.com/h6nt3r/payloads/tree/main/sqli">All SQLi payloads</a>

![multi-parameter](multi-parameter.png)
