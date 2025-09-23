# 🛡️ eJPTv2 Preparation CTFs

This repository is a curated collection of **CTFs and labs essential for preparing for the eJPTv2 certification**.  
It contains write-ups, notes, and resources to practice key penetration testing skills like enumeration, exploitation, password attacks, and privilege escalation.

> ⚠️ Note: Flags are **not included**. Only methodology, tools, and skills are documented to maintain the learning experience.

---

## 🧠 Featured Labs & Writeups

### TryHackMe Labs

| Lab / Machine | Skills Practiced | Tools Used |
|---------------|-----------------|------------|
| [Basic PenTesting](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/BasicPentesting.md) | Brute-force SSH login, Samba enumeration, web discovery, and privilege escalation via readable SSH key | Nmap, Gobuster, enum4linux, Hydra, John the Ripper, LinPEAS, SSH |
| [Pickle Rick](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/PickleRick.md) | Web Exploitation, Command Execution, File Access, Privilege Escalation (sudo less → reading root files) | Nmap, Gobuster, Nikto, browser, terminal (bash), sudo, less |
| [RootMe](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/RootMe.md) | File upload bypass via PHP reverse shell, limited shell acquisition, and privilege escalation using SUID Python with GTFOBins | Nmap, Gobuster, PHP Reverse Shell, Netcat, Python, GTFOBins |
| [SimpleCTF](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/SimpleCTF.md) | Port scanning, FTP enumeration, web discovery, SQL Injection exploitation, SSH access, privilege escalation via sudo/vim | Nmap, Gobuster, ExploitDB, Python2, SSH, GTFOBins |
| [Bounty Hacker](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/BountyHacker.md) | Initial access via anonymous FTP, SSH brute-force with discovered passwords, and privilege escalation using SUID tar binary via GTFOBins | Nmap, FTP, Hydra, SSH, GTFOBins, Bash |
| [LazyAdmin](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/LazyAdmin.md) | Web enumeration, CMS backup disclosure, credential recovery (MD5 cracking), arbitrary file upload (web shell), shell stabilization, sudo-based script exploitation for privilege escalation | Nmap, Gobuster, wget, Netcat (nc), Python (pty), MD5 cracking (CrackStation), sudo, Perl |
| [c4ptur3-th3-fl4g](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/c4ptur3-th3-fl4g.md) | Cryptography decoding (Leetspeak, Binary, Base32, Base64, Hex, ROT13, ROT47, Morse, Decimal), multi-layered encoding, spectrogram analysis, steganography on images and archives | CyberChef, dcode.fr, Aperi’Solve |
| [Skynet](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/Skynet.md) | Recon; SMB enumeration & anonymous access; credential harvesting; SquirrelMail brute-force; web discovery; RFI → PHP reverse shell; reverse shell hardening; Linux enum; priv-esc via wildcard injection on cron (SUID bash). | Nmap, smbmap, smbclient, whatweb, Gobuster, Hydra, SearchSploit, php-reverse-shell (custom), nano, python3 (http.server, pty), nc (netcat), wget, linpeas.sh, tar, chmod, bash, touch |
| [Ignite](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/Ignite.md) | Exploitation of Fuel CMS via known CVE, reverse shell acquisition, and privilege escalation using root credentials from database.php | Nmap, Gobuster, PHP Reverse Shell, Netcat, Python |
| [ToolsRus](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/ToolsRus.md) | Port/service scanning; directory enumeration; HTTP basic auth brute-force; Tomcat manager discovery; file upload → RCE via Tomcat manager; Metasploit → meterpreter (root). | Nmap, Gobuster, Hydra, Nikto, msfconsole/Metasploit (exploit/multi/http/tomcat_mgr_upload), Apache Tomcat, meterpreter |
| [Wgel CTF](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/WgelCTF.md) | Port scanning; web enumeration (Apache default page); directory brute-forcing; discovery & use of exposed SSH private key → SSH access; user flag capture; sudo enumeration; privilege escalation via wget (GTFObins technique) → root flag. | Nmap, Gobuster, SSH (id_rsa), chmod, nc (netcat), wget, sudo, GTFObins |
| [Startup](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/Startup.md) | Anonymous FTP (upload/download); web directory discovery; upload PHP webshell → RCE (browser); reverse shell stabilization; local file exfiltration (HTTP server + wget); credential capture from pcap → lateral su to user; sudo/cron analysis; privilege escalation via modifying cron-run script → cron-triggered root reverse shell. | Nmap, FTP (anonymous), Gobuster, PentestMonkey PHP reverse shell, nc (netcat), python / python3 (pty, http.server), wget, Wireshark, su, chmod, printf |
| [Brooklyn Nine-Nine](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/BrooklynNineNine.md) | Anonymous FTP login, SSH brute-force, and privilege escalation via sudo GTFOBins | Nmap, FTP, SSH, Hydra, GTFOBins |
| [Chill Hack](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/ChillHack.md) | SQL injection, filter bypass, reverse shell, lateral movement via MySQL & steganography, Docker exploitation, and privilege escalation | Nmap, Gobuster, FTP clients, Web tools, SQL tools, Steghide, zip2john, John the Ripper, Python3, Docker |
| [GamingServer](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/GamingServer.md) | Port scanning, web enumeration, directory enumeration, SSH key bruteforce, downloading files via curl, LXD container deployment, container breakout for root privileges | Nmap, Gobuster, WhatWeb, Curl, SSH, John the Ripper, LXD, Python, Git, Golang, debootstrap, rsync, squashfs-tools |
| [MrRobot](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/MrRobot.md) | WordPress enumeration, user discovery via Burp + fsocity.dic, password brute-force, PHP reverse shell via 404.php, shell stabilization with Python PTY, MD5 hash cracking, SUID nmap privilege escalation | Nmap, Gobuster, Burp Suite, Hydra, WPScan, wget, Netcat, PHP, Python, CrackStation/John the Ripper, GTFOBins |

### HackTheBox Labs

| Lab / Machine | Skills Practiced | Tools Used |
|---------------|-----------------|------------|
| [Pilgrimage](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/hackthebox/Pilgrimage.md) | Port scanning, web enumeration, Git repository discovery, ImageMagick arbitrary file read (CVE-2022-44268), credential discovery, SSH access, post-exploration (pspy), binwalk RCE via malwarescan (CVE-2022-4510), privilege escalation to root | Nmap, Gobuster, Git / git-dumper, ImageMagick, pngcrush, CyberChef, SSH, SCP, pspy64, inotifywait, Binwalk, Python3, Netcat (nc) |
| [Knife](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/hackthebox/Knife.md) | Port scanning, web enumeration, HTTP header analysis, PHP 8.1 RCE (upload backdoor, reverse shell), shell stabilization, privilege escalation via sudo NOPASSWD on knife binary | Nmap, Curl, Python3 (backdoor/revshell scripts), Netcat (nc), SSH, sudo, Knife (binary) |
| [Blue](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/hackthebox/Blue.md) | Vulnerability analysis, exploitation | Nmap, Metasploit, Netcat |

---
