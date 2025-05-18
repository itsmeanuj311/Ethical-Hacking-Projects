# Ethical Hacking Projects for Beginners

# 🛡️ Network Penetration Testing with Real-World Exploits and Security Remediation

This project simulates real-world network attacks and defense strategies using Kali Linux as the attacker machine and Metasploitable as the target. It includes scanning, enumeration, exploitation, password cracking, and remediation — all performed in a controlled lab environment for ethical learning purposes.

---

                                                
## 🎯 Objectives

- Understand and simulate real-world network attacks
- Perform scanning, enumeration, and exploitation using tools like Nmap and Metasploit
- Crack Linux password hashes using John the Ripper
- Identify outdated services and recommend security remediations

---

## 💻 Lab Setup

### 🖥️ Operating Systems
- **Kali Linux** – Attacker Machine
- **Metasploitable 2** – Target Machine

### 🛠️ Tools Used
- `nmap` – Port, OS, and service version scanning
- `Metasploit` – Exploitation
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

## Projects

### 1. [Scanning and Enumerating a Local Network with Nmap](https://github.com/itsmeanuj311/Ethical-Hacking-Projects/blob/main/Project-1-Scanning-and-Enumerating-a-Local-Network-with-Nmap.md)
Learn how to use Nmap to discover devices and services running on a local network. This project covers basic network scans, identifying open ports, and gathering information about network devices.

- **Key Topics:** Network Scanning, Enumeration, Nmap
- **Tools:** Kali Linux, Nmap

### 2. [Penetration Testing a Vulnerable Web Application using OWASP Juice Shop](https://github.com/itsmeanuj311/Ethical-Hacking-Projects-for-beginners/blob/main/Project-2-Penetration-Testing-a-Vulnerable-Web-Application.md)
Use various tools to perform penetration testing on OWASP Juice Shop, a deliberately insecure web application. This project covers identifying and exploiting web vulnerabilities.

- **Key Topics:** Web Application Testing, OWASP Juice Shop, Vulnerability Exploitation
- **Tools:** Kali Linux, OWASP Juice Shop, Burp Suite

### 3. [Cracking Password Hashes with John the Ripper](https://github.com//Ethical-Hacking-Projects/blob/main/Project-3-Cracking-Password-Hashes-with-John-the-Ripper-on-Kali-Linux.md)
Learn how to use John the Ripper to crack password hashes. This project covers basic password cracking, using custom wordlists, and cracking shadow file hashes.

- **Key Topics:** Password Cracking, John the Ripper, Hash Analysis
- **Tools:** Kali Linux, John the Ripper

### 4. [Deploying and Monitoring a Honeypot with Cowrie](https://github.com/itsmeanuj311/Ethical-Hacking-Projects/blob/main/project-4-Deploying-and-Monitoring-a-Honeypot-with-Cowrie-on-Kali-Linux.md)
Deploy and monitor a honeypot using Cowrie. This project covers setting up Cowrie, simulating attacks, monitoring logs, and analyzing captured data.

- **Key Topics:** Honeypot Deployment, Intrusion Monitoring, Cowrie
- **Tools:** Kali Linux, Cowrie, Docker, Splunk

### 5. [Auditing and Attacking a Wi-Fi Network with Aircrack-ng](https://github.com/itsmeanuj311/Ethical-Hacking-Projects/blob/main/Project-5-Auditing-and-Attacking-a-Wi-Fi-Network-with-Aircrack-ng.md)
Learn how to audit and attack Wi-Fi networks using Aircrack-ng. This project covers setting up a Wi-Fi adapter in monitor mode, capturing handshake packets, and cracking Wi-Fi passwords.

- **Key Topics:** Wi-Fi Auditing, Packet Capture, Password Cracking
- **Tools:** Kali Linux, Aircrack-ng, Wi-Fi Adapter

### 6. [Creating and Defending Against Phishing Attacks](https://github.com/itsmeanuj311/Ethical-Hacking-Projects/blob/main/Project-6-Building-Phishing-Simulation-on-kali-linux.md)
Simulate phishing attacks and learn how to defend against them. This project covers crafting phishing emails, launching phishing campaigns, and implementing anti-phishing measures.

- **Key Topics:** Phishing Simulation, Social Engineering, Defense Strategies
- **Tools:** Kali Linux, Gophish

### 7. [Exploiting and Securing a Database using SQL Injection on DVWA](https://github.com/itsmeanuj311/Ethical-Hacking-Projects/blob/main/Project-7-Exploiting-and-Securing-a-Database-using-SQL-Injection-on-DVWA.md)
Identify and exploit SQL injection vulnerabilities using DVWA. This project covers SQL injection techniques, using SQLMap for automated exploitation, and securing databases.

- **Key Topics:** SQL Injection, Database Security, DVWA
- **Tools:** Kali Linux, DVWA, SQLMap

## Getting Started

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/Ethical-Hacking-Projects.git
    cd Ethical-Hacking-Projects
    ```

2. **Navigate to Each Project Directory:**
    Each project has its own markdown file with detailed instructions. For example:
    ```bash
    cd project-1-scanning-using-nmap
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
