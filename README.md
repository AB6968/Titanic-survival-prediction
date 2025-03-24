# Titanic-survival-prediction
Overview

This project builds a machine learning model to predict whether a passenger survived the Titanic disaster. The dataset includes various features like age, gender, ticket class, fare, and cabin information. The goal is to preprocess the data effectively, build a classification model, and evaluate its performance.

Dataset

The dataset consists of the following key features:
Passanger id:passanger identification number
Pclass: Passenger class (1st, 2nd, 3rd)
Sex: Gender of the passenger
Age: Age of the passenger
SibSp: Number of siblings/spouses aboard
Parch: Number of parents/children aboard
Fare: Ticket fare
Cabin: which cabin alloted
Name: name of passanger
Ticket: Ticket number
Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
Survived: Target variable (0 = No, 1 = Yes)

Preprocessing Steps

Handling Missing Values
Filled missing values in Age using the mean.
Filled missing values in Fare with the mean.
No missing values in Embarked, but categorical encoding was performed.
Dropped duplicates.

Encoding Categorical Variables:

Converted Sex and Embarked to numerical representations.
Scaling Numerical Features
Standardized data using StandardScaler.

Model Training

I experimented with following classifier, :

Random Forest Classifier

The model was a Random Forest Classifier with the following hyperparameters:
RandomForestClassifier(n_estimators=100, max_depth=5, random_state=42)

Evaluation Metrics:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Cross-validation scores


Future Improvements

Tune hyperparameters for better performance
Try deep learning approaches like Neural Networks
Use advanced feature selection technique
