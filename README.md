#Overview
---
This project aims to improve the accuracy of diabetes prediction by leveraging ensemble machine learning models. Initial experiments were conducted using local machine learning methods, and further optimization was achieved using Azure AutoML. The best performing model was a voting ensemble model.

#Project Workflow
---
##1. Data Acquisition & Preprocessing:

Uploaded the diabetes dataset to Azure ML Studio.
Inspected the data for outliers and performed preprocessing to ensure data quality and readiness for modeling.
Handled missing values, scaled numerical features, and encoded categorical features as necessary.

##2. Model Selection with AutoML:

Utilized Azure AutoML to automate the exploration and evaluation of various machine learning algorithms suitable for predicting diabetes.
Identified the best performing model(s) based on predefined performance metrics.

##3. Ensemble Model Development:

Implemented an ensemble learning technique to combine the strengths of the individual models identified by AutoML.
Techniques such as stacking and bagging were considered to further enhance prediction accuracy.
The final voting ensemble model showed the best performance.

##4. Model Deployment & Local Execution:

Deployed the final model (individual or ensemble) as a REST endpoint on Azure ML Studio for real-time predictions.
Downloaded a pickle file of the final model for local execution, allowing for flexibility in deployment and use.
