# Elevate-Labs-AIML-Internship-Task4
## Breast Cancer Classification using Logistic Regression


This project builds a binary classification model using Logistic Regression to predict whether a tumor is malignant (cancerous) or benign (non-cancerous) based on medical features.

__Objective__

Perform binary classification using Logistic Regression
Apply preprocessing and feature scaling
Evaluate model using classification metrics
Understand sigmoid function and threshold tuning

__Tools & Technologies__

Python
Pandas
NumPy
Scikit-learn
Matplotlib

__Dataset Description__

Features: 30 numerical attributes (radius, texture, area, etc.)
Target: diagnosis
M → 1 (Malignant)
B → 0 (Benign)

__Steps Performed__

1. Data Preprocessing
Removed irrelevant columns (id, Unnamed: 32)
Converted categorical target to numeric (M → 1, B → 0)
Checked and handled missing values
2. Feature Scaling
Applied StandardScaler to normalize feature values
3. Model Training
Split dataset into training (80%) and testing (20%)
Trained Logistic Regression model
4. Evaluation Metrics
Confusion Matrix
Precision, Recall, F1-score
ROC-AUC Score
5. Threshold Tuning
Adjusted classification threshold from default (0.5) to 0.4
Improved balance between precision and recall

__Results & Performance__

🔹 ROC-AUC Score
0.997 → Excellent model performance
🔹 Confusion Matrix (Threshold = 0.4)
[[70  1]
 [ 1 42]]
🔹 Classification Report
Accuracy: 98%
Precision: 0.98 – 0.99
Recall: 0.98 – 0.99
F1-score: 0.98

__Key Insights__
Model achieves very high accuracy and near-perfect classification
Only 2 misclassifications out of 114 samples
Logistic Regression performs exceptionally well on this dataset
Threshold tuning helps balance false positives and false negatives
