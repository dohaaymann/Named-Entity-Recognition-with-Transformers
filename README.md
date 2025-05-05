# 🧠 Named Entity Recognition with BERT

This project fine-tunes a BERT-based Transformer model to perform Named Entity Recognition (NER) using Hugging Face Transformers and Datasets libraries.

## 🚀 Project Overview

Named Entity Recognition (NER) is the task of detecting and classifying named entities like people, organizations, locations, etc., from text. This project uses the `bert-base-cased` model to train on a labeled dataset for NER and evaluate its performance using standard NLP metrics.
<p align="center">
  <img src="https://github.com/dohaaymann/Named-Entity-Recognition-with-Transformers/raw/main/NER Image.png" width="600"/>
</p>
## 📁 Dataset

- **Source**: [Kaggle NER Dataset](https://www.kaggle.com/datasets/abhinavwalia95/entity-annotated-corpus)
- **Format**: CSV with columns: `Sentence #`, `Word`, `POS`, `Tag`
- **Preprocessing**:
  - Grouped tokens into sentences
  - Mapped tags to IDs
  - Created Hugging Face-compatible `DatasetDict`
  - Split into 80% train / 20% test

## 🧪 Model & Training

- **Model Used**: `bert-base-cased`
- **Framework**: PyTorch + Hugging Face Transformers
- **Tokenizer**: AutoTokenizer with token-label alignment
- **Training Config**:
  - Learning Rate: `2e-5`
  - Batch Size: `16`
  - Epochs: `3`
  - Weight Decay: `0.01`

