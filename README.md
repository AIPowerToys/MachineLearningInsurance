Copyright (2025): AIPowerToys

# Insurance ML Demos - 

## LinkedIn-Style Summary
Delivering a production-ready portfolio of seven insurance-focused machine learning notebooks that create synthetic data, perform rigorous EDA, and operationalize models across fraud, underwriting, climate, and customer analytics scenarios. Demonstrates end-to-end capability with MLOps readiness, interpretable insights, and stakeholder-facing storytelling tailored to regulated insurance environments.

## Project Overview
The **Insurance ML Demos** portfolio provides a full stack of analytics use cases commonly prioritized by insurance carriers. Each notebook is self-contained: it fabricates realistic synthetic data, saves the dataset under `data/`, explores risk drivers, trains a model, and visualizes performance insights executives and actuarial partners expect.

Key highlights:

- Seven specialized insurance scenarios spanning fraud detection, underwriting, customer retention, claims operations, text mining, vehicle damage, and climate risk.
- Automated synthetic data creation with domain-aligned feature engineering and reproducible seeds.
- Visual storytelling using Matplotlib, Seaborn, and Plotly-ready tidy outputs.
- Model interpretability with SHAP, feature importance diagnostics, and transparent evaluation metrics.
- CI-ready GitHub Actions workflow that executes every notebook to guarantee reproducibility.

## Project Structure
```text
insurance-ml-demos/
├── .github/workflows/test-notebooks.yml
├── data/
│   └── README.md
├── README.md
├── requirements.txt
├── 01_claims_fraud_detection.ipynb
├── 02_underwriting_risk_scoring.ipynb
├── 03_customer_churn_prediction.ipynb
├── 04_claims_severity_model.ipynb
├── 05_claim_text_mining.ipynb
├── 06_vehicle_damage_assessment.ipynb
└── 07_climate_risk_projection.ipynb
```

## Installation & Environment
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scriptsctivate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Launch notebooks with **JupyterLab** or **VS Code**. Each notebook persists its dataset to `data/` so results can be reviewed or version-controlled.

## Notebook Guide
| Notebook | Focus | Techniques | Output Dataset |
|----------|-------|------------|----------------|
| `01_claims_fraud_detection.ipynb` | Detect potentially fraudulent property claims | Probabilistic synthetic data, RandomForest, SHAP importance, ROC analysis | `data/claims_fraud.csv` |
| `02_underwriting_risk_scoring.ipynb` | Price risk via underwriting score regression | Gradient Boosting, cross-validation metrics, calibration plots | `data/underwriting_risk.csv` |
| `03_customer_churn_prediction.ipynb` | Retention modeling for personal lines customers | XGBoost classification, feature importance, pipeline-ready preprocessing | `data/customer_churn.csv` |
| `04_claims_severity_model.ipynb` | Estimate ultimate claim severity | XGBoost regression, SHAP explanations, residual diagnostics | `data/claim_severity.csv` |
| `05_claim_text_mining.ipynb` | Topic modeling on adjuster narratives | Faker-generated narratives, NLTK preprocessing, LDA topics, text classification | `data/claim_texts.csv` |
| `06_vehicle_damage_assessment.ipynb` | Predict major repair vs. fast-track outcome | LightGBM classification, cost-sensitivity simulation, feature importance | `data/vehicle_damage.csv` |
| `07_climate_risk_projection.ipynb` | Project climate-driven claims and cost exposures | Seasonal feature engineering, Gradient Boosting regression, forward projections | `data/climate_risk_projection.csv` |

## Launch Badges
Replace `AIPowerToys` after forking:

- [\![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<your-github-username>/insurance-ml-demos/HEAD?labpath=01_claims_fraud_detection.ipynb)
- [\![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<your-github-username>/insurance-ml-demos/blob/HEAD/01_claims_fraud_detection.ipynb)

## Skills Demonstrated
- **Synthetic data engineering** aligned to regulatory-grade insurance use cases
- **Supervised & unsupervised modeling** across classification, regression, and NLP topics
- **Model governance** with transparent metrics, interpretability artifacts, and artifact persistence
- **MLOps readiness** via reproducible requirements and notebook execution workflow
- **Stakeholder storytelling** through polished visuals and executive summaries

## Extension Ideas
1. Connect notebooks to a feature store or Snowflake/Spark warehouse layer.
2. Wrap models inside a FastAPI microservice for real-time scoring demos.
3. Add Monte Carlo reserve simulations using the severity model outputs.
4. Publish dashboards with Plotly Dash or Streamlit for business stakeholders.

## About This Portfolio
Crafted for recruiting conversations with insurance carriers and consulting partners. Showcases actuarial-aligned ML rigor, interpretable analytics, and production-friendly notebooks that can be extended into underwriting workbenches or claims automation pilots.
