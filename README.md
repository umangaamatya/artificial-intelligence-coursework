# Artificial Intelligence Coursework – Student Outcome Prediction

## Project Overview
This project focuses on the development of an Artificial Intelligence application designed to predict student academic outcomes using supervised machine learning techniques. The task is formulated as a **multiclass classification problem**, where the objective is to predict whether a student will **Dropout**, remain **Enrolled**, or **Graduate** at the end of the normal course duration.

The project is based on a real-world educational dataset containing demographic, socioeconomic, academic performance, and macroeconomic indicators. The solution adopts a **multi-model framework**, combining interpretable and performance-oriented classifiers to ensure robustness, fairness, and practical relevance.

---

## Objectives
- To design and implement an AI-driven system for predicting student outcomes.
- To analyze the impact of academic, demographic, and socioeconomic factors on student success.
- To compare multiple supervised learning models using consistent evaluation metrics.
- To address class imbalance and real-world data challenges in educational analytics.

---

## Dataset
The dataset is derived from the [*Predict Students’ Dropout and Academic Success*](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success) dataset and contains:
- **36 input features**
- **3 target classes**: Dropout, Enrolled, Graduate
- No missing values
- Mixed feature types (categorical, continuous, ordinal)

The dataset reflects realistic class imbalance commonly observed in educational systems.

---

## Methodology
The solution follows a structured machine learning pipeline:
1. Data loading and validation
2. Feature preprocessing (encoding and scaling)
3. Stratified dataset splitting
4. Model training and evaluation
5. Comparative analysis of model performance

The following models are implemented:
- **Decision Tree** (baseline and interpretability)
- **Support Vector Machine (SVM)** (robust generalization)
- **XGBoost** (nonlinear interactions and performance)
- Ensemble strategy for combined predictions

---

## Project Structure
``` bash
│
├── data/
│   ├── raw/                 # Original dataset
│   └── processed/           # Preprocessed dataset
│
├── models/
│   └── preprocessing/       # Saved encoders and scalers
│
├── notebooks/
│   └── 01_data_preparation.ipynb
│
├── src/                     # Source code (model training, evaluation)
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Evaluation Metrics
Model performance is assessed using:
- Accuracy
- Precision, Recall, and F1-score (macro and per-class)
- Confusion matrices
- ROC and Precision–Recall curves (one-vs-rest for multiclass)

---

## Ethical Considerations
The project acknowledges ethical concerns related to:
- Student data privacy and anonymization
- Potential bias due to class imbalance or socioeconomic factors
- The impact of misclassification on academic interventions

---

## Usage
All preprocessing and experimentation steps are executed through Jupyter notebooks, with reusable logic progressively refactored into source files. Generated artifacts and trained models are stored outside version control to ensure repository cleanliness.

---

## Module
Artificial Intelligence  
Coursework 2 – Working AI Application