---
title: "UPDRS"
excerpt: "Predicting UPDRS measurement for patients with early-stage Parkinson’s disease. <br/><img src='/images/UPDRS.jpeg'>"
collection: portfolio
---


The goal of this project was to predict the value of the Unified Parkinson Disease Rating Scale (UPDRS) measurement for patients with early-stage Parkinson’s
disease, using data recorded via a telemonitoring device for remote symptom progression monitoring and allowing medical staff to obtain speech recordings captured in the patients’ homes. This measure is often used to track the disease’s progression. To note, the data I used was first presented and analysed by Tsanas et al. (2009). 

The following models were used to predict the total UPDRS score, and compared against each other on their performance using out-of-sample Root Mean Square Error (RMSE):
- A regularised linear model.
- Random Forest.
- XGBoost Model.
- Polynomial Regression Model.

The XGBoost model demonstrated exceptional performance with the lowest out-of-sample RMSE. When pitted against models from our Analytics Honours classmates, our XGBoost model not only excelled but secured a position among the Top 8 best predicting models for UPDRS, as determined by the RMSE metric. 

Find the code [here](https://github.com/siphiwebogatsu/UPDRS-/blob/main/Parkinson.Rmd). 

This project was done in collaboration. 

