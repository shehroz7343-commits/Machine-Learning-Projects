# 📰 Fake News Prediction System using Machine Learning

This project implements a complete Natural Language Processing (NLP) and Machine Learning pipeline using Python, NLTK, and Scikit-Learn to classify news articles as **Real** or **Fake**.

---

## 📊 Dataset Overview

The dataset (`train.csv`) contains text data and metadata related to news articles.
* **Total Instances:** 20,822 records
* **Target Variable:** `label` 
  * `1` $\rightarrow$ Fake News
  * `0` $\rightarrow$ Real News

### Features:
1. **id:** Unique ID for a news article
2. **title:** The title of the news article
3. **author:** Author of the news article
4. **text:** The complete text body of the article
5. **content:** Merged column combining `author` and `title` for streamlined processing

---

## ⚙️ Project Pipeline & Steps

1. **Data Preprocessing & Cleaning:**
   * Handled and filled missing values (`NaN`) in text, author, and title columns.
   * Combined author and title columns to form a unified `content` feature.

2. **Text Stemming & Cleaning (NLP):**
   * Removed non-alphabetical characters using regular expressions (`re`).
   * Converted all text to lowercase and tokenized it.
   * Filtered out English stop words using NLTK's `stopwords` corpus.
   * Applied stemming using `PorterStemmer` to reduce words to their root forms.

3. **Feature Extraction (Vectorization):**
   * Converted preprocessed text data into numerical TF-IDF (Term Frequency-Inverse Document Frequency) features using `TfidfVectorizer`.

4. **Data Splitting & Stratification:**
   * Split data into features (`X`) and target (`y`).
   * Performed a stratified train-test split (`80% training, 20% testing`) to preserve class distribution.

5. **Model Training & Evaluation:**
   * Trained a **Logistic Regression** classifier on the training data.
   * Evaluated model accuracy using `accuracy_score`:
     * **Training Accuracy:** ~98.65%
     * **Testing Accuracy:** ~97.48%
   * Built a predictive system to test new unseen data samples.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Text Processing & NLP:** NLTK (Stopwords, PorterStemmer), Regular Expressions (`re`)
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Machine Learning & Modeling:** Scikit-Learn (LogisticRegression, TfidfVectorizer, train_test_split, accuracy_score)

---

## 🚀 How to Run the Code

1. Ensure you have the required libraries installed:
   ```bash
   pip install numpy pandas scikit-learn nltk seaborn matplotlib
