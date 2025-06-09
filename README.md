# 🛒 Online Retail Customer Behavior Analysis with ML

This project explores and analyzes online retail transaction data to gain insights into customer behavior. It includes data cleaning, visualization, feature engineering (RFM), and supervised machine learning classification to predict customer segments or patterns.

---

## 📌 Objective

To understand customer behavior from transactional data and apply machine learning models to classify or predict customer-related outcomes based on derived features.

---

## 🧰 Tools & Technologies

- Python (Jupyter Notebook)
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `sklearn`

---

## 📁 Dataset

- **Source**: UCI Machine Learning Repository
- **File**: `Online Retail.xlsx`
- **Features**:
  - InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🔍 Workflow Summary

### 1. Environment Setup
- Imported essential libraries and configurations

### 2. Data Loading
- Loaded Excel data using `pandas.read_excel()`
- Performed initial data inspection

### 3. Data Cleaning & Preprocessing
- Removed:
  - Null values (especially missing `CustomerID`)
  - Duplicate and invalid entries
  - Negative quantities and zero/negative pricing
- Handled datetime parsing

### 4. Exploratory Data Analysis (EDA)
- Identified:
  - Country-wise sales distribution
  - Most frequently sold products
  - Monthly and daily sales trends
- Used visualizations:
  - Line charts, bar plots, histograms

### 5. Feature Engineering (RFM)
- Included new fields that are required.
  - total_amount, number_of_orders, avg_order_value, unique_products, avg_quantity, days_since_first_purchase
### 6. Model Building
- Split dataset into `train/test`
- Applied and compared classification models:
  - Logistic Regression
  - Decision Tree Classifier
  - Random Forest Classifier
  - Gradient Boosting
  - K-Nearest Neighbors (KNN)

### 7. Model Evaluation
- Evaluated models using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
  - Classification Report

### 8. Conclusion
- Gradient Boosting achieved the highest performance
- RFM features are useful for customer classification
- Demonstrated the power of combining business logic (RFM) with machine learning

---

## 📈 Key Takeaways

- Most customers are from the UK
- Few products dominate sales frequency
- Gradient Boosting and Random Forest provided interpretable and accurate results
- RFM segmentation improves model effectiveness

---

## 📁 Folder Structure

```

📦Online-Retail-ML-Project
┣ 📜README.md
┣ 📓Online Retail Final Project - Updated.ipynb
┗ 📄Online Retail.xlsx

````
---
