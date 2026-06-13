# 🔴 Red Team Learning Journey – Day 11

## 📅 Day 11 – Post-Exploitation Basics in Active Directory

📍 Learned at RedTeam Hacker Academy (CPT4 Program) & TryHackMe

---

## 📌 Topics Covered

* What is Post-Exploitation
* Objectives of Post-Exploitation
* Privilege Escalation
* Credential Access
* Lateral Movement
* Persistence
* Enumeration After Compromise
* Windows Privileges
* Active Directory Enumeration
* Common Post-Exploitation Tools

---

## 🧠 What I Learned

### 🎯 What is Post-Exploitation

* Post-Exploitation is the phase that occurs after gaining initial access to a system
* Focuses on gathering information, escalating privileges, and expanding access within the environment

#### ⚙️ How It Works:

1. Gain initial access
2. Enumerate the system
3. Escalate privileges
4. Extract credentials
5. Move laterally through the network
6. Maintain access if authorized in the engagement scope

👉 The goal is to understand the impact of a successful compromise

---

### 🔍 Enumeration After Compromise

* Gathering information from the compromised system

#### ⚙️ How It Works:

* Identify users and groups
* Check running services
* View network configuration
* Discover shared resources

#### 🔧 Common Commands:

```cmd
whoami
hostname
ipconfig /all
net user
net localgroup administrators
systeminfo
```

---

### 🔑 Privilege Escalation

* Process of obtaining higher-level permissions

#### ⚙️ How It Works:

* Identify misconfigurations
* Find weak permissions
* Exploit privilege escalation paths

#### 🔧 Example Commands:

```cmd
whoami /priv
net user
```

👉 Administrative privileges provide greater access to the system

---

### 🔐 Credential Access

* Obtaining authentication-related information

#### ⚙️ How It Works:

* Search for stored credentials
* Identify password reuse
* Analyze authentication mechanisms

#### 🔧 Useful Commands:

```cmd
cmdkey /list
net accounts
```

👉 Credentials can reveal additional access paths in an environment

---

### 🌐 Lateral Movement

* Moving from one system to another within a network

#### ⚙️ How It Works:

* Use legitimate credentials
* Access network shares
* Connect to other systems

#### 🔧 Useful Commands:

```cmd
net view
net use
```

👉 Helps assess how far access can spread within a domain

---

### 📂 Active Directory Enumeration

* Discovering information about the AD environment

#### ⚙️ How It Works:

* Identify users
* Enumerate groups
* Discover domain information
* Map relationships between objects

#### 🔧 Common Commands:

```cmd
net user /domain
net group /domain
net group "Domain Admins" /domain
```

---

### ⚙️ Windows Privileges

* Permissions assigned to user accounts

#### ⚙️ How It Works:

* Define what actions users can perform
* Some privileges may provide escalation opportunities

#### 🔧 Command:

```cmd
whoami /priv
```

---

### 📌 Persistence

* Techniques used to maintain access during an authorized assessment

#### ⚙️ How It Works:

* Ensures continued access for testing purposes
* Demonstrates long-term impact of a compromise

👉 Must only be performed within the rules and scope of an authorized engagement

---

### 🛠️ Common Post-Exploitation Tools

#### 🔧 Examples:

* PowerShell
* Windows Command Prompt
* BloodHound
* SharpHound

#### ⚙️ How They Help:

* Gather information
* Visualize Active Directory relationships
* Identify privilege escalation paths

---

## 🛠️ Practical Understanding

* Learned what happens after initial compromise
* Practiced Windows and Active Directory enumeration
* Understood privilege escalation concepts
* Learned the importance of credential security
* Explored how attackers move within networks

---

## 💡 Key Takeaways

* Post-Exploitation begins after gaining access
* Enumeration is critical for understanding the environment
* Privilege escalation increases access levels
* Active Directory contains valuable information for assessments
* Lateral movement demonstrates the impact of compromised credentials
* Strong security controls can limit attacker movement and reduce risk

---

