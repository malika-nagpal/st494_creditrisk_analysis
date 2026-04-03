# ST494 - Credit Risk Analysis

This repository contains our group project for **ST494 Statistical Machine Learning**.  
The project analyzes the **Default of Credit Card Clients** dataset and compares several statistical learning models for predicting next-month default risk.

## Project Goal

The main objective of this project is to predict whether a credit card client will default on their payment in the following month, and to compare different modeling approaches in terms of predictive performance and practical usefulness.

## Dataset

We used the **Default of Credit Card Clients** dataset from the UCI Machine Learning Repository.

- Source: Yeh, I.-C., & Lien, C.-H. (2009). *Default of credit card clients* [Dataset]. UCI Machine Learning Repository.
- Link: https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients

## Repository Structure

### Main notebooks

- **EDA.ipynb**  
  Data cleaning, preprocessing checks, and exploratory data analysis.  
  Includes class balance, variable distributions, relationships with default, and correlation analysis.

- **LogReg.ipynb**  
  Logistic Regression modeling notebook.  
  Includes preprocessing, scaling, cross-validation, tuning, calibration, and final evaluation.

- **RandomForest.ipynb**  
  Random Forest modeling notebook.  
  Includes training, hyperparameter tuning, feature importance, and evaluation.

- **Tree(LGBM).ipynb**  
  LightGBM modeling notebook.  
  Includes training, tuning, feature handling, and final model results.

- **Evaluation.ipynb**  
  Final comparison notebook.  
  Compares all models using metrics such as ROC-AUC, accuracy, precision, recall, F1-score, and Brier score.

## Other folders

- **data/**  
  Contains the dataset files used in the analysis.

- **Models/**  
  Contains saved model-related files and artifacts generated during training.

## Suggested Reading Order

If reviewing the project for the first time, the recommended order is:

1. **EDA.ipynb**
2. **LogReg.ipynb**
3. **RandomForest.ipynb**
4. **Tree(LGBM).ipynb**
5. **Evaluation.ipynb**

This order follows the natural progression of the project:
data understanding → baseline model → tree-based models → final comparison.

## Models Compared

The project compares three models:

- Logistic Regression
- Random Forest
- LightGBM

## Final Summary

- **LightGBM** achieved the highest ROC-AUC and best overall ranking performance.
- **Random Forest** achieved the strongest recall/F1 trade-off for the default class at the standard threshold.
- **Logistic Regression** served as the most interpretable baseline.

## Reproducibility Notes

All analysis is contained in the notebooks listed above.  
To reproduce the project, run the notebooks in the suggested reading order.

## Course Context

This repository was created for the **ST494 Statistical Machine Learning** course project.
