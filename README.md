# Credit Card Fraud Detection Classification

## Overview

This repository contains the implementation and documentation for a machine learning classification task on the Credit Card Fraud Detection dataset obtained from Kaggle. The primary objective is to build a robust classifier capable of distinguishing between legitimate and fraudulent credit card transactions.

## Dataset

The dataset comprises numerical features extracted from clients' credit card transactions. Each transaction is labeled as either legitimate or fraudulent. Notably, the dataset presents a significant imbalance between the two classes, posing a challenge that requires careful consideration during model development.

## Task Description

### 1. Data Exploration

- **Understanding the Structure**: Explore the dataset to gain insights into its structure and identify any necessary data preparation steps.

### 2. Data Preparation and Model Training

- **Classifier Selection**: Choose an appropriate classification algorithm for the task.

- **Model Training**: Train the selected classifier using the dataset.

- **Imbalanced Dataset Handling**: Apply techniques such as undersampling or oversampling to address the class imbalance and enhance model performance.

### 3. Deployment Strategy

- **Real-time Querying**: Design a deployment strategy with the aim of querying the trained model in real-time.

## Repository Contents

- **Codebase**: Contains the implementation of the classification task.

- **README.md**: This documentation providing an introduction, task description, and instructions.

## Instructions

1. Clone this repository to your local machine.

  ```
  git clone https://github.com/dariobrunelli/credit_card_fraud_detection.git
  ```
2. Download the [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/) dataset and store it in the folder where the file *fraud_detection.ipynb* is.  
3. Ensure that you have the required dependencies installed. You can install them using:

  ```
  pip install -r requirements.txt
  ```
4. Execute the code in *fraud_detection.ipynb* to perform data exploration, model training, and any other necessary tasks.  

> [!NOTE]
> I run the code with *Google Colab* from a *Google Drive* folder, as it was faster in training the models than my local CPU
