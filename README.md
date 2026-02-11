An end-to-end forensic AI system that automates gender estimation from sternum anatomical measurements using both classical machine learning and deep learning techniques.

# 🦴 Gender Estimation Using Sternum Measurements
### (Machine Learning + Deep Learning Approach | Forensic AI Project)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-green)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-red)
![Domain](https://img.shields.io/badge/Domain-Forensic%20Anthropology-orange)

---

## 📌 Project Overview

This project focuses on automated gender estimation using sternum bone anatomical measurements. The system integrates both classical Machine Learning algorithms and Deep Learning models to predict gender from structured medical data.

The dataset was obtained from a hospital under restricted academic usage and contains real anatomical sternum measurements.

---

## 🧾 Dataset Description

- Total Samples: 150
- Features: 12 anatomical measurements
- Target Variable: Gender (Male / Female)

### Key Anatomical Features:

- Manubrium Length (ML)
- Mesosternum Length (BL)
- Manubrium Width (MW)
- Sternum Width 1 (SW1)
- Sternum Width 2 (SW2)
- Total Sternum Length (TSL)
- Sternal Index (M/B × 100)
- Sternal Area
- Age

These measurements are based on forensic anatomical principles including Hyrtl’s Law.

⚠️ Due to privacy and institutional restrictions, the dataset is not publicly shared.

---

# 🛠 Methodology

## 1️⃣ Data Preprocessing
- Handling structured measurement data
- Feature scaling using:
  - MinMaxScaler
  - StandardScaler
- Train-test split

---

# 🤖 Machine Learning Implementation

Multiple classification algorithms were evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- AdaBoost

### Best ML Performance:
- Accuracy: **83.33%**
- Achieved using MinMaxScaler
- Strong precision across multiple classifiers

---

# 🧠 Deep Learning Implementation

A fully connected neural network was implemented for structured data classification.

Two preprocessing techniques were tested:

### CNN + MinMaxScaler
- Test Accuracy: **83.33%**
- Test Loss: 0.3459

### CNN + StandardScaler
- Test Accuracy: **83.33%**
- Test Loss: 0.4668

MinMaxScaler demonstrated better optimization stability with lower loss.

---

# 📊 Performance Comparison

| Approach | Accuracy | Observation |
|-----------|----------|------------|
| Machine Learning | 83.33% | Stable across multiple models |
| Deep Learning | 83.33% | Lower loss with MinMaxScaler |

Both classical ML and Deep Learning approaches performed competitively.

---


## 📁 Repository Structure

```
Sternum-Gender-Estimation-ML-DL/
│
├── notebooks/
│   ├── ML_MinMaxScaler.ipynb
│   ├── ML_StandardScaler.ipynb
│   ├── DL_MinMaxScaler.ipynb
│   └── DL_StandardScaler.ipynb
│
├── models/
│   ├── best_ml_model.pkl
│   └── best_dl_model.h5
│
├── requirements.txt
└── README.md
```

---

# 🔬 Key Insights

- Feature scaling significantly impacts model performance.
- MinMaxScaler outperformed StandardScaler in both ML and DL pipelines.
- Structured anatomical measurements can effectively predict gender.
- Classical ML models can perform comparably to deep learning in small structured datasets.

---

# 🚀 Why This Project is Strong

✔ Real hospital-based dataset  
✔ Forensic anthropology application  
✔ Multiple ML algorithm comparison  
✔ Preprocessing experimentation  
✔ Deep Learning implementation  
✔ Performance evaluation and analysis  

---

# 🌍 Real-World Applications

- Forensic investigations
- Disaster victim identification
- Skeletal remains analysis
- Medico-legal cases

---

# 👨‍💻 Author

Nilesh Singh  
B.Tech CSE (AI & ML)  
Machine Learning | Deep Learning | Medical AI  

LinkedIn: https://www.linkedin.com/in/nilesh-singh-991a86290/

---
