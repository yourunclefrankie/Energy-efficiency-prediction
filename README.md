# Energy-efficiency-prediction
This project explores the use of machine learning to predict the energy efficiency rating of residential buildings in the UK. Using Energy Performance Certificate (EPC) data, the goal is to identify the most important features influencing efficiency while reducing reliance on redundant or leakage-prone attribute
Highlights

Built and evaluated predictive models using Random Forest and Gradient Boosting.

Preprocessed a dataset of 47,000+ records with 70+ features.

Achieved R² ≈ 0.72 with a reduced and interpretable feature set.

Applied SHAP explainability for model interpretation.

Key Results

Top predictive drivers of energy efficiency:
✅ Wall & roof descriptions
✅ Total floor area
✅ Number of heated rooms
✅ Main fuel type

Developed a model that balances accuracy (72%) and practical usability, avoiding leakage-prone variables like CO₂ emissions.

Business Value

This project shows how machine learning can support sustainable housing policies by predicting building efficiency without requiring full audits — saving time, cost, and enabling smarter energy decisions.

📌 Project Overview

Energy efficiency is critical for reducing environmental impact, lowering energy bills, and improving sustainability.
This project applies machine learning regression models to predict Current Energy Efficiency from building characteristics.

The workflow includes:

Data preprocessing & encoding

Model training & evaluation

Feature importance analysis

Reducing features for interpretability

SHAP-based explainability

⚙️ Dataset

Source: UK Energy Performance Certificate (EPC) data

Records: ~47,000+ rows, 70+ features

Target variable: CURRENT_ENERGY_EFFICIENCY

🧪 Methodology

Preprocessing

Filled missing values (mode imputation)

Ordinal encoding for ratings (A–G, Poor–Excellent)

Label encoding for categorical features

Baseline Model

Random Forest Regressor

Achieved R² = 0.99 (but overfitted due to leakage features)

Feature Reduction

Removed biased features (e.g., CO₂ emissions, energy consumption)

Iteratively dropped non-informative attributes

Built reduced models for interpretability

Final Model

Random Forest with top features

Achieved R² ≈ 0.72, MSE ≈ 25.8

Explainability

Feature importance visualisation

SHAP plots for interpretability

📊 Results

Key Predictors: wall/roof descriptions, total floor area, heating system, main fuel

Final Model Performance:

R² ≈ 0.72

Mean Squared Error ≈ 25.8

🚀 Future Work

Test XGBoost / LightGBM

Hyperparameter tuning

Deploy model with Streamlit for interactive predictions

Explore geospatial effects (postcode-level trends)
