# 🚀 NLP Task 5: Token Classification using DistilBERT

## 📌 Overview
This project focuses on fine-tuning a transformer model (**DistilBERT**) for **Token Classification** tasks such as:
- Part-of-Speech (POS) Tagging  
- Chunking (Phrase Detection)

The implementation uses Hugging Face Transformers and the WikiANN dataset.

---

## 🎯 Objective
To build and fine-tune a transformer-based model for sequence labeling tasks and understand preprocessing, label alignment, training, and evaluation.

---

## 📂 Dataset
- **Dataset Used:** WikiANN (English)
- **Task Type:** Token Classification (NER-style)
- **Labels Include:**
  - B-PER (Person)
  - B-ORG (Organization)
  - B-LOC (Location)
  - I-* (Inside entities)
  - O (Outside)

---

## ⚙️ Technologies Used
- Python
- Hugging Face Transformers
- Datasets Library
- PyTorch
- SeqEval

---

## 🔄 Workflow
Raw Data → Tokenization → Label Alignment → Model Training → Evaluation → Inference

---

## 🔧 Model Details
- **Model:** DistilBERT (`distilbert-base-uncased`)
- **Task:** Token Classification
- **Library:** Hugging Face Transformers

---

## 🧹 Data Preprocessing
- Tokenization using BERT tokenizer
- Alignment of labels with tokens
- Handling subwords:
  - First subword → label
  - Remaining → `-100`
- Special tokens ignored using `-100`

---

## 🏋️ Training Details
- Epochs: 2  
- Learning Rate: 3e-5  
- Batch Size: 16  
- Optimizer: AdamW  
- GPU used for faster training  

---

## 📊 Evaluation Metrics
- Precision  
- Recall  
- F1 Score  

---

## 📈 Results
- Precision: ~0.85  
- Recall: ~0.85  
- F1 Score: ~0.85  

---

## 🔍 Inference Example
**Input:**
