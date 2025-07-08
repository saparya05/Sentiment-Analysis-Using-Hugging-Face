# Sentiment-Analysis-Using-Hugging-Face
Sentiment Analysis Model Using Hugging Face Transformer
Sentiment and Emotion Analysis using Hugging Face Transformers
This project performs sentiment analysis on a dataset of tweets using the Hugging Face Transformers pipeline API, specifically the pre-trained sentiment-analysis model. It evaluates model performance using accuracy, confusion matrix, and ROC AUC score.

## Dataset
The dataset used is an Excel file named:

sentiment and emotion tweets dataset.xlsx
It contains the following columns:

Text: The tweet content.

sentiment: The labeled sentiment (positive, negative, or neutral).

emotion: The labeled emotion category (not used in this script but available for further work).

## Tasks Performed
Load and preprocess tweet data.

Run Hugging Face sentiment analysis on all tweets.

Map sentiment to binary target labels (positive = 1, negative = 0).

Calculate:

✅ Accuracy

✅ Confusion matrix

✅ ROC AUC score

Visualize:

✅ Sentiment class distribution

✅ Confusion matrix heatmap

## How It Works
1. Dependencies
Make sure you have the following Python libraries installed:

pip install numpy pandas seaborn matplotlib scikit-learn transformers torch openpyxl
2. Run the Script
The code:

Loads the Excel file

Filters out neutral sentiments

Runs a pre-trained Hugging Face sentiment analysis pipeline

Computes binary predictions and probability scores

Calculates and displays performance metrics

## Sample Output
Accuracy: ~83.54%

ROC AUC Score: (depends on model and data)

Confusion Matrix:


                Predicted
               0       1
Actual   0   [TN]   [FP]
         1   [FN]   [TP]
Plotted using a heatmap.


## Model Used
pipeline("sentiment-analysis") from 🤗 Hugging Face Transformers

This loads a default pre-trained BERT-based model fine-tuned on sentiment tasks.

