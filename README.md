# QuoteSense

**A Multi-Model Pipeline for Emotion Detection in Motivational Quotes**

QuoteSense is an end-to-end NLP pipeline designed to classify emotions in motivational quotes. It integrates traditional ML, deep learning (LSTM), and transformer models (DistilBERT), and introduces stylistic analysis to compare AI-generated and human-written quotes.

---

## 🔍 Project Overview

We used a dataset of 44,000 motivational quotes:
- 22,000 human-authored (scraped from the web)
- 22,000 AI-generated

Each quote is labeled with an emotion and augmented with four custom features:
- **CreativityScore**
- **PoeticToneScore**
- **EmotionalBalanceIndex**
- **SemanticClicheScore**

---

## Modeling Approaches

1. **TF-IDF + Logistic Regression** – Simple baseline model
2. **LSTM Neural Network** – Captures sequential patterns in text
3. **DistilBERT** – Transformer fine-tuned for emotion classification

---

## Key Findings

| Model             | Accuracy |
|------------------|----------|
| Logistic Regression | ~0.70 |
| LSTM               | ~0.73 |
| DistilBERT         | ~0.78 |

- DistilBERT performed best, especially with abstract/emotive quotes.
- Human quotes scored higher in creativity and emotional balance.
- AI quotes had higher cliché scores and more formulaic language.

---

## Visual Insights

- WordCloud and emotion distribution plots
- t-SNE and UMAP visualizations for clustering and misclassification
- Batch prediction functionality

---

##  Conclusion

QuoteSense effectively classifies emotional tone in quotes while revealing key stylistic differences between human and AI-generated content. This fusion of emotion detection and stylistic scoring opens pathways for deeper human-AI content analysis.

---

## Author

**Hariharan Sriram**  
Senior Research Assistant | NLP & Machine Learning  
University at Buffalo
