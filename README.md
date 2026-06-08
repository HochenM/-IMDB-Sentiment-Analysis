# 🎬 IMDB Sentiment Analysis

> **90% Accuracy** | NLP | Machine Learning | Text Classification

## 📌 Overview

This project analyzes IMDB movie reviews using Natural Language Processing (NLP) to classify them as **positive** or **negative**. Built from scratch with Python and Scikit-learn.

### ✨ Key Achievement
**90% accuracy** on 50,000 movie reviews using TF-IDF with n-grams and LinearSVC.

## 🧠 What Makes This Special

- **N-grams (1,2)** capture word pairs like "not good" to preserve **semantic meaning** and word order
- **LinearSVC** finds optimal hyperplane in high-dimensional space
- **GridSearchCV** automatically finds best parameters
- **Stratified K-Fold** ensures balanced evaluation

## 📊 Results
accuracy 0.90 

## Requirements 

 Download Dataset
Download IMDB Dataset from Kaggle

## 📦 Required Imports

```python
import pandas as pd
import numpy as np
import re

# NLP
from nltk.tokenize import word_tokenize
from nltk.corpus import stopwords

# Machine Learning
from sklearn.model_selection import train_test_split, GridSearchCV, StratifiedKFold
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.svm import LinearSVC
from sklearn.pipeline import Pipeline
from sklearn.metrics import classification_report

# Model Saving
import joblib
```
