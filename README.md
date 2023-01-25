# Credit_Risk_Analysis

Jill applauds me for all your efforts. Little by little, I built up my skills in data preparation, statistical thinking, and machine learning. Now are ready to apply machine learning to solve real-world problems.

Credit risk is an inherently unbalanced classification problem, with good credit easily overtaking bad credit. Credit risk is the risk that a borrower will default on a loan, credit card, or other type of credit facility. Credit risk is an important issue in finance as banks and other financial institutions invest heavily in reducing credit risk.

## Overview of the loan prediction risk analysis:
When preparing both data sets, we checked variables such as value_counts to show the balance of labels for each category. Since there was an imbalance between the 1s and 0s in the original data set, we resampled the data and used the RandomOverSampler module to randomly select instances of the minority class (i.e. 1s) and divide the majority and minority We added them to the training set until they were balanced. class.

Before this step, we use train_test_split to split the data into training and test sets so that we can train a logistic regression model on the trying data and evaluate the model on the test data. This allows unbiased evaluation of the model.

We then fit the model to the training data so that the model can mathematically learn and adapt to best represent that data, and finally we can use the test data to make predictions. increase. This allows us to better assess how well the model performs on new data.

## Results
# Machine learning model 1:
original recordIn contrast, out of all the times  the model predicted a value of 1 (high-risk loans), only 85% of those predictions were correct.This model is much better at predicting sound loans than risky onesMachine learning 

# Model 2:
Randomly Oversampled DatasetThis means that approximately 99.37% of the transactions in the test data were correctly classified by the model.This means that out of all the times  the model predicted test data observations with a  value of 0, 100% of those predictions were correct.This means that out of all the times  the model predicted test data observations with a  value of 0, 100% of those predictions were correct.In contrast, out of all the times  the model predicted a score of 1 (risky loans), only 84%  of those predictions (slightly worse) were correct.

## Summary
Therefore, the second model is recommended to for use when flagging people that may pose a high-risk when applying for loans as healthy loans easily outnumber risky loans so it is important to identify the latter.
