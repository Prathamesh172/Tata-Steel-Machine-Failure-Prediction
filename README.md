# 🔧 Predictive Maintenance: Machine Failure Prediction (TATA Steel Case Study)

## 📌 Project Overview
In the manufacturing sector, **predicting machine failures before they happen** can significantly reduce downtime, improve efficiency, and cut maintenance costs.  
This project simulates a **TATA Steel use case** using a synthetic dataset that mimics real-world failure scenarios.

The goal: **predict whether a machine will fail** based on sensor readings and operational parameters.

---

## 🛠️ Tech Stack
- **Python**: Data manipulation and modeling  
- **Pandas, NumPy**: Data cleaning & feature engineering  
- **Matplotlib, Seaborn**: Visualization & EDA  
- **Scikit-Learn**: Preprocessing, Logistic Regression, Random Forest  
- **XGBoost, LightGBM**: Gradient boosting models for predictive accuracy  

---

## 🔍 Workflow
1. **Business Understanding**: Minimize downtime & proactive maintenance.  
2. **EDA**: Checked target imbalance, feature distributions, and correlations.  
3. **Feature Engineering**:
   - Dropped leakage columns (failure flags).
   - Created engineered features like temperature difference, torque × speed.  
4. **Preprocessing**:
   - One-Hot Encoding for categorical variables (`Type`).  
   - Standard Scaling for numeric features.  
5. **Modeling & Evaluation**:
   - Logistic Regression (baseline).  
   - Random Forest (strong performance).  
   - **XGBoost (best)**: ROC-AUC = **0.95**, F1 = **0.87**.  
6. **Insights**:
   - Failures are rare (class imbalance).  
   - Key drivers: torque, tool wear, and process–air temperature differential.  

---

## 📈 Results
- **Best Model**: XGBoost  
- **ROC-AUC**: 0.95  
- **F1 Score**: 0.87  
- **Business Value**: Maintenance can focus on the top 5–10% of high-risk machines → prevent costly downtime.  

---

## 📊 Visualizations
- Target class imbalance  
- Feature distributions & correlations  
- Predicted failure probabilities (test set)  
- Feature importance (XGBoost)  

---

## 📂 Repository Structure
