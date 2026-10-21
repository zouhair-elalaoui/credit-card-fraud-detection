# Credit Card Fraud Detection

## Overview

This project explores the use of machine learning to detect fraudulent credit card transactions and distinguish them from legitimate payments.

## How It Works

1. **Data Preprocessing** — Prepare transaction data for model training.
2. **Model Training** — Train and compare machine learning models for fraud detection.
3. **Evaluation** — Assess model performance using classification metrics suited to an imbalanced dataset.
4. **Prediction** — Use the trained model to identify potentially fraudulent transactions.

## Results & Performance

**Random Forest** achieved the strongest overall performance in the project report.

| Metric | Score |
|:--|--:|
| Accuracy | 99.95% |
| Precision | 84.69% |
| Recall | 84.69% |
| F1-score | 84.69% |
| ROC-AUC | 96.80% |

On the test set, the model detected **83 out of 98 fraudulent transactions**, while missing 15.

Since fraudulent transactions represent a very small fraction of the dataset, accuracy alone is not sufficient to evaluate model quality. Precision, recall, F1-score, and ROC-AUC provide a more informative assessment.

These results are based on the project report and do not guarantee performance on real-world transactions.

For the complete methodology, model comparison, and detailed results, see the [**Project Report**](Credit_Card_Fraud_Detection.pdf).

## Team Members

- EL ALAOUI SALEH Zouhair
- GHOULAM Nouhaila
- BENSALAH Aya
- PROBI Nouhaila

**Supervisor:** Pr. ATTAOUI Naoual

**Academic Year:** 2025–2026

## Purpose

This project was completed for academic purposes to apply machine learning techniques to credit card fraud detection, explore strategies for handling imbalanced datasets, and evaluate classification models to identify fraudulent transactions more effectively.
