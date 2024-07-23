# credit-risk-classification Report

Dataset
The dataset, lending_data.csv, includes various features related to loan applications. The target variable, loan_status, indicates the health of the loan.

Methodology
The project follows these steps:

Data Preparation:
Load the data
Create feature (X) and target (y) datasets
Split the data into training and testing sets
Model Training with Original Data:
Train a logistic regression model on the original dataset
Evaluation:Assess the model's performance using accuracy, precision, recall, and F1 score
Resampling:Balance the training data using RandomOverSampler to address class imbalance
Model Training with Resampled Data:Train a logistic regression model on the resampled dataset
Evaluation and Comparison:Evaluate and compare the performance of the model trained on resampled data with the one trained on the original data

Results
The model trained on the original data showed high accuracy for the majority class but lower performance metrics for the minority class.
After resampling, the model displayed improved recall for the minority class, indicating enhanced capability in identifying high-risk loans, with a slight trade-off in precision.
Conclusion
Resampling techniques, such as oversampling the minority class, can significantly improve the performance of logistic regression models in predicting minority classes in imbalanced datasets. This approach led to a more balanced model capable of detecting high-risk loans more effectively.

Requirements
Python 3.x
pandas
numpy
scikit-learn
imbalanced-learn
