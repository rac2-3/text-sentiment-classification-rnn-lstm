# 📊 Text Sentiment Classification using RNN & LSTM

## 📌 Overview

This project focuses on performing **sentiment analysis** on text data using deep learning models. The goal is to classify movie reviews as **positive** or **negative** using **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** networks.

---

## 🎯 Objectives

* Load and preprocess the IMDB dataset
* Build a baseline **SimpleRNN model**
* Build an advanced **LSTM model**
* Compare performance of RNN vs LSTM
* Evaluate models using classification metrics

---

## 📂 Dataset

* **Dataset:** IMDB Movie Reviews
* **Total Samples:** 50,000

  * 25,000 Training
  * 25,000 Testing
* **Classes:**

  * `0` → Negative
  * `1` → Positive

---

## ⚙️ Data Preprocessing

* Tokenization (text → integer sequences)
* Vocabulary limited to top **10,000 words**
* Sequence padding to fixed length (**200**)
* Uniform input shape for neural networks

---

## 🧠 Models Used

### 🔹 SimpleRNN

* Embedding Layer (128 units)
* SimpleRNN Layer (64 units)
* Dense Output Layer (Sigmoid)

### 🔹 LSTM

* Embedding Layer (128 units)
* LSTM Layer (64 units)
* Dense Output Layer (Sigmoid)

---

## ⚙️ Training Configuration

* **Optimizer:** Adam
* **Loss Function:** Binary Crossentropy
* **Epochs:** 5
* **Batch Size:** 64
* **Validation Split:** 0.2

---

## 📊 Results

| Model     | Accuracy | F1 Score |
| --------- | -------- | -------- |
| SimpleRNN | ~82%     | ~0.82    |
| LSTM      | ~86%     | ~0.86    |

👉 LSTM outperforms RNN due to its ability to capture long-term dependencies.

---

## 📈 Visualizations

* Training vs Validation Accuracy
* Training vs Validation Loss
* Comparison of RNN and LSTM performance

---

## 🧪 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score

---

## 🔍 Key Observations

* LSTM achieves higher validation accuracy than RNN
* RNN shows signs of overfitting after a few epochs
* LSTM provides more stable and generalized performance

---

## 🧠 Why LSTM is Better?

LSTM uses:

* Input Gate
* Forget Gate
* Output Gate

These mechanisms help retain important information over long sequences, solving the **vanishing gradient problem** present in traditional RNNs.

---

## 🛠️ Tools & Technologies

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn

---

## 📁 Project Structure

```
├── Assignment3.ipynb
├── Assignment3_Report.pdf
└── README.md
```

---

## 🚀 Future Improvements

* Use Bidirectional LSTM
* Add Dropout for regularization
* Use pre-trained embeddings (GloVe, Word2Vec)

---

## 👨‍🎓 Author

**Raj Tilak Singh**
MCA (AI & ML)
K.R. Mangalam University

---

## 📌 Conclusion

This project demonstrates that **LSTM significantly improves sentiment classification performance** compared to traditional RNN models, making it more suitable for sequential text data tasks.
