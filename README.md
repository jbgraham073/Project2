# Project_2: Credit Card Default Prediction Model
AI Bootcamp Group Project 2

---
## Project Overview

This project focuses on developing predictive models to identify the likelihood of credit card default among users. Utilizing a dataset comprising various user attributes and historical financial behavior, we aim to employ machine learning techniques to forecast potential defaults. This initiative seeks to aid financial institutions in mitigating risks and making informed decisions regarding credit lending.

## Dataset

The dataset used for this project contains information on credit card users, including demographic data, credit history, payment records, and bill statements. It encompasses a wide range of attributes that are crucial for analyzing and predicting default behavior.

### Features

- `ID`: Unique identifier for each customer
- `LIMIT_BAL`: Amount of given credit (in New Taiwan dollars)
- `SEX`: Gender (1 = male; 2 = female)
- `EDUCATION`: Level of education (1 = graduate school; 2 = university; 3 = high school; 4 = others)
- `MARRIAGE`: Marital status (1 = married; 2 = single; 3 = others)
- `AGE`: Age in years
- `PAY_0` to `PAY_6`: Repayment status in past months
- `BILL_AMT1` to `BILL_AMT6`: Amount of bill statement (NT dollar)
- `PAY_AMT1` to `PAY_AMT6`: Amount of previous payment (NT dollar)
- `default.payment.next.month`: Default payment (1 = yes, 0 = no)

### Source

[Kaggle Default of Credit Card Clients in Taiwan](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)


## Data Overview

### Collection
We found inconsistencies in variable columns, such as unexpected values like 0 in the marriage status column which should’ve only contained 1,2 and 3. We removed rows with unknown values and eliminated the customer ID column to prevent potential model disruptions.

### Clean Up
We found inconsistencies in variable columns, such as unexpected values like 0 in the marriage status column which should’ve only contained 1,2 and 3. We removed rows with unknown values and eliminated the customer ID column to prevent potential model disruptions.

### Exploration
We explored the dataset by leveraging supervised learning models which included Decision Tree, Logistic Regression, Extra Trees Classifier, Gradient Boosting, and more


## Model Overview & Evaluation

In this project, we evaluated several supervised learning models, including Decision Tree, Logistic Regression, Extra Trees Classifier, and Gradient Boosting. Among these, the Gradient Boosting model stood out, achieving the highest performance with a training score of 0.823 and a testing score of 0.826. This indicates that Gradient Boosting is well-suited for this dataset and outperformed other models in terms of classification accuracy.

- Gradient Boosting: .826
- Random Forrest: .820
- Extra Trees Classifier: .820
- Adapted Boosting Classifier: .820
- Decision Tree: .724
- Logistic Regression: .600

The results suggest that Gradient Boosting is a powerful technique for classification tasks, offering several benefits. It excels at capturing complex patterns in the data, as evidenced by its superior performance compared to other models. Additionally, Gradient Boosting is robust against overfitting and can handle high-dimensional datasets effectively. Overall, these findings highlight the benefits of using Gradient Boosting for classification tasks, especially when dealing with complex datasets where accurate predictions are crucial.




