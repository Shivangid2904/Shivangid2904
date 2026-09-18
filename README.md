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

I study Computer Science with an AI & Machine Learning specialization at SRM University AP.

For me, building software always starts with curiosity: *What if a navigation system understood when an area feels unsafe? Can we mathematically catch the quiet signs of a habitable planet in noisy telescope data? Why send confidential documents across the internet when a local model can reason about them on your own machine?*

My work naturally bridges two core areas: **machine intelligence** and **cloud architecture**. I care about designing systems that are grounded in solid mathematics, respectful of privacy, and resilient when deployed into production.

My technical interests gravitate around:
- 🧠 **Machine Intelligence:** Local-first RAG pipelines, dense vector retrieval, and model explainability
- ☁️ **Cloud Systems:** Event-driven serverless architectures, decoupled pipelines, and least-privilege security on AWS
- 🌌 **Scientific & Space Data:** Machine learning applied to astronomical catalogs and planetary telemetry
- 🔐 **Cybersecurity:** Automated vulnerability ingestion and threat intelligence
- 🌸 **Human-Centered Technology:** Designing intelligent prototypes that directly protect and assist people

---

### ✦ Things I've Been Curious Enough to Build

#### 🌸 [SafeHer AI](https://github.com/Shivangid2904/safeher-ai) `Active Prototype`
> *"What if a map could understand when a route feels unsafe — rather than just calculating the shortest distance?"*

A safety-aware geospatial navigation prototype designed to prioritize personal safety over pure transit speed. The system imports road networks from OpenStreetMap into PostgreSQL/PostGIS with GiST spatial indexing and builds a directed graph with NetworkX. It computes a segment-by-segment **SafeHer Risk Index (SRI 0–100)** incorporating street lighting, road hierarchy, and proximity buffers around Safe Havens (police stations, hospitals, pharmacies). A modified Dijkstra routing engine evaluates multi-objective paths (`fastest`, `balanced`, `safest`) while dynamically factoring in community incident reports with a 7-day exponential time-decay model.

`Python` · `PostGIS` · `NetworkX` · `OSMnx` · `Dijkstra Algorithm` · `Flask API` · `Streamlit`

[explore safeher-ai →](https://github.com/Shivangid2904/safeher-ai)

---

#### 🧠 [IntelliAsk — Intelligent Question Answering System](https://github.com/Shivangid2904/Intelligent-Question-Answering-System)
> *"Why send private documents to an external API when your own machine can search and reason over them?"*

A local-first, privacy-preserving Retrieval-Augmented Generation (RAG) platform. To ensure zero data leakage and avoid recurring API costs, IntelliAsk processes documents locally: chunking PDFs, generating dense vector embeddings via Sentence Transformers, and indexing them in FAISS. The pipeline pairs semantic vector search with keyword matching for hybrid relevance scoring, feeding the most relevant passages to on-device quantized LLMs via Ollama for grounded answer generation with supporting passage attribution and persistent session history.

`documents` → `Sentence Transformers` → `FAISS vector index` → `hybrid retrieval` → `local LLM (Ollama)` → `grounded answer`

`Python` · `FAISS` · `Sentence Transformers` · `Ollama (Local LLMs)` · `Streamlit` · `RAG Architecture`

[explore intelliask →](https://github.com/Shivangid2904/Intelligent-Question-Answering-System)

---

#### ☁️ [CVE Vulnerability Intelligence Platform](https://github.com/Shivangid2904/cve-vulnerability-intelligence-platform)
> *"When a critical vulnerability appears in the middle of the night, security teams shouldn't have to discover it manually."*

An event-driven serverless threat intelligence pipeline built entirely on AWS to eliminate idle compute overhead. The system ingests upstream CVE feeds into Amazon S3, triggering AWS Lambda to parse records and classify vulnerability severity (Critical / Medium / Low). State is persisted in DynamoDB, cross-referenced against client technology profiles, and fanned out through Amazon EventBridge and Amazon SNS for instant email and webhook alert dispatch under tight IAM boundaries.

`S3 (CVE Ingestion)` → `Lambda (Parsing & Severity)` → `DynamoDB` → `Lambda (Stack Matching)` → `SNS Alerting`

`AWS Lambda` · `DynamoDB` · `Amazon S3` · `EventBridge` · `Amazon SNS` · `AWS IAM` · `Python`

[explore cve-platform →](https://github.com/Shivangid2904/cve-vulnerability-intelligence-platform)

---

#### 🪐 [ExoLife — Exoplanet Habitability Assessment](https://github.com/Shivangid2904/ExoLife-Exoplanet-Habitability-Assessment)
> *"What if machine learning could help separate meaningful planetary signals from an extremely imbalanced astronomical dataset?"*

A scientific ML platform benchmarking habitability predictions across 3,757 exoplanets from the NASA Exoplanet Archive. Addressing an extreme 75.7:1 class imbalance (only 49 habitable vs 3,708 non-habitable candidates), the project develops both a baseline model and a **Physics-Informed Proxy Model**. The proxy model intentionally excludes direct rule-based labeling features (radius, equilibrium temperature, insolation flux) to avoid target leakage, forcing the model to learn underlying astrophysical relationships from indirect stellar and orbital parameters (`st_teff`, `st_mass`, `pl_orbper`, `pl_orbeccen`, `st_met`, `sy_dist`). Benchmarked across Random Forest and XGBoost with Stratified 5-Fold Cross-Validation, PR-AUC evaluation, and local SHAP waterfall explainability.

`Python` · `scikit-learn` · `XGBoost` · `SHAP Explainability` · `NASA Archive` · `pandas` · `Streamlit`

[explore exolife →](https://github.com/Shivangid2904/ExoLife-Exoplanet-Habitability-Assessment) &nbsp;·&nbsp; [live demo ↗](https://exolife-exoplanet-habitability.onrender.com/)

---

### 🛠️ Workbench

The tools and environments I reach for when turning curiosity into working code:

* **Machine Intelligence & Scientific Data**  
  `Python` · `scikit-learn` · `XGBoost` · `FAISS` · `Sentence Transformers` · `Ollama` · `SHAP` · `pandas` · `NumPy` · `Streamlit`

* **Cloud Infrastructure & Serverless**  
  `AWS Lambda` · `Amazon DynamoDB` · `Amazon S3` · `EventBridge` · `Amazon SNS` · `AWS IAM` *(AWS Certified Cloud Practitioner)*

* **Core Engineering & Systems**  
  `Java` · `JavaScript` · `PostgreSQL / PostGIS` · `MySQL` · `Git` · `Linux / Bash`

---

### 🌌 Things I'm Curious About

A few areas I'm currently exploring in my reading, experiments, and side research:

* **Advanced Retrieval & Synthesis:** Exploring hybrid dense/sparse search, contextual cross-encoder re-ranking, and GraphRAG to handle multi-hop reasoning over complex knowledge graphs.
* **Model Calibration & Interpretability:** Designing models that express genuine uncertainty rather than confident hallucinations, combining physics-informed priors with SHAP feature attributions.
* **Scientific Machine Learning:** Applying learning methods to space telemetry and astrophysics catalogs where signal-to-noise ratios are challenging and ground truth is rare.
* **Resilient Distributed Architectures:** Designing event-driven serverless architectures with well-bounded failure domains and zero unnecessary idle compute.

---

### 🌷 Past Leadership

* **Former Lead — Smart Tech Club**  
  Led technical initiatives and organized campus hackathons, technical workshops, and peer-learning programs across AI/ML, Cloud Computing, Cybersecurity, Big Data, and IoT.

---

### 📜 Certifications

* **AWS Certified Cloud Practitioner** — Amazon Web Services *(2026)*

---

<div align="center">

*always curious, always building.* 🌸

<br/>

<sub>Curious about any of these systems or want to discuss AI, cloud pipelines, or astrophysics?</sub><br/>
<sub><a href="https://www.linkedin.com/in/shivangi-dubey-1783511a6">LinkedIn</a> &nbsp;·&nbsp; <a href="mailto:shivangi.d2904@gmail.com">shivangi.d2904@gmail.com</a></sub>

</div>
