# ds-loan-default-prediction
Source: Kaggle – Loan Default Dataset
Contains demographic and financial attributes of borrowers along with a binary target indicating loan default.

Methodology
1. Exploratory Data Analysis

Variable distributions

Missing value inspection

Correlation patterns

Basic target comparison across key features

2. Feature Engineering

Imputation (mean for numerical, most frequent for categorical)

Standardization of numerical variables

One-hot encoding of categorical variables

Pipeline-based preprocessing to prevent leakage

3. Modeling

Models evaluated:

Logistic Regression

XGBoost

Random Forest

The pipeline integrates preprocessing and the model to ensure consistent transformations during training and evaluation.


4. Results
| Model               | ROC_AUC |
| ------------------- | ------- |
| Logistic Regression | 0.847   |
| Random Forest       | 1.000   |
| XGBoost             | 1.000   |

Tree-based models separate the classes perfectly on the test split. This can indicate true separability or potential sensitivity to data partitioning. Cross-validation is recommended for further confirmation.



