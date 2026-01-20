🚀 API Latency Spike Prediction System
📌 Project Overview

This project focuses on predicting API latency spikes that may violate Service Level Agreements (SLAs).
Using historical cloud performance metrics, the system proactively identifies high-risk latency events to enable early mitigation and improve system reliability.
The solution combines feature engineering on time-series data with a machine learning classification model, and provides real-time latency risk assessment through a web interface.

🎯 Problem Statement
Modern cloud applications often experience sudden latency spikes due to traffic surges, infrastructure issues, or resource contention. These spikes are rare but critical, as they can severely impact user experience and SLA compliance.

Objective:
Build a machine learning system that can predict latency spikes in advance using historical performance data.

🧠 Solution Approach
1. Data Processing
Cleaned and analyzed 200K+ cloud performance records
Handled missing values and noisy signals
Converted raw metrics into structured numerical features

2. Feature Engineering
Lag features (previous latency values)
Rolling statistics (mean, variance, trends)
Temporal patterns capturing short-term fluctuations

3. Model Development
Framed the problem as a binary classification task
Trained an XGBoost classifier optimized for imbalanced data
Tuned decision thresholds to improve rare spike detection

4. Deployment
Deployed the trained model using Streamlit
Enabled real-time inference with sub-second latency
Visualized spike risk probabilities for user interpretation

🛠️ Tech Stack
Language: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
Model: XGBoost Classifier
Visualization & UI: Streamlit

📊 Model Performance
ROC-AUC: 0.72
Overall Accuracy: ~80%
Spike Detection Recall: ~50% for rare latency spike events
Optimized for early warning rather than pure accuracy

🖥️ Application Features
Real-time latency spike risk prediction
Interactive and lightweight Streamlit interface
Visual feedback for operational decision-making

Dataset - https://www.kaggle.com/datasets/abdurraziq01/cloud-computing-performance-metrics
