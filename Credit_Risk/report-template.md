## Overview of the Analysis

* This challenge's purpose is to train and evaluate data based on loan risk to identify the creditworthiness of borrowers. 
* The dataset is comprised of historical lending activity from a peer-to-peer lending services company. 
* The independent variables(X) are 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income', 'num_of_accounts', 'derogatory_marks', and 'total_debt'.
* The dependent variable(y) is 'loan_status'.
* MACHINE LEARNING PROCESS:
    * Separate the data into X and y DataFrames.
    * "Split" the data into training and testing datasets using the train_test_split module from sklearn.
    * Create a Logistic Regression Model with the original data(training data) using the LogisticRegression() module from sklearn.
    * Fit the Logistic Regression model with the training data.
    * Make a prediction using the testing data.
    * Generate a confusion matrix to see the number of TPs, FNs, FPs, and TNs.
    * Print the classification report to analyze the data.


## Results

* Machine Learning Model 1 Scores:
    * Accuracy - .99
        This means that ~99% of the total objects in the data was correctly classified
    * Precision in healthy loan - 1.00
        This score suggests that 100% of the true positives were correctly classified in the True Positive class. 
    * Precision in loan risk - .85
        This score suggests that ~85% of the true negatives were correctly classified in the True Negative class.
    * Recall in healthy loan - .99
        This score means that ~99% of the positives were correctly identified.
    * Recall in loan risk - .91
        This score means that ~91% of the negatives were correctly identified.
    * f1-score for healthy loan - 1.00
    * f1-score for loan rish - .88
        The f1 score for healthy loans suggest that ~100% of positive predictions were correct and that ~88% of negative predictions were correct.

## Summary

* This is a great model for the company to use because it provides a straigtforward analysis of the data that was given. We can see the measures for which the variables contribute loan risk and how significant those measures are. However, this model does not compare the effects of individual independent variables on the dependent variable.
* It is useful for a company like this one to get the most accurate data for creditworthy users so they don't enroll people who are actually high-risk borrowers. This is a good model in that respect because the logistic regression almost completely accounted for all creditworthy borrowers. 

