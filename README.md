# Web-Based Explainable Machine Learning Model for Early-Stage Heart Disease Detection

[![Conference - IEEE i-COSTE 2025](https://img.shields.io/badge/IEEE-i--COSTE%202025-blue.svg)](https://doi.org/10.1109/i-COSTE68047.2025.11467478)
[![DOI](https://img.shields.io/badge/DOI-10.1109%2Fi--COSTE68047.2025.11467478-brightgreen.svg)](https://doi.org/10.1109/i-COSTE68047.2025.11467478)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License - MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Official repository for the research paper **"Web-Based Explainable Machine Learning Model for Early-Stage Heart Disease Detection"**, presented at the **2025 IEEE International Conference on Science, Technology, and Engineering (i-COSTE)**.

---

## 📌 Abstract & Overview
Cardiovascular diseases (CVDs) remain a leading cause of global mortality. Early diagnosis using clinical and lifestyle metrics can substantially improve intervention success. This repository hosts a complete end-to-end Machine Learning pipeline integrated with Explainable AI (XAI) frameworks and deployed via an interactive web interface. The system enables non-expert users and healthcare professionals to obtain instant risk assessments along with transparent, human-interpretable explanations of feature importances driving each prediction.

---

## Key Contributions
* **Large-Scale Data Processing**: Preprocessed and structured 70,000 patient instances across 19 clinical, demographic, lifestyle, and early-symptom features.
* **Explainable AI Integration**: Embedded model-agnostic local and global explanation techniques (SHAP & LIME) directly into the prediction workflow to eliminate the "black-box" nature of medical AI models.
* **Interactive Web Platform**: Designed and deployed a lightweight web application allowing real-time parameter input and transparent prediction visualizations for clinical decision support.

---

## 🛠 Technologies Used

* **Core Language**: Python 3.8+
* **Data Processing & Analytics**: `pandas`, `numpy`
* **Machine Learning & Modeling**: `scikit-learn`
* **Explainable AI (XAI)**: `shap`, `lime`
* **Web Framework & Deployment**: `streamlit` (or `flask`)
* **Visualization**: `matplotlib`, `seaborn`

---

## 📊 Dataset Description
The underlying dataset comprises **70,000 instances** with **19 input features** and 1 binary target variable (`Heart_Risk`):

| Feature Category | Attributes | Description / Encoding |
| :--- | :--- | :--- |
| **Demographics** | `Age`, `Gender` | Basic demographic attributes |
| **Medical Conditions** | `High_BP`, `High_Cholesterol`, `Diabetes`, `Obesity` | Binary flags (`0` = No, `1` = Yes) |
| **Lifestyle & Genetics** | `Smoking`, `Sedentary_Lifestyle`, `Family_History`, `Chronic_Stress` | Lifestyle and hereditary risk metrics (`0` = No, `1` = Yes) |
| **Early Symptoms** | `Chest_Pain`, `Shortness_of_Breath`, `Fatigue`, `Palpitations`, `Dizziness`, `Swelling`, `Pain_Arms_Jaw_Back`, `Cold_Sweats_Nausea` | Reported preliminary symptoms (`0` = Absent, `1` = Present) |
| **Target Variable** | `Heart_Risk` | Binary classification (`0` = Low Risk, `1` = High Risk) |

---

## 🚀 Quickstart

### 1. Installation & Environment Setup
Clone the repository and install dependencies:
```bash
git clone [https://github.com/YOUR_USERNAME/Heart-Disease-XAI-Web.git](https://github.com/YOUR_USERNAME/Heart-Disease-XAI-Web.git)
cd Heart-Disease-XAI-Web
pip install -r requirements.txt
