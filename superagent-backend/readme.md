
# 🧠 Superagent Backend: Intelligence Engine

This directory contains the core reasoning and API routing layer for the Superagent platform. It is engineered to process unstructured data, orchestrate tools via MCP, and stream AI responses with absolute type safety.

## 🛠️ System Components

* **Framework:** FastAPI (Asynchronous Python)
* **Vector Engine:** ChromaDB (Local RAG)
* **Data Ingestion:** Unstructured (Document parsing pipeline)
* **Agent Orchestration:** LangGraph (Stateful agent routing)
* **Tool Integrations:** Composio (Model Context Protocol)

## ⚙️ Secure Vault Setup

You must configure your local environment variables before initializing the server. 

1. Duplicate the blueprint file to establish your local vault:
   `cp .env.example .env`
2. Open `.env` and inject your active credentials (LLM keys, Composio API tokens, etc.). Never commit your active `.env` file to version control.

## 🚀 Initialization Sequence

Isolate your AI dependencies using a standard virtual environment.

```bash
# 1. Initialize the virtual environment
python -m venv venv

# 2. Activate the environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 3. Install the dependency matrix
pip install -r requirements.txt

# 4. Ignite the server
uvicorn app.main:app --reload --host 0.0.0.0 --port 5050
```
