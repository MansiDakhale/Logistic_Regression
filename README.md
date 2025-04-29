# Logistic_Regression

Logistic Regression for Binary Classification


This project demonstrates the use of Logistic Regression for binary classification on the Breast Cancer Wisconsin Dataset. The objective is to predict whether a tumor is malignant or benign based on the features of the cancer cell images.

Steps Performed:
1. Dataset Loading and Preprocessing
Dataset: The Breast Cancer Wisconsin dataset was loaded using sklearn.datasets.load_breast_cancer().

Features and Target: We extracted the features (X) and target (y) from the dataset:

Features (X): 30 numerical features computed from breast cancer cell images.

Target (y): Binary labels (0 for benign, 1 for malignant).

2. Train-Test Split
The dataset was split into a training set (80%) and a testing set (20%) using train_test_split().

3. Feature Scaling
Features were standardized using StandardScaler() to normalize the data before applying the logistic regression model. This helps to speed up convergence during training and ensures that all features contribute equally.

4. Model Training
A Logistic Regression model was trained on the preprocessed data using sklearn.linear_model.LogisticRegression().

5. Model Evaluation
The model was evaluated using various metrics:

Confusion Matrix: To understand the performance of the classification model.

Precision and Recall: To evaluate the accuracy of predictions (especially for imbalanced classes).

ROC-AUC Curve: To visualize the trade-off between true positive rate and false positive rate at various thresholds.

6. Threshold Adjustment
The model's decision threshold was adjusted to optimize the balance between precision and recall, depending on the use case.