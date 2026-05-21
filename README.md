# Heart Disease Prediction using Machine Learning

## Overview
This project focuses on predicting heart disease severity using machine learning techniques. The objective was to analyze patient medical data and train different models to classify whether a patient has heart disease and determine its severity level. Since heart disease is a major global health issue, machine learning can help support faster and more accurate medical decision-making.

## Dataset
The dataset contains patient health information such as age, cholesterol level, blood pressure, chest pain type, ECG results, heart rate, and other clinical measurements. It includes multiple classes representing different severity levels of heart disease, making it a multi-class classification problem.

The dataset also contains both numerical and categorical features, requiring preprocessing before model training.

## Data Preprocessing
Several preprocessing steps were performed to prepare the dataset for machine learning models. Missing values were handled using imputation techniques, categorical variables were converted into numerical form using one-hot encoding, and numerical features were standardized using feature scaling.

The dataset was then divided into training, validation, and testing sets using stratified sampling to preserve class distribution.

## Exploratory Data Analysis
Exploratory Data Analysis (EDA) was conducted to better understand the dataset. Different visualizations such as histograms, boxplots, density plots, and correlation heatmaps were used.

The analysis showed that features like blocked vessels (`ca`) and ST depression (`oldpeak`) were strongly associated with heart disease severity, while maximum heart rate (`thalach`) showed a negative relationship with severity.

## Models Used
Three supervised machine learning models were implemented and compared:
- Decision Tree
- Logistic Regression
- Neural Network

In addition, K-Means Clustering was used as an unsupervised learning approach to observe natural grouping patterns within the dataset.

## Results
The models achieved moderate performance overall. Logistic Regression produced the highest overall accuracy, while the Neural Network provided better performance on minority classes and more balanced predictions across all severity levels.

The Decision Tree model offered easier interpretability but lower overall performance. K-Means Clustering showed weak clustering performance, indicating that the disease severity classes do not naturally form separate groups without supervised learning.

## Challenges
The project faced several real-world data challenges, including:
- Missing values
- Imbalanced classes
- Small dataset size
- Overfitting in Neural Networks

These issues affected model performance, especially for minority classes with very limited samples.

## Conclusion
This project demonstrates how machine learning can be applied in healthcare to predict heart disease severity from clinical data. Although the dataset presented multiple challenges, the models were able to identify meaningful patterns and achieve reasonable classification performance.

Future improvements could include using larger datasets, applying oversampling methods such as SMOTE, and exploring more advanced ensemble learning models like Random Forest or XGBoost.
