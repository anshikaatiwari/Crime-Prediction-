# Crime Category Prediction Project 
 # Project Overview
This project focuses on predicting crime categories based on various features using machine learning techniques. The goal is to build a model that accurately classifies crime incidents into different categories. The dataset contains information such as the type of crime, location, and time of occurrence, which are used to train several classification models.

The final model achieves an accuracy of 88.22%.

## Data Preprocessing
Missing values were handled.
Features were engineered, including extracting time-based features such as hour, month, and day of the week.
## Exploratory Data Analysis (EDA)
The EDA phase involved:

Visualizing the distribution of crime categories.
Correlating features to identify important predictors.
Exploring temporal patterns (e.g., crime rates by day or hour).
The insights gained from EDA helped in feature selection and model development.

## Models 
Three different models were used to solve this multiclass classification problem:

1. Gradient Boosting Classifier
Gradient Boosting is an ensemble method that builds models sequentially, correcting errors from previous models. It performed well on this dataset due to its ability to handle complex relationships between features.

Library Used: sklearn.ensemble.GradientBoostingClassifier
Tuning: Parameters such as the number of trees and learning rate were fine-tuned using cross-validation.

2. Support Vector Machine (SVM)
SVM is a powerful classifier that works well for complex datasets with clear boundaries between classes. A kernel trick was used to map data into a higher-dimensional space.

Library Used: sklearn.svm.SVC
Kernel: We used the rbf (Radial Basis Function) kernel for improved accuracy.

3. Linear Regression (Multiclass)
Though Linear Regression is not typically used for classification, it was adapted for multiclass classification by treating each class as a separate regression problem.

Library Used: sklearn.linear_model.LinearRegression

## Results
The final model, after tuning, achieved an accuracy of 88.22% on the test set. This result demonstrates that the models performed well in predicting crime categories based on the provided features.

##Model	Accuracy
Gradient Boosting Classifier:	0.88220
Support Vector Machine (SVM) :	0.87210
Linear Regression:	0.83560
Gradient Boosting provided the highest accuracy.
