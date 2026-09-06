# 🧠 WordPredict AI

### LSTM-Based Neural Language Prediction

**WordPredict AI** is a Deep Learning–based neural language modeling system designed to predict the most probable next word from a given textual context. The project leverages **Natural Language Processing, sequence modeling, word embeddings, and LSTM networks** to learn contextual and sequential dependencies within text.

The trained model is integrated with **Streamlit** to provide real-time inference through an interactive web interface.

---

## 🚀 Overview

The system transforms raw textual data into sequential training patterns and learns the probability distribution of the next token given a preceding word sequence.

**Core Objective:**

> Given a sequence of words, estimate the most probable subsequent word using a trained neural language model.

**Example:**

```text
Input:
life is too

Output:
short
```

## 🔄 Architecture & Workflow

```text
                    Text Corpus
                        │
                        ▼
              Text Normalization
                        │
                        ▼
          Tokenization & Vocabulary Mapping
                        │
                        ▼
             Sequence Construction
                        │
                        ▼
               Sequence Padding
                        │
                        ▼
                Word Embedding
                        │
                        ▼
              LSTM Sequence Modeling
                        │
                        ▼
             Dense + Softmax Layer
                        │
                        ▼
              Next-Word Inference
                        │
                        ▼
              Streamlit Deployment
```

## 🧠 Model Architecture

Input Sequence
      │
      ▼
Embedding Layer
      │
      ▼
LSTM Layer — 128 Units
      │
      ▼
Dense Layer
      │
      ▼
Softmax Output
      │
      ▼
Predicted Next Token


| Component               | Configuration             |
| ----------------------- | ------------------------- |
| **Vocabulary Size**     | 10,000 tokens             |
| **Embedding Dimension** | 50                        |
| **LSTM Units**          | 128                       |
| **Optimizer**           | Adam                      |
| **Loss Function**       | Categorical Cross-Entropy |
| **Output Activation**   | Softmax                   |


The LSTM architecture is used to capture sequential dependencies and contextual relationships across variable-length text sequences.

## 📊 Dataset

The model is trained on a quote-based textual corpus containing 3,038 records. After preprocessing and sequence construction, the corpus generates approximately 85K supervised training sequences for neural language modeling.

## ✨ Key Features
🔹 Context-aware next-word prediction
🔹 NLP-based text preprocessing and tokenization
🔹 Sequential data construction for language modeling
🔹 Word embedding representation
🔹 LSTM-based sequence learning
🔹 Softmax-based probabilistic word prediction
🔹 Multi-word text generation
🔹 Saved model and tokenizer for inference
🔹 Interactive Streamlit deployment


🛠️ Tech Stack

Programming Language:
Python

Deep Learning:
TensorFlow • Keras • LSTM • SimpleRNN

Natural Language Processing:
Tokenization • Sequence Modeling • Word Embeddings

Data Processing:
NumPy • Pandas

Visualization:
Matplotlib • Seaborn

Deployment:
Streamlit

Development Environment:
Google Colab • Jupyter Notebook • VS Code

## 🔮 Future Scope
🔹 Top-K probabilistic predictions
🔹 Temperature-based text sampling
🔹 Bidirectional LSTM and GRU architectures
🔹 Attention-based sequence modeling
🔹 Transformer-based language models
🔹 Larger and domain-diverse text corpora
