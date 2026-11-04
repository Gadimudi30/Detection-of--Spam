# SMS Spam Detection Using NLP and Machine Learning

## 📌 Project Overview

This project focuses on building a Machine Learning model to classify SMS messages as **Spam or Ham (Not Spam)** using Natural Language Processing (NLP) techniques.

The main objective is to identify unwanted spam messages automatically and distinguish them from genuine messages using text preprocessing, feature extraction, and machine learning classification.

## 🎯 Objectives

- Understand and explore the SMS Spam Collection dataset.
- Perform text preprocessing and cleaning.
- Convert text messages into numerical features.
- Train a machine learning classification model.
- Evaluate model performance using accuracy.
- Predict whether new SMS messages are Spam or Ham.

## 📂 Dataset

**Dataset Name:** SMS Spam Collection Dataset

- Total Records: 5,572
- Ham Messages: 4,825
- Spam Messages: 747
- Input Feature: SMS Message
- Target Variable: Label (Spam/Ham)

The dataset contains two important columns:

| Column | Description |
|---|---|
| label | Indicates whether the message is Spam or Ham |
| message | Contains the actual SMS text |

**Dataset Source:** [Kaggle – SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Scikit-learn
- Regular Expressions (re)
- Natural Language Processing (NLP)
- Machine Learning

## ⚙️ Project Workflow

### 1. Dataset Loading and Exploration
- Loaded the dataset using Pandas.
- Examined dataset shape, columns, and data types.
- Checked missing values.
- Analyzed Spam and Ham message distribution.

### 2. Data Preparation
- Selected the required columns.
- Renamed columns as `label` and `message`.
- Separated input messages and target labels.

### 3. Label Encoding
Used LabelEncoder to convert categorical labels into numerical values.

- Ham = 0
- Spam = 1

### 4. Train-Test Split
Divided the dataset into training and testing sets.

- Training Data: 80%
- Testing Data: 20%
- Random State: 42
- Stratification: Applied

### 5. Text Preprocessing
Cleaned the SMS messages using Regular Expressions.

- Converted text into lowercase.
- Removed unnecessary special characters.
- Removed numbers and unwanted symbols.
- Retained alphabets and spaces.

### 6. Feature Extraction – Bag of Words

Used `CountVectorizer` to convert text messages into numerical features.

- Learned vocabulary from training messages.
- Converted training and testing messages into numerical representations.
- Extracted 7,535 vocabulary features.

### 7. Model Building

Used the **Multinomial Naive Bayes** algorithm to train the classification model.

### 8. Model Evaluation

Evaluated the model using Accuracy Score.

## 📊 Model Performance

<escape>**Achieved Accuracy: 97.94%**</escape>

The model successfully learned to classify SMS messages into Spam and Ham categories.

## 🔍 Sample Prediction

Tested the trained model with a new SMS message:

**Input:**
"Congratulations! You won a free lottery prize"

**Predicted Output:**
Spam

The model can also classify genuine messages as Ham.

## 📁 Project Structure

```text
SMS-Spam-Detection/
│
├── SMS Spam Ham Project.ipynb
├── spam.csv
└── README.md
```

## 📌 Conclusion

This project helped me understand how Natural Language Processing and Machine Learning can be applied to real-world text classification problems.

By using text preprocessing, Bag of Words feature extraction, and the Multinomial Naive Bayes algorithm, I successfully developed an SMS Spam Detection model with 97.94% accuracy.

This project strengthened my practical knowledge of Python, NLP, and Machine Learning.
