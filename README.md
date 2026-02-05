<p align="center">
  <img src="assets/architecture.png" alt="SchemaSetu Architecture" width="700"/>
</p>

<h1 align="center">🌐 SchemaSetu</h1>

<p align="center">
  <b>The First AI That Calls the Farmer</b>
</p>

<p align="center">
  <em>A voice-first, multilingual AI platform to democratize access to government welfare schemes for 78 Million+ underserved citizens in India.</em>
</p>

<p align="center">
  <a href="#problem">Problem</a> •
  <a href="#solution">Solution</a> •
  <a href="#architecture">Architecture</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#docs">Documentation</a> •
  <a href="#team">Team</a>
</p>

---

| | |
|---|---|
| **Project Name** | SchemaSetu (सहायक सेतु) |
| **Hackathon** | AWS AI for Bharat Hackathon |
| **Organizer** | [Hack2Skill](https://hack2skill.com/) |
| **Team Name** | Vahini |
| **Team Lead** | Divyanshu Patel |

---

<h2 id="problem">🚨 The Problem</h2>

> **78 Million** eligible citizens miss out on **₹1.2 Trillion** in annual government benefits.

**Key Barriers:**
*   📢 **Language:** 70% of rural India speaks only local languages.
*   📱 **Digital Illiteracy:** 450M Indians cannot navigate digital interfaces.
*   📶 **Connectivity:** 400M users are on 2G networks.
*   ⏳ **Reactivity:** Existing solutions wait for users to ask; they don't proactively notify.

---

<h2 id="solution">💡 Our Solution</h2>

**SchemaSetu** is a **voice-first, proactive AI platform** that:

1.  **Calls Users Proactively:** When a user becomes eligible for a scheme, our AI initiates an IVR call to inform them in their own language.
2.  **Remembers Household Context:** Uses a Graph Database (Neo4j) to persist household information across conversations.
3.  **Works on 2G:** Optimized for low-bandwidth (<500KB per query) with IVR fallback.
4.  **Supports 22 Languages + 40 Dialects:** Powered by AI4Bharat for best-in-class Indic language support.

<p align="center"><b>"We don't just build an app. We build a bridge to government welfare for every Indian."</b></p>

---

<h2 id="architecture">🏗️ System Architecture</h2>

Our solution uses a robust, scalable 5-Layer AI System:

| Layer | Components | Purpose |
|---|---|---|
| **1. UI** | WhatsApp Bot, IVR, Web Portal, Mobile App | Multi-channel citizen access |
| **2. Gateway** | AWS API Gateway | Auth, Rate Limiting, Security |
| **3. AI Processing** | AI4Bharat ASR/TTS, AWS Bedrock LLM | Voice understanding & generation |
| **4. Intelligence** | ML Eligibility Engine, Neo4j Graph DB, Rules Engine | Smart matching & memory |
| **5. Integration** | UMANG APIs, PostgreSQL, AWS S3 | Data & Government services |

<p align="center">
  <img src="assets/process_flow_diagram.png" alt="Process Flow" width="700"/>
</p>

---

<h2 id="tech-stack">🛠️ Tech Stack</h2>

| Category | Technologies |
|---|---|
| **Voice & NLP** | AI4Bharat ASR/TTS, Whisper, Bhashini, AWS Bedrock |
| **ML & Intelligence** | Scikit-learn (92% accuracy), Neo4j, XGBoost |
| **Backend** | Node.js, FastAPI, PostgreSQL, Redis |
| **Infra & Cloud** | AWS Lambda, ECS, S3, CloudWatch |
| **Integration** | Twilio/Exotel (IVR), WhatsApp Business API, UMANG |

---

<h2 id="docs">📄 Documentation</h2>

Detailed technical specifications are available in the `/docs` folder:

*   📋 [**REQUIREMENTS.md**](docs/REQUIREMENTS.md) - Functional & Non-Functional Requirements
*   📐 [**DESIGN.md**](docs/DESIGN.md) - System Design Document

---

<h2>🌾 Use Case: Farmer Ramesh</h2>

<p align="center">
  <img src="assets/farmer_sceanrio.png" alt="Farmer Ramesh Use Case" width="700"/>
</p>

> Farmer Ramesh in Maharashtra receives a call from SchemaSetu in Marathi, informing him about the PM-KUSUM Solar Pump scheme. He confirms his eligibility via voice, sends a photo of his Aadhaar via WhatsApp, and the AI fills the form for him. **Total time: 8 minutes.**

---

<h2 id="team">👨‍💻 Team Vahini</h2>

| Role | Name |
|---|---|
| Team Lead | Divyanshu Patel |

---

<p align="center">
  <i>Built with ❤️ for Bharat</i>
</p>
