## Copyright and Licensing
© [2026] [Srinath Kuruva]. All rights reserved.

This project is provided for demonstration purposes only and is not intended for commercial use, modification, or redistribution without explicit written consent from the author. All intellectual property rights remain with the author

## Prerequisites
* googlecolab
* Jupyter

# Stock-market-news-sentiment-analysis
Aufbau eines Systems zur Sentimentanalyse von Finanznachrichten und deren Verknüpfung mit Markttrends


## Overview
Financial markets are highly sensitive to information. This project develops a predictive system to analyze the sentiment of stock market news and correlate it with market movements. By utilizing Natural Language Processing (NLP) and Deep Learning, the system classifies news headlines into Positive, Neutral, or Negative sentiments, providing a quantitative basis for sentiment-driven trading strategies.

## Objective
To build an end-to-end data science pipeline that:

Transforms unstructured financial news into dense numerical representations using advanced embedding techniques.

Employs Deep Learning architectures to accurately classify sentiment polarity.

Analyzes the relationship between news sentiment, trade volume, and stock price volatility to identify predictive market indicators.

## Technical Stack
Deep Learning Framework: TensorFlow / Keras

NLP Libraries: Gensim (Word2Vec), Sentence-Transformers (all-MiniLM-L6-v2)

Machine Learning: Scikit-learn (Random Forest, SVM)

Data Visualization: Matplotlib, Seaborn

Environment: Python (Jupyter Notebook / Google Colab)

## System Architecture & Approach
1. Data Preprocessing & EDA
The project begins with extensive Exploratory Data Analysis (EDA) to understand the distribution of news across different sectors and its correlation with historical trade volumes. Text data is cleaned by removing noise, handling contractions, and normalizing case.

2. Feature Engineering (Embeddings)
Two distinct vectorization strategies are implemented:

Custom Word2Vec: Trained specifically on the financial corpus to capture domain-specific semantic relationships.

Sentence Transformers: Leverages pre-trained BERT-based models to capture high-level contextual meaning across entire headlines.

3. Predictive Modeling
The system evaluates multiple modeling approaches:

Random Forest Classifier: Used as a robust baseline for sentiment classification.

Sequential Neural Networks: Built with multiple dense layers and Dropout regularization to prevent overfitting, achieving superior precision in sentiment detection.

## Performance Metrics
The models are evaluated using a comprehensive suite of metrics to ensure reliability in a financial context:

Accuracy & F1-Score: To measure overall classification effectiveness.

Precision & Recall: To minimize false signals that could lead to poor trading decisions.

Hyperparameter Tuning: Utilized GridSearchCV to optimize model parameters, ensuring the best possible performance on the test set.

## Actionable Insights
Sentiment Correlation: The analysis revealed a strong correlation between "Negative" news spikes and increased trading volume, indicating market panic or sell-offs.

Neural Network Advantage: Deep learning models consistently outperformed traditional ML models in capturing nuanced financial jargon.

## Setup and Usage
Open Full_Code_Srinath_Kuruva.ipynb (or the specific sentiment analysis notebook) in Jupyter or Google Colab.

Install required dependencies:

Bash

pip install tensorflow gensim sentence-transformers scikit-learn seaborn
Load the financial news dataset (CSV format).

Run the cells to perform embedding generation, model training, and visual analysis.
