# Credit Risk Prediction to Improve Loan Approval

## Project Overview
This project (March 2024) aims to enhance loan approval processes by developing a machine learning model to predict credit risk. The model identifies key predictors of loan default, enabling banks to make informed lending decisions with improved accuracy and efficiency.

## Objectives
- Select relevant features to predict credit risk while eliminating multicollinearity.  
- Evaluate multiple machine learning models to identify the best-performing algorithm.  
- Optimize the chosen model to achieve high accuracy, precision, and recall for reliable predictions.  

## Dataset
The dataset (e.g., **case_study1.xlsx**, **case_study2.xlsx**) contains loan and credit-related data.  
Specific details about features and target variables are available in the `Credit_Risk_Modelling.ipynb` notebook.

## Methodology

### Feature Selection
- **Chi-square Test**: Identified significant categorical predictors associated with loan default.  
- **Variance Inflation Factor (VIF)**: Detected and removed multicollinearity among features to ensure model stability.  
- **ANOVA**: Assessed numerical features to select those with significant variance related to the target variable.  

### Model Evaluation
Models evaluated:
- Decision Tree  
- Logistic Regression  
- Random Forest  
- XGBoost  

**Metrics Used**: Accuracy, Precision, Recall (and possibly AUROC, F1-score).  

### Model Optimization
- **Best Model**: XGBoost  
- **Hyperparameter tuning** applied, achieving:  
  - Accuracy: **82%**  
  - Precision & Recall: Balanced and robust, ensuring reliable predictions for both default and non-default cases.  


## Results
- **Feature Selection**: Successfully identified key predictors while eliminating multicollinearity, improving model interpretability.  
- **Model Performance**: XGBoost outperformed other models, achieving **82% accuracy** with strong precision and recall.  
- **Impact**: Provides a reliable tool for banks to assess credit risk, potentially reducing default rates and optimizing loan approvals.  

## Requirements
Install dependencies:
```bash
pip install pandas numpy scikit-learn xgboost statsmodels scipy


