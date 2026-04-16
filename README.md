# 📧 Spam Email Detection using TensorFlow

This project demonstrates how to build a **Spam Email Classifier** using **Natural Language Processing (NLP)** and **Deep Learning (LSTM)** in TensorFlow.

The model classifies emails into:

* 🚫 Spam
* ✅ Ham (Not Spam)

---

## 🚀 Features

* Text preprocessing (stopword removal, punctuation cleaning)
* Data balancing for improved performance
* Tokenization & sequence padding
* LSTM-based deep learning model
* Early stopping & learning rate optimization
* Visualization using WordCloud and accuracy plots

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* Numpy & Pandas
* Matplotlib & Seaborn
* NLTK
* Scikit-learn

---

## 📂 Dataset

* Contains labeled emails (`spam` or `ham`)
* Total records: **5171**
* Format: CSV file (`Emails.csv`)

---

## ⚙️ Workflow

### 1. Data Loading

* Load dataset using Pandas
* Inspect structure and distribution

### 2. Data Preprocessing

* Remove unnecessary text (e.g., "Subject")
* Remove punctuation
* Remove stopwords
* Convert text to lowercase

### 3. Data Balancing

* Downsample majority class (Ham)
* Create balanced dataset

### 4. Visualization

* Count plot for label distribution
* WordCloud for spam vs ham emails

### 5. Tokenization & Padding

* Convert text into sequences
* Pad sequences to fixed length

### 6. Model Building

* Embedding Layer
* LSTM Layer
* Dense Layers
* Sigmoid Output Layer

### 7. Model Training

* EarlyStopping callback
* ReduceLROnPlateau callback
* Train-validation split

### 8. Evaluation

* Accuracy and loss calculation
* Achieved ~**97% accuracy**

---

## 🧠 Model Architecture

Embedding → LSTM → Dense → Output

* Embedding: Converts words into vectors
* LSTM: Learns sequence patterns
* Dense: Extracts features
* Output: Binary classification

---

## 📊 Results

* ✅ Test Accuracy: ~97%
* 📉 Low loss
* 📈 Good generalization

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/spam-email-detection.git
cd spam-email-detection
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the project:

```bash
python main.py
```

---

## 📦 Requirements

```
numpy
pandas
matplotlib
seaborn
tensorflow
nltk
scikit-learn
wordcloud
```

---

## 💡 Future Improvements

* Use larger dataset
* Try Bidirectional LSTM / GRU
* Use pre-trained embeddings (GloVe, Word2Vec)
* Deploy using Flask or Streamlit
* Hyperparameter tuning

---

