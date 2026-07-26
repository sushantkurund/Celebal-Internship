# Document Question Answering System using RAG

## Overview

This project implements a Retrieval-Augmented Generation (RAG) based Document Question Answering System using LangChain, FAISS, Hugging Face embeddings, and Google's Gemini model. The system retrieves relevant information from a custom PDF document and generates accurate answers based on the retrieved context instead of relying only on the language model's internal knowledge.

The project demonstrates the complete RAG workflow, including document loading, text chunking, embedding generation, vector storage, retrieval, and response generation.

---

## Objectives

- Build a Retrieval-Augmented Generation (RAG) pipeline.
- Load and process a custom PDF document.
- Generate semantic embeddings for document chunks.
- Store embeddings using FAISS for efficient similarity search.
- Retrieve relevant document sections based on user queries.
- Generate context-aware answers using Gemini.
- Validate the system with multiple sample questions.

---

## Technologies Used

- Python
- Google Colab
- LangChain
- Hugging Face Embeddings
- FAISS Vector Store
- Google Gemini API
- PyPDF
- Sentence Transformers

---

## Workflow

1. Install and import the required libraries.
2. Load the PDF document.
3. Split the document into smaller text chunks.
4. Generate embeddings for each chunk.
5. Store embeddings in a FAISS vector database.
6. Create a retriever for similarity search.
7. Connect the retriever with the Gemini language model.
8. Accept user queries.
9. Retrieve relevant document chunks.
10. Generate answers using the retrieved context.
11. Validate the RAG system using multiple test questions.

---

## Features

- Supports custom PDF documents.
- Semantic document retrieval using embeddings.
- Fast similarity search with FAISS.
- Context-aware answer generation.
- Displays retrieved context for validation.
- Easy to modify for different documents.

---

## Sample Validation Questions

- What programming languages does the candidate know?
- What projects has the candidate completed?
- What is the candidate's MCA specialization?
- What is the candidate's UG CGPA?
- Which frameworks and tools does the candidate know?
- What is the candidate's email address?

---

## Results

The RAG system successfully retrieves relevant document chunks and generates answers based on the retrieved information. Validation results demonstrate that the generated responses are grounded in the document content, reducing hallucinations and improving factual accuracy.

---

## Conclusion

This project demonstrates the implementation of a complete Retrieval-Augmented Generation (RAG) pipeline for document question answering. By combining document retrieval with a large language model, the system provides accurate and context-aware responses from custom documents. The project also highlights the importance of embeddings, vector databases, and retrieval in building reliable AI-powered document assistants.
