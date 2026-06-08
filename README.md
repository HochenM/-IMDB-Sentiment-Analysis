# 🎬 IMDB Sentiment Analysis

NLP project for classifying movie reviews as positive or negative using Machine Learning.

## 📊 Performance

✅ **Accuracy: 90%**

![Classification Report](images/accuracy_score.png)

## 🔍 Feature Importance

![Positive Words](<img width="347" height="773" alt="positive " src="https://github.com/user-attachments/assets/b17e3218-030a-4b23-a1c5-f148f0dc694f" />
)


## 🛠️ Tech Stack

- Python
- Scikit-learn (TfidfVectorizer, LinearSVC, GridSearchCV)
- NLTK (Tokenization, Stopwords)
- Pandas, NumPy
- Joblib

## 📁 Files

- `sentiment_analysis.py` - Training script
- `predict.py` - Prediction script  
- `model/sentiment_model.joblib` - Trained model
- `requirements.txt` - Dependencies

## 🚀 Quick Start

```bash
pip install -r requirements.txt
python predict.py "Amazing movie!"
