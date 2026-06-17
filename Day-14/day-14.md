# 🔴 Red Team Learning Journey – Day 14

## 📅 Day 14 – Burp Suite & OWASP ZAP

📍 Learned at RedTeam Hacker Academy (CPT4 Program)

---

## 📌 Topics Covered

* Burp Suite
* OWASP ZAP
* Web Application Testing
* Intercepting Requests
* Modifying Requests and Responses
* Spidering / Crawling
* Active Scanning
* Passive Scanning
* Repeater
* Intruder
* Fuzzer

---

## 🧠 What I Learned

### 🟠 Burp Suite

* Burp Suite is a web application security testing tool used by penetration testers.
* It acts as a proxy between the browser and the target web application.

#### ⚙️ How It Works:

1. Configure the browser to use Burp Proxy.
2. Intercept HTTP/HTTPS requests.
3. Analyze and modify requests before forwarding them.
4. Test web application functionality and security.

#### 🔧 Common Features:

* Proxy
* Repeater
* Intruder
* Decoder
* Comparer
* Scanner (Professional Edition)

👉 One of the most popular tools for web application penetration testing.

---

### 🔄 Burp Proxy

* Used to intercept and inspect web traffic.

#### ⚙️ How It Works:

* Captures requests sent from the browser.
* Allows modification before sending them to the server.
* Displays server responses.

#### Example Workflow:

```text
Browser
   ↓
Burp Proxy
   ↓
Target Website
```

---

### 🔁 Burp Repeater

* Used to resend and modify individual HTTP requests.

#### ⚙️ How It Works:

1. Send a request to Repeater.
2. Modify parameters, headers, or cookies.
3. Resend the request.
4. Analyze the response.

👉 Useful for manual testing and parameter manipulation.

---

### 🎯 Burp Intruder

* Used for automated testing of input fields.

#### ⚙️ How It Works:

* Sends multiple requests with different payloads.
* Helps identify weak inputs and authentication issues.

#### Common Uses:

* Username enumeration
* Password testing (authorized environments only)
* Input validation testing

---

### 🔵 OWASP ZAP

* OWASP ZAP (Zed Attack Proxy) is an open-source web application security testing tool.

#### ⚙️ How It Works:

1. Configure browser proxy settings.
2. Route traffic through ZAP.
3. Crawl the application.
4. Identify security issues.

👉 Beginner-friendly and widely used in security assessments.

---

### 🕷️ Spider / Crawling

* Automatically discovers pages and resources.

#### ⚙️ How It Works:

* Follows links throughout the application.
* Maps the structure of the website.

#### Benefits:

* Identifies hidden pages
* Improves application visibility

---

### 🔍 Passive Scanning

* Analyzes traffic without sending additional requests.

#### ⚙️ How It Works:

* Observes requests and responses.
* Identifies common security misconfigurations.

#### Examples:

* Missing security headers
* Information disclosure

---

### ⚡ Active Scanning

* Sends additional requests to test for vulnerabilities.

#### ⚙️ How It Works:

* Performs security checks on discovered pages.
* Identifies potential weaknesses.

#### Examples:

* SQL Injection indicators
* Cross-Site Scripting (XSS) indicators
* Misconfigurations

---

### 🎲 Fuzzer

* Used to test application inputs with various payloads.

#### ⚙️ How It Works:

* Sends multiple input variations.
* Observes application behavior and responses.

👉 Helps identify input validation weaknesses.

---

## ⚖️ Burp Suite vs OWASP ZAP

| Feature         | Burp Suite                   | OWASP ZAP          |
| --------------- | ---------------------------- | ------------------ |
| Cost            | Community & Professional     | Free & Open Source |
| Ease of Use     | Beginner to Advanced         | Beginner Friendly  |
| Active Scanning | Limited in Community Edition | Available          |
| Web Testing     | Excellent                    | Excellent          |
| Industry Usage  | Very High                    | High               |

---

## 🛠️ Practical Understanding

* Learned how web proxies work.
* Intercepted and analyzed HTTP requests.
* Understood request and response modification.
* Learned the difference between passive and active scanning.
* Explored the major features of Burp Suite and OWASP ZAP.

---

## 💡 Key Takeaways

* Burp Suite and OWASP ZAP are powerful web application testing tools.
* Proxies allow testers to inspect and modify web traffic.
* Repeater helps perform manual testing.
* Intruder and fuzzing features help automate testing tasks.
* Active and passive scanning help identify security issues.
* Understanding these tools is essential for web application penetration testing.

---

