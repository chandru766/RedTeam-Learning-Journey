# 🔴 Red Team Learning Journey – Day 08

## 📅 Day 8 – OSINT Tools & Techniques

📍 Learned at RedTeam Hacker Academy (CPT4 Program)

---

## 📌 Topics Covered

* Shodan Tool
* Maltego
* theHarvester
* Hunter
* Google Dorking
* DorkFinder

---

## 🧠 What I Learned

### 🔎 Shodan

* Search engine for internet-connected devices

#### ⚙️ How It Works:

* Scans the internet for open ports and services
* Collects banners (service information)
* Indexes devices for searching

#### 🔧 Example Queries:

```bash id="f79a0o"
apache country:IN
nginx port:80
webcam
```

👉 Helps identify exposed systems and services

---

### 🧩 Maltego

* OSINT tool for link analysis and visualization

#### ⚙️ How It Works:

* Uses **transforms** to gather data from multiple sources
* Connects entities like domains, emails, IPs
* Displays relationships in a graph

#### 🔧 Usage:

1. Open Maltego
2. Add a domain/email entity
3. Run transforms
4. Analyze graph results

---

### 🐍 theHarvester

* Tool for collecting emails, subdomains, hostnames

#### ⚙️ How It Works:

* Queries public data sources (Google, Bing, LinkedIn, etc.)
* Extracts emails, domains, and IPs
* Aggregates results into one output

#### 🔧 Commands:

```bash id="8glwsl"
theHarvester -d example.com -b google
theHarvester -d example.com -b bing
theHarvester -d example.com -b linkedin
```

👉 Useful for reconnaissance phase

---

### 📧 Hunter

* Finds email addresses related to a domain

#### ⚙️ How It Works:

* Crawls websites and public sources
* Uses pattern recognition (e.g., [firstname@domain.com](mailto:firstname@domain.com))
* Verifies email validity

#### 🔧 Example:

* Visit: https://hunter.io
* Enter: `example.com`

---

### 🔍 Google Dorking

* Advanced Google search technique

#### ⚙️ How It Works:

* Uses special search operators
* Filters indexed web pages
* Finds publicly exposed sensitive data

#### 🔧 Examples:

```bash id="3rc03t"
site:example.com filetype:pdf
intitle:"index of" "backup"
inurl:login
```

👉 Uses search engine indexing to find data

---

### 🛠️ DorkFinder

* Automates Google dork searches

#### ⚙️ How It Works:

* Uses predefined dorks
* Runs multiple queries automatically
* Collects and displays results

#### 🔧 Usage:

* Enter target domain
* Select dork type
* Run scan

---

## 🛠️ Practical Understanding

* Learned how OSINT tools collect public data
* Understood how scanning and indexing work
* Practiced basic commands for reconnaissance
* Learned how attackers gather information

---

## 💡 Key Takeaways

* OSINT tools gather publicly available data
* Each tool uses different techniques (scanning, indexing, scraping)
* Commands are important for real-world usage
* Reconnaissance is the first step in hacking

---

