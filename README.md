# 📝 English-to-French Translation Model 🇬🇧➡️🇫🇷

This repository contains my **Kaggle notebook implementation** of an English-to-French machine translation model using Hugging Face’s `Helsinki-NLP/opus-mt-en-fr`.  
The goal was to experiment with multilingual NLP and understand the workflow of training & evaluating a translation model.
---
##  Project Overview
- Dataset: **2M+ English–French sentence pairs** (sampled **100K pairs** for training).  
- Approach: Notebook-based implementation for **data preprocessing, training, and evaluation**.  
- Frameworks: Hugging Face 🤗 + TensorFlow ⚡.  
---
## ⚙️ Workflow
### 🔹 Data Preprocessing
- Imported dataset (CSV).  
- Cleaned data by removing `NaN` values.  
- Dropped duplicates to avoid translation conflicts.  
### 🔹 Model
- Pretrained Hugging Face model: [`Helsinki-NLP/opus-mt-en-fr`](https://huggingface.co/Helsinki-NLP/opus-mt-en-fr).  
- Tokenizer linked with the model.  
- Custom preprocessing function for source (English) and target (French).  

### 🔹 Training Setup
- Train/Val/Test split: **70% / 15% / 15%**  
- Hyperparameters:
  - Batch size: `16`  
  - Learning rate: `2e-5`  
  - Weight decay: `0.01`  
  - Epochs: `1`  
- Optimizer: **AdamW**  
---
## Implementation process

   * Data loading & cleaning
   * Tokenization & preprocessing
   * Model training
   * Evaluation & inference
---
##  Results & Learnings

* Careful **data preprocessing** is key for cleaner translations.
* **Transformers** shine in sequence-to-sequence tasks ⚡.
* Hugging Face + TensorFlow simplify building **scalable NLP pipelines**.
---
##  Future Work

* Extend to **other languages** (Yoruba → French, Hausa → English).
* Experiment with more of the 2M+ dataset (instead of 100K).
* Explore **beam search decoding** for improved translations.
---
##  Tech Stack
* Python 🐍
* Jupyter Notebook 📓
* Hugging Face Transformers 🤗
* TensorFlow ⚡
---
## Data Source URL: [https://www.kaggle.com/datasets/dhruvildave/en-fr-translation-dataset]
