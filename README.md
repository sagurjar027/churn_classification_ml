# 📞 Customer Churn Prediction System

An end-to-end Machine Learning project designed to predict customer churn in the telecom industry. By utilizing multiple models and business-driven threshold optimization, this system helps identify customers who are likely to leave, enabling proactive and targeted retention strategies.

---

## 🚀 Project Overview

Customer churn directly impacts a company's bottom line. This project doesn't just predict churn; it optimizes those predictions for real-world business value. By prioritizing recall, the system ensures that the maximum number of at-risk customers are identified before they leave.

---

## 📊 Exploratory Data Analysis (EDA)

A deep dive into the dataset revealed several critical behavioral patterns. *(Check out the Jupyter Notebook in this repository for the full visual analysis).*

**Key Areas Explored:**
* **Churn Distribution:** Understanding the baseline churn rate.
* **Gender vs. Churn:** Analyzing demographic impacts.
* **Contract Type vs. Churn:** Evaluating commitment levels.
* **Monthly Charges vs. Churn:** Assessing price sensitivity.

### 🧠 Key Insights
* 📉 **Contract Length:** Customers with month-to-month contracts have the highest churn rate.
* 💰 **Pricing:** Higher monthly charges strongly correlate with a higher probability of churn.
* ⏳ **Loyalty:** Customers with a longer tenure are significantly more loyal.
* 📡 **Service Type:** Fiber optic internet users exhibit higher churn rates compared to DSL users.

---

## ⚙️ ML Pipeline

1.  **Data Cleaning & Preprocessing:** Handling missing values and formatting data.
2.  **Feature Encoding:** Manual mapping for categorical variables.
3.  **Feature Scaling:** Standardizing numerical features.
4.  **Model Training:** Training baseline and advanced ensemble models.
5.  **Threshold Tuning:** Adjusting decision boundaries for business alignment.
6.  **Model Comparison:** Evaluating performance metrics.
7.  **Deployment:** Building an interactive UI using Streamlit.

---

## 🎯 Modeling & Business Optimization

Standard machine learning models use a default threshold of `0.5`. However, in churn prediction, missing an at-risk customer (False Negative) is usually more costly than incorrectly flagging a loyal customer (False Positive). 

To align with the **business goal of reducing churn loss**, threshold tuning was applied to maximize **Recall**.

| Model | Focus | Optimal Threshold | Recall | Precision |
| :--- | :--- | :---: | :---: | :---: |
| **Random Forest** | High Recall (Detect max churners) | 0.4 | ~79% | ~52% |
| **XGBoost** | Balanced (Precision + Recall) | 0.6 | ~66% | ~60% |

---

## 💻 Streamlit App Features

The project includes a fully functional Streamlit web application that allows users to interact with the models:
* 🔍 **Real-time Prediction:** Input customer data to get immediate churn risk assessments.
* ⚙️ **Model Selection:** Toggle between the Random Forest (High Recall) and XGBoost (Balanced) models.
* 📊 **Risk Classification:** Probability-based scoring to categorize customers by risk level.
* 💡 **Business Recommendations:** Actionable insights based on the prediction.

---

## 📂 Project Structure

```text
📦 churn_classification_ml
 ┣ 📜 app.py               # Streamlit application
 ┣ 📜 rf_model.pkl         # Trained Random Forest model
 ┣ 📜 xgb_model.pkl        # Trained XGBoost model
 ┣ 📜 scaler.joblib        # Fitted scaler for numerical features
 ┣ 📜 requirements.txt     # Project dependencies
 ┗ 📜 README.md            # Project documentation

# Clone the repository
git clone [https://github.com/sagurjar027/churn_classification_ml.git](https://github.com/sagurjar027/churn_classification_ml.git)

# Navigate to the project directory
cd churn_classification_ml

# Install the required dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py

Gemini said
This is a solid foundation for a README! Customer churn is a high-impact business problem, and highlighting your threshold tuning (prioritizing recall) shows great product thinking, which recruiters and hiring managers love to see.

I've refined your draft to make it more professional, visually structured, and ready for your GitHub repository. I also fixed a small inconsistency in the "How to Run" section where the cloned folder name didn't match the cd command.

Here is the polished version:

Markdown
# 📞 Customer Churn Prediction System

An end-to-end Machine Learning project designed to predict customer churn in the telecom industry. By utilizing multiple models and business-driven threshold optimization, this system helps identify customers who are likely to leave, enabling proactive and targeted retention strategies.

---

## 🚀 Project Overview

Customer churn directly impacts a company's bottom line. This project doesn't just predict churn; it optimizes those predictions for real-world business value. By prioritizing recall, the system ensures that the maximum number of at-risk customers are identified before they leave.

---

## 📊 Exploratory Data Analysis (EDA)

A deep dive into the dataset revealed several critical behavioral patterns. *(Check out the Jupyter Notebook in this repository for the full visual analysis).*

**Key Areas Explored:**
* **Churn Distribution:** Understanding the baseline churn rate.
* **Gender vs. Churn:** Analyzing demographic impacts.
* **Contract Type vs. Churn:** Evaluating commitment levels.
* **Monthly Charges vs. Churn:** Assessing price sensitivity.

### 🧠 Key Insights
* 📉 **Contract Length:** Customers with month-to-month contracts have the highest churn rate.
* 💰 **Pricing:** Higher monthly charges strongly correlate with a higher probability of churn.
* ⏳ **Loyalty:** Customers with a longer tenure are significantly more loyal.
* 📡 **Service Type:** Fiber optic internet users exhibit higher churn rates compared to DSL users.

---

## ⚙️ ML Pipeline

1.  **Data Cleaning & Preprocessing:** Handling missing values and formatting data.
2.  **Feature Encoding:** Manual mapping for categorical variables.
3.  **Feature Scaling:** Standardizing numerical features.
4.  **Model Training:** Training baseline and advanced ensemble models.
5.  **Threshold Tuning:** Adjusting decision boundaries for business alignment.
6.  **Model Comparison:** Evaluating performance metrics.
7.  **Deployment:** Building an interactive UI using Streamlit.

---

## 🎯 Modeling & Business Optimization

Standard machine learning models use a default threshold of `0.5`. However, in churn prediction, missing an at-risk customer (False Negative) is usually more costly than incorrectly flagging a loyal customer (False Positive). 

To align with the **business goal of reducing churn loss**, threshold tuning was applied to maximize **Recall**.

| Model | Focus | Optimal Threshold | Recall | Precision |
| :--- | :--- | :---: | :---: | :---: |
| **Random Forest** | High Recall (Detect max churners) | 0.4 | ~79% | ~52% |
| **XGBoost** | Balanced (Precision + Recall) | 0.6 | ~66% | ~60% |

---

## 💻 Streamlit App Features

The project includes a fully functional Streamlit web application that allows users to interact with the models:
* 🔍 **Real-time Prediction:** Input customer data to get immediate churn risk assessments.
* ⚙️ **Model Selection:** Toggle between the Random Forest (High Recall) and XGBoost (Balanced) models.
* 📊 **Risk Classification:** Probability-based scoring to categorize customers by risk level.
* 💡 **Business Recommendations:** Actionable insights based on the prediction.

---

## 📂 Project Structure

```text
📦 churn_classification_ml
 ┣ 📜 app.py               # Streamlit application
 ┣ 📜 rf_model.pkl         # Trained Random Forest model
 ┣ 📜 xgb_model.pkl        # Trained XGBoost model
 ┣ 📜 scaler.joblib        # Fitted scaler for numerical features
 ┣ 📜 requirements.txt     # Project dependencies
 ┗ 📜 README.md            # Project documentation
▶️ How to Run Locally
Follow these steps to run the Streamlit app on your local machine:

Bash
# Clone the repository
git clone [https://github.com/sagurjar027/churn_classification_ml.git](https://github.com/sagurjar027/churn_classification_ml.git)

# Navigate to the project directory
cd churn_classification_ml

# Install the required dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
👨‍💻 Author
Sahil Kasana

[GitHub](https://github.com/sagurjar027)

[LinkedIn](https://www.linkedin.com/in/sahil-kasana6055/)
