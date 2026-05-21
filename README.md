# Predictive Analytics: Income Level Classification

This repository contains an end-to-end machine learning project developed using the **KNIME Analytics Platform**. The primary objective is to predict whether an individual earns more than $50,000 annually based on the 1994 US Census Income dataset.
👉 [Dataset](https://www.kaggle.com/datasets/uciml/adult-census-income)

## Project Overview
The project strictly follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology. It covers everything from exploratory data analysis and data preprocessing (handling hidden missing values, equal size sampling for class imbalance) to the training and evaluation of multiple classification models.

## Applied Machine Learning Models
* Random Forest
* Artificial Neural Networks (MLP)
* Logistic Regression
* Decision Trees

## 📊 Key Results
The models were evaluated based on Accuracy, Sensitivity, Specificity, and AUC (ROC). 

| Model | Accuracy | Sensitivity | Specificity | ROC (AUC) |
| :--- | :---: | :---: | :---: | :---: |
| Decision Tree | 0.775 | 0.817 | 0.762 | 0.828 |
| Logistic Regression | 0.809 | 0.857 | 0.793 | 0.907 |
| Neural Network (MLP) | 0.805 | **0.868** | 0.786 | 0.909 |
| **Random Forest** | **0.820** | 0.858 | **0.808** | **0.909** |

**Conclusion:** The **Random Forest** algorithm emerged as the most robust model, achieving the highest accuracy (82.0%) and an exceptional AUC score of 0.909. Variable importance analysis revealed that `CapitalGain` and `Relationship` status are the most critical predictors of high income.

## 📄 Detailed Report
For a comprehensive breakdown of the business understanding, data preparation steps, node configurations, decision tree splits, and detailed business insights, please refer to the full project report:
👉 [Read the Detailed CRISP-DM Report Here](./CRISP_DM_Detailed_Report.pdf)

## 🛠️ How to Run This Project
1. Download and install the [KNIME Analytics Platform](https://www.knime.com/).
2. Clone this repository to your local machine.
3. Open KNIME, go to `File > Import KNIME Workflow...` and select the `.knwf` file from this repository.
4. Execute the nodes sequentially to reproduce the results.
