# RAG-Enhanced Music Recommendation System

This project implements a novel **Retrieval-Augmented Generation (RAG)** framework to provide context-aware music recommendations. It leverages a vast knowledge base of Pitchfork music reviews to overcome limitations of traditional recommendation systems, offering more nuanced and relevant suggestions.

## Key Features

  * **Hybrid Retrieval:** Combines `BM25` (keyword-based) and `FAISS` (semantic vector search using `all-MiniLM-L6-v2` embeddings) for robust document retrieval.
  * **Contextual Reranking:** A `ms-marco-MiniLM-L-6-v2` cross-encoder re-ranks retrieved review passages, incorporating music-specific boosts (e.g., album score) for improved relevance.
  * **LLM-Powered Generation:** Uses `Mistral-7B-Instruct-v0.2` (4-bit quantized) to synthesize recommendations based on retrieved content and user queries.
  * **LLM-Based Query Expansion:** Expands user queries with synonyms and related terms to enhance retrieval accuracy.
  * **Conversational Interface:** Supports follow-up questions and refined recommendations.

## Architecture

The system operates as a multi-stage RAG pipeline:



## Authors

  * Gautam Krishna M
  * Tanna Rakesh Naidu
  * Surige Sai Yashaswi
  * Subramaniyaswamy Vairavasundaram

*(School of Computer Science and Engineering, Vellore Institute of Technology, Vellore, India)*

## License

This project is open-source. Please refer to the [GitHub repository](https://github.com/gautamk01/RAG_Music_RS) for licensing details.

-----
