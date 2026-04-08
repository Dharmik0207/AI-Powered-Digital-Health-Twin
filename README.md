🏥 AI-Powered Digital Health Twin : Patient Risk Prediction & Insight Generation System

📌 Project Overview

This project presents an end-to-end healthcare analytics pipeline that simulates a simplified Digital Health Twin system.
It predicts patient health risk and generates actionable insights using machine learning.

The goal is not only prediction, but also decision support, enabling better understanding of patient conditions.

🚀 Key Features
🔄 Complete data pipeline (loading → preprocessing → feature engineering)
🤖 Machine Learning models for risk prediction
📊 Model evaluation using multiple performance metrics
⚠️ Anomaly detection for identifying abnormal patient patterns
💡 Insight generation layer (human-readable explanations)
📈 Visualizations for better understanding of data and model behavior

📂 Dataset
Synthetic dataset with 400 patient records
Features include:
age
gender
blood_pressure
heart_rate
bmi
glucose_level
sleep_hours
activity_level
smoking_status

⚙️ Data Pipeline

The pipeline consists of:

Data Loading
CSV dataset ingestion using Pandas
Preprocessing
Handling missing values
Encoding categorical variables
Feature scaling (StandardScaler)
Feature Engineering
Derived features such as:
BMI risk category
Combined lifestyle indicators

🤖 Machine Learning Models
Baseline Model
Logistic Regression / Decision Tree
Advanced Model
Random Forest Classifier

📊 Model Evaluation

Models were evaluated using:

Accuracy
Precision
Recall
ROC-AUC Score

👉 The Random Forest model outperformed the baseline with better generalization and higher ROC-AUC.

⚠️ Anomaly Detection

Implemented to detect abnormal patient patterns such as:

Extremely high heart rate
High glucose with low BMI
Inconsistent lifestyle indicators

Techniques used:

Statistical thresholds (Z-score / IQR)
Rule-based detection

💡 Insight Layer (Key Highlight)

The system translates predictions into human-readable insights, for example:

“High risk due to elevated BMI, high glucose levels, and low activity level.”

This makes the system useful for decision support, not just prediction.

📈 Visualizations
Feature importance (Random Forest)
Risk distribution across patients
Correlation heatmap
Key health indicators vs risk


🧠 Tech Stack
Python
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn


📁 Project Structure
├── data/
│   └── synthetic_patient_dataset.csv
├── notebook/
│   └── health_risk_model.ipynb
├── visuals/
│   └── charts.png
├── report/
│   └── project_report.pdf
└── README.md


📊 Results Summary
Random Forest achieved the best performance
Strong correlation between:
High BMI + High Glucose → Higher risk
Low activity and smoking significantly increase risk

⚠️ Limitations
Synthetic dataset (not real-world clinical data)
Limited feature set
No temporal (time-series) data


🔮 Future Improvements
Use real-world healthcare datasets
Add deep learning models
Deploy as API (Flask/FastAPI)
Integrate with real Digital Health Twin systems
