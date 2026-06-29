# Sentiment Analysis Project (NLP)

## Overview
This project performs sentiment analysis on product reviews using Natural Language Processing (NLP).  
It classifies reviews into **Positive, Negative, and Neutral** sentiments.

The model is built using **TF-IDF Vectorization + Logistic Regression**.

---

## Dataset
- Amazon Fine Food Reviews / Reviews dataset
- Main columns used:
  - Review Text
  - Score
  - Sentiment (created from Score)

---

## Workflow

1. Load dataset
2. Data preprocessing (cleaning text)
3. Convert ratings into sentiment labels
4. Text vectorization using TF-IDF
5. Train-test split
6. Train Logistic Regression model
7. Evaluate model performance
8. Build real-time prediction system

---

## Model Used

- TF-IDF Vectorizer  
- Logistic Regression  

Parameters:
- max_features = 10000  
- ngram_range = (1,2)  
- class_weight = "balanced"  

---

## Accuracy

- Model Accuracy: ~83%

Evaluation includes:
- Confusion Matrix
- Classification Report

---

## Example Predictions

Input:
- "This product is very good" → Positive  
- "I received yesterday" → Negative (dataset bias issue)  
- "Not used yet" → Neutral  

---

## How to Run

### Install dependencies