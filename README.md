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

### Performance Comparison (with Preprocessing)

The following table shows the performance of the models when trained with preprocessing:

| **Model**     | **Accuracy** | **Precision** | **Recall** | **F1 Score** |
|---------------|--------------|---------------|------------|--------------|
| **XGBoost**   | 0.9553       | 0.9609        | 0.9608     | 0.9608       |
| **DistilBERT**| 0.5050       | 0.5146        | 0.5083     | 0.5114       |
| **ALBERT**    | 0.5034       | 0.4929        | 0.5077     | 0.5001       |

### Performance Comparison (on Raw Text)

The following table shows the performance of DistilBERT and ALBERT when trained on raw text:

| **Model**      | **Accuracy** | **Precision** | **Recall** | **F1 Score** |
|----------------|--------------|---------------|------------|--------------|
| **DistilBERT** | 0.9967       | 0.9871        | 0.9991     | 0.9931       |
| **ALBERT**     | 0.9983       | 0.9991        | 0.9975     | 0.9983       |

### Key Insights

- **XGBoost with Preprocessing** achieved the highest accuracy of 95%, making it the most effective model for distinguishing between AI-generated and human-generated text when preprocessing is applied.
- **DistilBERT and ALBERT** achieved nearly 99% accuracy when trained on raw text. This high accuracy indicates that the models might have memorized the small dataset used for training, as they performed exceptionally well without preprocessing. The high performance may be a result of overfitting, where the model "remembers" the training data instead of generalizing from it.

## Conclusion

- XGBoost performed the best with preprocessing, whereas DistilBERT and ALBERT performed exceptionally well when trained on raw text.
- The results suggest that larger datasets and additional regularization might help improve generalization and prevent overfitting, especially for transformer-based models like DistilBERT and ALBERT.


