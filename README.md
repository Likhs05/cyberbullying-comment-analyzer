# Cyberbullying and Bad Comments Analyzer Using NLP Techniques

## 📌 Project Overview
Cyberbullying and offensive language on social media platforms pose serious social and psychological challenges. This project presents an automated system to detect cyberbullying and harmful comments using Natural Language Processing (NLP). The system combines a traditional machine learning model (Logistic Regression) with a lightweight transformer-based deep learning model (DistilBERT), followed by severity scoring, sentiment analysis, and rule-based prevention mechanisms.

---

## 🎯 Objectives
- Detect cyberbullying and abusive comments from textual data
- Compare traditional machine learning and transformer-based models
- Assign severity levels to harmful content
- Analyze sentiment polarity of user comments
- Apply rule-based preventive actions based on severity score

---

## 🧠 Methodology

### 1. Data Collection
- English-language social media comments
- Labeled dataset containing bullying and non-bullying content

### 2. Data Preprocessing
- Conversion of text to lowercase  
- Removal of URLs, emojis, punctuation, and special characters  
- Tokenization  
- Stopword removal  
- Lemmatization  

### 3. Feature Extraction
- TF-IDF for Logistic Regression  
- Tokenizer and contextual embeddings for DistilBERT  

### 4. Model Building
**Logistic Regression**
- Uses TF-IDF features  
- Fast and interpretable  
- Serves as a baseline model  

**DistilBERT**
- Lightweight transformer model derived from BERT  
- Captures contextual meaning of text  
- Faster and more computationally efficient than BERT  

### 5. Severity Score Calculation
Severity score is calculated based on:
- Prediction confidence from the classification model  
- Presence and intensity of abusive keywords  

Severity levels:
- Low  
- Medium  
- High  

### 6. Sentiment Analysis
- Classifies comments into Positive, Neutral, or Negative  
- Helps assess emotional intensity of detected content  

### 7. Rule-Based Prevention
Actions applied based on severity level:

| Severity Level | Action Taken |
|---------------|--------------|
| Low | Warning issued |
| Medium | Comment flagged |
| High | Comment blocked or reported |

### 8. Evaluation
Models are evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

Performance comparison is performed between Logistic Regression and DistilBERT.

---

## 🛠 Technologies Used
- Programming Language: Python  
- NLP Techniques: Tokenization, Lemmatization, TF-IDF  
- Machine Learning: Logistic Regression  
- Deep Learning: DistilBERT  
- Libraries:
  - Scikit-learn  
  - NLTK  
  - Transformers  
  - PyTorch  
  - Pandas  
  - NumPy  
  - Matplotlib  

---

## 📂 Project Structure
cyberbullying-comment-analyzer/
│
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
├── src/
│ ├── preprocessing.py
│ ├── logistic_regression_model.py
│ ├── distilbert_model.py
│ ├── severity_score.py
│ ├── sentiment_analysis.py
│ ├── rule_based_prevention.py
│ └── evaluation.py
│
├── docs/
│ ├── SRS.md
│ ├── architecture.md
│ └── flow_diagram.png
│
├── data/
│ └── README.md
│
└── results/

## 👩‍💻 Contributors
Putluri Chandra Harinadha Reddy (Project Lead)

Likhitha Gopalam

## 📜 License
This project is released under the MIT License.
