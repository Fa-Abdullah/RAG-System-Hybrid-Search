# RAG System – Intelligent Question Answering from PDF Documents

A Retrieval-Augmented Generation (RAG) system that enables users to ask questions directly from PDF documents and receive accurate, context-aware answers. The project combines semantic search, keyword retrieval, reranking, and Large Language Models to improve response quality and reduce hallucinations.

## Overview

Finding information inside lengthy documents can be time-consuming and inefficient. This project addresses that challenge by transforming PDF files into a searchable knowledge base and allowing users to interact with their documents through natural language questions.

The system retrieves the most relevant document sections using a hybrid search strategy, reranks them to maximize relevance, and then generates answers grounded entirely in the retrieved content.

## Key Features

* Automated PDF text extraction and cleaning
* Intelligent document chunking with overlap preservation
* Semantic search using vector embeddings
* Keyword-based retrieval with BM25
* Hybrid retrieval for improved search accuracy
* Cross-encoder reranking for better relevance scoring
* Context-aware answer generation using LLMs
* Interactive chat interface powered by Gradio
* Reduced hallucinations through retrieval-grounded responses

## System Workflow

1. Upload one or more PDF documents
2. Extract and clean document text
3. Split content into meaningful chunks
4. Generate embeddings and store them in ChromaDB
5. Submit a natural language question
6. Retrieve relevant chunks using hybrid search
7. Rerank retrieved results using a Cross-Encoder model
8. Generate a final answer based solely on the retrieved context

## Technologies Used

* Python
* ChromaDB
* LangChain
* BM25 Retrieval
* Cross-Encoder Reranking
* OpenRouter API
* LLaMA 3.1 8B Instruct
* Gradio
* Hugging Face Embeddings
* RecursiveCharacterTextSplitter

## Technical Highlights

* **Embedding Model:** intfloat/multilingual-e5-large
* **Vector Database:** ChromaDB
* **Reranking Model:** ms-marco-MiniLM-L-6-v2
* **LLM Provider:** OpenRouter
* **Language Model:** LLaMA 3.1 8B Instruct

## Potential Applications

* Research paper exploration
* Academic document analysis
* Enterprise knowledge management
* Legal and policy document search
* Internal company documentation assistants
* Educational learning assistants



