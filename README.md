📌 RAG-Powered Document Chatbot using LangChain & OpenAI

📝 Description:
- This project implements a Retrieval-Augmented Generation (RAG) pipeline that allows users to upload documents (PDFs, text, or other formats) and interact with them via a conversational interface. It uses LangChain for orchestration, FAISS for vector storage, and OpenAI GPT models for natural language understanding.

⚡ Features:
- 📂 Document Ingestion: Upload and process multiple documents into embeddings.
- 🔍 Efficient Retrieval: Uses FAISS vector store for semantic search.
- 💬 Conversational Q&A: Ask context-aware questions based on your documents.
- ⚙ Customizable Pipelines: Easily swap out models, embeddings, or vector DBs.
- 🐍 Python Based: Simple to run locally or deploy to the cloud.

🛠️ Tech Stack:
- Python 3.10+
- LangChain
- OpenAI GPT API
- FAISS Vector Store
- PyPDF2 / Unstructured / Chroma (optional)

🏢 Code Architecture:
MedAI/
│
├── app/                        # Main application code
│   ├── __init__.py
│   ├── config.py              # Reads from .env
│   ├── ingestion.py           # Fetch + preprocess medical data
│   ├── embeddings.py          # Generate embeddings
│   ├── vectorstore.py         # Store/retrieve embeddings
│   ├── retrieval.py           # Query + retrieve passages
│   ├── llm.py                 # LLM query & synthesis
│   ├── ui.py                  # Streamlit/Flask UI
│
├── data/                      # Raw and processed data
│
├── tests/                     # Unit tests
│
├── prompts/
│   ├── retrieval_prompts.ini
│   ├── summarization_prompts.ini
│   ├── classification_prompts.ini
│   └── system_prompts.ini
|
├── requirements.txt
├── Pipfile
├── Pipfile.lock
├── README.md
├── .env
├── .env.example
└── .gitignore