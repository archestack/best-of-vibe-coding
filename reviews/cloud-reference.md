# ☁️ Backend and cloud templates reviews · Best of Vibe Coding

Backend service templates (FastAPI, Express, Hono) that expose models or agents over an API, and vendor reference apps for Azure or Google Cloud. Back to the [leaderboard](../README.md#%EF%B8%8F-backend-and-cloud-templates).

<sub>🌐 Also on the web: [Backend and cloud templates on archestack.com](https://archestack.com/best-of-vibe-coding/cloud-reference/), each project on its own page.</sub>

<a name="agent-service-toolkit"></a>
### 🥇 [agent-service-toolkit](https://github.com/joshuac215/agent-service-toolkit) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (63) · Easy to run: easy (50) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

**LangGraph agents served by FastAPI with a Streamlit chat client.**

Python service where LangGraph v1 agents (interrupt, Command, Store) are served by FastAPI with streaming and non-streaming endpoints, AG-UI support, per-agent URL paths, /threads history and a Postgres checkpointer via docker compose. Includes an AgentClient, a Streamlit chat UI with voice, LangSmith feedback, Groq moderation, a ChromaDB RAG agent, unit, integration and smoke tests. Needs at least one LLM API key.

- **+** AG-UI endpoint for CopilotKit-style frontends alongside the REST API
- **+** docker compose watch runs Postgres, API and Streamlit with live reload
- **+** Unit and integration tests plus smoke tests for Postgres, Mongo, AG-UI and Langfuse
- **+** Hosted demo on Streamlit Cloud
- **−** Solo maintainer; issues triaged roughly biweekly
- **−** Streamlit client is a demo UI, not a product frontend
- **−** Content moderation needs a Groq API key
- **−** Tests only run outside Docker

<sub>Python, LangChain providers: OpenAI, Anthropic, Google, Ollama, VertexAI, vLLM/SGLang, AG-UI protocol · Needs LLM API key (OpenAI, Anthropic, Google, Groq, Ollama or others), PostgreSQL (compose), LangSmith (optional), ChromaDB (RAG agent) · GitHub template · Docker · env example file · [Repo](https://github.com/joshuac215/agent-service-toolkit) · [▶️ Demo ↗](https://agent-service-toolkit.streamlit.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-service-toolkit/)</sub>

<a name="azure-agent-landing-zone"></a>
### 🥈 [agent-landing-zone](https://github.com/azure/agent-landing-zone) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Oct 2026</sub>

**Azure infrastructure templates for deploying enterprise agent apps on Microsoft Foundry.**

Agent Landing Zone is an azd and Bicep template that provisions a Zero-Trust Azure environment for agent applications on Microsoft Foundry. `azd up` deploys the infrastructure plus UI, orchestrator and ingestion apps, each from its own Azure repository. `azd provision` deploys the infrastructure alone. It was previously named GPT-RAG.

- **+** Infrastructure-only mode via `azd provision`, with apps deployed later using `azd deploy`
- **+** Component versions pinned in manifest.json for reproducible releases
- **+** Custom apps can replace the defaults through app-definition.json
- **+** MIT license; docs cover network-isolated deployment
- **−** Tied to Azure and Microsoft Foundry; no other cloud is mentioned
- **−** Default UI, orchestrator and ingestion code live in three separate repositories
- **−** README gives no cost, quota or resource sizing figures
- **−** Prerequisites and configuration are only in external docs, not the README

<sub>Python · Needs Azure, Microsoft Foundry, Azure OpenAI, Azure AI Search, Azure Developer CLI · GitHub template · [Repo](https://github.com/azure/agent-landing-zone) · [📖 Docs ↗](https://azure.github.io/AI-Landing-Zones/agent-landing-zone/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-agent-landing-zone/)</sub>

<a name="full-stack-ai-agent-template"></a>
### 🥉 [full-stack-ai-agent-template](https://github.com/vstorm-co/full-stack-ai-agent-template) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="fastapi-langgraph-agent-production-ready-template"></a>
### #&#8288;4 [fastapi-langgraph-agent-production-ready-template](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (57) · Easy to run: hard (17) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**FastAPI service for a LangGraph agent with auth, memory and tracing.**

FastAPI backend with a stateful LangGraph agent (Postgres checkpointing, tool calling, human-in-the-loop), mem0 long-term memory on pgvector, JWT auth and sessions, slowapi rate limiting, Alembic migrations, optional Valkey/Redis cache, Langfuse tracing, Prometheus and Grafana, and evals. make docker-up starts the API on port 8000 with PostgreSQL. OpenAI only via ChatOpenAI; any OpenAI-compatible base URL works.

- **+** JWT sessions, rate limiting and structured per-request logging included
- **+** mem0 long-term memory runs in-process on pgvector; no mem0 cloud
- **+** Circular model fallback with retries and a total timeout budget
- **+** Langfuse, Prometheus and Grafana wired; Langfuse can be disabled
- **−** OpenAI (or OpenAI-compatible) only; multi-provider is an open issue
- **−** README leads with a sponsor pitch for Atlas Cloud
- **−** Needs the pgvector extension and an OpenAI key for memory
- **−** Not a GitHub template; clone and strip

<sub>Python, OpenAI via langchain_openai.ChatOpenAI (any OpenAI-compatible base URL) · Needs PostgreSQL with pgvector, OpenAI API key, Valkey/Redis (optional), Langfuse (optional) · Docker · env example file · [Repo](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastapi-langgraph-agent-production-ready-template/)</sub>

<a name="monid"></a>
### #&#8288;5 [monid](https://github.com/monid-ai/monid) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (67) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Oct 2026</sub>

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

<a name="generative-ai-project-template"></a>
### #&#8288;6 [generative-ai-project-template](https://github.com/aminedjeghri/generative-ai-project-template) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: fair (61) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 118 · MIT · Oct 2026</sub>

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

<a name="fullstack-solution-template-for-agentcore"></a>
### #&#8288;7 [fullstack-solution-template-for-agentcore](https://github.com/awslabs/fullstack-solution-template-for-agentcore) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (67) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 599 · Apache-2.0 · Oct 2026</sub>

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

<a name="openai-chat-app-quickstart"></a>
### #&#8288;8 [openai-chat-app-quickstart](https://github.com/azure-samples/openai-chat-app-quickstart) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: weak (10) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 254 · MIT · Sep 2026</sub>

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

<a name="serverless-rag-demo"></a>
### #&#8288;9 [serverless-rag-demo](https://github.com/aws-samples/serverless-rag-demo) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: weak (26) · Easy to run: hard (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT-0 · Oct 2026</sub>

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

<a name="azurechat"></a>
### #&#8288;10 [azurechat](https://github.com/microsoft/azurechat) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: known (42) · Freshness: active (100) · Maintenance: weak (16) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Aug 2026</sub>

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

<a name="get-started-with-ai-agents"></a>
### #&#8288;11 [get-started-with-ai-agents](https://github.com/azure-samples/get-started-with-ai-agents) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: weak (13) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 376 · MIT · Oct 2026</sub>

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
### #&#8288;12 [openai-chat-vision-quickstart](https://github.com/azure-samples/openai-chat-vision-quickstart) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: weak (20) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 224 · MIT · Oct 2026</sub>

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

<a name="nodejs-api-boilerplate"></a>
### #&#8288;13 [nodejs-api-boilerplate](https://github.com/vyancharuk/nodejs-api-boilerplate) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (9) · Freshness: recent (64) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 164 · MIT · Apr 2026</sub>

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
### #&#8288;14 [genai-api](https://github.com/louisbrulenaudet/genai-api) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (1) · Freshness: recent (61) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 111 · Apache-2.0 · Apr 2026</sub>

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
