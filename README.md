# Hello, I'm John Kennedy 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/john-kennedy-70a224257/)



Aspiring IT and cybersecurity professional with a background in project management, a strong interest in technology, and a passion for solving complex problems. Experienced in managing projects from planning to execution and now transitioning into IT/cybersecurity with hands-on project work and in addition knowledge on GRC (Governance, Risk, and Compliance). Dedicated to continuous learning and bridging the gap between technical solutions and business objectives.

## Objective

Motivated and detail-oriented professional with a background in project management and a growing focus in IT and cybersecurity. Seeking an entry-level opportunity where I can apply my project coordination experience, passion for technology, and developing knowledge in GRC to support secure, efficient, and compliant business operations. Eager to contribute to a dynamic team while continuing to expand my technical and cybersecurity expertise.

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

git clone https://github.com/johnkennedy1025/elk-siem-portfolio.git

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
git clone https://github.com/johnkennedy1025/simple-python-honeypot.git
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





## Certifications
[Provide certifications that you have obtained. Use ChatGPT to help create the link - Remove this afterwards]]
<div>
<img src="https://img.shields.io/badge/-Security%2B-FF0000?&style=for-the-badge&logo=CompTIA&logoColor=white" />
<img src="https://img.shields.io/badge/-Network%2B-007ACC?&style=for-the-badge&logo=CompTIA&logoColor=white" />
<img src="https://img.shields.io/badge/-A%2B-4D4D4D?&style=for-the-badge&logo=CompTIA&logoColor=white" />
<img src="https://img.shields.io/badge/-CDSA-006400?&style=for-the-badge&logoColor=white" />
<img src="https://img.shields.io/badge/-CCD-000080?&style=for-the-badge&logoColor=white" />
</div>

## Projects
- Detection Lab
- SOC Automation Project
