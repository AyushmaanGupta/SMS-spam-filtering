﻿# SMS Spam Filtering with Machine Learning

This project focuses on building an intelligent SMS spam classifier using machine learning techniques. It uses text preprocessing, TF-IDF vectorization, and classification models to accurately detect spam messages.

## 🚀 Features
- Clean and labeled SMS dataset (5,572 messages)
- Preprocessing: Lowercasing, stopword removal, stemming, punctuation removal
- Vectorization using TF-IDF
- Multiple classifiers tested: Naive Bayes, SVM, Random Forest, etc.
- Streamlit web app for live spam classification
- Pickle-based model deployment

  
## 🧠 Algorithms Used
- **Multinomial Naive Bayes**: High precision, fast, effective on small datasets
- **Support Vector Classifier (SVC)**: High accuracy, works well with sparse text data
- **Random Forest & Ensemble Models**: Tested for comparison
- **Voting & Stacking Classifiers**: Combined models to improve results

## 📊 Model Performance (on test set)
| Model           | Accuracy | Precision |
|----------------|----------|-----------|
| Naive Bayes     | 97.2%    | 100%      |
| SVC             | 97.9%    | 93.3%     |
| Random Forest   | 98.0%    | 99.1%     |
| Stacking Classifier | 97.8% | 93.3%     |

> Note: Naive Bayes showed highest precision, while SVC and ensemble methods gave balanced accuracy.

## 📦 Dataset
- **Source:** [UCI SMS Spam Collection](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)
- **Size:** 5,572 labeled SMS messages
- **Classes:** `ham` (not spam), `spam`

## 🧪 How to Run

### ⚙️ Install dependencies
```bash
pip install streamlit
pip install scikit-learn
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install nltk
pip install -r requirements.txt
pip install joblib
pip install pickle-mixin
streamlit run app.py

