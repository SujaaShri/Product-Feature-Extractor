# Product Feature Extraction from E-Commerce Reviews

This project uses the **FLAN-T5** foundation model to extract key product features (like `battery life`, `design`, `smell`, etc.) from customer reviews. Sentiment analysis is performed to separate positive and negative opinions for each product.

## What It Does

- Splits each review into sentences.
- Applies sentiment analysis to label sentences as positive or negative.
- Uses prompt-based extraction via **FLAN-T5** to identify product features.
- Summarizes the most and least appreciated features for each product.

## Models Used

- Hugging Face Sentiment Analysis Pipeline
- `google/flan-t5-base` for feature extraction

## How to Use

1. Upload a CSV file with columns: `productId`, `Title`, and `Text`.
2. Run the notebook.
3. View extracted product features grouped by sentiment and product.
