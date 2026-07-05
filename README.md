# 📚 ResearchRAG – AI-Powered Research Paper Assistant

ResearchRAG is my **first Retrieval-Augmented Generation (RAG)** project built using **LangChain**, **ChromaDB**, and modern Large Language Models. It enables users to ask natural-language questions about research papers and receive context-aware answers via semantic retrieval and LLM-powered generation.

The project currently uses **Google Gemini 2.5 Flash** and **Qwen/Qwen3-32B** for answer generation, while **all-MiniLM-L6-v2** is used to generate embeddings, which are stored in **ChromaDB** for efficient semantic search.

This implementation demonstrates the complete RAG workflow, including document ingestion, text chunking, embedding generation, vector search, prompt construction, and answer generation.


## 🚀 Features

* 📄 Chat with research papers using natural language
* 🔍 Semantic search with vector embeddings
* 🧠 Retrieval-Augmented Generation (RAG)
* 📚 Context-aware question answering
* ⚡ Fast document retrieval using ChromaDB
* 🤖 LLM-powered responses
* 📝 Clean and modular LangChain implementation

---

## 📂 Research Papers Used

This project currently indexes and answers questions from the following research papers:

1. **Attention Is All You Need**
2. **Retrieval-Augmented Generation (RAG) Research Paper**

---

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **ChromaDB** (Vector Database)
* **Sentence Transformers**

  * `all-MiniLM-L6-v2`
* **PyMuPDFLoader**
* **RecursiveCharacterTextSplitter**
* **Large Language Models (LLMs)**

  * **Google Gemini 2.5 Flash**
  * **Qwen/Qwen3-32B**
* **Jupyter Notebook**


## 🏗️ RAG Pipeline

```text
Research Papers (PDF)
        │
        ▼
PyMuPDFLoader
        │
        ▼
Text Chunking
(RecursiveCharacterTextSplitter)
        │
        ▼
Embedding Generation
(all-MiniLM-L6-v2)
        │
        ▼
ChromaDB Vector Store
        │
        ▼
Retriever
        │
        ▼
Google Gemini 2.5 Flash
        │
        ▼
Context-Aware Answer
```

---

## 📁 Project Structure

```text
ResearchRAG/
│── data/
│   ├── attention_is_all_you_need.pdf
│   └── rag_research_paper.pdf
│
├── chroma_db/
├── notebook.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/research-rag.git
cd research-rag
```

### Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Add your API key

Create a `.env` file:

```text
GOOGLE_API_KEY=YOUR_API_KEY
```

---

## 💬 Example Questions

* What is Retrieval-Augmented Generation?
* Explain the Transformer architecture.
* What is self-attention?
* What are the limitations of RAG?
* How does the encoder differ from the decoder?
* Why was the Transformer introduced?

---

## 📌 Future Improvements

* Support multiple PDF uploads
* Source citations with page numbers
* Conversational memory
* Hybrid search
* Web interface using Streamlit
* Response streaming
* Support for local LLMs using Ollama

---

## 🎯 Learning Outcome

This project helped me understand:

* Retrieval-Augmented Generation (RAG)
* Semantic Search
* Vector Databases
* Embedding Models
* LangChain Workflows
* Prompt Engineering
* Research Paper Question Answering

---

## 🤝 Contributing

Contributions, suggestions, and feedback are always welcome.

If you find this project useful, consider giving it a ⭐ on GitHub.

---

## 📄 License

This project is licensed under the MIT License.
