# 📚 RAG and search reviews · Best of Vibe Coding

Retrieval over your own documents or data, answer engines, and natural-language-to-SQL starters. Back to the [leaderboard](../README.md#-rag-and-search).

<sub>🌐 Also on the web: [RAG and search on archestack.com](https://archestack.com/best-of-vibe-coding/rag-search/), each project on its own page.</sub>

<a name="xerj"></a>
### 🥇 [xerj](https://github.com/xerj-org/xerj) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (93) · Easy to run: hard (17) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

**Elasticsearch-compatible search server that auto-indexes folders for coding agents.**

XERJ is a single Rust binary that speaks the Elasticsearch API. `xerj autoindex <folder>` infers datasets from code, docs, logs, PDFs, SQLite and CSV, and creates one typed index per dataset, with tree-sitter symbols and line numbers for code. It supports BM25, kNN and hybrid search, a `/_memory` agent memory API, and a `xerj mcp` stdio server exposing 13 tools. Its main pitch is cutting agent token use by retrieving passages instead of reading files.

- **+** Single static binary, no JVM; prebuilt for Linux, macOS and Windows on x86-64 and arm64
- **+** Works with existing Elasticsearch clients pointed at localhost:9200; 1366/1369 ES-YAML conformance tests
- **+** Autoindex needs no schema; handles code, PDF, DOCX, XLSX, SQLite, mail and logs
- **+** Default lexical embedder runs offline; air-gapped deployment recipe is documented
- **−** Token savings come from the project's own 16-run study; neutral to negative on popular libraries
- **−** Default embedder is lexical feature-hashing; neural mode is opt-in and downloads about 90 MB
- **−** `--insecure` quick start disables TLS and auth; every caller becomes a superuser
- **−** Optional Jev rerank sends result text to TypeSafe's servers

<sub>Rust, lexical embedder (default, offline), neural embedder (opt-in, ~90 MB download), Jev reranker (optional, external service) · [Repo](https://github.com/xerj-org/xerj) · [▶️ Demo ↗](https://xerj.org/playground/) · [📖 Docs ↗](https://xerj.org/docs/recipes/) · [🌐 Site ↗](https://xerj.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xerj/)</sub>

<a name="llm-app"></a>
### 🥈 [llm-app](https://github.com/pathwaycom/serviette) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (51) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Oct 2026</sub>

**YAML-configured RAG server that keeps a vector database synced with a document folder.**

serviette watches a folder or remote source (Google Drive, S3/MinIO, SharePoint, FTP/SFTP/WebDAV), parses and embeds documents with Pathway, and writes them to one of 8 vector databases. A separate stateless server hosts a web chat UI on / and a REST API under /api/v1 on port 8989, answering with cited sources. Edits and deletions in the source become upserts and deletes in the store within seconds.

- **+** Edits, additions and deletions propagate to the vector store as real upserts and deletes
- **+** 8 backends: DuckDB (default, embedded), pgvector, Qdrant, Milvus, ChromaDB, Weaviate, Pinecone, MongoDB Atlas
- **+** Indexer and server are separate processes sharing only the database; server scales horizontally
- **+** Published benchmarks: 50 GB of text indexed at 14.65 GiB peak PSS, plus FRAMES retrieval results
- **−** Requires a Pathway license key, free but obtained via GitHub or LinkedIn sign-in
- **−** No conversation memory or user accounts; answers one question at a time
- **−** Default DuckDB backend is single-writer, so it suits laptops and demos only
- **−** Local embeddings pull in PyTorch (about 0.8 GB for the CPU build)

<sub>Python, OpenAI, LiteLLM, SentenceTransformers, Gemini · Needs Pathway license key, Python with pip 23.1+, OpenAI API key (optional, for generated answers), Vector database (embedded DuckDB by default) · [Repo](https://github.com/pathwaycom/serviette) · [📖 Docs ↗](https://github.com/pathwaycom/serviette/blob/main/docs/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llm-app/)</sub>

<a name="azure-search-openai-demo"></a>
### 🥉 [azure-search-openai-demo](https://github.com/azure-samples/azure-search-openai-demo) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (64) · Easy to run: hard (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Oct 2026</sub>

**Azure RAG chat reference on AI Search and Azure OpenAI.**

The canonical Azure RAG sample: a Python (Quart) backend and React frontend answering multi-turn questions over your documents with citations and a visible thought process, using Azure AI Search for retrieval and Azure OpenAI for generation. azd up provisions Container Apps, AI Search, Document Intelligence and Blob storage, with optional Cosmos DB chat history, Entra login with document ACLs, multimodal and speech. For teams already on Azure.

- **+** Optional Entra login with per-document access control and Cosmos DB chat history
- **+** Evaluation, safety evaluation, monitoring and productionizing guides in docs/
- **+** Multimodal, speech and agentic retrieval are switchable features
- **+** Commits within the last week; tests included
- **−** Cannot run locally until azd up has provisioned Azure resources
- **−** Provisions paid services by default (AI Search, Document Intelligence); run azd down
- **−** Azure OpenAI only; no other provider path
- **−** README itself says not production-ready without extra security work

<sub>Python, azure-openai · Needs azure-subscription, azd, azure-ai-search, azure-openai, azure-document-intelligence, azure-blob-storage · [Repo](https://github.com/azure-samples/azure-search-openai-demo) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/python/get-started-app-chat-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-search-openai-demo/)</sub>

<a name="rag-postgres-openai-python"></a>
### #&#8288;4 [rag-postgres-openai-python](https://github.com/azure-samples/rag-postgres-openai-python) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: patchy (49) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 508 · MIT · Oct 2026</sub>

**RAG over Postgres table rows with hybrid search and SQL filters.**

A FastAPI backend and React frontend that answer chat questions about rows in a PostgreSQL table. Retrieval is hybrid (pgvector similarity plus full-text search fused with RRF), an OpenAI function call turns phrases like cheaper than 30 dollars into WHERE clauses, and it runs against Azure OpenAI, OpenAI.com or Ollama; azd deploys it to Container Apps with managed identity. For teams whose knowledge is structured rows, not documents.

- **+** Hybrid vector plus full-text search with RRF is implemented in SQL, not a vendor service
- **+** Provider switch by env var: Azure OpenAI, OpenAI.com or Ollama
- **+** Evaluation, safety evaluation and load-testing docs included
- **+** Tests included; dev container and Codespaces configs
- **−** Deploy path is Azure-only (azd, Container Apps, Flexible Server)
- **−** Local run expects Postgres 14+ with pgvector installed yourself
- **−** Sample schema is one products table; multi-table questions need new code
- **−** No auth in the app itself

<sub>Python, azure-openai, openai, ollama · Needs postgres-pgvector, azure-openai-or-openai-or-ollama, azd · GitHub template · env example file · [Repo](https://github.com/azure-samples/rag-postgres-openai-python) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rag-postgres-openai-python/)</sub>

<a name="chat-langchain"></a>
### #&#8288;5 [chat-langchain](https://github.com/langchain-ai/chat-langchain) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: patchy (49) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

**LangChain docs Q&A agent with a Next.js chat frontend.**

Documentation assistant that answers questions about LangChain, LangGraph and LangSmith. A Python agent built with LangChain middleware and deployed as a Managed Deep Agent searches the docs through a managed MCP connector and a Pylon support knowledge base, then checks links before answering. A Next.js frontend in frontend/ provides the chat UI with Supabase auth.

- **+** Production example with guardrails, link validation and retry middleware as separate modules
- **+** Includes a Next.js chat UI with Supabase auth and per-user thread scoping
- **+** Docs search goes through a managed MCP connector declared in tools/mcp.py
- **+** MIT licensed; local dev with `mda dev .` and `npm run dev:local`
- **−** Tied to the Managed Deep Agents runtime for deploy, identity and checkpointing
- **−** Needs a Pylon API key and KB ID, plus Supabase for frontend auth
- **−** Prompts and tools are specific to LangChain docs; reuse means rewriting them
- **−** No Docker or compose files and no tagged releases

<sub>TypeScript, Anthropic (or another provider) · Needs Managed Deep Agents (mda), Supabase, Pylon, LangSmith, Anthropic API key (or another provider) · env example file · [Repo](https://github.com/langchain-ai/chat-langchain) · [📖 Docs ↗](https://docs.langchain.com/oss/python/langchain/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-langchain/)</sub>

<a name="chat-with-your-data-solution-accelerator"></a>
### #&#8288;6 [chat-with-your-data-solution-accelerator](https://github.com/azure-samples/chat-with-your-data-solution-accelerator) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: patchy (48) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Oct 2026</sub>

**Azure RAG chat app that answers from your documents with citations.**

Deploys a React frontend, a FastAPI backend and an Azure Functions ingestion worker to Azure Container Apps with `azd up`. Uploaded files and web pages are parsed, chunked and embedded, then answered with streamed responses and inline citations. Retrieval and chat history use either Azure AI Search with Cosmos DB or PostgreSQL with pgvector, chosen at deploy time.

- **+** Choice of Azure AI Search + Cosmos DB or PostgreSQL + pgvector at deploy time
- **+** Managed identity and RBAC for all calls; no Key Vault or app secrets
- **+** Admin UI for ingesting documents and editing prompts without code changes
- **+** Two selectable orchestrators: Agent Framework or LangGraph
- **−** Azure-only; requires Foundry, Document Intelligence, Storage, and Container Apps
- **−** Needs Contributor and RBAC rights on the subscription, plus model quota
- **−** README calls it a starting point, not production-ready
- **−** No Docker or compose files detected in the repo; local setup is in docs

<sub>Python, Azure AI Foundry chat and embedding models · Needs Azure AI Foundry, Azure AI Search, Azure Cosmos DB, Azure Database for PostgreSQL, Azure Document Intelligence, Azure Storage, Azure Container Apps, Azure Functions, Azure Content Safety, Azure AI Speech · Docker · env example file · [Repo](https://github.com/azure-samples/chat-with-your-data-solution-accelerator) · [📖 Docs ↗](https://github.com/Azure-Samples/chat-with-your-data-solution-accelerator/blob/main/docs/DeploymentGuide.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-with-your-data-solution-accelerator/)</sub>

<a name="llm-answer-engine"></a>
### #&#8288;7 [llm-answer-engine](https://github.com/developersdigest/llm-answer-engine) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: popular (59) · Freshness: recent (69) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Apr 2026</sub>

**Perplexity-style Next.js answer engine over Brave search results.**

A Next.js app that takes a question, pulls results from Brave Search and Serper, scrapes the top pages with Cheerio, chunks and embeds them with OpenAI embeddings, and streams an answer from Groq (Mixtral by default) with sources, images and follow-ups. Optional Ollama, Upstash rate limiting, a semantic cache and a Portkey gateway are toggles in app/config.tsx; there is no auth or persistence. For developers learning the search-scrape-answer loop.

- **+** Full pipeline readable in one config file: search, scrape, chunk, embed, answer
- **+** docker compose and a standalone Express API variant included
- **+** Optional rate limiting and semantic cache via Upstash
- **−** Four API keys to start (OpenAI, Groq, Brave, Serper)
- **−** No auth, no chat history, no tests
- **−** Pinned to Next.js 14.1 and dated defaults (mixtral-8x7b-32768)
- **−** Ollama mode skips follow-up questions; vectors are in-memory only

<sub>TypeScript, groq, openai, ollama, portkey · Needs openai-api-key, groq-api-key, brave-search-api-key, serper-api-key · Docker · env example file · [Repo](https://github.com/developersdigest/llm-answer-engine) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llm-answer-engine/)</sub>

<a name="azure-search-openai-javascript"></a>
### #&#8288;8 [azure-search-openai-javascript](https://github.com/azure-samples/azure-search-openai-javascript) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (10) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 323 · MIT · Sep 2026</sub>

**TypeScript RAG on Azure AI Search with separate indexer and search services.**

The Node.js counterpart of the Azure RAG sample: a search API, an indexer service and a web app that answer chat and Q&A questions over your documents with citations, using Azure AI Search and Azure OpenAI through LangChain.js. azd up provisions Container Apps for the backend and a Static Web App for the frontend, and the search API speaks the AI chat HTTP protocol so the Python backend can replace it. For TypeScript teams on Azure.

- **+** Indexer, search API and web app are separate services with their own deploys
- **+** Search API follows the AI chat HTTP protocol; the backend is swappable
- **+** Tests included; Codespaces and dev container configs
- **−** Cannot run locally until azd up has provisioned Azure resources
- **−** No authentication shipped; Entra setup is a linked tutorial
- **−** Azure OpenAI and Azure AI Search only
- **−** Less active than the Python sample (seed stars 322 vs 7776)

<sub>TypeScript, azure-openai, langchain · Needs azure-subscription, azd, azure-ai-search, azure-openai, azure-blob-storage · GitHub template · [Repo](https://github.com/azure-samples/azure-search-openai-javascript) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-search-openai-javascript/)</sub>

<a name="supabaseauthwithssr"></a>
### #&#8288;9 [SupabaseAuthWithSSR](https://github.com/electriccodeguy/supabaseauthwithssr) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: weak (20) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 397 · MIT · Oct 2026</sub>

**Claude chat on Next.js 16 with Supabase auth, pgvector RAG, cost dashboards.**

A Next.js 16 app on AI SDK v7 and Claude with complete Supabase SSR auth (signup, magic links, password reset, RLS on every table) and eight tools: PDF RAG (Mistral OCR, Voyage embeddings, hybrid RRF search in pgvector), Exa web search, versioned artifacts, memory, conversation search, sandboxed visualizations, PDF export and image generation. Per-step token usage feeds user and admin cost dashboards. For teams shipping a paid Claude assistant on Supabase.

- **+** Whole schema, RLS, triggers and search functions in one idempotent setup.sql
- **+** Per-step token and cache usage stored on messages; user and admin cost dashboards
- **+** Two-tier Anthropic prompt caching with a hit-rate readout
- **+** Live instance at supa-chat.dev; committed within the last day
- **−** Anthropic-only chat; OCR, embeddings and search add Mistral, Voyage and Exa keys
- **−** No tests listed
- **−** Image generation needs your own GPU server (RTX 5090 32 GB recommended)
- **−** One maintainer; large surface area to understand before customizing

<sub>TypeScript, anthropic, ai-sdk, mistral, voyage · Needs supabase, anthropic-api-key, mistral-api-key, voyage-api-key, exa-api-key · env example file · sign-in: Supabase Auth · [Repo](https://github.com/electriccodeguy/supabaseauthwithssr) · [▶️ Demo ↗](https://www.supa-chat.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabaseauthwithssr/)</sub>

<a name="nextjs-openai-doc-search"></a>
### #&#8288;10 [nextjs-openai-doc-search](https://github.com/supabase-community/nextjs-openai-doc-search) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: known (36) · Freshness: recent (73) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · May 2026</sub>

**Build-time embeddings of your MDX docs into Supabase pgvector.**

A Next.js starter that chunks the .mdx files in pages/ at build time, embeds each section with OpenAI and stores vectors in Supabase pgvector, skipping files whose checksum has not changed. At runtime an Edge function embeds the question, runs a similarity search and streams a completion with the matched sections in the prompt; the schema ships as a Supabase migration. For teams adding chat search to a Next.js docs site.

- **+** Checksum table avoids re-embedding unchanged files on every build
- **+** pgvector schema is a checked-in Supabase migration
- **+** One secret (OPENAI_KEY) when deployed with the Vercel Supabase integration
- **−** Uses the legacy OpenAI text completion endpoint; expect to port it
- **−** Only .mdx in pages/ is indexed; other sources need code
- **−** No auth, no conversation history, no tests
- **−** Design dates from 2023; last commit 2026-05

<sub>TypeScript, openai · Needs supabase, postgres-pgvector, openai-api-key, docker-for-local-supabase · env example file · [Repo](https://github.com/supabase-community/nextjs-openai-doc-search) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nextjs-openai-doc-search/)</sub>

<a name="ai-starter-kit"></a>
### #&#8288;11 [ai-starter-kit](https://github.com/sambanova/ai-starter-kit) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (6) · Freshness: active (84) · Maintenance: patchy (46) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 250 · Apache-2.0 · Oct 2026</sub>

**SambaNova Python kits for document RAG, search assistant, function calling.**

Nine Python kits, each with its own README: document text extraction, enterprise and multimodal knowledge retrieval with Streamlit demos, a RAG evaluation kit, a web search assistant, a financial assistant using function calling and scraping, a function-calling module, benchmarking and chat templates. Everything calls SambaNova models through SAMBANOVA_API_KEY. For teams on SambaCloud or SambaStack who want working retrieval code.

- **+** Knowledge retriever and search assistant kits include runnable Streamlit demos
- **+** Makefile base environment installs Python, Poetry, Tesseract and Poppler; Docker option
- **+** RAG evaluation kit included
- **−** SambaNova endpoints only; swapping providers means editing each kit
- **−** README states the code is as-is and not production-ready
- **−** Mixed notebooks and apps; no single app to fork
- **−** Heavy setup: pyenv, Poetry, a parsing service and OCR system packages

<sub>Jupyter Notebook, sambanova, langchain · Needs sambanova-api-key, tesseract, poppler · Docker · [Repo](https://github.com/sambanova/ai-starter-kit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-starter-kit/)</sub>

<a name="natural-language-postgres"></a>
### #&#8288;12 [natural-language-postgres](https://github.com/vercel-labs/natural-language-postgres) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (15) · Freshness: recent (67) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 326 · Apache-2.0 · Apr 2026</sub>

**Next.js text-to-SQL over Postgres with auto-picked charts.**

A Next.js app where the AI SDK and GPT-4o turn a plain-English question into SQL, run it against Postgres, show the rows, pick a chart type and render it with Recharts, and explain the query on request. It ships with a seed script for a unicorn-companies CSV you download yourself; there is no auth and no history. For developers who want a text-to-SQL and charting pattern to copy.

- **+** Shows the full loop: generate SQL, execute, explain, chart config, render
- **+** Deployed demo on Vercel
- **+** Two secrets to run: OPENAI_API_KEY and a Postgres URL
- **−** Single hardcoded dataset; the schema prompt must be rewritten for your tables
- **−** OpenAI GPT-4o only
- **−** No auth, tests or history
- **−** Dataset CSV must be fetched manually from CB Insights

<sub>TypeScript, openai, ai-sdk · Needs postgres, openai-api-key · env example file · [Repo](https://github.com/vercel-labs/natural-language-postgres) · [▶️ Demo ↗](https://natural-language-postgres.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/natural-language-postgres/)</sub>

<a name="openai-support-agent-demo"></a>
### #&#8288;13 [openai-support-agent-demo](https://github.com/openai/openai-support-agent-demo) <sub>score [4](../README.md#-how-we-rank "Score 4/100. Adoption: niche (1) · Freshness: quiet (20) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 204 · MIT · Dec 2025</sub>

**Support console where the model drafts and a human approves.**

A Next.js demo on the OpenAI Responses API with two chat views, one for the customer and one for the human agent. The model drafts replies from a file-search knowledge base, proposes tool calls like cancel_order for the agent to confirm and auto-runs non-sensitive ones like get_order_history; a /init_vs route creates the vector store and functions are placeholders. For teams prototyping agent-assist for support staff.

- **+** Human-in-the-loop pattern is concrete: suggested reply, suggested action, auto-run tiers
- **+** Knowledge base, prompts, tools and demo data each live in one config file
- **+** File search vector store bootstrapped from a route
- **−** README says not production-ready: no auth, no guardrails
- **−** Tool functions are stubs that change nothing
- **−** OpenAI Responses API only
- **−** Last commit 2025-12

<sub>TypeScript, openai · Needs openai-api-key · env example file · [Repo](https://github.com/openai/openai-support-agent-demo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-support-agent-demo/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
