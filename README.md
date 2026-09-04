# 🧠 Quora Question Pair — Duplicate Question Detection

### `NLP` • `Machine Learning` • `Text Classification` • `Bag of Words`

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/NLP-Text%20Classification-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikit-learn" />
  <img src="https://img.shields.io/badge/Quora-Duplicate%20Detection-red?style=for-the-badge" />
</p>

---

## 🚀 Project Overview    

Have you ever seen the **same question asked multiple times on Quora**, just written in a slightly different way?

For example:

> **Question 1:** How can I learn Python?
> **Question 2:** What is the best way to learn Python?

Although the wording is different, both questions are asking essentially the **same thing**.

This project uses **Natural Language Processing (NLP)** and **Machine Learning** to determine whether two Quora questions are **duplicate questions or not**.

### 🎯 Objective

Given two questions, the model predicts:

```text
1 → Duplicate Questions
0 → Non-Duplicate Questions
```

---

## ✨ Why This Problem Matters

Quora receives a huge number of questions every day.

Without duplicate detection:

```text
User Question
      ↓
Same / Similar Question Already Exists
      ↓
Duplicate Content
      ↓
Poor Search Experience
```

With duplicate detection:

```text
Question Pair
      ↓
NLP Processing
      ↓
Feature Extraction
      ↓
Machine Learning Model
      ↓
Duplicate / Non-Duplicate
```

The goal is to help identify questions that are asking the **same thing**, even when their wording is different.

---

# 🧩 Project Pipeline

```text
             Quora Question Dataset
                       │
                       ▼
              ┌─────────────────┐
              │ Data Loading    │
              │ & Exploration   │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Text            │
              │ Preprocessing   │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Bag of Words    │
              │ CountVectorizer │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Feature         │
              │ Representation  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ ML Classifier   │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Prediction      │
              │                 │
              │  Duplicate      │
              │      or         │
              │  Non-Duplicate  │
              └─────────────────┘
```

---

# 🔍 Example

### Example 1 — Duplicate

```text
Question 1:
How can I learn Python?

Question 2:
What is the best way to learn Python?
```

```text
Prediction → Duplicate (1) ✅
```

---

### Example 2 — Non-Duplicate

```text
Question 1:
How can I learn Python?

Question 2:
How can I learn Java?
```

```text
Prediction → Non-Duplicate (0) ❌
```

---

# 🛠️ Technologies Used

### 👨‍💻 Programming

`Python`

### 📊 Data Processing

`Pandas` • `NumPy`

### 🧠 NLP

`Text Preprocessing` • `Bag of Words` • `CountVectorizer`

### 🤖 Machine Learning

`Scikit-Learn` • `Logistic Regression` • `Random Forest` • `XGBoost`

### 📈 Visualization

`Matplotlib`

### 📓 Development

`Jupyter Notebook`

---

# 📂 Dataset

This project uses the **Quora Question Pairs Dataset** from Kaggle.

The dataset contains pairs of questions along with a binary label indicating whether the questions are duplicates.

```text
question1
question2
is_duplicate
```

Where:

```text
1 → Duplicate
0 → Not Duplicate
```

---

# 🔬 Machine Learning Approach

The project converts textual questions into numerical representations using **Bag of Words (BoW)**.

```text
Raw Text
   ↓
Text Preprocessing
   ↓
CountVectorizer
   ↓
Numerical Feature Matrix
   ↓
Machine Learning
   ↓
Prediction
```

The model learns patterns from the question pairs and predicts whether they belong to the duplicate or non-duplicate class.

---

# 📊 Models

The project explores multiple classification algorithms:

| Model               | Purpose                          |
| ------------------- | -------------------------------- |
| Logistic Regression | Baseline classification          |
| Random Forest       | Ensemble-based classification    |
| XGBoost             | Gradient boosting classification |

---

# 📈 Evaluation

Models are evaluated using classification metrics such as:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

> Model performance can vary depending on preprocessing, feature engineering, train/test split and model configuration.

---

# 📁 Project Structure

```text
Quora-Question-pair-competition/
│
├── README.md
│
├── only_BOW.ipynb
│
└── streamlit-app/
```

---

# 🌐 Streamlit Application

A Streamlit interface can be used to make the project interactive.

The idea is simple:

```text
       User enters Question 1
                  │
                  ▼
       User enters Question 2
                  │
                  ▼
          ┌───────────────┐
          │ NLP Pipeline  │
          └───────┬───────┘
                  │
                  ▼
        Machine Learning Model
                  │
                  ▼
       ┌─────────────────────┐
       │ Duplicate / Not     │
       │ Duplicate           │
       └─────────────────────┘
```

This makes the project easier to demonstrate and test.

---

# 🚀 Future Improvements

The current implementation uses **Bag of Words**, which is a traditional text representation technique.

The project can be improved further by implementing:

```text
Bag of Words
     ↓
TF-IDF
     ↓
Word2Vec / GloVe
     ↓
Sentence Embeddings
     ↓
BERT / Transformer Models
```

Possible future improvements include:

* 🔹 TF-IDF features
* 🔹 Word2Vec / GloVe embeddings
* 🔹 Sentence Transformers
* 🔹 Cosine similarity
* 🔹 Siamese Neural Networks
* 🔹 BERT-based duplicate detection
* 🔹 Advanced feature engineering
* 🔹 Better Streamlit UI
* 🔹 Model comparison dashboard

---

# 💡 What I Learned

Through this project, I explored:

* Natural Language Processing
* Text preprocessing
* Exploratory Data Analysis
* Bag of Words
* CountVectorizer
* Feature engineering
* Binary text classification
* Machine Learning model comparison
* Model evaluation
* Building NLP applications

---

# 🧠 Key Concept

The main idea behind the project is:

> **Two questions can be written differently while asking the same thing.**

The challenge is therefore to learn patterns from question pairs and classify them as:

```text
         Question Pair
              │
       ┌──────┴──────┐
       │             │
    Duplicate     Different
       │             │
       ▼             ▼
       1             0
```

---

# 👨‍💻 Author

### Muhammad Saad Bin Zubair

**AI/ML Engineer • Python • Machine Learning • NLP • Generative AI**

Interested in building practical AI systems using:

`Machine Learning` • `Deep Learning` • `NLP` • `RAG` • `LLMs` • `AI Agents`

---

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐

### 🚀 Learn → Build → Experiment → Improve

**Machine Learning • NLP • AI**
