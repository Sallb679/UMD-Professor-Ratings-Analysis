# PlanetTerp Professor Reviews Analysis

This project implements a mini data pipeline and machine learning workflow analyzing professor ratings from PlanetTerp review and grade data.

## Project Structure

The workflow is divided into three main files, each representing a stage in the pipeline:

1. **Data Extraction**  
   - Extract raw review data from the PlanetTerp API.  
   - Collect and consolidate initial review datasets for further processing.

2. **Data Cleaning & Feature Engineering**  
   - Clean and preprocess review text and grade data.  
   - Handle duplicates, missing values, and map categorical grades to numeric scores.  
   - Generate aggregated professor-level features such as average grades, review counts, and text statistics.

3. **Final Features, Modeling & Prediction**  
   - Apply sentiment analysis on reviews to extract sentiment scores using VADER.  
   - Combine all features into a final dataset.  
   - Train and evaluate machine learning models (KNN, Random Forest, XGBoost) to predict professor ratings.

## Highlights

- Sentiment analysis adds a qualitative dimension to numeric features.  
- Models achieve strong predictive performance, with XGBoost performing best.  
- The pipeline showcases end-to-end data science workflow from raw data to actionable insights.

## Technologies Used

- Python 3 with pandas, numpy for data processing  
- scikit-learn and xgboost for modeling  
- nltk’s VADER for sentiment analysis  
- tqdm for progress monitoring

---

This project demonstrates how to build a robust data flow and apply machine learning techniques to professor review data, providing valuable insights into professor performance.
