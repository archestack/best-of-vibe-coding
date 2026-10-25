# ☁️ Backend and cloud templates reviews · Best of Vibe Coding

Backend service templates (FastAPI, Express, Hono) that expose models or agents over an API, and vendor reference apps for Azure or Google Cloud. Back to the [leaderboard](../README.md#%EF%B8%8F-backend-and-cloud-templates).

<sub>🌐 Also on the web: [Backend and cloud templates on archestack.com](https://archestack.com/best-of-vibe-coding/cloud-reference/), each project on its own page.</sub>

<a name="full-stack-fastapi-template"></a>
### 🥇 [full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Oct 2026</sub>

**FastAPI and React starter with JWT auth, PostgreSQL and a generated API client.**

A GitHub template for a full-stack web app: a FastAPI backend using SQLModel and PostgreSQL, and a React/TypeScript frontend built with Vite, Tailwind CSS and shadcn/ui. The frontend is built into the backend and served on the same domain as the API. It includes JWT login, email password recovery, and Docker Compose with Traefik for self-hosting. It has no AI features built in.

- **+** Auto-generated frontend client for the FastAPI API
- **+** Pytest backend tests and Playwright end-to-end tests, with GitHub Actions CI/CD
- **+** Docker Compose with Traefik gives automatic HTTPS for self-hosting
- **+** Mailpit for local email testing and React Email templates
- **−** No AI or model integration; it is a generic app scaffold
- **−** No billing or payments wired in
- **−** Authentication is JWT with email recovery only; no OAuth or social login listed
- **−** PostgreSQL only; other databases are not mentioned

<sub>TypeScript · Needs PostgreSQL, Docker Compose, Traefik, Mailpit · GitHub template · ⚠️ .env file committed · [Repo](https://github.com/fastapi/full-stack-fastapi-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/full-stack-fastapi-template/)</sub>

<a name="full-stack-ai-agent-template"></a>
### 🥈 [full-stack-ai-agent-template](https://github.com/vstorm-co/full-stack-ai-agent-template) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Project generator for FastAPI and Next.js apps with agents and RAG.**

CLI (pip install fastapi-fullstack) scaffolding a FastAPI backend and Next.js frontend via a wizard or presets, with Pydantic AI, Pydantic Deep Agents, LangChain, LangGraph or DeepAgents, RAG on Milvus, Qdrant, pgvector or Chroma, WebSocket chat, JWT, OAuth, admin, teams, Stripe billing, Celery, Docker and K8s. make bootstrap starts Postgres, migrations and a seeded admin; projects can pull template upgrades later.

- **+** Wizard and presets pick framework, vector store, auth and billing per project
- **+** Template upgrades merge into generated projects on a branch
- **+** Chat UI renders tool calls, plans, subagents, charts and Python execution
- **+** 100% coverage badge and CI on the generator
- **−** Generator, not a repo to fork; output size depends on options chosen
- **−** Seeds admin@example.com with a fixed password; rotate before exposing
- **−** Optional services (Milvus, Redis, Celery) raise the local footprint
- **−** Windows needs GNU Make or WSL2

<sub>Python, Pydantic AI, Pydantic Deep Agents, LangChain, LangGraph · Needs PostgreSQL, Redis (optional), Milvus, Qdrant, pgvector or ChromaDB (RAG), Stripe (billing), LLM provider API key · [Repo](https://github.com/vstorm-co/full-stack-ai-agent-template) · [📖 Docs ↗](https://vstorm-co.github.io/full-stack-ai-agent-template/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/full-stack-ai-agent-template/)</sub>

<a name="agent-service-toolkit"></a>
### 🥉 [agent-service-toolkit](https://github.com/joshuac215/agent-service-toolkit) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

**LangGraph agent served by FastAPI with a Streamlit chat front end.**

Python template that wires a LangGraph agent to a FastAPI service with streaming and non-streaming endpoints, a reusable AgentClient, and a Streamlit chat app. It also serves every agent over the AG-UI protocol and includes a ChromaDB RAG agent, chat history via /threads, and LangSmith feedback. Fork it and add agents under src/agents.

- **+** Full path from agent to API, client and UI in one repo
- **+** Multiple agents routed by URL path, listed at /info
- **+** Token and message streaming, plus AG-UI endpoint for CopilotKit-style frontends
- **+** Unit and integration tests, plus smoke tests for Postgres, MongoDB and AG-UI
- **−** Tied to LangGraph; no other agent framework supported
- **−** Streamlit UI must be edited by hand to match new agents
- **−** Content moderation requires a Groq API key
- **−** Solo maintainer, issues triaged roughly biweekly; no tagged releases

<sub>Python, OpenAI, Ollama, VertexAI, vLLM · Needs LLM provider API key (e.g. OpenAI), PostgreSQL (in docker compose), ChromaDB (RAG agent), Groq API key (content moderation), LangSmith (optional) · GitHub template · Docker · env example file · [Repo](https://github.com/joshuac215/agent-service-toolkit) · [▶️ Demo ↗](https://agent-service-toolkit.streamlit.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-service-toolkit/)</sub>

<a name="monid"></a>
### #&#8288;4 [monid](https://github.com/monid-ai/monid) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

**Declarative connector framework behind a metered catalog of agent tool APIs.**

Monid is the connector layer for a hosted service that gives agents one base URL and key for 2,000+ tools across 72+ providers. Each provider and endpoint is a TypeScript definition (defineProvider, defineEndpoint) with zod input schemas, and the engine meters usage per call from the raw response. The repo lets you run connectors locally with your own vendor keys and add new ones by pull request.

- **+** Declarative connectors: no per-provider client or execution path, so coding agents can write them
- **+** Usage model per endpoint: flat, per result, or per unit, settled on the raw response
- **+** Tests replay recorded fixtures, so CI needs no network or vendor keys
- **+** Same compiled artifact runs locally, in CI, and on the hosted platform
- **−** Repo is only the connector layer; the hosted platform and billing are not included
- **−** Discovery, ranking and health data are described for the hosted service, not this repo
- **−** Requires Deno 2.x and your own vendor keys to run real endpoints
- **−** No Docker or compose setup provided

<sub>TypeScript · Needs Deno 2.x, Vendor API keys per provider · [Repo](https://github.com/monid-ai/monid) · [📖 Docs ↗](https://docs.monid.ai) · [🌐 Site ↗](https://monid.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/monid/)</sub>

<a name="fastapi-langgraph-agent-production-ready-template"></a>
### #&#8288;5 [fastapi-langgraph-agent-production-ready-template](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**FastAPI backend template for LangGraph agents with memory, auth and tracing.**

A Python backend template that wires a stateful LangGraph agent into FastAPI with JWT sessions, slowapi rate limiting, Alembic migrations and PostgreSQL checkpointing. Long-term memory runs in-process through mem0 and pgvector, and LLM calls go through a service with retries and circular model fallback. Observability comes from Langfuse tracing, Prometheus metrics and Grafana dashboards.

- **+** Circular model fallback with tenacity retries and a total timeout budget
- **+** Per-user long-term memory via mem0 and pgvector in your own PostgreSQL
- **+** Langfuse tracing, Prometheus metrics and Grafana dashboards included
- **+** Custom tools are added by registering a LangChain @tool function
- **−** Ships a single agent; supervisor or sub-agent setups must be wired by hand
- **−** mem0 memory needs an OpenAI API key for fact extraction and embeddings
- **−** Requires PostgreSQL with the pgvector extension
- **−** Non-OpenAI providers need extra packages and registry edits

<sub>Python, OpenAI, Anthropic, Ollama, Google GenAI · Needs PostgreSQL, pgvector, Langfuse (optional), Valkey/Redis (optional), Prometheus and Grafana (optional) · Docker · env example file · [Repo](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastapi-langgraph-agent-production-ready-template/)</sub>

<a name="azure-agent-landing-zone"></a>
### #&#8288;6 [agent-landing-zone](https://github.com/azure/agent-landing-zone) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Oct 2026</sub>

**Azure Bicep landing zone for deploying enterprise agent apps on Microsoft Foundry.**

Infrastructure-as-code template, deployed with Azure Developer CLI, that provisions a Zero-Trust network foundation on Azure for agent applications running on Microsoft Foundry. It can deploy the full stack with a default UI, orchestrator and optional ingestion component, infrastructure only, or a custom app on the same foundation. It is the renamed GPT-RAG project.

- **+** Three deploy paths: full stack, infrastructure only, or your own application
- **+** Zero-Trust network architecture with IaC-first deployment via azd
- **+** Component versions pinned in manifest.json for each release
- **+** Default UI, orchestrator and ingestion live in separate repos, so they can be swapped
- **−** Azure-only; requires Microsoft Foundry and an Azure subscription
- **−** README is a landing page; setup details live on an external docs site
- **−** No Docker or compose setup for local runs
- **−** Sizing, cost and RAM requirements are unknown from the README

<sub>Python, Azure OpenAI · Needs Azure subscription, Microsoft Foundry, Azure OpenAI, Azure AI Search, Azure Developer CLI · GitHub template · [Repo](https://github.com/azure/agent-landing-zone) · [📖 Docs ↗](https://azure.github.io/AI-Landing-Zones/agent-landing-zone/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-agent-landing-zone/)</sub>

<a name="fastcrud"></a>
### #&#8288;7 [fastcrud](https://github.com/benavlabs/fastcrud) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Async CRUD methods and auto-generated endpoints for FastAPI and SQLAlchemy 2.0.**

FastCRUD is a Python library that adds async CRUD operations on SQLAlchemy 2.0 models and a crud_router helper that generates FastAPI endpoints from a model and Pydantic schemas. It supports joins with auto-detected conditions, dynamic filtering and sorting, and offset and cursor pagination. It also ships a bundled agent skill that coding tools can load through library-skills.

- **+** crud_router generates endpoints from a model plus create and update schemas
- **+** Offset and cursor pagination built in, with auto-detected join conditions
- **+** Can be used inside hand-written FastAPI routes via FastCRUD(Model)
- **+** Bundled agent skill covers N+1 avoidance and when to use raw SQLAlchemy
- **−** Aggregates, CTEs, GROUP BY projections and bulk writes need raw SQLAlchemy
- **−** Requires Python 3.10+, SQLAlchemy 2.0.21+ and Pydantic 2.4.1+
- **−** Non-native column types such as sqlalchemy-utils may raise NotImplementedError
- **−** Library only: no auth, billing or frontend included

<sub>Python · Needs FastAPI, SQLAlchemy >=2.0.21, Pydantic >=2.4.1, SQLAlchemy-Utils (optional) · [Repo](https://github.com/benavlabs/fastcrud) · [📖 Docs ↗](https://benavlabs.github.io/fastcrud/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastcrud/)</sub>

<a name="node-typescript-boilerplate"></a>
### #&#8288;8 [node-typescript-boilerplate](https://github.com/jsynowiec/node-typescript-boilerplate) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: patchy (34) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

**Framework-free Node.js TypeScript starter with Vitest, ESLint and CI.**

A minimal repository template for Node.js 24 projects using TypeScript 6 with strict settings and native ESM. It ships Vitest, ESLint with typescript-eslint, Prettier, a GitHub Actions workflow, Mise toolchain config and an AGENTS.md file with guidance for AI coding agents. It deliberately includes no web framework, database, auth or Docker.

- **+** No framework, database or ORM imposed; small dependency surface
- **+** Native ESM with strict TypeScript 6 config targeting ES2024
- **+** Vitest, ESLint, Prettier and GitHub Actions CI preconfigured
- **+** Includes AGENTS.md so coding agents get project rules from the start
- **−** No HTTP server, auth, database or Docker; all of that is left to you
- **−** ESM only; CommonJS projects must convert, and issues about it are not accepted
- **−** Targets Node.js 24 only; older runtimes are not covered
- **−** AGENTS.md is a generic example that needs rewriting per project

<sub>TypeScript · Needs Node.js 24, npm, Mise (recommended) · GitHub template · [Repo](https://github.com/jsynowiec/node-typescript-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/node-typescript-boilerplate/)</sub>

<a name="nunu"></a>
### #&#8288;9 [nunu](https://github.com/go-nunu/nunu) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Aug 2026</sub>

**Go CLI that scaffolds layered Gin and Gorm projects with Wire injection.**

Nunu is a Go CLI that generates a project from a template repo (basic, advanced or monorepo) and creates handler, service, repository and model files per entity. It wires Gin, Gorm, Wire, Viper, Zap and go-redis into a layered layout, and `nunu run` starts the app with hot reload. It is a general backend scaffold; AI support is limited to an MCP server layout and an agent skill.

- **+** `nunu create all user` generates handler, service, repository and model in the right directories
- **+** `nunu run` gives hot reload; `nunu wire` regenerates Wire dependency injection code
- **+** Built on common libraries (Gin, Gorm, Viper, Zap, Casbin, gocron), so little new to learn
- **+** Separate agent skill and MCP server layout exist for coding agents
- **−** No AI or model-serving functionality in the core tool
- **−** Requires Go 1.25.8 or newer
- **−** README says updates will be infrequent
- **−** Templates are pulled from Git repos at creation time, so network access is needed

<sub>Go · Needs Go 1.25.8+, Git, MySQL 5.7+ (optional), Redis (optional), Docker (optional) · [Repo](https://github.com/go-nunu/nunu) · [📖 Docs ↗](https://github.com/go-nunu/nunu/blob/main/docs/en/guide.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nunu/)</sub>

<a name="fullstack-solution-template-for-agentcore"></a>
### #&#8288;10 [fullstack-solution-template-for-agentcore](https://github.com/awslabs/fullstack-solution-template-for-agentcore) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 600 · Apache-2.0 · Oct 2026</sub>

**React frontend and AgentCore backend starter, deployed to AWS with CDK or Terraform.**

A forkable starter that deploys a React/TypeScript chat frontend on Amplify Hosting, authenticated through Cognito, in front of an Amazon Bedrock AgentCore backend. The baseline is a multi-turn agent with a Lambda text-analysis tool behind AgentCore Gateway and the AgentCore Code Interpreter. Agent patterns exist for Strands and LangGraph, and the repo includes steering docs meant to be fed to coding assistants.

- **+** Deploys with CDK or Terraform; Cognito JWT auth and Cedar policies on Gateway are included
- **+** Agent patterns for both Strands and LangGraph under patterns/
- **+** Frontend uses React, Vite, Tailwind and shadcn components
- **+** Extensive docs for memory, streaming, sessions, observability and swapping out Cognito
- **−** Requires AWS and Amazon Bedrock AgentCore; no other backend is supported
- **−** README calls it a proof-of-value, not production-ready
- **−** Baseline is only a simple chat agent with two tools
- **−** No tagged releases

<sub>Python, Amazon Bedrock · Needs AWS account, Amazon Bedrock AgentCore, Amazon Cognito, AWS Amplify Hosting, AWS Lambda, API Gateway · Docker · [Repo](https://github.com/awslabs/fullstack-solution-template-for-agentcore) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fullstack-solution-template-for-agentcore/)</sub>

<a name="generative-ai-project-template"></a>
### #&#8288;11 [generative-ai-project-template](https://github.com/aminedjeghri/generative-ai-project-template) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 118 · MIT · Oct 2026</sub>

**uv workspace with FastAPI, NiceGUI, LiteLLM and Promptfoo evals.**

Python 3.12 uv workspace with a FastAPI backend (port 8000) and NiceGUI frontend (port 8080) for chat, information extraction and RAG over documents, with models served locally by Ollama or through any LiteLLM provider. Ships Makefiles for install, run, test, Docker (CPU and CUDA compose), pre-commit with ruff and detect-secrets, pytest, Promptfoo and Ragas evals, GitHub Actions, Renovate and an mkdocs site.

- **+** LiteLLM naming lets you switch between Ollama and cloud models by env
- **+** Promptfoo and Ragas evaluation wired into the template
- **+** CPU and CUDA docker compose variants
- **+** CI tests the app against local Ollama models
- **−** NiceGUI frontend is unusual for product UIs
- **−** No auth, database or persistence described
- **−** Ubuntu 22.04 or macOS only per prerequisites
- **−** CUDA path installs PyTorch; heavier install

<sub>Python, LiteLLM (any provider), Ollama · Needs Ollama (local models) or an LLM provider key via LiteLLM · GitHub template · Docker · env example file · [Repo](https://github.com/aminedjeghri/generative-ai-project-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/generative-ai-project-template/)</sub>

<a name="azurechat"></a>
### #&#8288;12 [azurechat](https://github.com/microsoft/azurechat) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (33) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Aug 2026</sub>

**Private enterprise chat on Azure OpenAI with document chat and personas.**

Microsoft solution accelerator: a Next.js chat app deployed into your own Azure subscription with azd up or a Deploy to Azure button, protected by an identity provider (Entra ID setup scripted), with chat over uploaded files, personas, extensions and managed-identity RBAC instead of keys. Supports private endpoints and ESLZ-compliant deployment. For organizations wanting a ChatGPT-like tenant on Azure OpenAI.

- **+** Managed identity removes almost all keys and secrets
- **+** Chat over files, personas and extensions documented in docs/
- **+** Private endpoints and ESLZ-compliant deployment supported
- **+** azd template plus GitHub Actions deploy path
- **−** Azure only; provisions several paid services
- **−** Identity provider setup is mandatory before first use
- **−** Contributions require a Microsoft CLA
- **−** README defers most detail to docs/; no tests mentioned

<sub>TypeScript, Azure OpenAI · Needs Azure subscription, Azure OpenAI, Entra ID or another identity provider · [Repo](https://github.com/microsoft/azurechat) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azurechat/)</sub>

<a name="serverless-rag-demo"></a>
### #&#8288;13 [serverless-rag-demo](https://github.com/aws-samples/serverless-rag-demo) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT-0 · Oct 2026</sub>

**AWS CDK sample for document RAG chat and multi-agent workflows on Bedrock.**

Deploys a RAG chat app on AWS with one `sh deploy.sh` wizard that runs `cdk deploy --all`. Documents are indexed through a Bedrock Knowledge Base into OpenSearch Serverless NextGen and queried with hybrid BM25 + KNN search. A Strands Graph multi-agent runtime on Bedrock AgentCore routes requests to specialist nodes for code, presentations, web search, weather and retrieval.

- **+** Hybrid BM25 + KNN search with per-user document isolation
- **+** Demo OCU mode scales to zero, so idle cost is listed as $0
- **+** Full infrastructure as Python CDK stacks, with Cognito auth and CloudFront hosting
- **+** MIT-0 license with no attribution requirement
- **−** AWS only: Bedrock, AgentCore, OpenSearch Serverless and Cognito are all required
- **−** Models fixed to Claude Sonnet/Opus 4.6 and Titan Embed V2; no other providers listed
- **−** Supported in six regions only; us-west-1 and ap-southeast-1 excluded
- **−** No release tags, and tests cover CDK unit checks only

<sub>Python, Claude Sonnet 4.6, Claude Opus 4.6, Amazon Titan Embed Text V2 · Needs AWS account, Amazon Bedrock, OpenSearch Serverless NextGen, Bedrock AgentCore, Amazon Cognito, CloudFront, S3, Docker, AWS CDK CLI · Docker · [Repo](https://github.com/aws-samples/serverless-rag-demo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless-rag-demo/)</sub>

<a name="get-started-with-ai-agents"></a>
### #&#8288;14 [get-started-with-ai-agents](https://github.com/azure-samples/get-started-with-ai-agents) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 376 · MIT · Oct 2026</sub>

**Azure azd template for a Foundry agent chat app with file search.**

Deploys a web chat app on Azure Container Apps backed by a Microsoft Foundry Agent Service agent. The agent answers from uploaded files using file search or optional Azure AI Search and returns citations. Tracing goes to Application Insights, and the repo includes Pytest-based agent evaluation and red-teaming scans.

- **+** Single `azd up` provisions Foundry project, model, Container App, storage and monitoring
- **+** Tracing via Application Insights and Azure Monitor included
- **+** Pytest agent evaluation and AI Red Teaming scans included
- **+** Managed Identity used for deployment and local development
- **−** Requires an Azure subscription and Foundry model quota; no non-Azure path
- **−** README warns the code is a showcase, not production-ready without extra security
- **−** Costs are usage-based and the README gives no estimate
- **−** Deployment takes 7–15 minutes with `azd up`; teardown up to 20

<sub>Bicep, gpt-5-mini (default), other Azure AI models configurable · Needs Microsoft Foundry, Foundry Agent Service, Azure Container Apps, Azure Container Registry, Azure Storage, Azure AI Search (optional), Application Insights (optional), Log Analytics (optional) · [Repo](https://github.com/azure-samples/get-started-with-ai-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/get-started-with-ai-agents/)</sub>

<a name="openai-chat-vision-quickstart"></a>
### #&#8288;15 [openai-chat-vision-quickstart](https://github.com/azure-samples/openai-chat-vision-quickstart) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT · Oct 2026</sub>

**Quart chat app that answers questions about uploaded images via Azure OpenAI.**

A Python Quart backend uses the openai package to send user messages and uploaded images to a GPT-4o deployment on Azure OpenAI. The frontend is plain HTML/JS that streams JSON Lines responses, with browser speech input and output buttons. Bicep files and azd provision Azure OpenAI, Container Apps, Container Registry and Log Analytics, using managed identity by default.

- **+** One azd up provisions Azure OpenAI, Container Apps, registry, logging and RBAC
- **+** Managed identity by default, so no API key in app config
- **+** Can point at a local OpenAI-compatible endpoint (Ollama doc) for development
- **+** Speech input/output uses free built-in browser APIs
- **−** Deploying needs Azure subscription and role-assignment write permissions
- **−** Basic HTML/JS frontend with no auth or multi-user features
- **−** Container Registry has a fixed daily cost even when idle
- **−** Local dev server still needs Azure credentials or a compatible endpoint

<sub>Jupyter Notebook, GPT-4o (Azure OpenAI), OpenAI-compatible endpoints · Needs Azure OpenAI, Azure Container Apps, Azure Container Registry, Azure Developer CLI · env example file · [Repo](https://github.com/azure-samples/openai-chat-vision-quickstart) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/ai/get-started-app-chat-vision?tabs=github-codespaces) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chat-vision-quickstart/)</sub>

<a name="openai-chat-app-quickstart"></a>
### #&#8288;16 [openai-chat-app-quickstart](https://github.com/azure-samples/openai-chat-app-quickstart) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 254 · MIT · Sep 2026</sub>

**Minimal Quart chat app on Azure OpenAI with managed identity.**

Python Quart backend using the openai package with a plain HTML/JS frontend that streams JSON Lines over a ReadableStream, plus Bicep for Azure OpenAI, Container Apps, Container Registry, Log Analytics and RBAC roles, deployed with azd up. Authenticates to Azure OpenAI with managed identity, so no API key; the local dev server runs on port 50505 after a first azd deploy. For teams starting a chat service on Azure.

- **+** Managed identity auth; no OpenAI key in config
- **+** Bicep provisions the full Container Apps stack
- **+** Codespaces and Dev Container configs included
- **+** IaC security scan GitHub Action included
- **−** Local run depends on a prior Azure deployment for the endpoint
- **−** No user auth; sibling repos add Entra ID
- **−** Frontend is minimal HTML/JS, not a component framework
- **−** Azure Container Registry has a fixed daily cost

<sub>Bicep, Azure OpenAI (openai package) · Needs Azure subscription with Azure OpenAI access, azd CLI · GitHub template · env example file · [Repo](https://github.com/azure-samples/openai-chat-app-quickstart) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/ai/get-started-securing-your-ai-app?tabs=github-codespaces) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chat-app-quickstart/)</sub>

<a name="nodejs-api-boilerplate"></a>
### #&#8288;17 [nodejs-api-boilerplate](https://github.com/vyancharuk/nodejs-api-boilerplate) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: niche (7) · Freshness: recent (62) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 165 · MIT · Apr 2026</sub>

**Express TypeScript CRUD API template with an LLM module generator.**

Express and TypeScript REST API with vertical-slice modules, Zod validation, InversifyJS DI, Knex transactions, ioredis caching, winston trace IDs, node-cron, S3 uploads and Supertest e2e tests, run via docker compose on port 8080. The llm-codegen folder runs three LLM micro-agents (Developer, Troubleshooter, TestsFixer) that generate a new CRUD module, migration, seeds and passing tests from a text description.

- **+** Codegen loop compiles and runs e2e tests until they pass
- **+** Supports OpenAI, Anthropic, DeepSeek and OpenRouter keys for generation
- **+** JWT auth routes, Redis cache and cron already in the base API
- **+** Tests run in Docker or against local SQLite
- **−** AI is a dev-time generator; the API itself has no AI features
- **−** Node badge pins v14 to v20; check against current LTS
- **−** Generated code still needs manual review and integration
- **−** Last commit 2026-04

<sub>TypeScript, OpenAI, Anthropic, DeepSeek, OpenRouter · Needs PostgreSQL or SQLite, Redis, AWS S3 (uploads), LLM API key for codegen · GitHub template · Docker · env example file · [Repo](https://github.com/vyancharuk/nodejs-api-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nodejs-api-boilerplate/)</sub>

<a name="genai-api"></a>
### #&#8288;18 [genai-api](https://github.com/louisbrulenaudet/genai-api) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: niche (1) · Freshness: recent (59) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 111 · Apache-2.0 · Apr 2026</sub>

**Hono API on Cloudflare Workers proxying Gemini with bearer auth.**

Hono TypeScript worker exposing POST /completion that forwards OpenAI-style messages (text and data-URL images) to Gemini 2.0 and 2.5 Flash models through Cloudflare AI Gateway, validated with Zod and returned as plain text. Secured by a BEARER_TOKEN secret, with an optional X-API-Key header to pass a provider key per request; deployed with make deploy. Built for Apple Shortcuts; local dev on port 8788.

- **+** Bearer-token auth and Zod validation on the single endpoint
- **+** Requests route through Cloudflare AI Gateway for caching and logs
- **+** Multimodal input via data-URL images
- **+** Biome lint and Snyk badge
- **−** Google AI Studio provider only; four Gemini Flash models
- **−** Plain-text responses, no streaming
- **−** No tests mentioned; last commit 2026-04
- **−** Needs a Cloudflare account and AI Gateway id

<sub>TypeScript, Gemini 2.5 Flash, 2.5 Flash Lite, 2.0 Flash, 2.0 Flash Lite via Cloudflare AI Gateway, OpenAI SDK client · Needs Cloudflare account with AI Gateway, Google AI Studio API key · GitHub template · [Repo](https://github.com/louisbrulenaudet/genai-api) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/genai-api/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
