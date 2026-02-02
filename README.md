📈 Global Market Interconnectedness & NIFTY50 Opening Direction Prediction

Author: Werner Visser
Period Analysed: 2019–2024

🔍 Project Overview

This project analyses the interconnectedness of major global equity markets and evaluates whether global index movements and volatility (VIX) can predict the daily opening direction of the NIFTY 50. The study demonstrates how global market shocks propagate across regions and influence short-term directional behaviour.

🎯 Research Objective

The core objective is to determine whether movements in global indices and volatility act as significant indicators for predicting NIFTY50 opening direction. Global co-movements are used as explanatory variables to capture short-term sentiment spillover and market risk dynamics.

📊 Data Sources
Market Data

Yahoo Finance (via yfinance)

Indices included:

NIFTY 50 (India)

Dow Jones (USA)

Nasdaq (USA)

Hang Seng (Hong Kong)

Nikkei 225 (Japan)

DAX (Germany)

VIX (Volatility Index)

Sentiment Data

Synthetic Financial Tweet Corpus

Generated programmatically using NIFTY50 return behaviour

Enables sentiment modelling without paid API access

🧹 Data Engineering Pipeline

The master dataset was constructed using:

Daily return calculation

Multi-index outer join merging

Linear interpolation for missing values

Feature engineering (Year, Quarter, Month)

Target variable creation (Nifty_Open_Dir)

Holiday and weekend adjustments

🧠 Modelling Approach
Models Implemented

Logistic Regression

Decision Trees

Random Forest Classifier

Evaluation Metrics

Accuracy

Confusion Matrix

ROC Curve

AUC Score

Random Forest produced the most stable and reliable predictive performance on unseen data.

📝 Sentiment Analysis Component

A synthetic tweet generator was developed to simulate market-aware financial sentiment:

Tone mapped to NIFTY return behaviour

Sentiment extracted using VADER

Classified into positive, neutral and negative sentiment

Linked sentiment patterns to market movement behaviour

📌 Key Findings

Global market movements contain meaningful predictive signals for NIFTY opening direction

Crisis-period volatility (COVID-19) shows strong international spillover effects

Random Forest outperformed classical statistical approaches

Combining multi-market indicators improves short-term prediction stability

⚙️ Tech Stack

Python

Pandas & NumPy

Scikit-Learn

yFinance API

NLTK / VADER

Matplotlib & Seaborn

Jupyter Notebook

🎓 Academic Context

This project demonstrates a full end-to-end data science workflow:

Data ingestion → cleaning → feature engineering → modelling → evaluation → NLP sentiment integration

👤 Author

Werner Visser
Data Scientist
