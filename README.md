# EJPT — Consolidated Notes (Brief Description)

This document provides a **brief yet comprehensive overview** of each EJPT module — covering every major stage of penetration testing, tools, and concepts.

---

## 1. Information Gathering

This is the **first step** in any penetration test. It focuses on collecting as much information as possible about the target without actively engaging it. Techniques include **OSINT (Open Source Intelligence)**, searching for domain info, IP addresses, email leaks, social media data, and technologies used. Tools like **whois, nslookup, Maltego, Recon-ng, Shodan, and Google Dorks** are commonly used.

**Goal:** Build an intelligence profile of the target before scanning or attacking.

**Link:** [https://dharmendrastm.medium.com/ejpt-1-1-information-gathering-0423a9bbc06e](https://dharmendrastm.medium.com/ejpt-1-1-information-gathering-0423a9bbc06e)

---

## 2. Footprinting & Scanning

After gathering information, the next phase involves **active probing** of the target system. You identify open ports, services, and operating systems. Tools like **Nmap, Masscan, and Netdiscover** are used to perform **port scanning, OS detection, and service enumeration**. This step helps create a clear attack surface.

**Goal:** Map the target network and identify potential entry points.

**Link:** [https://dharmendrastm.medium.com/ejpt-1-2-footprinting-scanning-f2f49b9564f5](https://dharmendrastm.medium.com/ejpt-1-2-footprinting-scanning-f2f49b9564f5)

---

## 3. Enumeration

Enumeration is a **deeper level of interaction** with the target. It involves extracting usernames, shares, services, and version details from open ports. Common protocols include **SMB, SNMP, DNS, LDAP, FTP, and HTTP**. Tools like **enum4linux, SNMPwalk, rpcclient, and Dirbuster** are used.

**Goal:** Discover valuable information for exploitation (e.g., usernames, directories, or misconfigurations).

**Link:** [https://dharmendrastm.medium.com/ejpt-1-3-enumeration-bf658c341ac1](https://dharmendrastm.medium.com/ejpt-1-3-enumeration-bf658c341ac1)

---

## 4. Vulnerability Assessment

In this stage, testers **identify and evaluate vulnerabilities** in systems or networks. Tools like **Nessus, OpenVAS, and Nmap scripts** are used to detect CVEs and weaknesses. The focus is on classifying vulnerabilities based on severity (Critical, High, Medium, Low).

**Goal:** Find potential vulnerabilities before attempting exploitation.

**Link:** [https://dharmendrastm.medium.com/ejpt-1-4-vulnerability-assessment-85ed97372f20](https://dharmendrastm.medium.com/ejpt-1-4-vulnerability-assessment-85ed97372f20)

---

## 5. Auditing Fundamentals

This module covers how to **analyze and assess security controls** in an organization. It focuses on **log analysis, compliance checks, and auditing tools**. Security auditing ensures all configurations meet best practices and policies.

**Goal:** Understand how auditors review systems and ensure data integrity.

**Link:** [https://dharmendrastm.medium.com/ejpt-2-1-auditing-fundamentals-d59d9b6d5bd1](https://dharmendrastm.medium.com/ejpt-2-1-auditing-fundamentals-d59d9b6d5bd1)

---

## 6. System / Host-based Attacks

This part explores **attacks targeting operating systems and applications**. You learn about privilege escalation, weak password policies, misconfigurations, and local exploits. Tools like **Metasploit, PowerShell, and Mimikatz** are commonly used.

**Goal:** Gain control or escalate privileges on a compromised system.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-1-system-host-based-attacks-956cfbe914bb](https://dharmendrastm.medium.com/ejpt-3-1-system-host-based-attacks-956cfbe914bb)

---

## 7. Network-based Attacks

These attacks exploit **network protocols and configurations**. Techniques include sniffing, spoofing, and performing man-in-the-middle (MITM) attacks. Tools such as **Wireshark, Ettercap, and Responder** are used to intercept and manipulate traffic.

**Goal:** Intercept, manipulate, or exploit network traffic for credentials or sensitive data.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-2-network-based-attacks-6f0d4d41b455](https://dharmendrastm.medium.com/ejpt-3-2-network-based-attacks-6f0d4d41b455)

---

## 8. The Metasploit Framework

Metasploit is a powerful exploitation framework that simplifies vulnerability research and exploitation. It allows you to use modules like **exploit, payload, post, and auxiliary** to perform attacks. It’s ideal for automating penetration tests.

**Goal:** Use Metasploit to exploit vulnerabilities and manage post-exploitation sessions.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-3-the-metasploit-framework-24439d1238c5](https://dharmendrastm.medium.com/ejpt-3-3-the-metasploit-framework-24439d1238c5)

---

## 9. Exploitation

This module teaches how to **use exploits to gain access** to vulnerable systems. You’ll learn manual and automated exploitation using public exploits, payload generation, and shell management.

**Goal:** Gain access and demonstrate impact through controlled exploitation.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-4-exploitation-d68f291951c8](https://dharmendrastm.medium.com/ejpt-3-4-exploitation-d68f291951c8)

---

## 10. Post-Exploitation

Once access is obtained, post-exploitation focuses on **maintaining control**, collecting credentials, and pivoting within the network. This step also involves cleaning up traces to remain undetected.

**Goal:** Understand how attackers maintain persistence and gather intelligence after a breach.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-5-post-exploitation-0ae5db04ef11](https://dharmendrastm.medium.com/ejpt-3-5-post-exploitation-0ae5db04ef11)

---

## 11. Social Engineering

This module covers **human-based attacks**, such as phishing, pretexting, and baiting. It explores psychological manipulation and defense measures. Tools like **SET (Social Engineering Toolkit)** are introduced.

**Goal:** Understand and defend against manipulation-based attacks.

**Link:** [https://dharmendrastm.medium.com/ejpt-3-6-social-engineering-ebb6e959b04f](https://dharmendrastm.medium.com/ejpt-3-6-social-engineering-ebb6e959b04f)

---

## 12. Web Application Penetration Testing

This section focuses on **web-based vulnerabilities** such as **SQL Injection, XSS, CSRF, authentication bypass, and file inclusion**. Tools like **Burp Suite, OWASP ZAP, Nikto, and SQLmap** are used.

**Goal:** Identify and exploit vulnerabilities in web applications safely and ethically.

**Link:** [https://dharmendrastm.medium.com/ejpt-4-1-web-application-penetration-testing-1fc636e6cabe](https://dharmendrastm.medium.com/ejpt-4-1-web-application-penetration-testing-1fc636e6cabe)

---

## Conclusion

These notes collectively cover the full **penetration testing lifecycle** — from reconnaissance to reporting. Mastering these topics ensures strong foundational knowledge for real-world cybersecurity engagements and eJPT certification success.
