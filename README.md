
# Quora Question Pairs - Duplicate Question Detection

A Natural Language Processing (NLP) and Machine Learning project to determine whether two Quora questions are semantically similar or duplicate.

The goal of this project is to build a model that can identify if two questions are asking the same thing, even if they are written differently.

---

📌 Problem Statement

Quora receives thousands of questions every day, and many users ask questions that have already been answered. Detecting duplicate questions helps improve search quality and user experience.

This project focuses on predicting whether a pair of questions are:

- **1 → Duplicate Questions**
- **0 → Non-Duplicate Questions**

---

## 📂 Dataset

Dataset used:

Quora Question Pairs Dataset (Kaggle)

Dataset Link:
https://www.kaggle.com/c/quora-question-pairs

The dataset contains question pairs along with a label indicating whether they are duplicates or not.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- NLP Techniques
- Machine Learning Algorithms

---

## 🔍 Project Workflow

### 1. Data Loading & Exploration
- Load dataset using Pandas
- Understand dataset structure
- Analyze duplicate and non-duplicate question distribution

### 2. Data Preprocessing
- Handle missing values
- Analyze repeated questions
- Perform exploratory data analysis

### 3. Feature Engineering

Text data is converted into numerical features using:

- Bag of Words
- CountVectorizer

The questions are transformed into machine-readable numerical vectors.

### 4. Model Training

Machine Learning models are trained on extracted features.

Models used:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### 5. Model Evaluation

Models are evaluated using:

- Accuracy Score
- Classification Metrics

---

## 🧠 Machine Learning Approach

```

Raw Questions
|
↓
Text Preprocessing
|
↓
CountVectorizer (Bag of Words)
|
↓
Feature Extraction
|
↓
Machine Learning Model
|
↓
Duplicate / Non-Duplicate Prediction

```

---

## 📊 Results

The trained models learn the semantic relationship between question pairs and predict whether they represent the same intent.

(Model performance can be updated after final training.)

---

## 📁 Project Structure

```

quora-question-pairs/
│
├── Dataset/
│
├── Notebook/
│   └── quora_question_pairs.ipynb
│
├── README.md
│
└── requirements.txt

🚀 Future Improvements

- Use TF-IDF instead of simple Bag of Words
- Apply Word Embeddings (Word2Vec, GloVe)
- Implement Deep Learning models
- Use Transformer-based models like BERT
- Improve semantic understanding

---

👨‍💻 Author

Muhammad Saad Bin Zubair

AI Engineer | Machine Learning & NLP Enthusiast  


⭐ If you find this project useful, consider giving it a star!



