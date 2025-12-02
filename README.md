# MY_FIRST_RAG_OPENAI_LANGCHAIN

This project demonstrates building a simple Retrieval-Augmented Generation (RAG) workflow with OpenAI and LangChain in a Jupyter Notebook.

## What You’ll Learn

- **Environment Setup**: How to configure Python and API keys for OpenAI with `.env` and `python-dotenv`.
- **OpenAI Integration**: How to connect to OpenAI models for both text generation and embeddings.
- **Prompt Engineering**: Using LangChain to create and format custom prompts for LLMs.
- **Semantic Search**: How to create and compare vector embeddings using scikit-learn’s `cosine_similarity`.
- **Vector Database with FAISS**: Store and retrieve embeddings with FAISS for fast similarity search.
- **RAG Workflow**: Combine document loading, chunking, embedding, retrieval, and LLM querying using LangChain.

## How It Works

1. **Install Dependencies**  
   Run notebook cells to install:  
   - `openai`  
   - `langchain-community`, `langchain`, `langchain_openai`  
   - `faiss-cpu`  
   - `python-dotenv`  
   - `scikit-learn`  
   - `pandas`

2. **Set Up API Keys**  
   - Place your OpenAI key in a `.env` file or enter directly in the notebook.

3. **Document Loading and Embedding**  
   - Read your CSV file with pandas.  
   - Convert data to LangChain documents.  
   - Split text with LangChain’s text splitters.  
   - Generate embeddings with OpenAI API.

4. **Store Embeddings in FAISS Vector DB**  
   - Store document embeddings for fast similarity search.  
   - Inspect total vectors stored.

5. **Prompt Engineering with LangChain**  
   - Create custom templates for asking questions.  
   - Use LangChain to send these prompts to OpenAI.

6. **RAG Chain**  
   - Retrieve relevant information from your data (with FAISS).  
   - Pass context and questions to the LLM.  
   - Format answers based on your requirements (e.g., structured output for employee database queries).

## Example Use Cases

- Ask questions about your own CSV data using natural language.
- Find similar entries based on embeddings.
- Retrieve structured answers (e.g., employee details) using RAG and LLMs.

## Quick Start

- Clone the repo.
- Add your `user.csv` file.
- Add your OpenAI key to `.env`.
- Open and run `MyRAG_OpenAI_LangChain.ipynb` in Jupyter.

---

This notebook gives you a clear, practical template for applying RAG and LangChain to your own projects!