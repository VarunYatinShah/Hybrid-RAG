# 🔍 Hybrid Search RAG (Retrieval-Augmented Generation)

**Hybrid Search RAG** is a Retrieval-Augmented Generation system that enhances large language model (LLM) responses by combining **semantic (vector-based)** and **keyword (BM25)** search techniques.  
This hybrid approach ensures both contextual understanding and precise keyword matching for more accurate and relevant information retrieval.

---

## 🧠 Overview

Traditional retrieval methods often struggle to balance **semantic relevance** and **exact keyword matching**.  
This project implements a **hybrid retrieval strategy** that merges the strengths of both approaches:

- **BM25** for lexical matching  
- **Vector Search** for semantic similarity  
- **Weighted Fusion** for final ranking of retrieved documents  

The retrieved results are then used to **augment an LLM**, grounding its responses in factual and contextually relevant data.

---

## 🚀 Features

- 🧩 **Hybrid Retrieval:** Combine BM25 and vector-based search for improved accuracy  
- 🤖 **RAG Integration:** Feed retrieved context into a large language model  
- ⚡ **Modular Components:** Plug-and-play retrievers, embeddings, and LLMs    
- ☁️ **Extensible:** Works with local embeddings or cloud-based vector databases  

---

## 🏗️ Architecture

```text
User Query
   │
   ├──► BM25 Retriever ──┐
   │                     ├──► Hybrid Fusion ──► Context Builder ──► LLM (RAG)
   └──► Vector Retriever ─┘
