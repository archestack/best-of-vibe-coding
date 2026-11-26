# 📚 RAG and search reviews · Best of Vibe Coding

Retrieval over your own documents or data, answer engines, and natural-language-to-SQL starters. Back to the [leaderboard](../README.md#-rag-and-search).

<sub>🌐 Also on the web: [RAG and search on archestack.com](https://archestack.com/best-of-vibe-coding/rag-search/), each project on its own page.</sub>

<a name="xerj"></a>
### 🥇 [xerj](https://github.com/xerj-org/xerj) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

**Single-binary Rust search engine with Elasticsearch API, MCP server and agent memory.**

XERJ is a Rust search engine that autoindexes folders of code, docs, logs, CSV, SQLite and PDFs for BM25, vector and hybrid search behind an Elasticsearch-compatible API. It also exposes an MCP server and a /_memory namespace API so coding agents can retrieve passages with file:line instead of grepping. Release binaries from rc.101 add XERJ Query-1, a proprietary model that answers questions over stored facts.

- **+** Single Rust binary, no JVM; reports 1448 of 1458 Elasticsearch YAML conformance tests passing
- **+** `xerj autoindex` infers datasets and indexes code with tree-sitter symbols, no schema needed
- **+** Default lexical embedder runs offline; neural embedder is opt-in at about 90 MB download
- **+** Ships MCP tools and /_memory API for agent long-term memory
- **−** XERJ Query-1 and /_facts are absent from the public source; release binaries only
- **−** Query-1 model crates are proprietary; training and evaluation data are not public
- **−** Query-1 mishandles sums and declines all 20 questions on a 95,000-fact namespace
- **−** rc.101 upgrades the data directory to format 4; rc.100 cannot reopen it

<sub>Rust, XERJ Query-1 (release binaries only), lexical embedder (default), neural embedder (opt-in) · [Repo](https://github.com/xerj-org/xerj) · [▶️ Demo ↗](https://xerj.org/playground/) · [📖 Docs ↗](https://xerj.org/docs/) · [🌐 Site ↗](https://xerj.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xerj/)</sub>

<a name="sonic"></a>
### 🥈 [sonic](https://github.com/valeriansaliou/sonic) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MPL-2.0 · Oct 2026</sub>

**Lightweight schema-less search index that returns object IDs, written in Rust.**

Sonic is a Rust search backend that indexes text pushed over its Sonic Channel TCP protocol and returns identifiers, which you resolve against your own database. It supports typo correction, autocomplete suggestions, and stop-word removal for 80+ languages, storing data in RocksDB and FST files. The README reports about 30MB RAM under load and sub-millisecond queries on a 1M-message benchmark.

- **+** README benchmark: ~28MB RAM peak and ~880μs average query on 1M messages
- **+** Built-in typo correction and autocomplete via the suggest operation
- **+** Buckets within collections allow separate per-user indexes
- **+** Official client libraries for NodeJS, Rust and PHP, plus many community ones
- **−** Returns only identifiers; no document storage, so an external database is needed
- **−** No HTTP API; access is only through the Sonic Channel TCP protocol
- **−** master is bug-fix only while a v2 rework is underway
- **−** Pre-built packages target 64-bit Debian 12 only; no semantic or vector search

<sub>Rust · Docker · [Repo](https://github.com/valeriansaliou/sonic) · [▶️ Demo ↗](https://help.crisp.chat/) · [📖 Docs ↗](https://github.com/valeriansaliou/sonic/blob/master/CONFIGURATION.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sonic/)</sub>

<a name="manticoresearch"></a>
### 🥉 [manticoresearch](https://github.com/manticoresoftware/manticoresearch) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · GPL-3.0 · Nov 2026</sub>

**C++ search database with full-text, vector and hybrid search over SQL and HTTP.**

Manticore Search is a C++ search database with SQL (MySQL protocol) and HTTP JSON interfaces, positioned as an Elasticsearch alternative. It combines full-text search, KNN vector search, hybrid queries and auto-embeddings with chunking, and adds conversational search through SQL CALL CHAT. Storage is row-wise or columnar, with real-time inserts, sharded tables and Galera-based multi-master replication.

- **+** Hybrid full-text and KNN retrieval in one query, with auto-embeddings and chunking
- **+** Speaks MySQL protocol and HTTP JSON; official clients for nine languages
- **+** Columnar storage for datasets larger than RAM; about 40MB RSS when empty
- **+** Replication, sharded tables, built-in auth, backup to S3-compatible storage
- **−** GPL-3.0 licence may constrain embedding in proprietary products
- **−** Not fully ACID; only isolated transactions and binary logging
- **−** Elasticsearch compatibility covers writes only, not the full query API
- **−** Benchmark claims come from the project's own suite and are workload-specific

<sub>C++, auto-embeddings, LLM-backed CALL CHAT · Needs Manticore Columnar Library (columnar storage), LLM provider (conversational search) · [Repo](https://github.com/manticoresoftware/manticoresearch) · [▶️ Demo ↗](https://play.manticoresearch.com) · [📖 Docs ↗](https://manual.manticoresearch.com) · [🌐 Site ↗](https://manticoresearch.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/manticoresearch/)</sub>

<a name="xberg"></a>
### #&#8288;4 [xberg](https://github.com/xberg-io/xberg) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · MIT · Nov 2026</sub>

**Rust document extraction engine with OCR, tables and 15 language bindings.**

Xberg is a Rust engine that detects and reads 107 document formats (PDF, Office, images, email, archives, audio, URLs, source code) and returns text, tables, metadata or schema-driven JSON. It adds OCR backends, layout and table models, chunking and embeddings, and runs as a library, a 14-command CLI, a REST server or an MCP server. It is the v1 rebrand of Kreuzberg.

- **+** 107 formats, including nested archives guarded by zip-bomb and depth limits
- **+** OCR via Tesseract, PaddleOCR, Candle or VLM backends with fallback chains
- **+** Bindings for 15 languages plus CLI, REST (`xberg serve`) and MCP stdio server
- **+** MIT license; CPU by default, no GPU required, with content-hash caching
- **−** URL ingestion, transcription and reranker need Cargo features in from-source builds
- **−** Structured extraction needs an external LLM such as Ollama, vLLM or a hosted API
- **−** v1 rebrand of Kreuzberg; migration path from the old package is not described
- **−** Bindings are generated by alef, so each language package depends on that toolchain

<sub>Rust, Whisper ONNX (tiny to large-v3), PaddleOCR, PP-DocLayout-V3, RT-DETR · Needs Tesseract (optional OCR backend), Ollama, LM Studio, vLLM or hosted LLM (structured extraction) · Docker · [Repo](https://github.com/xberg-io/xberg) · [▶️ Demo ↗](https://docs.xberg.io/demo.html) · [📖 Docs ↗](https://docs.xberg.io) · [🌐 Site ↗](https://xberg.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xberg/)</sub>

<a name="auto-ontology"></a>
### #&#8288;5 [auto-ontology](https://github.com/nvidia/auto-ontology) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**Ontology layer that grounds text-to-SQL agents in certified business definitions.**

Generates an ontology of terms, SQL attributes and relationships from database metadata, stores it in Postgres with pgvector, and uses it to answer natural-language questions with SQL and provenance. It ships a Next.js web UI, FastAPI backend and ingestion services, plus an MCP server, REST API and agent skills. Inference defaults to NVIDIA NIM endpoints; self-hosted or OpenAI-compatible endpoints can be set per model role.

- **+** Connects to ten engines including Postgres, Snowflake, Databricks, ClickHouse, DuckDB and SQLite
- **+** Each answer returns its SQL and steps; check_answerable flags questions the data cannot cover
- **+** Read-only MCP server and streaming REST API work with Cursor and Claude Desktop
- **+** Imports and exports semantic models as Apache Ossie YAML
- **−** Ingestion service has no authentication; ports 3001 and 3002 must stay private
- **−** Defaults need an NVIDIA API key unless each model role points elsewhere
- **−** Project is not accepting external contributions
- **−** Quickstart needs a second repo (auto-ontology-eval) and uv to seed the sample database

<sub>Python, NVIDIA NIM (Nemotron), OpenAI-compatible endpoints, self-hosted NIM · Needs PostgreSQL 17 with pgvector, NVIDIA NIM endpoint or OpenAI-compatible LLM, Docker Compose or Kubernetes (Helm), HashiCorp Vault (optional) · Docker · env example file · [Repo](https://github.com/nvidia/auto-ontology) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auto-ontology/)</sub>

<a name="paradedb"></a>
### #&#8288;6 [paradedb](https://github.com/paradedb/paradedb) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · AGPL-3.0 · Nov 2026</sub>

**Postgres extension adding BM25 full-text, vector and hybrid search.**

ParadeDB is a Rust Postgres extension that adds a custom index for BM25 full-text search, vector search, filters, facets, aggregations and joins. Search runs inside Postgres with standard SQL and ACID transactions, so no separate search engine is needed. It builds on pgrx, Tantivy and Apache DataFusion, and offers ORM integrations plus agent skills and MCP docs.

- **+** Search and application data share one Postgres with ACID transactions
- **+** Covers BM25, vector and hybrid search, facets and aggregates in SQL
- **+** ORM integrations for Drizzle, Django, SQLAlchemy, Rails and EF Core
- **+** Built on Tantivy and DataFusion rather than a custom engine
- **−** Community edition is AGPL-3.0; Enterprise needs a commercial license
- **−** Self-hosting Enterprise requires contacting sales
- **−** No embedding or document ingestion pipeline included
- **−** Prisma integration is not yet available

<sub>Rust · Needs PostgreSQL · Docker · [Repo](https://github.com/paradedb/paradedb) · [📖 Docs ↗](https://www.paradedb.com/docs/start/introduction) · [🌐 Site ↗](https://paradedb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/paradedb/)</sub>

<a name="azure-search-openai-demo"></a>
### #&#8288;7 [azure-search-openai-demo](https://github.com/azure-samples/azure-search-openai-demo) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

**RAG chat app over your documents using Azure OpenAI and Azure AI Search.**

Python backend with a web frontend that answers questions over your own documents using Azure OpenAI (gpt-5.4-mini in the sample) and Azure AI Search. It shows citations and the thought process for each answer and exposes retrieval settings in the UI. Deployment uses the Azure Developer CLI (`azd up`), which provisions resources and indexes the sample Zava data.

- **+** Multi-turn chat with citations and per-answer thought process
- **+** UI settings let you tweak prompts and retrieval options while testing
- **+** Optional multimodal, speech, Entra login with access control, and Cosmos DB chat history
- **+** Includes sample data plus docs on evaluation, monitoring and productionizing
- **−** Tied to Azure services; no other model or search providers listed
- **−** azd up provisions paid resources, mainly AI Search, that bill immediately
- **−** README advises against production use without extra security work
- **−** Deploying needs Azure role assignment and deployment write permissions

<sub>Python, Azure OpenAI GPT (gpt-5.4-mini) · Needs Azure OpenAI, Azure AI Search, Azure Blob Storage, Azure AI Document Intelligence, Azure Container Apps, Azure Developer CLI, Azure Cosmos DB (optional) · [Repo](https://github.com/azure-samples/azure-search-openai-demo) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/python/get-started-app-chat-template?toc=%2Fazure%2Fdeveloper%2Fai%2Ftoc.json&bc=%2Fazure%2Fdeveloper%2Fai%2Fbreadcrumb%2Ftoc.json&tabs=github-codespaces) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-search-openai-demo/)</sub>

<a name="qmd"></a>
### #&#8288;8 [qmd](https://github.com/tobi/qmd) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Nov 2026</sub>

**Local hybrid search over markdown notes and docs, with CLI and MCP server.**

QMD indexes markdown notes, transcripts and docs into a SQLite store and searches them with BM25 (FTS5), vector search and LLM reranking. Models run locally as GGUF through node-llama-cpp. It ships a CLI with JSON and file-list output for agents, an MCP server over stdio or HTTP (default port 8181), and a Node/Bun SDK.

- **+** Hybrid pipeline: query expansion, BM25 plus vector search, RRF fusion, then LLM reranking
- **+** Runs on-device with GGUF models via node-llama-cpp; no hosted API needed
- **+** CLI, MCP server (stdio or HTTP) and TypeScript SDK available
- **+** HTTP server rejects non-loopback Origin and Host headers to block DNS rebinding
- **−** HTTP endpoints are unauthenticated; off-host use needs your own auth in front
- **−** Built around markdown and text; other document formats are not mentioned
- **−** Embedding step must run before semantic search works

<sub>TypeScript, GGUF, qwen3-reranker · Needs Node.js or Bun, node-llama-cpp, SQLite · [Repo](https://github.com/tobi/qmd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qmd/)</sub>

<a name="llm-app"></a>
### #&#8288;9 [llm-app](https://github.com/pathwaycom/serviette) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Nov 2026</sub>

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

<a name="zvec-grep"></a>
### #&#8288;10 [zvec-grep](https://github.com/zvec-ai/zvec-grep) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · Apache-2.0 · Nov 2026</sub>

**Local CLI combining ripgrep, BM25 and vector search over code and documents.**

zg indexes a project into a .zvec-grep/ directory and searches it with exact text or regex, BM25 full-text, and vector retrieval, using the zvec engine. It can be run from the terminal or installed as a search tool for agents such as OpenCode (`zg --install --target opencode`). Results are ranked and linked to source locations; code is indexed with symbols and signatures, prose as sections and chunks.

- **+** Hybrid, FTS and vector queries in one CLI, with repeatable flags for multiple queries
- **+** Local embedding model option (local/potion-retrieval-32m); files and indexes stay on the machine
- **+** Same index serves terminal use and agent integration on macOS, Linux and Windows
- **+** Benchmarks with paired A/B runs and reproduction docs are published in the repo
- **−** Agent benefit varies by model and run, per the README's own caveat
- **−** Remote embeddings send data off-machine when enabled
- **−** Index lives in .zvec-grep/ per project and must be built before searching
- **−** Agent integration documented only for OpenCode in the README

<sub>Rust, local/potion-retrieval-32m, Qwen3.7 Text Embedding · Needs Node.js/npm for install, zvec · [Repo](https://github.com/zvec-ai/zvec-grep) · [📖 Docs ↗](https://zvec.org/en/docs/zvec-grep/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zvec-grep/)</sub>

<a name="chinese-poetry-api"></a>
### #&#8288;11 [chinese-poetry-api](https://github.com/palemoky/chinese-poetry-api) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · GPL-3.0 · Nov 2026</sub>

**Chinese classical poetry API with REST, GraphQL, MCP and optional semantic search.**

Go service that serves about 400,000 Chinese poems (Tang poetry, Song ci, Yuan qu and more) from SQLite with FTS5 search. It exposes REST with an OpenAPI document, GraphQL and a read-only MCP endpoint, and stores simplified and traditional text together, switched by `?lang=`. Optional semantic search uses a bge-m3 vector file plus any OpenAI-compatible embeddings endpoint.

- **+** Three interfaces on one port: REST with OpenAPI 3.2, GraphQL and MCP over Streamable HTTP
- **+** Simplified and traditional Chinese from one database via the lang parameter
- **+** Semantic search is optional; the service runs normally without the vector file
- **+** Built-in IP rate limiting and multi-arch Docker image (amd64/arm64)
- **−** Semantic search needs a roughly 200MB vector file and an external embeddings API
- **−** Semantic search adds about 350MB resident memory and a 2-second startup load
- **−** Building with plain `go` requires the `sqlite_fts5` tag, or search fails
- **−** Documentation is in Chinese only; the dataset comes in via git submodules

<sub>Go, bge-m3 · Needs SQLite with FTS5, Ollama or OpenAI-compatible embeddings API (optional, semantic search), Git submodules (dataset) · Docker · env example file · [Repo](https://github.com/palemoky/chinese-poetry-api) · [▶️ Demo ↗](https://poetry.palemoky.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chinese-poetry-api/)</sub>

<a name="chat-langchain"></a>
### #&#8288;12 [chat-langchain](https://github.com/langchain-ai/chat-langchain) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Nov 2026</sub>

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

<sub>Python, Anthropic (or another provider) · Needs Managed Deep Agents (mda), Supabase, Pylon, LangSmith, Anthropic API key (or another provider) · env example file · [Repo](https://github.com/langchain-ai/chat-langchain) · [📖 Docs ↗](https://docs.langchain.com/oss/python/langchain/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-langchain/)</sub>

<a name="rag-api"></a>
### #&#8288;13 [rag-api](https://github.com/librechat-ai/rag-api) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 928 · MIT · Nov 2026</sub>

**FastAPI service for per-file document embedding and retrieval on pgvector.**

Async FastAPI and Langchain service that ingests documents, embeds them under a file_id, and answers similarity queries against pgvector or Atlas MongoDB. Built mainly as the RAG backend for LibreChat, but usable for any ID-based retrieval. Reads and deletes are scoped to an owner taken from a verified JWT.

- **+** Many embedding providers: OpenAI, Azure, Bedrock, Google GenAI, VertexAI, Hugging Face, TEI, Ollama
- **+** Reads and deletes are scoped by JWT owner before ranking
- **+** Batched async ingestion with bounded memory and rollback on failure
- **+** Optional RAG_DISTANCE_THRESHOLD drops weak matches to cut downstream LLM tokens
- **−** entity_id is caller-asserted; untrusted callers need upstream authorization
- **−** Upgrading the service before the client orphans agent knowledge-base files on delete
- **−** Chunks with no user_id become unreadable after upgrade unless backfilled with SQL
- **−** Omitting JWT_SECRET disables authentication and stamps all chunks as public

<sub>Python, OpenAI, Azure OpenAI, AWS Bedrock, Google GenAI · Needs PostgreSQL with pgvector (or Atlas MongoDB), Embedding provider API (OpenAI by default) · Docker · [Repo](https://github.com/librechat-ai/rag-api) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rag-api/)</sub>

<a name="chat-with-your-data-solution-accelerator"></a>
### #&#8288;14 [chat-with-your-data-solution-accelerator](https://github.com/azure-samples/chat-with-your-data-solution-accelerator) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (32) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

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

<a name="launchstack"></a>
### #&#8288;15 [launchstack](https://github.com/deodat-lawson/launchstack) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (25) · Freshness: active (97) · Maintenance: patchy (39) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 898 · Apache-2.0 · Nov 2026</sub>

**TypeScript engine for document ingestion, OCR, hybrid RAG and knowledge graphs.**

Launchstack is a pnpm monorepo of TypeScript packages for ingestion, OCR, chunking, embeddings, hybrid retrieval with reranking, Neo4j entity sync and background jobs. A Next.js reference app and a durable worker wire them to Postgres with pgvector and S3-style storage. Chat goes through one OpenAI-compatible endpoint configured by YAML.

- **+** Two-command self-host installer generates secrets and sets up HTTPS for a domain
- **+** Lite stack uses about 400MB RAM; Docling OCR profile adds about 1.2GB
- **+** Lint-enforced boundaries keep engine bricks independent of Next.js and the host app
- **+** Permission-scoped citations and hybrid retrieval with reranking, backed by Postgres with pgvector
- **−** Packages are not on npm yet; consuming them means running this repository
- **−** Embeddings have no default; uploads are never searchable until a key is set
- **−** Needs a separate worker process, or uploaded documents stay queued
- **−** Wiring the engine into your own host takes seven separate registration calls

<sub>TypeScript, Gemini, Azure OpenAI, OpenAI-compatible chat endpoints, OpenAI-compatible embeddings · Needs Postgres with pgvector, S3-compatible storage, Neo4j (optional), Docling (optional OCR), Inngest (optional) · env example file · [Repo](https://github.com/deodat-lawson/launchstack) · [🌐 Site ↗](https://launchstack.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/launchstack/)</sub>

<a name="langchainrb"></a>
### #&#8288;16 [langchainrb](https://github.com/patterns-ai-core/langchainrb) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (44) · Freshness: recent (70) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Ruby library for LLM calls, RAG, vector search and tool-using assistants.**

Langchain.rb is a Ruby gem that wraps LLM providers behind one interface for embeddings, completions and chat. It adds prompt templates, output parsers, a vector search layer over eight databases, and an Assistant class that runs tools and keeps conversation threads. Rails integration lives in a separate gem, langchainrb_rails.

- **+** One LLM interface across 11 providers, including Anthropic, OpenAI, Gemini, Bedrock and Ollama
- **+** Vector search wrappers for Chroma, Hnswlib, Milvus, Pinecone, Pgvector, Qdrant, Weaviate, Elasticsearch
- **+** Loads docx, html, pdf, text, json, jsonl, csv, xlsx, eml and pptx into the index
- **+** Assistant class handles tool calls, image input and streaming for some providers
- **−** Provider and vector DB client gems are not bundled and must be added by hand
- **−** Streaming is not supported for all LLMs
- **−** Last release was 2025-05-01, well behind recent commits
- **−** Ruby only, and Rails integration needs a separate gem

<sub>Ruby, Anthropic, AWS Bedrock, Azure OpenAI, Cohere · Needs Ruby, LLM provider API key or Ollama, vector database client gem (optional) · env example file · [Repo](https://github.com/patterns-ai-core/langchainrb) · [📖 Docs ↗](http://rubydoc.info/gems/langchainrb) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/langchainrb/)</sub>

<a name="orama"></a>
### #&#8288;17 [orama](https://github.com/oramasearch/orama) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: popular (79) · Freshness: recent (72) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Jul 2026</sub>

**In-process full-text, vector and hybrid search library for JavaScript.**

Orama is a TypeScript search engine that runs in the browser, Node, Deno or Bun. It indexes documents against a typed schema and supports BM25 full-text, vector and hybrid search, plus filters, facets, geosearch and typo tolerance. An AnswerSession API builds RAG chat on top, calling OpenAI through an optional secure proxy plugin.

- **+** Runs in-process in browser, Node, Deno and Bun with no server required
- **+** Full-text, vector and hybrid modes in one API with BM25, facets and geosearch
- **+** Stemming and tokenization for 30 languages
- **+** Plugin system with official plugins for embeddings, persistence, Docusaurus, Astro and Nextra
- **−** Index lives in memory; persistence needs a separate plugin
- **−** Vector search needs embeddings supplied or generated via a plugin
- **−** Chat answers depend on OpenAI models via the secure proxy plugin
- **−** Library only, not a standalone search server with its own HTTP API

<sub>TypeScript, OpenAI chat models via secure proxy (e.g. gpt-4o-mini), TensorFlow.js embeddings (512-dimension) · Needs OpenAI API (optional, for chat answers), TensorFlow.js (optional, for embeddings plugin) · [Repo](https://github.com/oramasearch/orama) · [📖 Docs ↗](https://docs.orama.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orama/)</sub>

<a name="supabaseauthwithssr"></a>
### #&#8288;18 [SupabaseAuthWithSSR](https://github.com/electriccodeguy/supabaseauthwithssr) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 397 · MIT · Oct 2026</sub>

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

<a name="llm-apps-java-spring-ai"></a>
### #&#8288;19 [llm-apps-java-spring-ai](https://github.com/thomasvitale/llm-apps-java-spring-ai) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: weak (27) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 790 · Apache-2.0 · Nov 2026</sub>

**Spring AI sample projects for chat, RAG, tool calling and observability in Java.**

A collection of small Java 25 sample applications built on Spring AI. Each folder covers one topic: chat models, embeddings, prompts, structured output, tool calling, chat memory, guardrails, document ingestion, several RAG flows and LLM observability. Most samples use Ollama, some have Mistral AI and OpenAI variants, and retrieval samples use PGVector.

- **+** Covers sequential, branching and conditional RAG flows with Ollama and PGVector
- **+** Same pattern often shown for Ollama, OpenAI and Mistral AI side by side
- **+** Includes chat memory variants: in-memory, JDBC, Spring Security, vector store
- **+** Includes observability samples for models and PGVector
- **−** Separate sample modules, not one forkable app with auth or billing
- **−** Vector stores, evaluation and agents sections are marked coming soon
- **−** Requires Java 25, which many teams have not adopted
- **−** Only PGVector is shown as a vector store

<sub>Java, Ollama, OpenAI, Mistral AI, ONNX Transformers · Needs Java 25, Podman or Docker, Ollama, PGVector · [Repo](https://github.com/thomasvitale/llm-apps-java-spring-ai) · [📖 Docs ↗](https://docs.spring.io/spring-ai/reference/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llm-apps-java-spring-ai/)</sub>

<a name="rag-postgres-openai-python"></a>
### #&#8288;20 [rag-postgres-openai-python](https://github.com/azure-samples/rag-postgres-openai-python) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 512 · MIT · Oct 2026</sub>

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

<a name="serverless-chat-langchainjs"></a>
### #&#8288;21 [serverless-chat-langchainjs](https://github.com/azure-samples/serverless-chat-langchainjs) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 869 · MIT · Oct 2026</sub>

**RAG chatbot sample on Azure Functions, Cosmos DB and LangChain.js.**

A TypeScript sample that answers questions over PDF documents using LangChain.js, with a Lit chat web component on Azure Static Web Apps and an Azure Functions API. Azure Cosmos DB for NoSQL stores vectors and per-user chat history, and Blob Storage holds the source files. It runs against Azure OpenAI or locally with Ollama (llama3.1 and nomic-embed-text).

- **+** Full path wired: ingestion, vector store, retrieval, chat history and web UI
- **+** Runs locally with Ollama, so no cloud cost for testing
- **+** One-command Azure deploy with azd up, plus optional CI/CD via azd pipeline config
- **+** Uses the HTTP protocol for AI chat apps between web app and API
- **−** Tied to Azure services: Functions, Static Web Apps, Cosmos DB, Blob Storage
- **−** Azure deploy needs Azure OpenAI access and role-assignment permissions
- **−** Local Ollama models may not follow citation and follow-up question formatting
- **−** Sample data is a fictitious company; ingestion is shown for PDFs in /data

<sub>TypeScript, Azure OpenAI, Ollama llama3.1, Ollama nomic-embed-text · Needs Azure Static Web Apps, Azure Functions, Azure Cosmos DB for NoSQL, Azure Blob Storage, Azure OpenAI, Azure Developer CLI, Node.js 20+, Ollama (local mode) · [Repo](https://github.com/azure-samples/serverless-chat-langchainjs) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/javascript/ai/get-started-app-chat-template-langchainjs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless-chat-langchainjs/)</sub>

<a name="generativeaiexamples"></a>
### #&#8288;22 [generativeaiexamples](https://github.com/nvidia/generativeaiexamples) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (58) · Freshness: recent (70) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · Apache-2.0 · Sep 2026</sub>

**NVIDIA notebooks and sample apps for RAG, agents and NeMo microservices.**

A collection of Jupyter notebooks and example apps showing how to use NVIDIA NIM microservices, NeMo microservices and the NVIDIA API Catalog with LangChain, LlamaIndex and Haystack. It covers basic and advanced RAG (multi-turn, multimodal, CSV, query decomposition), tool-calling fine-tuning, guardrails and vision NIM workflows. The basic RAG example runs with docker compose and a playground UI on port 8090.

- **+** Covers basic and advanced RAG: multi-turn, multimodal, CSV data, query decomposition
- **+** Examples use LangChain, LlamaIndex and Haystack integrations
- **+** Defaults to hosted NVIDIA API Catalog endpoints; local NIM deployment is documented
- **+** Includes NeMo tutorials for fine-tuning, evaluation, guardrails and auditing
- **−** Tied to NVIDIA NIM, NeMo and API Catalog; not vendor-neutral
- **−** Mostly notebooks and reference examples, not a deployable product
- **−** Last tagged release is 2024-08-21; some links point to old v0.7.0
- **−** Several examples need an NVIDIA API key or NeMo microservices on Kubernetes

<sub>Jupyter Notebook, NVIDIA NIM endpoints, Llama 3.1, Llama-3.2-1B-Instruct, NV-CLIP · Needs NVIDIA API Catalog key, Docker Compose, NVIDIA NIM, NVIDIA NeMo Microservices, Milvus · [Repo](https://github.com/nvidia/generativeaiexamples) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/generativeaiexamples/)</sub>

<a name="ai-starter-kit"></a>
### #&#8288;23 [ai-starter-kit](https://github.com/sambanova/ai-starter-kit) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (2) · Freshness: active (81) · Maintenance: patchy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 251 · Apache-2.0 · Nov 2026</sub>

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

<a name="azure-search-openai-javascript"></a>
### #&#8288;24 [azure-search-openai-javascript](https://github.com/azure-samples/azure-search-openai-javascript) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 327 · MIT · Oct 2026</sub>

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

<a name="llm-answer-engine"></a>
### #&#8288;25 [llm-answer-engine](https://github.com/developersdigest/llm-answer-engine) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: popular (63) · Freshness: recent (56) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Apr 2026</sub>

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

<a name="ragbits"></a>
### #&#8288;26 [ragbits](https://github.com/deepsense-ai/ragbits) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: known (38) · Freshness: recent (68) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · May 2026</sub>

**Modular Python toolkit for LLM prompts, RAG ingestion, agents and chat APIs.**

Ragbits is a set of Python packages for building GenAI apps: typed prompts and LLM calls through LiteLLM, document ingestion and search over pluggable vector stores, agents with MCP and A2A, and a chat API with a UI. Packages install separately or as the `ragbits` bundle, and `create-ragbits-app` scaffolds projects from templates.

- **+** Typed prompts using Python generics and Pydantic input models
- **+** Ingests 20+ formats via Docling or Unstructured, with S3, GCS and Azure connectors
- **+** Ray-based distributed ingestion for large datasets
- **+** Separate packages for core, agents, search, evaluation, guardrails and chat
- **−** Library, not a deployable app; you write the Python wiring yourself
- **−** Python only
- **−** Quickstarts assume hosted OpenAI models; local model setup is in separate docs
- **−** Broad scope across prompts, RAG, agents and chat means many packages to learn

<sub>Python, 100+ LLMs via LiteLLM, local models, OpenAI · Needs LiteLLM, Qdrant, PgVector, Ray, Docling, Unstructured, OpenTelemetry, promptfoo · [Repo](https://github.com/deepsense-ai/ragbits) · [📖 Docs ↗](https://ragbits.deepsense.ai) · [🌐 Site ↗](https://deepsense.ai/rd-hub/ragbits/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ragbits/)</sub>

<a name="nano-graphrag"></a>
### #&#8288;27 [nano-graphrag](https://github.com/gusye1234/nano-graphrag) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (55) · Freshness: quiet (16) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Jan 2026</sub>

**Compact Python GraphRAG library with swappable LLM, vector and graph storage.**

nano-graphrag is a Python library that builds a knowledge graph from text, generates community reports, and answers queries in global, local or naive RAG modes. The core is about 1100 lines excluding tests and prompts, with async methods and type hints. LLMs, embeddings, vector stores and graph storage can be replaced with your own implementations.

- **+** About 1100 lines of core code, easy to read and modify
- **+** Pluggable storage: nano-vectordb, hnswlib, milvus-lite, faiss, networkx, Neo4j
- **+** Runs on OpenAI, Azure OpenAI, Bedrock, DeepSeek or ollama with local embeddings
- **+** Incremental insert dedupes chunks by md5 hash; async variant of every method
- **−** Does not implement the covariates feature of the original GraphRAG
- **−** Global search uses only top-K communities (default 512), unlike the original
- **−** Each insert recomputes communities and regenerates community reports
- **−** Library only, no server or UI; last release was 2024-10-01

<sub>Python, OpenAI, Azure OpenAI, Amazon Bedrock, DeepSeek · Needs OpenAI API key (default), Neo4j (optional) · [Repo](https://github.com/gusye1234/nano-graphrag) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nano-graphrag/)</sub>

<a name="nextjs-openai-doc-search"></a>
### #&#8288;28 [nextjs-openai-doc-search](https://github.com/supabase-community/nextjs-openai-doc-search) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: known (40) · Freshness: recent (61) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · May 2026</sub>

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

<a name="azure-search-openai-demo-csharp"></a>
### #&#8288;29 [azure-search-openai-demo-csharp](https://github.com/azure-samples/azure-search-openai-demo-csharp) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (19) · Freshness: recent (70) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 846 · MIT · Oct 2026</sub>

**.NET RAG chat sample over your documents with Azure OpenAI and AI Search.**

A C# reference app that answers questions over your own documents using Azure OpenAI (gpt-4o-mini) and Azure AI Search, orchestrated with Semantic Kernel. It ships a Blazor WebAssembly frontend, an ASP.NET Core Minimal API backend, and a .NET MAUI client, with Contoso Electronics sample data. Provisioning and deployment to Azure Container Apps run through azd and Bicep.

- **+** End-to-end sample: azd up provisions Azure resources, indexes ./data, and deploys the app
- **+** Includes Chat, Q&A and Voice Chat pages, with citations and in-UI settings
- **+** Blazor web client plus a .NET MAUI Blazor Hybrid client sharing code
- **+** Optional Application Insights tracing, authentication and GPT-4V support
- **−** Tied to Azure OpenAI, AI Search, Blob Storage and Document Intelligence; no other providers
- **−** Deployed app has no authentication by default; must be enabled separately
- **−** Default resources incur monthly cost; free SKUs have limits such as 2 pages per document
- **−** Needs Azure role-assignment permissions, plus Docker and azd locally

<sub>C#, gpt-4o-mini, Azure OpenAI embedding model, GPT-4V (optional) · Needs Azure OpenAI Service, Azure AI Search, Azure Blob Storage, Azure AI Document Intelligence, Azure Container Apps, Azure Developer CLI, Docker · [Repo](https://github.com/azure-samples/azure-search-openai-demo-csharp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-search-openai-demo-csharp/)</sub>

<a name="lightningrag"></a>
### #&#8288;30 [lightningrag](https://github.com/lightningrag/lightningrag) <sub>score [22](../README.md#-how-we-rank "Score 22/100. Adoption: niche (10) · Freshness: recent (63) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 456 · Apache-2.0 · Apr 2026</sub>

**Go and Vue RAG platform with knowledge bases, agent canvas and admin UI.**

LightningRAG is a Gin (Go) and Vue full-stack app that parses, chunks and embeds documents into pgvector or Elasticsearch, then serves chat and SSE streaming APIs with optional references. It adds a canvas for agent flows (Begin, Retrieval, LLM, Message, Agent nodes) and webhook connectors for Feishu, DingTalk, Slack and others. The admin layer provides JWT, Casbin, dynamic menus and code generation.

- **+** Retrievers include vector, keyword and PageIndex, with optional reranking per request
- **+** Webhook connectors bind published agents to Feishu, DingTalk, Slack, Teams, Telegram and more
- **+** Web UI can be embedded into a single Go binary via go:embed
- **+** Admin features included: JWT, Casbin roles, dynamic menus, Swagger docs
- **−** Needs MySQL, Redis and a vector store, so setup involves several services
- **−** No public demo; the README's demo link is struck out as not deployed
- **−** Much of the README covers generic admin-framework features unrelated to RAG
- **−** Removing copyright notices requires a separate license despite Apache-2.0

<sub>Go, Pluggable LLM, embedding, rerank, speech, TTS, OCR providers (list in server/rag/README.md) · Needs MySQL > 5.7, Redis, PostgreSQL with pgvector or Elasticsearch, Node > 18.16, Go >= 1.22 · Docker · [Repo](https://github.com/lightningrag/lightningrag) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lightningrag/)</sub>

<a name="natural-language-postgres"></a>
### #&#8288;31 [natural-language-postgres](https://github.com/vercel-labs/natural-language-postgres) <sub>score [18](../README.md#-how-we-rank "Score 18/100. Adoption: niche (5) · Freshness: recent (55) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 333 · Apache-2.0 · Apr 2026</sub>

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

<a name="vectordb"></a>
### #&#8288;32 [vectordb](https://github.com/epsilla-cloud/vectordb) <sub>score [7](../README.md#-how-we-rank "Score 7/100. Adoption: niche (23) · Freshness: quiet (0) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 873 · Apache-2.0 · Nov 2025</sub>

**C++ vector database with REST API and Python, JavaScript and Ruby clients.**

Epsilla is a vector database written in C++ that stores vectors as a field type in tables, with metadata filtering and hybrid search over dense and sparse vectors. It can embed text on insert and query, and exposes a REST API on port 8888 plus Python, JavaScript and Ruby clients. The README claims indexing about 10x faster than HNSW at over 99.9% precision, without published benchmarks.

- **+** Table, field and primary-key model, with vectors as just another field type
- **+** Hybrid dense and sparse search with metadata filtering
- **+** Built-in embedding lets you insert and query with plain text
- **+** LangChain and LlamaIndex integrations plus Python, JavaScript and Ruby clients
- **−** Speed and precision claims come from the README with no benchmark data shown
- **−** Embedded Python library mode is marked experimental and needs a manual C++ build
- **−** Last release was March 2025, so tagged releases trail recent commits
- **−** Cloud-native features like serverless and multi-tenancy are described for the hosted service

<sub>C++ · [Repo](https://github.com/epsilla-cloud/vectordb) · [📖 Docs ↗](https://epsilla-inc.gitbook.io/epsilladb/) · [🌐 Site ↗](https://cloud.epsilla.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vectordb/)</sub>

<a name="openai-support-agent-demo"></a>
### #&#8288;33 [openai-support-agent-demo](https://github.com/openai/openai-support-agent-demo) <sub>score [2](../README.md#-how-we-rank "Score 2/100. Adoption: niche (0) · Freshness: quiet (7) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 209 · MIT · Dec 2025</sub>

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
