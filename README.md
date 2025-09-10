# Customer Review Sentiment Analysis – NLP ML Model  

This repository contains a **Natural Language Processing (NLP) machine learning model** designed to analyze customer skincare product reviews and predict their sentiment (**positive** or **negative**).  

---
##  Project Overview  
This project demonstrates the full NLP pipeline:  

1. **Data Cleaning & Preprocessing**  
   - Removed nulls, symbols, and extra whitespace  
   - Tokenization, lemmatization, stopword removal with **spaCy**  
   - TF-IDF vectorization for feature extraction  

2. **Feature Engineering**  
   - Converted relative dates (e.g., "2 months ago") into numeric days  
   - Extracted year, month, weekday from scrape date  
   - Encoded categorical columns (Product, Verified Buyer)  

3. **Sentiment Labeling**  
   - Applied **VADER Sentiment Analyzer** to assign binary sentiment labels  
   - Fixed spelling issues (e.g., “excelent” → “excellent”)  

4. **Modeling**  
   - Logistic Regression trained on TF-IDF features  
   - Balanced class weights to handle class imbalance  

5. **Evaluation**  
   - Accuracy, Precision, Recall, F1-score  
   - Confusion matrix and prediction table  

---

##  Technologies Used  
- **Python**  
- **Pandas** – data preprocessing  
- **spaCy** – lemmatization, text preprocessing  
- **Scikit-learn** – TF-IDF, Logistic Regression, evaluation metrics  
- **VADER Sentiment** – rule-based sentiment labeling  

---

##  Results  

### **Classification Report**
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0 (Negative) | 0.61 | 0.75 | 0.67 | 110 |
| 1 (Positive) | 0.96 | 0.93 | 0.94 | 720 |
| **Accuracy** | - | - | **0.90** | 830 |
| **Macro Avg** | 0.79 | 0.84 | 0.81 | 830 |
| **Weighted Avg** | 0.91 | 0.90 | 0.91 | 830 |

### **Sample Prediction Table**
| Index | Actual | Predicted |
|-------|--------|-----------|
| 0 | 1 | 0 |
| 1 | 1 | 0 |
| 2 | 1 | 1 |
| 3 | 0 | 1 |
| 4 | 0 | 0 |

---

## 🚀 How to Run  

1. Clone this repo:  
   ```bash
   git clone https://github.com/zaralrubaie/nlp-ulta-skincare-reviews.git
   cd nlp-ulta-skincare-reviews
