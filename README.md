# HDB-Flat-Value-Predictor
# 🏠 HDB Resale Price Predictor

*Predict resale prices of HDB flats in Singapore using machine learning.*
---

## 🌟 Table of Contents
- [Project Overview](#-project-overview)
- [Motivation](#-motivation)
- [Features](#-features)
- [How it works](#-How-it-works)
- [Technologies Used](#-technologies-used)
- [Dataset](#-dataset)
- [Model Development](#-model-development)
- [Web App Interface](#-web-app-interface)
- [Installation & Usage](#-installation--usage)
- [Screenshots](#-screenshots)
- [Future Improvements](#-future-improvements)
- [Contact](#-contact)

---

## 🚀 Project Overview
The **HDB Resale Price Predictor** is a web application that estimates resale prices of HDB flats in Singapore.  
It uses a trained **machine learning model** and an interactive **Streamlit interface** to provide instant predictions.

---

## 🎯 Motivation
Singapore’s HDB resale market is fast-paced and complex. This app helps:  
- Buyers & sellers make **informed decisions**  
- Quickly estimate resale prices without manual research  
- Showcase **practical machine learning applications**

---

## ✨ Features
- **Predict HDB resale price** in seconds using a trained machine learning model.
- **User-friendly interface** with interactive sidebar inputs.
- **Supports multiple flat types, models, and towns** in Singapore.
- **Flexible input options** including floor area, storey range, lease commencement, remaining lease, and transaction date.
- **Instant results** with a clear display of the estimated resale price.
---
## ⚡ How It Works
1. **User Inputs**: Provide details such as block code, street code, flat type, flat model, town, floor area, storey range, lease start year, remaining lease, and transaction date.  
2. **Data Encoding**: Categorical values (e.g., flat type, flat model, town) are converted into numeric codes as required by the model.  
3. **Prediction**: The trained machine learning model (`resale_price_model.joblib`) predicts the resale price of the flat.  
4. **Output**: The app displays the predicted price in a **clear, formatted message**.

---

## 📥 Installation

1. Clone the repository:
    
```bash
git clone <your-repo-url>
```

2.Navigate to the project directory:

```bash
cd Resale_price_web_app.py
```
3.Install dependencies:
```bash
pip install -r requirements.txt
```
4.Run the app:
```bash
streamlit run Resale_price_web_app.py
```
---

## 🛠 Technologies Used
- **Python** – main programming language  
- **Pandas** – data manipulation  
- **Scikit-learn** – machine learning  
- **Joblib** – saving trained models  
- **Streamlit** – web app interface  

---

## 📊 Dataset
- **Source:** Singapore HDB Resale Flat Prices dataset  
- **Features:**  
  - Town, Flat Type, Block Code, Street Name Code  
  - Floor Area (sqm), Flat Model  
  - Lease Commence Year, Remaining Lease  
  - Storey Range, Transaction Month & Year  

---

## 🧠 Model Development
1. Cleaned dataset & handled missing values  
2. Encoded categorical variables to numeric codes  
3. Trained regression models (Random Forest, Linear Regression)  
4. Selected best-performing model  
5. Saved model using `joblib` for deployment  

---

## 🖥 Web App Interface
- **Sidebar Inputs:** User-friendly form to enter flat details  
- **Predict Button:** Click to generate price instantly  
- **Formatted Output:** Shows price in a clear, readable format  

---

## ⚡ Installation & Usage
### Requirements
- Python 3.8+  
- Streamlit, Pandas, Scikit-learn, Joblib  

### Steps
```bash
# Clone the repo
git clone https://github.com/yourusername/hdb-resale-predictor.git
cd hdb-resale-predictor

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py

