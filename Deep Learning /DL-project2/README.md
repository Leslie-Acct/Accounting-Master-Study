# Bitcoin Tweet Sentiment Analysis

*This project is the second assignment from the "Deep Learning in Text Analytics" course by Professor Stefan Lessmann, Humboldt-Universität zu Berlin.*

##  Project Goal
This project explores and compares multiple Natural Language Processing (NLP) techniques to classify the sentiment (positive/negative) of Bitcoin-related tweets. The goal is to benchmark a range of models, from simple dictionary-based methods to advanced fine-tuned transformers.

##  Models & Approaches
This repository implements six distinct sentiment classification approaches:

* **Dictionary-based:** Uses the `pysentiment2` library (HIV4 lexicon) to calculate a polarity score.
* **TF-IDF + XGBoost:** A classical machine learning baseline using TF-IDF features.
* **RNN with Random Embeddings:** A Bidirectional GRU model trained from scratch.
* **RNN with Pre-trained Embeddings:** A Bidirectional LSTM using pre-trained Word2Vec embeddings.
* **DistilBERT (Hugging Face Pipeline):** A pre-trained transformer used for zero-shot classification.
* **Fine-tuned DistilBERT:** The DistilBERT model fine-tuned on the tweet dataset using the Hugging Face `Trainer` API.
