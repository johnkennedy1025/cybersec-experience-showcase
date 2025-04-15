# Hello, I'm John Kennedy 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/john-kennedy-70a224257/)



Aspiring IT and cybersecurity professional with a background in project management, a strong interest in technology, and a passion for solving complex problems. Experienced in managing projects from planning to execution and now transitioning into IT/cybersecurity with hands-on project work and in addition knowledge on GRC (Governance, Risk, and Compliance). Dedicated to continuous learning and bridging the gap between technical solutions and business objectives.

## Objective

Motivated and detail-oriented professional with a background in project management and a growing focus in IT and cybersecurity. Seeking an entry-level opportunity where I can apply my project coordination experience, passion for technology, and developing knowledge in GRC to support secure, efficient, and compliant business operations. Eager to contribute to a dynamic team while continuing to expand my technical and cybersecurity expertise.


## Skills

- Policy Development and Management
- Regulatory Compliance
- Stakeholder Management and Collaboration
- Security Frameworks and Controls
- SIEM Tools
- Jira, Zendesk, and Microsoft Products
- Risk Management
- SQL, Python, and Linux
- Problem-Solving and Critical Thinking
- Incident Response Planning
- Threats, Risk, and Vulnerabilities
- Project Management



## Projects
**Project #1**: 
# 🛡️ Lightweight SIEM with ELK Stack & Filebeat

This project is a lightweight Security Information and Event Management (SIEM) system using the ELK Stack (Elasticsearch, Logstash, Kibana) and Filebeat for log collection. It demonstrates centralized log ingestion, parsing, visualization, and analysis 


---


## 🚀 Features

- Collects and parses system logs

- Stores and indexes logs in Elasticsearch

- Visualizes log data in Kibana dashboards

- Uses Filebeat for lightweight log shipping

- Easily extendable for custom log sources and alerts


---


## 🧱 Tech Stack

| Component     | Purpose                         |

|---------------|----------------------------------|

| Elasticsearch | Log indexing and search engine  |

| Logstash      | Pipeline for parsing logs       |

| Kibana        | Visualization and dashboards    |

| Filebeat      | Log shipper                     |

| Docker Compose| Container orchestration         |


---


## 📦 Project Structure

```

elk-siem-portfolio/

├── docker-compose.yml

├── elk-stack/

│   ├── logstash/

│   │   └── pipeline/

│   │       └── logstash.conf

│   └── filebeat/

│       └── filebeat.yml

└── logs/

    └── (drop your test .log files here)

```


---


## ⚙️ Setup & Usage

### Prerequisites


- Docker & Docker Compose


### Run the Stack


```bash

git clone [REPO_URL]

cd elk-siem-portfolio

docker-compose up --build

```


### Access Services


- **Kibana**: [http://localhost:5601](http://localhost:5601)

- Create index pattern: `syslog-*`


---


## 🧪 Simulate Logs


```bash

echo "Apr 14 18:22:45 ubuntu sshd[1234]: Failed password for invalid user admin" >> logs/auth.log

```


---


## 📊 Customization Ideas

- 🔥 Add Suricata or Zeek for IDS alerts
- 🎯 Create alerts using ElastAlert or Kibana rules
- 📉 Build dashboards for SSH brute-force or failed login attempts
- 🪪 Collect logs from a Windows system using Winlogbeat

---


## 🧠 Learning Objectives

- Understand log pipelines with ELK

- Parse logs using Logstash grok filters

- Build dashboards for security event visibility

- Lay the foundation for advanced SIEM setups


---


## 📚 Credits

Built as part of an IT/Cybersecurity learning journey.  

Inspired by open-source ELK and Beats projects from [Elastic.co](https://www.elastic.co/).


---


## 🪪 License

MIT License
---


**Project #2**: 

🛡️**Python Honeypot**
--
A lightweight, easy-to-understand honeypot written in Python that simulates a fake service and logs unauthorized access attempts.

---


📌 **Features**
--
🎯 Fake Service Simulation – Responds to incoming connections on a custom port

📝 Connection Logging – Captures IP addresses, timestamps, and request data

🔀 Multi-threading – Handles multiple connections concurrently

🔒 Minimal Footprint – No third-party libraries required

---

🚀 **Getting Started**
--
1. Clone the Repository
bash
git clone [REPO_URL]
cd simple-python-honeypot
2. Run the Honeypot
Make sure you're using Python 3.x.

bash
python honeypot.py
3. View the Logs
Connection attempts and received data are logged in:
honeypot_log.txt

---


⚙️ **Configuration**
---
You can easily change the port or welcome message in honeypot.py:

python
PORT = 9999  # Change to any unused port
message = "Welcome to the fake service! This is a honeypot.\n"

---


📂 **Example Output**
---
pgsql
2025-04-14 15:23:45 - Connection from ('192.168.1.101', 23456)
2025-04-14 15:23:45 - Data received: GET /admin HTTP/1.1

---

🧠 **How It Works**
---
Listens for incoming TCP connections on a configurable port

Responds with a welcome message to simulate a service

Logs the IP, timestamp, and any received payload

Threads each connection to handle multiple attackers

---


🛠️ **Tech Used**
---
Python 3

socket (built-in)

threading (built-in)

logging (built-in)

No external dependencies!

---

📄 **License**
This project is licensed under the MIT License. See the LICENSE file for details.

---

 **Project #3**:
 
🧬**Malware Analysis Lab**
---
A hands-on malware analysis project exploring the behavior, indicators, and technical breakdown of malicious software in a controlled lab environment. This project highlights reverse engineering, dynamic/static analysis, and reporting skills used in real-world threat investigations.

---

📌 **Project Overview**

This project focuses on analyzing malware samples using both static and dynamic techniques. The goal is to extract Indicators of Compromise (IOCs), understand malware functionality, and document behavior.

---

🔍 **Skills Demonstrated**

Static and dynamic malware analysis

String and function analysis

Network and file behavior tracking

Reporting and IOC documentation

---


🧪 **Tools & Environment**

Tool	Purpose
PEStudio	Static analysis (PE headers, strings, imports)
x64dbg / Ghidra	Disassembly, debugging, reverse engineering
Any.Run / Cuckoo Sandbox	Dynamic behavior analysis
Wireshark	Network traffic inspection
Procmon	File/Registry/Process monitoring
VirusTotal	Multi-engine detection
⚠️ Note: All analysis was conducted in a safe, isolated virtual lab to prevent accidental infection or system damage.

---

🛠️ **Setup Instructions**

⚠️ Warning: Never run malware samples on your host machine. Always use a secure and isolated VM.

Create a virtual machine using VirtualBox or VMware

Install the tools listed above

(Optional) Disable external network access or simulate LAN with controlled DNS/sniffer

Place malware samples inside the VM

Begin analysis and record all findings in reports

---


🧬 **Sample Analysis**: MalwareName.exe

---

🔎 **Static Analysis**
---
MD5 Hash: d41d8cd98f00b204e9800998ecf8427e

File Type: PE32 executable

Packed: Yes (UPX packed)

Suspicious Strings:

CreateRemoteThread

WinExec

cmd.exe /c powershell

🧪 **Dynamic Analysis**
---
Creates Files:
C:\Users\Victim\AppData\Roaming\evil.exe

Network Behavior:

Connects to: http://maliciousdomain[.]com/api

Downloads secondary payload

Persistence Mechanism:
Registry Run Key

🚨** IOCs Extracted**
---
Type	Value
File Path	C:\Users\Victim\AppData\evil.exe
Domain	maliciousdomain[.]com
IP Address	185.123.45.67
Registry	HKCU\Software\Microsoft\Windows\CurrentVersion\Run\evil

---
📖 **Report Format** (Included)
Each malware report includes:

📦 Basic file information

🔍 Static analysis findings

🧪 Dynamic behavior results

🚨 Extracted IOCs

📌 MITRE ATT&CK mapping (if applicable)

📄 Optional PDF export for visual reports

🔐 **Ethics & Legal**
This repository is strictly for educational and research purposes. All malware samples were analyzed in a controlled, isolated environment. Do not distribute or misuse any malicious files.

---

📂 **Directory Structure**
---
bash
malware-analysis-lab/
├── reports/
│   ├── agentstealer_report.md
│   ├── dropper_report.md
│   └── invoice_macro_report.md
├── samples-overview.md
├── report-template.md
├── tools/
│   └── setup_notes.md
└── README.md

---

# 🧬 Malware Analysis Report – [Sample Name / Hash]

## 📦 Basic Information
- **File Name**:  
- **MD5**:  
- **SHA-256**:  
- **File Size**:  
- **Type**: (e.g., PE32, ELF, Script)
- **Packed**: (Yes/No - with packer name if detected)

---

## 🔎 Static Analysis

### 🧵 Strings of Interest
- Example: `CreateRemoteThread`
- Example: `cmd.exe /c powershell`
- Example: `http://maliciousdomain.com/payload`

### 📚 Imports / APIs
- `WinExec`
- `GetProcAddress`
- `InternetOpen`

### 🗂️ Sections Overview
| Section | Entropy | Suspicious? |
|--------|---------|-------------|
| .text  | 6.7     | No          |
| .rsrc  | 7.8     | **Yes**     |

---

## 🧪 Dynamic Analysis

### 📁 File Behavior
- Drops file to: `C:\Users\Victim\AppData\Roaming\evil.exe`
- Creates: `*.tmp`, `*.bat` scripts

### 🌐 Network Activity
- Domain Contacted: `maliciousdomain[.]com`
- IP Address: `185.123.45.67`
- Protocols: HTTP, DNS

### 🔄 Persistence Mechanism
- Adds run key:
  - `HKCU\Software\Microsoft\Windows\CurrentVersion\Run\EvilApp`

### 📊 Behavior Summary
- Exhibits RAT behavior (remote shell)
- Exfiltrates clipboard data
- Spawns `powershell.exe`

---

## ⚔️ MITRE ATT&CK Mapping

| Technique ID | Name                        | Description                     |
|--------------|-----------------------------|---------------------------------|
| T1059.001    | PowerShell                  | Executes commands via PS        |
| T1547.001    | Registry Run Keys / Startup | Establishes persistence         |
| T1041        | Exfiltration Over C2 Channel| Sends data over HTTP            |

---

## 🚨 Indicators of Compromise (IOCs)

| Type       | Value                                       |
|------------|---------------------------------------------|
| File Path  | `C:\Users\Victim\AppData\evil.exe`          |
| IP Address | `185.123.45.67`                             |
| Domain     | `maliciousdomain[.]com`                     |
| Registry   | `HKCU\...\Run\EvilApp`                      |

---

## 🧼 Recommendations
- Block listed IOCs at firewall/proxy level
- Use EDR to detect persistence keys
- Re-image infected systems
- Report C2 domains to abuse contacts

---

## 📁 Sample Source
- [ ] MalwareBazaar
- [ ] VirusShare
- [ ] Malpedia
- [ ] Other: _____________________

---

## 📄 Notes
- Analysis performed in isolated Windows 10 VM (no network)
- Tools used: Ghidra, Procmon, PEStudio, x64dbg

---

> **Disclaimer**: This report is for educational use only. Do not deploy malicious files in uncontrolled environments.

---

# 🧾 Malware Samples Overview

| Sample Name     | MD5                              | Behavior Summary                | Persistence | Network IOCs          | MITRE IDs       |
|------------------|-----------------------------------|----------------------------------|-------------|------------------------|------------------|
| AgentStealer.exe | `a1b2c3d4e5f6g7...`              | Keylogging, clipboard theft     | Yes         | `185.10.20.30`         | T1056, T1041     |
| dropper.exe      | `abcd1234ef5678...`              | Drops RAT, C2 beaconing         | No          | `malicious[.]site`     | T1105, T1059.003 |
| invoice.docm     | `e4f5g6h7i8j9k0...`              | Macro execution, powershell     | Yes         | None                   | T1059.001, T1566 |
| trojan.dll       | `1234abcd5678ef...`              | Injects into explorer.exe       | Yes         | `evil[.]cloud`         | T1055, T1547     |

> For detailed analysis of each sample, refer to `/reports/sample_name_report.md`.




📄 License
This project is licensed under the MIT License. All malware samples used are publicly available and sourced from platforms like VirusShare, MalwareBazaar, and Malpedia for educational use.

---


# 📋 Project #4: GRC Audit Simulation

A Governance, Risk, and Compliance (GRC) project that simulates an internal IT audit of a fictional company. The project demonstrates understanding of security frameworks, control assessments, risk evaluation, and compliance documentation.

---

## 📌 Project Overview

This simulated GRC audit project walks through the process of evaluating a fictional company's information systems against a known security framework (e.g., **NIST 800-53**, **ISO 27001**, or **CIS Controls**). The focus is on identifying risks, assessing the effectiveness of existing controls, and creating documentation that aligns with industry compliance standards.

---

## 🎯 Objectives

- Simulate a basic internal IT security audit  
- Map controls to a known cybersecurity framework  
- Identify control gaps and risk impact  
- Recommend mitigations and document findings in audit reports  

---

## 🛠️ Tools & Artifacts

| Tool / Template        | Purpose                                           |
|------------------------|---------------------------------------------------|
| **Risk Register**      | Track risks, likelihood, impact, and response     |
| **Control Matrix**     | Map implemented controls to compliance framework  |
| **Audit Report Template** | Document findings and recommendations           |
| **Checklist (Excel/PDF)** | Checklist to guide audit steps and evidence     |

---

## 🧪 Simulated Environment

**Company:** ACME Corp  
**Industry:** SaaS / Cloud-based Software Provider  
**Employees:** ~200  
**Audit Scope:**  
- Identity & Access Management (IAM)  
- Data Protection  
- Change Management  
- Logging & Monitoring  
- Endpoint Security  

---

## 🔍 Framework Mapping Example

**Mapped Framework:** NIST SP 800-53 (Moderate Baseline)

| Control ID | Control Name               | In Place? | Evidence Reviewed           | Gap Identified |
|------------|----------------------------|-----------|-----------------------------|----------------|
| AC-2       | Account Management         | ✅ Yes     | AD User Lifecycle Policy     | ❌ No MFA Policy |
| SI-4       | System Monitoring          | ✅ Partial | Syslog Configs, No SIEM      | ✅ Needs Improvement |
| CM-2       | Baseline Configuration     | ❌ No      | None available               | ✅ No standard image |

---

## 📄 Deliverables

- ✅ **Audit Checklist**  
- ✅ **Control Mapping Matrix**  
- ✅ **Risk Register**  
- ✅ **Audit Report**  
- ✅ **Remediation Plan (optional)**  

---

## 📖 Sample Report Structure

1. **Executive Summary**  
2. **Scope & Methodology**  
3. **Findings Summary Table**  
4. **Detailed Findings**  
5. **Framework Mapping**  
6. **Risk Ratings (High / Med / Low)**  
7. **Recommendations**  
8. **Appendices (Policies, Logs, Screenshots)**  

---

## 🧠 Skills Demonstrated

- Risk identification and impact analysis  
- Framework mapping (NIST/CIS/ISO)  
- Documentation and reporting  
- Audit methodology and evidence review  
- Communication of technical issues to non-technical audiences  

---

## 🔐 Ethics & Confidentiality

This project is a **fictional simulation** and does not include any real company data. It is intended solely for educational and portfolio purposes.
                
---

## 🛡️ Certifications

| Certification | Issuer           | Status        | Badge |
|---------------|------------------|---------------|-------|
| [**Google Cybersecurity Certificate**](https://www.credly.com/badges/bbb95843-3257-4243-ab7f-5ed6f20e821c/public_url) | Google / Coursera | ✅ Completed | [![Google Cybersecurity](https://images.credly.com/size/110x110/images/0d604ca9-2c11-490b-9eb3-4c7fa7b70363/image.png)](https://www.credly.com/badges/bbb95843-3257-4243-ab7f-5ed6f20e821c/public_url) |
| [**Cybersecurity, Risk, and Compliance (GRC) Mastery Certificate**](https://www.credly.com/badges/9d616b24-3a84-4ba2-b509-8a9595d395f2/public_url) | GRC Mastery | ✅ Completed | [![GRC Mastery](https://images.credly.com/size/110x110/images/4ab29340-7c1b-4ee2-b466-818b1c54cbd3/image.png)](https://www.credly.com/badges/9d616b24-3a84-4ba2-b509-8a9595d395f2/public_url) |
| **CompTIA Security+** | CompTIA | ⏳ In Progress | ![Security+](https://via.placeholder.com/80x80.png?text=Security%2B) |



## Projects
- Lighweight SIEM
- Python Honeypot
- Malware Analysis Lab
- GRC Audit
- SOC Analyst Simulation(TryHackMe)

## Trainings 
 - Mastercard Cybersecurity Virtual Experience Program
 -  AIG Shields Up: Cybersecurity Virtual Experience Program
