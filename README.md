# MentorMesh AI Core

MentorMesh AI Core is the reusable multi-agent intelligence engine for the MentorMesh AI learning platform.

It provides:

- LangGraph workflow orchestration
- MCP-style filesystem and memory tools
- A2A quiz service architecture
- Ollama local LLM integration
- Langfuse observability
- DeepEval evaluation pipelines
- FastAPI AI Gateway
- Security middleware
- Dockerized runtime

## Repository Role

This repository owns only the AI backend core.

It does not own:

- Web frontend
- Web backend SaaS control plane
- Prisma/PostgreSQL business persistence
- Billing
- Mobile app
- Desktop app

## Local Setup

```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
make api