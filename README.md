# CSL7640: Natural Language Understanding

This repository contains solutions for:

1. **Problem 1:** Learning Word Embeddings from IIT Jodhpur Data
2. **Problem 2:** Character-Level Name Generation using RNN Variants

---

# 📌 Problem 1: Word Embeddings (Word2Vec)

## Overview

Text data is collected from IIT Jodhpur sources such as:

* Official website pages
* Academic regulation pages
* PDF documents (e.g., examination and attendance policies)

The collected text is cleaned and used to train Word2Vec models for semantic analysis.

---

## What is implemented

* Data collection (web + PDF)
* Text preprocessing:

  * Lowercasing
  * Tokenization
  * Noise and boilerplate removal
* Dataset statistics (documents, tokens, vocabulary size)
* Word cloud visualization
* Word2Vec training:

  * CBOW
  * Skip-gram with Negative Sampling
* Semantic analysis:

  * Nearest neighbors
  * Analogy tasks
* Visualization:

  * PCA
  * t-SNE

---

# 📌 Problem 2: Character-Level Name Generation

## Overview

A dataset of 1000 Indian names (`TrainingNames.txt`) is used to train sequence models that generate new names.

---

## Models implemented

* Vanilla RNN
* Bidirectional LSTM (BLSTM)
* RNN with Attention

---

## Evaluation

* Novelty Rate
* Diversity
* Qualitative analysis of generated names

---

# 📂 Repository Structure

```
.
├── problem1_word2vec.ipynb
├── problem2_rnn_names.ipynb
├── data/
│   └── TrainingNames.txt
└── README.md
```

---

## ⚙️ Requirements

The notebooks are designed to run on **Google Colab**.
All required libraries are installed within the notebooks using `pip install` commands.

---

# ⚙️ How to Run

## 🔹 Problem 1 (Word Embeddings)

1. Open `problem1_word2vec.ipynb` in **Google Colab**
2. Upload the required PDF files (e.g., academic regulations, circulars) 
3. Run all cells sequentially from top to bottom without skipping

The notebook will:

* extract text from PDFs and websites
* preprocess and create the corpus
* train Word2Vec models
* generate outputs such as statistics, word cloud, and embeddings

---

## 🔹 Problem 2 (Name Generation)

1. Open `problem2_rnn_names.ipynb` in **Google Colab**
2. Upload `TrainingNames.txt`
3. Run all cells sequentially from top to bottom

The notebook will:

* train RNN, BLSTM, and Attention models
* generate new names
* compute evaluation metrics
* display sample outputs

---

## 📎 Notes

* Outputs are generated during execution of the notebooks


