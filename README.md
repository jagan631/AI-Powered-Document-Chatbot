# 🤖 AI-Powered Document Chatbot (RAG)

> **Chat with your PDF documents using Retrieval-Augmented Generation (RAG), LangChain, ChromaDB, and Qwen 2.5 3B.**

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge\&logo=python)
![LangChain](https://img.shields.io/badge/LangChain-RAG-green?style=for-the-badge)
![ChromaDB](https://img.shields.io/badge/VectorDB-ChromaDB-orange?style=for-the-badge)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow?style=for-the-badge\&logo=huggingface)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge\&logo=googlecolab)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

---

## 📖 Overview

This project is an **AI-powered Document Question Answering System** built using **Retrieval-Augmented Generation (RAG)**.

Instead of relying only on an LLM's pre-trained knowledge, the application retrieves the most relevant content from uploaded PDF documents and uses it to generate accurate, context-aware responses.

The project demonstrates the complete RAG pipeline using **LangChain**, **BGE-M3 embeddings**, **ChromaDB**, and the **Qwen 2.5 3B Instruct** language model.

---

## ✨ Features

* 📄 Upload and process PDF documents
* ✂️ Intelligent document chunking
* 🧠 Semantic embeddings with BGE-M3
* 🗂️ Vector storage using ChromaDB
* 🔍 Semantic similarity search
* 🤖 Context-aware answer generation
* ⚡ Built with LangChain
* ☁️ Runs entirely on Google Colab
* 💬 Reduces hallucinations by grounding answers in document content

---

## 🛠️ Tech Stack

| Category             | Technology                     |
| -------------------- | ------------------------------ |
| Language             | Python                         |
| Framework            | LangChain                      |
| PDF Loader           | PyMuPDFLoader                  |
| Text Splitter        | RecursiveCharacterTextSplitter |
| Embedding Model      | BAAI BGE-M3                    |
| Vector Database      | ChromaDB                       |
| Large Language Model | Qwen 2.5 3B Instruct           |
| Environment          | Google Colab                   |
| ML Library           | Hugging Face Transformers      |

---

## 🏗️ Architecture

```text
                PDF
                 │
                 ▼
        PyMuPDFLoader
                 │
                 ▼
 RecursiveCharacterTextSplitter
                 │
                 ▼
           Text Chunks
                 │
                 ▼
      BGE-M3 Embeddings
                 │
                 ▼
            ChromaDB
                 │
                 ▼
      Semantic Retrieval
                 │
                 ▼
        Prompt Template
                 │
                 ▼
     Qwen 2.5 3B Instruct
                 │
                 ▼
         Generated Answer
```

---

## 🚀 Workflow

1. Upload a PDF document.
2. Extract text using **PyMuPDFLoader**.
3. Split the document into overlapping chunks.
4. Generate semantic embeddings using **BGE-M3**.
5. Store embeddings in **ChromaDB**.
6. Retrieve the most relevant chunks based on the user's query.
7. Pass the retrieved context to **Qwen 2.5 3B Instruct**.
8. Generate an accurate, context-aware response.

---

## 📂 Project Structure

```text
AI-Powered-Document-Chatbot/
│
├── data/
│   └── sample.pdf
│
├── notebooks/
│   └── RAG_Document_Chatbot.ipynb
│
├── chroma_db/
│
├── README.md
│
├── requirements.txt
│
└── assets/
```

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/AI-Powered-Document-Chatbot.git

cd AI-Powered-Document-Chatbot
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or run directly in **Google Colab**.

---

## 📦 Required Libraries

```text
langchain
langchain-community
langchain-core
langchain-chroma
langchain-huggingface
chromadb
sentence-transformers
transformers
accelerate
pymupdf
```

---

## 💻 Example Usage

```python
question = "What is Artificial Intelligence?" // Based on the uploaded PDF

answer = rag_chain.invoke(question)

print(answer)
```

---

## 📸 Sample Output

```text
Question:
What is Artificial Intelligence? // Question based on the uploaded document

Answer:
Response
```

---

## 🎯 Learning Outcomes

This project demonstrates practical knowledge of:

* Retrieval-Augmented Generation (RAG)
* Large Language Models (LLMs)
* Prompt Engineering
* Semantic Search
* Vector Databases
* Embedding Models
* LangChain Pipelines
* Hugging Face Transformers
* Document Processing
* Google Colab Development

---

## 🔮 Future Improvements

* Multi-PDF support
* Conversational memory
* Hybrid Search (BM25 + Vector Search)
* Reranking using Cross-Encoders
* Streamlit Web Interface
* FastAPI Backend
* Docker Deployment
* Authentication
* Cloud Deployment
* Source citation with page numbers

---

## 🤝 Contributing

Contributions, suggestions, and feature requests are welcome.

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Open a Pull Request

---


## 👨‍💻 Author

**Jagan A**

* MCA Student
* Java & Full Stack Developer
* AI & Generative AI Enthusiast

If you found this project helpful, consider giving it a ⭐ on GitHub!
