# Transactional Fraud Detection

## Overview

Transactional Fraud Detection is a machine learning project aimed at detecting fraudulent transactions in financial data. This project utilizes advanced algorithms and techniques to identify anomalous patterns and flag potential fraudulent activities, thus helping financial institutions mitigate risks and protect their customers.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Dataset](#dataset)
6. [Models](#models)
7. [Evaluation](#evaluation)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction

Fraudulent transactions pose significant challenges for financial institutions, leading to financial losses and reputational damage. Transactional Fraud Detection employs machine learning algorithms to analyze transactional data and distinguish legitimate transactions from fraudulent ones. By leveraging predictive models and anomaly detection techniques, this project aims to enhance fraud detection capabilities and improve fraud prevention strategies.

## Features

- Preprocessing of transactional data
- Training and evaluation of machine learning models
- Anomaly detection and fraud prediction
- Visualization of results
- Flexible and customizable architecture

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/hellybrine/TransactionalFraudDetection.git
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Navigate to the project directory:
   ```
   cd TransactionalFraudDetection
   ```

2. Run the main script:
   ```
   python main.py
   ```

3. Follow the prompts to preprocess data, train models, and evaluate performance.

## Dataset

The dataset comprises transactions that occurred over a span of two days, totaling 284,807 transactions. Among these transactions, there were 492 instances of fraud. As a result, the dataset is highly unbalanced, with fraudulent transactions accounting for only 0.172% of all transactions.

The dataset consists solely of numerical input variables, derived from a Principal Component Analysis (PCA) transformation. Due to confidentiality concerns, the original features and further background information about the data cannot be disclosed. However, features labeled as V1 through V28 represent the principal components obtained through PCA. Notably, the features 'Time' and 'Amount' were not subjected to PCA transformation.

The 'Time' feature denotes the elapsed time in seconds between each transaction and the initiation of the dataset, serving as a temporal indicator. On the other hand, the 'Amount' feature denotes the monetary value of each transaction, offering potential utility for context-dependent cost-sensitive learning.

The response variable, denoted by 'Class', is binary, with a value of 1 representing a fraudulent transaction and 0 representing a legitimate transaction.
It can be sourced from Kaggle at the following link: [on Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## Models

Transactional Fraud Detection employs various machine learning models, including:
- Logistic Regression
- Random Forest
- Support Vector Machines (SVM)
- Neural Networks
- Gradient Boosting

## Evaluation

The performance of each model is evaluated based on metrics such as precision, recall, and F1-score. Additionally, ROC curves and confusion matrices are used to assess model performance and identify trade-offs between true positive and false positive rates.

## Contributing

Contributions to Transactional Fraud Detection are welcome! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request on GitHub.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
