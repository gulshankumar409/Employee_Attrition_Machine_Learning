# EMPLOYEE ATTRITION
Employee attrition is a critical aspect of human resource management, representing the departure of employees from an organization. Understanding and predicting attrition can aid in strategic workforce planning and retention efforts. This comprehensive documentation outlines the entire process of analyzing employee attrition using a dataset, encompassing data preprocessing, visualization, and the implementation of various machine learning models.

# Project step

*Dataset
The dataset contains information about employees, including various attributes such as age, daily rate, department, education, etc. The goal is to predict employee attrition.

*Data Cleaning
Columns with more than 80% empty values were dropped

*Data Preprocessing
Categorical columns were encoded using LabelEncoder.
Attributes with standard deviation less than 0.8 were excluded after normalization.

 Encoding Categorical Columns:
         Categorical columns are identified and encoded using the LabelEncoder from scikit-learn, converting them into a format suitable for machine learning models
 Normalizing data and creating Gaussian Distribution:
        A Gaussian distribution is created for each attribute, and attributes with a standard deviation below the threshold (0.8) are excluded. This step ensures that the dataset adheres to a standard scale.

#Exploratory Data Analysis (EDA)
Explored the dataset to derive insights into employee characteristics and potential factors contributing to attrition.

#Principal Component Analysis (PCA)
Applied PCA for feature extraction and visualization.

#Machine Learning Models
This repository contains Python code for predicting employee attrition using various machine learning models. The following models are implemented:

#Mean-Shift
Utilizes Mean-Shift clustering for prediction.
Achieves an accuracy of 86.17%.

#K-Nearest Neighbors (KNN)
Employs a KNN classifier with k=3.
Achieves an accuracy of 78.68%.

#Support Vector Machine (SVM)
Implements an SVM classifier with a linear kernel.
Achieves an accuracy of 86.17%.

#K-Means
Applies K-Means clustering for prediction.
Achieves accuracy metrics, precision, recall, and F1 score.

#Decision Tree
Trains a Decision Tree classifier.
Achieves an accuracy of 86.17%.
