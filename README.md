# 🧠 AI-Generated Text Detection Using Classical ML and Transformers

**Author:** Fouzia Shile  
**MSc Applied Computer Science & Artificial Intelligence — University of Bradford**  
**Module:** COS7045-B Advanced Machine Learning

---

## 📘 Overview

This project implements a comparative framework to detect AI-generated text using both **classical machine learning** and **transformer-based models**. It evaluates models on a diverse and augmented dataset of ~46,000 essays, addressing the rising challenge of distinguishing between human- and LLM-generated content in academic and real-world settings.

---

## 🎯 Objectives

- Detect LLM-generated text with high accuracy across different input lengths.
- Compare classical ML models vs. transformer models (BERT, DistilBERT, RoBERTa).
- Assess robustness, generalisation, and explainability.
- Highlight ethical and practical limitations of current detection tools.

---

## 📊 Models Used

### Classical ML Models:
- Logistic Regression (LR)
- Support Vector Machine (SVM)
- Multilayer Perceptron (MLP)
- Random Forest, Decision Tree, Naive Bayes, KNN

### Transformer Models:
- BERT (frozen & fine-tuned)
- DistilBERT (frozen & fine-tuned)
- RoBERTa (frozen & fine-tuned)

---

## 🧪 Evaluation

- F1-scores up to **0.99** achieved by LR, SVM, and MLP
- Frozen **RoBERTa** outperformed fine-tuned counterparts (F1 = 0.97)
- Analysis by **essay length** (short, medium, long)
- Comparison against current benchmarks like DetectGPT, GPTDetector

---

## 📂 Dataset

- **Source:** [Kaggle LLM Detect AI-Generated Text](https://www.kaggle.com/competitions/llm-detect-ai-generated-text)
- **Size:** 46,246 samples
- **Structure:** Binary labels (0 = Human, 1 = AI)
- **Augmentation:** Essays from GPT-4, PaLM, and Cohere; quality filtering via RDizzl3 Seven

📁 Dataset too large for GitHub — [Download from Google Drive](#) *(insert your link)*

---

## ⚙️ Code Structure

