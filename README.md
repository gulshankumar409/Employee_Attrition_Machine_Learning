# Employee Attrition Prediction

Employee attrition is a crucial aspect of human resource management, influencing strategic workforce planning and retention efforts. This comprehensive documentation guides you through the process of analyzing employee attrition using a dataset. The project encompasses data preprocessing, exploratory data analysis (EDA), and the implementation of various machine learning models.

## V1 File

### Project Steps

#### Dataset
The dataset contains employee information for predicting attrition, including attributes like age, daily rate, department, and more.

#### Data Cleaning
Columns with over 80% empty values were dropped to streamline the dataset.

#### Data Preprocessing
1. **Encoding Categorical Columns:**
   Categorical columns were encoded using LabelEncoder.
2. **Normalizing Data:**
   A Gaussian distribution was created for each attribute. Attributes with a standard deviation below 0.8 were excluded after normalization.

### Exploratory Data Analysis (EDA)

Explored the dataset to derive insights into employee characteristics and potential factors contributing to attrition.

### Principal Component Analysis (PCA)

Applied PCA for feature extraction and visualization.

### Machine Learning Models

Implemented the following models:

- **Mean-Shift:**
  Utilizes Mean-Shift clustering for prediction. Achieves an accuracy of 86.17%.
  
- **K-Nearest Neighbors (KNN):**
  Employs a KNN classifier with k=3. Achieves an accuracy of 78.68%.
  
- **Support Vector Machine (SVM):**
  Implements an SVM classifier with a linear kernel. Achieves an accuracy of 86.17%.

- **K-Means:**
  Applies K-Means clustering for prediction. Achieves accuracy metrics, precision, recall, and F1 score.

- **Decision Tree:**
  Trains a Decision Tree classifier. Achieves an accuracy of 86.17%.

## V2 File

### Data Visualization and EDA

Explored through bar charts for feature comparison between different attributes to gain insights into employee attrition.

### Heatmap Analysis for Feature Selection

#### Encoding Categorical Labels
Categorical columns are encoded using LabelEncoder for numerical analysis.

#### Correlation Heatmap
A heatmap of the correlation matrix visualizes relationships between features, aiding in identifying potential correlations influencing employee attrition.

#### Filtered Heatmap for Top Features
Selected important features ('OverTime', 'MonthlyIncome', etc.) are analyzed in a filtered heatmap for deeper insights.


**Top 10 Features:**
- 'OverTime'
- 'MonthlyIncome'
- 'TotalWorkingYears'
- 'Age'
- 'YearsAtCompany'
- 'StockOptionLevel'
- 'JobLevel'
- 'YearsWithCurrManager'
- 'MaritalStatus'
- 'JobRole'
