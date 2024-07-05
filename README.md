# Credit Card Fraud Detection

## Overview

This project implements a credit card fraud detection system using machine learning techniques. The model predicts whether a transaction is fraudulent or not.

**Outstanding Performance Metrics** (Weighted Avg):

   - **Accuracy**: 0.9999205662742052
   - **Precision**: 0.9998416830847171
   - **Recall**: 1.00
   - **F1 Score**: 0.9999208352758011

**Confusion Matrix**:

  ![Confusion_Matrix_Random_Forest](https://github.com/hpluwang/credit_card_fraud_detection/assets/53874420/1d6335ca-abe7-418b-b4a3-6a73c4d37370)

## Files

- `model/credit_card_model_rf.pkl`: Trained Random Forest model for fraud detection.
- `dataset/creditcard.parquet`: Dataset containing credit card transaction details.

## Usage

1. **Requirements**

   Ensure you have Python 3.7+ installed. Install dependencies using `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

2. **Model Loading**: Load the trained model from `model/credit_card_model_rf.pkl`.

   ```python
   import joblib

   # Load the model
   model = joblib.load('model/credit_card_model_rf.pkl')
   ```

3. **Prediction**: Use the loaded model to predict fraudulence on new data.

   ```python
   # Example of prediction
   new_data = ...  # Load or generate new data
   prediction = model.predict(new_data)
   ```

## Dataset

- The dataset (`dataset/creditcard.parquet`) contains anonymized credit card transaction data.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---
