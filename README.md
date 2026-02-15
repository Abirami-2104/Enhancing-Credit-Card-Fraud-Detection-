💳** Credit Card Fraud Detection using Ensemble Learning**
📖 Overview

This project presents an end-to-end machine learning pipeline for detecting fraudulent credit card transactions using ensemble learning techniques. Since fraud detection datasets are highly imbalanced, special resampling and evaluation strategies were implemented to improve minority class prediction performance.

The model was trained and evaluated on two real-world datasets to ensure robustness and generalization.

🎯 Problem Statement

Credit card fraud detection is a classification problem where fraudulent transactions represent a very small percentage of total transactions. Traditional models often fail to correctly classify minority (fraud) cases.

This project focuses on:

Handling class imbalance effectively

Improving fraud detection recall

Ensuring model interpretability

📂 Datasets Used

European Credit Card Transactions Dataset

Sparkov Financial Fraud Detection Dataset

Both datasets include transaction-level details such as transaction amount, customer features, and transaction categories.

🛠️ Tech Stack

Language: Python

Libraries Used:

Pandas & NumPy

Scikit-learn

XGBoost

CatBoost

Imbalanced-learn (SMOTEENN)

SHAP

Matplotlib & Seaborn

⚙️ Methodology
1️⃣ Data Preprocessing

Checked for missing values and duplicates

Outlier detection using IQR and Z-score methods

Feature scaling using StandardScaler

2️⃣ Handling Class Imbalance

Applied SMOTEENN (Synthetic Minority Oversampling + Edited Nearest Neighbors) to:

Increase minority class samples

Remove noisy majority class samples

Improve fraud detection recall

3️⃣ Model Development

Implemented:

XGBoost Classifier

CatBoost Classifier

Used 10-Fold Cross Validation for reliable model evaluation.

4️⃣ Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

ROC-AUC

The ensemble models achieved approximately 99% accuracy, with strong fraud detection capability.

5️⃣ Model Interpretation

SHAP (SHapley Additive Explanations) for feature importance

Partial Dependence Plots (PDP) for understanding feature impact

Identified key fraud-driving features such as transaction amount and transaction category

📊 Results

Significant improvement in fraud detection after applying SMOTEENN

Balanced Precision and Recall values

Consistent performance across both datasets

Improved model interpretability using SHAP

📌 Key Highlights

✔ End-to-end ML pipeline
✔ Imbalance handling using hybrid resampling
✔ Ensemble learning models
✔ Explainable AI integration
✔ Cross-dataset validation

🚀 Future Enhancements

Hyperparameter tuning using Optuna

Real-time deployment using Flask/FastAPI

Model monitoring and drift detection

Integration into banking fraud monitoring systems

👩‍💻 Author

Abirami S
M.Sc Data Science
SASTRA Deemed University
