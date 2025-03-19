The purpose of this analysis is to assess the creditworthiness of borrowers using a logistic regression model. The dataset consists of historical lending data, where:

A loan_status of 0 represents a healthy loan (low risk of default).
A loan_status of 1 represents a high-risk loan (higher probability of default).
By building a predictive model, we aim to help the lending company determine the likelihood of a borrower defaulting on their loan.

Results
The logistic regression model was evaluated based on accuracy, precision, and recall:

Overall Accuracy: 99.22% → The model is highly accurate in predicting loan status.

Healthy Loans (0):

Precision: 99.69% → When the model predicts a loan is healthy, it's correct 99.69% of the time.
Recall: 99.50% → The model correctly identifies 99.50% of actual healthy loans.
F1-score: 99.60% → A strong balance between precision and recall.
High-Risk Loans (1):

Precision: 86.01% → When the model predicts a loan is high-risk, it's correct 86.01% of the time.
Recall: 90.93% → The model correctly identifies 90.93% of all actual high-risk loans.
F1-score: 88.40% → A decent balance between precision and recall.

The logistic regression model is highly effective at identifying healthy loans (0) with near-perfect precision and recall. It also does a fairly good job detecting high-risk loans (1), but I believe there is some room for improvement.

If the company prioritizes identifying safe borrowers and minimizing unnecessary rejections, this model is a great choice due to its high accuracy and precision for healthy loans.
However, if catching risky borrowers is the top priority, the model could be improved. Although it identifies 90.93% of high-risk loans, it sometimes misclassifies risky borrowers as safe.

I would recommend this model for general use, but with some caution when identifying high-risk borrowers.
