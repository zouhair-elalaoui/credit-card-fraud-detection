# Credit Card Fraud Detection

## Project Overview

This Machine Learning project focuses on detecting fraudulent credit card transactions using data analysis and supervised classification algorithms. It addresses the challenge of identifying rare fraudulent transactions in a highly imbalanced dataset while minimizing false positives.

The project compares several machine learning models to determine which one provides the best balance between fraud detection and prediction reliability.

## Dataset

- **Source:** Kaggle
- **Dataset:** Credit Card Fraud Detection
- **Link:** [Credit Card Fraud Detection on Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Number of transactions:** 284,807
- **Number of features:** 30 input features, plus the target variable
- **Target variable:** `Class` — 0 for legitimate transactions and 1 for fraudulent transactions
- **Fraudulent transactions:** 492 (approximately 0.172% of the dataset)

## Objectives

- Explore and understand the credit card transaction dataset.
- Perform exploratory data analysis (EDA).
- Analyze correlations and outliers.
- Prepare the data for machine learning.
- Address class imbalance using undersampling and SMOTE.
- Train and compare multiple classification algorithms.
- Evaluate models using precision, recall, F1-score, ROC-AUC, and confusion matrices.
- Identify the model that offers the best balance between fraud detection and false positive reduction.

## Methodology

1. **Exploratory Data Analysis:** Examine the distribution of fraudulent and legitimate transactions, analyze correlations, and visualize outliers.
2. **Data Preprocessing:** Select the input features, separate the target variable, and split the dataset into training and testing sets using stratified sampling.
3. **Feature Scaling:** Apply standardization where required by the models.
4. **Class Balancing:** Use Random Undersampling and SMOTE to address the severe imbalance between legitimate and fraudulent transactions.
5. **Model Training:** Implement and evaluate the following classification algorithms:
   - Logistic Regression
   - K-Nearest Neighbors (KNN)
   - Decision Tree
   - Random Forest
   - Support Vector Machine (SVM), including LinearSVC
   - Gaussian Naive Bayes
6. **Model Evaluation:** Compare model performance using classification metrics, cross-validation, confusion matrices, and Precision-Recall curves.

## Results

The **Random Forest** model achieved the strongest overall performance in the project report.

Reported test-set results:

| Metric | Score |
|---|---:|
| Accuracy | 99.95% |
| Precision | 84.69% |
| Recall | 84.69% |
| F1-score | 84.69% |
| ROC-AUC | 96.80% |

The model correctly detected 83 of the 98 fraudulent transactions in the test set, while 15 fraudulent transactions were missed.

Because fraudulent transactions represent only a very small fraction of the dataset, accuracy alone is not sufficient to assess model quality. Precision, recall, F1-score, and ROC-AUC provide a more informative evaluation.

*These results are those reported in the project report and are not a guarantee of performance on real-world transactions.*

## Technologies Used

- **Python** — Programming language
- **Jupyter Notebook** — Interactive development and experimentation
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Machine learning algorithms, preprocessing, model evaluation, and cross-validation
- **imbalanced-learn** — Class imbalance handling with SMOTE and Random Undersampling

## Repository Contents

- `projet_CCFD1_CodeSource.ipynb` — Jupyter Notebook containing the data analysis, preprocessing, model training, and evaluation.
- `Credit_Card_Fraud_Detection.pdf` — Project [Report](Credit_Card_Fraud_Detection.pdf) describing the methodology, experiments, results, and conclusions.
- `requirements.txt` — Python dependencies required to reproduce the project.

## Team Members

- EL ALAOUI SALEH Zouhair
- GHOULAM Nouhaila
- BENSALAH Aya
- PROBI Nouhaila

**Supervisor:** Pr. ATTAOUI Naoual

**Academic Year:** 2025–2026

**Institution:** École Nationale des Sciences Appliquées de Tétouan (ENSA Tétouan)

**Program:** Big Data and Artificial Intelligence

## Limitations and Future Improvements

- The dataset covers a limited period of transactions from September 2013.
- Features V1 to V28 are anonymized PCA components, which limits their direct interpretation.
- The dataset is highly imbalanced, making model evaluation challenging.
- Hyperparameter tuning could further improve model performance.
- Future work could explore more advanced ensemble methods and deep learning approaches.

## Purpose

This project was completed for academic purposes to apply machine learning techniques to credit card fraud detection, explore strategies for handling imbalanced datasets, and evaluate classification models to identify fraudulent transactions more effectively.
