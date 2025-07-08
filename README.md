# 🔍 Network Scanning with Nmap

## 🎯 Objective
To perform a basic network scan using Nmap on a target virtual machine, identify open ports and running services, and analyze the potential risks associated with each.

---

## 🛠 Tools Used
- **Operating System**: Kali Linux
- **Network Scanner**: Nmap
- **Target Machine**: Metasploitable2 (IP: 192.168.56.101)
- **Virtualization Platform**: VirtualBox

---

## 🧪 Nmap Command Used

```bash
sudo nmap -sV 192.168.56.101 -oN nmap_scan_results.txt
-sV: Enables version detection

-oN: Saves output in a readable format (nmap_scan_results.txt)

📊 Summary of Results
| Port | State | Service      | Version                      |
| ---- | ----- | ------------ | ---------------------------- |
| 21   | open  | ftp          | vsftpd 2.3.4                 |
| 22   | open  | ssh          | OpenSSH 4.7p1 Debian         |
| 23   | open  | telnet       | Linux telnetd                |
| 25   | open  | smtp         | Postfix smtpd                |
| 80   | open  | http         | Apache httpd 2.2.8 (Ubuntu)  |
| 139  | open  | netbios-ssn  | Samba smbd 3.x - 4.x         |
| 445  | open  | microsoft-ds | Samba smbd 3.x - 4.x         |
| 3306 | open  | mysql        | MySQL 5.0.51a-3ubuntu5       |
| 5432 | open  | postgresql   | PostgreSQL 8.3.0 - 8.3.7     |
| 5900 | open  | vnc          | VNC protocol 3.3             |
| 8180 | open  | http         | Apache Tomcat JSP Engine 1.1 |


📁 Output Files
nmap_scan_results.txt: Full scan result from the Nmap command.

📸 Screenshot
![Nmap Output](screenshots/nmap_output.png)

✅ Conclusion
This Nmap scan revealed various open ports and services running on the target system, many of which are outdated and potentially vulnerable. These results are useful for beginners learning penetration testing, vulnerability assessment, and network security analysis.

---

## 🚀 Author

**Shrishti Sharma**  
Beginner in Cybersecurity | Learning by Doing 💻🔒  


