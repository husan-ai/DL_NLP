# Yelp Sentiment RNN

This project uses **PyTorch** and an **LSTM-based RNN** model to classify Yelp reviews into **positive** or **negative** sentiment. The dataset is downloaded automatically, preprocessed, converted into numerical sequences, and then used to train a sentiment analysis model. :contentReference[oaicite:0]{index=0}

## Features

- Downloads and extracts the Yelp review dataset automatically
- Converts star ratings into binary sentiment labels
- Removes neutral (3-star) reviews
- Builds a vocabulary from the most frequent words
- Encodes and pads text sequences
- Trains an LSTM model for sentiment classification
- Predicts sentiment for new review texts :contentReference[oaicite:1]{index=1}

## Tech Stack

- Python
- Pandas
- PyTorch
- Regular Expressions

## How it Works

1. Load Yelp review data
2. Map ratings:
   - **4–5 stars** → positive
   - **1–2 stars** → negative
   - **3 stars** → removed
3. Tokenize and encode text
4. Pad sequences to a fixed length
5. Train an LSTM-based neural network
6. Predict sentiment for new reviews :contentReference[oaicite:2]{index=2}

## Run

```bash
python yelp_sentiment_rnn.py
