# 🏦 PRODIGY_DS_03 – Bank Marketing Decision Tree

## 📌 Overview
A Machine Learning project that predicts whether a customer will subscribe to a **Bank Term Deposit** using a **Decision Tree Classifier**.  
The project includes **EDA, Data Preprocessing, Model Training, and Evaluation** on the UCI Bank Marketing Dataset.

---

## 📊 Dataset
- **Source:** UCI Bank Marketing Dataset  
- **Records:** 45,211 Clients  
- **Features:** 16 Inputs + 1 Target  
- **Target:** `y` (Yes / No)  
- **Class Imbalance:** 11.7% Yes | 88.3% No  

**Key Features:** age, job, education, duration, campaign, pdays, poutcome

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## ⚙️ Methodology
- Data Cleaning & EDA  
- Label Encoding (Categorical Features)  
- Outlier Removal (IQR – `duration`)  
- Train/Test Split (75/25)  
- Decision Tree Classifier (Gini)

---

## 📈 Results

| Metric | Score |
|--------|-------|
| Accuracy | **89.2%** |
| ROC-AUC | **0.91** |
| Precision (Yes) | **0.58** |
| Recall (Yes) | **0.52** |

---

## 🔑 Important Features
- **pdays** – Last contact recency  
- **duration** – Call length  
- **age** – 30–50 most responsive  
- **poutcome** – Previous success  
- **campaign** – Optimal 1–3 contacts  

---

## ▶️ How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
git clone https://github.com/YOUR_USERNAME/PRODIGY_DS_03.git
cd PRODIGY_DS_03
jupyter notebook
