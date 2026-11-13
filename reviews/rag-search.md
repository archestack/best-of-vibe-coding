# 📚 RAG and search reviews · Best of Vibe Coding

Retrieval over your own documents or data, answer engines, and natural-language-to-SQL starters. Back to the [leaderboard](../README.md#-rag-and-search).

<sub>🌐 Also on the web: [RAG and search on archestack.com](https://archestack.com/best-of-vibe-coding/rag-search/), each project on its own page.</sub>

<a name="xerj"></a>
### 🥇 [xerj](https://github.com/xerj-org/xerj) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · Apache-2.0 · Nov 2026</sub>

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
### 🥈 [llm-app](https://github.com/pathwaycom/serviette) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Nov 2026</sub>

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

<a name="sonic"></a>
### 🥉 [sonic](https://github.com/valeriansaliou/sonic) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MPL-2.0 · Oct 2026</sub>

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

<a name="xberg"></a>
### #&#8288;4 [xberg](https://github.com/xberg-io/xberg) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · MIT · Nov 2026</sub>

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

<a name="qmd"></a>
### #&#8288;5 [qmd](https://github.com/tobi/qmd) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Oct 2026</sub>

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

<a name="manticoresearch"></a>
### #&#8288;6 [manticoresearch](https://github.com/manticoresoftware/manticoresearch) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (75) · Freshness: active (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · GPL-3.0 · Nov 2026</sub>

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

<a name="paradedb"></a>
### #&#8288;7 [paradedb](https://github.com/paradedb/paradedb) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · AGPL-3.0 · Nov 2026</sub>

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
### #&#8288;8 [azure-search-openai-demo](https://github.com/azure-samples/azure-search-openai-demo) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

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

<a name="chat-langchain"></a>
### #&#8288;9 [chat-langchain](https://github.com/langchain-ai/chat-langchain) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Nov 2026</sub>

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
### #&#8288;10 [chat-with-your-data-solution-accelerator](https://github.com/azure-samples/chat-with-your-data-solution-accelerator) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

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

<a name="supabaseauthwithssr"></a>
### #&#8288;11 [SupabaseAuthWithSSR](https://github.com/electriccodeguy/supabaseauthwithssr) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 399 · MIT · Oct 2026</sub>

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

<a name="rag-api"></a>
### #&#8288;12 [rag-api](https://github.com/librechat-ai/rag-api) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 926 · MIT · Sep 2026</sub>

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

<a name="orama"></a>
### #&#8288;13 [orama](https://github.com/oramasearch/orama) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: popular (71) · Freshness: recent (77) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Jul 2026</sub>

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

<a name="rag-postgres-openai-python"></a>
### #&#8288;14 [rag-postgres-openai-python](https://github.com/azure-samples/rag-postgres-openai-python) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 512 · MIT · Oct 2026</sub>

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

<a name="azure-search-openai-javascript"></a>
### #&#8288;15 [azure-search-openai-javascript](https://github.com/azure-samples/azure-search-openai-javascript) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 326 · MIT · Oct 2026</sub>

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

<a name="ai-starter-kit"></a>
### #&#8288;16 [ai-starter-kit](https://github.com/sambanova/ai-starter-kit) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (3) · Freshness: active (82) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 251 · Apache-2.0 · Oct 2026</sub>

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

<a name="llm-answer-engine"></a>
### #&#8288;17 [llm-answer-engine](https://github.com/developersdigest/llm-answer-engine) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: known (49) · Freshness: recent (61) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Apr 2026</sub>

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

<a name="nextjs-openai-doc-search"></a>
### #&#8288;18 [nextjs-openai-doc-search](https://github.com/supabase-community/nextjs-openai-doc-search) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: known (32) · Freshness: recent (65) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · May 2026</sub>

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

<a name="natural-language-postgres"></a>
### #&#8288;19 [natural-language-postgres](https://github.com/vercel-labs/natural-language-postgres) <sub>score [20](../README.md#-how-we-rank "Score 20/100. Adoption: niche (9) · Freshness: recent (59) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 331 · Apache-2.0 · Apr 2026</sub>

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
### #&#8288;20 [openai-support-agent-demo](https://github.com/openai/openai-support-agent-demo) <sub>score [4](../README.md#-how-we-rank "Score 4/100. Adoption: niche (1) · Freshness: quiet (12) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 206 · MIT · Dec 2025</sub>

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
