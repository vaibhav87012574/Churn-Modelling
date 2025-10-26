# 📊 Churn Modelling

A machine learning project to predict customer churn using structured data and neural networks. The goal is to identify customers at risk of leaving a service or organization so that targeted retention strategies can be implemented.

---

## 💡 Overview

This repository contains code, data, and saved models used to analyze and predict customer churn. It includes:
- Exploratory Data Analysis (EDA)
- Data preprocessing pipelines
- ANN-based machine learning model
- Model deployment using a simple web application

---

## 📊 Dataset Description

- **File:** `Churn_Modelling.csv`  
- **Target Variable:** `Exited`  
  - `1` → Customer churned  
  - `0` → Customer retained

### 🔹 Key Features
| Feature              | Description                          |
|----------------------|----------------------------------------|
| Geography            | Customer’s country                    |
| Gender               | Male / Female                         |
| Age                  | Age of the customer                   |
| Tenure               | Number of years with the bank         |
| Balance              | Account balance                       |
| NumOfProducts        | Number of bank products used          |
| HasCrCard            | Whether the customer has a credit card|
| IsActiveMember       | Active customer status                |
| EstimatedSalary      | Annual salary                         |

---

## 🧠 Models & Methods

### ✅ Data Preprocessing
- Handled missing values  
- Applied **Label Encoding (Gender)** and **One-Hot Encoding (Geography)**  
- Normalized features using **StandardScaler**

### ✅ Exploratory Data Analysis (EDA)
- Visualized churn distribution  
- Correlation heatmap of features  
- Outlier and imbalance detection  

### ✅ Machine Learning Models
| Model Type           | Purpose                          |
|----------------------|----------------------------------|
| Logistic Regression   | Baseline performance            |
| Decision Tree         | Tree-based interpretability     |
| Random Forest         | Ensemble learning               |
| Artificial Neural Network (ANN) | Final high-performance model |

- Final model saved as **`model.h5`**
- Encoders and scaler saved for deployment

---

## ⚙️ Deployment

- `app.py` loads:
  - Trained model (`model.h5`)
  - Preprocessing pipelines (`scaler.pkl`, encoder files)
- Web interface allows users to input data and get real-time churn predictions

---

## ⭐ Key Features

- ✔ End-to-end pipeline: Data → Model → Deployment  
- ✔ ANN with hyperparameter tuning for improved accuracy  
- ✔ Ready-to-use web app for predictions  
- ✔ Modular design for easy extension and customization  

---

## 🚀 Usage Scenarios

- 📌 **Banks & Financial Institutions** – Identify customers likely to churn and offer retention plans  
- 📌 **Telecom / Subscription Companies** – Reduce customer drop-offs  
- 📌 **Students & Developers** – Learn churn modelling, ANN implementation, and deployment techniques

---

## 🛠 Future Enhancements

- Add XGBoost / LightGBM models  
- Deploy web app with Docker / Cloud (AWS, Render)  
- Build a dashboard using Streamlit or Power BI  
- Improve model explainability (SHAP, LIME)

---

## 📜 License

This project is licensed under the **GNU General Public License v3.0**.  
See the `LICENSE` file for more details.

---
