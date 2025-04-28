# 🏡 Tenancy Agreement RAG Chatbot

This project builds a simple RAG chatbot to answer questions about tenancy agreements. It can help a real estate agent to answer questions about their tenants or rental properties quickly.

## Tools
- LangChain for RAG
- Chroma for vector storage
- FlashRank for reranking
- OpenAI GPT-4o-mini as the LLM

## Files

- `create_vector_db.ipynb` — Create and store tenancy agreement chunks into Chroma vectorstore.
- `tenancy_rag_pipeline.ipynb` — Load vectorstore, rewrite query with an LLM, retrieve relevant chunks, rerank, and generate answers with GPT-4o-mini.  
  It also provides a list of testing questions that a real estate agent may ask.
- `requirements.txt`

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
2. Create a `.env` file in the project root to store your `OPENAI_API_KEY` 

## On going
This is a demo project that I will carry on building. What I am thinking now is:
1. Try paragraph chunking or section chunking
2. Add a UI with Streamlit
3. Try to better handle the "how-many" type of questions
