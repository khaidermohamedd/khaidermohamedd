<a href="https://khaidermohamedd.github.io"><img width="100%" src="./assets/header.svg" alt="Mohamed Khaider — AI Engineer · Full-Stack & MLOps · Vision, Code, Data, Security" /></a>

<p align="center">
  <a href="https://khaidermohamedd.github.io"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=900&color=D6B97F&center=true&vCenter=true&width=780&lines=Real-time+computer+vision+for+industrial+safety;LLM+%2B+RAG+agents+%E2%80%94+with+a+human+in+the+loop;Federated+learning%3A+models+travel%2C+data+doesn't;Anomaly+detection+at+a+0.12%25+fraud+rate;Spring+Boot+%2B+Angular%2C+shipped+on+AWS" alt="Focus areas" /></a>
</p>

<p align="center">
  <a href="https://khaidermohamedd.github.io"><img src="https://img.shields.io/badge/Portfolio-khaidermohamedd.github.io-D6B97F?style=for-the-badge&logo=googlechrome&logoColor=black" alt="Portfolio"></a>
  <a href="mailto:mohamed.khaider7@gmail.com"><img src="https://img.shields.io/badge/Email-mohamed.khaider7@gmail.com-1A1A1A?style=for-the-badge&logo=gmail&logoColor=D6B97F" alt="Email"></a>
  <a href="https://www.linkedin.com/in/mohamed-khaider-aa3ab22a5/"><img src="https://img.shields.io/badge/LinkedIn-Mohamed%20Khaider-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <img src="https://img.shields.io/badge/Agadir-Morocco-2E7D32?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Agadir, Morocco">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/%F0%9F%8E%AF%20Seeking%20PFE%20internship-2027-D6B97F?style=flat-square&labelColor=1A1A1A" alt="Seeking a PFE internship in 2027">
  <br>
  <sub>AI Engineering · Computer Vision · Full-Stack (Spring Boot / Angular) · MLOps on AWS</sub>
</p>

---

## <img src="https://media.giphy.com/media/QssGEmpkyEOhBCb7e1/giphy.gif" width="26"> &nbsp;About

I build **AI systems end to end**: the model (computer vision, anomaly detection, LLM + RAG),
the **real-time data pipeline** behind it (Kafka, Spark Structured Streaming), and the **secure
full-stack application** that puts it in front of users (Java Spring Boot, Angular), containerised
and deployed on **AWS**.

I care about the parts that make a model usable in production: latency budgets, thresholds tuned on
business cost rather than accuracy, explainability for the people who act on alerts, and
**security built in from the start** (least-privilege IAM, encryption at rest, audit logs, image scanning).

`MSc Artificial Intelligence & Digital Computing · 2025–2027 · FST Béni Mellal, Université Sultan Moulay Slimane`

---

## <img src="https://media.giphy.com/media/iY8CRBdQXODJSCERIr/giphy.gif" width="26"> &nbsp;Flagship work

### 🛡️ SecureOps AI — Anomaly-detection copilot with an investigation agent

A secure full-stack platform that scores anomalies and lets an **AI agent prepare the investigation,
while a human makes every sensitive decision.**

| | |
|---|---|
| Scoring | **XGBoost** model ranks incoming alerts by risk |
| AI agent | **LLM + RAG** enriches each alert with a contextual summary and a recommended action |
| Guardrails | **No autonomous execution** — mandatory human approval on every sensitive step, immutable audit log |
| Backend | Java **Spring Boot** REST API — Spring Security, **JWT/OAuth2**, RBAC, rate limiting |
| Frontend | **Angular** console to visualise, triage and resolve alerts |
| Cloud | **AWS** ECS Fargate · RDS PostgreSQL · S3 (audit) · Secrets Manager — encryption at rest, least-privilege IAM, **Trivy**-scanned images |

`Spring Boot` `Angular` `XGBoost` `LLM/RAG` `Docker` `AWS` &nbsp;·&nbsp; <sub>🔒 private — demo on request</sub>

### 🦺 HSE Vision — Real-time safety monitoring · *Holcim internship*

Multi-camera system that detects **missing PPE** and **dangerous vehicle manoeuvres** on an industrial site.

- **YOLOv8** trained by transfer learning (**85% accuracy**), multi-object tracking with **ByteTrack**, OpenCV preprocessing
- Video inference pipeline running at **5 FPS** per camera
- **Event-driven, containerised architecture**: detections streamed through **Kafka**, per-camera statistics aggregated continuously with **Spark Structured Streaming**

`YOLOv8` `ByteTrack` `OpenCV` `Kafka` `Spark` `Docker` &nbsp;·&nbsp; <sub>🔒 internship work — not public</sub>

---

## <img src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="26"> &nbsp;Projects

<table>
<tr>
<td width="50%" valign="top">

#### 🌐 NIDS-FL — Federated intrusion detection

Network intrusion detection where **models travel, raw traffic never does.**

- **FedAvg** across 3 clients: **65 KB** of compressed weights per round instead of centralising **1.2 GB**
- **Hybrid Edge/Cloud**: local MLP **99.38%**, cloud XGBoost **99.44%** (7 classes)
- **Continual learning** with a replay buffer: **−2%** F1 over 8 weeks of drift vs **−16%** for a static model

`TensorFlow` `XGBoost` `FedAvg`

</td>
<td width="50%" valign="top">

#### 💳 Unsupervised fraud detection

VAE · Isolation Forest · LSTM-AE on unlabelled transactions at a **0.12% fraud rate**.

- Model selected on **AUC-PR**: VAE **0.1139** (≈ **95×** random, **+129%** vs Isolation Forest)
- Decision threshold calibrated on **business cost** → **−24%** operational cost
- **Streamlit** dashboard with per-transaction **SHAP** explanations

`TensorFlow` `scikit-learn` `SHAP` `Streamlit`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🔎 [ResearchWatch](https://github.com/khaidermohamedd/ResearchWatch)

Semantic search engine for scientific papers: arXiv corpus → cleaning and de-duplication →
**384-d sentence embeddings** indexed as `dense_vector` in **Elasticsearch 8**, explored in **Kibana**.

`Python` `Elasticsearch` `Sentence-Transformers` `Kibana` `Docker`

</td>
<td width="50%" valign="top">

#### 🧪 [PROJET.IA — Feature selection study](https://github.com/khaidermohamedd/PROJET.IA)

Filter (CFS, information gain), PCA and **wrapper** feature selection compared across KNN, SVM,
Naive Bayes, MLP and random forest classifiers, against a no-selection baseline.

`Python` `scikit-learn` `Jupyter`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### ⚙️ ETL pipeline & dynamic dashboard

Data preprocessing and visualisation chain orchestrated with **Apache NiFi**.

`Apache NiFi` `Python`

</td>
<td width="50%" valign="top">

#### ✨ [Portfolio](https://github.com/khaidermohamedd/khaidermohamedd.github.io)

My personal site — loader, liquid-distortion hero, stacked project cards. Hand-written HTML/CSS/JS.

`HTML` `CSS` `JavaScript`

</td>
</tr>
</table>

---

## <img src="https://media.giphy.com/media/LnQjpWaON8nhr21vNW/giphy.gif" width="26"> &nbsp;Experience

| | Role | Company |
|---|---|---|
| **Jul – Aug 2026** | AI & Computer Vision intern — real-time HSE monitoring | **Holcim** · Agadir |
| **2025 · 2 months** | Full-stack intern — industrial maintenance app (Spring Boot REST API + React) | **OCP Group** · Khouribga |

---

## <img src="https://media.giphy.com/media/WFZvB7VIXBgiz3oDXE/giphy.gif" width="26"> &nbsp;Tech

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java">
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch">
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow">
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV">
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot">
<img src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" alt="Angular">
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React">
<img src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka">
<img src="https://img.shields.io/badge/Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="Spark">
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS">
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white" alt="Elasticsearch">
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

| | |
|---|---|
| **AI & deep learning** | PyTorch · TensorFlow/Keras · scikit-learn · XGBoost · CNN (ResNet, U-Net) · RNN/LSTM · YOLOv5/v8 · OpenCV · federated learning (FedAvg) · FinBERT · LLM & RAG |
| **Full-stack** | Java (Spring Boot) · Angular · React · TypeScript · REST APIs · Spring Security (JWT/OAuth2) · HTML/CSS |
| **Cloud & MLOps** | AWS (ECS, EC2, RDS, S3, IAM, Secrets Manager) · Docker / Compose · Kafka · Spark Structured Streaming · CI/CD (GitHub Actions) |
| **Security** | RBAC · encryption at rest · rate limiting · least-privilege IAM · Trivy vulnerability scanning · audit logging |
| **Languages & data** | Python · Java · R · SQL · MongoDB · Neo4j |

---

<div align="center">

**MSc — Artificial Intelligence & Digital Computing** · FST Béni Mellal, USMS · 2025–2027
**BSc — Distributed Computer Systems** · FST Marrakech, Cadi Ayyad University · 2024–2025
**DEUST — Science & Technology** · FST Marrakech, Cadi Ayyad University · 2022–2024

![Arabic](https://img.shields.io/badge/Arabic-native-2E7D32?style=flat-square)
![French](https://img.shields.io/badge/French-professional-0055A4?style=flat-square)
![English](https://img.shields.io/badge/English-advanced-B22234?style=flat-square)

<br>

<a href="https://khaidermohamedd.github.io"><img width="100%" src="./assets/footer.svg" alt="Let's build something smart." /></a>

</div>
