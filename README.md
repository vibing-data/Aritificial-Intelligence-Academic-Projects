# 🏡 Airbnb Price Prediction in Rome, Italy

This project focuses on predicting Airbnb listing prices in Rome using a combination of structured listing features and unstructured guest review data. Our goal was to develop interpretable, high-performing machine learning models while extracting actionable insights for hosts, guests, and the Airbnb platform.

📍 **Project Title**: *Airbnb Data Analysis & Price Prediction – Rome*  
🧑‍🤝‍🧑 **Team Members**: AJ Payzant, Iseet Panja, Rohit Sarna  
📄 **Report**: [Final Report PDF](./Group_5_Final_Report.pdf)

---

## 📊 Overview

We analyzed over **28,000 listings** and **1.9 million reviews** from the March 2025 snapshot of Inside Airbnb data. Using natural language processing (NLP) and supervised learning models, we built two predictive pipelines:

- **Baseline Model**: Using structured listing data
- **Sentiment Model**: Integrating review sentiment scores using multilingual BERT

---

## 🔍 Key Techniques

### 🔧 Data Preparation
- Missing value imputation (median for skewed data)
- Outlier handling using IQR method
- Label encoding for categorical fields
- Feature engineering (occupancy rate, revenue per review, review quality, etc.)

### 💬 Sentiment Analysis
- Preprocessing with NLTK (lemmatization, stopword filtering)
- Sentiment classification using **XLM-Roberta** (via Hugging Face)
- Merged sentiment scores with structured features

### 🤖 Models Evaluated
- Linear, Ridge, Lasso Regression
- Random Forest, Extra Trees, Gradient Boosting, XGBoost
- Ensemble Models: **Voting Regressor**, **Stacking Regressor**

---

## 📈 Results

| Model Type     | Best R² | Best RMSE |
|----------------|---------|-----------|
| Baseline       | 0.695   | 28.80     |
| Sentiment-Enhanced | **0.869**   | **18.03**     |

> ✅ Sentiment features reduced RMSE by 37% and improved R² by nearly 25% over the baseline.

---

## 🧠 Key Insights

### 📌 For Hosts
- Sentiment strongly impacts pricing — invest in hospitality, cleanliness, and communication.
- Focus on revenue per review and high occupancy strategies.

### 📌 For Airbnb
- Integrate sentiment into smart pricing and search ranking algorithms.
- Offer improvement recommendations to hosts based on reviews.

### 📌 For Guests
- Listings with consistently positive sentiment generally offer better value.
- Don’t overlook higher-priced listings with strong sentiment signals.

---

## 📁 Project Structure
