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

# How to Run the Project

Follow the steps below to run the project correctly.

# 1. Requirements
Make sure you have Python 3.x installed.

Install the required libraries:
pip install numpy pandas scikit-learn matplotlib

# 2. Open the Project
Download or clone the repository and open it in Jupyter Notebook or Jupyter Lab.

# 3. Run the Notebooks (In Order)

Run each notebook from top to bottom in the following order:

- Midterm_LoanApproval.ipynb
Trains baseline models using the original dataset
Evaluates accuracy, precision, and ROC-AUC

- Methodology_on_German_Credit_Data.ipynb
Applies the same methodology to the German Credit dataset
Tests model generalization

- LoanApproval_Tuned_Models.ipynb
Performs hyperparameter tuning using GridSearchCV
Compares tuned model performance

- LoanApproval_plus_RF.ipynb
Adds and evaluates a Random Forest classifier

# 4. Expected Output

When running the notebooks, the following outputs are generated:
- Model performance metrics (Accuracy, Precision, ROC-AUC)
- Comparison tables and result visualizations
No additional configuration is required.

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

# Presentation link : https://www.canva.com/design/DAG4s6AaYZs/pcmlWUCdmwAF72XkfBcHZQ/edit?utm_content=DAG4s6AaYZs&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
