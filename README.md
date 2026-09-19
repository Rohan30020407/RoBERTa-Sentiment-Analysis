# RoBERTa Sentiment Analysis

A Natural Language Processing project that uses the RoBERTa transformer model for three-class sentiment classification: **Positive, Neutral, and Negative**.

## Project Overview

This project implements sentiment analysis using **RoBERTa**, a transformer-based language model.

The project covers the complete NLP workflow, including:

- Data cleaning
- Text preprocessing
- Sentiment visualization
- Dataset balancing
- RoBERTa tokenization
- Model fine-tuning
- Model evaluation
- Sentiment prediction
- Prediction confidence

## Features

- Remove duplicate and missing records
- Convert text to lowercase
- Remove special characters and numbers
- Remove URLs
- Remove extra whitespace
- Tokenization
- Stopword removal
- Lemmatization
- Sentiment distribution visualization
- Word clouds for different sentiment classes
- TF-IDF vectorization
- Balanced dataset creation
- RoBERTa tokenizer
- RoBERTa sequence classification
- Model training using PyTorch
- Accuracy evaluation
- Classification report
- Sentiment prediction with confidence score

## Tech Stack

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn
- WordCloud
- PyTorch
- Hugging Face Transformers
- RoBERTa

## Sentiment Classes

| Label | Sentiment |
|---|---|
| 0 | Negative |
| 1 | Neutral |
| 2 | Positive |

## Project Workflow

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
Text Preprocessing
     ↓
Sentiment Visualization
     ↓
Dataset Balancing
     ↓
Train/Test Split
     ↓
RoBERTa Tokenization
     ↓
RoBERTa Fine-Tuning
     ↓
Model Evaluation
     ↓
Sentiment Prediction
     ↓
Confidence Score

NLP Preprocessing

The project performs the following preprocessing steps:

Convert text to lowercase
Remove special characters and numbers
Remove URLs
Remove extra whitespace
Tokenize text
Remove stopwords
Lemmatize tokens
Join processed tokens
Encode sentiment labels
Model

The project uses the pretrained:

roberta-base

The RoBERTa model is fine-tuned for three-class sentiment classification using PyTorch and Hugging Face Transformers.

Training Configuration
Number of sentiment classes: 3
Maximum sequence length: 128
Batch size: 16
Learning rate: 2e-5
Number of epochs: 3
Optimizer: AdamW
Dataset Balancing

The project creates a balanced dataset containing samples from all three sentiment classes:

Negative
Neutral
Positive

The balanced dataset is then divided into training and testing sets using a stratified split.

Model Evaluation

The model evaluates sentiment predictions using:

Accuracy
Classification Report

The classification report provides performance information for the Negative, Neutral, and Positive classes.

Prediction

The trained model can take new text as input and return:

Predicted sentiment
Prediction confidence

Example:

Input:
"The product quality is excellent"

Output:
Sentiment: positive
Confidence: 0.xx
Project Structure
RoBERTa-Sentiment-Analysis/
│
├── sentiment_analysis_using_roberta.ipynb
├── data.csv
├── requirements.txt
├── .gitignore
└── README.md
Installation

Clone the repository:

git clone https://github.com/Rohan30020407/RoBERTa-Sentiment-Analysis.git

Navigate to the project directory:

cd RoBERTa-Sentiment-Analysis

Install the required dependencies:

pip install -r requirements.txt
Running the Project

Open the Jupyter Notebook:

sentiment_analysis_using_roberta.ipynb

Run the notebook cells sequentially to perform:

Data loading
Data cleaning
NLP preprocessing
Visualization
Dataset balancing
RoBERTa training
Model evaluation
Sentiment prediction
Future Improvements
Build an interactive Streamlit application
Deploy the sentiment analysis model
Add more evaluation metrics
Improve inference performance
Support real-time sentiment analysis
Train with larger datasets
Author

Rohan Soni

GitHub: https://github.com/Rohan30020407