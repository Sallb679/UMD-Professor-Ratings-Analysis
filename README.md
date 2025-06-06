# PlanetTerp Professor Reviews Analysis

This project builds a data pipeline and machine learning models to analyze and predict professor ratings using PlanetTerp review and grade data.

## Overview

The analysis is structured into three main stages:

1. **Data Extraction & Cleaning**  
   - Extract raw review data via API and clean it (remove duplicates, fill missing values).  
   - Clean and preprocess text reviews, map expected grades to numeric scores, and generate review-level features such as word and character counts.

2. **Feature Aggregation & Sentiment Analysis**  
   - Aggregate review and grade data at the professor level, computing averages and totals for various metrics.  
   - Use VADER sentiment analysis to extract sentiment scores from cleaned review texts and merge these into the feature set.

3. **Machine Learning Modeling**  
   - Train and evaluate multiple regression models (KNN, Random Forest, XGBoost) using optimized hyperparameters.  
   - Models predict professor ratings based on aggregated features and sentiment scores, with evaluation via RMSE and R² metrics.

## Results

- The XGBoost model achieved the best performance, balancing error and explained variance.  
- Sentiment analysis improved feature richness by capturing qualitative review insights.  

## Technologies & Libraries

- Python 3  
- pandas, numpy  
- scikit-learn, xgboost  
- nltk (VADER sentiment)  
- tqdm for progress bars  

## How to Use

- Run the data extraction and cleaning notebook first to prepare the dataset.  
- Next, run the sentiment analysis notebook to score reviews and generate sentiment features.  
- Finally, run the modeling notebook to train and evaluate regression models.  

---

This project demonstrates a full end-to-end workflow from raw data extraction to predictive modeling, highlighting the importance of feature engineering and text analysis in educational data contexts.

