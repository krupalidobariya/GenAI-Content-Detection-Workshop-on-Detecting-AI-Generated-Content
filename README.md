# GenAI Content Detection: Workshop on Detecting AI-Generated Content

# Overview
In this repository, we provide a solution to detect AI-generated text using XGBoost, Albert and Distilbert, three powerful models in natural language processing and machine learning. 
This project helps researchers, developers, and anyone interested to understand and address the challenges of identifying AI-generated content from human-written text.
<br />
<br />

# Dataset:
The dataset used in this project is hosted on Hugging Face and is available at the link below:

<a href="https://huggingface.co/datasets/Hello-SimpleAI/HC3" target="_blank">HC3 Dataset</a>: A comprehensive dataset designed for tasks involving AI-generated text detection.

## Project Highlights

- **Dual Model Approach**: Compare and analyze the performance of BERT and XGBoost for AI text detection.
- **Data Preprocessing**: Tokenization, lemmatization, stopword removal, and vectorization techniques such as TF-IDF.
- **Model Evaluation**: Accuracy, precision, recall, F1 score, and confusion matrices for robust performance measurement.
- **Visual Insights**: ROC curves, t-SNE plots, and feature importance graphs to understand model behavior.

# Performance comparison between XGBoost and BERT.

| Metric      | XGBoost  | DistilBERT | ALBERT   |
|-------------|----------|------------|----------|
| Accuracy    | 0.95086  | 0.5046     | 0.5034   |
| Precision   | 0.95091  | 0.5646     | 0.4929   |
| Recall      | 0.95083  | 0.5083     | 0.5077   |
| F1 Score    | 0.95086  | 0.3415     | 0.3585   |




