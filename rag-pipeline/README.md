# RAG Pipeline

Recreate the Retrieval-Augmented Generation (RAG) setup: ingest documents, chunk
and embed them, store the vectors, and answer questions by retrieving relevant
context before calling an LLM.

## Goals
- Ingest a folder of documents (text, markdown, PDF) and split them into chunks.
- Generate embeddings for each chunk and store them in a vector database.
- Given a user query, retrieve the top-k most relevant chunks.
- Combine the retrieved context with the query in a prompt sent to an LLM.
- Return an answer that cites which chunks/sources were used.

## Possible Tech Stack
- **Chunking/orchestration**: Python, LangChain or LlamaIndex
- **Embeddings**: OpenAI, Sentence-Transformers, or a local embedding model
- **Vector store**: Chroma, FAISS, Pinecone, or Weaviate
- **LLM**: OpenAI GPT, local model via Ollama, or another provider

## Getting Started
- [ ] Pick document sources to ingest for a first test run
- [ ] Choose a chunking strategy (fixed size, sentence, or semantic)
- [ ] Choose an embedding model and vector store
- [ ] Build the ingestion script (`ingest.py`)
- [ ] Build the query/answer script (`query.py`)
- [ ] Add example documents and a sample query for a smoke test
