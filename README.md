# Credit Card Fraud Detection

## Overview
The Credit Card Fraud Detection dataset, sourced from a research collaboration, contains transactions made by European cardholders in September 2013. This dataset includes 284,807 transactions, among which 492 are fraudulent, representing only 0.172% of the transactions. The dataset is highly imbalanced, which is typical for fraud detection scenarios.

The dataset contains numerical features resulting from a Principal Component Analysis (PCA) transformation. This means the original data has been transformed into a set of principal components, making it difficult to interpret the features directly. The dataset contains the following features:

- **Time**: The seconds elapsed between this transaction and the first transaction in the dataset.
- **V1 to V28**: The principal components obtained with PCA. These features are anonymized to preserve privacy.
- **Amount**: The transaction amount, which can be used for example-dependent cost-sensitive learning.
- **Class**: The response variable, where:
  - `1` indicates a fraudulent transaction.
  - `0` indicates a non-fraudulent transaction.

This dataset is widely used to benchmark fraud detection algorithms due to its challenging nature and high level of anonymization and privacy.

**Best Model Performance Metrics** (Weighted Avg):

   - **Accuracy**: 0.9991573329588147
   - **Precision**: 0.7049180327868853
   - **Recall**: **0.8775510204081632**
   - **F1 Score**: 0.7818181818181819

     ![Confusion_Matrix_XGBoost](https://github.com/user-attachments/assets/d27b8286-a5d3-4636-9ebc-8e866f28958e)


## Model Performance Comparison

| Model                   | Accuracy | Precision | Recall | F1 Score |
|-------------------------|----------|-----------|--------|----------|
| **Random Forest**       | 0.9994   | 0.8511    | 0.8163 | 0.8333   |
| **FFN DL Model**        | 0.9993   | 0.7810    | 0.8367 | 0.8079   |
| **XGBoost**             | 0.9992   | 0.7049    | **0.8776** | 0.7818   |
| **LightGBM**            | 0.9954   | 0.2595    | 0.9082 | 0.4036   |
| **Logistic Regression** | 0.9731   | 0.0558    | 0.9184 | 0.1053   |
| **IsolationForest**     | 0.9700   | 0.0400    | 0.8180 | 0.0800   |


## Files

- `model/`: Exported model files.
- `dataset/creditcard.parquet`: Dataset containing credit card transaction details.
- `images/`: Confusion Matrix for all models.

## Dataset

- The dataset (`dataset/creditcard.parquet`) contains anonymized credit card transaction data.

---
