# IMDB Sentiment Analysis

## What I Learned

### NLP Techniques
- Text preprocessing (lowercasing, removing punctuation, removing numbers)
- Tokenization with NLTK
- Stopword removal
- TF-IDF vectorization for feature extraction
- Handling repeated characters (e.g., "loveeee" → "love")

### Machine Learning
- Building pipelines with Scikit-learn
- Hyperparameter tuning using GridSearchCV
- Stratified K-Fold cross-validation
- LinearSVC for text classification
- Model evaluation with classification report

### Tools & Libraries
- Pandas for data manipulation
- NLTK for text processing
- Scikit-learn for ML algorithms
- Joblib for model serialization

## What I Built

A complete sentiment analysis pipeline that:
1. Takes raw IMDB movie reviews
2. Preprocesses and cleans the text
3. Converts text to TF-IDF features
4. Classifies as positive or negative using LinearSVC
5. Achieves 90% accuracy on 50,000 reviews

## My Code Structure

```python
# Preprocessing Function
def preprocess(text):
    - Lowercase text
    - Remove numbers and punctuation
    - Tokenize words
    - Remove stopwords
    - Handle repeated characters
    return cleaned_text

# Pipeline
pipeline = Pipeline([
    ('tfidf', TfidfVectorizer()),
    ('classifier', LinearSVC())
])

# Hyperparameter Tuning
param_grid = {
    'ngram_range': [(1,1), (1,2)],
    'min_df': [2, 3],
    'max_df': [0.85, 0.95],
    'C': [0.5, 1]
}

# Cross Validation
cv = StratifiedKFold(n_splits=5, shuffle=True)
