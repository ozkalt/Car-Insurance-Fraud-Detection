
# 🚗 Car Insurance Fraud Detection

This project simulates a realistic car insurance dataset and applies machine learning techniques to detect fraudulent claims.

## 📊 Dataset Description

The dataset contains **10,000 rows** and includes detailed information about:
- Vehicle specifications (type, brand, model, year, price)
- Policyholder demographics (age, gender, region, occupation)
- Insurance and claim details (claim amount, repair costs, submission method)
- Agent and channel info
- Fraud label (`fraud_reported`)

### 🧾 Sample Features
- `vehicle_make`, `vehicle_model`, `vehicle_age`
- `vehicle_price`, `net_premium`
- `claim_reason`, `damage_type`, `claim_amount`
- `policy_type`, `claims_history`
- `fraud_reported` (target)

## 🛠️ Project Goals

- Simulate a realistic dataset for supervised fraud detection
- Explore data distributions and feature relationships
- Train machine learning models (XGBoost, LightGBM, CatBoost, etc.)
- Handle class imbalance using SMOTE and/or class weights
- Evaluate model performance using AUC, precision, recall
- Explain model decisions using SHAP or LIME

## 🧪 Planned ML Pipeline

1. Data preprocessing & feature encoding
2. Imbalance handling with `SMOTE`
3. Model training with:
   - Random Forest
   - XGBoost
   - LightGBM
   - CatBoost
   - (Optional: Neural Networks)
4. Evaluation with metrics like:
   - Confusion Matrix
   - Precision, Recall, F1-Score
   - ROC AUC, PR AUC
5. Model explainability via SHAP

## 📁 File Structure (Suggested)

```
fraud-detection-insurance/
├── data/
│   └── simulated_data.csv
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb
│   └── 02_modeling_pipeline.ipynb
├── src/
│   ├── preprocessing.py
│   ├── modeling.py
│   ├── evaluation.py
├── reports/
│   └── fraud_insights_report.md
├── README.md
```

## 📌 Notes

- The dataset is fully synthetic and generated using NumPy and pandas.
- Fraud cases are ~3% of total, simulating real-world imbalance.
- Premium is calculated based on vehicle price using a multiplier between 3–8%.

## 👤 Author

Generated with ❤️ by [ChatGPT + User]
