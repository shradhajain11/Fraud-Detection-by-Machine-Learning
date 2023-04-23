# Fraud-Detection-by-Machine-Learning
# Fraud Detection Model

This code reads in a dataset of financial transactions and builds a model to predict whether a given transaction is fraudulent or not.

## Dataset

The dataset used in this code is `fraud.csv`. It contains the following columns:

- `step`: This is a numerical column representing the hour in the day (0 to 23) in which the transaction occurred.
- `type`: This is a categorical column representing the type of transaction (e.g. payment, transfer, cash-out).
- `amount`: This is a numerical column representing the amount of the transaction.
- `nameOrig`: This is a categorical column representing the customer who initiated the transaction.
- `oldbalanceOrg`: This is a numerical column representing the customer's balance before the transaction.
- `newbalanceOrig`: This is a numerical column representing the customer's balance after the transaction.
- `nameDest`: This is a categorical column representing the customer who is the recipient of the transaction.
- `oldbalanceDest`: This is a numerical column representing the recipient's balance before the transaction.
- `newbalanceDest`: This is a numerical column representing the recipient's balance after the transaction.
- `isFraud`: This is a binary column representing whether the transaction was fraudulent (1) or not (0).
- `isFlaggedFraud`: This is a binary column representing whether the transaction was flagged as fraudulent (1) or not (0).

## Model

The code uses a Linear Regression model from the `sklearn` library to predict whether a given transaction is fraudulent or not. The dataset is split into training and testing sets using the `train_test_split` function, and the model is fit on the training data. The accuracy of the model is then evaluated on the testing data.
