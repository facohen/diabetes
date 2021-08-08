# Early Stage Diabetes Risk Prediction Dataset
## Udacity Data Science Nanodegree 
## By Federico Alejandro Cohen
## Buenos Aires, Argentina - August 2021 


Project Description

The purpose of this project is to analize and develope a machine learning model to predict if a patient with certain condition has diabetes. 
We are using a dataset from Kaggle, which contains records collected from Sylhet Diabetes Hospital in Sylhet. The dataset comprises direct questionnaires filled out by patients and approved by a doctor. It comprises healthy and diabetes diagnosed patients, male and females aged 20 to 65. There are 14 conditions listed and whether they are present for each of the patients. The target variable is 'class' which indicates whether te patient has diabetes. 

# Motivation

According to Merk Manual:

> Diabetes mellitus is impaired insulin secretion and variable degrees of peripheral insulin resistance leading to hyperglycemia. Early symptoms are related to hyperglycemia and include polydipsia, polyphagia, polyuria, and blurred vision. Later complications include vascular disease, peripheral neuropathy, nephropathy, and predisposition to infection. Diagnosis is by measuring plasma glucose. Treatment is diet, exercise, and drugs that reduce glucose levels, including insulin, oral antihyperglycemic drugs, and non-insulin injectable drugs. Complications can be delayed or prevented with adequate glycemic control; heart disease remains the leading cause of mortality in diabetes mellitus.

# Project outline

We will use this dataset to deep dive into research questions: which conditions are most frequent for diabetes patients, since they can be an early sign at the onset, and those patients need to be carefully screened for the condition present. We also analyise if a patient age is relevant for diabetes disease, then we move into exploration for average patient age for each condition, and which conditions are gender related.

We will develop a machine learning model - Support Vector Classifer, in order to predict whether a patient has diabetes based on reported health condition(s). We chose a Support Vector Machine Classifier, because the dataset is rather small and it is less prone to overfitting. We are doing a first run without hyperparameter tuning and then we use Grid Search Cross Validation with radial basis function.In classification algorithms in general, and in machine learning applications for diagnoses purposes, it is critical to assess Type I and Type II errors, hence precision and recall are of the utmost importance. We will favor a model with high recall, as we want to keep false negatives -misdiagnosed diabetes patients as not having the disease-as close to zero as possible.


### Code is contained on diabetes.ipynb, written with Python 3.8.11

### Requirements
- Pandas
- Numpy
- Plotly
- Scikit-Learn

### Data Source
The dataset is available at  https://www.kaggle.com/ishandutta/early-stage-diabetes-risk-prediction-dataset

### Licensing
Dataset is licensed under Open Data Commons - Database Contents License (DbCL) v1.0

### Citations
- https://www.merckmanuals.com/professional/endocrine-and-metabolic-disorders/diabetes-mellitus-and-disorders-of-carbohydrate-metabolism/diabetes-mellitus-dm
- Islam, MM Faniqul, et al. 'Likelihood prediction of diabetes at early stage using data mining techniques.' Computer Vision and Machine Intelligence in Medical Image Analysis. Springer, Singapore, 2020. 113-125.
