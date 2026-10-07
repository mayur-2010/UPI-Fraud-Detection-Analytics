# 💳 UPI Transactions & Digital Payments Fraud Detection and Customer Behavior Analytics

## 📌 Project Overview

Digital payment platforms such as UPI process a large number of transactions every day. With the rapid growth of digital payments, fraudulent transactions and unusual customer behavior have also become important concerns.

This project develops a **Machine Learning-based fraud detection system** that analyzes UPI transaction data to identify potentially fraudulent transactions and understand customer transaction behavior.

The project uses **Ensemble Learning** and compares multiple machine learning algorithms to identify the best-performing model.

The algorithms compared are:

- Random Forest
- Extra Trees
- Gradient Boosting
- XGBoost

The best-performing model is selected using evaluation metrics such as **Precision, Recall, F1-Score, and ROC-AUC**.

---

## 🎯 Problem Statement

Digital payment companies need an efficient way to identify suspicious transactions while minimizing false fraud alerts.

The objective of this project is to:

- Detect fraudulent UPI transactions.
- Analyze customer transaction behavior.
- Identify suspicious transaction patterns.
- Compare multiple ensemble learning algorithms.
- Select the best-performing fraud detection model.
- Provide meaningful business insights from transaction data.

---

## 💡 Proposed Solution

The project follows an end-to-end machine learning workflow:

```text
UPI Transaction Data
        ↓
Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Feature Engineering
        ↓
Data Preprocessing
        ↓
Train-Test Split
        ↓
Ensemble Learning
        ↓
Model Comparison
        ↓
Best Model Selection
        ↓
Fraud Prediction
        ↓
Business Insights
```

---

## 🧠 Machine Learning Models

### 1. Random Forest

Random Forest combines multiple decision trees and uses their combined predictions to improve classification performance.

### 2. Extra Trees

Extra Trees is an ensemble of randomized decision trees that can provide strong performance on structured transaction data.

### 3. Gradient Boosting

Gradient Boosting builds models sequentially, where each new model attempts to correct errors made by previous models.

### 4. XGBoost

XGBoost is an optimized gradient boosting algorithm designed for high-performance classification and regression problems.

**XGBoost is used as the primary candidate model**, while the final model is selected based on actual evaluation results.

---

## 📊 Dataset Features

The dataset contains transaction and customer-related information such as:

| Feature | Description |
|---|---|
| Transaction_ID | Unique transaction identifier |
| Customer_ID | Unique customer identifier |
| Transaction_Date | Date of transaction |
| Transaction_Time | Time of transaction |
| Transaction_Amount | Transaction amount |
| Transaction_Type | Type of transaction |
| Merchant_Category | Merchant category |
| Payment_Method | Payment method |
| Device_Type | Device used |
| Location | Transaction location |
| Customer_Age | Customer age |
| Account_Age_Days | Age of customer account |
| Previous_Transactions | Previous transaction count |
| Avg_Transaction_Amount | Average transaction amount |
| Transactions_Last_24h | Transactions in last 24 hours |
| Failed_Transactions | Number of failed transactions |
| New_Device | Whether a new device was used |
| International_IP | Whether international IP was detected |
| Fraud | Target variable |

### Target Variable

```text
0 → Legitimate Transaction
1 → Fraudulent Transaction
```

---

## ⚙️ Feature Engineering

Additional features are created to improve fraud detection:

- Hour
- Day
- Month
- Day of Week
- Weekend Indicator
- Night Transaction Indicator
- Transaction Amount Ratio
- Failed Transaction Rate

### Transaction Amount Ratio

```text
Transaction Amount / Average Transaction Amount
```

This helps identify transactions that are unusually large compared with a customer's normal spending behavior.

---

## 🔍 Exploratory Data Analysis

The project performs analysis of:

- Fraud vs legitimate transactions
- Transaction amount distribution
- Fraud by transaction time
- Fraud by location
- Fraud by device type
- Fraud by merchant category
- Customer transaction frequency
- Failed transaction behavior
- Average transaction amount

---

## 📏 Model Evaluation

Because fraud detection is generally an imbalanced classification problem, accuracy alone is not sufficient.

The following metrics are used:

### Accuracy

Measures the percentage of correctly classified transactions.

### Precision

Measures how many transactions predicted as fraud are actually fraudulent.

### Recall

Measures how many actual fraudulent transactions are detected.

### F1-Score

Provides a balance between Precision and Recall.

### ROC-AUC

Measures the model's ability to distinguish between legitimate and fraudulent transactions.

---

## 🏆 Model Comparison

The project compares four ensemble algorithms:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Random Forest | — | — | — | — | — |
| Extra Trees | — | — | — | — | — |
| Gradient Boosting | — | — | — | — | — |
| XGBoost | — | — | — | — | — |

> The final values are generated from the actual dataset during model evaluation. The model with the strongest overall performance is selected as the final fraud detection model.

---

## 📈 Customer Behavior Analytics

Apart from fraud detection, the project analyzes customer behavior based on:

- Transaction frequency
- Average spending
- Transaction value
- Failed transactions
- Device usage
- Transaction timing
- Location patterns
- High-value transactions

These insights can help identify unusual customer activity and potential risk patterns.

---

## 🛠️ Technology Stack

### Programming
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn

### Analytics
- Exploratory Data Analysis
- Feature Engineering
- Statistical Analysis

### Machine Learning
- Random Forest
- Extra Trees
- Gradient Boosting
- XGBoost

### Visualization
- Matplotlib
- Seaborn

---

## 📁 Project Structure

```text
UPI-Fraud-Detection/
│
├── dataset/
│   └── upi_transactions.csv
│
├── notebooks/
│   └── UPI_Fraud_Detection.ipynb
│
├── results/
│   ├── model_comparison.csv
│   └── confusion_matrix.png
│
├── README.md

```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/UPI-Fraud-Detection.git
```

Navigate to the project:

```bash
cd UPI-Fraud-Detection
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost
```

---

## ▶️ How to Run

1. Place the UPI transaction dataset inside the `dataset` folder.
2. Open `UPI_Fraud_Detection.ipynb`.
3. Install the required libraries.
4. Run the notebook sequentially.
5. Perform data preprocessing and feature engineering.
6. Train the four ensemble models.
7. Compare model performance.
8. Select the best-performing model.
9. Evaluate the final model.
10. Analyze fraud and customer behavior.

---

## 📊 Expected Output

The project generates:

- Fraud distribution analysis
- Transaction behavior analysis
- Feature-engineered dataset
- Model comparison table
- Accuracy, Precision, Recall and F1-Score
- ROC-AUC comparison
- Confusion matrix
- Fraud prediction
- Customer behavior insights

---

## 🔮 Future Scope

The project can be further improved by:

- Real-time UPI fraud detection
- Real-time transaction monitoring
- Deep learning models
- Anomaly detection
- Explainable AI for fraud predictions
- Real-time fraud alerts
- Customer risk scoring
- API deployment using Flask/FastAPI
- Cloud deployment
- Integration with banking/payment systems

---

## 🎓 Learning Outcomes

Through this project, the following skills are demonstrated:

- Python Programming
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Classification
- Ensemble Learning
- Model Evaluation
- Imbalanced Dataset Handling
- Fraud Detection
- Customer Behavior Analytics
- Data Visualization
- Business Problem Solving

---

## 👨‍💻 Project Author

**Mayur Pawar**

M.Sc. Computer Science  
Data Analytics & Machine Learning

---

## ⭐ Conclusion

This project provides an end-to-end solution for **UPI fraud detection and customer behavior analytics** using ensemble machine learning.

By comparing **Random Forest, Extra Trees, Gradient Boosting, and XGBoost**, the project identifies the model that provides the best performance for detecting fraudulent transactions.

The combination of **Machine Learning, Python, SQL, and Power BI** makes this project suitable for demonstrating practical **Data Analytics and Machine Learning skills**.
