# credit-risk-classification
<h1>Credit Risk Analysis Report</h1>
<h3>Overview</h3>
The purpose of this analysis was to develop a machine learning model capable of predicting whether a loan is "risky" (high-risk) or "safe" (healthy). This is important for banks and financial companies because it helps them identify risky loans early and avoid potential losses. The data used for this analysis consisted of financial information from loan applications, with the target variable being loan_status, where 0 represented healthy loans and 1 represented high-risk loans. The dataset was imbalanced, with the majority of loans being healthy, and included various financial attributes, such as applicant details and loan characteristics, as predictors.

To conduct the analysis, the data was preprocessed by splitting it into features (X) and labels (y). Then, the dataset was divided into a training set (80% of the data) to teach the program and a testing set (20%) to check how well it worked. A logistic regression model was chosen because it’s simple and effective for problems where you’re predicting one of two outcomes. After training the model on the training data, it was tested to see how well it could predict the loan statuses. Key metrics like accuracy, precision, recall, and F1-score were used to measure how well the program performed. Overall, the model worked well, making it a good tool for predicting whether a loan is risky or safe.

<h3>Results</h3>

- Accuracy: 99%
- Precision:
    - Healthy loans (0): 1.00
    - High-risk loans (1): 0.84
- Recall:
    - Healthy loans (0): 0.99
    - High-risk loans (1): 0.94

<h3>Summary</h3>
The logistic regression model achieved outstanding overall performance, with an accuracy of 99%. It predicted a healthy loans (class 0), achieved perfect precision (1.00) and almost perfect recall (0.99), indicating that it correctly identifies almost all healthy loans without misclassification. For high-risk loans (class 1), the model performed slightly less precisely, with a precision of 0.84, meaning some loans were incorrectly flagged as high-risk. However, its recall for high-risk loans was strong at 0.94, ensuring the model successfully identified the majority of the high-risk loans.

This performance demonstrates the model's reliability, particularly for detecting high-risk loans, which is crucial for minimizing financial risk. While the lower precision for high-risk loans may lead to some false positives, the high recall ensures most high-risk loans are identified, making the model suitable for scenarios where identifying potential risks is a priority. If minimizing false positives is critical, further adjustments or complementary models might be explored, but the current model is a strong candidate for predicting loan statuses effectively.

----------------------------------------------------------------

<h1>Instructions</h1>
The instructions for this Challenge are divided into the following subsections:

- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Write a Credit Risk Analysis Report

<h3>Split the Data into Training and Testing Sets</h3>
Open the starter code notebook and use it to complete the following steps:

1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

<b>NOTE<b>: A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

3. Split the data into training and testing datasets by using train_test_split.

<h3>Create a Logistic Regression Model with the Original Data</h3>
Use your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the training data (X_train and y_train).
2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
3. Evaluate the model’s performance by doing the following:
    - Generate a confusion matrix.
    - Print the classification report.

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

<h3>Write a Credit Risk Analysis Report</h3>
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

1. <b>An overview of the analysis:</b> Explain the purpose of this analysis.

2. <b>The results:</b> Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

3. <b>A summary:</b> Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

