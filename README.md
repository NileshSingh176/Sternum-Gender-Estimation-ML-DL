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

⚠️ Dataset is private due to institutional restrictions.

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

### Best ML Performance
- Accuracy: **83.33%**  
- Achieved using MinMaxScaler  
- Strong precision across multiple classifiers  

**Machine Learning Notebooks:**  
- [StandardScaler.ipynb](Machine_Learning/StandardScaler.ipynb)  
- [MinMaxScaler.ipynb](Machine_Learning/MinMaxScaler.ipynb)  

---

# 🧠 Deep Learning Implementation

A fully connected CNN model for structured data classification. Two preprocessing techniques were tested:

### CNN + MinMaxScaler
- Test Accuracy: **83.33%**  
- Test Loss: 0.3459

### CNN + StandardScaler
- Test Accuracy: **83.33%**  
- Test Loss: 0.4668

MinMaxScaler showed better optimization stability with lower loss.

**Deep Learning Notebooks:**  
- [CNN_Standard_Scaler.ipynb](Deep_Learning/CNN_Standard_Scaler.ipynb)  
- [CNN_Min__Max_Scaler.ipynb](Deep_Learning/CNN_Min__Max_Scaler.ipynb)  

---

# 📊 Performance Comparison

| Approach | Accuracy | Observation |
|-----------|----------|------------|
| Machine Learning | 83.33% | Stable across multiple models |
| Deep Learning | 83.33% | Lower loss with MinMaxScaler |

Both classical ML and Deep Learning approaches performed competitively.

---

## 📁 Repository Structure

Sternum-Gender-Estimation-ML-DL/
│
├── Machine_Learning/       # Notebooks for classical ML experiments
│   ├── StandardScaler.ipynb
│   └── MinMaxScaler.ipynb
│
├── Deep_Learning/          # Notebooks for CNN-based deep learning experiments
│   ├── CNN_Standard_Scaler.ipynb
│   └── CNN_Min__Max_Scaler.ipynb
│
├── data/                   # Dataset used for experiments
│   └── hospital.csv
│
├── docs/                   # Thesis charts and additional documentation
│   └── thesis master chart.xlsx
│
├── visuals/                # Generated plots and visual outputs
│   └── normal.png
│
├── README.md               # Project overview and instructions
├── LICENSE                 # License file
├── .gitignore              # Git ignore rules
└── requirements.txt        # Python dependencies
