# 🔍 Nmap TCP SYN Scan - Local Network Recon

This repository documents the process of performing a basic Nmap TCP SYN scan on a local network, including a screenshot of the result.

## 🧰 Tools Used

- **Nmap** v7.97 (Network Mapper)
- **Windows Command Prompt**
- Local IP: `192.168.1.72`

## 📌 Objective

Perform a TCP SYN scan (`-sS`) on a local network IP to detect open ports and running services. The result is captured in a screenshot file (`Screenshot (21).png`).

## 🪜 Step-by-Step Process

### 1️⃣ Download & Install Nmap

1. Visit the official Nmap download page: [https://nmap.org/download.html](https://nmap.org/download.html)
2. Download the installer for your OS (e.g., **Windows**).
3. Run the installer and follow the installation steps.
4. After installation, Nmap can be accessed from Command Prompt.

### 2️⃣ Verify Nmap Installation

Open Command Prompt and run:

nmap --version
You should see the version info like Nmap version 7.97 if installed correctly.

3️⃣ Identify Target IP
Use the following command to find your IP:

"ipconfig"

Look for the IPv4 address under your Wi-Fi or Ethernet adapter. In this example, the target IP is:
IPv4 Address: 192.168.1.72
4️⃣ Perform a TCP SYN Scan
Run this command to scan the target:

"nmap -sS 192.168.1.72"

Explanation:
-sS → TCP SYN scan (stealthy and fast)
192.168.1.72 → target IP

5️⃣ Analyze the Output
You will see a result like:

PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
7070/tcp open  realserver
✔ These are common Windows networking and streaming ports.

6️⃣ Capture Screenshot
A screenshot of this scan result is saved as:

📁 Screenshot (21).png

You can view it in this repository.

📊 Scan Summary
Port	State	Service
135	open	msrpc
139	open	netbios-ssn
445	open	microsoft-ds
7070	open	realserver

🎯 Use Cases

🔐 Ethical hacking lab practice
🛡️ Internal network testing
🧪 Cybersecurity learning projects

⚠️ Disclaimer
This scan was done in a controlled environment on a local private network.
Do not scan devices or networks without permission. Unauthorized scanning is illegal.

📁 Repository Contents
Screenshot (21).png – Nmap scan result

README.md – Step-by-step guide

👨‍💻 Author
Ansh
BCA Student | Tech Enthusiast | Cybersecurity Learner

