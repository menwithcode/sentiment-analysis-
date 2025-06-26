# 🤖 Emotion Classification with Self-Healing LangGraph DAG

This project fine-tunes a DistilBERT-based emotion classifier on a multi-label emotion dataset and builds a self-healing pipeline using LangGraph. If the primary model fails (low confidence), it switches to a zero-shot fallback model and retrains dynamically when enough uncertain data is collected.

---

## 🚀 How to Run in Google Colab

### 1. 📥 Upload Dataset

Upload the following files into the `/content/` directory in Colab:

- `train.tsv`
- `dev.tsv`
- `test.tsv`

Each file should follow this format:

