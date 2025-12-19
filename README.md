# Final-Project
Loan Approval Prediction Using Machine Learning

# Authors:

Yoselin Reyes

Yael Sisniega

# Project Overview

This project explores the use of machine learning models to predict loan approval decisions.
The work reproduces an existing research methodology and extends it through:

- Cross-dataset validation
- Hyperparameter tuning
- Model comparison and extension using ensemble methods

The goal is to evaluate model performance, robustness, and generalization across different credit datasets.

# Objectives

Reproduce the baseline loan approval prediction methodology
-Evaluate model performance using standard classification metrics
-Test generalization on a different credit dataset
-Improve performance through hyperparameter tuning
-Extend the model set by incorporating a Random Forest classifier

# Datasets
1. Loan Approval Dataset

Used as the primary dataset to reproduce the original methodology.
It contains applicant financial and demographic information with a binary loan approval outcome.

2. German Credit Dataset

Used to evaluate model generalization on a different population and risk profile.
This dataset presents a more challenging classification problem.

# Methodology
Data Preprocessing

- Handling missing values
- Encoding categorical variables
- Feature scaling where required

# Modeling Approach

The following models were evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest (extension)

# Evaluation Strategy

- 80/20 Train-Test split
- Multiple randomized runs for stability
- Performance metrics:
- Accuracy
- Precision
- ROC-AUC

Project Structure
├── Midterm_LoanApproval.ipynb
│   └── Baseline models and original dataset analysis
│
├── Methodology_on_German_Credit_Data.ipynb
│   └── Cross-dataset validation using German Credit data
│
├── LoanApproval_Tuned_Models.ipynb
│   └── Hyperparameter tuning and performance optimization
│
├── LoanApproval_plus_RF.ipynb
│   └── Random Forest implementation and evaluation
│
├── images/
│   └── Results visualizations and performance comparisons
│
└── README.md

# Results Summary
Baseline Models

- Decision Tree achieved the highest accuracy on the original dataset
- Very high precision, but limited generalization

# Cross-Dataset Validation

- Performance decreased on the German Credit dataset
- Logistic Regression showed better generalization than more complex models

# Tuned Models

- Hyperparameter tuning improved stability and reduced overfitting
- Decision Tree performance improved slightly with better control of complexity

# Random Forest Extension

- Achieved the highest ROC-AUC score
- Provided the most stable and robust performance
- Demonstrated the benefits of ensemble learning

# Key Insights

- High accuracy on a single dataset does not guarantee generalization
- Model performance is highly dependent on data characteristics
- Hyperparameter tuning is essential for reliable evaluation
- Ensemble methods improve robustness and predictive stability

# Limitations and Future Work

- Address class imbalance more explicitly
- Explore feature selection and dimensionality reduction
- Evaluate additional datasets
- Implement cost-sensitive and fairness-aware learning

# Conclusion

This project successfully reproduces and extends an existing loan approval prediction methodology.
By introducing cross-dataset validation, hyperparameter tuning, and Random Forest models, the work highlights the importance of robustness and generalization in real-world machine learning applications.
