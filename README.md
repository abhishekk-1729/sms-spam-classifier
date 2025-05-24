# 📩 SMS Spam Classifier

This is a simple machine learning-based SMS/Email Spam Classifier built using Python, Streamlit, and Natural Language Processing (NLP). It classifies messages as either **Spam** or **Not Spam** based on their content.

## 🚀 Demo

Run the app locally and enter any SMS/Email message to check if it's spam or not.

---

## 🧠 How It Works

1. **Text Preprocessing:** 
   - Lowercasing
   - Tokenization
   - Removing stopwords and punctuation
   - Stemming

2. **Vectorization:** Uses a trained `TfidfVectorizer` to convert text to numerical format.

3. **Prediction:** A trained model (`model.pkl`) predicts if the message is spam.

---

## 🗂 Project Structure

```

SMS-SPAM-CLASSIFIER/
│
├── app.py                # Streamlit app script
├── model.pkl             # Trained classification model
├── vectorizer.pkl        # Trained TF-IDF vectorizer
├── spam.csv              # Dataset used for training
├── nltk.txt              # NLTK dependency instructions
├── requirements.txt      # Python dependencies
├── setup.sh              # Setup script (for deployment)
├── Procfile              # For deployment on Heroku
├── .gitignore            # Git ignore rules
└── README.md             # Project documentation

````

---

## 🛠 Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/abhishek_1729/sms-spam-classifier.git
cd sms-spam-classifier
````

2. **Create Virtual Environment (Optional but Recommended)**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. **Install Dependencies**

```bash
pip install -r requirements.txt
```

4. **Download NLTK Resources**

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

Alternatively, use:

```bash
python -m nltk.downloader punkt stopwords
```

5. **Run the App**

```bash
streamlit run app.py
```

---

## 📊 Dataset

The dataset (`spam.csv`) is used for training and testing the classifier. It contains labeled SMS messages as **spam** or **ham** (not spam).

---

## 📌 Dependencies

* streamlit
* scikit-learn
* nltk
* pickle

See `requirements.txt` for full list.

---


## 🙌 Acknowledgments

* [NLTK](https://www.nltk.org/)
* [Scikit-learn](https://scikit-learn.org/)
* [Streamlit](https://streamlit.io/)

---

### Made with ❤️ by \[Abhishek Kumar]
