.

🤖 LangChain Learning Project

This repository documents my hands-on learning of LangChain, focusing on building LLM-powered applications using core components like models, prompts, chains, embeddings, vector databases, and agents.

🚀 What is LangChain?

LangChain is a framework for building applications powered by Large Language Models (LLMs). It helps structure workflows like chatbots, RAG pipelines, and intelligent agents.

🧠 Core Terminologies
🔹 Models

LLMs like OpenAI GPT models that generate responses.

Used for: text generation, chat, reasoning
Example: OpenAI Chat Models
🔹 Prompts

Instructions or input given to the model.

Define behavior of LLM
Can include system + user messages
🔹 Chains

A sequence of operations where output of one step becomes input to the next.

Example: Prompt → Model → Output
Used to build structured workflows
🔹 Embeddings

Numerical representations of text.

Convert text into vectors
Used for similarity search
🔹 Vector Store

Database that stores embeddings.

Enables fast similarity search
Example: Pinecone
🔹 Agents

Advanced systems that decide what action to take next.

Can use tools (search, APIs, DB)
More dynamic than chains
⚙️ Project Workflow

This project follows a step-by-step pipeline to build a basic LLM + RAG system.

1️⃣ Requirements

Install dependencies:

pip install langchain openai pinecone-client
2️⃣ APIs Setup

Get API keys from:

OpenAI (for LLM + embeddings)
Pinecone (for vector database)

Set environment variables:

OPENAI_API_KEY=your_key
PINECONE_API_KEY=your_key
3️⃣ Initialize Message Schema

LangChain uses structured messages:

System Message → defines behavior
Human Message → user input
AI Message → model response
4️⃣ Open Chat Model

Initialize chat model:

Load OpenAI model
Start conversation pipeline
5️⃣ Create Chains

Build workflows using chains:

Prompt → Model → Output
Combine multiple steps
6️⃣ Chunking + Embeddings + Storage
Divide large text into smaller chunks
Generate embeddings
Store in vector database (Pinecone)
7️⃣ Similarity Search
Convert query into embedding
Search similar chunks in vector DB
Retrieve relevant information
🔄 End-to-End Flow
User Query
   ↓
Convert to Embedding
   ↓
Search Vector DB (Pinecone)
   ↓
Retrieve Relevant Chunks
   ↓
Send to LLM (OpenAI)
   ↓
Generate Response
📂 Project Files
langchain/
│
├── langchain-13-min.ipynb   # Core learning notebook
├── requirements.txt         # Dependencies
├── .gitignore
🎯 Key Learnings
Understanding LLM pipelines
Building chains and workflows
Using embeddings for semantic search
Working with vector databases
Designing RAG (Retrieval-Augmented Generation) systems
🔮 Future Improvements
Add Agents with tools
Implement full RAG pipeline
Add UI (Streamlit / FastAPI)
Add memory for chat history
👩‍💻 Author

Yogita Gupta
