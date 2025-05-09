# Credit Risk Analysis Report
**Creator**: Angelina Murdock  
**Date**: May 2025

## Overview of the Analysis
The purpose of this analysis was to train and evaluate a machine learning model that can predict loan risk and assess the creditworthiness of borrowers.
The dataset consisted of historical financial data from a peer-to-peer lending platform. The target variable, `loan_status`, indicated whether a loan was considered high risk (1) or healthy (0). The dataset was imbalanced, with significantly more healthy loans than high-risk loans.
The machine learning process involved preprocessing the data, splitting it into training and testing sets, training a `LogisticRegression` model, and evaluating its performance using a **confusion matrix** and **classification report**.

## Table of contents
- [Overview](#overview)
- [Results](#results)
- [Summary](#summary)
- [Installation](#installation)
- [Resources](#resources)

## Results
**Logistic Regression:**
- Accuracy: 0.99 
- Precision (Healthy): 1.00
- Recall (Healthy): 1.00
- Precision (High-Risk): 0.87
- Recall (High-Risk): 0.95

## Summary
The Logistic Regression model performed exceptionally well on the imbalanced dataset. It achieved **99% accuracy**, with a **precision of 0.87** and **recall of 0.95** for high-risk loans. The confusion matrix shows that the model correctly identified 593 high-risk loans, while misclassifying only 32 as low risk. This demonstrates a strong ability to detect borrowers who pose a higher default risk. However, there were still some false negatives and false positives.
The **classification report** supports these findings, with an **F1-score of 0.91** for the high-risk class and nearly perfect scores for the healthy class. Despite the class imbalance, the model maintained balanced performance, making it suitable for real-world credit risk assessment.

### **Recommendation:**
The model performs well in identifying high-risk loans, making it a strong choice for the company’s credit risk strategy. It effectively balances overall accuracy with the ability to detect risky borrowers. To maintain its reliability, ongoing monitoring and periodic updates with new data are recommended.

## Installation
**1. Clone the Repository:**
```bash
git clone https://github.com/Angelinamurdock/credit-risk-classification.git
```

**2. Open the Project**:
- Open the `credit_risk_classification.ipynb` Jupyter Notebook File to interact with the project. 

**3. View the analysis:** 
- Open the `credit-risk-analysis-report.md` file.

**Requirements include:**
- pandas
- sklearn
- numpy
- jupyter

## Resources
- **DU Bootcamp Module 20:** Used challenge files and class materials from the bootcamp.
- **ChatGPT:** Assisted with code explanations and debugging.