# Aura GPT - Advanced AI Infrastructure 🚀

This repository contains a fully containerized deployment of **LibreChat**, enhanced with **Model Context Protocol (MCP)** and a dedicated **Admin Dashboard** for comprehensive observability and control.

## 🌟 Key Features

- **Full-Stack Orchestration:** Deployed using Docker Compose, integrating MongoDB, PostgreSQL (pgvector), Meilisearch, and RAG API.
- **MCP Integration:** Empowered the AI with a GitHub MCP server, allowing it to analyze, read, and reason over codebase repositories directly.
- **Enterprise Observability:** Integrated a custom Admin Dashboard to monitor token consumption, track user requests, and analyze model performance (Claude 3.7, O3-mini, etc.).
- **Production-Ready Security:** - Managed via environment variables for sensitive data protection.
  - Secured with User-provided API keys (OpenRouter/OpenAI/Gemini).
  - Registration controls to protect infrastructure quotas.
- **RAG Support:** Built-in Retrieval-Augmented Generation for document and file processing.

## 🛠 Tech Stack

- **Platform:** [LibreChat](https://www.librechat.ai/)
- **Infrastructure:** Docker & Docker Compose
- **Databases:** MongoDB (NoSQL), PostgreSQL with `pgvector` (Vector DB)
- **Search Engine:** Meilisearch
- **Deployment:** Easypanel
- **Model Provider:** OpenRouter (Unified API for Claude 3.7, GPT-4o, Gemini 2.0)

## 🚀 Quick Start (Deployment)

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/abdelati88/librechat-assiut.git](https://github.com/abdelati88/librechat-assiut.git)
   cd librechat-assiut

2. Configure Environment Variables:
Copy the .env.example and fill in your credentials (never commit your actual .env file):

GITHUB_PERSONAL_ACCESS_TOKEN

MONGODB_URI

ADMIN_EMAIL

POSTGRES_USER

POSTGRES_PASSWORD


3. Deploy with Docker Compose:


docker-compose up -d
