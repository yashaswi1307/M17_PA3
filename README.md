# Bank Marketing Classifier
Will the Customer Subscribe to a Term Deposit?

## Overview

This project analyzes data from a Portuguese banking institution to predict whether a customer will subscribe to a term deposit after a telemarketing campaign. It compares several machine learning models (Logistic Regression, KNN, Decision Trees, and SVM) to find the most effective approach for improving marketing efficiency.

## Dataset

* **Source**: UCI Machine Learning Repository ("Bank Marketing" dataset)
* **Records**: ~41,188 entries
* **Columns**: 20 input features + 1 output label
* **Attributes**:  
  * **Client data**: `age`, `job`, `marital`, `education`, `default`, `housing`, `loan`  
  * **Campaign data**: `contact`, `month`, `day_of_week`, `duration`, `campaign`, `pdays`, `previous`, `poutcome`  

## Prerequisites

This project is designed to run in a Codio cloud workspace with full Jupyter Notebook and Python support. No local setup is required.

* **Codio Workspace**: Create or import this repository into a Codio project.
* **Python Environment**: Codio provides Python 3.x by default.
* **Notebook Server**: Launch Jupyter Notebooks directly from the Codio sidebar.

## Project Structure

├── data/
│   └── data-additional/
│       ├── bank-additional-full.csv
│       ├── bank-additional.csv
│       └── bank-additional-names.txt
├── solution.ipynb
└── README.md

## Usage

1. **Clone or download** this repository.  
2. Place `bank-additional-full.csv` in the `data/data-addiotinal/` folder.  
3. Open and run `solution.ipynb` step by step.  

## Analysis Steps

1. **Data Cleaning**: Handle missing values (`unknown`), drop unrealistic columns (`duration`).  
2. **Feature Engineering**: Encode categorical variables, scale numerics, create derived features (`pdays` flag).  
3. **Baseline**: Compute baseline accuracy (majority class).  
4. **Modeling**: Fit Logistic Regression, KNN, Decision Tree, and SVM.  
5. **Model Comparison**: Evaluate training time, train/test accuracy.  
6. **Improvements**: Hyperparameter tuning, feature engineering, adjusted metrics (F1/PR-AUC).  

## Key Findings

* **Best Models**: Logistic Regression and Linear SVM provided the strongest generalization.  
* **Business Value**: Predictive models can prioritize top customers for telemarketing, reducing costs and improving subscription rates.  

## Author

Yashaswi Raval

---

*For questions or contributions, please open an issue or submit a pull request.*

