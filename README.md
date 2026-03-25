#  DocuQuery-AI: Multi-PDF RAG Assistant

**DocuQuery-AI** A high-performance RAG-based AI chatbot built with LangChain, FAISS, and Google Gemini 2.5 Flash to chat with multiple PDF documents in real-time

---

##  Key Features

* **Multi-Document Analysis**: Upload and query multiple PDF files simultaneously.
* **Contextual Accuracy**: Uses semantic search to ensure answers are grounded in your data.
* **Scalable Vector Search**: Powered by FAISS (Facebook AI Similarity Search) for millisecond retrieval.
* **Modern UI**: A clean, intuitive interface built with Streamlit.

##  Technical Architecture

1.  **Ingestion**: PDFs are parsed using `PyPDF2`.
2.  **Chunking**: Text is split into segments using `RecursiveCharacterTextSplitter`.
3.  **Embeddings**: Text chunks are converted into vectors using `models/gemini-embedding-001`.
4.  **Vector Store**: Store indexed in a local `FAISS` database.
5.  **LLM**: `Gemini 2.5 Flash` generates detailed responses based on retrieved context.

---

