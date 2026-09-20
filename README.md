# RoBERTa Sentiment Analysis

A Natural Language Processing (NLP) project that uses the **RoBERTa Transformer model** for classifying text into **Positive, Negative, and Neutral** sentiment categories.

## Overview

This project implements a complete sentiment analysis pipeline using **RoBERTa (`roberta-base`)** and **PyTorch**.

The workflow includes:

- Data cleaning and preprocessing
- Sentiment distribution analysis
- Word cloud visualization
- Dataset balancing
- Tokenization using RoBERTa Tokenizer
- Fine-tuning RoBERTa for sentiment classification
- Model evaluation
- Sentiment prediction with confidence scores

## Features

- 3-class sentiment classification
- Positive, Negative, and Neutral sentiment detection
- Balanced dataset with equal samples from each class
- Text preprocessing using NLTK
- RoBERTa-based Transformer model
- PyTorch training pipeline
- Model evaluation using Accuracy and Classification Report
- Confidence score for predictions
- Sentiment visualization using charts and word clouds

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- RoBERTa
- NLTK
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- WordCloud
- Jupyter Notebook

## Sentiment Classes

The model classifies text into three categories:

| Label | Sentiment |
|------|-----------|
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
Sentiment Distribution Analysis
     ↓
Dataset Balancing
     ↓
RoBERTa Tokenization
     ↓
RoBERTa Model Initialization
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Sentiment Prediction
     ↓
Confidence Score

NLP Preprocessing

The text data is processed using the following steps:

Convert text to lowercase
Remove URLs
Remove special characters and numbers
Remove unnecessary whitespace
Tokenization
Stopword removal
Lemmatization
Convert processed text into model-ready input
Dataset Balancing

The dataset was balanced so that each sentiment class contains an equal number of samples.

Negative    → 1666 samples
Neutral     → 1666 samples
Positive    → 1666 samples

Total       → 4998 samples
Model

The project uses:

RoBERTa Base (roberta-base)

RoBERTa is a Transformer-based language model developed for improved natural language understanding.

The model is fine-tuned for a 3-class sentiment classification task.

Training Configuration
Parameter	Value
Model	roberta-base
Number of Classes	3
Epochs	3
Batch Size	16
Learning Rate	2e-5
Maximum Sequence Length	128
Optimizer	AdamW
Framework	PyTorch
Model Evaluation

The trained model is evaluated using:

Accuracy
Classification Report
Precision
Recall
F1-Score

The notebook also includes prediction functionality that returns the predicted sentiment along with its confidence score.

Prediction

The model can be used to predict the sentiment of new text.

Example:

Input:
"I really enjoyed this product."

Output:
Positive

Confidence:
High
Screenshots
Sentiment Distribution

Positive Word Cloud

Negative Word Cloud

Neutral Word Cloud

Project Structure
RoBERTa-Sentiment-Analysis/
│
├── screenshots/
│   ├── sentiment-distribution.png
│   ├── positive-wordcloud.png
│   ├── negative-wordcloud.png
│   └── neutral-wordcloud.png
│
├── data.csv
├── sentiment_analysis_using_roberta.ipynb
└── README.md
Installation

Clone the repository:

git clone https://github.com/Rohan30020407/RoBERTa-Sentiment-Analysis.git

Navigate to the project folder:

cd RoBERTa-Sentiment-Analysis

Install the required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn nltk wordcloud torch transformers
Running the Project

Open the Jupyter Notebook:

jupyter notebook

Then open:

sentiment_analysis_using_roberta.ipynb

Run the notebook cells sequentially to perform data preprocessing, visualization, model training, evaluation, and sentiment prediction.

Future Improvements
Train for more epochs
Experiment with other Transformer models
Improve model performance through hyperparameter tuning
Deploy the model as a web application
Create a REST API for sentiment prediction
Add real-time sentiment analysis
Author

Rohan Soni

GitHub:
https://github.com/Rohan30020407
