# 🐦 Twitter Sentiment Analysis

A machine learning project that predicts **positive** or **negative** sentiment of tweets using **Logistic Regression**.

---

## 📌 Project Overview
This project uses **Natural Language Processing (NLP)** and **machine learning** to classify tweets. The workflow includes:  
1. Downloading the dataset from **Kaggle**.  
2. Data preprocessing (cleaning, stemming, removing stopwords).  
3. Feature extraction using **TF-IDF vectorization**.  
4. Training a **Logistic Regression model**.  
5. Evaluating accuracy on training and testing data.  
6. Predicting sentiment for new tweets.  

> **Note:** The model outputs `0` for **Negative** and `1` for **Positive** sentiment.

---

## ⚡ Features
- Preprocess tweets automatically.  
- Train a Logistic Regression model on the dataset.  
- Evaluate model performance using **accuracy score**.  
- Predict sentiment for any tweet.

---

## 🛠️ Tech Stack
- **Python 3**  
- **Pandas, NumPy**  
- **NLTK** (stopwords, stemming)  
- **Scikit-learn** (TF-IDF, Logistic Regression, train/test split)  
- **Pickle** (save/load model)

---

## 📂 Project Structure
twitter-sentiment-analysis/
│── data/ # CSV dataset from Kaggle (gitignored)
│── notebooks/ # Jupyter Notebook with code
│── src/ # Optional Python scripts
│── trained_model.sav # Saved Logistic Regression model
│── requirements.txt # Dependencies
│── README.md # Project documentation

---

## 📊 Dataset
- Dataset: [Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140) from Kaggle.  
- The dataset contains tweets labeled as positive (`1`) or negative (`0`).

---

## 🚀 Getting Started

### 1️⃣ Clone the repo
```bash
git clone https://github.com/your-username/twitter-sentiment-analysis.git
cd twitter-sentiment-analysis

### 2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Download dataset from Kaggle
# Install Kaggle API
pip install kaggle

# Create .kaggle directory and add kaggle.json API key
mkdir ~/.kaggle
copy kaggle.json ~/.kaggle/

# Download dataset
kaggle datasets download -d kazanova/sentiment140
unzip sentiment140.zip -d data/

4️⃣ Run the notebook

Open notebooks/twitter_sentiment_analysis.ipynb

Run all cells to preprocess data, train the model, and evaluate accuracy.

5️⃣ Predict sentiment of a new tweet
prediction = loaded_model.predict(["I love AI!"])
# Output: 0 -> Negative, 1 -> Positive