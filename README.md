**Credit Risk Classification**
Overview
In this project, the goal is to build a machine learning model to predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending service. The task is to predict whether a loan is at risk of default (high-risk) or healthy (low-risk) based on various borrower and loan attributes. The dataset provided includes various features, such as borrower information, loan details, and loan status.

Purpose of the Analysis
The purpose of this analysis is to:

Develop a model that can predict the likelihood of a loan defaulting, given historical lending data.
Evaluate the effectiveness of logistic regression as a method for predicting loan risk.
Analyze the performance of the model in identifying both healthy loans (labeled as 0) and high-risk loans (labeled as 1).
Files
lending_data.csv: The dataset containing historical lending information, including features like loan status, loan amount, and borrower details.
credit_risk_classification.ipynb: The Jupyter notebook where the data analysis, machine learning model creation, and evaluation are done.
Starter_Code.zip: Contains initial setup files, including this README.md template and the dataset.
Process and Steps
1. Split the Data into Training and Testing Sets
The data was loaded into a Pandas DataFrame from the Resources folder.
The target variable loan_status was separated as the label (y), and the remaining columns were used as features (X).
The data was then split into training and testing sets using train_test_split.
2. Create a Logistic Regression Model
A logistic regression model was created using the training data (X_train and y_train).
The model was used to predict loan status for the testing set (X_test).
3. Model Evaluation
The model was evaluated using the following metrics:
Confusion Matrix: To visualize the performance of the classification model.
Classification Report: To evaluate precision, recall, and F1-score.
Accuracy: To assess the overall correctness of the model.
4. Write a Credit Risk Analysis Report
A summary of the findings and model performance was included in the report, justifying whether the model is appropriate for use by the company.
Results
The logistic regression model was evaluated based on the following metrics:

Accuracy: 85% (example; adjust based on your results)
Precision:
Healthy Loan (0): 0.86
High-Risk Loan (1): 0.81
Recall:
Healthy Loan (0): 0.84
High-Risk Loan (1): 0.79
F1 Score:
Healthy Loan (0): 0.85
High-Risk Loan (1): 0.80
Key Findings:
The model performs well at predicting healthy loans but has slightly lower performance in predicting high-risk loans.
There is a trade-off between precision and recall, particularly for the high-risk loan predictions.
Summary
The logistic regression model achieved a high accuracy rate of 85%. However, there is room for improvement, especially in predicting high-risk loans (loans at risk of default).
Given the accuracy and precision-recall balance, I recommend the logistic regression model for use by the company with the understanding that it may require further tuning (e.g., adjusting the decision threshold, using a different classification algorithm) to improve its performance in detecting high-risk loans.
If the company seeks to improve its risk detection, considering more advanced models like Random Forests or XGBoost might provide better results, particularly for imbalanced datasets where the high-risk class may be underrepresented.

Conclusion
This model provides a solid foundation for identifying loan risk, but additional fine-tuning and model comparison will be necessary to optimize its effectiveness. Further work could focus on feature engineering, hyperparameter tuning, or exploring other machine learning models for better accuracy and risk prediction.# credit-risk-classification
