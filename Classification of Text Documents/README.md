## 🩺 Medical Text Dataset - Cancer Document Classification
📌 Project Overview

This project focuses on classifying medical research texts into different cancer categories (e.g., Thyroid Cancer, Lung Cancer, Colon Cancer).
Using NLP techniques like TF-IDF and ML models such as Logistic Regression, the system can automatically identify the type of cancer-related document.

## 📊 Dataset

Total Samples: 7,570

Labels:

Colon Cancer

Lung Cancer

Thyroid Cancer

## Example Data
label	text
Thyroid_Cancer	Thyroid surgery in children in a single institute...
Lung_Cancer	Natural killer NK cells are innate lymphocytes...
Colon_Cancer	The study demonstrates high burden of depression among patients...
## ⚙️ Project Workflow

Data Preprocessing

Removed irrelevant columns

Renamed columns (label, text)

Train-Test split

Feature Engineering

TF-IDF vectorization

Model Training

Logistic Regression (baseline)

Compared with: Naive Bayes, SVM, Random Forest

Evaluation

Accuracy

Precision, Recall, F1-score

Confusion Matrix

## 🚀 Results

Best Model: Logistic Regression

Accuracy: ~94%

Classification Report:

| Class          | Precision | Recall   | F1-score |
| -------------- | --------- | -------- | -------- |
| Colon Cancer   | 0.91      | 0.91     | 0.91     |
| Lung Cancer    | 1.00      | 1.00     | 1.00     |
| Thyroid Cancer | 0.92      | 0.92     | 0.92     |
| **Overall**    | **0.94**  | **0.94** | **0.94** |


## 🛠️ Tech Stack

Language: Python 🐍

Libraries:

scikit-learn

pandas, numpy

matplotlib, seaborn

Optional: HuggingFace Transformers (for BERT fine-tuning)

## 🔮 Future Improvements

Fine-tune BERT/Transformer models for better performance

Build a web app (Streamlit/Flask) for real-time cancer doc classification

Extend dataset with more cancer types

✨ Author: Suraj Kumar
