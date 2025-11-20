# Stock Market Sentiment Prediction using FinBERT (82% Accuracy)

This project implements a Natural Language Processing (NLP) solution for classifying market sentiment based on financial news headlines. The core objective is to instantly categorize short text snippets into one of two categories: **Positive** or **Negative**, providing a crucial signal for automated trading or investment analysis.

## Methodology

The solution leverages the **FinBERT** model, a powerful transformer architecture pretrained specifically on massive corpora of financial text. This specialization is key, allowing the model to accurately capture the nuances and context of financial language, which is often missed by general-purpose NLP models.

The primary steps included:
1. Data preprocessing and cleaning of the financial headlines dataset.
2. Loading and configuring the specialized FinBERT tokenizer and model.
3. Training/Fine-tuning the model to classify sentiment based on the dataset’s **2** classes.
4. Detailed evaluation using standard metrics.

## Key Results

The model achieved a robust overall **Accuracy of 82%** on the test dataset.

### Classification Report

| Metric | Positive Class | Negative Class | Weighted Average |
| :---: | :---: | :---: | :---: |
| **Precision** | 0.85 | 0.76 | 0.82 |
| **Recall** | 0.87 | 0.72 | 0.82 |
| **F1-Score** | 0.86 | 0.74 | 0.82 |

### Confusion Matrix Insights

Out of 1159 test instances, the model confirmed a strong classification capability:
* **643 True Positives:** Correctly identified bullish sentiment.
* **305 True Negatives:** Correctly identified bearish sentiment.

The higher F1-score for the Positive class (0.86) indicates a strong reliability in predicting positive market movements based on news.

## Setup and Replication

To run this project, clone the repository and execute the `stock_market_sentiment_prediction.ipynb` notebook. The project is designed to run efficiently on environments like Google Colab with GPU acceleration enabled.
