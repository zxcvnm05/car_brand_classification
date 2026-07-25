# car_brand_classification
# Car Brand Classification Based on Customer and Vehicle Attributes

## 📌 Executive Summary
This project develops an end-to-end Machine Learning pipeline to infer vehicle brands from sales and configuration context (Engine, Body Style, Price, Color) without relying on text fields or model names. The solution addresses data quality issues in dealership management systems by preventing data leakage and enabling automated data backfilling.

## 🛠️ Tech Stack & Tools
- **Language:** Python
- **Libraries:** Scikit-learn, XGBoost, LightGBM, Pandas, NumPy
- **Optimization:** GridSearchCV with StratifiedKFold

## 📂 Project Structure
├── data/               # Vehicle sales context dataset (23,906 records)
├── notebooks/          # Jupyter Notebooks for EDA, feature engineering, and model training
├── outputs/            # Feature importance plots, confusion matrices, grid search logs
└── README.md           # Project documentation

## 🚀 Key Results & Findings
- **Model Performance:** Tuned XGBoost achieved **65.29% accuracy** across 30 classes (outperforming the 62.65% baseline and 20x better than random guessing).
- **Predictive Power:** Vehicle configuration attributes (Engine, Body Style, Price, Color) account for **84% of total predictive power**.
- **Data Leakage Control:** Successfully isolated brand features by explicitly excluding model names and text fields.

## 💼 Business Impact & Recommendations
- **Data Governance:** Automates the backfilling of missing historical brand data in CRM/ERP systems.
- **Fraud Prevention:** Serves as an anomaly detection mechanism to flag inconsistent vehicle listings.
