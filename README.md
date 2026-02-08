# Skin Cancer ML Risk Prediction

An end-to-end machine learning project for **skin cancer classification** based on structured clinical data.  
The project performs detailed data analysis, preprocessing, class imbalance correction, and model comparison, with **XGBoost emerging as the best-performing model**.

This repository includes both the **dataset** and the **fully refactored analysis notebook**, ensuring reproducibility.

---

## 📌 Project Motivation

Skin cancer datasets present several real-world challenges:
- Mixed numerical and categorical clinical features
- Missing values
- Strong class imbalance between benign and malignant cases
- Non-linear feature interactions

This project addresses these challenges through a systematic ML workflow and evaluates multiple models to identify the most effective approach.

---

## 📂 Repository Contents

```text
.
├── Data/
│   └── skin cancer data_transformed_2_classes.csv
├── skin-cancer-ml-risk-prediction.ipynb
├── README.md
````

The dataset is already transformed into **binary classes** and is ready for direct modeling.

---

## 📊 Dataset Overview

* **Type:** Structured clinical data
* **Target Variable:** Skin cancer diagnosis

  * `0` → Benign
  * `1` → Malignant
* **Features:**

  * Numerical clinical measurements
  * Encoded categorical attributes
* **Class Distribution:** Imbalanced (addressed explicitly in the pipeline)

Basic statistics, distributions, and feature relationships are explored directly in the notebook.

---

## 🧠 Methodology

### 1. Data Exploration

* Dataset structure and summary statistics
* Target class distribution analysis
* Numerical and categorical feature inspection

### 2. Missing Data Handling

* Missing value quantification
* Type-aware imputation strategies

### 3. Feature Engineering

* Categorical encoding
* Feature preparation for tree-based models

### 4. Feature Scaling

* Applied where required for fair model comparison

### 5. Train/Test Split

* Stratified splitting to preserve class proportions

### 6. Class Imbalance Handling

* **SMOTE-ENN** hybrid resampling technique

### 7. Model Training & Comparison

* Multiple machine learning models evaluated
* Performance compared using standard classification metrics

---

## 🏆 Final Model: XGBoost

After systematic evaluation, **XGBoost outperformed all other models**, achieving the best balance between:

* Precision
* Recall (especially for the malignant class)
* F1-score
* Overall robustness on imbalanced data

As a result, **XGBoost is selected as the final and recommended model** for this dataset.

All reported metrics and evaluation details are available in the notebook.

---

## 🛠️ Tech Stack

* **Python**
* **Pandas / NumPy**
* **Matplotlib / Seaborn**
* **Scikit-learn**
* **XGBoost**
* **Imbalanced-learn (SMOTE-ENN)**
* **Dython** (categorical association analysis)

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/skin-cancer-xgboost-classification.git
   cd skin-cancer-xgboost-classification
   ```

2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn dython
   ```

3. Run the notebook:

   ```bash
   jupyter notebook refactored_skin_cancer_analysis_latest.ipynb
   ```

---

## ⚠️ Disclaimer

This project is intended **for research and educational purposes only**.
It is **not a medical diagnostic tool** and must not be used for clinical decision-making.

---

## 📜 License

MIT License

---

## 🙌 Contributions

Contributions, discussions, and extensions are welcome.
Feel free to fork the repository and build upon the pipeline.


