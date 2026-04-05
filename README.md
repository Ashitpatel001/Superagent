# 🌟 Superagent AI Platform

Welcome to the Superagent mono-repo. This repository serves as my personal flagship architecture, showcasing the integration of cutting-edge agentic workflows, Model Context Protocol (MCP), and high-performance Retrieval-Augmented Generation (RAG).

This project demonstrates a production-ready separation of concerns, isolating the Python-based intelligence engine from the modern React user interface to ensure extreme scalability and maintainability.

## ✨ Core Capabilities

* **Advanced RAG Pipeline:** Leverages ChromaDB for high-speed vector storage and semantic context retrieval.
* **Complex Data Ingestion:** Integrates the Unstructured library to parse and extract clean data from dense enterprise documents and PDFs.
* **Dynamic Tool Integration (MCP):** Utilizes Composio to implement the Model Context Protocol, granting the AI agent secure, real-time execution capabilities across external APIs.
* **Full-Stack Orchestration:** A clean, modular bridge between the backend reasoning engine and the interactive frontend client.

## 🛠️ Technology Stack

* **Intelligence Routing:** LangGraph & LangChain
* **Backend:** Python, FastAPI, ChromaDB, Composio, Unstructured
* **Frontend:** React / Next.js, Tailwind CSS
* **Core Models:** Extensible architecture supporting Gemini, OpenAI, or local HuggingFace alternatives.

## 🚀 Quick Start

To execute this architecture locally, you must boot the backend server and the frontend client simultaneously in separate terminal instances.

**Terminal 1: Boot the Intelligence Layer**
```bash
cd superagent-backend
python -m venv venv
# Activate your virtual environment (Windows: venv\Scripts\activate | Mac/Linux: source venv/bin/activate)
pip install -r requirements.txt
uvicorn app.main:app --reload --port 5050
Terminal 2: Boot the User Interface
```

**Terminal 2: Boot the User Interface**

```bash
cd superagent-frontend
npm install
npm run dev
```
**For strict environment variable configurations and API requirements, consult the detailed documentation located within the backend and frontend directories.**
