# 📩 SMS Spam Classifier

A machine learning-based SMS Spam Detection system that classifies messages as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) techniques.

---

## 🚀 Project Overview

Spam messages are a common issue in communication systems. This project builds a classification model that automatically detects whether a given SMS is spam or not.

The model uses **text preprocessing, feature extraction (TF-IDF), and machine learning algorithms** to achieve high accuracy.

---

## 🧠 Problem Statement

Given a dataset of SMS messages, build a model that can:
- Classify messages as **Spam or Ham**
- Minimize false positives (important for business use)
- Be scalable for real-time applications

---

## 📊 Dataset

- Source: Public SMS Spam Collection Dataset
- Features:
  - `label`: spam or ham
  - `message`: actual SMS text

---

## ⚙️ Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- NLTK
- Matplotlib / Seaborn

---

## 🔍 Approach

### 1. Data Preprocessing
- Lowercasing text
- Removing punctuation
- Tokenization
- Stopword removal
- Stemming (Porter Stemmer)

### 2. Feature Engineering
- Converted text to numerical format using:
  - **TF-IDF Vectorization**

### 3. Model Building
- Trained multiple models:
  - Naive Bayes (Best performing)
  - Logistic Regression
  - Random Forest

### 4. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score

---

## 📈 Results

| Model               | Accuracy | Precision |
|--------------------|---------|----------|
| Naive Bayes        | ~97%    | High     |
| Logistic Regression| ~95%    | Medium   |
| Random Forest      | ~96%    | High     |

👉 **Final Model Selected:** Naive Bayes (Best balance of precision & recall)

---

## 💡 Key Insights

- Spam messages often contain promotional keywords (e.g., "free", "win", "offer")
- TF-IDF significantly improves classification performance
- Naive Bayes works extremely well for text classification problems

---

## 🖥️ How to Run the Project

### Step 1: Clone the repository
```bash
git clone https://github.com/your-username/sms-spam-classifier.git
cd sms-spam-classifier
