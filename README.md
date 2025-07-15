# Pima_Indians_Diabetes_Prediction
The Pima Indians Diabetes Dataset is a popular dataset from the UCI Machine Learning Repository. It contains medical data collected from female patients of Pima Indian heritage, aged 21 and older, to study diabetes risk.

#  Diabetes Prediction using Random Forest (Gradio App)

This project is a machine learning web application that predicts whether a person is diabetic or not based on health metrics. It uses the Pima Indians Diabetes Dataset, performs data preprocessing, trains a Random Forest Classifier, and deploys the model using an interactive Gradio interface.

---

## Dataset Description

The dataset used in this project is the Pima Indians Diabetes Dataset** from the UCI Machine Learning Repository. It consists of medical records for 768 female patients of Pima Indian heritage aged 21 and older. The goal is to predict whether a patient has diabetes (1) or not (0) based on 8 medical input features:

- Pregnancies– Number of times pregnant
- Glucose– Plasma glucose concentration
- BloodPressure– Diastolic blood pressure (mm Hg)
- SkinThickness– Triceps skin fold thickness (mm)
- Insulin– 2-Hour serum insulin (mu U/ml)
- BMI– Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction– Diabetes pedigree function (family history)
- Age– Age in years
- Outcome– Class variable (0: Non-diabetic, 1: Diabetic)

---

## Technologies Used

- Python
- Pandas / NumPy – Data processing
- Seaborn / Matplotlib– Visualization
- Scikit-learn – Machine Learning (Random Forest)
- imblearn (SMOTE)– Handling class imbalance
- Gradio – Web-based interface for model deployment

---

##  Data Preprocessing

- Replaced invalid 0 values in features like `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` with NaN.
- Imputed missing values using **mean** or median based on skewness.
- Handled class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)**.

---

## Model Training

- Model: Random Forest Classifier
- Training performed on 80% of the dataset after applying SMOTE
- Achieved high accuracy and good generalization on unseen data

---

## Gradio Interface

The model is deployed using Gradio, allowing users to input their health parameters and get real-time predictions.

###  Output:
"Diabetic"** if prediction is 1
"Not Diabetic"** if prediction is 0

