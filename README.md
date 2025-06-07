# 📘 Credi-Risk-Solution-with-Explainable-AI

## Overview

This project aims to develop a machine learning model to predict credit risk and enhance its interpretability using Explainable AI (XAI) methods. By leveraging techniques like SHAP (SHapley Additive exPlanations), the project provides insights into the model's decision-making process, ensuring transparency and trustworthiness in credit risk assessments.([arxiv.org][1])

## Repository Contents

* **`CreditRiskAISolution.ipynb`**: A Jupyter Notebook containing the end-to-end implementation, including data preprocessing, model training, evaluation, and explanation using SHAP.
* **`credit_risk_dataset.csv`**: The dataset used for training and evaluating the credit risk model.
* **`README.md`**: This file, providing an overview and guidance on using the repository.

## Dataset Description

The dataset comprises various features related to borrowers' financial and personal information, which are crucial for assessing credit risk. Key features include:

* **`loan_amnt`**: The total amount of the loan.
* **`term`**: The duration of the loan.
* **`int_rate`**: Interest rate on the loan.
* **`installment`**: Monthly payment amount.
* **`grade`**: Loan grade assigned by the lending institution.
* **`emp_length`**: Length of employment in years.
* **`home_ownership`**: Home ownership status.
* **`annual_inc`**: Annual income of the borrower.
* **`purpose`**: Purpose of the loan.
* **`dti`**: Debt-to-income ratio.
* **`delinq_2yrs`**: Number of delinquent accounts in the past 2 years.
* **`revol_util`**: Revolving line utilization rate.
* **`total_acc`**: Total number of credit lines.
* **`credit_risk`**: Target variable indicating credit risk (e.g., 'good' or 'bad').([github.com][2], [arxiv.org][3])

## Methodology

### 1. Data Preprocessing

* **Handling Missing Values**: Imputed or removed missing entries to ensure data quality.
* **Encoding Categorical Variables**: Converted categorical features into numerical representations using techniques like one-hot encoding.
* **Feature Scaling**: Applied scaling methods to normalize feature values, facilitating model convergence.([github.com][2])

### 2. Model Development

* **Model Selection**: Utilized machine learning algorithms suitable for classification tasks, such as Random Forest or Gradient Boosting.
* **Training and Validation**: Split the dataset into training and testing sets to evaluate model performance.
* **Evaluation Metrics**: Assessed model accuracy, precision, recall, and F1-score to determine effectiveness.

### 3. Explainable AI with SHAP

* **SHAP Integration**: Implemented SHAP to interpret the model's predictions by calculating feature contributions.
* **Visualization**: Generated plots like SHAP summary plots and dependence plots to visualize feature impacts.
* **Insights**: Identified key features influencing credit risk predictions, enhancing model transparency.([originalstatic.aminer.cn][4], [github.com][2])

## Getting Started

### Prerequisites

Ensure you have the following installed:

* Python 3.6 or higher
* Jupyter Notebook
* Required Python libraries:

  * pandas
  * numpy
  * scikit-learn
  * shap
  * matplotlib
  * seaborn([belfercenter.org][5], [arxiv.org][6], [github.com][7])

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Anish-code/Credi-Risk-Solution-with-Explainable-AI.git
   cd Credi-Risk-Solution-with-Explainable-AI
   ```


2. **Run the Notebook**:

   ```bash
   jupyter notebook CreditRiskAISolution.ipynb
   ```



## Results

The machine learning model achieved satisfactory performance in predicting credit risk, with key features like `int_rate`, `annual_inc`, and `dti` significantly influencing the predictions. SHAP visualizations provided clear insights into how each feature impacted individual predictions, facilitating better understanding and trust in the model's decisions.
## Future Work

* **Model Optimization**: Explore hyperparameter tuning to enhance model performance.
* **Feature Engineering**: Incorporate additional relevant features to improve predictive accuracy.
* **Alternative XAI Methods**: Experiment with other explainability techniques like LIME or ELI5 for comparison.

## References

* Molnar, Christoph. *Interpretable Machine Learning*. [https://christophm.github.io/interpretable-ml-book/](https://christophm.github.io/interpretable-ml-book/)
* Lundberg, Scott M., and Su-In Lee. "A unified approach to interpreting model predictions." *Advances in Neural Information Processing Systems* 30 (2017).([originalstatic.aminer.cn][4])
