# Credit Card Default Prediction
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

### Gradient Boosting: .826
  The hypothesis for the Gradient Boosting model was similar to the thoughts of deploying the AdaBoost model due to the general principles that it should be less prone to overfitting and handles mixed data 
  types well.

  Overall the Gradient Boost model was our highest performing model with both the Training and Testing Scores, proving our hypothesis true when looking at our dataset and the benefits of the model framework. 
### Random Forest: .665
Random Forest models can be used for both classification and regression tasks. Since we are trying to predict the likelihood of default, we should use a classifier, as the final output is a discrete label/category.

Random Forest modeling generally provides high accuracy even when using diverse or incomplete datasets. Because it uses random feature selection, it should resist overfitting data as well.

As predicted, we were able to attain a reasonable degree of accuracy, but it was not precise enough for our needs. Even adjusting the max depth of the trees, the number of estimators, and the minimum number of samples required for a split failed to improve performance.

### Extra Trees Classifier: .820
  The Extra Trees Classfier performed poorly out of the gate, coming in severely overfit with a 99.9% training score.  While the model performed much better after the SMOTE technique was applied, it was still 
  not our top performing model with this dataset.

  Initially we assumed the model would perform well due to the fact that it is generally good with noisy or high-dimensional data.

  Overall with this dataset, the Extra Trees Classifier stumbled initially with the imbalanced target data and still showed some weakness with the SMOTE technique due to the reletively high dimensional data. 
### Adapted Boosting Classifier: .820
  With fewer hyperparameters to tune and the model less prone to overfitting, the hypothesis was that the model should perform well.

  Overall, the model performed well and the hypothesis proved to be true.  The AdaBoost model improved our accuracy and seemed to handle the imbalanced data much better than others explored. 

### Decision Tree: .724
he Decision Tree model was one of the top performing models with a 72.41% Accuracy Score. Initially this was the highest performing model. 

We tried a multitude of techniques to get the accuracy score higher. Examples of this include resampling using SMOTE, testing scaled vs. unscaled data and removing a variety of variables.

Ultimately, this model wasn’t performing quite up to our standards. All of the techniques we used could not bring the accuracy score above a 0.7241. 

### Logistic Regression: .600
The Logistic Regression model was one of our weakest models with an ROC AUC Score of 60%, which ran on scaled/cleaned data.

Initially, we did not have strong confidence in the model due to the hypothesis that the feature set may be too complex.

he hypothesis proved true when analyzing the score, pointing us to explore more advanced models like the decision trees, random forests and gradient boosting classifers.

## Results
The results suggest that Gradient Boosting is a powerful technique for classification tasks, offering several benefits. It excels at capturing complex patterns in the data, as evidenced by its superior performance compared to other models. Additionally, Gradient Boosting is robust against overfitting and can handle high-dimensional datasets effectively. Overall, these findings highlight the benefits of using Gradient Boosting for classification tasks, especially when dealing with complex datasets where accurate predictions are crucial.




