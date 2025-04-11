# Semantic Analysis on Tech Product Reviews

This repository contains the full implementation, code, data (where permitted), and LaTeX report for our NLP course project: **Sentiment and Semantic Analysis of Technology Product Reviews**, with a special focus on Apple and Samsung.

## 🔍 Project Overview

We performed multi-class sentiment classification (positive, neutral, negative) on real-world product reviews from the Amazon 5-core Electronics dataset. Our work includes:

- Preprocessing and cleaning ~17,000 reviews
- Fine-tuning transformer models (e.g., RoBERTa, XLNet, DeBERTa)
- Deep learning with RNN variants (LSTM, GRU, BiLSTM + Attention)
- FastText baseline
- Classical ML models
- Topic modeling with LDA, LSA, NMF, and BERTopic

We also compared our current work with a previous sentiment analysis task we conducted on manually labeled Reddit comments related to the 2024 U.S. Election.

## 📁 Directory Structure

```
├── notebooks/
│   ├── transformers/
│   ├── deep_learning/
│   ├── classical_ml/
│   ├── topic_modeling/
├── data/
│   ├── semantic_tech_real.csv
│   ├── semantic_tech_10k.csv
│   └── reddit_us_election.csv
├── models/
│   ├── saved_transformer_checkpoints/
│   ├── fasttext.bin
├── report/
│   ├── NLP_project.pdf
│   └── presentation_slides/
├── logs/
│   └── cluster_logs/
├── README.md
└── requirements.txt
```

## 📊 Results

### 📈 Transformer Performance (Tech Dataset)

| Model              | Accuracy | F1-score |
|-------------------|----------|----------|
| CardiffNLP        | 75.98%   | 75.46%   |
| DeBERTa-v3-large  | 75.26%   | 75.32%   |
| RoBERTa           | 72.60%   | 72.23%   |

### 🔁 Deep Learning

| Model                        | Accuracy | F1-score |
|-----------------------------|----------|----------|
| BiLSTM + Attention + GloVe  | 70.00%   | 66.00%   |
| GRU + GloVe                 | 70.84%   | 70.99%   |

### ⚡ FastText Baseline

- Accuracy: 66.15%
- Macro F1: 62.63%

### 📚 Topic Modeling (Example from LDA)

| Topic | Top Keywords |
|-------|--------------|
| 1     | cable, usb, adapter, sound, iphone |
| 2     | laptop, lenovo, windows, mouse, computer |
| ...   | ... |

## 🧠 Tools & Libraries

- HuggingFace Transformers
- TensorFlow & Keras
- Scikit-learn
- FastText (Facebook AI)
- NLTK & Gensim
- BERTopic, SVD, NMF
- Google Colab & University HPC Cluster

## 🛠️ Reproducibility

- All notebooks are modular and self-contained.
- Pretrained models and log files are provided where possible.
- Run `requirements.txt` to install dependencies.
- Check `report/NLP_project.pdf` for methodology and results.

## 👥 Authors

- **Mohammadkazem Rajabi** – [Email](mailto:Mohammadkazem.rajabi@unipd.studenti.it)
- **Baharehsadat Khatami** – [Email](mailto:Baharehsadat.khatami@unipd.studenti.it)

Special thanks to **Amir Sadeghi** for contributing to the annotation of the Reddit dataset.

## 📄 License

This repository is for academic and research purposes only. If you use this project, please cite our report and acknowledge our work.
