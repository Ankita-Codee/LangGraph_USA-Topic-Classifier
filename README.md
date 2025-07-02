# 🇺🇸 LangGraph_USA-Topic-Classifier

## 🧠 Project Summary
This project demonstrates how to build a LangGraph-based intelligent routing system that classifies user questions and dynamically selects the appropriate response strategy.

🔍 Core Idea
- A supervisor node powered by an LLM (Gemini Flash) classifies each incoming user query into one of two categories:
- USA — questions specifically related to the United States (e.g., economy, GDP, industrial growth)
- Not Related — general questions not specific to the USA
- The classification is parsed using a PydanticOutputParser to ensure the output is structured and reliable.

---
## 🔀 Routing Logic
Based on the classification:
- ✅ If the topic is "USA", the system uses a RAG (Retrieval-Augmented Generation) pipeline to search over embedded documents and return a relevant answer.
- 🤖 If the topic is "Not Related", a general LLM node answers using world knowledge.

---
## 📦 Components
- Supervisor Node — Classifies the topic using LLM + Pydantic parsing
- Router Function — Directs the query to RAG or LLM based on classification
- RAG Node — Retrieves relevant context from a local vector DB
- LLM Node — Answers general queries using the model
- LangGraph Workflow — Orchestrates the nodes using a graph-based approach


---

