# Sentiment Analysis Using LSTM

## Overview

This project focuses on sentiment analysis using Long Short-Term Memory (LSTM) networks implemented with TensorFlow/Keras. The model aims to classify text data into binary sentiment categories, such as Positive or Negative.

## Dataset

The dataset used in this project is a CSV file containing text data with sentiment labels. The key column, `text`, holds the textual content, while the sentiment label column indicates the sentiment associated with each text entry.

**Preprocessing Steps:**
- Tokenization: Converts text into sequences of integers based on word frequency.
- Padding: Ensures that all text sequences have a uniform length for model compatibility.

## Modeling

The model architecture includes:
- **Embedding Layer**: Converts integer sequences into dense vectors of fixed size.
- **LSTM Layer**: Processes sequences with Long Short-Term Memory units to capture temporal dependencies in the text.
- **Dropout Layer**: Helps prevent overfitting by randomly setting a fraction of input units to zero during training.
- **Dense Layer**: Outputs a single value with a sigmoid activation function to predict the sentiment.

The model is trained using binary cross-entropy loss and the Adam optimizer. 

## Results

**Model Training:**
- The model is trained for a specified number of epochs, and its performance is evaluated on a validation set.

**Visualization:**
- **Accuracy and Loss Plots**: Visualizations are generated to track the training and validation accuracy and loss over epochs. These plots help assess how well the model is learning and generalizing.

