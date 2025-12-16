# LEXICON – Semantic Search Engine

LEXICON is a **semantic search engine** that retrieves relevant text passages using **word embeddings and transformer-based re-ranking**. It demonstrates how modern information retrieval systems combine **efficient vector search** with **deep semantic understanding** to improve search quality.

---

## 🚀 What This Project Does

- Builds a search engine over **100,000 MS MARCO passages**
- Supports **semantic search**, not just keyword matching
- Uses a **two-stage retrieval pipeline**:
  1. Fast candidate retrieval using Word2Vec embeddings
  2. Accurate re-ranking using BERT or BM25
- Provides an **interactive Streamlit demo**

---

## 🧠 Key Techniques Used

- **Word2Vec embeddings** for dense semantic representation  
- **FAISS** for high-performance vector similarity search  
- **Sentence-BERT (MiniLM)** for transformer-based re-ranking  
- **BM25** for lexical re-ranking comparison  
- **Evaluation with standard IR metrics** (MRR, Recall, NDCG)

---

## 📊 Results (Highlights)

- **Best model:** Word2Vec + BERT re-ranking  
- Improved ranking quality compared to pure embedding search  
- Demonstrates real-world **recall vs. accuracy tradeoffs**

| Model | MRR@10 | Recall@10 |
|------|--------|-----------|
| Word2Vec | 0.157 | 0.450 |
| Word2Vec + BERT | **0.198** | **0.525** |
| Word2Vec + BM25 | 0.170 | 0.478 |

---

## 🛠️ Tech Stack

- **Python**
- **Gensim** – Word2Vec
- **FAISS** – vector search
- **Hugging Face Transformers / Sentence-Transformers**
- **NLTK** – text preprocessing
- **scikit-learn** – clustering & analysis
- **Streamlit** – UI demo

---

## 📁 Project Structure

```text
.
├── notebooks/        # Experiments and evaluation
├── src/              # Retrieval and re-ranking logic
├── app/              # Streamlit demo
├── results/          # Metrics and visualizations
└── README.md








├── results/          # Metrics and visualizations
└── README.md
