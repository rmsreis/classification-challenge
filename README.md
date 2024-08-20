## Classification Challenge: Spam Detector

This project is designed to build and evaluate two supervised machine learning models to classify emails as spam or not spam. The task simulates a real-world scenario where an Internet Service Provider (ISP) aims to improve its email filtering system.

-----

### Background

As a data scientist at an ISP, your objective is to develop a machine learning model that accurately detects spam emails, helping the ISP to filter them out of customers' inboxes. You have been provided with a dataset containing email features and labels indicating whether each email is spam or not.

### Project Structure

This project involves the following key steps:

**Data Preparation:**

- Split the data into training and testing sets.

- Scale the features for optimal model performance.

**Model Development:**

- Create and train a Logistic Regression model.

- Create and train a Random Forest model.

**Model Evaluation:**

- Evaluate the performance of both models using accuracy as the primary metric.

- Compare the results to determine which model performs better in detecting spam.

F**iles**

- `spam_detector.ipynb`: The Jupyter notebook containing the code to execute the steps mentioned above.

- Dataset URL: [Spam Data](https://example.com/spam-data)

**Instructions**

1. Split the Data into Training and Testing Sets

- Load the dataset from the provided URL into a Pandas DataFrame.

- Create the labels set (y) from the "spam" column and the features set (X) from the remaining columns.

- Check the balance of the labels using the `value_counts` function.

- Split the data into training and testing datasets using `train_test_split`.

2. Scale the Features

- Instantiate a `StandardScaler` to normalize the feature values.
- Fit the `StandardScaler` to the training data.
- Transform both the training and testing feature sets using the scaler.

3. Create a Logistic Regression Model

- Instantiate a Logistic Regression model with `random_state=1`.

- Train the model on the scaled training data (`X_train_scaled` and `y_train`).

- Make predictions on the testing data (`X_test_scaled`) and evaluate the model’s accuracy.

4. Create a Random Forest Model

- Instantiate a Random Forest model with `random_state=1`.

- Train the model on the scaled training data (`X_train_scaled` and `y_train`).

- Make predictions on the testing data (`X_test_scaled`) and evaluate the model’s accuracy.

5. Evaluate the Models

Compare the performance of the Logistic Regression and Random Forest models.

Answer the following questions:

- Which model performed better?
- How does that compare to your initial prediction?

