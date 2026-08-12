# SMS Spam Detection

## Problem Statement

Mobile messaging is a widely used form of communication, with billions of users exchanging messages every day. However, SMS communication can be affected by **spam messages**, which may contain unwanted advertisements, fraudulent content, or malicious links.

The lack of effective message filtering can make mobile communication less secure and convenient. Therefore, this project aims to develop an **NLP-based machine learning model that accurately classifies an SMS message as either Spam or Ham (legitimate)**.

---

## Project Flow

```text
Problem Statement
       ↓
Data Gathering
       ↓
Data Preprocessing
       ↓
Text Vectorization
       ↓
Model Building
       ↓
Model Evaluation
       ↓
Model Deployment
       ↓
Prediction on Client Data
```

### 1. Data Gathering

The SMS dataset is collected containing messages labeled as:

* **Ham** – Legitimate SMS
* **Spam** – Unwanted or fraudulent SMS

### 2. Data Preprocessing

The raw SMS text is cleaned and prepared for machine learning.

#### A. Tokenization

Breaking the SMS into individual words or tokens.

#### B. Lowercasing

Converting all text into lowercase to maintain consistency.

#### C. Stopword Removal

Removing commonly used words that provide little useful information, such as:

```text
is, the, a, an, and, of, to
```

#### D. Lemmatization / Stemming

Reducing words to their root or base form.

Example:

```text
playing → play
played  → play
plays   → play
```

---

## 3. Text Vectorization

Machine learning models cannot directly process raw text. Therefore, text is converted into numerical vectors.

### A. Bag of Words (CountVectorizer)

**CountVectorizer** represents text based on the number of times each word occurs in a document.

### B. TF-IDF

**TF-IDF (Term Frequency–Inverse Document Frequency)** assigns importance to words based on how frequently they occur in a message and how common they are across the dataset.

---

## 4. Model Building

### A. Model Object Initialization

Machine learning classification algorithms are initialized and configured.

Possible algorithms include:

* Naive Bayes
* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree
* Random Forest

### B. Train and Test Model

The dataset is divided into training and testing sets.

```text
Dataset
   ↓
Training Data → Train Model
   ↓
Testing Data → Evaluate Model
```

The model learns patterns from the training data and predicts whether unseen SMS messages are **Spam or Ham**.

---

## 5. Model Evaluation

The trained model is evaluated using different performance metrics.

### A. Accuracy Score

Measures the percentage of correctly classified SMS messages.

### B. Confusion Matrix

Shows the number of:

* True Positives
* True Negatives
* False Positives
* False Negatives

### C. Classification Report

Provides important metrics such as:

* Precision
* Recall
* F1-score
* Support

---

## 6. Model Deployment

The trained model can be deployed as an application where users can enter an SMS message and receive a prediction.

```text
User enters SMS
       ↓
Text Preprocessing
       ↓
Vectorization
       ↓
Trained ML Model
       ↓
Spam / Ham Prediction
```

---

## 7. Prediction on Client Data

The deployed system accepts a new SMS message from the user and predicts whether it is **Spam** or **Ham**.

### Example

**Input:**

```text
Congratulations! You have won a free prize. Click here to claim.
```

**Output:**

```text
Prediction: Spam
```

---

## Tech Stack Used

### Programming Language

* Python

### Natural Language Processing

* NLP
* Tokenization
* Stopword Removal
* Stemming / Lemmatization
* Text Cleaning

### Text Vectorization

* CountVectorizer
* TF-IDF

### Machine Learning

* Naive Bayes
* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree
* Random Forest

### Model Evaluation

* Accuracy Score
* Confusion Matrix
* Classification Report

---

## Project Objective

The main objective of this project is to develop an **accurate and efficient SMS spam detection system using Natural Language Processing and Machine Learning** that can automatically distinguish between spam and legitimate messages.

---

## Keywords

`SMS Spam Detection` `NLP` `Machine Learning` `TF-IDF` `CountVectorizer` `Naive Bayes` `SVM` `Text Classification` `Spam Detection`

