# 🚀 KDD Cup 1999 Intrusion Detection System
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)
![Colab](https://img.shields.io/badge/Google%20Colab-Notebook-yellow?logo=googlecolab)
![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-blue?logo=kaggle)

### 🔥 ML Benchmarking of 15+ Algorithms | Achieving >99.9% Accuracy

---

## 📌 Overview

This project presents a **comprehensive benchmarking of 15+ Machine Learning algorithms** on the **KDD Cup 1999 dataset** for Network Intrusion Detection.

The goal is to:

* Compare multiple ML models under a **consistent pipeline**
* Evaluate performance across **different train-test splits**
* Identify the **most robust and scalable model**

---

## ⚡ Key Highlights

* ✅ Benchmarked **15+ ML Algorithms**
* ✅ Evaluated across **3 test sizes (0.2, 0.4, 0.6)**
* ✅ Achieved **>99.9% accuracy**
* ✅ Built using **Google Colab**
* ✅ Implemented **end-to-end ML pipeline**
* ✅ Real-world dataset (Cybersecurity domain)

---

## 🧠 Models Implemented

### 🔥 Ensemble Models

* Random Forest (RFC)
* LightGBM (LGBM)
* XGBoost (XGB)
* CatBoost
* Gradient Boosting (GBC)
* AdaBoost

### 📊 Classical ML Models

* Decision Tree (DTC)
* K-Nearest Neighbors (KNN)
* Kernel SVM (KSVM)
* Linear SVM (LSVM)
* Logistic Regression (LR)

### 📉 Statistical Models

* LDA (Linear Discriminant Analysis)
* QDA (Quadratic Discriminant Analysis)
* Naive Bayes (NB)

### 🧠 Neural Network

* MLP Classifier

---

## 📊 Results Summary

| Model     | 0.2     | 0.4     | 0.6     |
| --------- | ------- | ------- | ------- |
| RFC       | 0.99957 | 0.99955 | 0.99949 |
| LGBM      | 0.99953 | 0.99954 | 0.99940 |
| CatBoost  | 0.99933 | 0.99930 | 0.99925 |
| XGB       | 0.99931 | 0.99931 | 0.99926 |
| KNN       | 0.99948 | 0.99941 | 0.99931 |
| MLP       | 0.99915 | 0.99922 | 0.99928 |
| KSVM      | 0.99880 | 0.99840 | 0.99833 |
| GBC       | 0.99880 | 0.99896 | 0.99897 |
| ADA Boost | 0.99218 | 0.99227 | 0.99113 |
| QDA       | 0.98377 | 0.98344 | 0.98369 |
| LDA       | 0.98723 | 0.98735 | 0.98725 |
| LR        | 0.98710 | 0.98732 | 0.98701 |
| LSVM      | 0.98720 | 0.98741 | 0.98717 |
| DTC       | 0.99928 | 0.99927 | 0.99910 |
| NB        | 0.96975 | 0.93547 | 0.93136 |

<img width="1293" height="609" alt="Accuracy Comparison Chart" src="https://github.com/user-attachments/assets/4150fdf3-9bc9-4947-932c-60f67545687b" />

---

## 🏆 Key Insights

* 🥇 **Best Model:** Random Forest (Highest accuracy + stability)
* 🔥 **Top Performers:** LightGBM, CatBoost, XGBoost
* 🌲 **Tree-based models dominate tabular data**
* ⚠️ **Naive Bayes performed worst** due to independence assumption
* ⚡ **SVM showed high accuracy but poor scalability**
* 🧠 **MLP captured non-linear patterns effectively**

---

## 📂 Project Structure

```bash
KddCup-IDS-ML-Benchmark/
│
├── notebooks/
│   ├── CatBoost.ipynb
│   ├── DTC.ipynb
│   ├── GBC.ipynb
│   ├── KNN.ipynb
│   ├── KSVM.ipynb
│   ├── LSVM.ipynb
│   ├── LDA.ipynb
│   ├── QDA.ipynb
│   ├── LR.ipynb
│   ├── MLP.ipynb
│   ├── NB.ipynb
│   ├── RFC.ipynb
│   ├── XGB.ipynb
│   ├── LGBM.ipynb
│   ├── ADA Boost.ipynb
│
├── outputs/
│   ├── comparison_table.png
│   ├── confusion_matrices/
│
├── README.md
└── requirements.txt
```

---

## 📂 Dataset

[![Kaggle Dataset](https://img.shields.io/badge/Kaggle-KDD%20Cup%201999-blue?logo=kaggle)](https://www.kaggle.com/datasets/kavl31/kdd-cup-1999-data)

The dataset used in this project is the **KDD Cup 1999 Intrusion Detection Dataset**, widely used for evaluating machine learning models in cybersecurity.

### 🔗 Access Dataset

* 📊 Kaggle: https://www.kaggle.com/datasets/kavl31/kdd-cup-1999-data

---

## 📌 Dataset Details

* Total Records: ~4.9 Million (full dataset)
* Features: 41 input features + 1 target
* Task: Binary Classification (Normal vs Attack)
* Domain: Network Intrusion Detection

---

## ⚙️ Data Preprocessing

* Converted multi-class attacks → **Binary classification**
* One-hot encoding for categorical features:

  * protocol_type
  * service
  * flag
* Feature scaling using StandardScaler
* Dimensionality reduction using PCA

---

## 🚀 Reproducibility

To run this project:

1. Open any notebook from `notebooks/`
2. Mount Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

3. Load dataset:

```python
df = pd.read_csv('/content/drive/MyDrive/KddCup/data/kdd_clean.csv')
```

---

💡 *Dataset is not included in this repository due to GitHub file size limitations.*
---

## ⚙️ Tech Stack

* Python 🐍
* Scikit-learn
* XGBoost
* LightGBM
* CatBoost
* Google Colab

---

## 📈 Future Improvements

* 🔍 Hyperparameter tuning
* 📊 ROC-AUC comparison
* 🧠 SHAP explainability
* 🚀 Model deployment (Streamlit/Flask)

---

## 🧠 Key Learning

> Tree-based ensemble models outperform traditional ML models in large-scale tabular intrusion detection tasks.

---

## 👨‍💻 Author

**Arindam Karmakar**

---

## ⭐ Support

If you found this useful:

👉 ⭐ Star the repo
👉 🍴 Fork it
👉 🔗 Share it

---

## 🚀 Bonus

This project demonstrates:

* Real-world ML pipeline
* Model benchmarking
* Performance analysis
* Industry-level experimentation
