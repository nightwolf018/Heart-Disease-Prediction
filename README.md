# Heart Disease Prediction Using Logistic Regression

This project demonstrates a complete machine learning pipeline for heart disease prediction using the Cleveland Heart Disease dataset from the UCI Machine Learning Repository. The dataset contains patient characteristics from the Cleveland Clinic Foundation, where researchers recorded various medical indicators to classify the presence of heart disease.

## Dataset Information
The dataset used in this project provides information about patients and their cardiovascular health status. It includes the following columns:

| Variable | Description |
| --- | --- |
| age | Patient age in years |
| sex | Gender (0 = female, 1 = male) |
| cp | Chest pain type (1-4 scale) |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol level (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl (0 = false, 1 = true) |
| restecg | Resting electrocardiographic results (0-2 scale) |
| thalach | Maximum heart rate achieved during stress test |
| exang | Exercise induced angina (0 = no, 1 = yes) |
| oldpeak | ST depression induced by exercise relative to rest |
| slope | Slope of the peak exercise ST segment |
| ca | Number of major vessels colored by fluoroscopy (0-3) |
| thal | Thalassemia type (3 = normal, 6 = fixed defect, 7 = reversible defect) |
| present | Heart disease presence (0 = absent, 1 = present) |

The dataset contains 303 records with an almost equal distribution between patients with and without heart disease, making it well-balanced for classification tasks.

## Objective
The main objective of this project is to develop a logistic regression model that can accurately predict the presence of heart disease based on patient characteristics. The model focuses on providing interpretable coefficients for clinical insights while achieving reliable classification performance for potential use as a decision support tool in medical settings.

## Approach
The project follows a comprehensive machine learning methodology:
- **Data preprocessing**: Handling missing values, data type conversions, and feature selection
- **Exploratory data analysis**: Statistical analysis and visualization of patient characteristics
- **Feature selection**: Choosing age, maximum heart rate, resting ECG results, and coronary vessel count based on clinical significance
- **Model training**: Implementing logistic regression with 70-30 train-test split
- **Model evaluation**: Performance assessment using accuracy, sensitivity, and specificity metrics

Key preprocessing steps include converting object columns to numeric format and handling missing values through dropna approach to maintain data quality.

## Results
- **Test Accuracy**: 75.6% overall correct classification rate
- **Sensitivity**: 79.5% successfully identifies 4 out of 5 heart disease cases
- **Specificity**: 72.5% correctly identifies healthy patients
- **Key Risk Factors**: Coronary vessel blockages (OR = 3.25) emerged as the strongest predictor, followed by ECG abnormalities (OR = 1.47)
- **Model Generalization**: Stable performance between training and test sets with minimal overfitting

The analysis revealed that the number of affected coronary vessels is the dominant risk factor, which aligns with established clinical knowledge about cardiovascular disease progression.

## Impact
Accurate heart disease prediction has significant implications for healthcare delivery and patient outcomes. This model can serve as a decision support tool to enhance clinical practice by providing early detection capabilities and risk stratification. Healthcare providers can use these insights for improved patient screening, resource allocation, and treatment planning. The interpretable nature of logistic regression allows clinicians to understand the reasoning behind predictions, fostering trust and integration into medical workflows.

By leveraging machine learning techniques, this project contributes to more data-driven approaches in cardiovascular medicine and demonstrates the potential for automated screening tools to complement physician expertise in heart disease diagnosis.
