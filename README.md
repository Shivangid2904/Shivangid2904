<div align="center">

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fraunces&weight=500&size=26&duration=3800&pause=1200&color=F4A7BB&center=true&vCenter=true&width=650&lines=Shivangi+Dubey;ai+%26+machine+learning+%E2%80%A2+cloud+architecture;asking+questions+with+data+%26+code" alt="Shivangi Dubey" />

<p align="center">
  <sub>SRM University AP &nbsp;·&nbsp; AWS Certified Cloud Practitioner &nbsp;·&nbsp; AI & ML Specialization</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/shivangi-dubey-1783511a6">
    <img src="https://img.shields.io/badge/linkedin-F4A7BB?style=flat&logo=linkedin&logoColor=2D182B" alt="LinkedIn"/>
  </a>
  &nbsp;
  <a href="mailto:shivangi.d2904@gmail.com">
    <img src="https://img.shields.io/badge/email-D8B4E2?style=flat&logo=gmail&logoColor=2D182B" alt="Email"/>
  </a>
  &nbsp;
  <a href="https://drive.google.com/file/d/1lCXme23zL50PrehgWtcn2wvx_QKc_ObN/view?usp=sharing">
    <img src="https://img.shields.io/badge/r%C3%A9sum%C3%A9-FFB7D5?style=flat&logo=googledrive&logoColor=2D182B" alt="Resume"/>
  </a>
</p>

<br/>

</div>

---

### 🌸 About

I'm a Computer Science student at SRM University AP, specializing in AI & Machine Learning.

Most of what I build starts with a question I can't quite shake:
- *What if navigation understood when an area feels unsafe, rather than just calculating the fastest route?*
- *Can we find subtle signs of habitability in messy, imbalanced astronomical data?*
- *Why send confidential documents to external APIs when local models can search and reason over them on your own machine?*

I spend most of my time exploring the space between machine learning and cloud systems—building prototypes, learning where models break, and figuring out how to turn ideas into clean, functional software. I tend to gravitate toward projects that sit somewhere between useful, slightly unusual, and technically challenging.

---

### ✦ Things I've Been Curious Enough to Build

#### 🌸 [SafeHer AI](https://github.com/Shivangid2904/safeher-ai)
> *"What if a map could understand when a route feels unsafe — rather than just calculating the shortest distance?"*

A safety-aware navigation prototype exploring routing based on personal safety rather than pure travel time. The system imports road networks from OpenStreetMap into PostgreSQL/PostGIS, builds a spatial graph with NetworkX, and computes a segment-level SafeHer Risk Index (0–100). A modified Dijkstra algorithm then balances travel efficiency with safety to recommend lower-risk paths.

`Python` · `PostGIS` · `NetworkX` · `OSMnx` · `Dijkstra Algorithm` · `Flask API` · `Streamlit`

[explore safeher-ai →](https://github.com/Shivangid2904/safeher-ai)

---

#### 🧠 [IntelliAsk — Question Answering System](https://github.com/Shivangid2904/Intelligent-Question-Answering-System)
> *"Why send private documents to an external API when your own machine can search and reason over them?"*

A local-first, privacy-oriented Question Answering platform built on Retrieval-Augmented Generation (RAG). It chunks and embeds PDF documents with Sentence Transformers, indexes them locally in FAISS, and combines semantic similarity with keyword matching for hybrid retrieval. Relevant passages are then passed to an on-device quantized LLM through Ollama, generating grounded answers without sending any data over the network.

`documents` → `Sentence Transformers` → `FAISS vector index` → `hybrid retrieval` → `local LLM (Ollama)` → `answer`

`Python` · `FAISS` · `Sentence Transformers` · `Ollama (Local LLMs)` · `Streamlit` · `RAG`

[explore intelliask →](https://github.com/Shivangid2904/Intelligent-Question-Answering-System)

---

#### ☁️ [CVE Vulnerability Intelligence Platform](https://github.com/Shivangid2904/cve-vulnerability-intelligence-platform)
> *"When a critical vulnerability appears in the middle of the night, security teams shouldn't have to discover it manually."*

A serverless AWS pipeline that automates vulnerability tracking and alerting. Incoming CVE feeds land in S3 and trigger Lambda functions to parse records and classify severity (Critical / Medium / Low). Structured vulnerability data is stored in DynamoDB, cross-referenced against client technology stacks, and routed through EventBridge and SNS to dispatch instant email alerts under least-privilege IAM policies.

`S3 (CVE Ingestion)` → `Lambda (Parsing & Severity)` → `DynamoDB` → `Lambda (Stack Matching)` → `SNS Alerting`

`AWS Lambda` · `DynamoDB` · `S3` · `EventBridge` · `SNS` · `IAM` · `Python`

[explore cve-platform →](https://github.com/Shivangid2904/cve-vulnerability-intelligence-platform)

---

#### 🪐 [ExoLife — Exoplanet Habitability Assessment](https://github.com/Shivangid2904/ExoLife-Exoplanet-Habitability-Assessment)
> *"What if machine learning could help separate meaningful planetary signals from an extremely imbalanced astronomical dataset?"*

A scientific ML project evaluating habitability across 3,757 exoplanets from the NASA Exoplanet Archive. To address a severe 75.7:1 class imbalance and prevent target leakage, ExoLife pairs a baseline model with a **Physics-Informed Proxy Model** that learns true astrophysical relationships from indirect stellar and orbital indicators rather than direct labeling features. Benchmarked across Random Forest and XGBoost with Stratified 5-Fold Cross-Validation, PR-AUC, and local SHAP explainability.

`Python` · `scikit-learn` · `XGBoost` · `SHAP Explainability` · `NASA Archive` · `pandas` · `Streamlit`

[explore exolife →](https://github.com/Shivangid2904/ExoLife-Exoplanet-Habitability-Assessment) &nbsp;·&nbsp; [live demo ↗](https://exolife-exoplanet-habitability.onrender.com/)

---

### 🛠️ Workbench

The tools and environments I reach for when turning curiosity into working code:

* **Machine Intelligence & Scientific Data**  
  `Python` · `scikit-learn` · `XGBoost` · `FAISS` · `Sentence Transformers` · `Ollama` · `SHAP` · `pandas` · `NumPy` · `Streamlit`

* **Cloud Infrastructure & Serverless**  
  `AWS Lambda` · `DynamoDB` · `S3` · `EventBridge` · `SNS` · `IAM`

* **Core Engineering & Systems**  
  `Java` · `JavaScript` · `PostgreSQL/PostGIS` · `MySQL` · `Git` · `Linux/Bash`

---

### 🌌 Things I'm Curious About

A few topics I'm currently exploring through reading, side experiments, and prototypes:

* **Advanced Retrieval:** Experimenting with hybrid dense/sparse search, cross-encoder re-ranking, and GraphRAG to see how models handle multi-hop questions over structured knowledge.
* **Model Calibration & Explainability:** Exploring how to make ML models communicate uncertainty honestly rather than guessing, paired with SHAP to understand feature influence.
* **Scientific ML:** Reading about how statistical learning is applied to noisy space telemetry and planetary spectra where ground truth is rare.
* **Serverless Cloud Patterns:** Learning how to design clean event-driven architectures with well-defined boundaries and minimal idle overhead.

---

### 🌷 Past Leadership

* **Former Lead — Smart Tech Club**  
  Led technical initiatives and organized campus hackathons, hands-on workshops, and collaborative sessions across AI/ML, Cloud, and Cybersecurity.

---

<div align="center">

*always curious, always building.* 🌸

<br/>

<sub>Feel free to reach out to chat about AI, cloud systems, or exoplanets.</sub><br/>
<sub><a href="https://www.linkedin.com/in/shivangi-dubey-1783511a6">LinkedIn</a> &nbsp;·&nbsp; <a href="mailto:shivangi.d2904@gmail.com">shivangi.d2904@gmail.com</a></sub>

</div>
