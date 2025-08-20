# Customer Review Sentiment Analysis - NLP ML Model
This repository contains a Natural Language Processing (NLP) machine learning model designed to analyze customer reviews of a product and predict their sentiment (positive, negative, or neutral).

## Project Overview process
- Clean and preprocess customer review text
- Build an NLP model to classify sentiment
- Evaluate and deploy the model
  
## Technologies Used:
- Python
- Scikit-learn / TensorFlow / PyTorch
- NLTK / spaCy
- Pandas
-LogisticRegression model used for the target variable 'Sentiment', with model classification report

## Classification Report:
| Class / Metric | Precision | Recall | F1-Score | Support |
|----------------|-----------|--------|----------|---------|
| 0              | 0.61      | 0.75   | 0.67     | 110     |
| 1              | 0.96      | 0.93   | 0.94     | 720     |
| **Accuracy**   | -         | -      | 0.90     | 830     |
| **Macro Avg**  | 0.79      | 0.84   | 0.81     | 830     |
| **Weighted Avg** | 0.91    | 0.90   | 0.91     | 830     |
              
## Prediction Table

| Index | Actual | Predicted |
|-------|--------|-----------|
| 0     | 1      | 0         |
| 1     | 1      | 0         |
| 2     | 1      | 1         |
| 3     | 0      | 1         |
| 4     | 0      | 0         |
