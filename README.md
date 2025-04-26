# Aspect-Based Sentiment Analysis (ABSA) with BiLSTM and Attention

This project focuses on classifying fine-grained sentiments towards specific aspects within a sentence.  
I built a BiLSTM-Attention model that integrates word, aspect, POS, and dependency embeddings to predict sentiments as **positive**, **negative**, or **neutral**.

## Project Structure

- **data/** — Ttrain, validation, and test datasets (JSON format)
- **absa_bilstm_pipeline.ipynb** — Main notebook for preprocessing, feature engineering, model training, and evaluation
- **.gitignore** — Clean tracking setup

## Model Overview

- **Base architecture:** BiLSTM with attention mechanism
- **Embeddings used:**  
  - Pretrained Word2Vec word embeddings  
  - Aspect embeddings  
  - POS tag embeddings  
  - Dependency relation embeddings
- **Training:**  
  - PyTorch framework  
  - Trained with batch-level padding and masking  
  - Optimized using Adam optimizer
- **Evaluation:**  
  - Confusion matrix and classification report (precision, recall, F1)
  - Test set accuracy: ~63.7%

  ## Technologies

- Python
- PyTorch
- scikit-learn
- Matplotlib, Seaborn
- WandB (experiment tracking)

## Final Test Results

| Metric      | Value  |
|:------------|:-------|
| Test Accuracy | 63.7% |
| Best F1 Score | 73% (Neutral class) |