# 🧠 Machine Learning Project — Regression & Classification

## 📘 Overview
This project demonstrates the development of **two types of supervised machine learning models** — **Regression** and **Classification** — using real-world datasets.  
Each model follows a structured workflow: **Exploratory Data Analysis (EDA)** → **Preprocessing** → **Model Building** → **Evaluation** → **Interpretation**.  

---

## 🎯 Regression Model — Video Game Sales Prediction

### **Objective**
Predict global video game sales based on regional sales data (North America, Europe, Japan, and Others) using regression techniques.

### **Models Used**
1. **Linear Regression**
   - **Version 1:** Used 3 numerical features (`NA_Sales`, `EU_Sales`, `JP_Sales`).  
   - **Version 2:** Added `Other_Sales` and `Year` to improve predictive accuracy.  
   - **Evaluation Metrics:** R² Score, RMSE, and Residual Analysis.  
   - **Outcome:** The model performed well in explaining the relationship between regional and global sales, showing strong correlation across regions.

2. **K-Nearest Neighbors (KNN Regressor)**
   - Tested with **k=3** and **k=5** neighbors.  
   - Performance compared using R² and RMSE.  
   - While the model handled non-linear patterns, it was sensitive to scaling and dataset size.  
   - **Best result:** Linear Regression (5 features) showed the highest accuracy and interpretability.

---

## 🧾 Classification Model — Credit Score Prediction

### **Objective**
Predict a customer’s **Credit Score category** (*Good*, *Standard*, or *Poor*) based on financial and demographic data.  
The model helps financial institutions automate risk assessment and reduce human bias.

### **Models Used**
1. **Logistic Regression**
   - **Version 1:** Used only numeric features.  
   - **Version 2:** Included both numeric and encoded categorical features.  
   - **Metrics:** Accuracy, Precision, Recall, F1 Score.  
   - **Result:** Performed best overall — interpretable and consistent across all metrics.

2. **K-Nearest Neighbors (KNN Classifier)**
   - **Version 1:** k=3  
   - **Version 2:** k=5  
   - Evaluated with the same metrics.  
   - KNN showed good performance after scaling but was less stable compared to Logistic Regression.  

---

## 📊 Evaluation Summary
| Model Type | Version | Accuracy / R² | F1 / RMSE | Remarks |
|-------------|----------|---------------|------------|----------|
| Linear Regression | 3 features | High R² | Low RMSE | Simple & effective |
| Linear Regression | 5 features | **Best R²** | **Lowest RMSE** | Most reliable |
| KNN Regressor | k=3 / k=5 | Moderate | Medium RMSE | Non-linear, less stable |
| Logistic Regression | Numeric only | Balanced | Good F1 | Solid baseline |
| Logistic Regression | All features | **Best overall** | **Highest F1** | Recommended |
| KNN Classifier | k=3 / k=5 | Moderate | Fair F1 | Sensitive to scaling |

---

## 🧩 Tools & Libraries
- **Python**, **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **scikit-learn** for model training and evaluation
- **Jupyter Notebook** for code, visualizations, and documentation

---

## 🧠 Key Takeaways
- Linear and Logistic Regression models are **interpretable**, **efficient**, and perform consistently well.  
- KNN can capture **non-linear relationships** but requires careful scaling and parameter tuning.  
- EDA and preprocessing are essential steps to ensure model reliability.  
