# Depression Predictor

This project uses machine learning to predict the likelihood of depression among students based on various lifestyle and academic factors.

---

## Project Overview

This study analyzes a dataset of students, exploring how factors such as stress, satisfaction, sleep, and workload correlate with depression.  
A logistic regression model was trained to classify whether a student is likely to experience depressive symptoms.

---

## Files in This Repository

| File | Description |
|------|--------------|
| `train_model.ipynb` | Data cleaning, feature engineering, model training, and evaluation. |
| `predict_user.ipynb` | Loads the saved model and predicts depression risk from user input. |
| `depression_model.joblib` | The trained logistic regression model. |
| `depression_model_columns.json` | The list of expected input columns for predictions. |
| `Student Depression Dataset.csv` | Dataset used to train the model. |

---

## How It Works

1. **Training Phase (`train_model.ipynb`):**
   - Cleans and encodes the dataset.  
   - Computes correlations between variables and depression.  
   - Trains a logistic regression model.  
   - Evaluates performance using accuracy, confusion matrix, and ROC curve.  
   - Saves the trained model (`.joblib`) and its column structure (`.json`).

2. **Prediction Phase (`predict_user.ipynb`):**
   - Loads the saved model.  
   - Takes user input (stress, sleep, etc.).  
   - Predicts whether the user is at risk of depression (0 = no, 1 = yes).  

---

## Example of User Interaction

