# LangGraph_USA-Topic-Classifier

# 🇺🇸 USA Classifier Agent with LangGraph

This repository demonstrates how to build a basic agent using [LangGraph](https://python.langchain.com/docs/langgraph/) — a state-machine-based framework for controlling LLM workflows.

---

## 🔧 Features

- 🧠 **Supervisor Node**: Classifies user query into "USA" or "Not Related"
- 🧩 **Pydantic Parser**: Parses and enforces structured output from LLM
- 🔀 **Router Function**: Directs the question to RAG or LLM node
- 📚 **RAG Node**: Retrieves answers from a vector database built on custom `.txt` files
- 🤖 **LLM Node**: Answers general questions using Gemini Flash

---
