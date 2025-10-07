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

📁 detectAItext Dataset is too large for GitHub, please find it here [Download from Google Drive](#) *(https://drive.google.com/file/d/1_nm_Ebw9SbntGoWnLhAWK9M3PZV5Afol/view?usp=share_link)*

---

## ⚙️ Code Structure


- Each notebook includes:
  - Preprocessing pipeline
  - Training and evaluation
  - Confusion matrices, F1 scores, and comparative plots

---

## 💻 Requirements

- Python ≥ 3.8  
- scikit-learn  
- pandas  
- matplotlib / seaborn  
- transformers (HuggingFace)  
- KerasNLP or TensorFlow  
- Jupyter / Google Colab  

> 📝 No external preprocessing needed — full pipeline is self-contained in notebooks.

---

## 📈 Key Findings

- Classical models (especially LR, SVM) **outperformed** fine-tuned transformers on the extended dataset.
- Freezing transformer backbones gave better stability.
- Input length affects performance — long essays reduced F1-scores across models.
- Detection is **non-trivial**, especially with advanced LLMs (e.g., GPT-4).

---

## ⚖️ Ethical Note

This project addresses a real-world problem with legal, ethical, and social implications. The study includes:
- Fairness and misclassification risks
- Legal compliance (e.g., GDPR)
- Limitations in model generalisability and dataset bias

---

## 📜 License

For academic use only. Contact [fouzia.shile@gmail.com](mailto:fouzia.shile@gmail.com) for permissions or collaborations.
