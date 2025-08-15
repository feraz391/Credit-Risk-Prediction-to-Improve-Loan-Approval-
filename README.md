Credit Risk Prediction to Improve Loan Approval
Project Overview
This project, completed in March 2024, aims to enhance loan approval processes by developing a machine learning model to predict credit risk. The model identifies key predictors of loan default, enabling banks to make informed lending decisions with improved accuracy and efficiency.
Objectives

Select relevant features to predict credit risk while eliminating multicollinearity.
Evaluate multiple machine learning models to identify the best-performing algorithm.
Optimize the chosen model to achieve high accuracy, precision, and recall for reliable predictions.

Dataset
The dataset (e.g., case_study1.xlsx, case_study2.xlsx) contains loan and credit-related data. Specific details about features and target variables are available in the Credit_Risk_Modelling.ipynb notebook.
Methodology
Feature Selection

Chi-square Test: Identified significant categorical predictors associated with loan default.
Variance Inflation Factor (VIF): Detected and removed multicollinearity among features to ensure model stability.
ANOVA: Assessed numerical features to select those with significant variance related to the target variable.

Model Evaluation
The following models were evaluated:

Decision Tree
Logistic Regression
Random Forest
XGBoost

Metrics used: Accuracy, Precision, Recall, and potentially others (e.g., AUROC, F1-score).
Model Optimization

XGBoost was selected as the best-performing model.
Hyperparameter tuning was performed to optimize XGBoost, achieving:
Accuracy: 82%
Precision and Recall: Balanced and robust, ensuring reliable predictions for both default and non-default cases.



Repository Structure

Credit_Risk_Modelling.ipynb: Jupyter Notebook containing the full code for data preprocessing, feature selection, model training, evaluation, and optimization.
case_study1.xlsx, case_study2.xlsx: Datasets used for analysis (ensure access to these files for replication).
README.md: This file, providing an overview of the project.

Results

Feature Selection: Successfully identified key predictors while eliminating multicollinearity, improving model interpretability.
Model Performance: XGBoost outperformed other models, achieving 82% accuracy with strong precision and recall after hyperparameter tuning.
Impact: The model provides a reliable tool for banks to assess credit risk, potentially reducing default rates and optimizing loan approval processes.

Requirements
To run the notebook, install the following dependencies:

Python 3.x
Jupyter Notebook
Libraries: pandas, numpy, scikit-learn, xgboost, statsmodels, scipy

Install dependencies using:
pip install pandas numpy scikit-learn xgboost statsmodels scipy

How to Run

Clone the repository:git clone https://github.com/feraz391/Credit-Risk-Prediction-to-Improve-Loan-Approval-.git


Navigate to the project directory:cd Credit-Risk-Prediction-to-Improve-Loan-Approval-


Open the Jupyter Notebook:jupyter notebook Credit_Risk_Modelling.ipynb


Ensure the datasets (case_study1.xlsx, case_study2.xlsx) are in the same directory as the notebook.
Run the notebook cells to reproduce the analysis and results.

Future Improvements

Incorporate additional features (e.g., external credit bureau data) to enhance predictive power.
Address potential class imbalance in the dataset using techniques like SMOTE or weighted loss functions.
Experiment with ensemble methods or advanced models like LightGBM or CatBoost.

Author

Feraz (GitHub: feraz391)

License
This project is licensed under the MIT License. See the LICENSE file for details.
