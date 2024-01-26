# EMPLOYEE ATTRITION
Employee attrition is a critical aspect of human resource management, representing the departure of employees from an organization. Understanding and predicting attrition can aid in strategic workforce planning and retention efforts. This comprehensive documentation outlines the entire process of analyzing employee attrition using a dataset, encompassing data preprocessing, visualization, and the implementation of various machine learning models.

# Project step


* Cleaning data
    * Try to remove the attributes which are mostly None:
        The columns with more than 90% empty values are dropped
    * Encoding Categorical Columns:
         Categorical columns are identified and encoded using the LabelEncoder from scikit-learn, converting them into a format suitable for machine learning models
    * Normalizing data and creating Gaussian Distribution:
        A Gaussian distribution is created for each attribute, and attributes with a standard deviation below the threshold (0.8) are excluded. This step ensures that the dataset adheres to a standard scale.
* Feature Extraction with PCA 
    Principal Component Analysis (PCA) is applied to reduce the dimensionality of the dataset
* Machine Learning Models
    * K-Nearest Neighbors (KNN)
        A K-Nearest Neighbors classifier is trained on the PCA-transformed features, and its performance is evaluated using key metrics and a confusion matrix.
    * Support Vector Machine (SVM)
        A Support Vector Machine (SVM) classifier with a linear kernel is trained on the PCA-transformed features, and its performance is evaluated using key metrics and a confusion matrix
    * Decision Tree
        A Decision Tree classifier is trained on the PCA-transformed features, and its performance is evaluated using key metrics and a confusion matrix.
Note - Some models (e.g., Mean-Shift, SVM, Decision Tree) resulted in precision, recall, and F1-Score being set to 0.0 due to no predicted samples. This could indicate issues with the model or the dataset.

