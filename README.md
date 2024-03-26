# Project_2
AI Bootcamp Group Project 2
Creating a README file is a crucial step for documenting your project on building models for credit card default prediction. Below is a template you can customize and expand based on your project's specifics. This README aims to be clear, concise, and informative for anyone who wants to understand, use, or contribute to your project.

---

# Credit Card Default Prediction Model

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

Provide information about where the dataset comes from, any necessary citations, and if there are any restrictions on its use.

## Installation

Instructions on setting up the project environment:

```bash
git clone https://github.com/yourrepository/CreditCardDefaultPrediction.git
cd CreditCardDefaultPrediction
pip install -r requirements.txt
```

## Usage

Detailed steps on how to run the model:

```bash
python model_train.py
python model_evaluate.py
```

## Model Overview

Briefly describe the model(s) you've experimented with, including their type (e.g., logistic regression, random forest, neural networks), key features, and rationale for selection.

### Training

Discuss the training process, including any data preprocessing, feature engineering, and model tuning techniques employed.

### Evaluation

Explain the evaluation metrics (e.g., accuracy, F1-score, ROC AUC) and the performance of the model.

## Results

Summarize the results, including key findings and any limitations encountered during the project.

## Contributing

Guidelines for contributing to the project, including coding standards, pull request process, etc.

## License

Specify the license under which the project is released, such as MIT, GPL, etc.

## Contact

Provide information on how to reach you for further inquiries or contributions to the project.

---

Remember to keep your README updated as your project evolves. It's the first place people will look to understand what your project does, how they can use it, or how they can contribute.
