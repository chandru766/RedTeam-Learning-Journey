# 🔴 Red Team Learning Journey – Day 15

## 📅 Day 15 – API Security & Web Application Vulnerabilities

📍 Learned at RedTeam Hacker Academy (CPT4 Program)

---

## 📌 Topics Covered

* API Penetration Testing
* IDOR (Insecure Direct Object Reference)
* Excessive Data Exposure
* Broken Authentication
* Broken Access Control
* Reflected XSS
* Stored XSS
* DOM-Based XSS
* Security Misconfiguration
* Improper Asset Management
* Injection Attacks
* Lack of Rate Limiting
* PortSwigger Web Security Academy

---

## 🧠 What I Learned

### 🔌 API Penetration Testing

* API Pentesting is the process of assessing APIs for security vulnerabilities.
* APIs expose functionality and data between applications.

#### ⚙️ How It Works:

* Analyze API endpoints
* Test authentication and authorization
* Inspect requests and responses
* Identify security weaknesses

#### 🔧 Common Tools:

* Burp Suite
* OWASP ZAP
* Postman

👉 APIs are a common target because they often expose sensitive business logic and data.

---

### 🔓 IDOR (Insecure Direct Object Reference)

* Occurs when users can access resources they shouldn't have access to.

#### ⚙️ How It Works:

* Application exposes direct object identifiers.
* Access control checks are missing or weak.
* Attackers modify identifiers to access other users' data.

#### Example:

```text
/user/profile?id=1001
```

Changing the ID may expose another user's profile if authorization is not enforced.

---

### 📤 Excessive Data Exposure

* APIs return more information than necessary.

#### ⚙️ How It Works:

* Backend sends sensitive data.
* Frontend hides some fields.
* Attackers inspect API responses and discover exposed information.

#### Examples:

* Email addresses
* Internal IDs
* Phone numbers
* User roles

---

### 🔑 Broken Authentication

* Weak authentication mechanisms allow unauthorized access.

#### ⚙️ How It Works:

* Poor session management
* Weak password policies
* Predictable tokens

#### Risks:

* Account takeover
* Unauthorized access

---

### 🚪 Broken Access Control

* Users can perform actions beyond their intended permissions.

#### ⚙️ How It Works:

* Missing authorization checks
* Privilege escalation opportunities
* Unauthorized access to resources

👉 One of the most critical web security issues.

---

### 🪞 Reflected XSS

* Malicious input is reflected immediately in the response.

#### ⚙️ How It Works:

1. User submits input.
2. Server reflects the input.
3. Browser executes the script.

👉 Requires user interaction.

---

### 💾 Stored XSS

* Malicious payload is permanently stored by the application.

#### ⚙️ How It Works:

1. Attacker submits input.
2. Application stores the payload.
3. Other users load the page.
4. Browser executes the payload.

👉 More dangerous because it affects multiple users.

---

### 🌐 DOM-Based XSS

* Vulnerability occurs entirely in the browser.

#### ⚙️ How It Works:

* Client-side JavaScript processes untrusted input.
* DOM is modified dynamically.
* Malicious code executes in the browser.

👉 The vulnerability exists in client-side code rather than server-side code.

---

### ⚙️ Security Misconfiguration

* Improper security settings expose systems to risk.

#### Examples:

* Default credentials
* Unnecessary services
* Verbose error messages
* Missing security headers

#### Impact:

* Increased attack surface
* Information disclosure

---

### 📦 Improper Asset Management

* Failure to properly manage and track assets.

#### Examples:

* Forgotten APIs
* Deprecated endpoints
* Unused servers
* Shadow IT resources

#### Risks:

* Unpatched vulnerabilities
* Unauthorized access paths

---

### 💉 Injection Attacks

* Untrusted input is interpreted as commands or queries.

#### ⚙️ How It Works:

* Application fails to validate input.
* Backend processes malicious input.
* Unexpected actions occur.

#### Examples:

* SQL Injection
* NoSQL Injection
* Command Injection

👉 Input validation is critical for preventing injection vulnerabilities.

---

### ⏱️ Lack of Rate Limiting

* Application fails to restrict excessive requests.

#### ⚙️ How It Works:

* Attackers send large numbers of requests.
* Application does not enforce limits.

#### Risks:

* Brute-force attacks
* Resource exhaustion
* API abuse

---

### 🎓 PortSwigger Web Security Academy

* Free platform for learning web application security.

#### ⚙️ How It Works:

* Provides interactive labs.
* Demonstrates real-world vulnerabilities.
* Allows safe hands-on practice.

#### Topics Available:

* XSS
* SQL Injection
* Authentication
* Access Control
* API Security

👉 Excellent platform for improving web application security skills.

---

## 🛠️ Practical Understanding

* Learned common API security vulnerabilities.
* Understood authentication and authorization weaknesses.
* Explored different types of XSS vulnerabilities.
* Learned how misconfigurations increase risk.
* Practiced identifying common web application security issues.
* Used PortSwigger labs to reinforce concepts.

---

## 💡 Key Takeaways

* APIs require strong authentication and authorization.
* IDOR and Broken Access Control can expose sensitive data.
* Excessive Data Exposure reveals unnecessary information.
* XSS vulnerabilities can impact users and applications.
* Security Misconfiguration is a common cause of breaches.
* Rate limiting helps prevent abuse and automated attacks.
* Hands-on practice platforms like PortSwigger are valuable for learning web security.

---

