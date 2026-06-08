# 🎬 IMDB Sentiment Analysis

NLP project for classifying movie reviews as positive or negative using Machine Learning.

## 📊 Performance

✅ **Accuracy: 90%**

![Classification Report](images/accuracy_score.png)




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
