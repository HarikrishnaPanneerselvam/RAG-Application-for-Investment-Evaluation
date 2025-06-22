# 💼 RAG Application for Investment Pitch Deck Evaluation

A Retrieval-Augmented Generation (RAG)-based application that enables investors to upload pitch decks (PDFs), extract valuable insights, and ask context-aware questions to support data-driven investment decisions.

---

## 📌 Problem Statement

**Objective:**  
Develop a RAG-based system that:

- ✅ Allows investors to upload a pitch deck in PDF format.
- 🔍 Extracts key business information from the document.
- 💬 Answers investor-relevant questions using context from the pitch deck.

---

## 🎯 Features

- 📁 Upload PDF pitch deck via UI or script
- 📄 Extracts slide-level content using **PyMuPDF**
- ✂️ Splits text into meaningful chunks
- 🧠 Converts chunks into embeddings using **SentenceTransformers**
- 💾 Stores embeddings in **FAISS** for fast retrieval
- 💬 Enables question answering with **LangChain + Transformers**
- 📊 Responds with:
  - Reasonable investment amount & equity range
  - Key risk factors from the deck
  - 5+ useful insights for investors

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| **PyMuPDF (`fitz`)** | Extract text from PDF |
| **FAISS** | Vector store for semantic search |
| **LangChain** | Manages retrieval and LLM-based responses |
| **Sentence-Transformers** | Generates text embeddings |
| **HuggingFace Transformers** | Handles natural language generation and QA |

---

## 🚀 Installation

Run the following commands in your environment:

```bash
pip install pymupdf
pip install faiss-cpu
pip install langchain
pip install sentence-transformers
pip install transformers
