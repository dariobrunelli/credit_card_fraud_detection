# Credit Card Fraud Detection Classification

## Overview

This repository contains the implementation and documentation for a machine learning classification task on the Credit Card Fraud Detection dataset obtained from Kaggle. The primary objective is to build a robust classifier capable of distinguishing between legitimate and fraudulent credit card transactions.

## Dataset

The dataset comprises numerical features extracted from clients' credit card transactions. Each transaction is labeled as either legitimate or fraudulent. Notably, the dataset presents a significant imbalance between the two classes, posing a challenge that requires careful consideration during model development.

## Task Description

### 1. Data Exploration

- **Understanding the Structure**: The dataset is explored to gain insights into its structure and to identify any necessary data preparation steps.

### 2. Data Preparation and Model Training

- **Classifier Selection**: The classification algorithm selected for the task is Random Forest.

- **Model Training**: The selected classifier is trained using the dataset.

- **Imbalanced Dataset Handling**: The following techniques are applied to address the class imbalance and enhance model performance:  
  1. Weightd classes
  2. Random oversampling
  3. Random undersampling
  4. SMOTE - Synthetic Minority Oversampling Technique
  5. Combined approach of undersampling, SMOTE and weighted classes  
  
### 4. Deployment Strategy

A deployment strategy design with the aim of querying the trained model in real-time is suggested.

## Considerations
Some of the aforementioned techniques contribute to enhancing the model's performance.  
However, in the presence of such an imbalanced dataset, effectively tackling the challenge of minimizing both false positives (legitimate transactions classified as fraudulent) and false negatives (fraudulent transactions classified as legitimate) poses a particular difficulty.  
Given the application context, prioritizing the minimization of false negatives becomes more crucial. These represent fraudulent transactions that manage to go undetected, making it more significant to select a model proficient at identifying false negatives.

## Repository Contents

- **fraud_detection.ipynb**: Contains the implementation of the classification task.

- **README.md**: This documentation providing an introduction, task description, and instructions.
- **requirements.txt**: Contains the necessary Python modules to be installed to run the code.

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
> I ran the code on *Google Colab* from a *Google Drive* folder since it proved to be faster in training the models compared to my local CPU.
