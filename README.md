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
| c4ptur3-th3-fl4g | Encoding/decoding, hashes | CyberChef, Python |
| Skynet | SMB enumeration, web exploitation, privilege escalation | Nmap, SMB client, Burp Suite, Python |
| [Ignite](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/Ignite.md) | Exploitation of Fuel CMS via known CVE, reverse shell acquisition, and privilege escalation using root credentials from database.php | Nmap, Gobuster, PHP Reverse Shell, Netcat, Python |
| ToolsRus | Bruteforcing, web exploitation | Nmap, Hydra, Burp Suite |
| Wgel CTF | Enumeration, SSH persistence, privilege escalation | Nmap, SSH, Netcat, Bash |
| Startup | Steganography (optional), bruteforcing, privilege escalation, log analysis, web exploitation, cron | Nmap, Hydra, Python, Bash, Steghide |
| [Brooklyn Nine-Nine](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/BrooklynNineNine.md) | Anonymous FTP login, SSH brute-force, and privilege escalation via sudo GTFOBins | Nmap, FTP, SSH, Hydra, GTFOBins |
| [Chill Hack](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/ChillHack.md) | SQL injection, filter bypass, reverse shell, lateral movement via MySQL & steganography, Docker exploitation, and privilege escalation | Nmap, Gobuster, FTP clients, Web tools, SQL tools, Steghide, zip2john, John the Ripper, Python3, Docker |
| GamingServer | SSH key cracking, web enumeration, privilege escalation | Nmap, SSH, Netcat, Python |
| [MrRobot](https://github.com/R0drx69/pentesting-portfolio/blob/main/writeups/tryhackme/MrRobot.md) | WordPress enumeration, user discovery via Burp + fsocity.dic, password brute-force, PHP reverse shell via 404.php, shell stabilization with Python PTY, MD5 hash cracking, SUID nmap privilege escalation | Nmap, Gobuster, Burp Suite, Hydra, WPScan, wget, Netcat, PHP, Python, CrackStation/John the Ripper, GTFOBins |

### HackTheBox Labs

| Lab / Machine | Skills Practiced | Tools Used |
|---------------|-----------------|------------|
| Pilgrimage | Web exploitation, SQL, privilege escalation | Nmap, Gobuster, Burp Suite, SQL tools |
| Knife | Web exploitation, privilege escalation | Nmap, Gobuster, Burp Suite, Netcat |
| Blue | Vulnerability analysis, exploitation | Nmap, Metasploit, Netcat |

---
