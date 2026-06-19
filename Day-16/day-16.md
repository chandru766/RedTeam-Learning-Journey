# 🔴 Red Team Learning Journey – Day 16

## 📅 Day 16 – Burp Suite Fundamentals

📍 Learned at RedTeam Hacker Academy (CPT4 Program)

---

## 📌 Topics Covered

* What is Burp Suite
* How Burp Suite Works
* Proxy
* Intercept
* HTTP Requests & Responses
* Repeater
* Intruder
* Decoder
* Comparer
* Target Tab
* Site Map

---

## 🧠 What I Learned

### 🟠 What is Burp Suite

* Burp Suite is a web application security testing tool.
* It acts as a proxy between a browser and a web application.
* Widely used by penetration testers to analyze and test web applications.

#### ⚙️ How It Works:

```text
Browser
   ↓
Burp Suite
   ↓
Target Website
```

* Captures HTTP/HTTPS traffic.
* Allows inspection and modification of requests and responses.

👉 One of the most important tools for Web Application Penetration Testing.

---

### 🔄 Proxy

* The Proxy feature intercepts traffic between the browser and the target application.

#### ⚙️ How It Works:

1. Browser sends a request.
2. Burp intercepts the request.
3. Tester reviews or modifies it.
4. Request is forwarded to the server.

#### Benefits:

* Analyze traffic
* Modify requests
* Test application behavior

---

### ✋ Intercept

* Allows requests to be paused before reaching the server.

#### ⚙️ How It Works:

* Capture requests
* Modify parameters
* Forward modified requests

👉 Useful for testing authentication, authorization, and input validation.

---

### 📨 HTTP Requests & Responses

#### Request Components:

* Method (GET, POST, PUT, DELETE)
* URL
* Headers
* Body

#### Response Components:

* Status Code
* Headers
* Body

#### Example:

```http
GET /login HTTP/1.1
Host: example.com
```

---

### 🔁 Repeater

* Used to resend and modify individual requests.

#### ⚙️ How It Works:

1. Send request to Repeater.
2. Modify values.
3. Click Send.
4. Analyze the response.

👉 Excellent for manual testing.

---

### 🎯 Intruder

* Used to automate testing with multiple payloads.

#### ⚙️ How It Works:

1. Select target parameter.
2. Add payload list.
3. Launch attack.
4. Analyze results.

#### Common Uses:

* Parameter testing
* Input validation testing
* Security assessments

---

### 🔐 Decoder

* Encodes and decodes data.

#### Supported Formats:

* URL
* Base64
* HTML
* Hexadecimal

#### Example:

```text
SGVsbG8=
```

Decoded Output:

```text
Hello
```

---

### ⚖️ Comparer

* Compares two pieces of data.

#### ⚙️ How It Works:

* Compare requests
* Compare responses
* Identify differences

👉 Useful during testing and analysis.

---

### 🎯 Target Tab

* Displays discovered hosts and web content.

#### Features:

* Scope management
* Target organization
* Site mapping

---

### 🗺️ Site Map

* Shows all discovered application content.

#### Benefits:

* Understand application structure
* Identify hidden pages
* Discover attack surface

---

## 🛠️ Practical Understanding

* Configured browser proxy settings.
* Intercepted HTTP requests and responses.
* Modified parameters using Repeater.
* Explored Burp Suite modules.
* Learned how web application traffic flows.
* Understood how testers analyze web applications.

---

## 💡 Key Takeaways

* Burp Suite is a powerful web application testing tool.
* Proxy and Intercept are fundamental features.
* Repeater is useful for manual testing.
* Intruder helps automate testing tasks.
* Decoder and Comparer assist with analysis.
* Understanding HTTP traffic is essential for web security testing.

---

## 🚀 Tools Practiced

* Burp Suite Community Edition
* Web Browser Proxy Configuration
* HTTP Request Analysis
* Manual Web Application Testing

---

