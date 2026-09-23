<p align="center">
  <img src="./assets/banner.svg" alt="Manvendra Pratap: student, developer, cybersecurity enthusiast, problem solver" width="100%"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=900&color=00E5A0&center=true&vCenter=true&width=820&lines=I+build+defensive+security+tooling;Honeypot+logs+%E2%86%92+ML+%E2%86%92+attacker+archetypes;Local+LLMs+for+red-team+%2F+blue-team+automation;Currently%3A+occupancy+heatmaps+from+WiFi+CSI" alt="Typing intro"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/manvendra-pratap-834995299/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:pratapmanvendra0209@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://img.shields.io/badge/Dehradun,_India-0d1117?style=for-the-badge&logo=googlemaps&logoColor=00E5A0" alt="Location"/>
  <img src="https://img.shields.io/badge/Open_to-Security_Internships-00E5A0?style=for-the-badge&logoColor=black" alt="Open to security internships"/>
</p>

---

## 🛡️ About me

```yaml
# ~/whoami.yml
name:        Manvendra Pratap
studying:    B.Tech CSE (Cyber Security & Forensics) @ UPES Dehradun
internship:  IBM Summer Internship Programme — lead developer & ML engineer on CDHAS
focus:
  - detection engineering with unsupervised ML
  - attacker-behaviour analytics from honeypot telemetry
  - local LLMs (Ollama) as red-team / blue-team agents
now_building: WiFi CSI → people-presence heatmaps (major project)
preparing:    CompTIA Security+
approach:     "Collect real attack data → model it → make it readable for humans"
```

---

## 🚀 Featured projects

### 🍯 CDHAS — Cyber Deception & Honeypot Analytics System

**Turns raw honeypot traffic into attacker profiles a SOC analyst can read.** *(IBM SIP project)*

A Cowrie SSH/Telnet honeypot feeds a streaming ingestion pipeline. CDHAS answers three questions: *who* is attacking, *what* is unusual, and *what* they are trying to do.

- 📥 **~1.8M attack records** in MongoDB, fed by a watchdog log tailer with geo-IP enrichment
- 🧠 **Isolation Forest + KMeans written from scratch in pure Python** over a 6-feature session vector: anomaly scores with no labelled data, plus attacker archetypes (recon bot, credential harvester, manual prober, malware deployer)
- 🎯 Executed commands mapped to **MITRE ATT&CK** techniques (e.g. `wget`/`curl` → T1105)
- 📊 React dashboard with a live WebSocket feed: world map, session timeline, full command transcripts, alerts

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Cowrie-honeypot-ff5f6d?style=flat-square"/>
  <img src="https://img.shields.io/badge/MITRE-ATT%26CK-C8102E?style=flat-square"/>
</p>

**[→ View repo](https://github.com/Manvendra-Pratap/cdhas)**

---

### 📡 IoTGuard — IoT Guardian

**An IoT network scanner that explains risk to people who aren't security engineers.**

Scans the local network, flags anomalous devices, then runs a two-model AI debate: one local LLM plays attacker, the other plays defender.

- 🔍 Nmap discovery of hosts, ports, services and OS fingerprints across the local CIDR
- 🧠 Isolation Forest scoring each device on a 9-feature vector (Telnet/SSH exposure, OS risk, port entropy…)
- 🤖 **Dual-LLM red-team / blue-team reports**, 100% offline: models run sequentially and unload after use, so it fits on a **4 GB VRAM** laptop GPU
- 🚦 Traffic-light risk view with plain-language fixes for non-technical users

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white"/>
  <img src="https://img.shields.io/badge/nmap-4682B4?style=flat-square"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white"/>
</p>

**[→ View repo](https://github.com/Manvendra-Pratap/IoTGuard)**

---

### 🔐 Zero-Trust Access Framework

**"Never trust, always verify", implemented as an API.**

Every request gets an explainable risk score out of 100, and a policy engine turns it into one of five decisions: allow, allow + monitor, step-up MFA, read-only, or deny.

- ⚖️ Weighted scoring across **identity 35% · device 30% · behaviour 20% · context 15%**, with a reason logged for every point added
- 🔑 JWT + bcrypt auth, lockout after 5 failures, anti-enumeration responses, device-posture checks
- 🧪 Built-in simulator replays scenarios from "trusted employee" to "compromised account"; **54 unit tests**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white"/>
  <img src="https://img.shields.io/badge/tests-54_passing-2ea44f?style=flat-square"/>
</p>

**[→ View repo](https://github.com/Manvendra-Pratap/ZERO-TRUST-PROJECT)**

---

### 💊 MediSage *(hackathon team project)*

**Reads handwritten prescriptions and turns them into structured, searchable text.**

OCR + NLP pipeline built in a 4-person hackathon team.

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white"/>
</p>

**[→ View repo](https://github.com/Manvendra-Pratap/MediSage)**

---

## 🧰 Toolbox

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,react,js,ts,mongodb,docker,linux,bash,git,sklearn&perline=11" alt="Tech stack"/>
</p>

<p align="center">

`Cowrie` • `nmap` • `MITRE ATT&CK` • `Log parsing & enrichment` • `Zero-trust access control` • `Isolation Forest` • `KMeans` • `Ollama` • `LangGraph` • `CrewAI`

</p>

---

## 🔭 Currently exploring

```text
Detection engineering
    ├── Unsupervised anomaly detection on security telemetry
    ├── Attacker behaviour clustering
    └── Evaluating models with no labelled ground truth

AI × Security
    ├── Local-LLM agents for red/blue-team simulation
    ├── Plain-language explanations of findings
    └── Running agent pipelines on a 4 GB VRAM GPU

RF sensing
    ├── WiFi Channel State Information (CSI)
    └── Presence heatmaps → 3D room occupancy
```

---

## 🐍 Contribution graph

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Manvendra-Pratap/Manvendra-Pratap/output/github-snake-dark.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Manvendra-Pratap/Manvendra-Pratap/output/github-snake.svg"/>
    <img alt="Snake eating my contribution graph" src="https://raw.githubusercontent.com/Manvendra-Pratap/Manvendra-Pratap/output/github-snake-dark.svg" width="100%"/>
  </picture>
</p>

---

<p align="center">
  <b>🛡️ Collect the attack. Model the attacker. Explain it to a human.</b><br/>
  <i>Open to security internships and blue-team / detection collaborations. Say hi on <a href="https://www.linkedin.com/in/manvendra-pratap-834995299/">LinkedIn</a> or <a href="mailto:pratapmanvendra0209@gmail.com">email</a>.</i>
</p>
