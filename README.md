<div align="center">

# ☁️ MeghRakshak

### Explainable AI for High-Impact Rainfall Prediction & Disaster Decision Support

> **See the storm. Understand the risk. Act before impact.**

[![SIH 2026](https://img.shields.io/badge/SIH-2026-FF6B35?style=for-the-badge)](https://sih.gov.in)
[![Problem Statement](https://img.shields.io/badge/PS-SIH1521-0A66C2?style=for-the-badge)](#-smart-india-hackathon-2026)
[![Organization](https://img.shields.io/badge/ISRO-Space%20Technology-1C7293?style=for-the-badge)](https://mosdac.gov.in)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev/)
[![XGBoost](https://img.shields.io/badge/XGBoost-ML-EA4335?style=flat-square)](https://xgboost.readthedocs.io/)
[![SHAP](https://img.shields.io/badge/SHAP-Explainable%20AI-8A2BE2?style=flat-square)](https://shap.readthedocs.io/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com/)

![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=flat-square)
![Contributions](https://img.shields.io/badge/Contributions-Team%20Only-lightgrey?style=flat-square)

</div>

---

## 📑 Table of Contents

- [About MeghRakshak](#-about-meghrakshak)
- [Problem Statement](#-problem-statement)
- [Our Solution](#-our-solution)
- [What Makes MeghRakshak Different](#-what-makes-meghrakshak-different)
- [System Architecture](#️-system-architecture)
- [Core Technology](#-core-technology)
- [Screenshots & Demo](#-screenshots--demo)
- [Quick Start](#-quick-start)
- [API Reference](#-api-reference)
- [Dashboard](#️-meghrakshak-dashboard)
- [Technology Stack](#️-technology-stack)
- [Expected Output](#-expected-output)
- [Target Users](#-target-users)
- [Potential Impact](#-potential-impact)
- [Evaluation Metrics](#-evaluation-metrics)
- [Research Foundation](#-research-foundation)
- [Responsible AI & Safety](#️-responsible-ai--safety)
- [Development Roadmap](#-development-roadmap)
- [Demonstration Strategy](#-demonstration-strategy)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [Team](#-team-meghrakshak)
- [License](#-license)

---

## 🌧️ About MeghRakshak

**MeghRakshak** is an explainable, satellite-driven early-warning and decision-support system designed to predict **high-impact rainfall events** and help disaster-management authorities understand *why* a particular event is predicted.

Modern AI weather models can generate highly accurate predictions, but their outputs can often be difficult to interpret. During high-stakes situations such as floods, cloudbursts, and extreme rainfall, decision-makers need more than a probability score.

They need to know:

> **What is happening? Why is it happening? How confident are we? And what should we do next?**

MeghRakshak addresses this gap by combining **Indian satellite observations, rainfall ground truth, machine learning, explainable AI, uncertainty estimation, and an operational decision-support layer** into one unified platform.

---

## 🎯 Problem Statement

Extreme rainfall events can rapidly transform into floods, landslides, infrastructure failures, transport disruptions, and loss of life.

India has access to extensive Earth-observation data through satellite missions such as **INSAT-3D and INSAT-3DR**, along with rainfall observations and meteorological information.

However, transforming this information into a system that is:

* timely,
* region-specific,
* explainable,
* uncertainty-aware,
* and directly actionable

remains a significant challenge.

### The core problem

Existing rainfall prediction systems may provide a forecast without sufficiently explaining the factors driving the prediction.

For disaster-response authorities, a prediction such as:

> **"82% probability of extreme rainfall."**

is less useful than:

> **"82% probability of extreme rainfall. The prediction is primarily driven by rapidly decreasing cloud-top temperature, strong moisture convergence, and persistent cloud development over the region."**

MeghRakshak aims to bridge this **prediction-to-decision gap**.

| Problem Statement ID | Title | Organization | Theme | Category |
|---|---|---|---|---|
| **SIH1521** | Development of Explainable AI (XAI) based model for prediction of heavy/high impact rain events using satellite data | ISRO | Space Technology | Software |

---

## 💡 Our Solution

MeghRakshak processes satellite and meteorological information to identify conditions associated with high-impact rainfall.

The system then:

1. Collects satellite and meteorological observations.
2. Extracts relevant atmospheric and cloud features.
3. Predicts the probability of high-impact rainfall.
4. Estimates prediction confidence and uncertainty.
5. Uses Explainable AI to identify the major factors influencing the prediction.
6. Converts the prediction into a regional risk level.
7. Generates decision-support recommendations.
8. Displays everything through an intuitive geospatial dashboard.

### In simple terms:

```text
Satellite & Meteorological Data
              ↓
       Data Processing
              ↓
      Feature Extraction
              ↓
       ML Prediction Model
              ↓
    Risk + Confidence Score
              ↓
       Explainable AI
              ↓
     Decision Support Engine
              ↓
     Actionable Alert Level
              ↓
     Interactive GIS Dashboard
```

---

## 🚨 What Makes MeghRakshak Different?

MeghRakshak is not designed to be just another rainfall prediction model.

Our approach focuses on the complete chain:

> **Prediction → Explanation → Confidence → Decision → Action**

### 1. 🇮🇳 India-focused satellite intelligence

MeghRakshak is designed around Indian Earth-observation data, particularly **INSAT-3D/3DR**, rather than treating India's monsoon environment as just another region in a global model. Large global AI weather models are trained on global reanalysis data and have shown systematic underestimation of extreme precipitation over the South Asian monsoon region — a gap an India-native model is built to close.

### 2. 🔍 Explainable predictions

Using **SHAP-based explainability**, the system identifies the features that contributed most strongly to a prediction.

Instead of:

> "Extreme rainfall predicted."

the system can communicate:

> "Extreme rainfall risk is elevated primarily due to cloud-top cooling, moisture convergence, and atmospheric pressure conditions."

### 3. 📊 Confidence-aware predictions

Every prediction should communicate not only **what the model predicts**, but also **how confident the model is**. This helps avoid overconfident automated warnings.

### 4. 🧠 Decision-support layer

MeghRakshak goes beyond prediction. It translates model outputs into operational risk categories and potential preparedness actions.

```text
LOW RISK            → Normal monitoring
MODERATE RISK        → Increase monitoring and verify local conditions
HIGH RISK             → Prepare emergency resources and issue targeted warnings
CRITICAL RISK          → Activate emergency preparedness and evacuation-readiness protocols
```

The final decisions remain with authorized disaster-management personnel.

### 5. 🗺️ Geospatial visualization

The dashboard provides a map-centric view of rainfall risk, affected regions, prediction confidence, contributing factors, historical observations, alerts, and recommended preparedness level.

### How we compare

| Capability | Global AI models (e.g. GraphCast) | IMD Nowcast / Mausam | **MeghRakshak** |
|---|:---:|:---:|:---:|
| India-native satellite training | ❌ | ✅ | ✅ |
| Explainable per-prediction reasoning | ❌ | ❌ | ✅ |
| Confidence/uncertainty reporting | Partial | Partial | ✅ |
| Actionable decision-support tiers | ❌ | ❌ | ✅ |
| Open, extensible architecture | ❌ | ❌ | ✅ |

---

## 🏗️ System Architecture

```text
                     ┌───────────────────────┐
                     │  INSAT-3D / INSAT-3DR │
                     │    Satellite Data     │
                     └───────────┬───────────┘
                                 │
                     ┌───────────▼───────────┐
                     │    Data Ingestion     │
                     │ & Preprocessing Layer │
                     └───────────┬───────────┘
                                 │
                     ┌───────────▼───────────┐
                     │   Feature Extraction  │
                     │ Cloud / IR / Moisture │
                     │ Atmospheric Features  │
                     └───────────┬───────────┘
                                 │
              ┌──────────────────▼──────────────────┐
              │          Prediction Engine          │
              │      XGBoost / Random Forest /      │
              │           Temporal Models           │
              └──────────────────┬──────────────────┘
                                 │
                 ┌───────────────┴────────────────┐
                 │                                 │
       ┌─────────▼─────────┐             ┌─────────▼────────┐
       │   Risk Prediction │             │   Confidence /   │
       │                   │             │   Uncertainty    │
       └─────────┬─────────┘             └─────────┬────────┘
                 │                                  │
                 └───────────────┬──────────────────┘
                                 │
                     ┌───────────▼───────────┐
                     │       XAI Layer       │
                     │     SHAP / Feature    │
                     │      Attribution      │
                     └───────────┬───────────┘
                                 │
                     ┌───────────▼───────────┐
                     │  Decision Support &   │
                     │  Risk Classification  │
                     └───────────┬───────────┘
                                 │
                     ┌───────────▼───────────┐
                     │      FastAPI API      │
                     └───────────┬───────────┘
                                 │
                     ┌───────────▼───────────┐
                     │    MeghRakshak Web    │
                     │     GIS Dashboard     │
                     └────────────────────────┘
```

---

## 🧠 Core Technology

### Data Layer

Potential data sources include:

* INSAT-3D / INSAT-3DR
* MOSDAC
* IMD rainfall observations
* Meteorological observations
* Historical rainfall datasets
* Terrain / geospatial datasets
* Relevant open government datasets

### Machine Learning

The initial model pipeline evaluates classical and temporal approaches.

**Baseline models:** Random Forest · XGBoost
**Advanced models:** LSTM · ConvLSTM · Temporal deep-learning architectures

The final model is selected based on measurable validation performance rather than complexity alone.

### Explainable AI — SHAP

SHAP identifies the contribution of individual features to model predictions, turning a black-box probability into an interpretable result:

```text
High-Impact Rainfall Risk: 87%

Major contributing factors:

Cloud-top temperature       ████████████████
Moisture convergence        █████████████
Pressure gradient           █████████
Recent rainfall             ██████
Cloud persistence           █████
```

---

## 📸 Screenshots & Demo

> _Add dashboard screenshots, architecture diagrams, and a short demo GIF/video link here once the prototype is ready._

| Risk Map View | Explainability Panel | Alert Center |
|---|---|---|
| _screenshot placeholder_ | _screenshot placeholder_ | _screenshot placeholder_ |

**Demo video:** _[link once recorded]_

---

## 🚀 Quick Start

### Prerequisites

* Python 3.10+
* Node.js 18+
* npm or yarn
* Docker & Docker Compose (optional, for containerized setup)
* MOSDAC account (for INSAT-3D/3DR data access — [register here](https://mosdac.gov.in))

### 1. Clone the repository

```bash
git clone https://github.com/<your-org>/MeghRakshak.git
cd MeghRakshak
```

### 2. Backend setup (FastAPI + ML)

```bash
cd backend
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

### 3. Frontend setup (Next.js)

```bash
cd frontend
npm install
npm run dev
```

The dashboard will be available at `http://localhost:3000`, with the API served at `http://localhost:8000`.

### 4. Run with Docker (alternative)

```bash
docker-compose up --build
```

### 5. Environment variables

Create a `.env` file in `backend/` based on `.env.example`:

```env
MOSDAC_API_KEY=your_mosdac_key
IMD_DATA_PATH=./data/raw/imd
MODEL_PATH=./ml/models/latest.pkl
CORS_ORIGINS=http://localhost:3000
```

---

## 📡 API Reference

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/health` | Service health check |
| `POST` | `/predict` | Returns rainfall risk prediction + confidence for a given region/time window |
| `POST` | `/explain` | Returns SHAP feature attribution for a given prediction |
| `GET` | `/regions` | Lists available monitored regions |
| `GET` | `/alerts` | Returns currently active high-risk alerts |

**Example request:**

```bash
curl -X POST http://localhost:8000/predict \
  -H "Content-Type: application/json" \
  -d '{"region": "Assam", "timestamp": "2026-08-10T06:00:00Z"}'
```

**Example response:**

```json
{
  "region": "Assam",
  "risk_level": "HIGH",
  "rainfall_probability": 0.87,
  "confidence": 0.91,
  "prediction_horizon": "0-6 hours",
  "key_drivers": [
    "Cloud-top temperature decrease",
    "Moisture convergence",
    "Pressure gradient"
  ],
  "recommended_action": "High-alert preparedness"
}
```

> Full interactive API docs are auto-generated by FastAPI at `http://localhost:8000/docs` once the backend is running.

---

## 🗺️ MeghRakshak Dashboard

The web application provides an operational map-based interface.

| Component | Description |
|---|---|
| 🌧️ **Rainfall Risk Map** | Region-wise rainfall risk, color-coded by severity |
| 📍 **Location Intelligence** | Select a district/region to inspect current predictions |
| 📈 **Prediction Panel** | Predicted risk, probability, severity, horizon, confidence |
| 🔍 **Explainability Panel** | Top contributing features, SHAP values, human-readable explanation |
| 🚨 **Alert Center** | Active high-risk regions |
| 🧭 **Decision Support** | Preparedness recommendations based on severity, confidence, and historical context |

---

## ⚙️ Technology Stack

<table>
<tr>
<td valign="top" width="25%">

**AI / ML**
- Python
- XGBoost
- Scikit-learn
- TensorFlow / PyTorch
- SHAP
- Pandas · NumPy

</td>
<td valign="top" width="25%">

**Backend**
- FastAPI
- Python
- REST APIs

</td>
<td valign="top" width="25%">

**Frontend**
- Next.js · React
- JavaScript / TypeScript
- Leaflet
- GIS visualization

</td>
<td valign="top" width="25%">

**Data & DevOps**
- INSAT-3D/3DR · MOSDAC
- IMD datasets · GeoJSON
- Git · GitHub
- Docker · VS Code

</td>
</tr>
</table>

---

## 📊 Expected Output

For each monitored region, MeghRakshak produces a structured prediction:

```json
{
  "region": "Example District",
  "risk_level": "HIGH",
  "rainfall_probability": 0.87,
  "confidence": 0.91,
  "prediction_horizon": "0-6 hours",
  "key_drivers": [
    "Cloud-top temperature decrease",
    "Moisture convergence",
    "Pressure gradient"
  ],
  "recommended_action": "High-alert preparedness"
}
```

---

## 🎯 Target Users

| User | Benefit |
|---|---|
| 🏛️ **State Disaster Management Authorities** | Support preparedness and resource allocation decisions |
| 🚨 **NDRF / SDRF** | Support emergency resource pre-positioning and response planning |
| 🌦️ **IMD & Meteorological Experts** | Provide an interpretable AI-based second opinion |
| 🏘️ **Local Administration** | Support district-level risk monitoring |
| 🌾 **Agricultural Communities** | Provide earlier awareness of potentially damaging rainfall |
| ✈️ **Infrastructure & Transport Operators** | Support preparedness and operational decisions during extreme rainfall |

---

## 🌍 Potential Impact

MeghRakshak is designed around a simple principle:

> **Every minute of additional warning can matter during a high-impact weather event.**

Potential impact areas include earlier disaster preparedness, improved emergency resource positioning, faster risk assessment, better interpretation of AI predictions, reduced uncertainty in decision-making, improved regional monitoring, and stronger integration between satellite intelligence and disaster response.

The system will ultimately be evaluated using measurable forecasting and operational metrics rather than relying solely on visual demonstrations.

---

## 📏 Evaluation Metrics

**Prediction metrics:** Precision · Recall · F1 Score · ROC-AUC · PR-AUC · False Alarm Rate · Critical Success Index · Brier Score

**Operational metrics:** Warning lead time · Spatial accuracy · Regional false-positive rate · Confidence calibration · Alert usefulness · Decision-support response time

---

## 🔬 Research Foundation

MeghRakshak builds upon research and publicly available resources in Explainable AI for Earth Observation, satellite-based rainfall prediction, short-term precipitation forecasting, AI weather forecasting, South Asian monsoon modelling, and disaster early-warning systems.

### References

1. *Development of XAI-Based Model for Prediction of Heavy Impact Rain Using Satellite Data* — IJITRS, 2025
2. *Explainable AI for Earth Observation: Current Methods, Open Challenges, and Opportunities* — arXiv:2311.04491
3. *Deep Learning for Short-Term Precipitation Prediction in Four Major Indian Cities: A ConvLSTM Approach with Explainable AI* — arXiv:2511.11152
4. Ravuri et al. — *Skilful precipitation nowcasting using deep generative models of radar*, Nature, 2021
5. *MAUSAM: An Observations-focused Assessment of Global AI Weather Prediction Models During the South Asian Monsoon* — arXiv:2509.01879
6. MOSDAC — ISRO Earth Observation Data Platform
7. IMD — Nowcast Warning System
8. Mission Mausam

---

## 🛡️ Responsible AI & Safety

MeghRakshak is intended as a **decision-support system**, not an autonomous authority. The system should never independently determine that a population must evacuate.

Instead, it provides:

```text
Prediction + Confidence + Explanation + Risk Assessment + Recommended Preparedness Level
```

Final decisions remain with authorized disaster-management officials. This approach is particularly important because false positives and false negatives have different consequences during disaster response.

---

## 🚀 Development Roadmap

<details>
<summary><b>Phase 1 — Research & Data</b></summary>

- [ ] Study high-impact rainfall events
- [ ] Identify available satellite datasets
- [ ] Obtain and preprocess historical observations
- [ ] Define prediction targets
- [ ] Establish evaluation methodology
</details>

<details>
<summary><b>Phase 2 — Baseline ML</b></summary>

- [ ] Build preprocessing pipeline
- [ ] Train Random Forest baseline
- [ ] Train XGBoost baseline
- [ ] Establish benchmark metrics
- [ ] Perform validation
</details>

<details>
<summary><b>Phase 3 — Explainability</b></summary>

- [ ] Integrate SHAP
- [ ] Generate feature attribution
- [ ] Develop human-readable explanations
- [ ] Validate explanation consistency
</details>

<details>
<summary><b>Phase 4 — Decision Support</b></summary>

- [ ] Develop risk classification
- [ ] Develop confidence scoring
- [ ] Design preparedness tiers
- [ ] Generate recommendation logic
</details>

<details>
<summary><b>Phase 5 — Dashboard</b></summary>

- [ ] Build GIS interface
- [ ] Integrate backend APIs
- [ ] Display regional risk
- [ ] Display prediction confidence
- [ ] Display explanations
- [ ] Build alert center
</details>

<details>
<summary><b>Phase 6 — Advanced Model</b></summary>

- [ ] Evaluate temporal modelling
- [ ] Explore LSTM / ConvLSTM
- [ ] Compare against baseline
- [ ] Perform ablation studies
</details>

<details>
<summary><b>Phase 7 — Deployment & Validation</b></summary>

- [ ] Containerize services
- [ ] Test end-to-end pipeline
- [ ] Evaluate latency
- [ ] Evaluate robustness
- [ ] Demonstrate historical event replay
- [ ] Prepare SIH presentation and prototype
</details>

---

## 🧪 Demonstration Strategy

For the prototype, MeghRakshak demonstrates a historical high-impact rainfall scenario:

```text
Historical Satellite Observation
            ↓
      Model Prediction
            ↓
      Risk Probability
            ↓
      Confidence Score
            ↓
      Why? → SHAP Explanation
            ↓
      What next? → Decision Support
            ↓
      Map + Alert Dashboard
```

This allows judges to see the complete **data-to-decision pipeline** rather than only a machine-learning model.

---

## 📁 Project Structure

```text
MeghRakshak/
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── maps/
│   └── dashboard/
│
├── backend/
│   ├── api/
│   ├── models/
│   ├── services/
│   └── main.py
│
├── ml/
│   ├── preprocessing/
│   ├── feature_engineering/
│   ├── training/
│   ├── evaluation/
│   └── explainability/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── notebooks/
├── docs/
├── tests/
├── docker/
│
├── .env.example
├── .gitignore
├── docker-compose.yml
├── requirements.txt
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

---

## 🤝 Contributing

MeghRakshak is currently developed by Team MeghRakshak for Smart India Hackathon 2026.

For internal team members:

1. Create a feature branch: `git checkout -b feature/your-feature-name`
2. Commit with clear messages: `git commit -m "feat: add SHAP explanation panel"`
3. Push and open a Pull Request against `main`
4. Request review from at least one other team member before merging

**Commit convention:** `feat:` new feature · `fix:` bug fix · `docs:` documentation · `refactor:` code change with no behavior change · `test:` adding tests

Future collaboration and research contributions may be opened up as the project evolves.

---

## 🔐 Data & Privacy

The project prioritizes publicly available, research-appropriate datasets and follows the usage requirements of respective data providers. No personally identifiable information is required for the core rainfall prediction pipeline.

---

## 🌱 Future Scope

Flood forecasting · Landslide-risk prediction · Cyclone impact assessment · Flash-flood risk estimation · Multi-satellite data fusion · Radar + satellite fusion · Soil moisture integration · River-level forecasting · Urban flood modelling · Hyperlocal alert generation · Multilingual public alerts · CAP-compatible alert generation · Integration with disaster-management APIs · Advanced spatiotemporal deep learning

---

## 👩‍💻 Team MeghRakshak

| Member | Role | GitHub |
|---|---|---|
| **Aditi Rajput** | Team Lead · AI/ML · Product & System Architecture | [@Aditi-963](https://github.com/Aditi-963) |
| **Addya Mishra** | AI/ML · Data Processing | _add handle_ |
| **Vaidehi Wate** | Frontend · UI/UX · GIS Visualization | _add handle_ |
| **Rahul Kumar** | Backend · API Development · Integration | _add handle_ |
| **Pranjal Gupta** | AI/ML · Cloud & Deployment | _add handle_ |
| **Hiranya Raut** | Research · Data Analysis · Documentation | _add handle_ |

> Roles are intentionally collaborative. All team members contribute to research, development, testing, and the final MeghRakshak prototype.

### 👩‍🏫 Faculty Guide

**Dr. Ankita Gandhi** — Industry Embedded Program (CSE-IEP), Parul Institute of Engineering & Technology, Parul University

### 🏫 Institution

**Parul Institute of Engineering & Technology (PIET)**, Limda, Waghodia, Vadodara, Gujarat, India
**Program:** B.Tech Computer Science Engineering — Industry Embedded Program (CSE-IEP)

---

## 🏆 Smart India Hackathon 2026

| | |
|---|---|
| **Edition** | Software Edition |
| **Problem Statement** | SIH1521 |
| **Organization** | Indian Space Research Organisation (ISRO) |
| **Theme** | Space Technology |
| **Category** | Software |

---

## 📜 License

This project is intended for academic, research, and innovation purposes as part of Smart India Hackathon 2026, licensed under the [MIT License](LICENSE). The final licensing model will be determined based on project requirements, data licensing conditions, and institutional guidelines.

---

<div align="center">

## ☁️ MeghRakshak

> **See the storm. Understand the risk. Act before impact.**

**Built with technology, data, and a mission to make extreme-weather intelligence more explainable and actionable.**

### Team MeghRakshak
**Parul Institute of Engineering & Technology · Parul University**
**Smart India Hackathon 2026 · ISRO · Space Technology**

⭐ **Star this repo if you find it useful!** ⭐

</div>
