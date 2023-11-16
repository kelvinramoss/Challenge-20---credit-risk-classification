# Challenge-20---credit-risk-classification

# Instructions

## Split the Data into Training and Testing Sets

1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

3. Split the data into training and testing datasets by using train_test_split.

## Create a Logistic Regression Model with the Original Data

1. Fit a logistic regression model by using the training data (X_train and y_train).

2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

3. Evaluate the model’s performance by doing the following:

    - Generate a confusion matrix.

    - Print the classification report.

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

## Write a Credit Risk Analysis Report

Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository, including:

    - An overview of the analysis: Explain the purpose of this analysis.

    - The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

    - A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.


 # Credit Risk Analysis Report   

 ## Overview
 The main goal of this challenge is to analize if the Logistic Regression machine learning model can better predict loans that are safe versus those that are risky, checking if using the original dataset or a bigger dataset makes the predictions more accurate.

## Results

- Model 1

Accuracy score: The first model shows an accuracy score of 0.95 (95%), which indicates a very good effectiveness. 

Precision score: Related to low risk class the precison is 1.00, which is almost always accurate. However, for high risk class, the precision is 0.85, which means that 85% of the time the predictions made were correct.

Recall score: Overall, for low risk class, the recall rate is 1.00, meaning that 100% of the low-risk cases were correctly identified. However, for high risk the recall rate is 0.88, which means that 88% of the cases were identified.

- Model 2 

Accuracy score: The first model shows an accuracy score of 0.99 (99%), which indicates high performance and precision.

Precision score: Regarding to low risk class the precison is 1.00, which is almost always accurate. However, for high risk class, the precision is 0.84 which means that 84% of the time the predictions made were correct.

Recall score: Overall, for low risk class, the recall rate is 0.99, meaning that 99% of the low-risk cases were correctly identified. However, for high risk the recall rate is 0.99, which means that 99% of the cases were identified.


## Summary

Model 2 outperforms Model 1 in terms of accuracy, precision, and recall. It's evident that Model 2's improved performance is directly linked to having a balanced dataset. Meanwhile, Model 1, despite also exhibiting a high accuracy level, remains effective in identifying high-risk loans. Overall, both models using Logistic Regression show strong performance.