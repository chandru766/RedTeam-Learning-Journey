# 🔴 Red Team Learning Journey – Day 09

## 📅 Day 9 – Nmap & Network Scanning

📍 Learned at RedTeam Hacker Academy (CPT4 Program)

---

## 📌 Topics Covered

* What is Nmap
* How Nmap Works
* Host Discovery
* TCP Connect Scan
* SYN Scan
* UDP Scan
* ACK Scan
* FIN Scan
* NULL Scan
* Xmas Scan
* Service Enumeration
* OS Detection
* Aggressive Scan
* Nmap Scripting Engine (NSE)
* Common Nmap Commands

---

## 🧠 What I Learned

### 🌐 What is Nmap

* Nmap (Network Mapper) is an open-source network scanning tool
* Used for host discovery, port scanning, service detection, and OS identification

#### ⚙️ How It Works:

* Sends specially crafted packets to a target
* Analyzes responses from the target machine
* Determines open ports, services, and operating system information

#### 🔧 Basic Scan:

```bash
nmap 192.168.1.10
```

👉 One of the most important tools for penetration testing and reconnaissance

---

### 🟢 Host Discovery Scan

* Used to identify live hosts on a network

#### ⚙️ How It Works:

* Sends discovery probes
* Identifies active devices
* Does not perform port scanning

#### 🔧 Command:

```bash
nmap -sn 192.168.1.0/24
```

---

### 🔵 TCP Connect Scan

* Performs a full TCP three-way handshake

#### ⚙️ How It Works:

* Connects completely to the target port
* Easy to detect but reliable

#### 🔧 Command:

```bash
nmap -sT 192.168.1.10
```

---

### ⚡ SYN Scan (Half-Open Scan)

* Most commonly used Nmap scan

#### ⚙️ How It Works:

* Sends SYN packet
* Receives SYN-ACK
* Sends RST instead of completing connection

#### 🔧 Command:

```bash
sudo nmap -sS 192.168.1.10
```

👉 Faster and stealthier than TCP Connect Scan

---

### 🟠 UDP Scan

* Used to discover UDP services

#### ⚙️ How It Works:

* Sends UDP packets to target ports
* Analyzes responses

#### 🔧 Command:

```bash
sudo nmap -sU 192.168.1.10
```

👉 Useful for DNS, SNMP, DHCP services

---

### 🟣 ACK Scan

* Used for firewall analysis

#### ⚙️ How It Works:

* Sends ACK packets
* Determines whether ports are filtered

#### 🔧 Command:

```bash
sudo nmap -sA 192.168.1.10
```

---

### 🟤 FIN Scan

* Sends FIN packets to the target

#### ⚙️ How It Works:

* Open ports ignore the packet
* Closed ports respond with RST

#### 🔧 Command:

```bash
sudo nmap -sF 192.168.1.10
```

---

### ⚫ NULL Scan

* Sends packets without any TCP flags

#### ⚙️ How It Works:

* Useful for identifying filtered ports
* Can sometimes bypass basic filtering

#### 🔧 Command:

```bash
sudo nmap -sN 192.168.1.10
```

---

### ⚪ Xmas Scan

* Sends packets with FIN, PSH, and URG flags enabled

#### ⚙️ How It Works:

* Checks target responses to identify port states

#### 🔧 Command:

```bash
sudo nmap -sX 192.168.1.10
```

---

### 🔧 Service Enumeration

* Identifies services and versions running on open ports

#### ⚙️ How It Works:

* Connects to services
* Reads banners and responses

#### 🔧 Command:

```bash
nmap -sV 192.168.1.10
```

---

### 🖥️ Operating System Detection

* Detects the target operating system

#### ⚙️ How It Works:

* Compares responses against Nmap's fingerprint database

#### 🔧 Command:

```bash
sudo nmap -O 192.168.1.10
```

---

### 🚀 Aggressive Scan

* Performs advanced enumeration

#### ⚙️ How It Works:

* Combines multiple scanning techniques
* Detects OS, versions, scripts, and traceroute information

#### 🔧 Command:

```bash
sudo nmap -A 192.168.1.10
```

---

### 📜 Nmap Scripting Engine (NSE)

* Powerful scripting feature in Nmap

#### ⚙️ How It Works:

* Uses scripts to automate enumeration and information gathering

#### 🔧 Commands:

```bash
nmap --script=vuln 192.168.1.10
```

```bash
nmap --script=http-title 192.168.1.10
```

```bash
nmap --script=smb-os-discovery 192.168.1.10
```

👉 Extends Nmap beyond simple port scanning

---

### 🛠️ Common Nmap Commands

#### Scan All Ports

```bash
nmap -p- 192.168.1.10
```

#### Scan Specific Ports

```bash
nmap -p 22,80,443 192.168.1.10
```

#### Save Results

```bash
nmap -oN scan.txt 192.168.1.10
```

#### Faster Scan

```bash
nmap -T4 192.168.1.10
```

#### Scan Entire Subnet

```bash
nmap 192.168.1.0/24
```

---

## 🛠️ Practical Understanding

* Learned how to discover live hosts
* Understood different scanning techniques
* Practiced service and version enumeration
* Learned OS detection methods
* Explored Nmap NSE scripts

---

## 💡 Key Takeaways

* Nmap is a powerful reconnaissance and scanning tool
* Different scan types provide different information
* Service enumeration helps identify attack surfaces
* OS detection provides valuable target information
* NSE scripts automate advanced scanning tasks
* Reconnaissance is the foundation of penetration testing

---
