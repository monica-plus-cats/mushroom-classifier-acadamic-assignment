# Mushroom Classification with PCA and Supervised Learning

This project classifies mushrooms as **edible** or **poisonous** using supervised learning models. It applies dimensionality reduction via PCA and compares model performance on full and reduced datasets.

## Dataset

- **Source:** UCI Machine Learning Repository – [Mushroom Dataset](https://archive.ics.uci.edu/ml/datasets/Mushroom)
- The dataset includes categorical features describing physical characteristics of mushrooms and a binary target indicating edibility.

## Objectives

- Preprocess and encode categorical data
- Train K-Nearest Neighbors (KNN) and Decision Tree models on full dataset
- Apply Principal Component Analysis (PCA) to reduce dimensionality while preserving 95% variance
- Retrain models (Random Forest and Logistic Regression) on PCA-reduced data
- Compare training time and model performance (accuracy, precision, recall)

## Methods

- Label encoding and OneHotEncoding
- Dimensionality reduction using PCA
- Supervised classification with:
  - KNN
  - Decision Tree
  - Random Forest
  - Logistic Regression
- Evaluation metrics: accuracy, precision, recall
- Timing of model training to compare efficiency pre- and post-PCA

## Key Findings

- Random Forest achieved perfect accuracy but likely overfit, especially on reduced data
- PCA helped improve training speed and generalization for Logistic Regression
- Dimensionality was reduced by over 35%, retaining 41 features from the original 116

## Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
