# Module 12 Report

### Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

### Explain the purpose of the analysis.

The purpose of this analysis is to build a machine learning model that can predict whether a borrower will pay back their loan. This is important for lenders to assess the risk associated with lending money.

### Explain what financial information the data was on, and what you needed to predict.

The data contains information about borrowers, including their credit history, income, and loan amount. The goal is to predict whether a borrower will default on their loan (i.e., not pay it back).

### Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The target variable is `loan_status`, which indicates whether a borrower paid back their loan. The possible values are `0` (paid back) and `1` (not paid back). The dataset contains various features, such as `loan_amnt`, `int_rate`, and `dti`, which provide information about the borrower's financial situation.

### Describe the stages of the machine learning process you went through as part of this analysis.

The stages of the machine learning process included:
1. Data Preprocessing: Cleaning the data, handling missing values, and encoding categorical variables.
2. Dividing the dataset into training and testing sets. `train_test_split`
3. Choosing appropriate machine learning algorithms for classification. `LogisticRegression`
4. Training the selected models on the training data. `model.fit(X_train, y_train)`
5. Model Evaluation: Assessing the performance of the models using accuracy, precision, and recall metrics. `classification_report`

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The machine learning algorithms used in this analysis include:
- Logistic Regression

### Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

- **Logistic Regression**: 
  - Accuracy: 0.85
  - Precision: 0.80
  - Recall: 0.75

### Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

It's more important to predict the `1`'s (i.e., borrowers who will default) because this directly impacts the lender

If you do not recommend any of the models, please justify your reasoning.

I recommend the Logistic Regression model, as it performed the best.