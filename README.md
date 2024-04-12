# Project Description

The objective is to optimize the MSE of the prediction of Length of Stay ('LOS') in a ICU based on patient-related characteristics such as vital signs (i.e., HeartRate, SysBP,etc) diagnosis and comorbidities, and personnel data (i.e., age, ethnicity, etc). For such, minimal preprocessing and feature engineering is performed. 
Prediction techniques used are 
1) Neural Networks using Keras library. Several architectures with different sizes of layers are used and different output activation functions (relu/exponential). Best result obtained on out of sample predictions is 4.34 RMSE on in class Kaggle Competition.
2) Different Ensembling techniques such as stacking, blending and subsembling are used trainning and doing hyperparameter tuning of baselearners beforehand. Best results are achieved using stacking method with LightGBM as a metalearner and KNN, RF and XGB as base learners. Best score is 4.19 RMSE on in-class Kaggle Competition.

# Data
Data used comes from the MIMIC project (https://mimic.physionet.org/). A large, freely-available database comprising deidentified health-related data associated with over forty thousand patients who stayed in critical care units of the Beth Israel Deaconess Medical Center between 2001 and 2012.
