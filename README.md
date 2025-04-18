# churn-prediction
# 📊 Customer Churn Prediction – Telecom Dataset

This project aims to predict whether a telecom customer will **churn (leave)** using machine learning classification techniques. The model is trained on historical customer data and provides insights into what factors lead to churn, helping businesses retain customers effectively.

---

## 📌 Problem Statement

**Goal:**  
Build a classification model that accurately predicts whether a customer will churn.

**Churn** is defined as a customer who discontinues the service.

---

## 🧾 Dataset Description

- 📁 **File Name:** `5. Classify Customer Churn.csv`
- 🧮 **Rows:** 7043
- 🧾 **Columns:** 21
- 🎯 **Target Variable:** `Churn` (1 = churned, 0 = not churned)

**Features include:**
- Categorical: gender, Partner, Dependents, PhoneService, etc.
- Numerical: tenure, MonthlyCharges, TotalCharges

✅ No missing values  
✅ Cleaned and encoded before model training

---

## 🧠 ML Pipeline Used

1. **Exploratory Data Analysis (EDA)**
   - Dataset info, null check, dtype inspection
   - Class imbalance checked

2. **Preprocessing**
   - Converted `TotalCharges` to numeric
   - Label encoding for target
   - One-hot encoding for categorical features

3. **Model Building**
   - Used `RandomForestClassifier`
   - 80-20 train-test split
   - GridSearchCV for hyperparameter tuning

4. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report
   - Feature Importance Plot

---

## 📈 Results

- ✅ **Accuracy Score:** `~79.7%`
- 📊 **Classification Report:**

| Metric     | Churn = 0 | Churn = 1 |
|------------|-----------|-----------|
| Precision  | 0.83      | 0.66      |
| Recall     | 0.91      | 0.48      |
| F1-Score   | 0.87      | 0.56      |

- 🧮 **Confusion Matrix:**

- 🌟 **Top 10 Important Features:**
  - Tenure
  - MonthlyCharges
  - TotalCharges
  - CustomerID
  - Contract
  - OnlineSecurity
  - PaymentMethod
  - TechSupport
  - OnlineBackup
  - Gender

*(See feature importance bar chart in screenshots)*

---

## 🖼️ Screenshots

### 📋 Dataset Info + Missing Values Check  
![Dataset Info](./images/dataset_info.png)

### 🧪 Model Accuracy and Feature Importance  
![Model Output](./images/model_output.png)

---

## ⚙️ Technologies Used

| Tool/Library     | Purpose                    |
|------------------|-----------------------------|
| Python           | Core Programming            |
| Pandas, Numpy    | Data manipulation           |
| Matplotlib, Seaborn | Visualization            |
| Scikit-learn     | ML model, metrics, pipeline |
| Google Colab     | Execution environment       |

---

## 🚀 How to Run This Project

### 📍 Google Colab

1. Open Google Colab
2. Upload the dataset `.csv` file
3. Copy-paste the provided code blocks
4. Run each cell step-by-step

### 📍 Local (Optional)

```bash
pip install pandas numpy matplotlib seaborn scikit-learn

---

### ✅ Next Steps:
1. Want me to generate this as a downloadable `.md` or `.pdf`?
2. Need help setting up `/images` folder for GitHub screenshots?
3. Want this content added directly to your GitHub repo?

Let me know how you’d like to proceed!
