# HDB-Flat-Value-Predictor
# 🏠 HDB Resale Price Predictor

*Predict resale prices of HDB flats in Singapore using machine learning.*
---

## 🌟 Table of Contents
- [Project Overview](#-project-overview)
- [Motivation](#-motivation)
- [Features](#-features)
- [How it works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Dataset](#-dataset)
- [Model Development](#-model-development)
- [Web App Interface](#-web-app-interface)
- [Screenshots](#-screenshots)
- [Prediction Result](#prediction-result)
- [Useful Links](#useful-links)
- [Future Improvements](#-future-improvements)
- [Key Learnings](#key-learnings)

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

This project leverages the following technologies and libraries to predict HDB resale prices and provide a user-friendly web interface:

| Technology          | Description                                                                |
| ------------------- | -------------------------------------------------------------------------- |
| 🐍 **Python**       | Core programming language used for the machine learning model and web app. |
| 📊 **Pandas**       | Library for data manipulation and preprocessing.                           |
| 🤖 **Scikit-learn** | Machine learning library for training the resale price prediction model.   |
| 💾 **Joblib**       | Used for saving and loading trained machine learning models efficiently.   |
| 🌐 **Streamlit**    | Framework to build an interactive web application interface.               |
| 🔢 **NumPy**        | Library for numerical computations and matrix operations.                  |

---

## 📊 Dataset
- **Source:** Singapore HDB Resale Flat Prices dataset  
- **Purpose:**
    -The dataset provides historical resale transactions of HDB flats, which is used to train the machine learning model to predict resale prices accurately.

- **Key Features:**
  
 | Feature                      | Description                                                    |
| ---------------------------- | -------------------------------------------------------------- |
| **Town**                     | Location of the HDB flat                                       |
| **Flat Type**                | Type of flat (e.g., 2 ROOM, 3 ROOM, 4 ROOM, 5 ROOM, EXECUTIVE) |
| **Block Code**               | Numerical code representing the block number                   |
| **Street Name Code**         | Numerical code representing the street                         |
| **Floor Area (sqm)**         | Size of the flat in square meters                              |
| **Flat Model**               | Design/model of the flat                                       |
| **Lease Commence Year**      | The year the flat lease started                                |
| **Remaining Lease**          | Remaining lease duration in years                              |
| **Storey Range**             | Range of storey levels for the flat                            |
| **Transaction Month & Year** | Date when the resale transaction occurred                      |


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
## 📸 Screenshots

**Average Resale Price by Town**
<img width="1187" height="490" alt="by town" src="https://github.com/user-attachments/assets/7b74fdda-cab3-4692-9d8a-5c8844706ffd" />
**Top 10 Streets by Average Resale Price**
<img width="1139" height="547" alt="Top 10 Streets by Average Resale Price" src="https://github.com/user-attachments/assets/22627396-fda9-479c-8a0a-5464f0a32252" />
**Distribution of Flat Types**
<img width="989" height="489" alt="Distribution of Flat Types" src="https://github.com/user-attachments/assets/f56ac949-d291-441a-9b59-d25d17544172" />
**Distribution of Lease Commencement Year**
<img width="988" height="490" alt="Distribution of Lease Commencement Year" src="https://github.com/user-attachments/assets/9963ffb6-3af4-40b1-ad64-c379b9ad77e6" />
**corelation**
<img width="921" height="826" alt="corelation" src="https://github.com/user-attachments/assets/c1c5b0b2-ae19-4b66-958d-dcdeeb9cc48f" />

---
## Prediction Result
This screenshot shows the HDB Resale Price Predictor built with Streamlit. Users input flat details like Block Code, Flat Type, Town, Floor Area, and Storey range in the sidebar. After clicking Predict Resale Price, the estimated resale price is displayed clearly on the main page. The interface is simple and user-friendly for quick price predictions.

<img width="1770" height="909" alt="Screenshot 2025-10-30 165722" src="https://github.com/user-attachments/assets/10e9272c-ae2e-4486-bcc2-76d8a0189175" />

---
## Useful Links
Project Link:https://github.com/pavanimudireddy/HDB-Flat-Value-Predictor

LinkedIn: www.linkedin.com/in/pavani-mudireddy

## 🚀 Future Improvements

- **Expand Dataset Coverage:** Add more towns, flat types, and recent resale transactions to improve accuracy.  
- **Advanced ML Models:** Explore XGBoost, LightGBM, or Neural Networks for better predictions.  
- **Enhanced Features:** Include proximity to MRT, amenities, schools, and time-based trends.  
- **Prediction Confidence:** Provide a price range or confidence interval instead of a single value.  
- **Interactive Visualizations:** Display historical trends and compare predictions with area averages.  
- **Better UX:** Support CSV uploads for batch predictions and map-based town selection.  
- **Real-time Updates:** Integrate APIs to keep resale data current.  
- **Mobile Optimization:** Make the Streamlit app mobile-friendly.  
- **Explainable AI:** Show feature importance to explain predictions.  
- **Localization:** Add multi-language support for wider accessibility.

## Key Learnings

- Effectively preprocessed data by converting categorical variables into numeric codes for model input.
- Built, trained, and saved a machine learning model for predicting HDB resale prices.
- Identified important features that influence resale price predictions.
- Developed an interactive web app using Streamlit for real-time user input and predictions.
- Handled diverse user inputs and implemented input validation for reliable predictions.
- Integrated the trained model with a user-friendly frontend interface.
- Recognized opportunities for future improvements such as advanced models and better feature engineering.
- Gained practical experience in deploying an end-to-end machine learning project from data to web application.

## Feel free to:

⭐ Star this repository if you found it helpful

🐞 Report issues or suggest improvements

🚀 Contribute and help make this project better!



