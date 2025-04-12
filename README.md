# 📊 Semantic Sentiment Analysis & Topic Modeling

This repository contains the full implementation, experiments, and results of our NLP project focused on **multi-class sentiment classification** and **topic modeling** on technology product reviews.

We explore a wide spectrum of models:
- ✅ Classical Machine Learning (Logistic Regression, Decision Trees)
- ✅ Deep Learning Models (LSTM, GRU, BiLSTM + Attention)
- ✅ Transformers (RoBERTa, XLNet, DeBERTa, CardiffNLP)
- ✅ Topic Modeling (LDA, LSA, NMF, BERTopic)
- ✅ FastText Baseline

## 📁 Project Structure

```bash
├── models/              # All sentiment classification models
│   ├── transformer/
│   ├── deep_learning/
│   ├── fasttext/
│   └── classical_ml/
├── topic_modeling/      # LDA, NMF, LSA, BERTopic scripts and results
├── data/                # Processed and labeled datasets
├── utils/               # Helper functions and preprocessing code
├── NLP_project.pdf      # 📄 **Final report describing all methods and findings**
├── requirements.txt     # Python dependencies
└── README.md            # You're here
```

## 🚀 Highlights

- Stratified 5-fold cross-validation across all models
- Robust handling of **class imbalance** using **focal loss**
- Topic modeling insights revealing brand-specific concerns
- Experimented with two datasets:
  - Custom Reddit-based dataset (U.S. Election 2024)
  - Real-world Amazon product reviews (Apple, Samsung, Lenovo)

---

## 📌 **Report**

📎 **You can find the full project report with all experiments, results, and explanations in [`NLP_project.pdf`](./NLP_project.pdf).**

---

## 📦 Installation

```bash
pip install -r requirements.txt
```

or for BERTopic:

```bash
pip install bertopic
```

---

## 📬 Contact

Made with ❤️ by:
- **Mohammadkazem Rajabi**  
- **Baharehsadat Khatami**

---
