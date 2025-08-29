# Sentiment Analysis on Amazon Fine Food Reviews

## 📌 Overview
This project was developed as part of my **Data Science Internship at Pinnacle Labs**.  
The goal is to perform **sentiment analysis** on the Amazon Fine Food Reviews dataset using **Natural Language Processing (NLP)** and **Machine Learning techniques**.  

The analysis includes:
- **Exploratory Data Analysis (EDA)**
- **Text preprocessing**
- **Sentiment polarity scoring**
- **Naive Bayes classification** (Positive/Negative reviews)

---

## 📂 Dataset
- **Source**: [Amazon Fine Food Reviews dataset (Kaggle)](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)  
- **Size**: 500,000+ reviews (subset of 500 rows used in this project for demonstration)  
- **Columns include**:  
  - `Id`, `ProductId`, `UserId`  
  - `ProfileName`, `HelpfulnessNumerator`, `HelpfulnessDenominator`  
  - `Score` (star rating: 1–5)  
  - `Time`, `Summary`, `Text` (main review body)  

---

## 🔑 Key Steps

### 1. Data Preprocessing
- Handled missing values & cleaned DataFrame  
- Selected a smaller subset (500 rows) for analysis  
- Converted text to lowercase, removed punctuation & stopwords  

### 2. Exploratory Data Analysis (EDA)
- Distribution of star ratings (pie chart, bar chart, line chart)  
- Review length analysis  
- Word cloud visualization for **positive** and **negative** reviews  

### 3. Natural Language Processing (NLP)
- Tokenization using **NLTK**  
- Stopword removal  
- Stemming (PorterStemmer)  
- Frequency distribution of words  

### 4. Sentiment Analysis
- **TextBlob** for sentiment polarity scoring  
- Classified reviews into **Positive**, **Negative**, or **Neutral**  

### 5. Machine Learning Model
- Built a **Naive Bayes classifier (NLTK)**  
- Features: Bag-of-Words representation  
- Trained model to classify sentiment  
- Evaluated performance with **accuracy** and sample predictions  

---

## 📊 Results
- Positive reviews dominate the dataset (scores 4–5).  
- Negative reviews are fewer but often detailed (scores 1–2).  
- **Naive Bayes model** achieved promising results on small-scale data.  
- Word clouds clearly highlight common positive (e.g., *great, love, delicious*) and negative (e.g., *bad, waste, disappointed*) terms.  

---

## 🚀 Technologies Used
- **Python**  
- **Pandas, NumPy** – Data manipulation  
- **Matplotlib, Seaborn, WordCloud** – Data visualization  
- **NLTK** – Tokenization, stopwords, stemming, Naive Bayes model  
- **TextBlob** – Sentiment polarity scoring  

---

## 📌 Future Work
- Train on the **full dataset (500k+ reviews)** for better generalization  
- Experiment with advanced models (e.g., Logistic Regression, SVM, LSTM, BERT)  
- Implement **aspect-based sentiment analysis** (taste, packaging, delivery, etc.)  
- Build a **streamlit web app** for real-time sentiment prediction  

---

## 🏢 Acknowledgements
- **Pinnacle Labs** – Internship mentorship and guidance  
- **Kaggle** – Dataset source  
- **NLTK & TextBlob** – Open-source NLP tools  
