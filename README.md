# 🧮 DATA ANALYTICS LAB - Assignment 6
### **DA5401 A6: Imputation via Regression for Missing Data**

**Name:** Aravindhan Mohanraj  
**Roll No:** DA25S006  

---

## 📂 Repository Overview
**Files included:**
- `DA_Assignment_6.ipynb` — Jupyter Notebook with full solution and visualizations  
- `DA5401 A6 Imputation via Regression.pdf` — Problem statement and task description
- `UCI_Credit_Card.csv` - UCI Credit Card Default Clients Dataset

---

## 🎯 Objective
To apply **linear and non-linear regression** techniques for imputing missing values in the **UCI Credit Card Default Dataset**, and evaluate their effectiveness via a **classification task**.  
The goal is to analyze how imputation strategies impact model performance.

---

## 🧩 Problem Statement
You are working on a **credit risk assessment project** using the UCI Credit Card Default dataset.  
The dataset contains missing values in several important columns, preventing direct use for classification.  
Your tasks are to:
1. Implement three different **imputation strategies**.
2. Train and evaluate a **Logistic Regression** classifier on each resulting dataset.
3. Compare performance across methods to understand the effect of imputation.

---

## ⚙️ Methodology

### **Part A: Data Preparation & Imputation Strategies**
1. **Data Loading:** Load and preprocess the dataset, removing unnecessary columns.  
2. **Introducing Missing Values:** Randomly introduce Missing At Random (MAR) values in selected columns (`BILL_AMT1`, `BILL_AMT4`, `PAY_AMT4`).  
3. **Imputation Techniques:**
   - **A. Median Imputation (Baseline):** Replace missing values with column medians — robust to outliers.  
   - **B. Linear Regression Imputation:** Predict missing values using a Linear Regression model trained on complete data.  
   - **C. Non-Linear Regression Imputation:** Use a non-linear model (e.g., KNN or Decision Tree Regressor) for prediction.  
   - **D. Listwise Deletion:** Drop rows with missing values for comparison.

---

## 🤖 Model Training & Evaluation
For each imputed dataset (A–D):
- Data split into **train/test** sets  
- Standardized features using `StandardScaler`  
- Trained **Logistic Regression** classifier  
- Evaluated using **Accuracy, Precision, Recall, F1-score**, and classification reports  

Performance metrics were compared across all four datasets.

---

## 📈 Key Insights
- Regression-based imputation (Linear & Non-Linear) generally outperforms simple median imputation.  
- Listwise deletion often leads to **data loss** and degraded performance.  
- The **choice of imputation** method significantly affects classifier results.  

---

## 🧠 Notebook Structure (High-Level)
- Introduction & Objective  
- Problem Statement  
- Data Loading & Preprocessing  
- Imputation Strategies (A–C)  
- Model Training and Evaluation (A–D)  
- Comparative Analysis & Discussion  
- Hyperparameter Tuning and Threshold Analysis  
- Final Recommendations  

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate    # Windows
   ```

3. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter
   ```

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook DA_Assignment_6.ipynb
   ```

---

## 👨‍💻 Author
**Aravindhan M** 
**MS Scholar in Data Science and Artficial Intelligence at IIT Madras**  
*Data Engineer | Data Science Enthusiast*

---
