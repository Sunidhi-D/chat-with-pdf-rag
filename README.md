<div align="center">

# 📚✨ Chat With Your PDFs — RAG Based AI App  
### Built with Streamlit • LangChain • FAISS • MiniLM • Google Gemini

<br>

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![LangChain](https://img.shields.io/badge/LangChain-RAG-green)
![FAISS](https://img.shields.io/badge/FAISS-VectorDB-purple)
![Gemini](https://img.shields.io/badge/Gemini-LLM-blue)

<br>

### 🚀 Interact with your PDF documents using an AI-powered RAG pipeline.

Upload PDFs → Extract text → Create embeddings → Retrieve context →  
**Ask questions and get accurate answers based only on the PDF content!**

</div>

---

## 🌟 Features

✨ Upload multiple PDFs  
✨ Automatic text extraction  
✨ Intelligent text chunking  
✨ Embeddings with **MiniLM-L6-v2**  
✨ Vector search using **FAISS**  
✨ Accurate Q&A using **Google Gemini**  
✨ Clean, chat-style Streamlit UI  
✨ Download conversation history as CSV  

---

## 🧠 Tech Stack

| Layer | Technology |
|-------|------------|
| LLM | Google Gemini |
| Framework | Streamlit + LangChain |
| Embeddings | Sentence Transformers (MiniLM-L6-v2) |
| Vector DB | FAISS |
| PDF Parsing | PyPDF |
| Language | Python |

---

## 📁 Project Structure

pdf-chat-rag-app/
│
├── app.py               # Streamlit UI  
├── rag_model.py         # RAG logic  
│
├── assets/
│   └── screenshot.png   # Add your app screenshot here
│
├── sample_pdfs/         # Optional demo PDFs
│
├── requirements.txt
└── README.md

---
## CLONE THE REPOSITORY

steps:
  - step: "Clone the repository"
    command: |
      git clone https://github.com/yourusername/yourrepo.git
      cd yourrepo

  - step: "Install dependencies"
    command: |
      pip install -r requirements.txt

  - step: "Add your Google API key"
    create_file: ".env"
    content: |
      GOOGLE_API_KEY=your_api_key_here

  - step: "Run the Streamlit app"
    command: |
      streamlit run app.py

---
## 🟩 HOW THE RAG PIPELINE WORKS
---


(But without spaces — GitHub needs exact ticks.)

---

# ⭐ **Copy–Paste THIS — It will render perfectly!**

```yml
rag_pipeline:
  description: "Retrieval Augmented Generation (RAG) workflow for PDF-based Q&A"

  steps:
    - "✨ Extract text from uploaded PDFs using PyPDF"
    - "✨ Split extracted text into overlapping semantic chunks"
    - "✨ Generate embeddings using Sentence Transformers (MiniLM-L6-v2)"
    - "✨ Store embeddings in FAISS vector database"
    - "✨ For each question:"
      - "🔹 Retrieve top-k most relevant chunks"
      - "🔹 Send retrieved context + question to Gemini LLM"
      - "🔹 Gemini answers ONLY using the retrieved PDF context"

  flow_diagram:
    upload_pdfs: "📂 User uploads PDF files"
    extract_text: "📝 Raw text extracted"
    split_chunks: "✂️ Recursive text splitting"
    embed_chunks: "🧠 MiniLM embeddings created"
    vector_store: "📦 FAISS stores vector representations"
    ask_question: "❓ User asks a question"
    retrieve_context: "🔍 Most relevant chunks returned"
    llm_response: "🤖 Gemini generates grounded answer"
