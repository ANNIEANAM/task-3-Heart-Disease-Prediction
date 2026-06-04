# Heart Disease Prediction Using Logistic Regression

## Task Objective

The objective of this project is to develop a machine learning model that predicts whether a patient is at risk of heart disease based on medical and clinical attributes. Early prediction of heart disease can assist healthcare professionals in making informed decisions and improving patient outcomes.

---

## Dataset Used

**Dataset:** Heart Disease UCI Dataset

The dataset contains patient health information such as:

* Age
* Sex
* Chest Pain Type (cp)
* Resting Blood Pressure (trestbps)
* Cholesterol Level (chol)
* Fasting Blood Sugar (fbs)
* Resting ECG Results (restecg)
* Maximum Heart Rate Achieved (thalch)
* Exercise-Induced Angina (exang)
* ST Depression (oldpeak)
* Slope of Peak Exercise ST Segment (slope)
* Number of Major Vessels (ca)
* Thalassemia (thal)

The original target variable (`num`) was converted into a binary classification problem:

* 0 → No Heart Disease
* 1 → Heart Disease

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Created a binary target variable from the original disease severity column.
3. Removed unnecessary columns.
4. Handled missing values using:

   * Mode for categorical features
   * Median for numerical features
5. Applied One-Hot Encoding to categorical variables.
6. Standardized numerical features using StandardScaler.
7. Split the dataset into training and testing sets.

---

## Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset:

* Heart Disease Distribution
* Age Distribution
* Heart Disease by Gender
* Correlation Heatmap

These visualizations helped identify patterns and relationships among clinical features.

---

## Model Applied

### Logistic Regression

Logistic Regression was selected as the classification model because it is effective for binary classification tasks and provides interpretable feature coefficients.

The model was trained on 80% of the dataset and evaluated on the remaining 20%.

---
## Exploratory Data Analysis (EDA)
Heart Disease Distribution: The dataset contains both heart disease and non-heart disease cases, making it suitable for binary classification.
Age Distribution: Most patients belong to middle-aged and older age groups, indicating that heart disease risk increases with age.
Heart Disease by Gender: The distribution suggests differences in heart disease occurrence between genders.
Correlation Heatmap: Several clinical features showed noticeable relationships with heart disease and with each other.

## Model Evaluation

The model was evaluated using:

1. Classification Report: Precision, Recall, and F1-Score were used to evaluate model performance for both classes.
2. Confusion Matrix: The model correctly classified the majority of patients, demonstrating good predictive capability.
3. ROC Curve: The ROC curve showed the model's effectiveness in distinguishing between patients with and without heart disease.
4. ROC-AUC Score: The AUC value indicated strong classification performance and reliable discrimination between classes.
These metrics provide a comprehensive assessment of classification performance.

## Important Features

Feature importance analysis revealed that the following attributes had the strongest influence on heart disease prediction:
Chest Pain Type (CP)
Maximum Heart Rate Achieved (Thalach)
Exercise-Induced Angina (Exang)
ST Depression (Oldpeak)
Thalassemia (Thal)
These factors contributed significantly to determining whether a patient was at risk of heart disease.
---

## Key Results and Findings
* The Logistic Regression model successfully classified patients into heart disease and non-heart disease categories.
* ROC-AUC analysis demonstrated the model's ability to distinguish between positive and negative cases.
* Feature importance analysis revealed that clinical factors such as chest pain type, exercise-induced angina, maximum heart rate achieved, ST depression, and thalassemia significantly influenced predictions.
* The results indicate that machine learning can be effectively used to support heart disease risk assessment and early diagnosis.

---

## Conclusion

This project demonstrates the application of machine learning techniques for heart disease prediction using the Heart Disease UCI dataset. After preprocessing, exploratory analysis, and model training, Logistic Regression achieved reliable performance and identified important health indicators associated with heart disease risk.

The project highlights the potential of data-driven approaches in assisting healthcare professionals with early disease detection and decision-making.
