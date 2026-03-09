# BLENDED_LEARNING
# Implementation of Logistic Regression Model for Classifying Food Choices for Diabetic Patients

## AIM:
To implement a logistic regression model to classify food items for diabetic patients based on nutrition information.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import Libraries: Bring in the necessary libraries.
2. Load the Dataset: Load the diabetic food choices dataset into your environment.
3. Data Preprocessing: Handle any missing data and encode categorical variables as needed.
4. Define Features and Target: Split the dataset into features (X) and the target variable (y).
5. Split Data: Divide the dataset into training and testing sets.
6. Build Logistic Regression Model: Initialize and create a logistic regression model.
7. Train the Model: Fit the model to the training data.
8. Evaluate Performance: Assess the model's performance using cross-validation or evaluation metrics.
9. Display Model Parameters: Output the model’s coefficients and intercept.
10. Make Predictions & Compare: Predict food choices for diabetic patients and compare them with the actual values

## Program:
```
/*
Program to implement Logistic Regression for classifying food choices based on nutritional information.
Developed by: Sanjeev Kumar K
RegisterNumber:  25012334

import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.preprocessing import LabelEncoder, MinMaxScaler
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, confusion_matrix, classification_report
import seaborn as sns
import matplotlib.pyplot as plt
df = pd.read_csv('food_items (1).csv')
print('Name:')
print('Reg. No: ')
print("Dataset Overview:")
print(df.head())
print("\nDataset Info:")
print(df.info())
X = scaler.fit_transform(X_raw)
label_encoder = LabelEncoder()
y = label_encoder.fit_transform(y_raw.values.ravel())X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, stratify=y, random_state = 123)
penalty = 'l2'
multi_class = 'multinomial'
solver = "lbfgs"
max_iter = 1000
model = LogisticRegression(random_state=123, penalty=penalty, multi_class=multi_class, solver=solver, max_iter=max_iter)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
print('Name:Sanjeev Kumar.K')
print('Reg. No:212225230246')
print("\nModel Evaluation:")
print("Accuracy:", accuracy_score(y_test, y_pred))
print("\nClassification Report:")
print(classification_report(y_test, y_pred))
conf_matrix = confusion_matrix(y_test, y_pred)
print(conf_matrix)
print('Name:Sanjeev Kumar.K')
print('Reg. No:212225230246')

*/
```

## Output:
![alt text](<Screenshot 2026-03-09 134004.png>) 
![alt text](<Screenshot 2026-03-09 134035.png>) 
![alt text](<Screenshot 2026-03-09 134045.png>) 
![alt text](<Screenshot 2026-03-09 134059.png>)

## Result:
Thus, the logistic regression model was successfully implemented to classify food items for diabetic patients based on nutritional information, and the model's performance was evaluated using various performance metrics such as accuracy, precision, and recall.
