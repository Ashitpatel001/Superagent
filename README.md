# Superagent AI Platform

Welcome to the Superagent mono-repo. This is an advanced, AI-powered predictive maintenance and intelligent agent platform designed for enterprise scalability.

This repository is structured as a mono-repo containing both the intelligence layer and the user interface. By isolating our domains, we maintain strict architectural boundaries while enabling seamless deployment.

## Architecture Overview

* **superagent-backend:** The intelligence engine. Built with FastAPI, LangGraph, and PostgreSQL. It handles secure authentication, routing, and Retrieval-Augmented Generation (RAG) using ChromaDB and HuggingFace CPU optimized embeddings.
* **superagent-frontend:** The interactive user interface. Built with Next.js, providing a highly responsive and state-driven experience for interacting with the AI agents.

## Quick Start

To run the full stack locally, you will need two terminal windows open.

**Terminal 1: Boot the Intelligence Layer**
```Bash
cd superagent-backend
python -m venv venv
# Activate your virtual environment (Windows: venv\Scripts\activate | Mac/Linux: source venv/bin/activate)
pip install -r requirements.txt
uvicorn app.main:app --reload --port 5050
```

**Terminal 2: Boot the User Interface**
```Bash
cd superagent-frontend
npm install
npm run dev
```
**For detailed setup instructions, including environment variable configurations, please refer to the specific README files located inside each respective directory.**
