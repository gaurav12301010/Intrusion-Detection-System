# CICIDS2017 Intrusion Detection — ML Pipeline

## Overview

This project builds a complete Machine Learning pipeline for intrusion detection using the **CICIDS2017 dataset**.
The goal is to classify network traffic into **benign vs multiple attack types** using supervised learning.

---

## Dataset

* **Name:** CICIDS2017 (Canadian Institute for Cybersecurity)
* **Size:** ~2.8 million records (sampled for efficiency)
* **Features:** 78 numerical features + 1 label
* **Classes:**

  * Benign
  * DoS / DDoS
  * Brute Force
  * Heartbleed
  * Botnet
  * Web Attacks
  * Infiltration

 Due to large size, **stratified sampling** is used to maintain class distribution.

---

## Pipeline

The notebook follows a full ML workflow:

```
Data Loading
→ Stratified Sampling
→ Exploratory Data Analysis (EDA)
→ Feature Engineering
→ Data Preprocessing
→ Train / Validation / Test Split
→ Model Training
→ Cross Validation
→ Evaluation & Analysis
```

---

## ⚙️ Features Implemented

* Handling large-scale dataset efficiently
* Class imbalance handling via stratified sampling
* Data cleaning & preprocessing
* Feature scaling & transformation
* Model training with evaluation metrics
* Cross-validation for robustness
* Visualization for EDA & results

---

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## How to Run

1. Download CICIDS2017 dataset (CSV files)
2. Update dataset path in notebook
3. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. Run the notebook:

   ```bash
   jupyter notebook CICIDS2017_Analysis_complete.ipynb
   ```

---

## Notes

* Adjust `SAMPLE_SIZE` based on your system RAM
* Full dataset training requires high memory (16GB+ recommended)
* Sampling preserves real-world class distribution

---

## Future Improvements

* Deep Learning models (LSTM, Autoencoders)
* Real-time intrusion detection system
* Deployment with FastAPI
* Integration with network monitoring tools

---

##  Author

Developed as part of ML/IDS experimentation project.

---
