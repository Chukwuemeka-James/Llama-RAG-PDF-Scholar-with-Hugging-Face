Here's a comprehensive `README.md` file for your Streamlit app using Groq, HuggingFace, and LangChain:

---

# Llama-RAG PDF Scholar with Hugging Face

**Llama-RAG PDF Scholar** is an AI-powered tool designed for efficient document-based question answering. This project leverages **LangChain**, **Groq API**, and **Hugging Face Embeddings** to enable interactive querying over research papers in PDF format. By embedding and indexing research papers, the app allows users to ask questions and receive context-based answers from the ingested documents.

## Features

- **Document Embedding:** Index and create vector embeddings from research papers in PDF format.
- **Query & Answer:** Input queries, and the app retrieves the most relevant sections from the documents using Retrieval-Augmented Generation (RAG).
- **Custom LLM:** Powered by Groq API's `Llama3-8b-8192` model to generate accurate, context-based answers.
- **Hugging Face Embeddings:** Efficient document vectorization using Hugging Face's `all-MiniLM-L6-v2` model.
- **Document Similarity Search:** Displays document sections most relevant to the input query.

## How It Works

1. **Document Embedding:**
   - Uploads and loads PDFs from the `research_papers` directory.
   - Splits documents into smaller chunks for more efficient vector embeddings.
   - Creates a vector database using **FAISS** for fast document retrieval.

2. **Query Input:**
   - Users input a query into the text box. The query is processed through the **Llama3** model to generate responses.
   - Retrieves the most relevant documents from the vector store to generate the best context-based answers.

3. **Document Similarity Search:**
   - View relevant document sections that contribute to the final answer via a document similarity search feature.
