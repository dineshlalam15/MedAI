# 📌 RAG-Powered Document Chatbot using LangChain & OpenAI

## 📝 Description:
- This project implements a Retrieval-Augmented Generation (RAG) pipeline that allows users to upload documents (PDFs, text, or other formats) and interact with them via a conversational interface. It uses LangChain for orchestration, FAISS for vector storage, and OpenAI GPT models for natural language understanding.

## ⚡ Features:
- 📂 Document Ingestion: Upload and process multiple documents into embeddings.
- 🔍 Efficient Retrieval: Uses FAISS vector store for semantic search.
- 💬 Conversational Q&A: Ask context-aware questions based on your documents.
- ⚙ Customizable Pipelines: Easily swap out models, embeddings, or vector DBs.
- 🐍 Python Based: Simple to run locally or deploy to the cloud.

## 🛠️ Tech Stack:
- Python 3.10+
- LangChain
- OpenAI GPT API
- FAISS Vector Store
- PyPDF2 / Unstructured / Chroma (optional)

## 🗂 Project Structure
```
📦 MedAI
 ┣ 📂 app
 ┃ ┣ 📜 __init__.py
 ┃ ┣ ⚙ config.py         # Reads environment variables
 ┃ ┣ 📄 ingestion.py     # Document ingestion & preprocessing
 ┃ ┣ 🤖 embeddings.py    # Embedding generation
 ┃ ┣ 📦 vectorstore.py   # FAISS vector DB operations
 ┃ ┣ 🔍 retrieval.py     # Document retrieval logic
 ┃ ┣ 🧠 llm.py           # LLM interaction
 ┃ ┗ 🎨 ui.py            # Streamlit/Flask frontend
 ┣ 📂 data               # Raw & processed files
 ┣ 📂 tests              # Unit tests
 ┣ 📂 prompts            # Prompt templates
 ┃ ┣ retrieval_prompts.ini
 ┃ ┣ summarization_prompts.ini
 ┃ ┣ classification_prompts.ini
 ┃ ┗ system_prompts.ini
 ┣ 📜 requirements.txt
 ┣ 📜 Pipfile
 ┣ 📜 README.md
 ┣ ⚙ .env
 ┣ ⚙ .env.example
 ┗ 📜 .gitignore
```
