# Fake News Detector using LSTMs

This project implements a fake news detector using Long Short-Term Memory (LSTM) networks with TensorFlow. The model is designed to classify news articles as either "real" or "fake" based on their content.

## Overview

The Fake News Detector leverages LSTM networks to analyze text data and detect fake news. The model is trained on a dataset of news articles and can predict the authenticity of new articles.

## Features

- **Text Classification**: Classifies news articles as "real" or "fake."
- **LSTM-Based Model**: Utilizes LSTM networks for handling sequential data and capturing contextual information.
- **TensorFlow Implementation**: Built using TensorFlow for efficient training and prediction.

## Installation

To get started with this project, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/sohamfcb/fake-news-detector.git
    cd fake-news-detector
    ```

2. **Create and Activate a Virtual Environment**:

    On MacOS and Linux:
    ```bash
    python3 -m venv env
    source env/bin/activate
    ```

    On Windows:
    ```bash
    python -m venv env
    .\env\Scripts\activate
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Prepare the Dataset**: Ensure you have a dataset of news articles. The dataset should be in a CSV file with columns for the text and labels.

2. **Train the Model**:
    Run the training script to train the LSTM model on your dataset:
    ```bash
    python train_model.py
    ```

3. **Evaluate the Model**:
    Evaluate the model's performance on a test set:
    ```bash
    python evaluate_model.py
    ```

4. **Make Predictions**:
    Use the trained model to make predictions on new articles:
    ```bash
    python predict.py --text "Your news article text here"
    ```

## File Structure

- `train_model.py`: Script for training the LSTM model.
- `evaluate_model.py`: Script for evaluating the model’s performance.
- `predict.py`: Script for making predictions on new articles.
- `requirements.txt`: Python packages required for the project.
- `model.h5`: (If applicable) Saved model file.

## Dependencies

- TensorFlow
- numpy
- pandas
- scikit-learn

You can install the dependencies by running:
```bash
pip install -r requirements.txt
