# Web-Based Explainable Machine Learning Model for Early-Stage Heart Disease Detection

[![Conference - IEEE i-COSTE 2025](https://img.shields.io/badge/IEEE-i--COSTE%202025-blue.svg)](https://doi.org/10.1109/i-COSTE68047.2025.11467478)[cite: 1]
[![DOI](https://img.shields.io/badge/DOI-10.1109%2Fi--COSTE68047.2025.11467478-brightgreen.svg)](https://doi.org/10.1109/i-COSTE68047.2025.11467478)[cite: 1]
[![License - MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Official repository for the research paper **"Web-Based Explainable Machine Learning Model for Early-Stage Heart Disease Detection"**, presented at **i-COSTE 2025**[cite: 1].

---

## 📌 Overview
This project presents an explainable machine learning (XAI) framework to predict early-stage heart disease risk[cite: 1]. It features an interactive web interface allowing users and clinical professionals to make real-time predictions while providing transparent feature attribution explanations[cite: 1].

---

## 📊 Dataset Description
The dataset comprises **70,000 instances** across **19 clinical and lifestyle features**[cite: 1]:

| Category | Features Included |
| :--- | :--- |
| **Demographics** | `Age`, `Gender`[cite: 1] |
| **Medical History** | `High_BP`, `High_Cholesterol`, `Diabetes`, `Obesity`[cite: 1] |
| **Lifestyle & Genetics** | `Smoking`, `Sedentary_Lifestyle`, `Family_History`, `Chronic_Stress`[cite: 1] |
| **Early Symptoms** | `Chest_Pain`, `Shortness_of_Breath`, `Fatigue`, `Palpitations`, `Dizziness`, `Swelling`, `Pain_Arms_Jaw_Back`, `Cold_Sweats_Nausea`[cite: 1] |
| **Target Variable** | `Heart_Risk` (`0` = Low Risk, `1` = High Risk)[cite: 1] |

---

## 🚀 Quickstart

### Data Preprocessing
```python
import pandas as pd

# Load dataset
df = pd.read_csv('data/heart_disease_risk_dataset_earlymed.csv')[cite: 1]

# Convert floating-point features to integers
for col in df.columns:
    if df[col].dtype == "float64":
        df[col] = df[col].astype(int)[cite: 1]
