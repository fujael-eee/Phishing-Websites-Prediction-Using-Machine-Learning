### Phishing Website Prediction Using Machine Learning
🔹 Project Overview

Phishing websites are malicious sites designed to deceive users into revealing sensitive information such as passwords, credit card numbers, and personal data. Traditional rule-based detection methods struggle to detect newly created phishing websites due to their dynamic and evolving nature.

This project implements machine learning models to accurately predict phishing websites, providing a reliable approach to enhance online security.

🔹 Dataset

Dataset: Publicly available phishing websites dataset (features extracted from URLs, domains, and website characteristics)

Target Variable: Result

1 → Phishing

-1 → Legitimate

Note: The dataset is clean with no missing values. No additional class imbalance handling techniques were applied.

🔹 Models Implemented

Model	Description:

Random Forest: Ensemble tree-based model for robust classification
XGBoost:	Gradient boosting ensemble with strong class separation
Gradient Boosting:	Tree-based boosting model for prediction
AdaBoost:	Adaptive boosting for improving weak learners

🔹 Workflow

* Exploratory Data Analysis (EDA): Visualizing feature distributions, understanding class balance, and inspecting correlations.

* Data Preprocessing: Scaling features using StandardScaler.

* Model Training & Evaluation: Training the four models on the dataset and evaluating using metrics:

Accuracy, Precision, Recall, F1-score, ROC-AUC

Model Comparison: Random Forest achieved the most balanced performance; XGBoost had highest ROC-AUC.

🔹 Key Findings

Ensemble models perform effectively even without advanced preprocessing.

Random Forest gives the most balanced results for phishing detection.

XGBoost provides excellent class separability (high ROC-AUC).


🔹 Results

Random Forest: Accuracy = 96.7%, F1-score = 97.1%

XGBoost: Accuracy = 96.65%, ROC-AUC = 99.5%

Gradient Boosting: Accuracy = 95.97%

AdaBoost: Accuracy = 92.4%

Confusion matrices and performance metrics for each model are included in the notebook.

🔹 Conclusion

This project demonstrates that machine learning models can reliably detect phishing websites using only standard preprocessing and a clean dataset. Random Forest provides a robust balance between precision and recall, while XGBoost ensures high separability between phishing and legitimate websites.
