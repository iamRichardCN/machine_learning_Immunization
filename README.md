This repository contains the code used to develop a machine learning model for predicting immunization completion in a rural community in Nigeria. In this README file, we will provide an overview of the project, highlight its significance, and discuss valuable lessons learned during its development.

## Project Overview

Immunization is a crucial healthcare intervention to prevent the spread of infectious diseases and protect public health. However, immunization completion rates can vary significantly across different regions and communities, particularly in rural areas. This project focuses on predicting immunization completion in a specific rural community in Nigeria.

### Code Overview

The code in this repository is organized into several sections, each serving a specific purpose:

#### 1. Data Loading and Preprocessing

- We start by loading the dataset from an Excel file (`ajet data update.xlsx`) into a pandas DataFrame.
- Data preprocessing steps include handling missing values and encoding categorical variables.

#### 2. Exploratory Data Analysis (EDA)

- We perform exploratory data analysis to visualize patterns in the dataset.
- Plots include pair plots to understand feature relationships and count plots to analyze immunization completion by various factors, such as gender, income level, and mother's age.
- We also calculate percentages and create crosstabs to gain insights into the distribution of immunization completion.

#### 3. Feature Engineering

- We convert categorical variables into numerical format using one-hot encoding.
- This step prepares the data for machine learning model training.

#### 4. Principal Component Analysis (PCA)

- We apply Principal Component Analysis (PCA) to reduce the dimensionality of the dataset while retaining important information.
- The explained variance ratio is calculated to understand the contribution of each principal component.

#### 5. Model Training and Evaluation

##### Logistic Regression

- We train a logistic regression model to predict immunization completion.
- Cross-validation is performed to assess model performance.
- Evaluation metrics such as Mean Squared Error (MSE), Absolute Mean Error (MAE), and R-squared are calculated.
- Classification metrics including accuracy, precision, recall, and F1-score are provided.

##### Support Vector Machine (SVM)

- We explore different SVM kernels (linear, polynomial, RBF, sigmoid) and select the sigmoid kernel due to the best performance.
- Grid search is used to find the best hyperparameters for the SVM model.
- Cross-validation is performed to assess the SVM model's performance.
- Evaluation metrics, including MSE, MAE, R-squared, and classification metrics, are calculated.

## Project Significance

This project is of significant importance as it addresses the challenge of improving immunization completion rates in rural communities. By predicting immunization completion, healthcare providers and policymakers can target interventions more effectively, ensuring that all children receive essential vaccinations.

## Lessons Learned

During the development of this project, several valuable lessons were learned:

- Data preprocessing and cleaning are critical for model performance.
- Feature engineering techniques, such as one-hot encoding, can improve model accuracy.
- Dimensionality reduction techniques like PCA help manage high-dimensional data.
- Model selection and hyperparameter tuning are essential for achieving the best predictive performance.
- Cross-validation is a valuable tool for assessing model generalization.

## Conclusion

This project demonstrates the application of machine learning techniques to address a real-world healthcare challenge. By predicting immunization completion, we can contribute to improving public health outcomes in rural Nigerian communities.

For detailed code implementation and results, please refer to the Jupyter Notebook files in this repository.
