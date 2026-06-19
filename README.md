# IMDb Movie Reviews Sentiment Analysis

## Overview

This project implements a complete sentiment analysis pipeline for IMDb movie reviews, classifying reviews as either **positive** or **negative**. The project explores and compares both traditional Machine Learning and Deep Learning approaches to determine the most effective solution for sentiment classification.

Two models were developed and evaluated:

* Logistic Regression with TF-IDF features
* Bidirectional LSTM with word embeddings

The results demonstrate that traditional machine learning can outperform deep learning when data size, preprocessing, and model complexity are carefully considered.

---

## Objectives

* Build an end-to-end sentiment analysis system.
* Compare Machine Learning and Deep Learning approaches.
* Analyze model performance using multiple evaluation metrics.
* Create a reusable pipeline for predicting sentiment on unseen reviews.

---

## Dataset

The project uses the IMDb Movie Reviews dataset containing labeled movie reviews:

* Positive Reviews
* Negative Reviews

The dataset was preprocessed and transformed into machine-readable features before training.

---

## Data Preprocessing

The following preprocessing steps were applied:

* Text lowercasing
* HTML tag removal
* Punctuation removal
* Stopword removal
* Lemmatization using NLTK
* Text cleaning and normalization

---

## Exploratory Data Analysis

EDA was performed to better understand the dataset through:

* Sentiment distribution visualization
* Review length analysis
* Word frequency analysis
* Positive and negative word clouds

---

## Models Implemented

### 1. Logistic Regression + TF-IDF

Feature Extraction:

* TF-IDF Vectorization

Classifier:

* Logistic Regression

Results:

* Test Accuracy: 89.2%
* ROC-AUC Score: 0.961

Advantages:

* Fast training and inference
* High interpretability
* Excellent classification performance

---

### 2. Bidirectional LSTM

Architecture:

* Embedding Layer
* Bidirectional LSTM Layer
* Dense Output Layer

Results:

* Test Accuracy: 50.9%
* ROC-AUC Score: 0.515

Advantages:

* Captures sequential information
* Learns contextual word relationships

---

## Performance Comparison

| Model               | Test Accuracy | ROC-AUC Score |
| ------------------- | ------------- | ------------- |
| Logistic Regression | 89.2%         | 0.961         |
| Bidirectional LSTM  | 50.9%         | 0.515         |

### Best Model

Logistic Regression achieved the highest performance, outperforming the Bidirectional LSTM in both accuracy and ROC-AUC score while providing faster inference and better interpretability.

---

## Technologies Used

* Python 3.9+
* Scikit-learn
* TensorFlow / Keras
* NLTK
* Pandas
* NumPy
* Matplotlib
* Seaborn
* WordCloud
* Joblib

---

## Project Structure

```text
IMDb-Sentiment-Analysis/
│
├── data/
├── notebooks/
├── models/
├── images/
├── sentiment_analysis.ipynb
├── requirements.txt
├── README.md
└── saved_model.pkl
```

---

## Results and Insights

* Traditional Machine Learning proved highly effective for this binary text classification task.
* TF-IDF combined with Logistic Regression achieved strong predictive performance.
* Feature importance analysis provided interpretable insights into influential words affecting sentiment predictions.
* Deep Learning models require additional tuning and larger datasets to outperform simpler ML approaches.

---

## Future Improvements

* Hyperparameter optimization
* Transformer-based models (BERT, RoBERTa)
* Deployment using Streamlit or Flask
* Real-time sentiment prediction API
* Model monitoring and performance tracking

---

## Author

Shahd Yehia

Computer Science (AI) Student | Aspiring Data Scientist & Machine Learning Engineer

GitHub: https://github.com/shahdyehia105
LinkedIn: [www.linkedin.com/in/shahd-yehia](http://www.linkedin.com/in/shahd-yehia)
