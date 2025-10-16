# RAG Q&A Bot

## Project Overview
A Retrieval-Augmented Generation (RAG) bot for advanced question-answering over documents.  
This system uses LangChain, local embeddings, and Groq LLM to let users upload a PDF and interactively query its contents with accurate, context-aware answers.

## Data & Tech Stack
- **Input:** Any local PDF file
- **Key Libraries:** LangChain, HuggingFace Embeddings, ChromaDB, Groq LLM, PyPDFLoader
- **Core Feature:** Combines document retrieval (vector search) with GenAI Q&A

## Workflow

1. **Environment Setup**
    - Installs all dependencies for document processing, embeddings, and answer generation

2. **Data Loading**
    - Loads the PDF and splits text into overlapping chunks for retrieval

3. **Embedding & Indexing**
    - Embeds all document chunks using HuggingFace transformers
    - Stores vectors in ChromaDB for fast similarity search

4. **LLM Integration**
    - Uses Groq Llama-3 model to provide natural, reliable answers (with temperature control for factuality)

5. **Query Engine**
    - On any user question, retrieves relevant chunks and generates answers
    - Includes conversational memory for multi-turn Q&A
    - Returns “I do not know” when the answer isn't present—no hallucinations

## Results

- **Handles any PDF with instant, context-rich answers**
- **Conversational memory lets users build on previous queries**
- **Accurate, safe responses with plug-and-play LLM integration**

***

*This project showcases RAG for robust document Q&A—ideal for resumes, reports, or technical PDFs. A hands-on demo of the future of natural language search!*

