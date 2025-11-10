# 🏦 CrediCheck: Loan Approval Analysis and Prediction System

## 📘 About the Project
The **CrediCheck** project implements a classification system to predict the **loan approval status (`loan_status`)** based on various financial and demographic characteristics of applicants.

We utilized a **Deep Neural Network (DNN)** model built with **TensorFlow/Keras** to maximize **accuracy** and **recall** in identifying loans that should be approved or rejected.

---

## ⚙️ Technical Highlights
- **Deep Learning:** Neural Networks (Keras/TensorFlow) for high predictive performance.  
- **Class Balancing:** Application of **SMOTE (Synthetic Minority Over-sampling Technique)** to mitigate class imbalance.  
- **Focused Metrics:** The model tracks **Recall**, **Precision**, and **Accuracy**, which are crucial for financial classification.

---

## 🧠 Technologies Used

| Category | Library | Notable Version | Main Purpose |
|-----------|----------|------------------|---------------|
| Data Science | `pandas` | 2.0.3 | Dataset manipulation and loading |
| Machine Learning | `scikit-learn` | – | Data preprocessing and splitting |
| Deep Learning | `tensorflow` | 2.16.1 | Building and training the Neural Network |
| Balancing | `imblearn (SMOTE)` | – | Oversampling the minority class |
| Visualization | `matplotlib`, `seaborn` | – | Generating plots, Confusion Matrix, ROC Curve |

---

## 📊 Methodology

The workflow in the **CrediCheck.ipynb** notebook follows these steps:

1. **Data Loading and Cleaning:** Load `loan_approval_dataset.csv` and drop irrelevant columns like `loan_id` and `self_employed`.  
2. **Preprocessing:**  
   - Standardize numerical variables using `StandardScaler`.  
   - One-Hot Encode categorical variables like `education`.  
   - Encode target variable (`loan_status`) with `LabelEncoder`.  
3. **Class Balancing:** Apply **SMOTE** to handle class imbalance.  
4. **Model Training:** Train a Neural Network for 100–150 epochs with validation monitoring.  
5. **Evaluation:** Assess model with **Confusion Matrix**, **Accuracy**, **Precision**, **Recall**, and **ROC Curve**.

---

## 🚀 How to Run the Project

### Prerequisites
Make sure you have **Python** installed (compatible with the library versions below).

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/CrediCheck.git
cd CrediCheck

### 2️⃣ Install Dependencies
```bash
Create a virtual environment (optional) and install the libraries:
pip install pandas==2.0.3 tensorflow==2.16.1 scikit-learn
pip install scikeras imblearn matplotlib seaborn

### 3️⃣ Run the Notebook
```bash
Ensure the dataset file loan_approval_dataset.csv is in the same folder as the notebook.
Then execute it using Jupyter Notebook, JupyterLab, or Google Colab:
jupyter notebook CrediCheck.ipynb
