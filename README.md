# 🛡️ eJPT — Consolidated Study Notes

> **eJPT** (eLearnSecurity Junior Penetration Tester) — A practical, entry-level certification covering the full penetration testing lifecycle.

---

## 📌 About This Repository

This repo contains **consolidated notes** for every major module of the eJPT certification. Each section covers the core concepts, tools, and techniques required to pass the exam and apply skills in real-world ethical hacking engagements.

Whether you're just starting out in cybersecurity or preparing for your eJPT exam — these notes have you covered.

---

## 📂 Module Index

| # | Module | Phase |
|---|--------|-------|
| 01 | [Information Gathering](#1-information-gathering) | Reconnaissance |
| 02 | [Footprinting & Scanning](#2-footprinting--scanning) | Reconnaissance |
| 03 | [Enumeration](#3-enumeration) | Reconnaissance |
| 04 | [Vulnerability Assessment](#4-vulnerability-assessment) | Assessment |
| 05 | [Auditing Fundamentals](#5-auditing-fundamentals) | Assessment |
| 06 | [System / Host-Based Attacks](#6-system--host-based-attacks) | Exploitation |
| 07 | [Network-Based Attacks](#7-network-based-attacks) | Exploitation |
| 08 | [The Metasploit Framework](#8-the-metasploit-framework) | Exploitation |
| 09 | [Exploitation](#9-exploitation) | Exploitation |
| 10 | [Post-Exploitation](#10-post-exploitation) | Post-Exploitation |
| 11 | [Social Engineering](#11-social-engineering) | Exploitation |
| 12 | [Web Application Penetration Testing](#12-web-application-penetration-testing) | Web |

---

## 🔍 Phase 1 — Reconnaissance & Assessment

### 1. Information Gathering

The **first step** in any penetration test. Collect maximum intelligence about the target using passive methods — without directly touching or alerting it.

**Key Concepts:** OSINT, DNS Recon, Email Harvesting, Social Media Recon

**Tools:**
- `whois` — Domain registration info
- `nslookup` / `dig` — DNS lookup
- `Maltego` — Visual OSINT mapping
- `Recon-ng` — Modular recon framework
- `Shodan` — Internet-connected device search
- `Google Dorks` — Advanced Google search operators
- `theHarvester` — Email & subdomain harvesting

🎯 **Goal:** Build an intelligence profile of the target before scanning or attacking.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-1-1-information-gathering-0423a9bbc06e)

---

### 2. Footprinting & Scanning

Active probing of the target to identify open ports, running services, and OS details. Creates a clear **attack surface map**.

**Key Concepts:** Port Scanning, OS Fingerprinting, Service Detection, Banner Grabbing

**Tools:**
- `Nmap` — The go-to port scanner
- `Masscan` — Ultra-fast port scanning
- `Netdiscover` — Network host discovery
- `Zenmap` — GUI front-end for Nmap

🎯 **Goal:** Map the target network and identify all potential entry points.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-1-2-footprinting-scanning-f2f49b9564f5)

---

### 3. Enumeration

A **deeper level of interaction** with discovered services. Extract usernames, shares, directories, and configuration details that can lead to exploitation.

**Key Protocols:** SMB, SNMP, DNS, LDAP, FTP, HTTP

**Tools:**
- `enum4linux` — SMB/NetBIOS enumeration
- `SNMPwalk` — SNMP data extraction
- `rpcclient` — RPC-based Windows enumeration
- `Dirbuster` / `Gobuster` — Web directory brute-force
- `NBTscan` — NetBIOS name scanning

🎯 **Goal:** Discover usernames, directories, and misconfigurations valuable for exploitation.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-1-3-enumeration-bf658c341ac1)

---

### 4. Vulnerability Assessment

Systematically identify, classify, and prioritize security weaknesses in systems and networks using automated scanners and manual analysis.

**Key Concepts:** CVE Identification, CVSS Scoring, False Positive Analysis

**Tools:**
- `Nessus` — Enterprise vulnerability scanner
- `OpenVAS` — Open-source vuln scanner
- `Nmap NSE Scripts` — Lightweight vuln checks
- `Nikto` — Web server scanner

**Severity Levels:** 🔴 Critical → 🟠 High → 🟡 Medium → 🟢 Low

🎯 **Goal:** Find and classify vulnerabilities before attempting any exploitation.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-1-4-vulnerability-assessment-85ed97372f20)

---

### 5. Auditing Fundamentals

Analyze the effectiveness of an organization's security controls. Covers log analysis, compliance checks, and policy reviews.

**Key Concepts:** Log Analysis, CIS/NIST Compliance, File Integrity Monitoring, Access Control Review

**Tools:**
- `Lynis` — Linux system auditing
- `Chkrootkit` — Rootkit detection
- `Auditd` — Linux audit daemon

🎯 **Goal:** Verify that systems meet security best practices and organizational policies.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-2-1-auditing-fundamentals-d59d9b6d5bd1)

---

## ⚔️ Phase 2 — Exploitation

### 6. System / Host-Based Attacks

Attacks targeting the OS and application layer. Covers privilege escalation on both **Windows and Linux** systems.

**Key Concepts:** Privilege Escalation, UAC Bypass, Kernel Exploits, Password Cracking

**Tools:**
- `Metasploit` — Exploitation framework
- `PowerShell` — Windows post-exploitation
- `Mimikatz` — Credential dumping on Windows
- `LinPEAS` / `WinPEAS` — Privilege escalation enumeration

🎯 **Goal:** Gain elevated (root/SYSTEM) privileges on a compromised machine.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-1-system-host-based-attacks-956cfbe914bb)

---

### 7. Network-Based Attacks

Exploit weaknesses in network protocols to intercept traffic and harvest credentials.

**Key Concepts:** ARP Poisoning, MITM, DNS Spoofing, LLMNR/NBT-NS Poisoning

**Tools:**
- `Wireshark` — Packet capture & analysis
- `Ettercap` — MITM attack suite
- `Responder` — LLMNR/NetBIOS poisoning
- `Bettercap` — Modern network attack framework

🎯 **Goal:** Intercept, manipulate, or exploit network traffic for credentials or sensitive data.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-2-network-based-attacks-6f0d4d41b455)

---

### 8. The Metasploit Framework

Industry-standard exploitation framework. Automates vulnerability research and exploitation with a massive library of modules.

**Module Types:**
| Type | Purpose |
|------|---------|
| `exploit` | Attack a specific vulnerability |
| `payload` | Code executed after exploitation |
| `auxiliary` | Scanning, fuzzing, enumeration |
| `post` | Post-exploitation actions |

**Tools:**
- `msfconsole` — Main CLI interface
- `msfvenom` — Payload generation
- `meterpreter` — Advanced post-exploitation shell

🎯 **Goal:** Use Metasploit to exploit vulnerabilities and manage post-exploitation sessions.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-3-the-metasploit-framework-24439d1238c5)

---

### 9. Exploitation

Apply manual and automated techniques to gain unauthorized access to vulnerable systems.

**Key Concepts:** Reverse Shells, Bind Shells, Payload Staging, Public Exploit Usage

**Tools:**
- `Metasploit` — Automated exploitation
- `SearchSploit` / `ExploitDB` — Public exploit database
- `msfvenom` — Custom payload generation
- `netcat` — Manual shell handling

🎯 **Goal:** Gain initial foothold and demonstrate real-world impact through controlled exploitation.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-4-exploitation-d68f291951c8)

---

### 10. Post-Exploitation

Activities after gaining access — maintaining persistence, moving laterally, and exfiltrating data.

**Key Concepts:** Persistence, Lateral Movement, Pivoting, Credential Dumping, Covering Tracks

**Tools:**
- `Meterpreter` — Advanced post-exploitation shell
- `BloodHound` — Active Directory attack path mapping
- `Mimikatz` — Windows credential extraction
- `Empire` — PowerShell post-exploitation framework

🎯 **Goal:** Demonstrate how attackers maintain long-term persistence and gather intelligence post-breach.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-5-post-exploitation-0ae5db04ef11)

---

### 11. Social Engineering

Human-based attack vectors that exploit psychological weaknesses rather than technical flaws.

**Attack Types:** Phishing, Spear Phishing, Vishing, Pretexting, Baiting, Impersonation

**Tools:**
- `SET` (Social Engineering Toolkit) — Automated SE attack framework
- `GoPhish` — Phishing campaign management
- `BeEF` — Browser exploitation framework

🎯 **Goal:** Understand, simulate, and build defenses against human manipulation attacks.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-3-6-social-engineering-ebb6e959b04f)

---

## 🌐 Phase 3 — Web Application Testing

### 12. Web Application Penetration Testing

Test web applications against the **OWASP Top 10** and beyond. Covers injection attacks, broken auth, access control flaws, and client-side vulnerabilities.

**Key Vulnerabilities:**
- 💉 SQL Injection (SQLi)
- 🖥️ Cross-Site Scripting (XSS) — Reflected & Stored
- 🔄 Cross-Site Request Forgery (CSRF)
- 📁 File Inclusion (LFI / RFI)
- 🔐 Authentication Bypass
- 🚪 IDOR / Broken Access Control

**Tools:**
- `Burp Suite` — The industry standard web proxy
- `OWASP ZAP` — Open-source web app scanner
- `SQLmap` — Automated SQL injection tool
- `Nikto` — Web server misconfiguration scanner
- `Dirbuster` / `Gobuster` — Directory enumeration

🎯 **Goal:** Identify and safely exploit vulnerabilities in web applications for ethical security assessments.

📖 [Read Full Notes](https://dharmendrastm.medium.com/ejpt-4-1-web-application-penetration-testing-1fc636e6cabe)

---

## 🗺️ The Penetration Testing Lifecycle

```
[Recon] → [Scanning] → [Enumeration] → [Vuln Assessment]
                                                ↓
                                         [Exploitation]
                                                ↓
                                      [Post-Exploitation]
                                                ↓
                                           [Reporting]
```

---

## 💡 Quick Exam Tips

- ✅ eJPT is a **practical, hands-on** exam — not just theory
- ✅ Know your **Nmap flags** inside out (`-sV`, `-sC`, `-A`, `-p-`)
- ✅ Practice **Metasploit** workflows — `search`, `use`, `set`, `run`
- ✅ Understand **SMB enumeration** thoroughly (very common in exam)
- ✅ Learn basic **pivoting** with Metasploit's `route` command
- ✅ Web attacks: focus on **SQLi and basic XSS** for the exam

---

## 📚 Resources

| Resource | Link |
|----------|------|
| eJPT Official Page | [ine.com/learning/certifications/internal/elearnsecurity-junior-penetration-tester-cert](https://ine.com) |
| Full Notes Blog | [dharmendrastm.medium.com](https://dharmendrastm.medium.com) |
| Exploit Database | [exploit-db.com](https://www.exploit-db.com) |
| OWASP Top 10 | [owasp.org/www-project-top-ten](https://owasp.org/www-project-top-ten/) |
| TryHackMe Practice | [tryhackme.com](https://tryhackme.com) |
| HackTheBox Practice | [hackthebox.com](https://www.hackthebox.com) |

---

## 🙌 Credits

Notes compiled and maintained by **Dharmendra** — aspiring cybersecurity professional and eJPT candidate.

> *"The quieter you become, the more you are able to hear."* — Kali Linux motto

---

⭐ **Star this repo** if it helped you in your eJPT journey!
