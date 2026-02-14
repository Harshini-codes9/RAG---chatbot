# RAG---chatbot
An end-to-end RAG-based document question answering system that retrieves relevant context using vector embeddings and generates grounded responses using an LLM.
This project implements a Retrieval-Augmented Generation (RAG) chatbot that answers user questions strictly from uploaded PDF documents or web content. It prevents hallucinations by grounding responses in retrieved context from a vector database.

---

## 🧠 How It Works

1. Load and chunk PDF
2. Generate embeddings using SentenceTransformers
3. Store embeddings in ChromaDB
4. Retrieve relevant chunks based on user query
5. Generate answer using Flan-T5 (LLM)
6. If answer not found → returns "Not found in the document"

---

## 🛠 Tech Stack

* Python
* ChromaDB (Vector Database)
* SentenceTransformers
* HuggingFace Transformers (Flan-T5)
* LangChain (optional for chunking)

---

## 📂 Project Structure

```
rag-chatbot/
│
├── data/
├── chroma_db/
├── main.py
├── requirements.txt
└── README.md
```

---

## 📌 Features

* PDF-based knowledge grounding
* Semantic search using embeddings
* Controlled LLM responses
* Minimal hallucination
* Modular architecture

---

## 🎯 Use Cases

* College syllabus chatbot
* Legal document QA assistant
* Research paper assistant
* Company internal knowledge bot

---

## ⚡ Future Improvements

* Add chat history memory
* Streamlit UI
* Multi-document support
* Deployment via FastAPI
* Support for open-source LLMs (LLaMA, Mistral)

---



