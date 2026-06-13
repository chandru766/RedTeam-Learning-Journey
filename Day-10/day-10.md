# 🔴 Red Team Learning Journey – Day 10

## 📅 Day 10 – Active Directory Fundamentals

📍 Learned at RedTeam Hacker Academy (CPT4 Program) & TryHackMe

---

## 📌 Topics Covered

* What is Active Directory (AD)
* How Active Directory Works
* Domain
* Domain Controller (DC)
* Organizational Units (OU)
* Users and Groups
* Authentication
* Kerberos
* LDAP
* Group Policy Objects (GPO)
* Active Directory Structure

---

## 🧠 What I Learned

### 🏢 What is Active Directory

* Active Directory (AD) is a directory service developed by Microsoft
* Used to manage users, computers, groups, and resources within a network

#### ⚙️ How It Works:

* Stores information about network objects
* Centralizes authentication and authorization
* Allows administrators to manage users and devices from a single location

👉 Widely used in enterprise environments

---

### 🌐 Domain

* A domain is a logical group of network objects

#### ⚙️ How It Works:

* Contains users, computers, groups, and policies
* Provides centralized management

#### 🔧 Example:

```text
corp.local
company.local
```

---

### 🖥️ Domain Controller (DC)

* A server that manages Active Directory services

#### ⚙️ How It Works:

* Stores the AD database
* Authenticates users
* Enforces security policies

👉 The heart of an Active Directory environment

---

### 📂 Organizational Units (OU)

* Containers used to organize AD objects

#### ⚙️ How It Works:

* Groups users and computers
* Makes administration easier
* Allows policies to be applied to specific departments

#### 🔧 Example:

```text
HR
IT
Finance
Marketing
```

---

### 👤 Users and Groups

* Users represent individual accounts
* Groups are collections of users

#### ⚙️ How It Works:

* Permissions can be assigned to groups
* Easier to manage access control

#### 🔧 Example:

```text
Domain Admins
Domain Users
IT Support
```

---

### 🔐 Authentication

* Process of verifying a user's identity

#### ⚙️ How It Works:

1. User enters credentials
2. Domain Controller verifies them
3. Access is granted if valid

👉 Ensures only authorized users can access resources

---

### 🎫 Kerberos

* Default authentication protocol in Active Directory

#### ⚙️ How It Works:

1. User requests a Ticket Granting Ticket (TGT)
2. Domain Controller issues the ticket
3. User uses the ticket to access services

👉 More secure than older authentication methods

---

### 📖 LDAP

* Lightweight Directory Access Protocol

#### ⚙️ How It Works:

* Used to query and manage directory information
* Allows applications to interact with Active Directory

#### 🔧 Example Port:

```text
389  - LDAP
636  - LDAPS (Secure LDAP)
```

---

### ⚙️ Group Policy Objects (GPO)

* Used to manage settings across the domain

#### ⚙️ How It Works:

* Administrators create policies
* Policies are applied to users and computers
* Enforces security configurations

#### 🔧 Examples:

* Password policies
* Desktop restrictions
* Software deployment

---

### 🏗️ Active Directory Structure

#### Components:

```text
Forest
 └── Tree
      └── Domain
           └── Organizational Units
                ├── Users
                ├── Groups
                └── Computers
```

👉 AD uses a hierarchical structure for organization and management

---

## 🛠️ Practical Understanding

* Learned how organizations manage users centrally
* Understood the role of Domain Controllers
* Learned how Kerberos authentication works
* Explored LDAP and Active Directory structure
* Understood how GPOs enforce security policies

---

## 💡 Key Takeaways

* Active Directory is the backbone of many enterprise networks
* Domain Controllers manage authentication and authorization
* Kerberos provides secure authentication
* LDAP is used to query directory information
* GPOs help enforce organizational security policies
* Understanding AD is essential for both Red Team and Blue Team operations

---

