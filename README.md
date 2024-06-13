# Overview

This project aims to improve the accuracy of diabetes prediction by leveraging ensemble machine learning models. Initial experiments were conducted using local machine learning methods, and further optimization was achieved using Azure AutoML. The best performing model was a voting ensemble model.

# Core Azure Services Used
* Container Registry - (Registering Best Performing Models)
* Container Instances - (Deployment and Testing the Model using Real Time Data)
* Storage Account - (Storing the datasets required)
* Key Vault - (Securing the resources and configuring the workspace)

# Azure AI Services Used

* Azure Machine Learning - (AutoML WorkFlows)

# Project Workflow

## 1. Data Acquisition & Preprocessing:

Uploaded the diabetes dataset to Azure ML Studio.
Inspected the data for outliers and performed preprocessing to ensure data quality and readiness for modeling.
Handled missing values, scaled numerical features, and encoded categorical features as necessary.

## 2. Model Selection with AutoML:

Utilized Azure AutoML to automate the exploration and evaluation of various machine learning algorithms suitable for predicting diabetes.
Identified the best performing model(s) based on predefined performance metrics.

## 3. Ensemble Model Development:

Implemented an ensemble learning technique to combine the strengths of the individual models identified by AutoML.
Techniques such as stacking and bagging were considered to further enhance prediction accuracy.
The final voting ensemble model showed the best performance.

## 4. Model Deployment & Local Execution:

Deployed the final model (individual or ensemble) as a REST endpoint on Azure ML Studio for real-time predictions.
Downloaded a pickle file of the final model for local execution, allowing for flexibility in deployment and use.

# Screenshots of the Project

## Various Models Tested
![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/452a5177-6cc9-4bdc-a8df-af1bb7689ad2)

## Features By Importance

![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/02b12df7-ee14-4ecb-8945-61b717e7450c)

## Testing the REST Endpoint with real time data in Jupyter Notebook

![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/ced8e8d9-380e-4155-8e6f-2f2977ad2f57)

## AutoML Execution

![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/22ff3510-453d-4bca-83a9-c669735a9fff)

## Dataset Used 
The columns that are present in the dataset
* Pregnancies
* Glucose Levels in Blood (Before Meals)
* Blood Pressure
* Skin Thickness
* Insulin (Before Meals)
* BMI
* Diabetes Pedigree Function
* Age
* OutCome (Target Variable, 0 for Negative and 1 for Positive)
![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/26faec00-46cb-40c3-9020-38cea44e78a1)

## Resource Group in Azure Portal

![image](https://github.com/Sahana-Lakshmipathy/Diabetes-Prediction-Model/assets/132273934/38c35144-a94e-468b-9ad1-06b2718eecf4)
