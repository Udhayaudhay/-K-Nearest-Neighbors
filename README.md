
🩺 Diabetes Prediction using K-Nearest Neighbors (KNN)
📘 Overview

This project predicts whether a patient has diabetes or not using the K-Nearest Neighbors (KNN) algorithm.
The model is trained on the Pima Indians Diabetes Dataset, which contains various medical attributes such as glucose level, blood pressure, insulin, BMI, and age.

🧩 Dataset Description

The dataset consists of 768 records and 9 columns.

The Outcome column indicates:

1 → Diabetic

0 → Non-Diabetic

Input features include Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, and Age.

⚙️ Project Workflow
1️⃣ Data Collection and Preparation

The dataset is loaded and cleaned by replacing invalid or missing values.
Zero values in features such as glucose, blood pressure, and BMI are treated as missing and replaced with appropriate averages.

2️⃣ Data Splitting

The dataset is divided into training and testing subsets to evaluate model performance effectively.

3️⃣ Feature Scaling

Since KNN is a distance-based algorithm, all features are standardized to bring them to the same scale.
This ensures no single feature dominates the distance calculation.

4️⃣ Model Training (KNN Algorithm)

The K-Nearest Neighbors algorithm is applied with a chosen value of K (commonly 5).
When predicting a new sample, the model:

Calculates the distance from all training samples.

Identifies the K nearest neighbors.

Uses majority voting to determine whether the sample is diabetic or not.

5️⃣ Model Evaluation

Model performance is assessed using:

Accuracy Score

Confusion Matrix

Precision, Recall, and F1-Score

📊 Results

The KNN model achieved around 80–84% accuracy, depending on the chosen K value.

Performance may vary slightly when data is scaled or normalized differently.
