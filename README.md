## Overview of the Analysis

The purpose of this analysis was to evaluate whether or not it would be ideal to lend a loan out to certain borrowers based on specific factors including financial information along with loan status. 
Provided financial information in the dataset included:
- Loan size
- Loan interest rate
- Borrower income
- Borrower debt-to-income ratio
- Number of borrower accounts
- Derogatory marks
- Total borrower debt

The main objective was to predict the amount of healthy (0) loans and high-risk (1) loans based on the provided financial data.

One of the main variables involved was *"loan_status"* - I had to separate it from the rest of the data and use a prediction method for the remaining data to determine the accuracy of loan prediction.
The stages that I went through during this analysis included:
- Using 'train_test_split' to split the loan status variable apart from the rest of the financial data in the dataset
    - Loan status was assigned to a y variable
    - The remaining finacial data was assigned to an X variable
- Using 'LogisticRegression' to fit the two variables
- Using 'logistic_regression_model' to use the two varibales to predict loan status

Once those algorithms were implemented, I then used 'classification_report' to print the accuracy, precision and recall scores from the predicted data.  

## Results

* **Classification Report:**
    * Accuracy score: 99%
    * Precision score:
      * 0 - 100%
      * 1 - 86%
    * Recall score:
      * 0 - 99%
      * 1 - 94%

## Summary

Based on the results from the classification report, it is extremely reliable for predicting healthy and high-risk loans. 

* The accuracy score is extremely high along with the precision ad recall scores for the healthy loans. 
* Although the scores for the high-risk loans are not as high as those for the healthy loans, they are still high enough to warrant implementation of the classification report model.
* It is vital to ensure that high-risk loans are as accurate as possible in order to prevent borrowers from falling into unsustainable debt.
  Therefore, this model should certainly still be used for prediction both 0 and 1 loans, but further analysis might be necessary for predicting 1 loans.
