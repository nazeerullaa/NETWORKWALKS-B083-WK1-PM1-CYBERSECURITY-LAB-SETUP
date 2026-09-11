# NETWORKWALKS-B083-WK1-PM1-CYBERSECURITY(soc)-LAB-SETUP
# 🔐 Cybersecurity Lab Environment

**Building an isolated virtual cybersecurity lab using VirtualBox, Kali Linux, and Windows 10**

![Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000)
![VirtualBox](https://img.shields.io/badge/VirtualBox-7.x-0070C0?style=flat-square&labelColor=000000)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-Linux-557C94?style=flat-square&labelColor=000000)
![Windows 10](https://img.shields.io/badge/Windows%2010-Target-0078D6?style=flat-square&labelColor=000000)
![Networking](https://img.shields.io/badge/Networking-10.0.0.0%2F24-238F89?style=flat-square&labelColor=000000)
![Penetration Testing](https://img.shields.io/badge/Penetration%20Testing-000000?style=flat-square&labelColor=000000)

---

## 📌 Project Overview

This project focuses on building a **controlled cybersecurity laboratory** using VirtualBox, Kali Linux, and Windows 10.

The lab provides an isolated environment for learning and practicing cybersecurity concepts such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Windows security monitoring
- Linux security tools
- Web security testing
- Penetration-testing fundamentals

The environment is designed so that Kali Linux can be used as the security-testing machine and Windows 10 can be used as a controlled target machine.

---

## 🎯 Objectives

The main objectives of this project are to:

- Install and configure VirtualBox.
- Set up Kali Linux as the security-testing VM.
- Set up Windows 10 as a target VM.
- Create a private virtual network.
- Configure communication between the virtual machines.
- Verify IP addressing and network connectivity.
- Perform basic network reconnaissance.
- Practice port scanning in the isolated lab.
- Capture and analyze network traffic.
- Create VM snapshots for recovery.
- Document the complete cybersecurity lab.

---

## 🏗️ Lab Architecture

```text
                    HOST COMPUTER
                          │
                      VirtualBox
                          │
              ┌───────────┴───────────┐
              │                       │
         KALI LINUX               WINDOWS 10
       Security VM                Target VM
              │                       │
              └───────────┬───────────┘
                          │
                 Private Lab Network
                     10.0.0.0/24
```

## ⚙️ Lab Configuration

| 🧩 Component | ⚙️ Configuration |
|---|---|
| 🖥️ Host OS | Windows 10 |
| 🧠 Host RAM | 8 GB |
| ⚡ Processor | Intel Core i7 |
| 🧰 Hypervisor | VirtualBox 7.2 |
| 🐉 Security OS | Kali Linux 2026.2 |
| 🧠 Kali RAM | 2048 MB |
| 🌐 Virtual Network | NAT Network |
| 📡 Network Address | 10.0.0.0/24 |
| 🐧 Kali IP Address | 10.0.0.2/24 |
| 🚪 Default Gateway | 10.0.0.1 |





| Machine    | Role                        | Operating System |
| ---------- | --------------------------- | ---------------- |
| Kali Linux | Security / Testing Machine  | Kali Linux       |
| Windows 10 | Target / Monitoring Machine | Windows 10       |



phase-1
Step 1. Download & install 7-zip: https://7-zip.org/download.html

<img width="1877" height="897" alt="Screenshot 2026-09-10 110243" src="https://github.com/user-attachments/assets/493dae43-779c-46a2-93af-3b3be256bf58" />


Step 2. Download & install Virtualbox on your laptop/PC: https://virtualbox.org/wiki/Downloads


<img width="1890" height="891" alt="Screenshot 2026-09-10 112143" src="https://github.com/user-attachments/assets/9fdb4a81-d477-4f5b-a4d0-a7ebefd0a86f" />

<img width="1916" height="1015" alt="Screenshot 2026-09-10 112425" src="https://github.com/user-attachments/assets/d633b236-7602-4a2e-afc0-fb840ab94337" />

Step 3.importent step3** Configure the network settings on your Virtualbox (create NATNetwork in 10.0.0.0/24)

go to virtualbox file>tools>network

<img width="1920" height="1080" alt="Screenshot 2026-09-10 114804" src="https://github.com/user-attachments/assets/beb521fd-e687-4743-9aa0-661ab2a91779" />

<img width="1920" height="1080" alt="Screenshot 2026-09-10 114944" src="https://github.com/user-attachments/assets/64957932-8f83-49fe-a500-d417c1e374a1" />

change ipaddress 10.0.0.0/24 click on apply

Step 4. Download & import Kali Linux Virtual Machine in your Virtualbox: https://kali.org/get-kali

click on given link>select virtual machine>recommed virtual box

<img width="1887" height="955" alt="Screenshot 2026-09-10 115607" src="https://github.com/user-attachments/assets/5f9f751f-a39a-473c-a475-bca190b95c50" />

Step 5. after downloading extract kail linex file in 7-zip

<img width="1178" height="533" alt="Screenshot 2026-09-10 120620" src="https://github.com/user-attachments/assets/c3272172-ea26-4647-88c9-78226b736baf" />

Step 6.after extraction copy the path

<img width="625" height="155" alt="Screenshot 2026-09-10 121025" src="https://github.com/user-attachments/assets/c78f8b74-201a-4d1d-a4f7-d90f1024db82" />

Step 7.open virtual machine>add>then past the path

<img width="1400" height="880" alt="image" src="https://github.com/user-attachments/assets/54b5a8ff-db2d-4c62-a9fe-683790f3ba4a" />

phase-2

step 1.download windows 10 https://www.microsoft.com/en-ca/software-download/windows10 
<img width="1867" height="827" alt="image" src="https://github.com/user-attachments/assets/4563668b-13ac-4c6d-a7d0-a16d600e92f9" />

step 2.open MediaCreationTool_22H2>click on Next
<img width="1166" height="988" alt="Screenshot 2026-09-10 172358" src="https://github.com/user-attachments/assets/af570114-b847-4014-acad-7f591c36c184" />

step 3.import windows 10 Machine in your Virtualbox

<img width="1882" height="932" alt="Screenshot 2026-09-10 172719" src="https://github.com/user-attachments/assets/b5120cae-3689-4d5a-b618-6879695e1852" />

step 4.click on "New">enter Name>iso image: windows 10 path
<img width="1597" height="975" alt="Screenshot 2026-09-10 172852" src="https://github.com/user-attachments/assets/95d55a72-ea14-4488-8d9a-d7115a3a25e0" />

step 5.windows 10 will be added in vm
<img width="1660" height="910" alt="image" src="https://github.com/user-attachments/assets/f1defa84-31a1-477a-bfbf-9a5dc673e3c5" />
step 6.click on start 

<img width="715" height="447" alt="Screenshot 2026-09-10 173006" src="https://github.com/user-attachments/assets/3a4c1912-a152-46fe-b29a-5bc81475dfc3" />

step 7.select language allow the permission

<img width="882" height="636" alt="Screenshot 2026-09-10 173034" src="https://github.com/user-attachments/assets/a1fd704b-878e-498a-a5e5-05271ff8da74" />

<img width="953" height="597" alt="Screenshot 2026-09-10 173121" src="https://github.com/user-attachments/assets/942dfb7e-0e50-4ef8-9b2b-6def9e708adf" />

🌐 Network Configuration

The virtual machines are configured on a private virtual network.

Example:
Network:       10.0.0.0/24

Kali Linux:    10.0.0.x
Windows 10:    10.0.0.x


🛠️ Tools & Technologies
-Virtualization
-VirtualBox
-Operating Systems
-Kali Linux
-Windows 10
-Security Tools
-Nmap
-Wireshark
-Metasploit Framework
-Burp Suite
-Netcat
-Networking
-TCP/IP
-IPv4
-DNS
-NAT
-Private IP addressing
-Ports and protocols
🔍 Lab Activities
1. Network Discovery

Identify the machines available inside the isolated lab network.

Example:

nmap -sn 10.0.0.0/24
2. Port Scanning

Perform authorized port scanning against the Windows 10 VM.

nmap <WINDOWS-IP>

The objective is to understand:

Open ports
Closed ports
Running services
Network exposure
3. Service Enumeration

Identify services running on the target machine.

nmap -sV <WINDOWS-IP>
4. Packet Analysis

Wireshark can be used to capture and analyze traffic between the virtual machines.

Topics investigated:

TCP traffic
UDP traffic
DNS queries
ICMP
TCP three-way handshake
Source and destination IP addresses
Source and destination ports
5. Vulnerability Assessment

The Windows 10 VM can be used as a controlled target for vulnerability-assessment exercises.

All testing is restricted to the isolated lab environment.


🔐 Security Considerations

This laboratory is intended only for education and authorized security testing.

The security-testing activities performed in this repository should only target:

Systems owned by me
Virtual machines created for testing
Systems for which explicit authorization has been provided

Testing external or unauthorized systems is not part of this project.

📚 Learning Outcomes

Through this project, I developed practical understanding of:

-Virtual machine configuration
-Linux security environment
-Windows target environment
-Virtual networking
-IP addressing
-Network reconnaissance
-Port scanning
-Service enumeration
-Packet analysis
-Cybersecurity lab management
-Ethical penetration-testing practices


⚠️ Disclaimer

This project is created strictly for educational purposes and authorized security testing.

Do not use the techniques or tools demonstrated here against systems without proper authorization.












