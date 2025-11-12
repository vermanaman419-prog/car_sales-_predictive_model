# 🚗 Car Purchase Prediction System

### *From Customer Preferences to Smart Car Recommendations*

This project applies **Machine Learning (ML)** to predict which **car company, model, and estimated price** a customer is likely to choose based on their **Annual Income, Transmission Type, and Body Style**.

The solution includes **data cleaning, exploratory data analysis (EDA)**, model building, and a **Flask + Ngrok web app** for interactive predictions — all implemented using Python in Google Colab.

---

## 🧠 Project Overview

**Objective:**  
Build a predictive system that uses historical car sales data to recommend the most suitable car for a customer profile.

**Goal:**  
Transform structured sales data into an interactive, user-driven recommendation app powered by Machine Learning.

---

## 🧩 Tools & Technologies

| **Category** | **Tools Used** |
|---------------|----------------|
| Programming | Python (Pandas, NumPy, Scikit-learn) |
| Data Visualization | Matplotlib, Seaborn |
| Environment | Google Colab |
| Machine Learning | Random Forest, Linear Regression |
| Web Framework | Flask |
| Deployment | Pyngrok |
| Model Serialization | Joblib |

---

## ⚙️ Key Steps

### **1️⃣ Data Cleaning & Pre-processing**
- Handled missing and inconsistent data.
- Encoded categorical features (Transmission, Body Style).
- Scaled numeric features (Annual Income).
- Removed outlier values for stable regression.

### **2️⃣ Exploratory Data Analysis (EDA)**
- Analyzed most popular car companies and models by sales.
- Visualized relationships between **income and car price**.
- Identified top car body styles and transmission preferences.
- Evaluated seasonal sales trends across years.

### **3️⃣ Machine Learning Modeling**
| Model | Task | Algorithm | Metric | Performance |
|--------|------|------------|----------|--------------|
| 🏢 `company_clf` | Predict car company | Random Forest Classifier | Accuracy | **85%** |
| 🚘 `model_clf` | Predict car model | Random Forest Classifier | Accuracy | **2%** (due to class imbalance) |
| 💰 `price_reg` | Predict car price | Linear Regression | R² Score | **0.80** |
| | | | RMSE | **\$15,905** |

> 🔧 Future versions will exclude “Other” labels and focus on top 20 models per company for improved accuracy.

### **4️⃣ Model Deployment (Flask + Ngrok)**
- Created a Flask web app with a user form:
  - **Input:** Annual Income, Transmission, Body Style  
  - **Output:** Predicted Company, Model, and Price
- Deployed via Ngrok to access live from Colab.  
- Integrated real-time predictions from saved `.joblib` models.

---

## 🧮 Model Workflow
**Input → ML Prediction → Output**

| Input | Output |
|--------|---------|
| Annual Income | 💰 Price prediction |
| Transmission | ⚙️ Company preference |
| Body Style | 🚗 Model recommendation |

---

## 💻 Dashboard / Web Interface

**Interactive Flask App**

Users can:
- Enter their **annual income, transmission, and preferred body style**  
- Instantly receive:
  - Predicted **car company**
  - Predicted **model**
  - Estimated **price**

**Deployment Flow:**
1. Upload your trained `.joblib` models in Colab.
2. Run Flask app + Ngrok tunnel.
3. Access your unique public URL for live predictions.

---

## 📊 Key Insights

- Higher income groups lean toward premium car brands (BMW, Audi, Mercedes).  
- Manual transmission and Hatchback combinations dominate mid-range customers.  
- Price strongly correlates with annual income (R² ≈ 0.8).  
- “Other” models dilute accuracy — better performance on top-selling models.

---

## 🧭 Example Predictions

| Annual Income | Transmission | Body Style | Predicted Company | Predicted Model | Predicted Price |
|----------------|--------------|-------------|--------------------|-----------------|-----------------|
| 45,000 | Manual | Sedan | Toyota | Corolla | \$21,500 |
| 75,000 | Automatic | SUV | BMW | X5 | \$58,000 |
| 38,000 | Manual | Hatchback | Hyundai | i20 | \$16,200 |

---

## 🧱 Folder Structure

---

## 📈 Dashboard Preview
Interactive Flask App deployed via **Ngrok**.  
*https://jene-unpulleyed-kieran.ngrok-free.dev/*

---

## 🧭 Learnings
- Enhanced understanding of **classification vs regression** modeling.  
- Improved **EDA storytelling** and **feature engineering** using Python.  
- Gained hands-on experience deploying ML models with **Flask**.  
- Learned to build interactive, real-time ML apps using **Ngrok + Colab**.

---

## 🧰 Future Enhancements
- 🧩 Add **Top-3 model suggestions** for each company.  
- 🧮 Train per-brand model classifiers for higher precision.  
- ☁️ Deploy to **Render** or **Railway** for 24/7 access.  
- 📊 Add Streamlit dashboard for interactive visualization.

---

## 👨‍💻 Author

**Naman Verma**  
Machine Learning Enthusiast

📍 Gurugram, India  
📧 [vermanaman419@gmail.com](mailto:vermanaman419@gmail.com)  
🔗 [LinkedIn](www.linkedin.com/in/naman419)  
  
