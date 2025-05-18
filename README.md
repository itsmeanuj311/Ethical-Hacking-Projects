# Ethical Hacking Project

# 🛡️ Network Penetration Testing with Real-World Exploits and Security Remediation

This project simulates real-world network attacks and defense strategies using Kali Linux as the attacker machine and Metasploitable as the target. It includes scanning, enumeration, exploitation, password cracking, and remediation — all performed in a controlled lab environment for ethical learning purposes.

---

                                                
## 🎯 Objectives

- Understand and simulate real-world network attacks
- Perform scanning, enumeration, and exploitation using tools like Nmap and Metasploit
- Crack Linux password hashes using John the Ripper
- Identify outdated services and recommend security remediations

---

## 📂 Project Contents

- 📄 `Polished_CEH_Project_Swapnil.pdf` — Full report with screenshots and command outputs  
- 📄 `CEH_Project_Swapnil.pdf` — Full report with screenshots and command outputs  
- 🖼️ `Screenshots/` — Real-time evidence of network attacks and defenses  

---

## 💻 Lab Setup

### 🖥️ Operating Systems
- **Kali Linux** – Attacker Machine
- **Metasploitable 2** – Target Machine

### 🛠️ Tools Used
- `nmap` – Port, OS, and service version scanning
- `Metasploit Framework` – Exploitation
- `John the Ripper` – Password hash cracking
- Linux built-in commands – user management and enumeration

---

## 🚀 Tasks Performed

### 🔍 Network Scanning
- `nmap -v IP` – Basic scan
- `nmap -v -p- IP` – Full port scan
- `nmap -sV IP` – Service version detection
- `nmap -O IP` – OS detection

### 🔐 Hidden Ports Discovered
Ports like `8787`, `36588`, `53204`, etc., found through full port scans.

### 📡 Enumeration
- OS: Linux 2.6.x (Metasploitable)
- Open services: vsftpd, OpenSSH, Apache, MySQL, Samba, etc.
- Vulnerable ports: 21 (FTP), 445 (SMB), 512–514 (R Services)

### 💥 Exploitation
- **vsftpd 2.3.4** backdoor
- **SMB 3.0.20-Debian** using Metasploit
- **Rexec/Rlogin/Rsh** services using script-based vulnerabilities

### 👤 Privilege Escalation
- Created user `rahul` with root permissions
- Extracted and cracked password hash using John the Ripper

### 🔧 Remediation Steps
| Service   | Vulnerability                  | Fix                              |
|-----------|--------------------------------|----------------------------------|
| vsftpd    | Backdoor (CVE-2011-2523)       | Upgrade to 3.0.5 / use SFTP      |
| SMB       | RCE, Null Sessions             | Upgrade to Samba 4.20.1          |
| R Services| Plaintext creds (CVE-1999-0651)| Disable & use SSH instead        |

---

## 📚 Major Learning

Through this project, I learned how to create and manage users in Linux, analyze system files, crack password hashes, and detect services using Nmap. I practiced using commands like `nmap -sV`, `nmap -O`, and `john` to identify system weaknesses. I also understood how outdated services like FTP, SMB, and R services pose serious security risks and how to patch or replace them.

---

## ⚠️ Disclaimer

This project is for **educational purposes only**. All activities were performed in a **safe, offline lab environment**. Do not attempt these techniques on real networks without explicit permission.

---

## 📎 References

- [CVE-2011-2523](https://nvd.nist.gov/vuln/detail/CVE-2011-2523)
- [Metasploit Documentation](https://docs.rapid7.com/metasploit/)
- [John the Ripper](https://www.openwall.com/john/)
- [Apache Vulnerabilities](https://httpd.apache.org/security/)

## Overview

This repository contains seven beginner-level projects focused on ethical hacking and cybersecurity. Each project provides hands-on experience with essential techniques for network scanning, web application testing, password cracking, honeypot deployment, Wi-Fi auditing, phishing attack simulation, and SQL injection exploitation.


## Getting Started

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/Ethical-Hacking-Projects.git
    cd Ethical-Hacking-Projects
    ```

3. **Follow the Instructions:**
    Open the corresponding markdown file and follow the step-by-step instructions to complete the exercises.

## About Me

Hi, I'm Anuj Priyadarshi, attended at Rungta College of Engineering and Technology pursuing my B.Tech CSE(AIML) degree and currently I am in 4th Semester. 

## Connect with Me

- **LinkedIn**: [Anuj Priyadarshi](https://www.linkedin.com/in/itsmeanuj311)
- **Twitter**: [Anuj Priyadarshi](https://twitter.com/itsmeanuj311)

Feel free to connect with me on any of these platforms!

Thank you for visiting my GitHub page!
