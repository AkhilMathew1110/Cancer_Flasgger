# Breast Cancer Prediction Model and Frontend UI using Flasgger
## Introduction
This Project focuses mainly on the prediction of breast cancer classes and the effective way of representation of data on a web-based user interface using Flasgger API
which is available in Python. Our goal is to test the interactive prediction UI using csv file. Python programming is used in this Project to develop the model and Flasgger
and Swagger API's are used for the formation of User Interface.

## Dataset
The dataset we used for this analysis contains 569 entries and 33 columns. Model creation is focused on the diagnosis of cancer level based on the features available in the
dataset. Diagnosis is the dependent variable which we are trying to predict and it has two classes Malignant (M) & Benign (B), where all remaining variables are inddependent 
contribute to the prediction of our model. As the system will not be understand the character variables we converted the values of our dependent variable to numerical values
0 for Malignant and 1 for Benign. One of the main challeges we have seen during our model implementation was the class imbalance and we used 'class_weight' parameter to avoid 
this issue. A few of the variables are mutually correlated which are really not providing any significant roles to the analysis. No null values were in dataset and we have 
excluded id column because it doesn't add any value to our analysis.

## Prerequisites
Python setup on the local machine will be required for the execution. Latest version of sklearn package.
Flasgger and Swagger package to be installed on the local machine. Postman setup to test the API incase of any issues.

## Training & Testing of the Model
Logistic regression algorithm is used for the creation of this prediction model. Our dataset has divided into training and testing for the evaluation. 80% of the datapoints
are assigned for training and rest of the datapoints for testing the model.

## Flasgger & Swagger
Flask is a small package available in Python to create web-based applications easier. Flasgger is an extension to extract open-API specification from Flask views in the API.
Flasgger comes up with SwaggerUI, which helps to create the UI so people can access web using http://localhost:5000/apidocs 

## Model
Logistic regression algorithm is used for the implementation of Cancer Prediction Model. You can use saved model file in the repository for testing the prediction.
Saved model is already trained on a breast_cancer.csv dataset with an accuracy of 94% on test dataset.

## Contact
Akhil Mathew (mathewakhil1110@gmail.com)
