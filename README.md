# Credit Card Fraud Detection

## Overview
The Credit Card Fraud Detection dataset, sourced from a research collaboration, contains transactions made by European cardholders in September 2013. This dataset includes 284,807 transactions, among which 492 are fraudulent, representing only 0.172% of the transactions. The dataset is highly imbalanced, which is typical for fraud detection scenarios.

The dataset contains numerical features resulting from a Principal Component Analysis (PCA) transformation. This means the original data has been transformed into a set of principal components, making it difficult to interpret the features directly. The dataset includes:

Time: The seconds elapsed between this transaction and the first transaction in the dataset.
V1 to V28: The principal components obtained with PCA. These are anonymized features.
Amount: The transaction amount, which can be used for example-dependent cost-sensitive learning.
Class: The response variable, where 1 indicates fraud and 0 indicates a non-fraudulent transaction.
This dataset is widely used to benchmark fraud detection algorithms due to its challenging nature and high level of anonymization and privacy.

**Best Model Performance Metrics** (Weighted Avg):

   - **Accuracy**: 0.9991573329588147
   - **Precision**: 0.7049180327868853
   - **Recall**: **0.8775510204081632**
   - **F1 Score**: 0.7818181818181819

## Files

- `model/`: Exported model files.
- `dataset/creditcard.parquet`: Dataset containing credit card transaction details.

## Dataset

- The dataset (`dataset/creditcard.parquet`) contains anonymized credit card transaction data.

---
