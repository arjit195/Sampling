# Credit Card Fraud Detection Project

## Overview
Credit card fraud detection is a crucial task, especially when dealing with highly imbalanced datasets that can negatively impact the performance of machine learning models. This project addresses these challenges by:
1. Balancing the dataset using the Synthetic Minority Oversampling Technique (SMOTE).
2. Creating five distinct samples of varying sizes using multiple sampling techniques.
3. Training five different machine learning models on these samples.
4. Comparing the performance of these models to determine the most effective sampling technique for each.

---

## Dataset Details
The dataset used is `Creditcard_data.csv`, containing the following key features:
- **Features (V1 to V28):** Principal components derived from transaction data.
- **Time:** Time elapsed (in seconds) between transactions.
- **Amount:** The monetary value of the transaction.
- **Class:** Fraud label, where:
  - `0` represents legitimate transactions.
  - `1` represents fraudulent transactions.

### Class Imbalance
The dataset is highly imbalanced:
- **Class 0 (Legitimate):** 98.83% of transactions.
- **Class 1 (Fraudulent):** 1.17% of transactions.

---

## Sampling Techniques
To address class imbalance, the following sampling methods were employed:
1. **Random Sampling:** Randomly selects a subset of the data.
2. **Stratified Sampling:** Ensures class proportions are preserved within the samples.
3. **Systematic Sampling:** Selects every nth record from the dataset.
4. **Cluster Sampling:** Divides the dataset into clusters and selects entire clusters.
5. **Oversampling:** Increases the representation of the minority class using SMOTE.

---

## Machine Learning Models
Five machine learning models were implemented for this project:
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine (SVM)
5. Gradient Boosting

---

## Observations
The following insights were derived based on model performance:
1. Logistic Regression performs best with Stratified Sampling and Oversampling.
2. Decision Tree works best with Stratified Sampling.
3. Random Forest achieves the best results with Oversampling.
4. SVM performs optimally with Oversampling.
5. Gradient Boosting works best with Stratified Sampling.

---

## Conclusion
This project demonstrates the importance of sampling techniques in handling imbalanced datasets and highlights how model performance varies based on the sampling approach used. By leveraging the insights from this analysis, organizations can enhance their ability to detect credit card fraud effectively and minimize losses.
