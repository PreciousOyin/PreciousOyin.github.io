# Diabetes Predictor App
Name: Precious Oyinloye
Link to Presentation Video: https://github.com/PreciousOyin/PreciousOyin.github.io/blob/main/Oyinloye_Precious_CapstoneVideo.mp4
## App Instructions
Enter patient health information into the form and click "Submit" to receive a predicted diabetes risk score.

## Project Overview
This capstone is based on an interactive app that predicts the likelihood of diabetes using a logistic regression model trained on certain patient health data features. The user can input their data such as age, glucose levels, BMI and other clinical measurements and it will return an estimated risk score of diabetes.

## Description of Dataset Contents
The dataset is from the Pima Indians Diabetes Database and originally collected from the National Institute of Diabetes and Digestive and Kidney Diseases. It contains medical measurements and a binary outcome indicating if the patient has not diabetes (0) or does have diabetes (1). All patients are all females, 21 years or older, and of Pima Indian heritage. 
## Data Cleaning
Data cleaning was performed on this dataset. Variables such as glucose levels, diastolic blood pressure, and BMI contained zero values which are not physiologically possible. Rows that contained zero values in these columns were removed prior to modelling to improve the quality and relevance of the data.
Link to dataset: https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

## Modeling
Logistic regression was chosen since the diabetes outcomes are binary (healthy = 0 or diabetes = 1). Predictor s for include Age, BMI, Diastolic Blood Pressure, Insulin Intake, Glucose levels and number of pregnancies. 

## Model Evaluation
To evaluate the model, the data was split into an 80/20 training and testing sets to understand model performance. The ROC-AUC metric was used, which measures the model’s ability to separate the non-diabetic cases (0) from the diabetic cases (1).

## Limitaiton and Interpretation
The dataset is imbalanced with a larger proportion of non-diabetic patients than diabetic patients. Due to this, the model may be biased toward predicting a lower probability of diabetes.  Also, the dataset only includes Pima Indian female patients aged 21 years or older. This limits the generalizability of the model because it doesn’t capture full biological and demographic range of the general population. There is a risk of overfitting due to the limited scope of the dataset. This may lead to the model performing well for the training data but not for new populations. Future work could involve increasing the variation of race, age and sex to assess if model performance will improve.

The output of this app represents a probability (risk score) of having diabetes and not an actual medical diagnosis.
