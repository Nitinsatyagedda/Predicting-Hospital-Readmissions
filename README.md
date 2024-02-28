# Predicting-Hospital-Readmissions
This is an open-source project repo which deals with predicting if the patients will get readmitted to the hospital or not in the next 30 Days.
# Introduction
The primary goal of this project is to build a predictive model that can identify patients who are at high risk of hospital readmission within 30 days after their initial discharge.
This project involves ETL of data from the csv file, cleaning, performing EDA, data visualization, feature extraction and classification model building using the machine learning algorithms available.
# Pre-requsites
Install the following packages to run the project.
pip install pandas

pip install numpy 

pip install seaborn 

pip install matplotlib 

pip install plotly 

pip install scikit-learn 

pip install imbalanced-learn 
# Technology Stack
Python scripting

Pandas

Jupyter Notebook

ETL from CSV

Data Pre-processing

Encoding of Categorical to Numerical data

Sklearn - Model Building

EDA and Feature Engineering

Plotly, Seaborn, Matplotlib
# Data Cleaning and Transformation
Load the dataset from CSV file to a pandas dataframe.

Handle missing values.

Remove outliers.

Transform the categorical variables to numerical.
# Model Building
Train_test_split of the dataset. Independent Columns = 17, Target Columns = 1.

Models Used for Comparison :

Logistic Regression

KNN Classifier

SVC

Random Forest

Ada Boosting

Gradient Boosting
# Model Evaluation
All the models mentioned above are evaluated to predict the train and test metrics.

Training Evaluation Metrics

accuracy,precision,r2_score
# Final Thoughts & Insights
Male are getting readmitted more than female and others.

If the Num_Medications is more than 30, then all "Male" are likely to get readmitted.

If the Num_Medications is more than 30, then all "Other"(Gender) are NOT likely to get readmitted.

If the Num_Medications is more than 30 and the age group of a person is between 20 and 30, then there is a high chance of 66.6% for him/ her to get readmitted.

If the Num_Outpatient_Visits increases, the chance of getting readmitted also increases (ie) Num_Outpatient_Visits are directly proportional to Readmitted_Yes columns.

There is a high probability of 16.59% for people of age 40-50 to get readmitted (Count=81) than any other age groups.

There is a high probability of 16.13% for people of age 70-80 to NOT get readmitted (Count=81) than any other age groups.

After applying EDA and feature importance, it is clear that the columns - "Gender", "Diagnosis", "Admission_Type" - majorly contributes to the model built.

It is evident that the hospital readmissions focuses primarily on these 3 fields. Other fields have a minor impact on the target column (Readmission_Yes).
