# NLP-Ulta-Skincare-Reviews
# Customer Review Sentiment Analysis - NLP ML Model

This repository contains a Natural Language Processing (NLP) machine learning model designed to analyze customer reviews of a product and predict their sentiment (positive, negative, or neutral).

# Project Overview
This project aims to:
- Clean and preprocess customer review text
- Build an NLP model to classify sentiment
- Evaluate and deploy the model
  
Technologies Used:
Python
Scikit-learn / TensorFlow / PyTorch
NLTK / spaCy
Pandas

model used -  LogisticRegression for the target variable 'Sentiment', with model classification report:
Accuracy: 0.9036144578313253
Classification Report:
               precision    recall  f1-score   support

           0       0.61      0.75      0.67       110
           1       0.96      0.93      0.94       720

    accuracy                           0.90       830
   macro avg       0.79      0.84      0.81       830
weighted avg       0.91      0.90      0.91       830

some of prediction done by the model :

Prediction Table:
   Actual  Predicted
0       1          0
1       1          0
2       1          1
3       0          1
4       0          0
