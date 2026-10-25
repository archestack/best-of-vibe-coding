# 🔌 MCP servers for developers reviews · Best of Vibe Coding

MCP servers that give coding agents tools: docs lookup, browsers, GitHub, databases and code navigation. Back to the [leaderboard](../README.md#-mcp-servers-for-developers).

<sub>🌐 Also on the web: [MCP servers for developers on archestack.com](https://archestack.com/best-of-vibe-coding/dev-mcp/), each project on its own page.</sub>

<a name="codegraph"></a>
### 🥇 [codegraph](https://github.com/colbymchenry/codegraph) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

**Local code knowledge graph that coding agents query over MCP.**

CodeGraph indexes a project into a local `.codegraph/` graph of symbols, call edges and dependencies, then exposes it to coding agents through an MCP server. Agents can fetch relevant source, call paths and change impact in one call instead of grepping and reading files. `codegraph install` wires it into Claude Code, Cursor, Codex, opencode, Gemini, Kiro, Copilot and others; the index auto-syncs on file changes.

- **+** Auto-configures nine agents with one `codegraph install` command
- **+** Index stays current by watching files; no manual re-indexing
- **+** Covers about 35 languages with cross-file resolution in one graph
- **+** Benchmarks published with method: 7 repos, median of 4 runs, CLI blocked in both arms
- **−** Benchmark figures come from the author and use one model, Claude Opus 4.8
- **−** README says responses leave about 80% more context resident in long sessions
- **−** Must run `codegraph init` in every project to build its graph
- **−** Hosted CodeGraph platform is a waitlist product, separate from this tool

<sub>no GPU · Models: Claude Code, Cursor, Codex CLI, opencode, Hermes Agent · safety checks passed 14 of 16 · [Repo](https://github.com/colbymchenry/codegraph) · [📖 Docs ↗](https://colbymchenry.github.io/codegraph/) · [🌐 Site ↗](https://colbymchenry.github.io/codegraph/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegraph/)</sub>

<a name="gitnexus"></a>
### 🥈 [gitnexus](https://github.com/abhigyanpatwari/gitnexus) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · custom license · Oct 2026</sub>

**Code knowledge graph exposed to coding agents through MCP tools.**

GitNexus indexes a repository with Tree-sitter into a knowledge graph of dependencies, call chains, clusters and execution flows, stored in LadybugDB. It exposes 19 MCP tools (impact, trace, detect_changes, rename, cypher and others) plus agent skills and hooks for Claude Code, Cursor, Codex and similar editors. A browser Web UI adds graph exploration and chat.

- **+** Precomputes clusters and flows at index time, so one tool call returns impact context
- **+** 19 MCP tools including impact, trace, detect_changes, rename and raw Cypher
- **+** One setup command writes MCP config for Claude Code, Cursor, Codex, Antigravity and others
- **+** Installs agent skills and Claude Code and Codex pre/post tool hooks
- **−** PolyForm Noncommercial license restricts commercial use
- **−** In-browser Web UI mode is limited to roughly 5k files
- **−** npm 11 install crash and native grammar builds complicate installation
- **−** Render deploy costs about $35/month; the access token is the only control

<sub>RAM ≥ 2 GB · GPU optional · Docker + Compose · Needs Node.js, LadybugDB, Tree-sitter · safety checks passed 12 of 18 · [Repo](https://github.com/abhigyanpatwari/gitnexus) · [▶️ Demo ↗](https://gitnexus.vercel.app) · [🌐 Site ↗](https://gitnexus.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitnexus/)</sub>

<a name="serena"></a>
### 🥉 [serena](https://github.com/oraios/serena) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · custom license · Oct 2026</sub>

**MCP server giving coding agents symbol-level code search, editing and refactoring.**

Serena is an MCP server that exposes IDE-style tools to coding agents: find symbol, find referencing symbols, symbol-body replacement, rename, and a memory system. It uses language servers (LSP, 40+ languages) by default, or a paid JetBrains plugin that adds move, inline, type hierarchy and debugging. It works with Claude Code, Codex, Cursor, VSCode, Claude Desktop and other MCP clients.

- **+** Symbol-level find, reference lookup and edit tools instead of line-number or regex operations
- **+** Language server backend covers 40+ languages and is free to use
- **+** Works with any MCP client, including Claude Code, Codex, Cursor and OpenWebUI
- **+** Layered YAML configuration: global, per-project, per-client context and modes
- **−** Move, inline, type hierarchy and debugging need the paid JetBrains plugin
- **−** LSP backend rename covers symbols only; some languages need extra dependencies installed
- **−** Mixed licensing: GPL-3.0-or-later application with MIT SolidLSP component
- **−** README warns against marketplace installs; setup requires uv and per-client configuration

<sub>no GPU · Docker + Compose · Needs uv, language servers (per language), JetBrains IDE plugin (optional, paid) · Models: any MCP-capable client/LLM · safety checks passed 12 of 14 · [Repo](https://github.com/oraios/serena) · [📖 Docs ↗](https://oraios.github.io/serena/02-usage/000_intro.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serena/)</sub>

<a name="n8n-mcp"></a>
### #&#8288;4 [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Oct 2026</sub>

**MCP server exposing n8n node docs, templates and workflow management to AI assistants.**

n8n-MCP is a TypeScript MCP server that gives AI assistants searchable access to 3,135 n8n nodes (840 core, 2,295 community), their property schemas, and 2,352 workflow templates. With an n8n API URL and key configured, it also creates, updates, validates, tests and deploys workflows on a live n8n instance. It can be used through a hosted dashboard or self-hosted via npx, Docker or Railway.

- **+** Node, template and validation tools (search_nodes, get_node, validate_workflow) cover core and community nodes
- **+** 21 management tools create, patch, autofix and test workflows on a connected n8n instance
- **+** Hosted option with free tier of 100 tool calls/day, or self-host via npx, Docker or Railway
- **+** Setup guides for Claude Code, Cursor, VS Code, Windsurf and Codex
- **−** Operation coverage is 66.5% and docs coverage 86%, so some nodes lack detail
- **−** Management tools need N8N_API_URL and N8N_API_KEY; some also need a separate MCP access token
- **−** README warns AI edits to production workflows are unpredictable; backups needed
- **−** Split-host n8n instance-level MCP (N8N_MCP_BASE_URL) is not supported

<sub>no GPU · Docker + Compose · Needs n8n instance (optional, for management tools), n8n API key · [Repo](https://github.com/czlonkowski/n8n-mcp) · [▶️ Demo ↗](https://dashboard.n8n-mcp.com) · [📖 Docs ↗](https://github.com/czlonkowski/n8n-mcp/blob/main/docs/SELF_HOSTING.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/n8n-mcp/)</sub>

<a name="chrome-devtools-mcp"></a>
### #&#8288;5 [chrome-devtools-mcp](https://github.com/chromedevtools/chrome-devtools-mcp) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · Apache-2.0 · Oct 2026</sub>

**MCP server and CLI that lets coding agents control and debug live Chrome.**

Runs as an MCP server and a `chrome-devtools` CLI that give a coding agent control of a live Chrome instance through Puppeteer and Chrome DevTools. It records performance traces, inspects network requests, reads console messages with source-mapped stack traces, and takes screenshots. The package also ships skills for accessibility, LCP, cookie and memory-leak debugging.

- **+** Built on Puppeteer and DevTools: traces, network inspection, console and screenshots
- **+** Installs with one npx config entry; setup guides for Claude Code, Cursor, Copilot, Gemini CLI
- **+** Bundled skills and plugin installs for Claude Code, Copilot/VS Code and Gemini CLI
- **+** `--slim` flag exposes a reduced tool set for basic browser tasks
- **−** Usage statistics sent to Google are on by default; opt out with a flag
- **−** Performance tools may send trace URLs to the Google CrUX API unless disabled
- **−** Officially supports only Google Chrome and Chrome for Testing
- **−** Exposes all browser content to the MCP client, including sensitive data

<sub>no GPU · Needs Node.js LTS, npm, Google Chrome (current stable) · safety checks passed 17 of 17 · [Repo](https://github.com/chromedevtools/chrome-devtools-mcp) · [📖 Docs ↗](https://github.com/chromedevtools/chrome-devtools-mcp/blob/main/docs/tool-reference.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chrome-devtools-mcp/)</sub>

<a name="code-review-graph"></a>
### #&#8288;6 [code-review-graph](https://github.com/tirth8205/code-review-graph) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Oct 2026</sub>

**Local Tree-sitter code graph served over MCP so agents read only affected files.**

Parses a repository with Tree-sitter into a SQLite graph of functions, classes, imports, calls, inheritance and tests, then serves blast-radius and review context to AI coding tools over MCP. A single install command detects and configures about 16 tools, including Claude Code, Cursor, Codex, Windsurf and Zed. It also ships a GitHub Action that posts risk-scored PR comments, and updates the graph incrementally by SHA-256 hash.

- **+** One install command configures about 16 coding tools; uninstall leaves other config intact
- **+** Incremental re-parse by SHA-256; two-file edit on a ~3,000-file repo took about 2.5 s
- **+** Covers 30+ languages and notebooks, plus custom languages via languages.toml
- **+** Pinned-SHA benchmarks with a reproduction recipe; median 63x token reduction across 6 repos
- **−** Impact recall of 1.0 is circular, since ground truth comes from the same graph
- **−** Graph context can exceed a plain file read for small single-file edits
- **−** Search ranking needs work; Express queries can return no hits
- **−** Flow detection is strongest for Python and PHP/Laravel; JavaScript and Go are weaker

<sub>no GPU · Needs Python 3.10+, Tree-sitter, SQLite · Models: sentence-transformers (all-MiniLM-L6-v2), Google Gemini, MiniMax, Voyage AI, OpenAI-compatible endpoints · safety checks passed 16 of 18 · [Repo](https://github.com/tirth8205/code-review-graph) · [🌐 Site ↗](https://code-review-graph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-review-graph/)</sub>

<a name="fastmcp"></a>
### #&#8288;7 [fastmcp](https://github.com/prefecthq/fastmcp) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Oct 2026</sub>

**Python framework for building MCP servers, clients, and interactive apps.**

FastMCP is a Python framework for the Model Context Protocol. A decorated Python function becomes an MCP tool, with schema, validation and documentation generated from its signature. It also ships a client for local or remote servers and an Apps feature for interactive UIs rendered in the conversation.

- **+** Tool schemas and validation are generated from Python type hints and docstrings
- **+** Covers servers, clients and interactive Apps in one package
- **+** Minimal server is about ten lines; installs with uv add fastmcp
- **+** Upgrade guides for FastMCP 2/3 and MCP SDK; docs published as llms.txt
- **−** Python only; TypeScript needs the separate fastmcp-ts project
- **−** SSO, RBAC and audit logs belong to the separate Prefect Horizon product
- **−** Multiple major-version upgrade guides suggest breaking changes between releases
- **−** README gives no Docker image or hardware requirements

<sub>no GPU · Needs Python, uv (recommended) · [Repo](https://github.com/prefecthq/fastmcp) · [📖 Docs ↗](https://gofastmcp.com) · [🌐 Site ↗](https://gofastmcp.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastmcp/)</sub>

<a name="python-sdk"></a>
### #&#8288;8 [python-sdk](https://github.com/modelcontextprotocol/python-sdk) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Oct 2026</sub>

**Official Python SDK for building MCP servers and clients.**

Python implementation of the Model Context Protocol. It lets you write MCP servers that expose tools, resources and prompts from type-hinted functions, and clients that connect to any MCP server over stdio, Streamable HTTP or SSE. An optional cli extra adds the mcp dev, mcp run and mcp install commands.

- **+** Tool schemas come from Python type hints and docstrings, no hand-written JSON Schema
- **+** Server and client in one package
- **+** Supports stdio, Streamable HTTP and SSE transports
- **+** Docs include a get-started guide, API reference and v2 migration guide
- **−** Requires Python 3.11 or newer
- **−** A library, not a ready-made server; you write the tools yourself
- **−** v2 has a migration guide, so v1 code may need changes
- **−** README gives no auth or deployment details; those are only in the docs

<sub>no GPU · Needs Python 3.11+ · port 8000 · [Repo](https://github.com/modelcontextprotocol/python-sdk) · [📖 Docs ↗](https://py.sdk.modelcontextprotocol.io/) · [🌐 Site ↗](https://modelcontextprotocol.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/python-sdk/)</sub>

<a name="context7"></a>
### #&#8288;9 [context7](https://github.com/upstash/context7) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 64k · MIT · Oct 2026</sub>

**MCP server and CLI that feed current library docs to coding agents.**

Context7 retrieves version-specific documentation and code examples for libraries and injects them into a coding agent's context. It works either as an MCP server exposing resolve-library-id and query-docs, or as a ctx7 CLI plus an installed skill. The repository holds the MCP server source; the API backend, parsing and crawling engines are private.

- **+** One command, npx ctx7 setup, configures the skill or MCP for Cursor, Claude Code or OpenCode
- **+** Two modes: MCP tools or CLI with skill, so MCP support is optional
- **+** Version-aware lookup, and library IDs like /vercel/next.js skip the matching step
- **+** Also ships a TypeScript SDK and Vercel AI SDK tools as npm packages
- **−** Docs index, API backend, parsing and crawling engines are private; not self-hostable from this repo
- **−** Needs network access to mcp.context7.com; the README gives no offline mode
- **−** Free API key recommended for higher rate limits; limits are not stated
- **−** Docs are community-contributed; accuracy and security are not guaranteed

<sub>no GPU · Needs Node.js 22.13+ (ctx7 CLI), Context7 hosted API (mcp.context7.com), Context7 API key (recommended) · safety checks passed 15 of 17 · [Repo](https://github.com/upstash/context7) · [📖 Docs ↗](https://context7.com/docs/resources/all-clients) · [🌐 Site ↗](https://context7.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context7/)</sub>

<a name="mcp-toolbox"></a>
### #&#8288;10 [mcp-toolbox](https://github.com/googleapis/mcp-toolbox) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Oct 2026</sub>

**MCP server that exposes databases to agents through prebuilt and custom SQL tools.**

A Go MCP server that connects AI agents and IDEs to databases. The `--prebuilt=<database>` flag provides generic tools such as `list_tables` and `execute_sql`, and a `tools.yaml` file defines custom parameterized tools, toolsets, prompts and resources. Client SDKs exist for Python, JS/TS, Go and Java, and the server handles connection pooling, IAM auth and OpenTelemetry.

- **+** Prebuilt tools for many databases: PostgreSQL, MySQL, BigQuery, Spanner, MongoDB, Redis, Snowflake and more
- **+** Custom tools defined in YAML with parameterized SQL statements and toolsets
- **+** Client SDKs for Python, JS/TS, Go and Java, with LangChain and LlamaIndex integrations
- **+** Built-in connection pooling, IAM-integrated auth and OpenTelemetry metrics and tracing
- **−** Many sources and tools are tied to Google Cloud databases, so non-Google setups need per-source config
- **−** README container example pins version 0.24.0 while install steps use 1.15.0
- **−** npx run method is described as optimized for convenience, not performance
- **−** Managed Google Cloud MCP Servers are a separate product with differences from this one

<sub>no GPU · Docker · Needs A supported database (e.g. PostgreSQL), Node.js (only for the npx install) · port 5000 · [Repo](https://github.com/googleapis/mcp-toolbox) · [📖 Docs ↗](https://mcp-toolbox.dev/) · [🌐 Site ↗](https://mcp-toolbox.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-toolbox/)</sub>

<a name="unity-mcp"></a>
### #&#8288;11 [unity-mcp](https://github.com/coplaydev/unity-mcp) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

**MCP server that lets AI clients control the Unity Editor.**

A Unity package plus a Python MCP server that exposes 50 tool entrypoints for creating scenes and GameObjects, editing C# scripts, managing assets, running tests, profiling and building. It works with any MCP client, including Claude Desktop and Code, Cursor, VS Code, Windsurf, Cline and Gemini CLI. Installed through Unity Package Manager from a git URL or OpenUPM.

- **+** Covers scenes, scripts, assets, tests, profiling and builds in 50 tool entrypoints
- **+** Works with any MCP client; one menu action configures detected clients
- **+** Supports Unity 2021.3 LTS through 6.x
- **+** MIT licensed; docs cover multi-instance routing, tool groups and remote server auth
- **−** Requires Python 3.10+ via uv alongside the Unity install
- **−** Only targets the Unity Editor; no runtime or other engine support
- **−** Install tracks the main branch by default unless a version tag is pinned
- **−** Sponsored by a vendor that also sells a premium assistant, Aura for Unity

<sub>Compose · Needs Unity 2021.3 LTS to 6.x, Python 3.10+, uv · Models: Any MCP client (Claude, Codex, Cursor, VS Code, Windsurf, Cline, Gemini CLI) · safety checks passed 17 of 18 · [Repo](https://github.com/coplaydev/unity-mcp) · [📖 Docs ↗](https://coplaydev.github.io/unity-mcp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unity-mcp/)</sub>

<a name="github-mcp-server"></a>
### #&#8288;12 [github-mcp-server](https://github.com/github/github-mcp-server) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

**GitHub's official MCP server for repos, issues, PRs and Actions.**

Official MCP server from GitHub that lets AI hosts read repositories and code, manage issues and pull requests, inspect GitHub Actions runs, and view security findings and Dependabot alerts. It runs as a GitHub-hosted remote endpoint (api.githubcopilot.com/mcp/) or as a local Go binary or Docker image over stdio, authenticating with OAuth or a personal access token.

- **+** Maintained by GitHub; hosted remote endpoint needs no local install
- **+** Covers issues, PRs, Actions, code security, Dependabot, discussions and notifications
- **+** OAuth or PAT auth; GitHub Enterprise Server and ghe.com via GITHUB_HOST
- **+** Local option as Go binary or ghcr.io Docker image; toolsets configurable
- **−** Remote server is not available for GitHub Enterprise Server; local server required
- **−** Remote OAuth depends on each MCP host registering its own GitHub or OAuth App
- **−** Local Docker OAuth needs a fixed callback port (8085) published to loopback
- **−** PAT scopes are chosen manually; broad tokens expose more of your account

<sub>no GPU · Docker · Needs GitHub account, Docker (optional, for local image), MCP host · safety checks passed 14 of 15 · [Repo](https://github.com/github/github-mcp-server) · [📖 Docs ↗](https://github.com/github/github-mcp-server/blob/main/docs/remote-server.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github-mcp-server/)</sub>

<a name="typescript-sdk"></a>
### #&#8288;13 [typescript-sdk](https://github.com/modelcontextprotocol/typescript-sdk) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · custom license · Oct 2026</sub>

**Official TypeScript SDK for building MCP servers and clients.**

Split npm packages, @modelcontextprotocol/server and @modelcontextprotocol/client, implementing the 2026-07-28 MCP spec on Node.js, Bun and Deno. The server side covers tools, resources, prompts, Streamable HTTP, stdio and auth helpers; the client side covers transports and OAuth helpers. Optional thin adapters exist for Node HTTP, Express, Fastify and Hono.

- **+** Reference SDK maintained in the modelcontextprotocol organization, tracking the 2026-07-28 spec
- **+** Runs on Node.js, Bun and Deno
- **+** Tool and prompt schemas use Standard Schema: Zod v4, Valibot, ArkType
- **+** Separate Express, Fastify, Hono and Node HTTP adapter packages
- **−** v2 is a breaking change from v1; migration guide required
- **−** v1.x stays on a separate branch with its own package name and docs
- **−** Library only: no ready-made servers, so you write the tool logic
- **−** License is mixed: Apache-2.0 for new contributions, MIT for existing code

<sub>no GPU · Needs Node.js, Bun or Deno, zod or another Standard Schema library · [Repo](https://github.com/modelcontextprotocol/typescript-sdk) · [📖 Docs ↗](https://ts.sdk.modelcontextprotocol.io/v2/) · [🌐 Site ↗](https://modelcontextprotocol.io/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typescript-sdk/)</sub>

<a name="codebase-memory-mcp"></a>
### #&#8288;14 [codebase-memory-mcp](https://github.com/deusdata/codebase-memory-mcp) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · MIT · Oct 2026</sub>

**Local MCP server that indexes a codebase into a queryable code knowledge graph.**

A native C MCP server that indexes functions, classes, imports and HTTP routes across 162 languages into a local graph, and exposes 17 tools for search, call tracing, impact analysis and Cypher queries. The installer configures 45 agent client surfaces, including Claude Code and Codex. A browser UI (CBM Lens Beta) for source reading, 3D architecture maps and local chat is on main but not in the v0.11.0 release.

- **+** Single native binary for macOS, Linux and Windows; no Docker, runtime or API key needed
- **+** Vendored tree-sitter grammars cover 162 languages; Hybrid LSP type resolution for 13 of them
- **+** Reports Linux kernel (28M LOC) indexed in about 3 minutes, all processing local
- **+** Also indexes Dockerfiles, compose files and Kubernetes manifests as graph nodes
- **−** CBM Lens Beta UI requires building from source; v0.11.0 ships the older graph UI
- **−** Preprint reports 83% answer quality versus 92% for file-by-file exploration
- **−** All active CBM processes must run the exact same build and cache root
- **−** Windows Defender may flag the release binary as a false positive

<sub>GPU optional · Models: Optional local model for CBM Lens chat, downloaded from Hugging Face · port 9749 · safety checks passed 13 of 16 · [Repo](https://github.com/deusdata/codebase-memory-mcp) · [📖 Docs ↗](https://github.com/DeusData/codebase-memory-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codebase-memory-mcp/)</sub>

<a name="ghidra-mcp"></a>
### #&#8288;15 [ghidra-mcp](https://github.com/bethington/ghidra-mcp) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · Apache-2.0 · Oct 2026</sub>

**MCP server exposing Ghidra reverse-engineering tools to AI clients.**

A Ghidra extension (Java) plus a Python MCP bridge that exposes 209 tools for decompilation, cross-references, renaming, typing, structs, P-code emulation and debugger control. The extension serves HTTP on 127.0.0.1:8089 inside Ghidra, and the bridge relays MCP calls to it. It runs in the Ghidra GUI or headless, and naming and type rules are enforced on writes.

- **+** 209 tools covering read and write: decompile, rename, retype, comment, structs, batch edits
- **+** P-code emulation and 16 debugger endpoints via TraceRmi (GUI plugin only)
- **+** Naming and type conventions enforced in the tool layer: auto-fix, warn or reject
- **+** Release zip plus wheel install; headless mode and Ghidra Server support
- **−** Extension loads only in the exact Ghidra version it was built for (12.1.4)
- **−** Needs Ghidra, Java 21 and Python 3.10+ with uv; no Docker files detected
- **−** Script execution is opt-in via GHIDRA_MCP_ALLOW_SCRIPTS=1; .py scripts need Jython
- **−** main is beta and dev is experimental; only tagged releases are stable

<sub>no GPU · Docker + Compose · Needs Ghidra 12.1.4, Java 21, Python 3.10+, uv · port 8089 · [Repo](https://github.com/bethington/ghidra-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ghidra-mcp/)</sub>

<a name="mcp"></a>
### #&#8288;16 [mcp](https://github.com/awslabs/mcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · Apache-2.0 · Oct 2026</sub>

**AWS-maintained MCP servers for docs, IaC, containers, databases and cost tools.**

A collection of MCP servers from AWS Labs that give coding agents and chat clients access to AWS documentation, CloudFormation/CDK guidance, EKS and serverless tooling, databases, and cost and operations data. The local servers are Python packages launched with uvx over stdio; two remote servers (AWS MCP Server in preview, AWS Knowledge) are hosted by AWS. The README says Agent Toolkit for AWS is the successor and the most useful projects here will move there.

- **+** Many servers in one repo: docs, IaC, EKS, databases, cost, healthcare and more
- **+** One-click install links for Kiro, Cursor and VS Code, plus config examples for Cline, Windsurf, Claude Code
- **+** Hosted AWS Knowledge server needs no local install; AWS MCP Server adds IAM and CloudTrail logging
- **+** Apache-2.0, published by AWS Labs with active commits and recent releases
- **−** Local servers support stdio only; SSE was removed May 2025 and Streamable HTTP is not yet supported
- **−** README names Agent Toolkit for AWS as successor; projects here may move
- **−** Most servers need AWS credentials and the right IAM permissions
- **−** Some servers are deprecated, such as the Cloud Control API server

<sub>no GPU · Needs uvx, AWS credentials, MCP client · [Repo](https://github.com/awslabs/mcp) · [📖 Docs ↗](https://docs.aws.amazon.com/aws-mcp/latest/userguide/what-is-mcp-server.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp/)</sub>

<a name="browser-tools-mcp"></a>
### #&#8288;17 [browser-tools-mcp](https://github.com/agentdeskai/browser-tools-mcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

**MCP server that feeds Chrome console, network and Lighthouse data to coding agents.**

Runs as an npx-launched MCP server paired with a Chrome DevTools extension, and passes console logs, network requests, screenshots and Lighthouse audits from your logged-in browser session to MCP clients such as Cursor, Claude Code and Cline. Version 2.0 is a single-process rewrite that binds to loopback only, requires a per-run token and redacts credentials before data leaves the browser.

- **+** Reads your existing logged-in Chrome session, no throwaway debug profile needed
- **+** Per-tab capture with limit, offset and keyword filters to keep context small
- **+** Loopback-only binding, per-run token and credential redaction by default
- **+** Four Lighthouse audit tools, including accessibility, performance and SEO
- **−** Requires manually loading an unpacked Chrome extension
- **−** Capture starts only when DevTools is open; earlier requests are not recorded
- **−** Firefox support is unverified and untested
- **−** Audits launch a separate browser and can take up to a minute

<sub>no GPU · Needs Node 22.19+, Chrome extension, Chromium-based browser for audits · port 3025 · [Repo](https://github.com/agentdeskai/browser-tools-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browser-tools-mcp/)</sub>

<a name="dbhub"></a>
### #&#8288;18 [dbhub](https://github.com/bytebase/dbhub) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**MCP server that gives coding agents SQL access to six database engines.**

DBHub is an MCP server that connects clients such as Claude Desktop, Claude Code, Cursor and VS Code to PostgreSQL, MySQL, MariaDB, SQL Server, Oracle and SQLite. It exposes two tools by default, execute_sql and search_objects, with opt-in explain_sql and health_check, plus custom parameterized tools defined in a TOML file. A built-in web workbench runs queries without an MCP client.

- **+** Two default tools at about 1.4k tokens, versus 19k for MCP Toolbox per README
- **+** Read-only mode, row limit and query timeout guard against runaway queries
- **+** Several databases in one process via TOML config; SSH tunneling and SSL/TLS supported
- **+** Runs via npx, Docker, MCP Bundle or Claude Code plugin; includes a web workbench
- **−** No approval flow, access control, data masking or audit logging; README points to Bytebase
- **−** Development requires Node.js 22.5 or newer because it uses node:sqlite
- **−** Only six SQL engines listed; no NoSQL or warehouse engines mentioned
- **−** Token comparison figures are the project's own, not independently verified

<sub>no GPU · Docker · Needs Node.js >= 22.5.0 (development), A target database: PostgreSQL, MySQL, MariaDB, SQL Server, Oracle or SQLite · port 8080 · [Repo](https://github.com/bytebase/dbhub) · [📖 Docs ↗](https://dbhub.ai/installation) · [🌐 Site ↗](https://dbhub.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dbhub/)</sub>

<a name="jcodemunch-mcp"></a>
### #&#8288;19 [jcodemunch-mcp](https://github.com/jgravelle/jcodemunch-mcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · custom license · Oct 2026</sub>

**MCP server that returns code by symbol using tree-sitter indexing.**

jCodeMunch indexes a repository locally with tree-sitter (70+ languages) and exposes MCP tools such as search_symbols and get_symbol_source, so agents fetch single functions instead of whole files. It also provides structural queries like find_importers, get_blast_radius and check_edit_safe. On the project's pinned benchmark (express, fastapi, gin) it used 29.2x fewer tokens than a grep-and-read baseline.

- **+** Symbol-level retrieval with byte offsets; README benchmark shows 96.6% fewer tokens than grep-and-read
- **+** Structural tools grep lacks: find_importers, get_blast_radius, find_dead_code, check_edit_safe
- **+** Local index in ~/.code-index/; works with Claude Code, Cursor, VS Code, Codex CLI, Windsurf
- **+** Benchmark harness, pinned commits and methodology are published for reproduction
- **−** License is dual-use: free for personal use, commercial use needs a paid license
- **−** Gains are small for edits needing whole-file context; README lists ~0% savings there
- **−** Agent must be told to prefer the tools (CLAUDE.md line), or it keeps reading files
- **−** Sends an anonymous savings counter by default; opt out with share_savings: false

<sub>no GPU · Docker + Compose · Needs Python, uv, pipx or pip, tree-sitter-language-pack · [Repo](https://github.com/jgravelle/jcodemunch-mcp) · [📖 Docs ↗](https://github.com/jgravelle/jcodemunch-mcp/blob/main/QUICKSTART.md) · [🌐 Site ↗](https://jcodemunch.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jcodemunch-mcp/)</sub>

<a name="mobile-mcp"></a>
### #&#8288;20 [mobile-mcp](https://github.com/mobile-next/mobile-mcp) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · Apache-2.0 · Oct 2026</sub>

**MCP server that lets agents drive iOS and Android devices and simulators.**

Mobile MCP exposes tools for tapping, swiping, typing, app install/launch, screenshots, screen recording and device logs on iOS simulators, Android emulators and real devices. It reads the native accessibility tree first and falls back to screenshots with coordinates. It runs over stdio by default, or as a Streamable HTTP server with an optional Bearer token.

- **+** Same tool set across iOS simulators, Android emulators and real devices
- **+** Accessibility-tree-first, so most steps need no vision model
- **+** Covers app management, logs, crash reports, screen recording and batch commands
- **+** Optional Streamable HTTP mode via --listen with MOBILEMCP_AUTH Bearer token
- **−** Needs Xcode command line tools and Android platform tools installed locally
- **−** iOS real devices need USB and trust; Android needs USB debugging enabled
- **−** Cloud devices depend on the separate Mobile Next Cloud service
- **−** Anonymous telemetry is on by default; disable with an env var

<sub>no GPU · Docker · Needs Node.js v20+, Xcode command line tools, Android Platform Tools (adb) · Models: Any MCP-compatible client · [Repo](https://github.com/mobile-next/mobile-mcp) · [📖 Docs ↗](https://github.com/mobile-next/mobile-mcp/wiki) · [🌐 Site ↗](https://mobilenext.ai/cloud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mobile-mcp/)</sub>

<a name="agent-device"></a>
### #&#8288;21 [agent-device](https://github.com/callstack/agent-device) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

**CLI and MCP server that lets coding agents drive and verify mobile apps.**

agent-device lets coding agents open, inspect and control apps on iOS, Android, HarmonyOS, TV platforms, web, macOS and Linux. It exposes the same runtime as a CLI, a stdio MCP server (`agent-device mcp`) and a typed Node.js client. Agents read accessibility-tree snapshots, act through refs and selectors, and save screenshots, video and logs as evidence.

- **+** Same session model across CLI, MCP server and typed Node.js API
- **+** Token-efficient accessibility snapshots with refs instead of screenshot-only reasoning
- **+** Records runs as .ad replay scripts for CI, with strict Maestro YAML export
- **+** Per-worktree sessions and device claims keep parallel agents off each other's simulators
- **−** HarmonyOS and Vega OS backends support only a subset of commands
- **−** Reliability depends on clear accessibility labels, roles and test IDs in the app
- **−** Web automation needs Node.js 24 and agent-browser; core CLI needs Node.js 22.12
- **−** Backends depend on platform toolchains such as XCTest, ADB and HDC being installed

<sub>Needs Node.js 22.12+ (24+ for web), XCTest/iOS Simulator (iOS, tvOS), ADB (Android), HDC (HarmonyOS), agent-browser (web) · [Repo](https://github.com/callstack/agent-device) · [📖 Docs ↗](https://oss.callstack.com/agent-device/) · [🌐 Site ↗](https://agent-device.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-device/)</sub>

<a name="repowise"></a>
### #&#8288;22 [repowise](https://github.com/repowise-dev/repowise) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · AGPL-3.0 · Oct 2026</sub>

**Local codebase index answering call-graph, risk and dead-code questions for agents.**

Repowise indexes a repository's call graph (26 parsed languages), git history, tests, docs and design decisions locally, then exposes ten task-shaped MCP tools plus a CLI and dashboard. It answers what calls a symbol, what a diff may break, which tests to run, what is dead and what to fix first. Graph, risk, health and dead-code analysis make no LLM calls; model-written docs are optional.

- **+** Core indexing, risk, health and dead-code analysis need no API key and make zero LLM calls
- **+** Ten MCP tools take multiple targets per call, reducing sequential agent lookups
- **+** Publishes benchmarks against other tools, including rows where it loses, in docs/BENCHMARKS.md
- **+** Also covers CI coverage gates, secret scanning and cross-repo contract checks in workspaces
- **−** AGPL-3.0 with a commercial option; may block some company use
- **−** Benchmark figures are the authors' own and not independently verified in the README
- **−** Foresight models and the PR bot with AI review are hosted-only
- **−** Wide scope (53 detectors, decisions, workspaces) means a larger surface to learn

<sub>no GPU · Docker + Compose · Needs Python, uv or pipx or pip · [Repo](https://github.com/repowise-dev/repowise) · [▶️ Demo ↗](https://www.repowise.dev/?src=oss_readme_hero) · [📖 Docs ↗](https://docs.repowise.dev) · [🌐 Site ↗](https://www.repowise.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repowise/)</sub>

<a name="semble"></a>
### #&#8288;23 [semble](https://github.com/minishlab/semble) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · Oct 2026</sub>

**Local code search for coding agents, via MCP server or CLI.**

Semble indexes a local path or git URL with tree-sitter chunking, then ranks chunks by fusing static Model2Vec embeddings (potion-code-16M-v2) with BM25 using Reciprocal Rank Fusion. It runs on CPU and returns only matching snippets to agents such as Claude Code, Cursor, Codex and OpenCode. It ships as an MCP server with search and find_related tools, a CLI, a sub-agent installer and a Python library.

- **+** Runs on CPU with no API keys or external services; model downloads once from Hugging Face
- **+** Reports NDCG@10 of 0.855 over ~1,250 queries across 63 repos and 19 languages
- **+** Searches several repos or git URLs as one corpus with incremental, cached indexes
- **+** Interactive `semble install` configures MCP, AGENTS.md instructions or a sub-agent per detected agent
- **−** First run needs network access to fetch the embedding model unless SEMBLE_MODEL_NAME points locally
- **−** Files over 1 MB and data files such as .json and .csv are skipped by default
- **−** The ~99% token savings figure is the project's own benchmark against grep+read
- **−** Retrieval only; it does not edit code or run commands

<sub>no GPU · Needs uv, Hugging Face (first-run model download) · Models: Model2Vec static embeddings (potion-code-16M-v2) · [Repo](https://github.com/minishlab/semble) · [📖 Docs ↗](https://github.com/MinishLab/semble/blob/main/docs/installation.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/semble/)</sub>

<a name="desktopcommandermcp"></a>
### #&#8288;24 [desktopcommandermcp](https://github.com/wonderwhy-er/desktopcommandermcp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

**MCP server giving AI clients terminal, process and file editing tools.**

Desktop Commander is a TypeScript MCP server that lets clients such as Claude Desktop, Cursor, Codex and Claude Code run terminal commands, manage long-running processes and edit files. It adds search and replace editing, in-memory code execution (Python, Node.js, R), and read/write support for Excel, PDF and DOCX files. A remote mode connects ChatGPT and Claude web to commands running on your machine.

- **+** Installs with one npx command or JSON entry in many MCP clients
- **+** Interactive process control for SSH sessions, databases and dev servers, with paginated output
- **+** Reads and edits Excel, PDF and DOCX files, not only plain text
- **+** Local tool-call history and audit logs stored on your machine
- **−** Not a sandbox: commands run with your user permissions, blocklist is only a guardrail
- **−** Docker isolation is optional and needs separate setup with folder mounts
- **−** Remote mode depends on browser OAuth and the hosted mcp.desktopcommander.app service
- **−** Most install paths pull @latest, so versions change on client restart

<sub>no GPU · Docker · Needs Node.js, Docker (optional) · [Repo](https://github.com/wonderwhy-er/desktopcommandermcp) · [🌐 Site ↗](https://mcp.desktopcommander.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/desktopcommandermcp/)</sub>

<a name="aos-ce"></a>
### #&#8288;25 [aos-ce](https://github.com/unicity-aos/aos-ce) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Oct 2026</sub>

**Local runtime that runs agent tools as permissioned WebAssembly capsules.**

AOS is a Rust CLI and runtime that gives agents such as Claude, Codex and Grok a shared local environment. Tools run as isolated WebAssembly capsules with explicit permissions, approval prompts and an audit trail, exposed through `aos mcp serve`. Community Edition bundles 22 first-party capsules, a Command Center app and Forge tooling for building new capsules.

- **+** Capsules run in WebAssembly isolation with explicit permissions and an audit trail
- **+** Releases ship checksums, Sigstore bundles and build-provenance attestations
- **+** Per-principal environments keep agents separate from the operator's installation
- **+** Local approval UI on macOS, Windows and Linux when the client lacks MCP elicitation
- **−** Fresh install of all 22 capsules waits about two minutes on rate-limit windows
- **−** Native execution on macOS 11–15 is untested
- **−** Linux install fails unless the host setup check passes
- **−** Community Edition distro is fixed; other distributions need a standalone astrid install

<sub>no GPU · Needs Astrid runtime (bundled), Pinentry (Linux approval prompts) · Models: Claude, Codex, Grok · [Repo](https://github.com/unicity-aos/aos-ce) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aos-ce/)</sub>

<a name="wigolo"></a>
### #&#8288;26 [wigolo](https://github.com/knockoutez/wigolo) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · custom license · Oct 2026</sub>

**Local MCP and REST server for web search, fetch, crawl and extraction by agents.**

wigolo gives coding and self-hosted agents one tool surface for web search (18 engine adapters with rank fusion and on-device reranking), fetch, crawl, extract, cache, find-similar, research and an autonomous gather loop. It runs as an MCP server over stdio, a REST API on port 3333, or through TypeScript and Python SDKs. Core tools need no API keys; research and agent synthesis need an LLM provider or return a raw brief.

- **+** Search, fetch, crawl, extract and cache work without API keys; data stays under ~/.wigolo/
- **+** Results include verbatim excerpts with byte-offset source spans and a per-result score breakdown
- **+** Fetch escalates from plain HTTP to a headless browser on challenges or SPA shells
- **+** Also ships REST/OpenAPI, TS and Python SDKs, and LangChain, CrewAI, LlamaIndex, Vercel AI SDK wrappers
- **−** Public beta status per the README
- **−** AGPL-3.0 per README badge; detected license is NOASSERTION, so check LICENSING.md
- **−** Synthesized answers from research and agent need an external or local LLM configured
- **−** Datacenter IPs may fail on challenge-protected sites; proxy is opt-in

<sub>no GPU · Docker · Needs Node.js >= 20, ~1.5 GB disk for browser engine and models, Optional LLM provider (Gemini, Anthropic, OpenAI, Groq, Ollama) · Models: Gemini, Anthropic, OpenAI, Groq, Ollama · port 3333 · [Repo](https://github.com/knockoutez/wigolo) · [📖 Docs ↗](https://github.com/KnockOutEZ/wigolo/blob/main/docs/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wigolo/)</sub>

<a name="ivanmurzak-unity-mcp"></a>
### #&#8288;27 [unity-mcp](https://github.com/ivanmurzak/unity-mcp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

**Unity Editor and runtime plugin exposing 70+ MCP tools to coding agents.**

Unity package that runs an MCP server connected to the Unity Editor, so agents such as Claude Code, Cursor, Codex and Copilot can create GameObjects, edit scenes and assets, write and run C# scripts, run tests and read console logs. It also generates agent skills for the project and can run inside a compiled game for in-game LLM use. Connects over stdio locally or HTTP remotely.

- **+** 70+ built-in tools covering assets, scenes, components, scripts, console logs, tests and screenshots
- **+** Works with many MCP clients: Claude, Codex, Cursor, Copilot, Gemini, Cline, Rider, VS Code
- **+** Runs in compiled games, not only the Editor, for in-game AI and debugging
- **+** Custom tools can be added in project C# code; extension packages exist for Terrain, Timeline and others
- **−** Unity-only; no use outside Unity projects
- **−** Project path cannot contain spaces
- **−** CLI quick start includes sign-in to ai-game.dev; local-only requirements unclear in the README
- **−** Reflection and dynamic Roslyn script execution give agents broad access to the project

<sub>Needs Unity Editor, Node.js and npm (for unity-mcp-cli), Docker (optional, for hosting the MCP server) · Models: Claude, Codex, Cursor, GitHub Copilot, Gemini · [Repo](https://github.com/ivanmurzak/unity-mcp) · [📖 Docs ↗](https://ai-game.dev/docs/tools) · [🌐 Site ↗](https://ai-game.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ivanmurzak-unity-mcp/)</sub>

<a name="arxiv-mcp-server"></a>
### #&#8288;28 [arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Oct 2026</sub>

**MCP server for searching, reading and citing arXiv papers by section.**

A local MCP server, run over stdio via `uvx arxiv-mcp-server`, that exposes 19 tools for arXiv literature work: search, Markdown download, outline and section reads, original-LaTeX section retrieval, BibTeX export and saved topic watches. Papers are stored on disk (default `~/.arxiv-mcp-server/papers`), and reads are bounded to 12,000 characters by default. Citation graphs come from the Semantic Scholar API; optional extras add PDF conversion and local semantic search.

- **+** Reads author-submitted LaTeX one section at a time, with outline IDs
- **+** Exports BibTeX from arXiv metadata and keeps topic watches locally
- **+** Bounded 12,000-char reads keep single tool calls from flooding client context
- **+** Plugin or Power packaging for Claude Code, Codex and Kiro, plus MCP registry listing
- **−** Search, LaTeX source and downloads depend on remote arXiv services; arXiv rate-limits to ~3 s per request
- **−** Citation graph relies on Semantic Scholar; an API key is optional but improves reliability
- **−** Semantic search needs the `[pro]` extra; PDF fallback needs `[pdf]`
- **−** Name collides with an unrelated npm package; installing via npx gets the wrong one

<sub>no GPU · Docker · Needs uv, arXiv API, Semantic Scholar API, Python 3.11 · port 8080 · [Repo](https://github.com/blazickjp/arxiv-mcp-server) · [🌐 Site ↗](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.blazickjp%2Farxiv-mcp-server/versions/latest) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/arxiv-mcp-server/)</sub>

<a name="devspace"></a>
### #&#8288;29 [devspace](https://github.com/waishnav/devspace) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Sep 2026</sub>

**Self-hosted MCP server that lets ChatGPT edit and run code in local projects.**

DevSpace is a Node-based MCP server that exposes selected local project folders to ChatGPT or other MCP clients. The client can read, write and edit files, search code, run shell commands, and use isolated Git worktrees. You expose the `/mcp` endpoint through your own HTTPS tunnel and approve connections with an Owner password.

- **+** Access limited to folder roots you allow; connections need an Owner password
- **+** Reads AGENTS.md and CLAUDE.md and discovers local agent skills
- **+** Isolated Git worktrees for parallel coding sessions
- **+** Works with Linux, macOS and Windows via Git Bash or WSL
- **−** Connected client gets shell execution on your machine
- **−** Needs a public HTTPS tunnel you set up yourself for ChatGPT
- **−** Windows PowerShell or cmd.exe alone is not supported
- **−** Requires Node >=22.19 and a Bash-compatible shell

<sub>no GPU · Needs Node >=22.19 <27, Git, Bash, HTTPS tunnel (Cloudflare Tunnel, ngrok, Pinggy, Tailscale Funnel or reverse proxy) · Models: ChatGPT (MCP connector), Other MCP clients · port 7676 · [Repo](https://github.com/waishnav/devspace) · [📖 Docs ↗](https://github.com/Waishnav/devspace/blob/main/docs/setup.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devspace/)</sub>

<a name="linkedin-mcp-server"></a>
### #&#8288;30 [linkedin-mcp-server](https://github.com/stickerdaniel/linkedin-mcp-server) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Oct 2026</sub>

**MCP server that lets agents read and act on LinkedIn via your browser session.**

Python MCP server that drives a Patchright Chromium browser logged in as you. It exposes 20 tools for LinkedIn profiles, companies, jobs, posts, feed and messaging. It runs over stdio by default or streamable HTTP (127.0.0.1:8000/mcp), and can import an existing session from a local Chromium-based browser.

- **+** 20 tools covering profiles, company data, job search, feed, post search and messaging
- **+** Reuses a signed-in session from Chrome, Brave, Edge, Arc and other Chromium browsers
- **+** Runs over stdio or streamable HTTP; installs with a single uvx config entry
- **+** Tool calls are serialized across processes to protect the shared browser session
- **−** Browser automation depends on LinkedIn page structure; README relies on @latest auto-updates
- **−** Not affiliated with LinkedIn; automating a personal account may conflict with its terms
- **−** Chrome 127+ app-bound (v20) cookies cannot be imported; manual login needed
- **−** Session auto-import and inline login are skipped in Docker and non-loopback HTTP binds

<sub>no GPU · Docker + Compose · Needs uv, Patchright Chromium, LinkedIn account · port 8000 · [Repo](https://github.com/stickerdaniel/linkedin-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/linkedin-mcp-server/)</sub>

<a name="dev-browser"></a>
### #&#8288;31 [dev-browser](https://github.com/sawyerhood/dev-browser) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · MIT · Oct 2026</sub>

**CLI that lets coding agents drive Chrome with short Puppeteer scripts.**

dev-browser runs JavaScript scripts against a persistent Chrome instance through a warm local daemon, so an agent can navigate, snapshot, act and verify across separate calls. Pages are real Puppeteer objects with added helpers such as accessibility-tree snapshots with element refs. It can launch an isolated profile or attach to an existing browser over CDP, and also exposes an MCP server and an installable agent skill.

- **+** Named tabs persist between scripts, so agents keep page state across calls
- **+** Snapshots return accessibility trees with refs like e12 usable in Puppeteer selectors
- **+** Can launch an isolated profile or attach via port, HTTP, WebSocket or CDP socket
- **+** Ships a CLI, MCP server and skill installer for Codex, Claude and generic agents
- **−** Windows and musl Linux are not supported
- **−** Scripts run in node:vm, which the README says is not a security sandbox
- **−** Version 1.0 breaks 0.2 scripts; snapshotForAI and page.cua helpers are removed
- **−** Scripts sharing a named page can still interleave

<sub>no GPU · Needs Chrome or Chromium · [Repo](https://github.com/sawyerhood/dev-browser) · [▶️ Demo ↗](https://github.com/user-attachments/assets/c6cf7fb9-b1dc-46ed-93b9-6e7240990c53) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dev-browser/)</sub>

<a name="sem"></a>
### #&#8288;32 [sem](https://github.com/ataraxy-labs/sem) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · Apache-2.0 · Oct 2026</sub>

**Entity-level git diff, impact analysis and checks for code and agents.**

sem is a Rust CLI that parses code with tree-sitter and reports changes as functions, classes and methods instead of lines. It adds verbs for finding definitions and callers, selecting affected tests, running the project's own checkers on a change, and producing review certificates for commit ranges. Every verb supports --json, and `sem mcp` exposes them as MCP tools.

- **+** Works in any Git repo with no setup; also diffs arbitrary files outside Git
- **+** Every verb has --json output, and sem mcp serves the same verbs as MCP tools
- **+** sem impact --tests selects affected tests; sem check returns exit 0, 1 or 2
- **+** Many install routes: Homebrew, winget, Scoop, npm, cargo, Docker, release binaries
- **−** Binary name collides with GNU Parallel's sem; needs PATH or alias fix
- **−** Cloud queries and reviews need an account; opt-in per repo
- **−** Module graph and affected-test selection are most detailed for JS/TS
- **−** sem promises is hidden from sem --help; README shows license badge as MIT

<sub>no GPU · Docker · Needs Git, tree-sitter, SQLite cache · [Repo](https://github.com/ataraxy-labs/sem) · [🌐 Site ↗](https://ataraxy-labs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sem/)</sub>

<a name="supabase-mcp"></a>
### #&#8288;33 [mcp](https://github.com/supabase/mcp) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

**MCP server that lets AI assistants manage and query Supabase projects.**

Official Supabase MCP server, hosted at https://mcp.supabase.com/mcp, that gives clients such as Cursor, Claude and Windsurf tools for managing tables, fetching config and querying data. The TypeScript package @supabase/mcp-server-supabase also exports typed schemas for the Vercel AI SDK and a handler for serving the tools from your own HTTP endpoint. A separate PostgREST MCP server is included.

- **+** Hosted endpoint with OAuth login; client config is a short JSON block
- **+** URL options for project_ref, read_only and feature groups limit what the LLM can do
- **+** createToolSchemas() gives typed tool inputs and outputs for Vercel AI SDK
- **+** createSupabaseMcpHandler() allows serving the tools from your own endpoint
- **−** CLI and self-hosted setups expose only a limited tool subset and no OAuth 2.1
- **−** Connects an LLM to real projects; README points to security risks to mitigate
- **−** Does not send structuredContent; AI SDK parses JSON from text content
- **−** Self-hosted handler rejects clients that only speak the 2025-era protocol (HTTP 400)

<sub>no GPU · Needs Supabase project, Supabase account (OAuth) · [Repo](https://github.com/supabase/mcp) · [📖 Docs ↗](https://supabase.com/docs/guides/getting-started/mcp) · [🌐 Site ↗](https://supabase.com/mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase-mcp/)</sub>

<a name="mcp-memory-service"></a>
### #&#8288;34 [mcp-memory-service](https://github.com/doobidoo/mcp-memory-service) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

**Self-hosted memory service for AI agents with REST API and MCP.**

Python service that stores and retrieves agent memories through a REST API, MCP, a CLI and a web dashboard on port 8000. It combines local ONNX embeddings with BM25 search, a typed knowledge graph, and scheduled consolidation, on SQLite by default. Hybrid (Cloudflare or another instance) and Milvus backends are optional.

- **+** Same store reachable via REST, MCP, CLI and dashboard; no MCP client needed for LangGraph or CrewAI
- **+** Embeddings run locally with ONNX and SQLite; core operations stay on your machine
- **+** Backends: SQLite, Cloudflare, Hybrid sync, Milvus; also imports mem0 exports
- **+** Binds to 127.0.0.1 by default; OAuth 2.0 supported for remote claude.ai and ChatGPT use
- **−** Maintained by one person, per the README
- **−** No Docker or compose file detected in the repository
- **−** Summaries, bootstrap profiles and quality scoring need extra env flags or an LLM endpoint
- **−** Bootstrap profiles are not isolated by project

<sub>no GPU · Needs SQLite, Cloudflare (optional), Milvus (optional), OpenAI-compatible LLM endpoint (optional) · Models: ONNX embeddings (local), OpenAI-compatible endpoints (Ollama, LiteLLM, vLLM) for quality scoring · port 8000 · [Repo](https://github.com/doobidoo/mcp-memory-service) · [📖 Docs ↗](https://github.com/doobidoo/mcp-memory-service/blob/main/docs/setup-guide.md) · [🌐 Site ↗](https://mcpmemory.services) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-memory-service/)</sub>

<a name="mobilebuildmcp"></a>
### #&#8288;35 [mobilebuildmcp](https://github.com/getsentry/mobilebuildmcp) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

**MCP server and CLI for building and testing iOS and macOS projects.**

MobileBuildMCP is a TypeScript MCP server and CLI that lets coding agents drive xcodebuild for iOS and macOS projects. It builds for simulators, prepares and runs portable test products, and supports device tools. The CLI uses a per-workspace daemon for stateful work such as log capture and debugging, and optional agent skills install with `mobilebuildmcp init`.

- **+** One package provides both an MCP server and a direct terminal CLI
- **+** Installs via Homebrew or npm; npx runs the MCP server without a global install
- **+** Can build test products separately, then run them on a named simulator
- **+** Optional MCP and CLI skills prime agents on tool usage
- **−** macOS only; requires macOS 14.5+ and Xcode 16.x or later
- **−** Device tools need code signing already configured in Xcode
- **−** Sends runtime error telemetry to Sentry unless you opt out
- **−** Docs live in a separate repo, not in this README

<sub>no GPU · Needs macOS 14.5+, Xcode 16.x+, Node.js 18+ (not needed with Homebrew) · [Repo](https://github.com/getsentry/mobilebuildmcp) · [📖 Docs ↗](https://github.com/getsentry/xcodebuildmcp.com/blob/main/app/docs/_content/installation.mdx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mobilebuildmcp/)</sub>

<a name="mcp-server-cloudflare"></a>
### #&#8288;36 [mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · Apache-2.0 · Oct 2026</sub>

**Remote MCP servers for Cloudflare docs, browser rendering, containers and security.**

A set of remote MCP servers hosted under *.mcp.cloudflare.com that let MCP clients such as Cursor or Claude read and change Cloudflare account resources in natural language. Servers cover docs lookup, Browser Run (page fetch, markdown, screenshots), sandbox containers, DEX, CASB and the Cloudflare blog. All expose a stateless Streamable HTTP handler at /mcp and /sse; the broader API server lives in cloudflare/mcp.

- **+** Hosted endpoints per product area; any remote-capable MCP client connects by URL
- **+** Typed, purpose-built tools per domain: docs, browser, containers, DEX, CASB
- **+** Stateless Streamable HTTP handler at /mcp shared across all servers
- **+** Works with the OpenAI Responses API using a scoped Cloudflare API token
- **−** Requires a Cloudflare account; some features need a paid Workers plan
- **−** Ten servers are deprecated, including Observability, Radar and AI Gateway
- **−** Recommended broad-coverage API server is in a separate repository
- **−** Legacy SSE GET on /sse returns 410 Gone, so older clients need reconfiguring

<sub>no GPU · Needs Cloudflare account, Cloudflare API token · [Repo](https://github.com/cloudflare/mcp-server-cloudflare) · [▶️ Demo ↗](https://playground.ai.cloudflare.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-cloudflare/)</sub>

<a name="google-workspace-mcp"></a>
### #&#8288;37 [google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**MCP server exposing Gmail, Drive, Calendar, Docs, Sheets and more to AI clients.**

Python MCP server with 120+ tools across twelve Google Workspace services, including Gmail, Drive, Calendar, Docs, Sheets, Slides, Forms, Tasks, Contacts, Chat and Apps Script. It runs over stdio or streamable HTTP, supports OAuth 2.1 multi-user auth, and ships a CLI (workspace-cli). Tool tiers (core, extended, complete), read-only mode and per-service selection keep the tool list small.

- **+** Tool tiers, --tools, --read-only and --disabled-tools limit what the model sees
- **+** OAuth 2.1 multi-user auth, stateless mode, service accounts and external OAuth provider support
- **+** MIT licensed with no built-in telemetry; OpenTelemetry tracing is optional and off by default
- **+** Includes workspace-cli and a bundled Claude Code skill for tool routing
- **−** Requires your own Google Cloud project, enabled APIs and OAuth client credentials
- **−** Google Chat needs a one-time Chat app configuration and a Workspace account
- **−** Complete tier loads 120+ tools, which can bloat model context
- **−** OAuth 2.1 mode requires HTTP transport, so stdio-only clients use the legacy auth path

<sub>no GPU · Docker + Compose · Needs Google Cloud project with OAuth client, Google Workspace APIs, Valkey/Redis (optional) · port 8000 · [Repo](https://github.com/taylorwilsdon/google_workspace_mcp) · [📖 Docs ↗](https://workspacemcp.com/docs) · [🌐 Site ↗](https://workspacemcp.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-workspace-mcp/)</sub>

<a name="cocoindex-code"></a>
### #&#8288;38 [cocoindex-code](https://github.com/cocoindex-io/cocoindex-code) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · Apache-2.0 · Oct 2026</sub>

**Semantic code search CLI, MCP server and skill for coding agents.**

cocoindex-code indexes a repository into AST-based chunks and answers natural-language queries through the `ccc` CLI, an MCP `search` tool, or a `ccc` skill for Claude Code, Codex, Cursor and others. Embeddings run locally via sentence-transformers or through a cloud provider with LiteLLM. It also includes `ccc grep` for structural pattern search that needs no index.

- **+** Works as CLI, MCP stdio server, or skill, with plugin bundles for Claude Code, Grok and Oh My Pi
- **+** Local embeddings need no API key; default model is Snowflake/snowflake-arctic-embed-xs
- **+** Search filters by language and path glob, with pagination and optional index refresh
- **+** `ccc grep` does structural syntax-tree matching locally without index, daemon or embeddings
- **−** Full install pulls about 1 GB of torch and transformers; full Docker image is about 5 GB
- **−** Docker on macOS runs local embeddings on CPU only, with no Metal access
- **−** `ccc grep` depends on a cocoindex feature that may not be in a released version
- **−** The 70% token saving claim comes with no benchmark in the README

<sub>GPU optional · Docker + Compose · Needs CocoIndex, Python (pipx or uv), LiteLLM cloud embedding provider (slim variant), Docker (optional) · Models: sentence-transformers (local), Snowflake/snowflake-arctic-embed-xs, LiteLLM: OpenAI, Voyage, Gemini, Ollama · [Repo](https://github.com/cocoindex-io/cocoindex-code) · [📖 Docs ↗](https://cocoindex.io/docs/getting_started/quickstart) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cocoindex-code/)</sub>

<a name="cli-anything"></a>
### #&#8288;39 [cli-anything](https://github.com/hkuds/cli-anything) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 57k · Apache-2.0 · Sep 2026</sub>

**Generates command-line wrappers so AI agents can drive desktop and backend software.**

CLI-Anything runs a 7-phase generator inside a coding agent such as Claude Code, Cursor or Codex. It produces a Python (Click) CLI harness with JSON output and a SKILL.md for a target application or codebase. A companion package, cli-anything-hub, installs community-built CLIs from a registry, covering GIMP, Blender, LibreOffice, QGIS, n8n and others.

- **+** Ready-made registry of community CLIs installable with `cli-hub install <name>`
- **+** Generated CLIs emit structured JSON and ship a SKILL.md for agent discovery
- **+** Works with several agent hosts: Claude Code, Codex, Cursor, OpenClaw, Pi, OpenCode
- **+** Apache-2.0 license; README reports 2,461 passing tests
- **−** Many CLIs only wrap an upstream app, which must be installed separately
- **−** Generating a new CLI requires a supported AI coding agent, so output quality varies
- **−** Harness quality is per-CLI and community-contributed; test depth differs between harnesses
- **−** Windows use with Claude Code needs Git for Windows or WSL for bash and cygpath

<sub>no GPU · Needs Python 3.10+, A supported AI coding agent (for generating new CLIs), Upstream apps the chosen CLI wraps (e.g. GIMP, Blender, LibreOffice) · safety checks passed 9 of 13 · [Repo](https://github.com/hkuds/cli-anything) · [📖 Docs ↗](https://arxiv.org/abs/2606.03854) · [🌐 Site ↗](https://hkuds.github.io/CLI-Anything/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-anything/)</sub>

<a name="dashboard-icons"></a>
### #&#8288;40 [dashboard-icons](https://github.com/homarr-labs/dashboard-icons) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · Apache-2.0 · Oct 2026</sub>

**Icon library for dashboards with CDN links and a hosted MCP server.**

A collection of over 3,400 service and application logos, published as SVG, PNG and WEBP with light and dark variants, and served through jsDelivr or raw GitHub URLs. A hosted MCP server at dashboardicons.com/api/mcp lets coding agents match services in a docker-compose.yml to icons and return CDN links. It also searches the selfh.st, LobeHub and Simple Icons catalogs.

- **+** Predictable kebab-case URLs on jsDelivr; PNG and WEBP are 512px height
- **+** Hosted MCP server needs no API key and works with Claude Code, Codex and Cursor
- **+** MCP can match every service in a docker-compose.yml to icons in one call
- **+** Used by Homarr, Homepage and Dashy
- **−** Icon submissions go through the website form only; GitHub issues are not accepted
- **−** Approved icons go live only after a maintainer publishes them
- **−** Brand icons stay subject to third-party trademark rules
- **−** MCP server is hosted by the project; no self-hosting instructions in the README

<sub>no GPU · Needs jsDelivr CDN, dashboardicons.com MCP endpoint · [Repo](https://github.com/homarr-labs/dashboard-icons) · [🌐 Site ↗](https://dashboardicons.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dashboard-icons/)</sub>

<a name="webcodex"></a>
### #&#8288;41 [webcodex](https://github.com/yyjeqhc/webcodex) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · Apache-2.0 · Oct 2026</sub>

**Self-hosted MCP runtime that lets ChatGPT or Claude work in your local repos.**

WebCodex is a Rust Server and Runner pair that exposes development tools over MCP to cloud AI clients such as ChatGPT and Claude. The Server authenticates requests and routes them to a Runner on the machine that holds the repository, where the agent can read and edit files, run tests and compilers, and use Git. A browser Runtime Console and a Desktop app cover jobs, sessions and diff review.

- **+** Repository and toolchain stay on your machine, not in a hosted workspace
- **+** Server/Runner split lets several computers join one Server
- **+** `webcodex share` gives a temporary one-repository trial
- **+** Long-running jobs, sessions and Git diffs are reviewable in a browser console
- **−** Unified installers are still under development; native install acceptance is incomplete
- **−** Tool results and requested file content can still be returned to the AI client
- **−** Can edit files and run commands, so project roots must be scoped carefully
- **−** README says maintainer response time may vary

<sub>no GPU · Docker + Compose · Needs Node.js 18+, Git, Rust toolchain (build from source) · Models: ChatGPT, Claude, MCP clients · [Repo](https://github.com/yyjeqhc/webcodex) · [📖 Docs ↗](https://github.com/yyjeqhc/webcodex/blob/main/docs/INDEX.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/webcodex/)</sub>

<a name="ida-pro-mcp"></a>
### #&#8288;42 [ida-pro-mcp](https://github.com/mrexodia/ida-pro-mcp) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (77) · Freshness: active (83) · Maintenance: fair (57) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Sep 2026</sub>

**MCP server that lets LLM clients decompile and annotate binaries in IDA Pro.**

Exposes IDA Pro to MCP clients as tools for decompiling, disassembling, cross-references, renaming, retyping, commenting and patching. It runs as an IDA GUI plugin or as a headless idalib supervisor with one persistent worker process per open database (default max 4). The README now points to the official Hex-Rays IDA MCP Server as the recommended alternative.

- **+** Broad tool set: decompile, disasm, xrefs, rename, set_type, patch, find_bytes, py_eval, debugger
- **+** Headless idalib mode with multiple databases, each in its own persistent worker
- **+** Install paths for Claude Code, Codex and Kimi Code plus a config generator for other clients
- **+** Batch-first API with paginated searches (default limit 1000, max 10000) to avoid token overflow
- **−** Author recommends the official Hex-Rays IDA MCP Server instead
- **−** Requires a licensed IDA Pro 8.3+; IDA Free is not supported
- **−** GUI plugin install is no longer recommended and will eventually be deprecated
- **−** Last release is 2025-10-06; installs track the main branch

<sub>no GPU · Needs IDA Pro 8.3+ (9 recommended), idalib, uv, Python 3.11+ · port 13337 · [Repo](https://github.com/mrexodia/ida-pro-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ida-pro-mcp/)</sub>

<a name="ext-apps"></a>
### #&#8288;43 [ext-apps](https://github.com/modelcontextprotocol/ext-apps) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · custom license · Oct 2026</sub>

**SDK for rendering interactive MCP tool UIs inline in chat clients.**

TypeScript SDK and spec for the MCP Apps extension, where an MCP tool declares a ui:// HTML resource that the host renders in a sandboxed iframe. Packages cover building Views (with React hooks), embedding them in a host, and registering UI tools on a server. The repo also ships about 20 example servers, starter templates for six frameworks, and four Agent Skills.

- **+** Four npm entry points cover View, React hooks, host app-bridge and server helpers
- **+** Starter templates for React, Vue, Svelte, Preact, Solid and vanilla JS
- **+** Example servers (map, PDF, Three.js, QR) run via npx with --stdio
- **+** Wire protocol unchanged between ext-apps 1.x and 2.x
- **−** No supported host implementation; only the basic-host example is included
- **−** Host support varies, since it is an extension to core MCP
- **−** Requires Node.js 20+, MCP SDK 2.x peer packages and zod 4
- **−** License detected as NOASSERTION, while the README badge says Apache 2.0

<sub>no GPU · Needs Node.js 20+, @modelcontextprotocol/client ^2.0.0, zod ^4.2.0 · port 8080 · [Repo](https://github.com/modelcontextprotocol/ext-apps) · [📖 Docs ↗](https://apps.extensions.modelcontextprotocol.io/api/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ext-apps/)</sub>

<a name="x64dbg-mcp-server"></a>
### #&#8288;44 [x64dbg-mcp-server](https://github.com/duty1g/x64dbg-mcp-server) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

**x64dbg plugin that exposes debugger control to MCP clients over HTTP.**

A native plugin written in Zig that runs an MCP server inside x64dbg, letting an AI assistant set breakpoints, step code, read and patch memory, and inspect registers, modules and the PEB. It supports Streamable HTTP and SSE transports with mandatory Bearer token auth. The README lists 84 tools in the features section but documents 72 in the tool tables.

- **+** Runs inside x64dbg's process, so tools call the debugger SDK directly
- **+** No runtime dependencies; separate x32 and x64 plugin builds from one codebase
- **+** Bearer token auto-generated on first run and required on every request
- **+** Covers breakpoints, tracing, memory patching, PE analysis, OEP detection and module dumping
- **−** Windows-only target, since it is an x64dbg plugin
- **−** Plain HTTP with no TLS; README warns against untrusted networks
- **−** Default bind address is 0.0.0.0, exposing full debugger control to the network
- **−** README tool count is inconsistent: 84 in features, 72 in the tool list

<sub>no GPU · Needs x64dbg · port 9094 · [Repo](https://github.com/duty1g/x64dbg-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/x64dbg-mcp-server/)</sub>

<a name="codedb"></a>
### #&#8288;45 [codedb](https://github.com/justrach/codedb) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · BSD-3-Clause · Sep 2026</sub>

**MCP server that gives coding agents symbols, callers and repo context.**

codedb is a Zig code-intelligence engine that indexes a local repository and serves symbol lookup, callers, outlines, dependency graphs and trigram search to coding agents over MCP (stdio) or a localhost HTTP server. It has no edit capability; the client uses its own tools to change code. Default hybrid retrieval in codedb_context uses hosted embeddings, and semantic=local keeps it on-device.

- **+** Native binaries for macOS, Linux and Windows; installer registers MCP in about 16 clients
- **+** Structural queries run locally: symbols, callers, call paths, outlines, dependency graph, trigram search
- **+** Reported cold index of 6,315 files in 346 ms on an M4 Pro
- **+** Parsers for Zig, C/C++, Python, TS/JS, Rust, Go, PHP, Ruby and more; CLI and HTTP also available
- **−** Marked alpha: APIs and snapshot formats can change
- **−** Default hybrid retrieval sends data to hosted embeddings unless semantic=local is set
- **−** Each MCP process runs its own watcher, so many clients multiply background work
- **−** Installer adds a Claude Code PreToolUse hook by default; opting out needs an env var or file

<sub>no GPU · Needs Hosted embeddings service (default hybrid retrieval), DeepWiki remote MCP (optional, installer-registered) · port 7719 · [Repo](https://github.com/justrach/codedb) · [📖 Docs ↗](https://github.com/justrach/codedb/blob/main/docs/mcp.md) · [🌐 Site ↗](https://codedb.codegraff.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codedb/)</sub>

<a name="open-computer-use"></a>
### #&#8288;46 [open-computer-use](https://github.com/ifuryst/open-computer-use) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**MCP server that lets AI agents control desktop apps on macOS, Linux and Windows.**

open-computer-use exposes Computer Use as an MCP server, built on the accessibility APIs rather than screenshots alone. It ships as an npm package (`open-computer-use` or `ocu`) with installers for Codex, Claude Code, Gemini CLI and opencode. The `ocu mcp` command serves nine core native tools, plus a `query` tool on macOS.

- **+** Runs on macOS 14+, Linux and Windows from one npm package
- **+** One-command MCP installers for Codex, Claude Code, Gemini CLI and opencode
- **+** CLI can call single tools, run JS scripts or open a REPL for testing
- **+** macOS `query` finds controls by text or role without taking a screenshot
- **−** macOS needs Accessibility and Screen Recording permissions granted manually
- **−** README says the project is nearly 100% AI-generated
- **−** Needs Node.js 18 or newer for the npm launcher
- **−** Linux and Windows setup details are not covered in the README

<sub>no GPU · Needs Node.js 18+, macOS 14.0+ (macOS only) · [Repo](https://github.com/ifuryst/open-computer-use) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-computer-use/)</sub>

<a name="jadx-ai-mcp"></a>
### #&#8288;47 [jadx-ai-mcp](https://github.com/zinja-coder/jadx-ai-mcp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · Apache-2.0 · Oct 2026</sub>

**JADX plugin and MCP server that lets LLMs inspect decompiled Android APKs.**

A JADX-GUI plugin paired with a separate Python MCP server (jadx-mcp-server). The server relays MCP tool calls over HTTP to the plugin, so an LLM client can read classes, smali, manifest and resources, search and cross-reference code, rename symbols, add comments and read debugger state in the open JADX project.

- **+** About 30 MCP tools: source, smali, manifest, resources, xrefs, renaming, comments, debugger state
- **+** One-command plugin install: jadx plugins --install github:zinja-coder:jadx-ai-mcp
- **+** Works over stdio (Claude Desktop, Cherry Studio, LM Studio) or an optional HTTP mode
- **+** Plugin and MCP server can run on different machines via --jadx-host and --jadx-port
- **−** Two components to set up: the JADX plugin and the separate Python MCP server
- **−** HTTP mode on non-localhost binds has no authentication, per the README's own warning
- **−** Needs a running JADX-GUI session with the project open
- **−** Android APK analysis only, not general code navigation

<sub>no GPU · Needs JADX GUI, Java 11+, Python 3.10+, uv, fastmcp, httpx · Models: Claude Desktop, Cherry Studio, LM Studio, any MCP client · port 8651 · [Repo](https://github.com/zinja-coder/jadx-ai-mcp) · [📖 Docs ↗](https://jadx-ai-mcp.readthedocs.io/en/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jadx-ai-mcp/)</sub>

<a name="gitlab-mcp"></a>
### #&#8288;48 [gitlab-mcp](https://github.com/zereight/gitlab-mcp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**MCP server exposing GitLab projects, merge requests, issues and pipelines to agents.**

TypeScript MCP server that wraps the GitLab API with 276 tools covering projects, merge requests, issues, pipelines, wiki, releases, tags and milestones. It runs over stdio, SSE or Streamable HTTP and authenticates with a personal access token, OAuth2, an MCP OAuth proxy, or per-request remote authorization. Toolsets, permission modes and a regex deny list limit what an agent can call.

- **+** Four auth modes: PAT, local OAuth2, MCP OAuth proxy, per-request remote authorization
- **+** Permission modes readonly, modify and full, plus toolset, allow-list and deny-regex filtering
- **+** Works with self-hosted GitLab through a configurable API URL
- **+** Ships as npm package, Homebrew formula, Nix flake and a Claude Desktop .mcpb bundle
- **−** 276 tools is large; default is a lean core toolset and others must be enabled
- **−** The gitlab_api_request tool bypasses group and project restrictions and is exposed to prompt injection
- **−** Several legacy flags (USE_GITLAB_WIKI, USE_MILESTONE, USE_PIPELINE) are deprecated and removed in v3.0.0
- **−** README is long, with many env vars and flags spread across docs

<sub>no GPU · Docker + Compose · Needs GitLab instance, Node.js >=18.17, GitLab personal access token or OAuth · [Repo](https://github.com/zereight/gitlab-mcp) · [📖 Docs ↗](https://zereight.github.io/gitlab-mcp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitlab-mcp/)</sub>

<a name="mcp-server-kubernetes"></a>
### #&#8288;49 [mcp-server-kubernetes](https://github.com/flux159/mcp-server-kubernetes) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**MCP server that lets coding agents manage Kubernetes clusters via kubectl and Helm.**

TypeScript MCP server that wraps kubectl and Helm so an MCP client can get, describe, apply, scale, patch and delete resources, read logs, port-forward and drain nodes. It reads kubeconfig (default ~/.kube/config) and runs over stdio via npx, with an optional Streamable HTTP mode on port 3000. A non-destructive mode removes delete, drain and exec tools.

- **+** Covers kubectl, Helm, port-forward, node drain and pod cleanup in one server
- **+** Non-destructive mode via env var removes delete, drain, generic and exec tools
- **+** Opt-in OpenTelemetry tracing of tool calls to any OTLP backend
- **+** Install steps for Claude Code, Codex, Cursor, VS Code and mcpb
- **−** Requires kubectl on PATH and a working kubeconfig; Helm needed for chart tools
- **−** Streamable HTTP transport is gated behind an ENABLE_UNSAFE_ env flag
- **−** Secrets masking applies to kubectl get secrets only, not logs
- **−** kubectl_generic can run arbitrary kubectl commands outside non-destructive mode

<sub>no GPU · Docker · Needs kubectl, kubeconfig, Helm v3 (optional), Node.js/npx · port 3000 · [Repo](https://github.com/flux159/mcp-server-kubernetes) · [📖 Docs ↗](https://github.com/Flux159/mcp-server-kubernetes/tree/main/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-kubernetes/)</sub>

<a name="cursor-talk-to-figma-mcp"></a>
### #&#8288;50 [cursor-talk-to-figma-mcp](https://github.com/grab/cursor-talk-to-figma-mcp) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Jul 2026</sub>

**MCP server that lets Cursor or Claude Code read and edit Figma files.**

Connects an AI agent to Figma through three parts: a TypeScript MCP server, a WebSocket relay, and a Figma plugin. The agent joins a channel and calls tools to read document and node info, create frames and text, set auto-layout and styles, replace text in bulk, and export nodes as images. It also ships MCP prompts for design, text replacement and annotation workflows.

- **+** Broad tool set: about 40 tools covering reading, creation, auto layout, styling and components
- **+** Bulk text replacement and instance override propagation cut repetitive edits
- **+** Bundled MCP prompts guide multi-step tasks like annotation conversion and prototype-to-connector mapping
- **+** Plugin is published on the Figma community page, or can be linked locally
- **−** Needs three pieces running: MCP server, WebSocket server (bun socket) and Figma plugin
- **−** Requires Bun; Windows WSL needs a manual edit to src/socket.ts
- **−** Image export is limited and returns base64 as text
- **−** No tagged releases; setup docs focus on Cursor, with Claude Code only mentioned

<sub>no GPU · Docker · Needs Bun, Figma, WebSocket server (bun socket), Figma plugin · Models: Cursor, Claude Code · [Repo](https://github.com/grab/cursor-talk-to-figma-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cursor-talk-to-figma-mcp/)</sub>

<a name="lanhu-mcp"></a>
### #&#8288;51 [lanhu-mcp](https://github.com/dsphper/lanhu-mcp) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Oct 2026</sub>

**MCP server that feeds Lanhu requirement docs and designs to coding agents.**

A FastMCP server in Python that reads Lanhu (蓝湖) Axure requirement pages and UI designs using a session cookie. It returns screenshots, region crops, style parameters, HTML+CSS references and exported slices to MCP clients such as Cursor, Claude Code and Windsurf. It also includes a shared message board so several developers' agents can read the same notes, with optional Feishu notifications.

- **+** Region tools crop requirement pages and designs by text, block ID or coordinates
- **+** Runs over HTTP on port 8000 or on demand via stdio scripts, no Docker required
- **+** Caches results by document version and downloads only changed assets
- **+** Shared message board with five message types, regex search and Feishu @mentions
- **−** Needs a Lanhu account cookie copied manually from browser developer tools
- **−** Requires a vision-capable model; text-only models are not supported
- **−** Message board data is stored as JSON files; README shows no auth on the HTTP endpoint
- **−** Main README is in Chinese; the English version is a separate file

<sub>no GPU · Docker + Compose · Needs Lanhu account cookie, Playwright Chromium, Feishu webhook (optional) · Models: Claude, GPT, Gemini, Kimi, Qwen · port 8000 · [Repo](https://github.com/dsphper/lanhu-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lanhu-mcp/)</sub>

<a name="gortex"></a>
### #&#8288;52 [gortex](https://github.com/zzet/gortex) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

**Code knowledge graph exposed to coding agents through MCP, CLI and a web UI.**

Gortex indexes repositories with tree-sitter (257 languages/grammars) into a persistent SQLite-backed graph of symbols, call chains, HTTP routes and cross-repo contracts. A long-running daemon serves it to coding agents as configurable MCP tools (README cites 175 and also 100+), plus a CLI and a Next.js web UI. `gortex init` configures 19 or more detected agents such as Claude Code, Cursor and Codex CLI.

- **+** Single static Go binary; semantic search works with embedded GloVe, no model download
- **+** Multi-repo graph with cross-repo contract matching (HTTP, gRPC, GraphQL, Kafka, and more)
- **+** Indexed vscode (10.7k files) in about 1 minute with 580 MB peak heap
- **+** One install configures every detected agent; telemetry is off by default
- **−** Source build needs Go 1.26+ and CGO for tree-sitter bindings
- **−** Large repos are memory-heavy: Linux kernel took about 3 min and 5.07 GB heap
- **−** The 50x token saving claim is the project's own; independent verification is unknown
- **−** README gives inconsistent tool counts (175 vs 100+) and agent counts (19 vs 20)

<sub>no GPU · Models: llama.cpp, Anthropic, OpenAI, Ollama, Gemini · [Repo](https://github.com/zzet/gortex) · [📖 Docs ↗](https://github.com/zzet/gortex/blob/main/docs/onboarding.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gortex/)</sub>

<a name="artemis"></a>
### #&#8288;53 [artemis](https://github.com/google/artemis) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Sep 2026</sub>

**Drives real Android phones from natural language via CLI, web console, SDK or MCP.**

ARTEMIS runs a multimodal agent that operates an Android device or emulator over ADB from plain-language instructions. It ships an MCP server for IDEs such as Claude Code, Codex, Antigravity and Windsurf, plus a CLI, a web console on port 8000 and a Python client. Two profiles exist: Flash, a reactive loop at about 3–5s per step, and Pro, a planner/operator/checker graph at about 15–40s per step.

- **+** Native MCP server with install commands for Claude Code, Cursor, Codex, Windsurf and others
- **+** Flash and Pro profiles trade speed against planning and checkpoint verification
- **+** Falls back from accessibility tree to OCR and visual locating for Compose and Flutter UIs
- **+** Python client with no runtime dependencies for pytest or CI use
- **−** Android only; iOS support is a roadmap item
- **−** Installs an accessibility helper app on the phone at first task
- **−** Flash profile has no task plan, safety net, final report or ADB shell
- **−** Needs an external multimodal model; hardware and cost requirements are unknown

<sub>Docker · Needs ADB, scrcpy, FFmpeg, uv, Python 3.12+, Android device or emulator with USB debugging · Models: Gemini, Claude, GPT-4o, Qwen-VL · port 8000 · safety checks passed 12 of 17 · [Repo](https://github.com/google/artemis) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/artemis/)</sub>

<a name="codexpro"></a>
### #&#8288;54 [codexpro](https://github.com/rebel0789/codexpro) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Local MCP server that lets ChatGPT read and edit allowed repos.**

CodexPro is a Node.js MCP server that connects a ChatGPT session to repositories on your machine that you explicitly allow. ChatGPT can search, edit, apply patches, run allowlisted bash checks, review diffs and write handoff plans under .ai-bridge. Code analysis runs locally without a model API key or vector database. ChatGPT web reaches it through an HTTPS tunnel such as Cloudflare, ngrok or Tailscale.

- **+** Local symbol, references and impact search with no embedding service or vector database
- **+** Separate controls for reads, writes and commands; blocked paths include .env and .git
- **+** One process can serve several allowed repos via repeated --project flags
- **+** Supports Cloudflare, ngrok, Tailscale and named tunnels, or local-only mode
- **−** ChatGPT web needs a public HTTPS URL, so a tunnel must be exposed
- **−** Requires a ChatGPT account that can create custom MCP plugins in Developer mode
- **−** Auth is a token inside the Server URL; a leaked URL grants access
- **−** Declarations recognized for nine language families; others get only lexical search

<sub>no GPU · Needs Node.js 20+, ChatGPT account with custom MCP plugins, HTTPS tunnel (Cloudflare, ngrok or Tailscale Funnel) · Models: ChatGPT · [Repo](https://github.com/rebel0789/codexpro) · [📖 Docs ↗](https://rebel0789.github.io/codexpro/) · [🌐 Site ↗](https://rebel0789.github.io/codexpro/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codexpro/)</sub>

<a name="chunkhound"></a>
### #&#8288;55 [chunkhound](https://github.com/chunkhound/chunkhound) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Semantic code search and cited research over a codebase and its git history.**

ChunkHound indexes a repository with Tree-sitter and answers questions about it through a CLI, with source citations. It supports regex and semantic search, research over commit ranges, tags or the last N commits, and web search for external docs. Semantic search needs an embedding provider; deep research also needs an LLM provider.

- **+** Searches git history by last N commits, commit hash, tag or range
- **+** Regex search works with no API keys or providers
- **+** Ollama can serve embeddings locally, avoiding sending code to external services
- **+** Parses many languages through Tree-sitter, including Python, TypeScript, Go, Rust and C/C++
- **−** Semantic search requires an embedding provider; deep research also needs an LLM and reranking
- **−** Editor and agent integration is documented only on the external docs site
- **−** README gives no RAM, index size or performance figures
- **−** README states the code is 100% AI generated

<sub>Needs Python 3.10+, uv, VoyageAI, OpenAI or Ollama for embeddings, Claude Code CLI, Codex CLI, Anthropic, OpenAI or Grok for LLM · Models: VoyageAI, OpenAI, Ollama, Anthropic, Grok · [Repo](https://github.com/chunkhound/chunkhound) · [📖 Docs ↗](https://chunkhound.ai/docs/getting-started/) · [🌐 Site ↗](https://chunkhound.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chunkhound/)</sub>

<a name="stealth-browser-mcp"></a>
### #&#8288;56 [stealth-browser-mcp](https://github.com/vibheksoni/stealth-browser-mcp) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (42) · Freshness: active (94) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Oct 2026</sub>

**MCP server that drives real Chrome via nodriver to get past anti-bot checks.**

Python MCP server built on FastMCP, nodriver and the Chrome DevTools Protocol that lets an AI agent control a real Chrome, Chromium or Edge instance. It exposes 101 tools for navigation, element interaction, network inspection, element cloning, cookies and CDP execution. Sections can be disabled, down to a 21-tool core, and it runs over stdio or HTTP with an optional bearer token.

- **+** Modular: full 101 tools, 21-tool --minimal mode, or per-section --disable-* flags
- **+** Network inspection and restricted Python hooks to intercept, block, redirect or modify requests
- **+** Element cloning extracts CSS, DOM structure, events, animations and assets via CDP
- **+** Runs over stdio or HTTP; HTTP supports a bearer token via environment variable
- **−** Anti-bot results vary by site, region, browser and detector version, per the README
- **−** Exposes CDP, page JS, cookies and interception; README says to trust only local clients
- **−** Needs a local Chrome, Chromium or Edge install and a Python 3.10+ venv
- **−** README carries a paid sponsor placement for a proxy provider

<sub>no GPU · Docker · Needs Python 3.10+, Chrome, Chromium or Edge, nodriver, FastMCP · port 8000 · [Repo](https://github.com/vibheksoni/stealth-browser-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/stealth-browser-mcp/)</sub>

<a name="mcp-unity"></a>
### #&#8288;57 [mcp-unity](https://github.com/codergamester/mcp-unity) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**MCP server that lets coding agents drive the Unity Editor.**

A Unity package plus a Node.js MCP server that connects to the Editor over WebSocket. AI clients such as Cursor, Claude Code, Codex CLI, GitHub Copilot, Windsurf and OpenCode can manage scenes, GameObjects, components, materials and prefabs, run Unity Test Runner tests, read console logs and control play mode. It also exposes resources, prompts and a batch tool with optional rollback.

- **+** About 30 tools covering scenes, GameObjects, transforms, materials, prefabs, packages and tests
- **+** Editor Configure buttons write client configs, with project-relative variants to commit to git
- **+** batch_execute groups multiple operations in one request with optional rollback on failure
- **+** Read-only resources such as unity://scenes-hierarchy, unity://logs and unity://assets
- **−** Requires Unity 6 or later
- **−** Needs Node.js 18+ in addition to the Unity package
- **−** Server must be started manually from the Editor window
- **−** UPM cache path contains a hash, so configs need updating after package upgrades

<sub>no GPU · Needs Unity 6 or later, Node.js 18 or later, npm 9 or later (for debugging the server) · Models: Cursor, Windsurf, Claude Code, Codex CLI, GitHub Copilot · [Repo](https://github.com/codergamester/mcp-unity) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-unity/)</sub>

<a name="code2prompt"></a>
### #&#8288;58 [code2prompt](https://github.com/mufeedvh/code2prompt) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (65) · Freshness: active (89) · Maintenance: patchy (48) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Sep 2026</sub>

**Rust CLI that packs a codebase into one formatted LLM prompt.**

code2prompt walks a directory, filters files with glob patterns and .gitignore rules, and renders them through Handlebars templates into a single prompt. Output goes to stdout, a file, or the clipboard, with per-file token estimates and optional Git diffs and logs. It ships as a Rust core library, a CLI with a TUI, a Python SDK (code2prompt-rs) and an MCP server, plus an agent skill.

- **+** Handlebars templates let you customize the prompt layout per use case
- **+** Respects .gitignore and supports include/exclude glob patterns
- **+** Includes Git diffs, logs and branch comparisons in the prompt
- **+** Available as CLI, TUI, Python SDK on PyPI, and MCP server
- **−** Token count is an estimate; the full rendered prompt is not re-tokenized
- **−** Agent skill needs the CLI installed separately
- **−** Entity map for the skill requires an optional build feature
- **−** Wayland clipboard support needs a feature flag at build time

<sub>no GPU · [Repo](https://github.com/mufeedvh/code2prompt) · [📖 Docs ↗](https://code2prompt.dev/docs/welcome/) · [🌐 Site ↗](https://code2prompt.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code2prompt/)</sub>

<a name="exa-mcp-server"></a>
### #&#8288;59 [exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Oct 2026</sub>

**Exa web search and page-fetch tools for MCP clients.**

MCP server that gives agents Exa's web search and page fetching, with the page content returned as clean markdown. It is mainly used as the hosted endpoint at mcp.exa.ai/mcp, and the repo also ships as an Agent Plugin with two skills (search, exa-agent). Optional tools add advanced filtered search and multi-step Exa Agent runs.

- **+** Hosted endpoint works anonymously, so no local install is needed to try it
- **+** Default tools are only web_search_exa and web_fetch_exa, so the tool surface stays small
- **+** Supports OAuth, API key in URL, Bearer header or x-api-key header
- **+** Install links or config notes for about a dozen clients, including Cursor, VS Code, Claude and Codex
- **−** Depends on Exa's hosted service and API; anonymous use is rate limited
- **−** Exa Agent (agent_run) requires OAuth or an API key
- **−** Setting the tools parameter replaces the defaults, so you must list all wanted tools
- **−** README does not describe self-hosting or the Docker setup

<sub>no GPU · Docker · Needs Exa API (hosted MCP at mcp.exa.ai), Exa API key or OAuth for higher limits and Exa Agent · [Repo](https://github.com/exa-labs/exa-mcp-server) · [📖 Docs ↗](https://docs.exa.ai/reference/exa-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/exa-mcp-server/)</sub>

<a name="ios-simulator-mcp"></a>
### #&#8288;60 [ios-simulator-mcp](https://github.com/joshuayoes/ios-simulator-mcp) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Aug 2026</sub>

**MCP server that lets agents tap, type, inspect and record the iOS Simulator.**

Node.js MCP server that drives a booted iOS Simulator through Facebook IDB and xcrun simctl. It exposes tools for tapping, typing, swiping, reading the accessibility tree, taking screenshots, recording video, and installing, launching and terminating apps. It is meant for agent-driven QA after a feature change, from clients such as Cursor or Claude Code.

- **+** Covers UI input, accessibility inspection, screenshots, video and app install/launch/terminate in one server
- **+** Runs via npx or pnpm dlx, with no build step for normal use
- **+** Env vars can filter out tools and set the output directory and IDB path
- **+** open_url handles deep links, which shortens agent navigation to a target screen
- **−** macOS only; requires Xcode and installed iOS simulators
- **−** Requires Facebook IDB installed separately
- **−** ui_type accepts ASCII printable characters only
- **−** Versions before 1.3.3 had command injection flaws; older installs must update

<sub>no GPU · Needs Node.js 20+, macOS, Xcode, iOS simulators, Facebook IDB · [Repo](https://github.com/joshuayoes/ios-simulator-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ios-simulator-mcp/)</sub>

<a name="agentdock"></a>
### #&#8288;61 [agentdock](https://github.com/uvwt/agentdock) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Oct 2026</sub>

**MCP server that lets AI assistants use files, shell and Git on your machines.**

AgentDock is a Go MCP server (Streamable HTTP) that gives ChatGPT, Claude or Codex access to files, shell commands, Git, browser automation and Skills on local computers, VPS hosts and containers. Several instances can be connected so one conversation works across machines. It installs from OS packages, Docker or systemd, and pairs with the hosted NexusDock service or a self-hosted one.

- **+** Multiple instances can be connected, so one chat reaches several machines
- **+** Covers files, shell, Git, browser automation and macOS desktop control in one server
- **+** Installers for Docker, Linux, systemd, macOS and Windows
- **+** Bearer token or OAuth on the MCP endpoint; task checkpoints survive interruptions
- **−** Easiest pairing path goes through the NexusDock hosted service
- **−** Desktop control is documented for macOS only
- **−** Shell access on real machines needs careful auth and exposure settings
- **−** README gives no RAM figures or tested model list

<sub>no GPU · Docker + Compose · Needs Cloudflare (optional, for public address), NexusDock (optional, for pairing) · Models: ChatGPT, Claude, Codex · port 8765 · [Repo](https://github.com/uvwt/agentdock) · [📖 Docs ↗](https://docs.nexusdock.co/agentdock/) · [🌐 Site ↗](https://www.nexusdock.co/download/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentdock/)</sub>

<a name="magic-mcp"></a>
### #&#8288;62 [magic-mcp](https://github.com/21st-dev/magic-mcp) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · ISC · Sep 2026</sub>

**MCP proxy that gives coding agents 21st.dev UI component search and generation.**

Formerly the Magic MCP server, this package is now a stdio proxy that forwards MCP messages to the hosted 21st MCP at 21st.dev/api/mcp, so old `@21st-dev/magic` configs keep working. The hosted server offers component, theme and template search, code retrieval, and UI generation when AI access is enabled. The repo is also packaged as a plugin for Claude Code, Codex CLI and Grok Build.

- **+** Legacy Magic tool names are translated, so old agent prompts and mcp.json entries still work
- **+** Installs with one CLI command for Cursor, Claude, VS Code, Windsurf or Codex
- **+** Accepts the API key in several historical argument forms and two environment variables
- **+** Ships plugin manifests for Claude Code, Codex CLI and Grok Build
- **−** Requires a 21st.dev API key and a hosted backend; the server logic is not in this repo
- **−** Old Magic API keys were reset and must be regenerated
- **−** Hosted AI generation is separate from builder access; `generate` is listed only when AI is enabled
- **−** Package is a compatibility shim; the README recommends moving to the 21st CLI

<sub>no GPU · Docker · Needs 21st.dev API key, hosted 21st MCP server (21st.dev/api/mcp), Node.js/npx · [Repo](https://github.com/21st-dev/magic-mcp) · [📖 Docs ↗](https://21st.dev/mcp) · [🌐 Site ↗](https://21st.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/magic-mcp/)</sub>

<a name="claude-context"></a>
### #&#8288;63 [claude-context](https://github.com/zilliztech/claude-context) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (76) · Freshness: active (95) · Maintenance: weak (3) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Jul 2026</sub>

**MCP server adding hybrid semantic code search to coding agents.**

Claude Context indexes a codebase into Milvus or Zilliz Cloud and exposes index_codebase, search_code, clear_index and get_indexing_status tools over stdio MCP. Search combines BM25 with dense vectors, chunks code with an AST splitter, and re-indexes only changed files using Merkle trees. It works with Claude Code, Codex CLI, Gemini CLI, Cursor and other MCP clients.

- **+** Hybrid BM25 plus dense vector search over an indexed repo
- **+** Incremental re-indexing of changed files via Merkle trees
- **+** Embedding choice: OpenAI, VoyageAI, Ollama or Gemini
- **+** Also ships a core npm package and a VS Code extension
- **−** Needs a Milvus or Zilliz Cloud instance; no embedded vector store mentioned
- **−** Default setup sends code to OpenAI for embeddings unless Ollama is configured
- **−** README claims ~40% token reduction from its own evaluation only
- **−** No tagged releases listed on the repository

<sub>no GPU · Needs Node.js >= 20, Milvus or Zilliz Cloud, OpenAI API key (default embedding provider) · Models: OpenAI, VoyageAI, Ollama, Gemini · safety checks passed 7 of 13 · [Repo](https://github.com/zilliztech/claude-context) · [📖 Docs ↗](https://github.com/zilliztech/claude-context/tree/master/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-context/)</sub>

<a name="shadcn-ui-mcp-server"></a>
### #&#8288;64 [shadcn-ui-mcp-server](https://github.com/jpisnice/shadcn-ui-mcp-server) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (39) · Freshness: active (100) · Maintenance: patchy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

**MCP server that gives coding agents shadcn/ui component source, demos and blocks.**

An MCP server that fetches shadcn/ui v4 component source, demos, blocks and metadata from GitHub for AI assistants. It supports React (Radix or Base UI), Svelte, Vue and React Native, and runs over stdio or a stateless Streamable HTTP endpoint at /mcp. GitHub API use is limited to 60 requests/hour without a token and 5000 with one.

- **+** Covers React, Svelte, Vue and React Native component sources from one server
- **+** Runs via npx, stdio, stateless HTTP on port 7423, or a Claude Desktop .mcpb file
- **+** Caching and rate-limit handling for GitHub API calls
- **+** Ships Dockerfile and Docker Compose with a /health endpoint
- **−** Depends on the GitHub API; 60 requests/hour without a token
- **−** Read-only lookup of component code; README does not mention installing into a project
- **−** Legacy SSE transport was removed; --mode sse is only a deprecated alias
- **−** Framework and UI library are chosen at startup, one per server instance

<sub>no GPU · Docker + Compose · Needs GitHub API, Node.js >= 20 · port 7423 · [Repo](https://github.com/jpisnice/shadcn-ui-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shadcn-ui-mcp-server/)</sub>

<a name="jshookmcp"></a>
### #&#8288;65 [jshookmcp](https://github.com/vmoranv/jshookmcp) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Oct 2026</sub>

**MCP server for reverse-engineering web pages, WASM, APKs and processes.**

jshookmcp is a TypeScript MCP server exposing 735 tools across 36 domains: Chromium/Camoufox browser automation over CDP, network interception, JS deobfuscation, WASM disassembly via wabt, Frida/Ghidra/IDA bridges, and APK analysis. A search-first profile (about 3K tokens of metadata) can be promoted to workflow or full (about 109K tokens) as the task grows. It runs over stdio or Streamable HTTP.

- **+** Profile ladder keeps tool metadata near 3K tokens in search mode versus about 109K in full
- **+** Covers browser, network, WASM, APK, Frida and memory tooling in one server
- **+** Streamable HTTP daemon shares browser runtime across agents and restores session state after reconnects
- **+** Hot-reload plugins and declarative workflows extend domains without redeploying
- **−** AGPL-3.0 license restricts use in closed-source network services
- **−** Full profile pulls optional runtimes (ONNX, Z3, Binaryen, Camoufox, Playwright) on demand
- **−** Requires Node.js 22.22.2+ or 24.15+; no Docker or compose files provided
- **−** README says npm package is not yet published; badge is commented out

<sub>no GPU · Needs Node.js 22.22.2+, pnpm 10.x (build from source), ONNX (optional), Z3 (optional), Binaryen (optional), Camoufox (optional), Playwright (optional) · port 3000 · [Repo](https://github.com/vmoranv/jshookmcp) · [📖 Docs ↗](https://vmoranv.github.io/jshookmcp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jshookmcp/)</sub>

<a name="figma-context-mcp"></a>
### #&#8288;66 [figma-context-mcp](https://github.com/glips/figma-context-mcp) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: widely used (81) · Freshness: active (92) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Jun 2026</sub>

**MCP server that feeds simplified Figma layout and style data to coding agents.**

Framelink MCP for Figma (npm package figma-developer-mcp) is an MCP server that fetches file, frame or group data from the Figma API. It trims the response to layout and styling information before passing it to the model, so the agent builds from structured data instead of screenshots. It runs via npx over stdio and needs a Figma personal access token.

- **+** Starts with one npx command; no install or build step needed
- **+** Trims Figma API responses to layout and styling to reduce model context
- **+** Works with MCP clients through a standard config entry, including Cursor
- **+** MIT licensed, written in TypeScript, with a docs site and demo video
- **−** Requires a Figma personal access token, passed as a CLI flag or env var
- **−** README says it is designed specifically for Cursor; other clients are not detailed
- **−** README does not list the exposed tools or parameters; docs are on an external site
- **−** One-shot accuracy claims are not backed by benchmarks in the README

<sub>no GPU · Needs Figma API, Figma personal access token, Node.js (npx) · safety checks passed 16 of 18 · [Repo](https://github.com/glips/figma-context-mcp) · [▶️ Demo ↗](https://youtu.be/6G9yb-LrEqg) · [📖 Docs ↗](https://www.framelink.ai/docs/quickstart) · [🌐 Site ↗](https://www.framelink.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/figma-context-mcp/)</sub>

<a name="claude-task-master"></a>
### #&#8288;67 [claude-task-master](https://github.com/eyaltoledano/claude-task-master) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: widely used (88) · Freshness: recent (73) · Maintenance: weak (6) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Apr 2026</sub>

**Task manager that turns a PRD into tasks for AI coding agents.**

Task Master runs as an MCP server or CLI (task-master) and parses a PRD into structured tasks with dependencies, subtasks, tags and a research command. Editors such as Cursor, Windsurf, VS Code and Q CLI, plus Claude Code, call it to plan and pick the next task. It needs a provider API key (Anthropic, OpenAI, Gemini, Perplexity, xAI, OpenRouter and others) or the Claude Code or Codex CLI.

- **+** Works as an MCP server or CLI, installed with npx or npm
- **+** Separate main, research and fallback models across many providers
- **+** Claude Code and Codex CLI usable without an API key
- **+** TASK_MASTER_TOOLS limits loaded tools to 7, 15 or all 36
- **−** MIT with Commons Clause: no selling it or offering it as a hosted service
- **−** Default loads all 36 tools, about 21,000 tokens of context
- **−** Task quality depends on writing a detailed PRD first
- **−** AI commands need a provider API key or a Claude Code/Codex CLI login

<sub>no GPU · Needs Node.js, npm, AI provider API key or Claude Code/Codex CLI · Models: Anthropic, OpenAI, Google Gemini, Perplexity, xAI · safety checks passed 12 of 17 · [Repo](https://github.com/eyaltoledano/claude-task-master) · [📖 Docs ↗](https://tryhamster.com/docs/taskmaster) · [🌐 Site ↗](https://tryhamster.com/product/taskmaster) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-task-master/)</sub>

<a name="repobrain"></a>
### #&#8288;68 [repobrain](https://github.com/study8677/repobrain) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Per-module AI agents that answer codebase questions with file paths and line numbers.**

RepoBrain runs `rb-refresh` to have model agents read each code module and write knowledge docs into a `.repobrain/` folder in the repo. `rb-ask` then routes a question to the relevant module agent and answers with source references. It works as a CLI, as Claude Code and Codex CLI plugins, or through an optional `rb-mcp` server for other agents and IDEs.

- **+** Knowledge lives in `.repobrain/` inside the repo, so several IDEs and agents share it
- **+** Refresh is incremental after commits and resumes interrupted runs, keeping the last good generation
- **+** Native plugins for Claude Code and Codex CLI, plus CLI/JSON output and optional MCP for other hosts
- **+** Answers cite file paths and line numbers; README links a benchmark on four repos
- **−** Needs a configured model backend (OpenAI-compatible API or a logged-in headless CLI such as Trae)
- **−** First build can take several minutes or longer on large repos and consumes model tokens
- **−** Requires a Git repo with at least one commit and a clean worktree before refresh
- **−** Answers lag behind code until `rb-refresh` is rerun; `rb-ask` only warns when stale

<sub>no GPU · Docker + Compose · Needs Git, OpenAI-compatible API or headless CLI backend (e.g. Trae) · Models: OpenAI-compatible API, Headless CLI backends (Trae) · [Repo](https://github.com/study8677/repobrain) · [📖 Docs ↗](https://deepwiki.com/study8677/repobrain) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repobrain/)</sub>

<a name="mcp-server-chart"></a>
### #&#8288;69 [mcp-server-chart](https://github.com/antvis/mcp-server-chart) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (49) · Freshness: active (95) · Maintenance: patchy (34) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Aug 2026</sub>

**MCP server that renders 26+ AntV chart types from tool calls.**

TypeScript MCP server exposing one tool per chart type (line, bar, pie, sankey, treemap, mind map, fishbone, spreadsheet and others), built on AntV. It runs over stdio, SSE or streamable HTTP, and by default sends chart specs to a hosted AntV rendering service that returns an image URL. A private rendering backend can be set with VIS_REQUEST_SERVER.

- **+** 26+ chart tools, each individually disableable via DISABLED_TOOLS
- **+** Supports stdio, SSE and streamable HTTP transports; default port 1122
- **+** Starts with one npx line in any MCP client config
- **+** Rendering backend can be self-hosted using GPT-Vis-SSR via VIS_REQUEST_SERVER
- **−** Default setup sends chart data to a third-party hosted service (antv-studio.alipay.com)
- **−** Map tools use AMap and only work for locations within China
- **−** Private deployment does not support the three map tools
- **−** Record viewing requires an Alipay mini program to get a SERVICE_ID

<sub>no GPU · Docker + Compose · Needs AntV chart rendering service (antv-studio.alipay.com) or self-hosted GPT-Vis-SSR, AMap service (map tools), Node.js · port 1122 · [Repo](https://github.com/antvis/mcp-server-chart) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-chart/)</sub>

<a name="mysql-mcp-server"></a>
### #&#8288;70 [mysql_mcp_server](https://github.com/designcomputer/mysql_mcp_server) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Aug 2026</sub>

**MCP server that lets AI clients query and explore MySQL databases.**

Python MCP server exposing a MySQL database through tools for running SQL, reading schema metadata and sampling table rows. It runs over stdio or SSE/HTTP, supports SSL and SSH tunneling, and offers a multi-database mode when MYSQL_DATABASE is unset. Two MCP prompts, explore_database and analyze_table, wrap the schema and sampling tools.

- **+** Three tools: execute_sql, get_schema_info, get_table_sample (sample capped at 20 rows)
- **+** Built-in SSH tunneling and SSL modes (DISABLED to VERIFY_IDENTITY) for remote databases
- **+** Identifier whitelist on schema and sample tools; passwords and SSH keys masked in logs
- **+** Installs from PyPI and runs via uvx; stdio and SSE transports
- **−** execute_sql permits INSERT, UPDATE and DELETE; no read-only mode is documented
- **−** SSE transport has no authentication and binds 0.0.0.0 by default
- **−** Single SQL statements only; multi-statement queries like USE db; SELECT fail
- **−** Claude hosts do not find .env; credentials must go in the MCP config env block

<sub>no GPU · Docker · Needs MySQL server, uv (for uvx), SSH jump host (optional) · port 8000 · [Repo](https://github.com/designcomputer/mysql_mcp_server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mysql-mcp-server/)</sub>

<a name="nitrostack"></a>
### #&#8288;71 [nitrostack](https://github.com/nitrocloudofficial/nitrostack) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Oct 2026</sub>

**TypeScript framework for building MCP servers with decorators and DI.**

NitroStack is a TypeScript framework for writing MCP servers. Tools, resources and prompts are declared with decorators, backed by a DI container, guards, interceptors, pipes and Zod validation. It adds JWT, OAuth 2.1 and API key auth, React widgets attached to tool output, a CLI scaffolder, and a separate NitroStudio desktop app for testing.

- **+** Decorator stack combines validation, auth guards, caching and widgets on one tool
- **+** Built-in JWT, OAuth 2.1 and API key authentication
- **+** DI container with singleton, transient and scoped lifecycles
- **+** CLI scaffolds a project with npx @nitrostack/cli init
- **−** TypeScript only; requires Node.js >= 20.18 and npm >= 9
- **−** NitroStudio is a separate desktop download, not an npm package
- **−** Opinionated decorator and DI style adds weight for small servers
- **−** README shows no Docker setup; deployment is left to the docs

<sub>no GPU · Needs Node.js >= 20.18, npm >= 9 · [Repo](https://github.com/nitrocloudofficial/nitrostack) · [📖 Docs ↗](https://docs.nitrostack.ai) · [🌐 Site ↗](https://nitrostack.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nitrostack/)</sub>

<a name="git-mcp"></a>
### #&#8288;72 [git-mcp](https://github.com/idosal/git-mcp) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: popular (69) · Freshness: recent (71) · Maintenance: weak (4) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · May 2026</sub>

**Remote MCP server that exposes any GitHub repo's docs and code to AI tools.**

GitMCP is a remote MCP server that turns a GitHub repository or GitHub Pages site into documentation and code-search tools for assistants such as Cursor, Claude Desktop, Windsurf, VSCode and Cline. It reads llms.txt first, then AI-optimized docs, then README.md, and uses GitHub code search for source. Use the hosted URL (gitmcp.io/{owner}/{repo} or gitmcp.io/docs) or self-host it.

- **+** Hosted URL works with no install or signup; paste it into the MCP client config
- **+** Per-repo endpoints or one generic gitmcp.io/docs endpoint for switching repos
- **+** Prefers llms.txt, falling back to README.md, with search tools to limit token use
- **+** Self-hostable; README states it stores no queries or personal information
- **−** Only public GitHub repositories and Pages sites are supported
- **−** Falls back to README.md when a project has no llms.txt
- **−** Generic endpoint depends on the model picking the correct repository each call
- **−** No release tags; self-hosting steps cover only a local dev server

<sub>no GPU · Needs GitHub, Node.js, pnpm · port 5173 · [Repo](https://github.com/idosal/git-mcp) · [▶️ Demo ↗](https://gitmcp.io) · [🌐 Site ↗](https://gitmcp.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/git-mcp/)</sub>

<a name="pal-mcp-server"></a>
### #&#8288;73 [pal-mcp-server](https://github.com/beehiveinnovations/pal-mcp-server) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (75) · Freshness: slowing (32) · Maintenance: weak (4) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Dec 2025</sub>

**MCP server that lets Claude Code, Codex CLI and Cursor call multiple LLMs.**

PAL is a Python MCP server that exposes tools such as chat, thinkdeep, planner, consensus, codereview, precommit and debug to a host CLI or IDE, and routes each call to a chosen model from Gemini, OpenAI, Azure, X.AI, OpenRouter, DIAL or Ollama. It keeps conversation threads across tools and models, and its clink tool launches other CLIs (Gemini CLI, Codex, Claude Code) as subagents with role prompts.

- **+** Works with many hosts: Claude Code, Gemini CLI, Codex CLI, Qwen CLI, Cursor
- **+** Supports Gemini, OpenAI, Azure, X.AI, OpenRouter, DIAL and local Ollama models
- **+** Conversation threading carries context across models and after host context resets
- **+** clink spawns other CLIs as isolated subagents with roles like planner and codereviewer
- **−** Needs at least one provider API key or a local Ollama setup
- **−** Each enabled tool adds to the context window; six tools are disabled by default
- **−** License is reported as NOASSERTION, so terms need manual checking
- **−** Last commit was 2025-12-15, so recent model releases may lack support

<sub>GPU optional · Docker + Compose · Needs Python 3.10+, Git, uv, Provider API key (Gemini, OpenAI, OpenRouter, Azure, X.AI, DIAL) or Ollama · Models: Gemini, OpenAI, Anthropic, Grok, Azure OpenAI · safety checks passed 10 of 12 · [Repo](https://github.com/beehiveinnovations/pal-mcp-server) · [📖 Docs ↗](https://github.com/BeehiveInnovations/pal-mcp-server/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pal-mcp-server/)</sub>

<a name="markdownify-mcp"></a>
### #&#8288;74 [markdownify-mcp](https://github.com/zcaceres/markdownify-mcp) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: known (37) · Freshness: recent (78) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · May 2026</sub>

**MCP server that converts PDFs, Office files, audio and web pages to Markdown.**

Markdownify is a TypeScript MCP server that wraps Microsoft's markitdown to turn PDF, DOCX, XLSX, PPTX, images, audio, YouTube transcripts, Bing results and web pages into Markdown. Each format has its own tool, such as pdf-to-markdown or webpage-to-markdown. Setup uses bun, and a preinstall step creates a Python venv with markitdown[all].

- **+** One tool per format: PDF, DOCX, XLSX, PPTX, image, audio, YouTube, Bing, web page
- **+** MD_ALLOWED_PATHS restricts file-reading tools to listed directories
- **+** Paths to markitdown and repomix can be overridden by environment variable
- **+** Docker image available for the MCP catalog
- **−** Needs both Node/bun and a Python venv for markitdown
- **−** Published Docker image installs markitdown[pdf] only; audio and image tools fail there
- **−** File access is unrestricted unless MD_ALLOWED_PATHS is set
- **−** Desktop config requires a manual clone, build and absolute path to dist/index.js

<sub>no GPU · Docker · Needs bun, Python, markitdown, repomix · [Repo](https://github.com/zcaceres/markdownify-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/markdownify-mcp/)</sub>

<a name="mcpjungle"></a>
### #&#8288;75 [mcpjungle](https://github.com/mcpjungle/mcpjungle) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (25) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MPL-2.0 · Aug 2026</sub>

**Self-hosted MCP gateway that exposes many MCP servers through one endpoint.**

MCPJungle is a Go gateway that registers stdio and Streamable HTTP MCP servers once and serves their tools, prompts and resources at a single /mcp endpoint on port 8080. Clients such as Claude, Cursor and Copilot connect to that endpoint instead of each configuring every server. It adds tool groups, global tool enable/disable, a CLI and a dashboard UI, with SQLite by default and Postgres for shared deployments.

- **+** Single /mcp endpoint replaces per-client MCP configuration
- **+** Supports stdio and Streamable HTTP upstream servers, with env var placeholders in JSON configs
- **+** SQLite by default, Postgres supported for team deployments
- **+** Tool groups limit which tools a given client sees
- **−** Access control and OpenTelemetry are listed as enterprise-mode features
- **−** SSE upstream support is described as not mature
- **−** Stdio servers need the larger stdio image or a custom image
- **−** Default stateless connections respawn stdio servers on every tool call

<sub>no GPU · Docker + Compose · Needs Docker (optional), PostgreSQL (optional), SQLite · port 8080 · [Repo](https://github.com/mcpjungle/mcpjungle) · [📖 Docs ↗](https://docs.mcpjungle.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcpjungle/)</sub>

<a name="gemini-mcp-tool"></a>
### #&#8288;76 [gemini-mcp-tool](https://github.com/jamubc/gemini-mcp-tool) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (26) · Freshness: active (90) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · custom license · Jun 2026</sub>

**MCP server that lets Claude Code hand large-file analysis to Gemini or Antigravity CLI.**

A TypeScript MCP server that wraps the Gemini CLI and, from 2026-06-18, defaults to the Antigravity CLI (`agy`). It exposes `ask-gemini` and `sandbox-test` tools plus slash commands, so Claude can pass `@file` references to Gemini for large codebase analysis. Installed with `npx -y gemini-mcp-tool`.

- **+** One-line install: claude mcp add gemini-cli -- npx -y gemini-mcp-tool
- **+** Supports @ file and directory references for analyzing large codebases
- **+** Backend chosen with GEMINI_MCP_BACKEND (gemini or agy); timeout default 45 minutes
- **+** Provides AI-callable tools and user slash commands (/analyze, /sandbox)
- **−** Needs Gemini CLI or Antigravity CLI installed and signed in separately
- **−** agy backend is experimental: Gemini 3.5 Flash only in print mode, tools unsandboxed
- **−** Gemini CLI was retired for free, Pro and Ultra tiers on 2026-06-18
- **−** Unofficial tool; detected license is NOASSERTION while README states MIT

<sub>no GPU · Needs Node.js 16+, Gemini CLI or Antigravity CLI (agy) · Models: gemini-2.5-pro (default), Gemini 3.5 Flash (agy backend) · [Repo](https://github.com/jamubc/gemini-mcp-tool) · [📖 Docs ↗](https://jamubc.github.io/gemini-mcp-tool/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-mcp-tool/)</sub>

<a name="apple-docs-mcp"></a>
### #&#8288;77 [apple-docs-mcp](https://github.com/kimsungwhee/apple-docs-mcp) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: niche (8) · Freshness: slowing (48) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Mar 2026</sub>

**MCP server for searching Apple developer docs and WWDC transcripts.**

A TypeScript MCP server, run with npx over stdio, that gives coding assistants 15 tools for Apple's developer documentation. It covers doc search, framework symbol lookup, platform compatibility, sample code, and WWDC 2014-2025 sessions with transcripts. WWDC data is bundled in the npm package (about 35MB), while documentation queries go to Apple's public endpoints.

- **+** WWDC videos and transcripts are bundled in the package and work offline
- **+** 15 tools: symbol search, related APIs, platform compatibility, sample code
- **+** Install is one npx line; README gives configs for Claude, Cursor, VS Code, Zed and others
- **+** In-memory TTL cache per content type reduces repeat requests to Apple
- **−** Documentation queries depend on Apple's unofficial public endpoints and may break or be rate limited
- **−** Rotates browser User-Agent strings to improve reliability, which is fragile
- **−** Package is about 35MB because of bundled WWDC data
- **−** Last release 2025-09-15; the sample code tool has framework filtering limitations

<sub>no GPU · Needs Node.js, npx, Apple Developer Documentation public endpoints · [Repo](https://github.com/kimsungwhee/apple-docs-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apple-docs-mcp/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
