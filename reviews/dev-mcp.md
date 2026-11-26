# 🔌 MCP servers for developers reviews · Best of Vibe Coding

MCP servers that give coding agents tools: docs lookup, browsers, GitHub, databases and code navigation. Back to the [leaderboard](../README.md#-mcp-servers-for-developers).

<sub>🌐 Also on the web: [MCP servers for developers on archestack.com](https://archestack.com/best-of-vibe-coding/dev-mcp/), each project on its own page.</sub>

<a name="gitnexus"></a>
### 🥇 [gitnexus](https://github.com/abhigyanpatwari/gitnexus) <sub>score [97](../README.md#-how-we-rank "Score 97/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 49k · custom license · Nov 2026</sub>

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

<a name="codegraph"></a>
### 🥈 [codegraph](https://github.com/colbymchenry/codegraph) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 79k · MIT · Nov 2026</sub>

**Local code knowledge graph exposed to coding agents over MCP.**

CodeGraph indexes a repository into a local graph of symbols, call edges and dependencies stored in a .codegraph/ directory, then serves it to coding agents through an MCP server. Agents query the graph for relevant source, call paths and change blast radius instead of grepping and reading files. One installer wires it into Claude Code, Cursor, Codex, opencode, Gemini CLI, Copilot and others, and the index auto-syncs on file changes.

- **+** codegraph install auto-configures about 18 agents, including Claude Code, Cursor, Codex and Copilot
- **+** Indexes dozens of languages into one graph with cross-file resolution
- **+** Watches files and updates the index automatically, so no manual re-indexing
- **+** Self-contained install with bundled runtime; Node.js is not required
- **−** Responses stay resident in context: about 80% more retrieval context at session end, per its own numbers
- **−** Benchmarks are the author's own: seven repos, one question each
- **−** Index is per project and must be rebuilt with codegraph index after some upgrades
- **−** Hosted PR-analysis platform is only a waitlist; the open-source part is the local tool

<sub>no GPU · Models: Claude Code, Cursor, Codex CLI, opencode, Gemini CLI · safety checks passed 14 of 16 · [Repo](https://github.com/colbymchenry/codegraph) · [📖 Docs ↗](https://colbymchenry.github.io/codegraph/) · [🌐 Site ↗](https://colbymchenry.github.io/codegraph/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegraph/)</sub>

<a name="playwright-mcp"></a>
### 🥉 [playwright-mcp](https://github.com/microsoft/playwright-mcp) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · Apache-2.0 · Nov 2026</sub>

**MCP server that lets LLMs drive a browser through Playwright accessibility snapshots.**

Runs as an MCP server, started with `npx @playwright/mcp@latest`, and exposes Playwright browser control to any MCP client. It feeds the model structured accessibility-tree snapshots instead of screenshots, so no vision model is required. Options cover Chrome, Firefox, WebKit and Edge, CDP or extension attachment to a running browser, proxies, device emulation and origin allow/block lists.

- **+** Uses accessibility snapshots, so text-only models can operate pages without vision
- **+** Works with many MCP clients: VS Code, Cursor, Claude Code, Codex, Gemini CLI, Goose and others
- **+** Can attach to a running Chrome or Edge via CDP endpoint or the Playwright Extension
- **+** Many flags: isolated profiles, secrets file, URL param redaction, init scripts, proxy, device emulation
- **−** README says tool schemas and verbose snapshots cost more tokens than the Playwright CLI with skills
- **−** README recommends the separate Playwright CLI for high-throughput coding agents
- **−** Origin allow/block lists are documented as not a security boundary
- **−** Headed browser by default, so servers need --headless

<sub>no GPU · Docker · Needs Node.js 18 or newer, Playwright browsers (Chrome, Firefox, WebKit or Edge), MCP client · Models: Any LLM via an MCP client · [Repo](https://github.com/microsoft/playwright-mcp) · [🌐 Site ↗](https://playwright.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/playwright-mcp/)</sub>

<a name="fastmcp"></a>
### #&#8288;4 [fastmcp](https://github.com/prefecthq/fastmcp) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Nov 2026</sub>

**Python framework for building MCP servers, clients and interactive apps.**

FastMCP is a Python framework for the Model Context Protocol. Decorating a plain Python function with `@mcp.tool` generates the schema, validation and docs, and the same package includes a client that handles transport negotiation, authentication and protocol lifecycle. It also supports Apps, which render interactive UIs inside the conversation. A separate TypeScript port exists in another repo.

- **+** Tool schemas and validation are generated from Python function signatures and docstrings
- **+** One package covers servers, clients and interactive Apps
- **+** Documentation is also published as llms.txt and llms-full.txt for coding agents
- **+** Upgrade guides cover FastMCP 2 and 3 and MCP SDK v1 and v2
- **−** Python only here; TypeScript needs the separate fastmcp-ts package
- **−** Enterprise features (SSO, tool-level RBAC, audit logs) are in the separate FastMCP Gateway product
- **−** Several major-version upgrade guides suggest migration work between releases
- **−** It is a framework, not a runnable app, so you write your own server code

<sub>[Repo](https://github.com/prefecthq/fastmcp) · [📖 Docs ↗](https://gofastmcp.com) · [🌐 Site ↗](https://gofastmcp.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastmcp/)</sub>

<a name="cua"></a>
### #&#8288;5 [cua](https://github.com/trycua/cua) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**Desktop automation tools and VM sandboxes for computer-use agents.**

Monorepo for running agents on full desktops. It holds Cua Driver (CLI, MCP and SDKs to operate native apps on macOS, Windows and Linux), Lume (macOS and Linux VMs on Apple Silicon), the `cua` SDK and CLI for sandboxes, the Cua Spaces app, CUA-S1 research models and Cua Bench. You bring your own agent and model.

- **+** Cua Driver covers macOS, Windows and Linux via CLI, MCP and typed SDKs
- **+** SDK has the same API in Python, TypeScript and Rust
- **+** Cua Bench runs a first simulated task with no VM, Docker or model API key
- **+** Lume creates local macOS and Linux VMs through Apple's Virtualization.Framework
- **−** Cua Spaces and Cua Driver Bench are FSL-1.1-MIT, not MIT
- **−** Spaces app install needs macOS 26 or later; Lume needs Apple Silicon
- **−** Many deprecated packages remain listed, including cuabot with known security issues
- **−** Swift and Kotlin SDK bindings are not yet released

<sub>Needs Apple Silicon (Lume), macOS 26 or later (Spaces app), Python 3.12 or 3.13 and uv (Cua Bench) · Models: Bring your own agent and model, CUA-S1-FORMS (Hugging Face) · [Repo](https://github.com/trycua/cua) · [📖 Docs ↗](https://cua.ai/docs) · [🌐 Site ↗](https://cua.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cua/)</sub>

<a name="code-review-graph"></a>
### #&#8288;6 [code-review-graph](https://github.com/tirth8205/code-review-graph) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**Local Tree-sitter code graph that gives coding assistants review context over MCP.**

Parses a repository with Tree-sitter into a SQLite graph of functions, classes, imports, calls and tests, then serves blast-radius and risk-scored context over MCP so the assistant reads only affected files. The installer configures about 16 tools (Claude Code, Cursor, Codex, Windsurf, Zed and others) and updates incrementally via hooks, git hooks or watch mode. A GitHub Action posts risk-scored PR comments.

- **+** One install command detects and configures about 16 AI coding tools, with a clean uninstall
- **+** Incremental updates re-parse only SHA-256-changed files; two-file edit on django took about 2.5 s
- **+** Covers 30+ languages plus notebooks, and custom grammars via languages.toml
- **+** Runs locally; the GitHub Action builds the graph on the CI runner without sending code out
- **−** Impact recall of 1.0 is circular, since ground truth comes from the same graph
- **−** Against a grep baseline, median token reduction is 6.65x, not the 63x headline
- **−** Graph context can cost more tokens than a plain read for small single-file edits
- **−** Cold build of a roughly 3,000-file repository took about 40 seconds

<sub>no GPU · Docker · Needs Python 3.10+, Tree-sitter, SQLite · Models: all-MiniLM-L6-v2 (local embeddings) · safety checks passed 16 of 18 · [Repo](https://github.com/tirth8205/code-review-graph) · [📖 Docs ↗](https://github.com/tirth8205/code-review-graph/blob/main/docs/USAGE.md) · [🌐 Site ↗](https://code-review-graph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-review-graph/)</sub>

<a name="serena"></a>
### #&#8288;7 [serena](https://github.com/oraios/serena) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · custom license · Nov 2026</sub>

**MCP server giving coding agents symbol-level code search, editing and refactoring.**

Serena is an MCP server that exposes IDE-style tools to a coding agent: find symbol, find referencing symbols, symbol overview, rename, and replace or insert at symbol level. It uses language servers (LSP) for over 40 languages by default, or a paid JetBrains plugin that adds move, inline, type hierarchy and a debugger. It plugs into MCP clients such as Claude Code, Codex, Gemini-CLI, VSCode and Claude Desktop, and includes a per-project memory system.

- **+** Symbol-level retrieval and editing instead of line numbers or text search
- **+** Language server backend covers over 40 languages and is free
- **+** Works with any MCP client; stdio launch command or HTTP mode
- **+** Layered YAML config: global, per-project, per-client context, and modes
- **−** Move, inline, type hierarchy and debugging need the paid JetBrains plugin
- **−** Language server backend only renames symbols; no move or inline
- **−** Some languages need extra language server dependencies installed manually
- **−** Mixed licensing: GPL-3.0-or-later app with MIT SolidLSP component, plus a CLA

<sub>Docker + Compose · Needs uv, Python 3.13, language servers per language (LSP backend), JetBrains IDE and Serena plugin (optional, paid) · Models: Any LLM through an MCP client · safety checks passed 12 of 14 · [Repo](https://github.com/oraios/serena) · [📖 Docs ↗](https://oraios.github.io/serena/02-usage/000_intro.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serena/)</sub>

<a name="n8n-mcp"></a>
### #&#8288;8 [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

**MCP server that lets AI assistants build, edit, validate and debug n8n workflows.**

n8n-MCP exposes n8n's Public API to MCP clients such as Claude, ChatGPT and Cursor. Tools cover reading failed executions, partial workflow edits with snapshots and rollback, validation and autofix, test runs, and credential management. It bundles a database of 3,501 nodes and 2,352 templates, so node docs and validation work without an n8n connection.

- **+** Partial workflow edits avoid resending whole workflows; up to 10 snapshots per workflow allow rollback
- **+** Bundled database of 3,501 nodes and 2,352 templates; docs and validation work without n8n
- **+** Can route Public API gaps to n8n's built-in MCP server through one connection
- **+** Self-host via npx, Docker or Railway, or use the hosted multi-instance service
- **−** Read-modify-write without conditional writes: UI edits made mid-session get overwritten
- **−** A failed snapshot does not block the edit, so rollback is not guaranteed
- **−** Hosted free tier is capped at 100 tool calls per day
- **−** Pinned-data tests and Agents need a separate N8N_MCP_ACCESS_TOKEN and recent n8n

<sub>no GPU · Docker + Compose · Needs n8n instance with Public API enabled, n8n API key · [Repo](https://github.com/czlonkowski/n8n-mcp) · [▶️ Demo ↗](https://dashboard.n8n-mcp.com) · [📖 Docs ↗](https://www.n8n-mcp.com/docs/multi-instance) · [🌐 Site ↗](https://www.n8n-mcp.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/n8n-mcp/)</sub>

<a name="inspector"></a>
### #&#8288;9 [modelcontextprotocol/inspector](https://github.com/modelcontextprotocol/inspector) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Nov 2026</sub>

**Inspector for testing and debugging MCP servers via web, CLI or terminal UI.**

MCP Inspector is a developer tool for connecting to Model Context Protocol servers and exercising them. One npm package provides a Vite/React web app with a Node backend, a scriptable CLI for CI smoke tests, an Ink-based TUI, and an experimental `mcpdo` connection CLI. OAuth tokens and stdio env values go to the OS keychain when one is available.

- **+** Four interfaces in one package: web, CLI, TUI and experimental mcpdo
- **+** CLI supports JSON output and exit codes for shell or CI smoke tests
- **+** Stores OAuth tokens and stdio env values in the OS keychain by default
- **+** Runs with a single npx command, no install step
- **−** Without a keychain, secrets fall back to unencrypted ~/.mcp-inspector/secrets.json
- **−** v2 requires a recent patched Node (^22.23.4, ^24.22.1 or >=26.12.1)
- **−** External contributions accepted as issues only, not pull requests
- **−** Mixed licensing mid-transition from MIT to Apache-2.0; license detected as NOASSERTION

<sub>no GPU · Docker · Needs Node.js ^22.23.4 || ^24.22.1 || >=26.12.1 · [Repo](https://github.com/modelcontextprotocol/inspector) · [🌐 Site ↗](https://modelcontextprotocol.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/inspector/)</sub>

<a name="chrome-devtools-mcp"></a>
### #&#8288;10 [chrome-devtools-mcp](https://github.com/chromedevtools/chrome-devtools-mcp) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · Apache-2.0 · Nov 2026</sub>

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

<a name="open-seo"></a>
### #&#8288;11 [open-seo](https://github.com/every-app/open-seo) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Nov 2026</sub>

**SEO toolkit for keyword research, rank tracking and audits, with an MCP server.**

OpenSEO is a self-hostable alternative to Semrush and Ahrefs covering keyword research, rank tracking, competitor insights, backlinks, site audits and AI visibility. SEO data comes from your own DataForSEO API key, billed pay-as-you-go. It exposes an MCP server and agent skills so Claude Code, ChatGPT, Codex and similar clients can query the data directly.

- **+** Pay-as-you-go via your own DataForSEO key, no subscription when self-hosting
- **+** Ships an MCP server plus prebuilt agent skills for Claude Code, Codex and ChatGPT
- **+** Two self-host paths: Docker Compose or one-command Cloudflare deploy on the free plan
- **+** Email/password accounts with admin bootstrap and invitation links for teammates
- **−** Requires a paid DataForSEO account; no SEO data without it
- **−** Hosted version adds 28% on DataForSEO requests and costs $10/month
- **−** Narrower workflow set than full Semrush or Ahrefs suites
- **−** Running without sign-in needs your own network controls such as Tailscale

<sub>no GPU · Docker + Compose · Needs DataForSEO API key, Docker Compose or Cloudflare account · [Repo](https://github.com/every-app/open-seo) · [📖 Docs ↗](https://openseo.so/docs/mcp) · [🌐 Site ↗](https://openseo.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-seo/)</sub>

<a name="context7"></a>
### #&#8288;12 [context7](https://github.com/upstash/context7) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · MIT · Nov 2026</sub>

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

<a name="cli-cli"></a>
### #&#8288;13 [cli/cli](https://github.com/cli/cli) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · MIT · Nov 2026</sub>

**Official GitHub command-line client for pull requests, issues and repos.**

gh is GitHub's official CLI, written in Go. It runs pull request, issue and other GitHub operations from the terminal, alongside git, on macOS, Windows and Linux. It works with GitHub.com, GitHub Enterprise Cloud and supported Enterprise Server versions, and ships an agent skill that coding agents can use to drive it.

- **+** Official GitHub project; packages for Homebrew, WinGet, apt, rpm and precompiled binaries
- **+** Releases carry Sigstore build provenance attestations, verifiable with gh or cosign
- **+** Preinstalled on GitHub-hosted Actions runners and available as a devcontainer feature
- **+** Installs an agent skill via `gh skill install cli/cli gh` for coding agents
- **−** Only talks to GitHub; no GitLab, Bitbucket or other forges
- **−** Not an AI project or starter; it fits this list only as a tool for agents
- **−** Not an MCP server; agents must shell out to the gh binary
- **−** Needs GitHub authentication to do anything useful

<sub>no GPU · Needs GitHub.com, GitHub Enterprise Cloud or Enterprise Server, git · [Repo](https://github.com/cli/cli) · [📖 Docs ↗](https://cli.github.com/manual/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-cli/)</sub>

<a name="mcp-toolbox"></a>
### #&#8288;14 [mcp-toolbox](https://github.com/googleapis/mcp-toolbox) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

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

<a name="python-sdk"></a>
### #&#8288;15 [python-sdk](https://github.com/modelcontextprotocol/python-sdk) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Nov 2026</sub>

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

<a name="unity-mcp"></a>
### #&#8288;16 [coplaydev/unity-mcp](https://github.com/coplaydev/unity-mcp) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

**MCP server that lets AI clients control the Unity Editor.**

Unity package plus a Python MCP server that connects MCP clients (Claude Desktop and Code, Cursor, VS Code, Windsurf, Cline, Gemini CLI) to the Unity Editor. It exposes 50 tool entrypoints for creating scenes and GameObjects, editing C# scripts, managing assets, running tests, profiling and building.

- **+** 50 MCP tool entrypoints covering scenes, scripts, assets, tests, profiling and builds
- **+** Works with any MCP client; one-step client configuration from a Unity menu
- **+** Supports Unity 2021.3 LTS through 6.x; install via git URL or OpenUPM
- **+** Optional Roslyn script validation, multi-instance routing and remote server auth
- **−** Tied to the Unity Editor; no use outside Unity projects
- **−** Requires Python 3.10+ via uv alongside the Unity package
- **−** Sponsored by Aura, which also sells a separate premium assistant
- **−** Contributions go to the beta branch while install URL points at main

<sub>no GPU · Compose · Needs Unity 2021.3 LTS to 6.x, Python 3.10+, uv · Models: Any MCP client, Claude, Codex, local LLMs · safety checks passed 17 of 18 · [Repo](https://github.com/coplaydev/unity-mcp) · [🌐 Site ↗](https://coplaydev.github.io/unity-mcp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unity-mcp/)</sub>

<a name="fff"></a>
### #&#8288;17 [fff](https://github.com/dmtrkovalenko/fff) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**Fast typo-tolerant file and content search for MCP clients, Pi and Neovim.**

fff is a Rust file search library with a resident in-memory index, frecency ranking, git-status annotations and a background watcher. It ships as an MCP server (tools grep, find_files, multi_grep) for Claude Code, Codex, OpenCode, Cursor and Cline, as a Pi agent extension, and as the fff.nvim picker. Search is typo-tolerant, with fuzzy fallback on zero matches and a definitions-only mode.

- **+** Index stays resident across tool calls, so repeated searches avoid re-scanning the repo
- **+** Frecency ranking and git status tags surface files you are actively editing
- **+** Definitions-only search with staged fallback from exact to fuzzy matches, with notices
- **+** Prebuilt binaries via install script or Homebrew; same core serves MCP, Pi and Neovim
- **−** Benchmarks in the README show mixed results: one held-out model was slower and used more tokens
- **−** Install is a curl-piped shell script or Homebrew; no container image
- **−** Agents need a prompt hint in CLAUDE.md to prefer fff over built-in search
- **−** Index is scoped to a git-indexed directory; globs cannot override ignore rules

<sub>no GPU · Needs Rust (fallback cargo build for Neovim plugin), git · [Repo](https://github.com/dmtrkovalenko/fff) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fff/)</sub>

<a name="tabularis"></a>
### #&#8288;18 [tabularis](https://github.com/tabularisdb/tabularis) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · Apache-2.0 · Nov 2026</sub>

**Desktop SQL client with notebooks, plugin drivers and a built-in MCP server.**

Tabularis is a desktop SQL workspace with built-in PostgreSQL, MySQL/MariaDB and SQLite drivers. It adds 29 shipped driver plugins (DuckDB, ClickHouse, MongoDB and others) that speak JSON-RPC over stdio. A built-in MCP server lets agents such as Claude and Cursor read schemas and run queries. It also includes SQL notebooks, a visual query builder, visual EXPLAIN and optional AI text-to-SQL.

- **+** Built-in MCP server exposes schema and query access to coding agents
- **+** Drivers are plugins over JSON-RPC/stdio, so they can be written in any language
- **+** SQL notebooks mix SQL and Markdown cells, with cross-cell variables and charts
- **+** Text-to-SQL can use local models through Ollama
- **−** Only 3 drivers built in; every other database needs a plugin
- **−** Built-in PostgreSQL driver is deprecated in favour of a separate plugin
- **−** Several plugins are third-party repos, hosted outside the main org
- **−** Snap needs a manual password-manager-service connect to save credentials

<sub>Docker + Compose · Needs Ollama (optional, for local text-to-SQL) · Models: Ollama · [Repo](https://github.com/tabularisdb/tabularis) · [📖 Docs ↗](https://tabularis.dev/wiki) · [🌐 Site ↗](https://tabularis.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tabularis/)</sub>

<a name="ghidra-mcp"></a>
### #&#8288;19 [ghidra-mcp](https://github.com/bethington/ghidra-mcp) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Nov 2026</sub>

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

<a name="dbx"></a>
### #&#8288;20 [dbx](https://github.com/t8y2/dbx) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Nov 2026</sub>

**Rust database client for 100+ databases with an AI assistant and MCP server.**

DBX is a database manager written in Rust that connects to MySQL, PostgreSQL, SQLite, Redis, MongoDB, ClickHouse, Oracle, SQL Server, Elasticsearch and many others, including Chinese vendor databases and generic JDBC. It ships as a desktop app, a Docker image and a CLI, and includes a built-in AI assistant and an MCP server. The README advertises a 25 MB footprint.

- **+** Covers SQL, document, key-value, search and time-series stores, plus JDBC, in one client
- **+** README claims a 25 MB install size
- **+** Desktop app, CLI and MCP server share one tool
- **+** Actively maintained: commit and release both dated 2026-10-29
- **−** Primarily a GUI database client; the MCP server is one feature, not the core
- **−** Detected repo has no Docker or compose files despite the Docker claim
- **−** Support depth varies across 100+ databases, since many rely on generic JDBC

<sub>no GPU · Docker + Compose · [Repo](https://github.com/t8y2/dbx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dbx/)</sub>

<a name="opencli"></a>
### #&#8288;21 [opencli](https://github.com/jackwener/opencli) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · Apache-2.0 · Nov 2026</sub>

**Browser automation CLI for agents, using your logged-in Chrome.**

OpenCLI controls a logged-in Chrome or Chromium through a Browser Bridge extension and a local daemon. It has generic browser commands (open, state, click, fill, extract, network, screenshot) and 100+ site adapters such as Bilibili, Reddit, Twitter/X and HackerNews. Output is JSON by default, and bundled skills let agents like Claude Code or Cursor drive it.

- **+** Reuses your logged-in Chrome session, so no per-site credential handling
- **+** JSON envelope with error codes and sysexits-style exit codes suits scripts and agents
- **+** Bundled skills help agents write, test and repair site adapters
- **+** Plugin system installs third-party adapters from GitHub or local paths
- **−** Needs a Chrome extension and local daemon; remote browsers need a CDP endpoint
- **−** Adapters depend on site internals and can break when sites change
- **−** Adapter list leans toward Chinese platforms; many commands act on real accounts
- **−** Video downloads need yt-dlp installed separately

<sub>no GPU · Needs Node.js >= 20.18.1, Chrome or Chromium, OpenCLI Browser Bridge extension, yt-dlp (video downloads) · [Repo](https://github.com/jackwener/opencli) · [🌐 Site ↗](https://opencli.info/download) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencli/)</sub>

<a name="omniget"></a>
### #&#8288;22 [omniget](https://github.com/tonhowtf/omniget) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · GPL-3.0 · Nov 2026</sub>

**Desktop video downloader on yt-dlp with a built-in MCP server and agent window.**

OmniGet is a Rust desktop app for Windows, macOS and Linux that downloads video, audio, galleries, torrents and direct files from its own extractors and yt-dlp. Its MCP server, bound to 127.0.0.1 with per-client tokens, lets Claude Code, Cursor, VS Code, Codex and Goose queue and monitor downloads. It also hosts Claude Code, Codex, Gemini CLI and local models as agents with permission prompts and undo.

- **+** MCP server with per-client tokens and permissions, listening only on 127.0.0.1
- **+** Installs and updates yt-dlp and FFmpeg itself; yt-dlp checked by SHA-256
- **+** Resumable queue with backoff retries, and each download keeps its exact yt-dlp command
- **+** Ships omniget-cli, a Chrome/Firefox extension and a Claude Code plugin that works without the app
- **−** Scope is wide: downloader, agent client and MCP server in one app
- **−** Agent shell sandbox is described only for macOS (seatbelt)
- **−** Firefox extension is a temporary add-on and must be reloaded after each restart
- **−** Desktop GUI only; no Docker image or headless server mode

<sub>Needs yt-dlp, FFmpeg, gallery-dl · Models: Claude Code, Codex, Gemini CLI, Ollama, LM Studio · [Repo](https://github.com/tonhowtf/omniget) · [🌐 Site ↗](https://getomniget.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omniget/)</sub>

<a name="jarvis-registry"></a>
### #&#8288;23 [jarvis-registry](https://github.com/ascending-llc/jarvis-registry) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Nov 2026</sub>

**MCP and A2A gateway with OAuth, access control and a private skill registry.**

Jarvis Registry is a reverse proxy that puts MCP servers (SSE or Streamable HTTP) and A2A agents behind one authenticated endpoint. It uses OAuth 2.0/OIDC with Keycloak, Amazon Cognito or Microsoft Entra ID, applies role scopes and resource ACLs, and logs requests with OpenTelemetry and Prometheus. It also includes semantic discovery of servers and agents, and a skill registry that syncs SKILL.md packages to coding clients through a CLI.

- **+** Supports Keycloak, Cognito and Entra ID for auth without custom code
- **+** Request logging, OpenTelemetry tracing and Prometheus metrics are built in
- **+** Per-skill permissions for users and groups, synced to Claude Code, Codex, Cursor and Copilot
- **+** Deployment guides for EKS, AKS and GKE plus a Docker Compose local stack
- **−** Needs an external identity provider configured before first use
- **−** Removing registry access does not erase skill copies already downloaded
- **−** Production setup targets Kubernetes clusters, which is heavy for small teams
- **−** Skill delivery is separate from MCP tool authorization, so two access models to manage

<sub>Docker + Compose · Needs Keycloak, Amazon Cognito or Microsoft Entra ID, Docker Compose, uv · port 80 · [Repo](https://github.com/ascending-llc/jarvis-registry) · [▶️ Demo ↗](https://youtu.be/EUqWc_mAaXs) · [📖 Docs ↗](https://jarvisregistry.com/) · [🌐 Site ↗](https://ascendingdc.com/jarvis-ai/jarvis-registry/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jarvis-registry/)</sub>

<a name="typescript-sdk"></a>
### #&#8288;24 [typescript-sdk](https://github.com/modelcontextprotocol/typescript-sdk) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · custom license · Nov 2026</sub>

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
### #&#8288;25 [codebase-memory-mcp](https://github.com/deusdata/codebase-memory-mcp) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 49k · MIT · Nov 2026</sub>

**MCP server that indexes a repo into a local code knowledge graph.**

A native C MCP server that parses source, docs and infrastructure config into a persistent local graph, exposed through 17 MCP tools and a CLI. An installer registers it with 46 agent client integrations, adding skills, profiles and hooks. An optional beta browser UI, CBM Lens (v0.0.1), shows architecture maps, a 3D graph and source.

- **+** Native C binary; no Docker or language runtime, indexing needs no API key
- **+** 17 MCP tools over a persistent graph: callers, dependencies, search, change impact
- **+** Parses 163 languages plus Docker, Kubernetes, Terraform and CI config
- **+** Installer configures 46 client integrations; hooks can be disabled with --no-hooks
- **−** CBM Lens UI is open beta, v0.0.1
- **−** Smart CI test impact is experimental and limited to supported C/C++ harnesses
- **−** All active CBM processes must run the identical build and cache root
- **−** Install is a curl-to-bash script; Defender may flag binaries as a false positive

<sub>no GPU · port 9749 · safety checks passed 13 of 16 · [Repo](https://github.com/deusdata/codebase-memory-mcp) · [📖 Docs ↗](https://github.com/DeusData/codebase-memory-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codebase-memory-mcp/)</sub>

<a name="lingo-dev"></a>
### #&#8288;26 [lingo.dev](https://github.com/lingodotdev/lingo.dev) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · Apache-2.0 · Nov 2026</sub>

**Hosted translation engines with a CLI, API and GitHub App for app localization.**

Lingo.dev is a localization platform where you configure translation engines (model routing, brand voice, rules, glossaries, AI reviewers) and call them from a CLI, HTTP API, MCP server or GitHub App. The CLI pushes source files such as JSON, YAML, Markdown, PO and XLIFF (18 formats) and pulls translations back, locally or in CI. Engines are configured and run on the Lingo.dev platform.

- **+** CLI supports 18 file formats including XLIFF, PO, Flutter ARB, Android and Xcode strings
- **+** GitHub App opens translation PRs without a CI runner or API key secret
- **+** Glossaries, rules and brand voices are shared across engines by attachment
- **+** API responses report the model used and token cost per request
- **−** Engines are configured and run on the hosted platform, not self-hosted
- **−** Requires a Lingo.dev account and API key to translate anything
- **−** CLI and CI usage need Node.js 22 or newer
- **−** Translation quality and cost depend on the chosen LLM per language pair

<sub>no GPU · Docker · Needs Lingo.dev platform account and API key, Node.js 22+ · Models: 400+ LLMs via the platform (e.g. anthropic/claude-sonnet-4.5) · [Repo](https://github.com/lingodotdev/lingo.dev) · [📖 Docs ↗](https://lingo.dev/en/docs) · [🌐 Site ↗](https://lingo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lingo-dev/)</sub>

<a name="terminal-browser"></a>
### #&#8288;27 [terminal-browser](https://github.com/zenbu-labs/terminal-browser) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Nov 2026</sub>

**Chromium browser that renders inside kitty-graphics terminals, scriptable by coding agents.**

terminal-browser runs Chromium via Electron offscreen rendering and draws the pixels in the terminal using the kitty graphics protocol, sending only changed regions. Mouse and keyboard input from the terminal is converted to synthetic Chromium events. It includes an agent-browser compatible `action` CLI, a Claude Code plugin, split-pane integration with several terminals, and an `--ssh` mode that proxies network requests through a remote host.

- **+** Agents can drive open browsers through an agent-browser compatible `action` CLI
- **+** `--ssh` runs the page locally and proxies requests, so remote localhost sites load quickly
- **+** Built-in split-pane support for ghostty, kitty, iTerm2, wezterm, tmux, vscode and others
- **+** Sends only changed regions of the page to the terminal
- **−** Requires a terminal with kitty graphics protocol support
- **−** Windows works only under WSL, with very few compatible terminals
- **−** Collects usage telemetry and crash reports by default; opt-out required
- **−** Chrome extensions and design mode are still on the roadmap

<sub>Needs Electron/Chromium, Terminal with kitty graphics protocol, WSL (Windows only) · [Repo](https://github.com/zenbu-labs/terminal-browser) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terminal-browser/)</sub>

<a name="socraticode"></a>
### #&#8288;28 [socraticode](https://github.com/giancarloerra/socraticode) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · AGPL-3.0 · Nov 2026</sub>

**MCP server that indexes a codebase for hybrid semantic and BM25 search.**

SocratiCode is a local stdio MCP server, also packaged as plugins for Claude Code, Codex and VS Code, that indexes a repository into Qdrant using AST-aware chunking and RRF-fused semantic plus BM25 search. It also builds dependency graphs, symbol-level impact and call-flow analysis across 18 languages, and searchable artifacts such as database schemas and API specs. A file watcher keeps the index current, and embeddings run on local Ollama by default.

- **+** Hybrid semantic and BM25 search with AST-aware chunking over a Qdrant index
- **+** Impact analysis and call-flow tracing across 18 languages, plus dependency graph explorer
- **+** Resumable batched indexing and a file watcher; README cites repos up to about 40M lines
- **+** Local embeddings by default, with OpenAI or Google Gemini and external Qdrant as options
- **−** AGPL-3.0 license may constrain embedding in proprietary products
- **−** Default setup needs Docker running for managed Qdrant and Ollama
- **−** Docker containers cannot use the GPU on macOS or Windows; native Ollama is needed for speed
- **−** Hosted team index, SSO and audit logs are only in the separate Cloud beta

<sub>GPU optional · Compose · Needs Node.js 18.17+, Docker, Qdrant, Ollama · Models: Ollama (local embeddings), OpenAI embeddings, Google Gemini embeddings · [Repo](https://github.com/giancarloerra/socraticode) · [📖 Docs ↗](https://github.com/giancarloerra/socraticode/blob/main/docs/guides/README.md) · [🌐 Site ↗](https://socraticode.cloud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/socraticode/)</sub>

<a name="jcodemunch-mcp"></a>
### #&#8288;29 [jcodemunch-mcp](https://github.com/jgravelle/jcodemunch-mcp) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · custom license · Nov 2026</sub>

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

<a name="github-mcp-server"></a>
### #&#8288;30 [github-mcp-server](https://github.com/github/github-mcp-server) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Nov 2026</sub>

**GitHub's MCP server exposing repos, issues, PRs and Actions to AI agents.**

Official GitHub MCP server, written in Go, that lets MCP hosts read code, manage issues and pull requests, inspect Actions runs, and view security findings and Dependabot alerts. It runs either as a GitHub-hosted remote endpoint (api.githubcopilot.com/mcp/) or locally over stdio from a Docker image or a built binary. Authentication is OAuth or a personal access token.

- **+** Maintained by GitHub, with a hosted remote endpoint that needs no local install
- **+** Covers repos, issues, PRs, Actions, Dependabot, discussions and notifications
- **+** Supports OAuth or PAT, plus GitHub Enterprise Server and ghe.com via GITHUB_HOST
- **+** Toolsets can be configured to limit which tools the agent sees
- **−** GitHub Enterprise Server cannot use the hosted remote server; local only
- **−** Remote OAuth depends on each MCP host registering its own GitHub or OAuth app
- **−** Local Docker OAuth needs a fixed callback port (8085) published to loopback
- **−** Only works with GitHub; no support for other forges

<sub>no GPU · Docker · Needs GitHub account, Docker (for local container), GitHub personal access token or OAuth · port 8085 · safety checks passed 14 of 15 · [Repo](https://github.com/github/github-mcp-server) · [📖 Docs ↗](https://github.com/github/github-mcp-server/blob/main/docs/remote-server.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github-mcp-server/)</sub>

<a name="vapi-network"></a>
### #&#8288;31 [vapi-network](https://github.com/vapi-network/vapi-network) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · Apache-2.0 · Nov 2026</sub>

**Non-custodial CLI and MCP client for paying x402 APIs in USDC on Base.**

TypeScript client that discovers x402 API listings, applies local spend policy, signs USDC payments on Base from an encrypted device vault, and writes a local receipt per call. It exposes the same wallet through a CLI, an MCP server with namespaced tools (call.*, router.*, wallet.*, swarm.*), and an SDK. It also launches Claude Code and Codex against a model Router, and runs capped local agents and swarms.

- **+** Keys stay in a local encrypted vault; spend policy is applied before signing
- **+** Payments go directly to the service, with a local receipt per paid call
- **+** One wallet is reachable from CLI, MCP server and SDK
- **+** Launchers for Claude Code and Codex fall back to your own login below $0.50 Compute
- **−** Tasks (escrow) is preview only and not live on production
- **−** Solana listings are searchable but cannot be inspected or paid yet
- **−** Headless Linux needs VAPI_VAULT_PASSWORD when no OS keyring exists
- **−** Router and some features depend on hosted vAPI services, not fully self-contained

<sub>no GPU · Needs Node.js and npm, Base network (USDC), vAPI hosted services (Router, catalogue) · Models: Claude (via vAPI Router, Venice), OpenAI GPT (Codex, via Router) · [Repo](https://github.com/vapi-network/vapi-network) · [📖 Docs ↗](https://docs.vapinetwork.ai) · [🌐 Site ↗](https://vapinetwork.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vapi-network/)</sub>

<a name="agent-device"></a>
### #&#8288;32 [agent-device](https://github.com/callstack/agent-device) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Nov 2026</sub>

**CLI and MCP server that lets coding agents drive mobile, TV, web and desktop apps.**

agent-device lets coding agents open apps on iOS, Android, HarmonyOS, tvOS, Android TV, Fire OS, web, macOS and Linux, read accessibility-tree snapshots, and act through refs and selectors. It runs as a CLI, a stdio MCP server (`agent-device mcp`), or a typed Node.js client. Sessions are scoped per git worktree, runs can be saved as `.ad` replay scripts or exported as Maestro YAML, and remote device clouds are supported.

- **+** Same runtime exposed as CLI, stdio MCP server and typed Node.js API
- **+** Token-efficient accessibility snapshots instead of screenshot-only reasoning
- **+** Worktree-scoped sessions and device claims keep parallel agents off each other's simulators
- **+** Saves runs as .ad replay scripts for CI; exports strict Maestro YAML
- **−** Command support varies by target; HarmonyOS and Vega OS cover only a subset
- **−** Snapshot reliability depends on the app's accessibility labels, roles and test IDs
- **−** Requires Node.js 22.12+; web automation needs Node.js 24+
- **−** Web support is basic and delegates to agent-browser

<sub>no GPU · Needs Node.js 22.12+, XCTest (iOS), ADB (Android), HDC (HarmonyOS), AT-SPI (Linux), agent-browser (web) · [Repo](https://github.com/callstack/agent-device) · [📖 Docs ↗](https://agent-device.dev/docs/quick-start) · [🌐 Site ↗](https://agent-device.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-device/)</sub>

<a name="dembrandt"></a>
### #&#8288;33 [dembrandt](https://github.com/dembrandt/dembrandt) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Nov 2026</sub>

**CLI that extracts a website's design tokens and flags design drift in CI.**

Dembrandt renders a page in Chromium through playwright-core, reads computed styles from the DOM, and outputs colors, typography, spacing, borders, shadows, motion, and component styles. It exports W3C DTCG tokens, Tailwind v4 theme CSS, shadcn/ui themes, DESIGN.md, and HTML or PDF reports. It also compares runs against a baseline and exits 1 on drift, with a GitHub Action and an MCP server for agents.

- **+** Exports DTCG, Tailwind v4 @theme, shadcn/ui theme, and DESIGN.md from one extraction
- **+** --compare exits 1 on token drift; GitHub Action annotates PRs
- **+** MCP server with job-based tools, installable via npx in Cursor, VS Code, Claude Code
- **+** Multi-page crawl, sitemap discovery, dark mode, mobile viewport, and authenticated page access
- **−** Requires a separate one-time Chromium download via install-browser
- **−** Canvas/WebGL sites cannot be analyzed; dark mode needs an explicit flag
- **−** Hover and focus states are sampled; pointer-path or timer-driven states are missed
- **−** Team drift dashboard and ingest API sit in a separate beta app tied to an account

<sub>no GPU · Needs Node.js 18+, Chromium via playwright-core · [Repo](https://github.com/dembrandt/dembrandt) · [📖 Docs ↗](https://github.com/dembrandt/dembrandt/blob/main/docs/usage.md) · [🌐 Site ↗](https://www.dembrandt.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dembrandt/)</sub>

<a name="dbhub"></a>
### #&#8288;34 [dbhub](https://github.com/bytebase/dbhub) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Nov 2026</sub>

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

<a name="repowise"></a>
### #&#8288;35 [repowise](https://github.com/repowise-dev/repowise) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · AGPL-3.0 · Nov 2026</sub>

**Local code index exposed to coding agents over MCP, plus a dashboard.**

Repowise indexes a repository's call graph (29 languages), git history, tests and mined decisions locally, then serves them to coding agents through ten MCP tools and to people through a web dashboard. Indexing makes no LLM calls and needs no API key. It reports callers, change risk, tests to run, per-file health scores and dead code, and can run as CI gates.

- **+** Graph, risk, health, tests and dead-code analysis are deterministic and need no API key
- **+** Ten task-shaped MCP tools work with Claude Code, Codex, Cursor and other MCP hosts
- **+** README benchmark on django/django: 3.8 tool calls versus 7.2 without it
- **+** CI gates for patch coverage, doc drift, security and change risk, with SARIF output
- **−** AGPL-3.0 license limits embedding in closed-source products
- **−** Dashboard needs Node 20+ and downloads the UI on first run
- **−** Generated answers and docs need a separate `repowise generate` step with a model
- **−** Benchmark figures come from the project's own docs, not independent tests

<sub>Docker + Compose · Needs Node 20+ (dashboard), uv, pipx or pip · [Repo](https://github.com/repowise-dev/repowise) · [▶️ Demo ↗](https://www.repowise.dev/) · [📖 Docs ↗](https://docs.repowise.dev) · [🌐 Site ↗](https://www.repowise.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repowise/)</sub>

<a name="wigolo"></a>
### #&#8288;36 [wigolo](https://github.com/knockoutez/wigolo) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · custom license · Nov 2026</sub>

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

<a name="mcp-memory-service"></a>
### #&#8288;37 [mcp-memory-service](https://github.com/doobidoo/mcp-memory-service) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="mobile-mcp"></a>
### #&#8288;38 [mobile-mcp](https://github.com/mobile-next/mobile-mcp) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Nov 2026</sub>

**MCP server that lets agents drive iOS and Android devices and emulators.**

Mobile MCP exposes MCP tools for controlling iOS simulators, Android emulators and real devices: listing devices, installing and launching apps, tapping, swiping, typing, screenshots, screen recording and device logs. It prefers the native accessibility tree and falls back to screenshots and coordinates. It runs over stdio by default, or as a Streamable HTTP server with an optional Bearer token.

- **+** Same tool set across iOS simulators, Android emulators and real devices
- **+** Reads the accessibility tree first, so most steps need no vision model
- **+** Install command configures detected clients; HTTP mode supports Bearer auth
- **+** Includes device logs, crash reports, screen recording and a batch command tool
- **−** Requires Xcode command line tools and Android Platform Tools installed locally
- **−** Remote device tools depend on the separate Mobile Next Cloud service
- **−** Mirroring plugin needs a kitty-graphics terminal such as kitty or Ghostty
- **−** Some tools are platform-limited, e.g. clear app data on Android and iOS Simulator only

<sub>no GPU · Docker · Needs Node.js 20+, Xcode command line tools, Android Platform Tools (adb), MCP-compatible client · [Repo](https://github.com/mobile-next/mobile-mcp) · [📖 Docs ↗](https://github.com/mobile-next/mobile-mcp/wiki) · [🌐 Site ↗](https://mobilenext.ai/cloud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mobile-mcp/)</sub>

<a name="aos-ce"></a>
### #&#8288;39 [aos-ce](https://github.com/unicity-aos/aos-ce) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="browser-tools-mcp"></a>
### #&#8288;40 [browser-tools-mcp](https://github.com/agentdeskai/browser-tools-mcp) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

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

<a name="semble"></a>
### #&#8288;41 [semble](https://github.com/minishlab/semble) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Nov 2026</sub>

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

<a name="devspace"></a>
### #&#8288;42 [devspace](https://github.com/waishnav/devspace) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Nov 2026</sub>

**MCP server that gives ChatGPT and Claude your local repo and coding agents.**

DevSpace runs locally and exposes an MCP endpoint (/mcp on port 7676) through a tunnel you provide, so ChatGPT, Claude or Grok Bot can open an allowed folder, edit files, run shell commands and show a diff review card. It also has a `devspace agents` CLI that lets one coding agent hand work to Codex, Claude Code, OpenCode, Pi, Cursor, Copilot or Grok Build, using Git worktrees for parallel writers.

- **+** Runs locally with your own credentials; no DevSpace-hosted service
- **+** Delegates to existing agent CLIs and subscriptions, with per-task Git worktrees
- **+** Markdown agent profiles map named roles like planner and reviewer to models
- **+** Owner password approval on connect; you choose which root folders a host may open
- **−** Connected hosts get shell execution on your machine, so the trust surface is large
- **−** Needs a public HTTPS tunnel you set up for ChatGPT or Claude connectors
- **−** Windows needs Git Bash or WSL; PowerShell and cmd.exe alone are unsupported
- **−** Dynamic workflows are experimental and gated behind an environment variable

<sub>no GPU · Needs Node >=22.19 <27, Git, Bash, Tunnel (Cloudflare Tunnel, ngrok, Pinggy, Tailscale Funnel or HTTPS reverse proxy), SQLite · Models: ChatGPT, Claude, Grok Bot, Codex, Claude Code · port 7676 · [Repo](https://github.com/waishnav/devspace) · [📖 Docs ↗](https://devspace.run/docs) · [🌐 Site ↗](https://devspace.run) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devspace/)</sub>

<a name="supabase-mcp"></a>
### #&#8288;43 [supabase/mcp](https://github.com/supabase/mcp) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="mcphub"></a>
### #&#8288;44 [mcphub](https://github.com/samanhappy/mcphub) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · Apache-2.0 · Nov 2026</sub>

**Self-hosted gateway that aggregates MCP servers behind one authenticated endpoint.**

MCPHub sits between AI clients and MCP servers, exposing local stdio and remote SSE or Streamable HTTP servers through stable endpoints for all servers, groups, or single servers. It adds bearer keys, OAuth 2.0, per-user credentials, a web dashboard, tool-call logs and health checks. Smart Routing uses pgvector semantic search to pick tools. Config lives in mcp_settings.json or PostgreSQL.

- **+** Routes by group, single server, or semantic Smart Routing at /mcp/$smart
- **+** Supports stdio, SSE and Streamable HTTP servers behind one endpoint
- **+** Per-user encrypted credentials with isolated stdio runtimes
- **+** Hot config changes without downtime; file-based config by default, no database needed
- **−** Social login needs PostgreSQL database mode; Smart Routing uses pgvector
- **−** Database mode requires you to persist MCPHUB_CREDENTIAL_ENCRYPTION_KEY; losing it loses credentials
- **−** Multiple replicas need PostgreSQL and explicit session affinity
- **−** Rust and Playwright servers need the larger latest-full image

<sub>no GPU · Docker + Compose · Needs Docker, PostgreSQL (optional, pgvector for Smart Routing), Node.js >=22 and pnpm 10.12.4 (source builds only) · port 3000 · [Repo](https://github.com/samanhappy/mcphub) · [▶️ Demo ↗](https://demo.mcphub.app/) · [📖 Docs ↗](https://docs.mcphub.app/) · [🌐 Site ↗](https://www.mcphub.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcphub/)</sub>

<a name="desktopcommandermcp"></a>
### #&#8288;45 [desktopcommandermcp](https://github.com/wonderwhy-er/desktopcommandermcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Nov 2026</sub>

**MCP server giving AI clients terminal, filesystem, and document editing access.**

Desktop Commander is an MCP server that lets clients such as Claude Desktop, Cursor, Codex and Gemini CLI run terminal commands, manage processes, and read, search and edit local files. It builds on the MCP Filesystem Server, adding ripgrep-based search, surgical text replacement, in-memory Python/Node/R execution, and Excel, PDF and DOCX support. A remote mode lets ChatGPT and Claude web drive a local machine.

- **+** Interactive process control and sessions for long-running commands like SSH, databases and dev servers
- **+** Native Excel, PDF and DOCX read, write and edit without external tools
- **+** Works with any MCP client; install via npx, Smithery, bash script or Docker
- **+** Remote mode connects ChatGPT and Claude web to commands running locally
- **−** Safety guardrails are a command blocklist and symlink checks, not a sandbox
- **−** Commands run with your user permissions unless you use the Docker option
- **−** Local checkout install requires manual git updates
- **−** Remote mode relies on the mcp.desktopcommander.app service and browser OAuth

<sub>no GPU · Docker · Needs Node.js (npx install), Docker (optional) · Models: Any MCP-compatible client · safety checks passed 14 of 17 · [Repo](https://github.com/wonderwhy-er/desktopcommandermcp) · [🌐 Site ↗](https://mcp.desktopcommander.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/desktopcommandermcp/)</sub>

<a name="mcp"></a>
### #&#8288;46 [awslabs/mcp](https://github.com/awslabs/mcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · Apache-2.0 · Nov 2026</sub>

**MCP servers that give coding agents access to AWS docs and services.**

A monorepo of MCP servers from AWS Labs, each covering an AWS area: documentation lookup, CloudFormation and CDK, EKS, serverless, databases, cost, and healthcare and lifesciences workflows. Local servers run over stdio via uvx and work with Kiro, Cursor, VS Code, Cline, Windsurf and Claude Code. The README points new users to the Agent Toolkit for AWS, which it calls the successor to these servers.

- **+** Many servers (docs, IaC, EKS, databases, cost), each installed separately via uvx
- **+** One-click install links for Kiro, Cursor and VS Code
- **+** Active: last release 2026-11-09, Apache-2.0 licensed
- **+** Hosted AWS Knowledge server needs no local setup
- **−** Servers in this repo support stdio only; Streamable HTTP is not yet available
- **−** SSE support was removed in the latest major versions in May 2025
- **−** README says the most useful projects will move to Agent Toolkit for AWS
- **−** Some servers are deprecated, such as the Cloud Control API server

<sub>no GPU · Needs AWS account and credentials, uv/uvx, MCP client · [Repo](https://github.com/awslabs/mcp) · [📖 Docs ↗](https://docs.aws.amazon.com/aws-mcp/latest/userguide/what-is-mcp-server.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp/)</sub>

<a name="ruvector"></a>
### #&#8288;47 [ruvector](https://github.com/ruvnet/ruvector) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Nov 2026</sub>

**Rust vector database with persistent agent memory and an MCP server.**

RuVector is a Rust vector store with Node.js, Python and WASM bindings. It persists embeddings and metadata to disk, runs local ONNX embeddings (all-MiniLM-L6-v2), and exposes memory recall to agents through an MCP server in the npm package. Graph memory, feedback-based learning (SONA) and typed local decisions are separate packages.

- **+** Embeds in Rust, Node.js and browser WASM; Python via source build
- **+** Local ONNX embeddings, so default retrieval needs no hosted service
- **+** MCP server has a readonly profile; writes need an explicit policy
- **+** Store reopens across processes with metadata filtering
- **−** Python needs a Rust source build; no PyPI wheel is documented
- **−** Typed decisions, graph and learning are separate packages, not default
- **−** Default hash embedder is a test double, not for production decisions
- **−** Broad scope (SONA, RVF, MinCut) makes choosing an entry point harder

<sub>no GPU · Needs Node.js and npm, Rust toolchain (Rust and Python source builds), MCP-compatible client (for MCP use) · Models: ONNX all-MiniLM-L6-v2 embeddings · [Repo](https://github.com/ruvnet/ruvector) · [▶️ Demo ↗](https://ruvnet.github.io/RuVector/explorer/) · [🌐 Site ↗](https://cognitum.one/ruvector) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruvector/)</sub>

<a name="ivanmurzak-unity-mcp"></a>
### #&#8288;48 [ivanmurzak/unity-mcp](https://github.com/ivanmurzak/unity-mcp) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · Apache-2.0 · Nov 2026</sub>

**Unity package exposing Editor and runtime tools to AI agents over MCP.**

Unity-MCP (AI Game Developer) is a Unity package, `com.ivanmurzak.unity.mcp`, plus a Node-based CLI that lets MCP clients such as Claude Code, Codex, Cursor and Copilot read and change scenes, prefabs, assets and C# code, run tests and take screenshots. It can use a local gamedev-mcp-server on 127.0.0.1 or the ai-game.dev cloud relay, and any C# method becomes a tool with an `[AiTool]` attribute.

- **+** RQL query tools cut tool calls and tokens versus one-tool-per-action servers, per the project's benchmark
- **+** Custom C# tools via `[AiTool]`, including runtime tools inside a built game
- **+** CLI covers install, compile, test and RQL queries for scripts and CI
- **+** CI tests on Unity 2022.3, 6000.0, 6000.3 and 6000.6; optional extension packs
- **−** Unity-only; requires Unity 2022.3 or newer
- **−** Cloud is the default and relays tool calls via ai-game.dev, with 90-day event metadata
- **−** Local server defaults to auth `none`; any local process can call tools
- **−** `script-execute` runs arbitrary C# with Editor rights

<sub>no GPU · Needs Unity 2022.3+, Node.js 22.14+ (CLI only), gamedev-mcp-server (local mode) or ai-game.dev account (cloud mode) · Models: Any MCP client: Claude Code, Codex, Cursor, GitHub Copilot, Gemini · [Repo](https://github.com/ivanmurzak/unity-mcp) · [📖 Docs ↗](https://github.com/IvanMurzak/Unity-MCP/blob/main/docs/installation.md) · [🌐 Site ↗](https://ai-game.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ivanmurzak-unity-mcp/)</sub>

<a name="linkedin-mcp-server"></a>
### #&#8288;49 [linkedin-mcp-server](https://github.com/stickerdaniel/linkedin-mcp-server) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · Apache-2.0 · Nov 2026</sub>

**MCP server that drives your LinkedIn browser session for profiles, jobs and messages.**

Python MCP server that automates a Patchright Chromium session logged in to your LinkedIn account. It exposes about 25 tools to read profiles, companies, jobs, feed and posts, search people, and send messages or connection requests. Runs over stdio or streamable HTTP, with install paths for uvx, Docker, Claude Desktop MCPB and Claude Code, Codex and Cursor plugins.

- **+** Broad tool set: profiles, companies, jobs, inbox, people and post search, connection requests
- **+** Can import an existing LinkedIn session from Chrome, Brave, Edge, Arc and others
- **+** HTTP mode supports bearer-token auth, required for non-loopback hosts
- **+** Several MCP clients can share one browser session and login
- **−** Scrapes through a browser session, so LinkedIn page changes can break tools and need frequent updates
- **−** Automating a personal account may conflict with LinkedIn terms of service
- **−** Chrome 127+ app-bound (v20) cookies cannot be imported; manual login is needed
- **−** README promotes several paid hosted alternatives as sponsors

<sub>no GPU · Docker + Compose · Needs uv, Patchright Chromium, LinkedIn account · port 8000 · [Repo](https://github.com/stickerdaniel/linkedin-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/linkedin-mcp-server/)</sub>

<a name="argent"></a>
### #&#8288;50 [argent](https://github.com/software-mansion/argent) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Nov 2026</sub>

**Tools that let coding agents drive iOS, Android, TV and Electron apps.**

Argent is a tool set installed with `npx @swmansion/argent@latest init` that lets an AI assistant control iOS simulators, Android emulators and devices, Apple TV, Android TV, Fire TV, and Electron/Chromium apps. It covers taps, swipes and typing, e2e recording and replay, visual regression diffs, profiling (Hermes, React DevTools, Xcode Instruments, Perfetto), and log and network inspection. It is aimed at React Native workflows.

- **+** Covers iOS, Android, Apple TV, Android TV, Fire TV and Electron/Chromium targets
- **+** Records a path once as an e2e test and replays it deterministically
- **+** Profiling via Hermes, React DevTools, Xcode Instruments and Perfetto
- **+** Inspects logs, XHR/fetch/native network traffic and native and React trees
- **−** Ships proprietary binaries (simulator-server, ax-service, .dylib files) under restricted terms
- **−** Telemetry is opt-out rather than opt-in
- **−** Protocol and supported editors are not described in the README itself
- **−** Strongest fit is React Native; other stacks get less documented support

<sub>Needs Node.js (npx), iOS simulator / Android emulator or device · [Repo](https://github.com/software-mansion/argent) · [📖 Docs ↗](https://docs.swmansion.com/argent/docs/fundamentals/installation) · [🌐 Site ↗](https://argent.swmansion.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/argent/)</sub>

<a name="grepai"></a>
### #&#8288;51 [grepai](https://github.com/yoanbernabeu/grepai) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**CLI for semantic code search with call-graph tracing and an MCP server.**

grepai indexes a codebase with vector embeddings and answers natural-language queries such as "authentication logic", instead of exact text or regex matches. A file watcher daemon keeps the index current, and `grepai trace callers` finds callers of a function. It also runs as an MCP server so agents like Claude Code, Cursor and Windsurf can call it as a tool.

- **+** Natural-language queries find code even when naming conventions differ
- **+** Embeddings can come from local Ollama or LM Studio, so code stays on the machine
- **+** File watcher daemon keeps the index updated without manual reindexing
- **+** Call-graph tracing and MCP server support, installable via Homebrew, shell script or PowerShell
- **−** Needs a separately installed embedding provider (Ollama, LM Studio or OpenAI)
- **−** Using OpenAI as provider sends code to an external service
- **−** Pull requests are not accepted; contributions go through issues only
- **−** Token-saving claims come from user quotes, with no benchmark in the README

<sub>Compose · Needs Ollama, LM Studio, OpenAI · Models: nomic-embed-text · [Repo](https://github.com/yoanbernabeu/grepai) · [📖 Docs ↗](https://yoanbernabeu.github.io/grepai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/grepai/)</sub>

<a name="mcp-grafana"></a>
### #&#8288;52 [mcp-grafana](https://github.com/grafana/mcp-grafana) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · Apache-2.0 · Nov 2026</sub>

**MCP server exposing Grafana dashboards, datasources, alerting and incidents to agents.**

A Go MCP server that lets an MCP client query a Grafana instance: search and patch dashboards, run PromQL and LogQL, manage alert rules, incidents, OnCall schedules and annotations. Many integrations (SQL, CloudWatch, InfluxDB, Elasticsearch, admin) are off by default and enabled with --enabled-tools. Runs via uvx, Docker, binary or Helm, authenticating with a Grafana service account token.

- **+** Covers dashboards, Prometheus, Loki, alerting, incidents and OnCall in one server
- **+** Dashboard summary and JSONPath property tools reduce context window use
- **+** SQL queries go through Grafana datasource plugins, so the server never sees credentials
- **+** Optional tool groups and a --disable-write flag limit what the agent can do
- **−** Requires Grafana 9.0 or later; some datasource features fail on older versions
- **−** Many tool groups (SQL, CloudWatch, InfluxDB, admin, panel queries) are disabled by default
- **−** Agent Observability tools work only in Grafana Cloud
- **−** Fetching full dashboard JSON can consume large amounts of context

<sub>no GPU · Docker + Compose · Needs Grafana 9.0+, Grafana service account token, uv (for uvx quick start) · [Repo](https://github.com/grafana/mcp-grafana) · [📖 Docs ↗](https://pkg.go.dev/github.com/grafana/mcp-grafana) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-grafana/)</sub>

<a name="open-computer-use"></a>
### #&#8288;53 [open-computer-use](https://github.com/ifuryst/open-computer-use) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Nov 2026</sub>

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

<a name="kubeshark"></a>
### #&#8288;54 [kubeshark](https://github.com/kubeshark/kubeshark) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

**eBPF network traffic indexing for Kubernetes, with an MCP server for AI agents.**

Kubeshark captures and indexes cluster-wide traffic at the kernel level with eBPF, parses L7 protocols such as HTTP, gRPC, Redis, Kafka and DNS, and decrypts TLS without key management. It offers a web dashboard, a workload dependency map, a CEL-based filter language (KFL) and PCAP export for Wireshark. An MCP server and Claude Code skills let AI agents query traffic for root cause analysis.

- **+** eBPF TLS/mTLS decryption without sidecars or key management
- **+** Retrospective PCAP export by time, node, workload and IP, with S3, Azure Blob or GCS storage
- **+** MCP server plus Network RCA and KFL skills installable as a Claude Code plugin
- **+** Parses HTTP, gRPC, GraphQL, Redis, Kafka and DNS with no code instrumentation
- **−** Only useful on Kubernetes clusters; no standalone or non-Kubernetes mode is described
- **−** Kernel-level capture on every node; resource overhead is not documented in the README
- **−** Port-forward setup is not for production; an ingress controller is recommended
- **−** KFL is a custom query language that users must learn to filter effectively

<sub>no GPU · Needs Kubernetes, Helm · Models: MCP-compatible assistants (Claude Code, Cursor, Copilot) · port 8899 · [Repo](https://github.com/kubeshark/kubeshark) · [▶️ Demo ↗](https://demo.kubeshark.com/) · [📖 Docs ↗](https://docs.kubeshark.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubeshark/)</sub>

<a name="dev-browser"></a>
### #&#8288;55 [dev-browser](https://github.com/sawyerhood/dev-browser) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · MIT · Nov 2026</sub>

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

<sub>no GPU · Needs Chrome or Chromium · [Repo](https://github.com/sawyerhood/dev-browser) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dev-browser/)</sub>

<a name="docs-mcp-server"></a>
### #&#8288;56 [docs-mcp-server](https://github.com/arabold/docs-mcp-server) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2026</sub>

**Version-aware docs index that feeds library documentation to coding assistants.**

Fetches documentation from websites, GitHub repositories, npm, PyPI, local folders and archives, and indexes it per library version in a local SQLite database. Search is exposed over MCP (stdio or Streamable HTTP), a CLI and a web UI. Full-text search works by default; vector search is optional via OpenAI, Ollama, Gemini, Vertex AI, AWS Bedrock, Azure OpenAI or OpenAI-compatible servers.

- **+** Stores each library version separately, so searches match the version a project uses
- **+** Indexes websites, GitHub, npm, PyPI, ZIP/TAR, PDF, Office, EPUB and notebooks
- **+** Runs via npx or Docker with a local SQLite index, no external database
- **+** Works without an embedding model; Ollama keeps document text on the machine
- **−** Usage telemetry is on by default and must be turned off manually
- **−** Docs indexed before an embedding model is set get no vectors until re-scraped
- **−** You add and refresh each library yourself; scrape refuses existing versions
- **−** MCP endpoint is unauthenticated unless OAuth2/OIDC is configured separately

<sub>no GPU · Docker + Compose · Needs Node.js 22+ or Docker, Optional embedding provider (OpenAI, Ollama, Gemini, Vertex AI, AWS Bedrock, Azure OpenAI) · Models: OpenAI, Ollama, Gemini, Vertex AI, AWS Bedrock · port 6280 · [Repo](https://github.com/arabold/docs-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/docs-mcp-server/)</sub>

<a name="figwright"></a>
### #&#8288;57 [figwright](https://github.com/awdr74100/figwright) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**Two-way Figma MCP server that reads and edits designs through a plugin.**

Figwright runs an MCP server over stdio and relays tool calls through a local WebSocket on 127.0.0.1:3055 to a Figma plugin. Its 135 tools read selections and design context for codegen, and write frames, auto-layout, styles, variables, components and animations back to the canvas. It works on the free Figma tier, with no Dev Mode seat needed, and ships two optional skills for codegen and building designs.

- **+** Reads and writes the canvas with 135 tools, not read-only
- **+** Works on the free Figma tier, no paid Dev Mode seat
- **+** Runs locally; relay checks Host and Origin headers on loopback
- **+** Several agents can work at once, each claiming its own open Figma file
- **−** Plugin is not on Figma Community; manual import from a release zip
- **−** Server and plugin update separately, so version drift is common
- **−** Needs Figma desktop app to import the plugin
- **−** Write and export tools can be misused by prompt-injected agents

<sub>no GPU · Needs Node.js 20.19+ or 22.12+, Figma desktop app, MCP client (Claude Code, Cursor, etc.), Figwright Figma plugin · port 3055 · [Repo](https://github.com/awdr74100/figwright) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/figwright/)</sub>

<a name="mobilebuildmcp"></a>
### #&#8288;58 [mobilebuildmcp](https://github.com/getsentry/mobilebuildmcp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Oct 2026</sub>

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

<a name="androguard"></a>
### #&#8288;59 [androguard](https://github.com/androguard/androguard) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · Apache-2.0 · Oct 2026</sub>

**Python toolkit and MCP server for Android APK reverse engineering.**

Androguard 5 opens APKs and DEX files to inspect the manifest, permissions, classes and strings, disassemble Dalvik, decompile to Java, find cross-references and run a vulnerability scanner. Optional extras cover ARM64 native code and APK decode/rebuild. It is usable from a CLI, a Python Application API, Claude Code skills, or an androguard-mcp server for LLM hosts.

- **+** Covers APK, DEX, Dalvik disassembly, Java decompilation, ARM64 and APK patching in one toolkit
- **+** Ships an MCP server and Claude Code skills (/analyze-apk, /scan-vulns, /find-refs)
- **+** scan_vulns is validated against all OWASP MASTG Android demos, with results in docs
- **+** Parsing layers are separate Rust-backed libraries with Python bindings
- **−** v5 is not on PyPI yet; pip install androguard currently pulls 4.1.4 and replaces 5.0.0
- **−** Source install needs a Rust toolchain and sibling apk-parser and dex-parser checkouts
- **−** Docs are marked outdated; the cross-reference Analysis object is not yet restored in v5
- **−** Releases since 4.0 dropped features from 3.3.5, which can break older scripts

<sub>no GPU · Needs Python, Rust toolchain (source install and optional extras), apk-parser, dex-parser · [Repo](https://github.com/androguard/androguard) · [📖 Docs ↗](http://androguard.github.io/androguard/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/androguard/)</sub>

<a name="playwriter"></a>
### #&#8288;60 [playwriter](https://github.com/remorses/playwriter) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Nov 2026</sub>

**Lets agents drive your running Chrome via Playwright, CLI or MCP.**

Playwriter attaches to your already-running Chrome through an extension and exposes the full Playwright API via a CLI and an MCP server with a single `execute` tool. Agents reuse your logins, cookies and extensions instead of launching a fresh browser. A local WebSocket relay on port 19988 bridges the extension and the client, with optional remote control and tunnel access.

- **+** Uses your real Chrome profile: logins, cookies and extensions, no relaunch or debug flags
- **+** One `execute` tool exposes full Playwright API plus raw CDP, debugger and live code editing
- **+** Sessions keep persistent `state` between calls and can use named Chrome tab groups
- **+** Remote control and `serve --token` let another machine or agent drive the browser
- **−** Requires the Chrome extension and a click on each tab to grant control
- **−** Remote control is not a sandbox; the agent gets full access to shared tabs
- **−** Sends anonymous usage telemetry to Strada by default; opt out via env var
- **−** Agent code runs in your real logged-in sessions, so mistakes affect real accounts

<sub>no GPU · Needs Chrome or Chromium, Playwriter Chrome extension, Node.js, ffmpeg (video recording) · port 19988 · [Repo](https://github.com/remorses/playwriter) · [📖 Docs ↗](https://playwriter.dev/docs/sessions) · [🌐 Site ↗](https://playwriter.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/playwriter/)</sub>

<a name="ext-apps"></a>
### #&#8288;61 [ext-apps](https://github.com/modelcontextprotocol/ext-apps) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · custom license · Nov 2026</sub>

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

<a name="codedb"></a>
### #&#8288;62 [codedb](https://github.com/justrach/codedb) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · BSD-3-Clause · Nov 2026</sub>

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

<a name="gitdiagram"></a>
### #&#8288;63 [gitdiagram](https://github.com/ahmedkhaleel2004/gitdiagram) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

**Turns a GitHub repository into an interactive architecture diagram.**

Next.js app that takes a public or private GitHub repository and generates a Mermaid architecture diagram with a streamed explanation. Components link to files and directories in the repo, and diagrams export as PNG or Mermaid source. It also exposes a remote MCP server at gitdiagram.com/mcp and a Markdown version of each diagram, and can generate narrated explainer videos.

- **+** Hosted instance and MCP server need no key or sign-in
- **+** Diagram nodes link to the repo's files and directories
- **+** Exports PNG or Mermaid source; Markdown view at /owner/repo.md
- **+** Private repos supported with a GitHub token
- **−** Self-hosting needs Cloudflare R2, Upstash Redis and an OpenAI or OpenRouter key
- **−** Creating new explainer videos is early access and off by default locally
- **−** Local video generation needs Anthropic, OpenAI and OpenRouter keys
- **−** MCP server only covers public repositories

<sub>no GPU · Docker · Needs Bun, Cloudflare R2, Upstash Redis, OpenAI or OpenRouter API key, Anthropic API key (videos) · Models: OpenAI, OpenRouter, Anthropic Claude (videos) · port 3000 · [Repo](https://github.com/ahmedkhaleel2004/gitdiagram) · [▶️ Demo ↗](https://gitdiagram.com/) · [🌐 Site ↗](https://gitdiagram.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitdiagram/)</sub>

<a name="browsermcp-mcp"></a>
### #&#8288;64 [browsermcp/mcp](https://github.com/browsermcp/mcp) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.4k · Apache-2.0 · Nov 2026</sub>

**MCP server that lets coding agents drive your own signed-in Chrome.**

Browser MCP runs an MCP server (npx @browsermcp/mcp@latest) that forwards a `browser` tool to a per-user local daemon. The daemon controls Chrome tabs with Playwright through a chrome.debugger extension that only talks to 127.0.0.1. It works with Claude Code, Cursor, VS Code, Codex and Claude Desktop, using your existing profile and logged-in sites.

- **+** Uses your real Chrome profile and signed-in sessions instead of a fresh headless browser
- **+** Everything runs locally; extension connects only to the daemon on 127.0.0.1
- **+** Pairing requires clicking Allow and matching a six-digit code once per computer
- **+** Extension refuses incognito, browser pages and extension pages unless configured, and has a Stop button
- **−** Chromium browsers only; Firefox has no debugger API so it does not work
- **−** Self-built extension must be updated by hand with git pull and rebuild
- **−** Needs Node.js 24 or later to build; having both store and self-built extensions causes double connections
- **−** No release published; version tracking relies on the npm package

<sub>no GPU · Needs Node.js 24+, Chrome or Chromium browser, Browser MCP extension, Playwright · [Repo](https://github.com/browsermcp/mcp) · [📖 Docs ↗](https://browsermcp.io/docs) · [🌐 Site ↗](https://browsermcp.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browsermcp-mcp/)</sub>

<a name="maildev"></a>
### #&#8288;65 [maildev](https://github.com/maildev/maildev) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Sep 2026</sub>

**Local SMTP catcher with a web inbox and an optional MCP server.**

MailDev is a Node.js SMTP server for development that accepts mail on port 1025 and shows it in a React web UI on port 1080, with HTML, text and header views, attachments and live updates over WebSocket. It also has a REST API, a Node.js API, optional relay to a real SMTP server, and an `--mcp` flag that exposes the inbox to MCP clients at `/mcp`.

- **+** Install with npm or `docker run -p 1080:1080 -p 1025:1025 maildev/maildev`
- **+** Selective or auto relay to an outgoing SMTP server, with allow/deny rules
- **+** MCP endpoint lets agents search emails and extract verification links and tokens
- **+** Optional web basic auth, HTTPS, mail persistence directory and `--max-emails` cap
- **−** MCP is a side feature; the core job is catching mail, not agent tooling
- **−** Keeps all emails in memory by default; about 150 MB heap per 10,000 emails
- **−** v3 is a full rewrite; v2 users must follow the upgrade guide

<sub>no GPU · Docker · Needs Node.js · port 1080 · [Repo](https://github.com/maildev/maildev) · [📖 Docs ↗](https://maildev.github.io/maildev/docs/guides/upgrading/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maildev/)</sub>

<a name="google-workspace-mcp"></a>
### #&#8288;66 [google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Nov 2026</sub>

**MCP server exposing Gmail, Drive, Calendar, Docs, Sheets and more to AI clients.**

Python MCP server with 120+ tools across twelve Google services, including Gmail, Drive, Calendar, Docs, Sheets, Slides, Forms, Tasks, Contacts, Chat and Apps Script. It runs over stdio or streamable HTTP, supports OAuth 2.1 multi-user auth, and uses your own Google OAuth client. A companion CLI, workspace-cli, lists and calls tools against a running server.

- **+** Tool tiers (core, extended, complete) plus --tools, --read-only and --disabled-tools limit context size
- **+** OAuth 2.1 multi-user auth, stateless mode, external OAuth provider and service-account delegation
- **+** Sends no data except to Google APIs; no telemetry, tracing off unless OTLP is configured
- **+** Includes workspace-cli and a bundled Claude Code skill for tool routing
- **−** Requires creating your own Google Cloud project, OAuth client and enabling each API
- **−** Google Chat needs a separate Chat app configuration and a Workspace account
- **−** OAuth 2.1 mode needs HTTP transport; stdio is described as legacy
- **−** Full tool set is large; loading everything inflates client context

<sub>no GPU · Docker + Compose · Needs Google Cloud OAuth client, Google Workspace APIs, Valkey/Redis (optional), GCS (optional) · port 8000 · [Repo](https://github.com/taylorwilsdon/google_workspace_mcp) · [📖 Docs ↗](https://workspacemcp.com/docs) · [🌐 Site ↗](https://workspacemcp.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-workspace-mcp/)</sub>

<a name="sem"></a>
### #&#8288;67 [sem](https://github.com/ataraxy-labs/sem) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · Apache-2.0 · Nov 2026</sub>

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

<a name="webcodex"></a>
### #&#8288;68 [webcodex](https://github.com/yyjeqhc/webcodex) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

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

<a name="mcp-server-kubernetes"></a>
### #&#8288;69 [mcp-server-kubernetes](https://github.com/flux159/mcp-server-kubernetes) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

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

<a name="claude-code-agent-monitor"></a>
### #&#8288;70 [claude-code-agent-monitor](https://github.com/hoangsonww/claude-code-agent-monitor) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Local dashboard for monitoring Claude Code, Cursor and Codex agent sessions.**

CCAM collects Claude Code, Cursor and Codex activity through native hooks and transcript discovery. It shows sessions, conversations, agent trees, token usage and estimated cost in a React dashboard backed by SQLite. It can also launch and resume Claude Code or Codex runs, and ships a `ccam` CLI, an MCP server, desktop apps and plugins.

- **+** Covers Claude Code, Cursor and Codex in the same views
- **+** Binds to 127.0.0.1 by default; optional tokens for remote exposure
- **+** Ships CLI, MCP server, desktop apps, Docker, Kubernetes and Terraform
- **+** Cost snapshot script compares usage before and after an upgrade
- **−** Requires Node.js 22.22 or newer and npm 9 or newer
- **−** Cost figures are API-equivalent estimates, not billed amounts
- **−** Run-agent launching covers Claude Code and Codex, not Cursor
- **−** Large surface (plugins, desktop, IaC) adds setup and maintenance overhead

<sub>no GPU · Docker + Compose · Needs Node.js >=22.22, npm >=9, SQLite · Models: Claude Code, Cursor, OpenAI Codex · port 4820 · [Repo](https://github.com/hoangsonww/claude-code-agent-monitor) · [📖 Docs ↗](https://github.com/hoangsonww/Claude-Code-Agent-Monitor/wiki) · [🌐 Site ↗](https://hoangsonww.github.io/Claude-Code-Agent-Monitor/wiki/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-agent-monitor/)</sub>

<a name="cloudbase-ai-toolkit"></a>
### #&#8288;71 [cloudbase-ai-toolkit](https://github.com/tencentcloudbase/cloudbase-ai-toolkit) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**MCP server, skills and plugins connecting AI coding tools to CloudBase.**

Ships the npm package @cloudbase/cloudbase-mcp plus Agent Skills and IDE plugins, so AI coding tools can manage a Tencent CloudBase backend from chat. The MCP server covers PostgreSQL and document databases, cloud functions, Cloud Run, storage, auth, static hosting and logs. It runs locally via npx or as a remote HTTP endpoint with OAuth or static keys.

- **+** Remote MCP endpoint with browser OAuth; no local Node or keys in config
- **+** Deletes and destructive SQL pause for a confirmation naming the target
- **+** Setup guides for over 20 IDEs and CLIs, including Cursor and Claude Code
- **+** MIT licensed; v2.37.x released in November 2026
- **−** Requires a Tencent CloudBase environment; backend is tied to one vendor
- **−** Remote mode lacks local file upload and template download
- **−** International site does not yet expose NoSQL tools in remote mode
- **−** Usage beyond CloudBase free quotas is billed

<sub>no GPU · Needs Tencent CloudBase environment, Node.js 18.15.0+ (local mode) · [Repo](https://github.com/tencentcloudbase/cloudbase-ai-toolkit) · [▶️ Demo ↗](https://cloud1-5g39elugeec5ba0f-1300855855.tcloudbaseapp.com/gobang/#/) · [📖 Docs ↗](https://docs.cloudbase.net/ai/cloudbase-ai-toolkit/getting-started) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloudbase-ai-toolkit/)</sub>

<a name="flint-chart"></a>
### #&#8288;72 [flint-chart](https://github.com/microsoft/flint-chart) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

**Chart spec compiler and MCP server for agents, with five rendering backends.**

Flint compiles short, human-editable chart specs (data, semantic types, chart type, theme, interactions) into native specs for Vega-Lite, ECharts, Chart.js, Plotly and Excel. It ships as an npm library with a React component and as an MCP server that agents use over stdio or a hosted HTTP endpoint. It covers 52 chart types, 14 preset themes and 23 interaction presets.

- **+** Same spec renders on Vega-Lite, ECharts, Chart.js, Plotly and native Excel charts
- **+** Semantic field types drive parsing, scales, axes and colors, so specs stay short
- **+** MCP server runs locally via npx (stdio) or as a hosted HTTP endpoint
- **+** Includes authoring skills for coding agents, plus themes and interaction events
- **−** Python port is source-only in packages/flint-py and not yet released
- **−** FlintChart component needs React as a peer; other pages use mountChart
- **−** Hosted MCP endpoint sends chart data to a third-party server
- **−** Only at version 1.x, released October 2026, so the API may still change

<sub>no GPU · Needs Node.js (npx), React (optional peer) · [Repo](https://github.com/microsoft/flint-chart) · [▶️ Demo ↗](https://microsoft.github.io/flint-chart/#/gallery) · [📖 Docs ↗](https://microsoft.github.io/flint-chart/#/mcp) · [🌐 Site ↗](https://microsoft.github.io/flint-chart/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flint-chart/)</sub>

<a name="stealth-browser-mcp"></a>
### #&#8288;73 [stealth-browser-mcp](https://github.com/vibheksoni/stealth-browser-mcp) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Nov 2026</sub>

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

<a name="arxiv-mcp-server"></a>
### #&#8288;74 [arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Nov 2026</sub>

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

<a name="markdownify-mcp"></a>
### #&#8288;75 [markdownify-mcp](https://github.com/zcaceres/markdownify-mcp) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

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

<a name="x64dbg-mcp-server"></a>
### #&#8288;76 [x64dbg-mcp-server](https://github.com/duty1g/x64dbg-mcp-server) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Nov 2026</sub>

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

<a name="gortex"></a>
### #&#8288;77 [gortex](https://github.com/zzet/gortex) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

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

<a name="aktools"></a>
### #&#8288;78 [aktools](https://github.com/akfamily/aktools) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**HTTP API and MCP server exposing AKShare financial data.**

AKTools wraps the AKShare financial data library (over a thousand interfaces) behind a FastAPI HTTP API at /api/public/<interface_name> and an MCP server. The MCP server offers three tools: search_interfaces, describe_interface and get_data. Results can be returned as JSON, CSV or XLSX, with a 60-second default result cache and optional bearer-token auth.

- **+** Every AKShare function is reachable by name; new AKShare interfaces work after an upgrade
- **+** MCP server runs via uvx with no prior install or manual service start
- **+** Built-in interface search and parameter lookup at /api/interfaces
- **+** Optional --token auth, CSV/XLSX export, and Gunicorn + Uvicorn Docker deployment
- **−** Data quality and breakage depend on upstream sites scraped by AKShare
- **−** Some interfaces need a mainland China network environment
- **−** No user login; per-user access needs an external authenticating reverse proxy
- **−** Docs and README are primarily in Chinese

<sub>no GPU · Docker · Needs AKShare, Python 3.11+, uv (for MCP via uvx), FastAPI, Gunicorn + uvicorn-worker (production) · port 8080 · [Repo](https://github.com/akfamily/aktools) · [📖 Docs ↗](https://aktools.akfamily.xyz/) · [🌐 Site ↗](https://aktools.akfamily.xyz/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aktools/)</sub>

<a name="cocoindex-code"></a>
### #&#8288;79 [cocoindex-code](https://github.com/cocoindex-io/cocoindex-code) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (50) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="jshookmcp"></a>
### #&#8288;80 [jshookmcp](https://github.com/vmoranv/jshookmcp) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Nov 2026</sub>

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

<a name="gitlab-mcp"></a>
### #&#8288;81 [gitlab-mcp](https://github.com/zereight/gitlab-mcp) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Nov 2026</sub>

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

<a name="terravision"></a>
### #&#8288;82 [terravision](https://github.com/patrickchugh/terravision) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · AGPL-3.0 · Nov 2026</sub>

**Cloud architecture diagrams from Terraform or a prompt, via CLI or MCP.**

TerraVision draws AWS, Azure and GCP architecture diagrams with official icons, grouped by VPC, subnet, zone or resource group. It builds them from `terraform plan` output locally, or from a plain-English description through an MCP server, Claude Desktop extension or ChatGPT/Codex plugin. Output is PNG, SVG, draw.io or interactive HTML, and a GitHub Action can redraw diagrams in CI.

- **+** Draws from code and a tfvars file, so no cloud account access is needed
- **+** Runs locally; code is not uploaded anywhere
- **+** Outputs PNG, SVG, editable draw.io and clickable interactive HTML
- **+** Ships plugins for Claude, ChatGPT, Codex, plus an MCP server for Copilot and Cursor
- **−** Requires Graphviz and Git installed; Terraform needed for code-to-diagram
- **−** AGPL-3.0 license may restrict use in some organisations
- **−** Terraform generated from a diagram depends on the AI model's quality
- **−** Does not scan live cloud accounts, so drift from deployed state is not shown

<sub>no GPU · Docker · Needs Graphviz, Git, uv, Terraform (optional) · Models: Ollama, AWS Bedrock · [Repo](https://github.com/patrickchugh/terravision) · [📖 Docs ↗](https://patrickchugh.github.io/terravision/) · [🌐 Site ↗](https://terravision.online/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terravision/)</sub>

<a name="sim-use"></a>
### #&#8288;83 [sim-use](https://github.com/lycorp-jp/sim-use) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Nov 2026</sub>

**CLI that lets AI agents read and tap iOS Simulator and Android screens.**

sim-use is a Swift CLI that prints a compact text outline of the current iOS Simulator or Android screen (`ui`) and acts on it with alias, id or label selectors (`tap @9`). It uses Apple Accessibility APIs, the Simulator HID pipeline and an Android AccessibilityService bridge APK behind one command set with `--json` output. A per-device daemon keeps round trips near 300 ms, and `sim-use init` installs a bundled agent skill.

- **+** Outline output is claimed ~16x more compact than a raw JSON accessibility tree
- **+** Same verbs and `--json` shape on iOS Simulator and Android emulator/device
- **+** Selectors: @N alias, #id, --label, or raw coordinates; orientation-aware on iOS
- **+** Installs via Homebrew; `sim-use init` adds a skill for Claude and other clients
- **−** Full feature set is macOS 14+ only; Linux build covers Android verbs only
- **−** Physical iPhones are experimental and limited to ui, tap and screenshot
- **−** Building from source needs locally built idb XCFrameworks and XcodeGen
- **−** Android needs a bridge APK installed per device via `sim-use android init`

<sub>no GPU · Needs macOS 14+, Xcode, Homebrew, adb (Android), Android bridge APK, Swift 6 toolchain (Linux, Android only) · [Repo](https://github.com/lycorp-jp/sim-use) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sim-use/)</sub>

<a name="claude-context"></a>
### #&#8288;84 [claude-context](https://github.com/zilliztech/claude-context) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: patchy (34) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Nov 2026</sub>

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

<sub>no GPU · Needs Node.js >= 20, Milvus or Zilliz Cloud, OpenAI API key (default embedding provider) · Models: OpenAI, VoyageAI, Ollama, Gemini · safety checks passed 9 of 13 · [Repo](https://github.com/zilliztech/claude-context) · [📖 Docs ↗](https://github.com/zilliztech/claude-context/tree/master/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-context/)</sub>

<a name="dashboard-icons"></a>
### #&#8288;85 [dashboard-icons](https://github.com/homarr-labs/dashboard-icons) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="phone-harness"></a>
### #&#8288;86 [phone-harness](https://github.com/phone-harness/phone-harness) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Nov 2026</sub>

**CLI that lets coding agents tap, type and read a real iPhone or Android.**

phone-harness is a Python CLI with pre-imported helpers (open_app, tap_text, type_text, screen, screenshot) that agents call to drive a phone. iPhone control goes through the Mac's iPhone Mirroring window with Apple Vision OCR; Android uses adb and the accessibility tree. A hosted cloud service adds remote Androids and iPhones, and a hosted MCP endpoint plus Hermes and OpenClaw plugins are provided.

- **+** Nothing installed on the phone: no jailbreak, no Xcode
- **+** Same helper API across iPhone, Android and cloud phones
- **+** Android works from macOS, Linux or Windows over USB or Wi-Fi
- **+** Ships a skill, hosted MCP endpoint, and Hermes and OpenClaw plugins
- **−** Local iPhone control needs macOS 15+ and iPhone Mirroring paired to iOS 18+
- **−** OCR reads text only; unlabeled icons need a screenshot and vision model
- **−** No multi-touch, camera or Face ID flows; DRM video renders black
- **−** Hosted MCP supports only cloud phones, which need a Phone Harness Cloud account

<sub>no GPU · Needs adb, uv, Python 3.12, macOS 15+ with iPhone Mirroring (iPhone), Phone Harness Cloud account (cloud phones) · Models: Claude Code, Codex, any MCP client · [Repo](https://github.com/phone-harness/phone-harness) · [📖 Docs ↗](https://phone-harness.com/docs) · [🌐 Site ↗](https://phone-harness.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/phone-harness/)</sub>

<a name="sourcebot"></a>
### #&#8288;87 [sourcebot](https://github.com/sourcebot-dev/sourcebot) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Nov 2026</sub>

**Self-hosted code search and MCP server across all your Git repos.**

Sourcebot indexes repos from GitHub, GitLab, Bitbucket, Azure DevOps or local Git directories. It offers regex and boolean code search in a web app, plus an MCP server exposing code search, file reads, and symbol definitions and references to agents. An optional Ask Sourcebot chat answers codebase questions with cited code, using a language model provider you configure with your own key.

- **+** Indexes GitHub, GitLab, Bitbucket, Azure DevOps and local Git directories in one place
- **+** MCP server gives agents search, file reading, and symbol definitions and references
- **+** Permission syncing can follow code host repository permissions
- **+** Public demo available, and Ask uses your own model provider key
- **−** Requires Docker and Docker Compose; the setup wizard also needs Node.js
- **−** Ask Sourcebot needs a configured language model provider and key
- **−** README points to a pricing page, so some features may be plan-gated

<sub>Compose · Needs Docker, Docker Compose, Node.js · [Repo](https://github.com/sourcebot-dev/sourcebot) · [▶️ Demo ↗](https://app.sourcebot.dev) · [📖 Docs ↗](https://docs.sourcebot.dev) · [🌐 Site ↗](https://www.sourcebot.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sourcebot/)</sub>

<a name="kubernetes-mcp-server"></a>
### #&#8288;88 [kubernetes-mcp-server](https://github.com/containers/kubernetes-mcp-server) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · Apache-2.0 · Nov 2026</sub>

**MCP server that lets agents manage Kubernetes and OpenShift clusters.**

A Go MCP server that talks directly to the Kubernetes API server instead of shelling out to kubectl or helm. It offers generic CRUD on any resource, plus pod logs, exec, top and events, with optional toolsets for Helm, Tekton, KubeVirt, Kiali and observability backends. It ships as a native binary, npm and PyPI packages, and a container image.

- **+** Native Go binary for Linux, macOS and Windows; no kubectl, helm, Node or Python needed
- **+** Toolsets are opt-in, which keeps tool context small for the LLM
- **+** read_only mode and denied_resources (e.g. Secrets) restrict what agents can touch
- **+** Multi-cluster via kubeconfig contexts; optional OTEL tracing and OAuth/OIDC in HTTP mode
- **−** Requires access to a Kubernetes cluster; nothing to try without one
- **−** Runtime settings moved from CLI flags to TOML, so older flag-based setups need migration
- **−** Exec, delete and Helm install tools can change a live cluster unless read_only is set
- **−** Some toolsets (kiali, netobserv, kubevirt) need matching components in the cluster

<sub>no GPU · Docker · Needs Kubernetes or OpenShift cluster, kubeconfig or in-cluster config · [Repo](https://github.com/containers/kubernetes-mcp-server) · [▶️ Demo ↗](https://www.youtube.com/watch?v=l05jQDSrzVI) · [📖 Docs ↗](https://github.com/containers/kubernetes-mcp-server/tree/main/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubernetes-mcp-server/)</sub>

<a name="openlore"></a>
### #&#8288;89 [openlore](https://github.com/aakarim/openlore) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Nov 2026</sub>

**Shared Markdown knowledge server for agents over SSH, MCP and web.**

OpenLore serves a folder of Markdown as a virtual filesystem that agents read with cat, grep and find over SSH, SFTP, or an MCP endpoint, plus a web view. Access is scoped per identity with ro, publish and rw grants per docset, and writes are atomic with compare-and-swap checks. The shell is an in-memory Go interpreter rather than a real OS shell, and no vector database or ingestion pipeline is involved.

- **+** Plain Markdown with no vector database, ingestion pipeline or SDK
- **+** Per-identity docset grants (ro, publish, rw) with inbox-style publishing
- **+** Shell is a Go interpreter: no OS shell escape or process execution
- **+** Same files over SSH, SFTP/SSHFS, MCP and a web view
- **−** Retrieval is grep and find over files, with no semantic search
- **−** Raw SSH has no hostname routing; Render deploy has no public SSH
- **−** Production use needs HTTPS, token and persistent volume setup
- **−** No Docker or compose files detected in the repository

<sub>no GPU · Docker · port 8080 · [Repo](https://github.com/aakarim/openlore) · [📖 Docs ↗](https://openlore.sh/docs/) · [🌐 Site ↗](https://openlore.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openlore/)</sub>

<a name="chunkhound"></a>
### #&#8288;90 [chunkhound](https://github.com/chunkhound/chunkhound) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

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

<a name="mcp-gateway-registry"></a>
### #&#8288;91 [mcp-gateway-registry](https://github.com/agentic-community/mcp-gateway-registry) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Authenticated gateway and registry for MCP servers, A2A agents and skills.**

An nginx reverse proxy (data plane) paired with a FastAPI registry (control plane) that inventories MCP servers, A2A agents, skills and custom entity types, and routes calls through one OAuth-authenticated entry point. It integrates identity providers such as Keycloak, Entra ID, Okta, Auth0, Cognito and PingFederate, and stores state in MongoDB or DocumentDB. Deploys via Docker Compose, Amazon ECS (Terraform) or Amazon EKS (Helm).

- **+** Per-user egress auth (3LO, OBO) keeps third-party SaaS tokens off laptops
- **+** Supports six identity providers, with scope-based access control and audit logging
- **+** Semantic and lexical search for tool discovery; virtual MCP servers aggregate backends
- **+** Helm charts, Terraform for ECS, Compose and prebuilt images provided
- **−** Needs MongoDB or DocumentDB plus an identity provider; heavy for a single developer
- **−** Deployment guides and tooling center on AWS (EC2, ECS, EKS)
- **−** Telemetry is on by default; disable with MCP_TELEMETRY_DISABLED=1
- **−** Recent releases carry breaking changes, e.g. tools wildcard scope semantics in 1.37.0

<sub>no GPU · Docker + Compose · Needs MongoDB or DocumentDB, Identity provider (Keycloak, Entra ID, Okta, Auth0, Cognito or PingFederate), nginx · Models: OpenAI, Amazon Bedrock, OpenAI-compatible endpoints · port 80 · [Repo](https://github.com/agentic-community/mcp-gateway-registry) · [📖 Docs ↗](https://agentic-community.github.io/mcp-gateway-registry/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-gateway-registry/)</sub>

<a name="mcp-for-blender"></a>
### #&#8288;92 [mcp-for-blender](https://github.com/ahujasid/mcp-for-blender) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Nov 2026</sub>

**MCP server and Blender addon that let LLMs build and edit 3D scenes.**

Pairs a Blender addon, which runs a socket server inside Blender, with a Python MCP server that forwards tool calls from clients such as Claude Desktop, Claude Code, Codex and Cursor. The AI can create and modify objects and materials, run Blender Python, check its work through viewport views and renders, and pull assets from Poly Haven, Sketchfab and Poly Pizza or generate models via Meshy, Tripo, Hyper3D Rodin and Hunyuan3D.

- **+** Works with many MCP clients: Claude Desktop, Claude Code, Codex, Cursor, VS Code, OpenCode, Antigravity
- **+** One-line installer configures detected clients and enables the addon, keeping .bak copies of changed files
- **+** Optional safe mode (BLENDER_MCP_SAFE_MODE=1) validates scripts before they run in Blender
- **+** Multiple Blender instances supported by pointing separate client entries at different ports
- **−** Addon socket has no authentication or encryption; anyone reaching the port can run Python in Blender
- **−** Arbitrary Python execution is the default; script checking is opt-in
- **−** Hosted AI 3D generation without your own API keys is a paid Premium feature
- **−** Only one MCP server instance should run at a time, not both Cursor and Claude Desktop

<sub>Docker · Needs Blender 3.0+, Python 3.10+, uv · Models: Poly Haven, Sketchfab, Poly Pizza, Meshy, Tripo · [Repo](https://github.com/ahujasid/mcp-for-blender) · [🌐 Site ↗](https://mcp-for-blender.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-for-blender/)</sub>

<a name="mcp-server-cloudflare"></a>
### #&#8288;93 [mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="lanhu-mcp"></a>
### #&#8288;94 [lanhu-mcp](https://github.com/dsphper/lanhu-mcp) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

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

<a name="api-anything"></a>
### #&#8288;95 [api-anything](https://github.com/goodnight000/api-anything) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Nov 2026</sub>

**Learns a website's own HTTP requests and exposes them to agents as operations.**

API Anything records the request a site's page sends for two example inputs, turns what changed into parameters, and replays it later over plain HTTP, falling back to an in-page fetch or page execution if blocked. It runs as an MCP server over stdio, an HTTP/OpenAPI server, a CLI, a TypeScript library and a Python client. It ships 323 read operations across 114 sites and syncs learned operations through a shared catalog.

- **+** Tier 1 calls are one plain HTTP request, with no browser or account
- **+** Learning uses no LLM; cookies are stored as references, not values
- **+** Ships 114 sites and 323 read operations; setup connects Claude Code, Codex, Cursor and others
- **+** setup --local-only keeps learning and calls on your machine with nothing shared
- **−** Covers only operations someone has taught it; the catalog is described as young
- **−** Reddit and similar sites block plain HTTP; there is no CAPTCHA solving
- **−** Benchmarks cover few sites, one model and a few runs
- **−** No write operations bundled; writes are off by default

<sub>no GPU · Needs Node.js >= 22.13, headless browser (for learning and tier 2/3 fallback) · Models: MCP clients (Claude Code, Codex, Cursor, Claude Desktop, Gemini CLI, VS Code, Hermes), Vercel AI SDK, LangChain.js, OpenAI Agents SDK · [Repo](https://github.com/goodnight000/api-anything) · [▶️ Demo ↗](https://api-anything-registry.forth-site.workers.dev) · [📖 Docs ↗](https://github.com/goodnight000/api-anything/blob/main/INSTALL.md) · [🌐 Site ↗](https://api-anything-registry.forth-site.workers.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/api-anything/)</sub>

<a name="responsively-app"></a>
### #&#8288;96 [responsively-app](https://github.com/responsively-org/responsively-app) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (90) · Freshness: active (91) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · AGPL-3.0 · Nov 2026</sub>

**Desktop browser that previews a page on many device sizes at once.**

Responsively App is an Electron-based browser for macOS, Windows and Linux that renders one URL across many device viewports with mirrored clicks and scrolling. It includes 30+ device profiles, a shared element inspector, and one-click screenshots. It also ships a built-in MCP server on 127.0.0.1:12720, so agents such as Claude Code and Cursor can navigate, click, type and capture per-device screenshots.

- **+** Interactions mirror across all device previews, with one inspector for every device
- **+** MCP tools cover navigate, click, type_text, read_page and per-device screenshots
- **+** Installs via brew, choco, winget, rpm or AppImage; browser extensions send links to it
- **+** 30+ device profiles plus custom devices; hot reloading works with dev servers
- **−** AGPL-3.0 license may restrict use in some commercial or embedded settings
- **−** MCP screenshots capture only the visible viewport, downscaled to at most 1000px wide
- **−** MCP server needs the desktop app running; agent use launches a GUI
- **−** MCP tool set is small: eight tools, no network or console inspection listed

<sub>Needs Node.js (npx) for the MCP launcher · port 12720 · [Repo](https://github.com/responsively-org/responsively-app) · [🌐 Site ↗](https://responsively.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/responsively-app/)</sub>

<a name="ida-pro-mcp"></a>
### #&#8288;97 [ida-pro-mcp](https://github.com/mrexodia/ida-pro-mcp) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (84) · Freshness: active (80) · Maintenance: fair (51) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

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

<a name="ios-simulator-mcp"></a>
### #&#8288;98 [ios-simulator-mcp](https://github.com/joshuayoes/ios-simulator-mcp) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

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

<a name="matlab-mcp-server"></a>
### #&#8288;99 [matlab-mcp-server](https://github.com/matlab/matlab-mcp-server) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · custom license · Nov 2026</sub>

**Official MathWorks MCP server that lets AI agents run and check MATLAB code.**

A Go stdio MCP server that starts or attaches to a local MATLAB (R2021a or later). It exposes tools to evaluate code, run scripts and unit tests, lint files, and list installed toolboxes. It also serves MATLAB coding guideline resources and supports custom tools via JSON extension files.

- **+** Five tools: evaluate code, run .m/.p files, run unit tests, static check, detect toolboxes
- **+** Can attach to an already running MATLAB session (R2023a+) via shareMATLABSession()
- **+** Prebuilt binaries for Windows, Linux and macOS, plus an .mcpb bundle for Claude Desktop
- **+** Custom tools can be added through JSON extension files
- **−** Requires a locally installed, licensed MATLAB; no standalone use
- **−** Usage terms restrict it to one user per server; shared use needs MathWorks contact
- **−** Anonymized telemetry is on by default and must be disabled with a flag
- **−** License is a custom MathWorks file, not a standard open-source license

<sub>no GPU · Needs MATLAB R2021a or later · [Repo](https://github.com/matlab/matlab-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/matlab-mcp-server/)</sub>

<a name="toolkit"></a>
### #&#8288;100 [toolkit](https://github.com/getsentry/toolkit) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 977 · custom license · Nov 2026</sub>

**Sentry MCP server and CLI for debugging errors and traces from coding agents.**

Monorepo containing the Sentry CLI and the Sentry MCP server, which exposes Sentry issues, errors, traces and logs to coding agents such as Cursor and Claude Code. It runs as a hosted remote server on Cloudflare at mcp.sentry.dev, or locally over stdio via `sentry mcp`, including against self-hosted Sentry. A Claude Code plugin adds a `sentry-mcp` subagent.

- **+** Hosted remote endpoint with OAuth, plus stdio mode that reuses the CLI login
- **+** Works with self-hosted Sentry via SENTRY_HOST or an http:// SENTRY_URL
- **+** Skills can be scoped or disabled; calls can be limited to one org or project
- **+** Claude Code plugin delegates Sentry questions to a dedicated subagent
- **−** AI search tools need an OpenAI, Azure OpenAI, Anthropic or OpenRouter key
- **−** Tool set targets debugging workflows, not full Sentry API coverage
- **−** Seer skill is unavailable on self-hosted Sentry unless explicitly enabled
- **−** Parallel tool calls can hit Sentry API rate limits

<sub>no GPU · Needs Sentry (sentry.io or self-hosted), LLM provider API for search tools (OpenAI, Azure OpenAI, Anthropic, OpenRouter), Cloudflare (remote deployment) · Models: OpenAI, Azure OpenAI, Anthropic, OpenRouter · port 5173 · [Repo](https://github.com/getsentry/toolkit) · [📖 Docs ↗](https://cli.sentry.dev/) · [🌐 Site ↗](https://mcp.sentry.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/toolkit/)</sub>

<a name="obsidian-mcp-server"></a>
### #&#8288;101 [obsidian-mcp-server](https://github.com/cyanheads/obsidian-mcp-server) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 717 · Apache-2.0 · Nov 2026</sub>

**MCP server for reading, searching and editing Obsidian vault notes.**

TypeScript MCP server that talks to the Obsidian Local REST API plugin and exposes 14 tools and 3 resources for notes, tags and frontmatter. It can edit a single heading, block or frontmatter field in place, search by text, JSONLogic or Omnisearch, and restrict access with folder-scoped read/write paths. Runs over STDIO or Streamable HTTP.

- **+** Section-level edits to one heading, block or frontmatter field instead of whole-file rewrites
- **+** Folder-scoped read/write paths, deny list and read-only switch
- **+** Mutating tools return before/after byte sizes and recovery hints on errors
- **+** Optional delete confirmation via MCP elicitation; command execution is opt-in
- **−** Requires Obsidian running with the Local REST API plugin v4.0.0 or later
- **−** Delete runs on the first call by default, with no confirmation
- **−** Heading writes on plugin v4.x misplace content in CRLF notes
- **−** Omnisearch mode is unavailable when read or deny path scoping is set

<sub>no GPU · Docker · Needs Obsidian, Obsidian Local REST API plugin (v4.0.0+), Node.js or Bun · [Repo](https://github.com/cyanheads/obsidian-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/obsidian-mcp-server/)</sub>

<a name="artemis"></a>
### #&#8288;102 [artemis](https://github.com/google/artemis) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Sep 2026</sub>

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

<a name="exa-mcp-server"></a>
### #&#8288;103 [exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Nov 2026</sub>

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

<a name="tamery"></a>
### #&#8288;104 [tamery](https://github.com/wannabespace/tamery) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · AGPL-3.0 · Nov 2026</sub>

**Desktop and web database client with an AI SQL assistant and MCP server.**

Tamery is a database client with a table browser, a schema-aware query editor, a schema visualizer and an AI assistant that writes, explains and fixes SQL. It connects to PostgreSQL, MySQL, SQL Server, Oracle, ClickHouse, MongoDB, SQLite and DuckDB, among others. It also runs an MCP server so Claude Code, Cursor and similar agents can query your databases, with writes held for manual approval.

- **+** Supports PostgreSQL, MySQL, SQL Server, Oracle, ClickHouse, MongoDB, SQLite, DuckDB and variants
- **+** MCP server lets coding agents query databases; every write waits for user approval
- **+** Desktop app reaches localhost and private networks; SSH tunnels and SSL supported
- **+** Metadata-only mode keeps connection strings on your machine
- **−** Full AI assistant is part of the paid Pro plan
- **−** Pull requests are not accepted; contributions are limited to issues
- **−** Self-hosting needs pnpm, Bun, Postgres and Redis; the README gives no production guide
- **−** AGPL-3.0 license restricts closed-source network use

<sub>Compose · Needs PostgreSQL, Redis, pnpm, Bun, Docker (optional) · [Repo](https://github.com/wannabespace/tamery) · [🌐 Site ↗](https://tamery.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tamery/)</sub>

<a name="mcp-searxng"></a>
### #&#8288;105 [mcp-searxng](https://github.com/ihor-sokoliuk/mcp-searxng) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

**MCP server giving AI assistants web search and URL reading through SearXNG.**

An MCP server that connects clients such as Claude Desktop and Cursor to an existing SearXNG instance with JSON search enabled. It exposes four tools: web search, search suggestions, instance info and URL reading (HTML, text and bounded PDF). It runs over local STDIO by default, or Streamable HTTP with static bearer or optional OAuth protection.

- **+** Needs no search-vendor API key, only a SearXNG base URL in SEARXNG_URL
- **+** URL reader handles HTML, structured text and bounded PDF, with heading inspection
- **+** Optional replica failover, caching, proxies and FlareSolverr or Byparr solvers
- **+** Ships on npm and Docker, with STDIO and Streamable HTTP transports
- **−** Does not install SearXNG; you must run or trust an instance with JSON enabled
- **−** Public instances may log queries; privacy depends on the SearXNG deployment
- **−** HTML fallback parsing is approximate and returns limited metadata
- **−** npm and npx installs require Node.js 22 or later

<sub>no GPU · Docker + Compose · Needs SearXNG instance with JSON output enabled, Node.js 22+ (npm/npx installs) · [Repo](https://github.com/ihor-sokoliuk/mcp-searxng) · [📖 Docs ↗](https://github.com/ihor-sokoliuk/mcp-searxng/blob/main/docs/index.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-searxng/)</sub>

<a name="agentdock"></a>
### #&#8288;106 [uvwt/agentdock](https://github.com/uvwt/agentdock) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Nov 2026</sub>

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

<a name="mcpc"></a>
### #&#8288;107 [mcpc](https://github.com/apify/mcpc) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Command-line client that maps MCP operations to shell commands.**

mcpc is a TypeScript CLI for the Model Context Protocol. It connects to remote (Streamable HTTP) or local stdio servers, keeps named sessions alive through a background bridge process, and exposes tools, prompts, resources, tasks and skills as subcommands. It prints text or spec-consistent JSON, so it works for debugging servers, shell scripting, or as a single Bash tool for AI agents.

- **+** Covers tools, prompts, resources, async tasks and skills over stdio and Streamable HTTP
- **+** Persistent named sessions work with both stateful and stateless (2026-07-28) servers
- **+** OAuth 2.1 with credentials in the OS keychain, file fallback on headless Linux
- **+** `grep` searches tools across sessions, so agents load only the tools they need
- **−** Requires Node.js or Bun unless installed through Homebrew
- **−** x402 agentic payments support is marked experimental
- **−** It is a client only; it does not provide MCP servers or tools itself
- **−** Bulk auto-discovery skips config entries that reference environment variables

<sub>no GPU · Needs Node.js or Bun, OS keychain (Secret Service on Linux, optional) · [Repo](https://github.com/apify/mcpc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcpc/)</sub>

<a name="codeseek"></a>
### #&#8288;108 [codeseek](https://github.com/codebendkit/codeseek) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 765 · MIT · Nov 2026</sub>

**Call-graph and hybrid semantic code search CLI that registers as MCP tools.**

CodeSeek is a Rust CLI that parses source with Tree-sitter (7 languages), builds a call graph, and indexes functions in LanceDB and Tantivy BM25. Search fuses dense and sparse results with RRF and optionally reranks them. `codeseek install` registers it as MCP tools in Claude Code and Codex; there is no daemon or HTTP server.

- **+** Call graph queries (callers, callees, bidirectional depth) work offline from a serialized graph
- **+** Hybrid pipeline: LanceDB vectors, Tantivy BM25, RRF fusion, Qwen3 reranker
- **+** Incremental MD5 re-indexing, plus git post-commit/post-merge hooks
- **+** Reports reproducible evals: MTEB(Code) nDCG@10 0.9182, RepoQA 84.0%
- **−** Semantic search needs an external embedding API; the example config uses SiliconFlow
- **−** Prebuilt binaries only for macOS (arm64, x64) and Linux x64; no Windows
- **−** Covers 7 languages only: Rust, Python, JS, TS, Go, C/C++, Java
- **−** Without embedding or reranker access it falls back to symbol-name matching

<sub>no GPU · Needs OpenAI-compatible embedding API, Reranker API (optional), protoc (source build), Node.js/npm (wrapper install) · Models: Qwen/Qwen3-Embedding-4B, Qwen/Qwen3-Reranker-4B · [Repo](https://github.com/codebendkit/codeseek) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeseek/)</sub>

<a name="ix"></a>
### #&#8288;109 [ix](https://github.com/ix-infrastructure/ix) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**Local code graph of symbols and calls, queryable by CLI and MCP.**

Ix parses a repository with tree-sitter into a graph of symbols, calls and imports, stored locally in ArangoDB. You query it with the `ix` CLI (explain, trace, impact, callers, rank) or through a stdio MCP server that `ix mcp install` registers with Claude Code, Codex, Cursor, VS Code, Gemini CLI, OpenClaw and opencode. It also includes a visualizer and an agent skill.

- **+** Covers 27 languages plus config formats like SQL, YAML and Protocol Buffers
- **+** One command registers the MCP server with seven detected clients, with dry-run
- **+** Graph persists locally between sessions; `ix watch` re-maps on change
- **+** Output formats include a token-minimal `llm` mode and `json` for chaining
- **−** Needs Docker to run the ArangoDB backend, which is a released image, not built from this repo
- **−** Token savings of 30-99.7% are internal measurements, not a published benchmark
- **−** No pre-built CLI for Intel Macs; Homebrew builds from source
- **−** Install relies on piping a remote script to sh

<sub>Compose · Needs Docker, Docker Compose, ArangoDB, Node.js 22+, Git, ripgrep · [Repo](https://github.com/ix-infrastructure/ix) · [🌐 Site ↗](https://www.ix-infra.com/ix) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ix/)</sub>

<a name="anymd"></a>
### #&#8288;110 [anymd](https://github.com/sylphxai/anymd) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Rust MCP server and CLI that converts documents and media to Markdown.**

anymd converts PDF, Word, PowerPoint, Excel, EPUB, HTML, URLs, images (OCR) and audio/video (metadata, subtitles, transcripts) to Markdown with page anchors. It runs as a stdio MCP server exposing outline, read, search and inspect tools, and as a CLI. Parsing is native Rust and local; the README's own benchmark reports 96.4 overall on 38 documents in 11.5 s.

- **+** Four MCP tools with page-cited output, token budget and cursor pagination
- **+** Native Rust parsing; no Python, LibreOffice or cloud service needed
- **+** One-command setup configures Claude Code, Cursor, Codex, VS Code and others
- **+** Open benchmark with reproducible harness; converted 38/38 docs in 11.5 s
- **−** cite_check and video timeline/render_frame require paid Pro licence (US$29)
- **−** Benchmarks are self-published; OmniDocBench image OCR score is 21.4
- **−** OCR setup downloads about 2 GB of models; ASR weights need explicit opt-in
- **−** Audio and video features depend on ffmpeg/ffprobe being installed

<sub>GPU optional · Docker · Needs Node 18+ (npx install), ffmpeg/ffprobe (audio, video), tesseract (optional OCR) · Models: Qwen3-ASR (local transcripts), local doc-VLM OCR models · [Repo](https://github.com/sylphxai/anymd) · [📖 Docs ↗](https://sylphxai.github.io/anymd/) · [🌐 Site ↗](https://sylphxai.github.io/anymd/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/anymd/)</sub>

<a name="photoshop-mcp"></a>
### #&#8288;111 [photoshop-mcp](https://github.com/alisaitteke/photoshop-mcp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 972 · MIT · Nov 2026</sub>

**MCP server that drives Adobe Photoshop with 128 tools and a built-in chat UI.**

Exposes 128 Photoshop tools (111 atomic, 17 one-step recipes) over MCP, so Cursor, Claude Code, Claude Desktop or VS Code can edit open documents. Recipes cover background removal, portrait retouching, web/social export, carousel splitting and batch watermarking, each landing as one undo step. It also ships a browser chat UI launched with npx, and an opt-in Jev router that runs simple commands without an LLM call.

- **+** Installs with a single npx command; no build step needed
- **+** Multi-step recipes are a single undo step in Photoshop
- **+** Standalone chat UI can reuse a Claude Code or Gemini CLI login
- **+** Works on Windows and macOS with Photoshop versions from 2012 onward
- **−** Requires a running Photoshop install, which is commercial Adobe software
- **−** No Linux support; platforms are Windows and macOS only
- **−** Anonymous usage analytics are on by default and must be disabled
- **−** Jev routing and Action Plan are experimental or beta; Jev sends prompts to api.typesafe.ai

<sub>Needs Adobe Photoshop (Windows or macOS), Node.js 18+ · Models: Claude Code account, Gemini CLI account, AI provider API keys, Jev (TypeSafe AI, opt-in) · [Repo](https://github.com/alisaitteke/photoshop-mcp) · [🌐 Site ↗](https://photoshop-mcp.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/photoshop-mcp/)</sub>

<a name="mcp-nixos"></a>
### #&#8288;112 [mcp-nixos](https://github.com/utensils/mcp-nixos) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 892 · MIT · Nov 2026</sub>

**MCP server that looks up NixOS packages, options and Nix docs.**

Exposes two MCP tools, `nix` and `nix_versions`, that query search.nixos.org, Home Manager, nix-darwin, Nixvim, NVF, FlakeHub, Noogle, the NixOS Wiki, nix.dev and NixHub. It also reports binary cache status and historical package versions with nixpkgs commit hashes. Runs over stdio by default or HTTP at `/mcp`, and does not require Nix to be installed.

- **+** Only two tools, about 1,030 tokens of context
- **+** Runs with `uvx mcp-nixos`; Nix not required
- **+** Covers many sources: nixpkgs, Home Manager, darwin, Nixvim, NVF, Noogle, wiki
- **+** Supports stdio and HTTP transports; packaged in nixpkgs and as a flake
- **−** Depends on live third-party web services for most queries
- **−** Local flake-input and store actions require Nix installed
- **−** HTTP mode has no documented auth; configuration is limited to env vars
- **−** Single-purpose: only useful for Nix ecosystem questions

<sub>no GPU · Needs Python 3.11+, uvx or pip, search.nixos.org, NixHub.io, FlakeHub, noogle.dev, Nix (optional, for local flake inputs and store) · port 8000 · [Repo](https://github.com/utensils/mcp-nixos) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-nixos/)</sub>

<a name="yahoo-finance2"></a>
### #&#8288;113 [yahoo-finance2](https://github.com/gadicc/yahoo-finance2) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 817 · MIT · Nov 2026</sub>

**Unofficial Yahoo Finance client for Node, Bun, Deno and Cloudflare, with CLI and MCP.**

TypeScript library that queries Yahoo Finance for quotes, charts, historical data, options, screeners, search and the many quoteSummary modules. It also ships a CLI (npx yahoo-finance2), MCP tools for clients such as Codex, Claude, Cursor and VS Code, and an Agent Skill. It relies on an unofficial Yahoo endpoint with no availability or consistency guarantee.

- **+** Typed API with many modules: quote, chart, options, screener, fundamentalsTimeSeries, quoteSummary submodules
- **+** Runs on Node 22+, Bun 1+, Deno 2+ and Cloudflare Workers
- **+** Includes CLI, MCP docs and an installable Agent Skill (npx skills add)
- **+** MIT licensed, with CI tests and semantic-release versioning
- **−** Unofficial; Yahoo makes no guarantees on availability or API consistency
- **−** Cannot run in the browser due to CORS and cookie issues; needs a server
- **−** Delisted stocks lose all Yahoo data, including earlier historical and chart data
- **−** Finance data client, not a developer-tooling MCP server; the MCP is a side feature

<sub>no GPU · Needs Yahoo Finance (unofficial endpoints), Node 22+, Bun 1+, Deno 2+ or Cloudflare Workers · [Repo](https://github.com/gadicc/yahoo-finance2) · [▶️ Demo ↗](https://codesandbox.io/p/devbox/gxvftx) · [📖 Docs ↗](https://jsr.io/@gadicc/yahoo-finance2/doc/~/default) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yahoo-finance2/)</sub>

<a name="cli-anything"></a>
### #&#8288;114 [cli-anything](https://github.com/hkuds/cli-anything) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · Apache-2.0 · Sep 2026</sub>

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

<a name="mcp-unity"></a>
### #&#8288;115 [mcp-unity](https://github.com/codergamester/mcp-unity) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="kanzo"></a>
### #&#8288;116 [kanzo](https://github.com/emanuele-em/kanzo) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · AGPL-3.0 · Nov 2026</sub>

**Kanban board and MCP server that coding agents and you share.**

Kanzo is a single Rust binary that serves a kanban board in the browser and an MCP server for coding agents such as Claude Code and Codex. Agents take tasks, move cards and comment, while you use the web UI or the `kanzo` CLI. Data lives in SQLite under `~/kanzo`, and a board can be shared live over a network or synced between machines through a git repo.

- **+** Single 4.7 MB binary with SQLite included; no account or server setup
- **+** Task dependencies via waits_on; next_task skips blocked tasks
- **+** Live board sharing between computers, plus git-based sync
- **+** GitHub-style filter syntax shared by the UI and the MCP tools
- **−** Sharing has no logins; only safe on a trusted network or VPN
- **−** AGPL-3.0 requires sharing source of modified versions offered over a network
- **−** No Docker or compose files in the repo
- **−** Board UI languages are limited to English and Chinese

<sub>no GPU · port 4242 · [Repo](https://github.com/emanuele-em/kanzo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kanzo/)</sub>

<a name="awwwards-mcp"></a>
### #&#8288;117 [awwwards-mcp](https://github.com/insane0777/awwwards-mcp) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 958 · MIT · Nov 2026</sub>

**MCP server for Awwwards search and design analysis of any live site.**

TypeScript MCP server that searches Awwwards sites by color, tag, technology or award through a local FTS5/BM25 index and returns screenshots and design details. It also runs Playwright-based captures on any URL: band maps, scroll and hover motion censuses, bundle analysis and accessibility evidence. Agents can rebuild a page, convert it to a Vite, Astro or Next.js project, and score the build against the original with verify_build.

- **+** Analysis tools (band map, motion, hover, bundles) work on any URL, not only Awwwards sites
- **+** Closes the loop: build_project exports Vite, Astro or Next.js, and verify_build scores the result
- **+** Search runs on a local FTS5 index with BM25 ranking and 7-day caches for several tools
- **+** Most tools return evidence rather than grades, and unknowns are reported explicitly
- **−** Capture, motion and verify tools need Playwright; record_site_motion also needs ffmpeg-static
- **−** Several tools are limited to personal, non-commercial use
- **−** Requests are rate-limited (e.g. 1 request/second), so batch hydration is slow
- **−** The README states shortlist_references adoption is unproven

<sub>no GPU · Needs Playwright, ffmpeg-static, Chrome or Edge (audit_url), webcrack (optional) · [Repo](https://github.com/insane0777/awwwards-mcp) · [🌐 Site ↗](https://awwwards-mcp.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awwwards-mcp/)</sub>

<a name="computer-use-linux"></a>
### #&#8288;118 [computer-use-linux](https://github.com/agent-sh/computer-use-linux) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 949 · MIT · Nov 2026</sub>

**Rust MCP server and CLI for controlling a Linux desktop from AI agents.**

Exposes a local Linux desktop to MCP clients and a CLI: AT-SPI accessibility trees, bounded screenshots, window listing and focus, and Wayland/X11 input (click, drag, scroll, type). Window targeting tries backends for GNOME, KDE, Hyprland, niri, COSMIC, i3, Sway, labwc and X11/EWMH. Mutating tools can return a post-action screenshot and fresh tree in one call, and a `doctor` command reports readiness as JSON.

- **+** Covers many compositors: GNOME, KDE, Hyprland, niri, COSMIC, i3, Sway, labwc, X11
- **+** Semantic AT-SPI selectors and element indexes, with pixel coordinates as fallback
- **+** Post-action screenshot and tree returned in the same tool call
- **+** Installs via Claude Code/Codex plugins, Pi, npm, cargo or prebuilt x86_64/aarch64 binaries
- **−** Acts on the real desktop, mouse and focus; isolation needs the separate agent-workspace-linux
- **−** Wayland input needs /dev/uinput or the RemoteDesktop portal; coordinate actions are otherwise refused
- **−** GNOME Wayland needs a bundled Shell extension for exact window activation and move/resize
- **−** X11 text via xdotool can substitute symbols under non-US keyboard layouts

<sub>no GPU · Needs AT-SPI, /dev/uinput or xdg-desktop-portal RemoteDesktop, xdotool (X11), wtype or ydotool (Wayland text), glibc 2.28+ · [Repo](https://github.com/agent-sh/computer-use-linux) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/computer-use-linux/)</sub>

<a name="ghidramcp"></a>
### #&#8288;119 [ghidramcp](https://github.com/lauriewired/ghidramcp) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: patchy (34) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

**MCP server and Ghidra plugin for LLM-driven reverse engineering.**

A Ghidra extension that runs an HTTP server inside Ghidra, plus a Python MCP server (ghidra-mcp) that forwards MCP tool calls to it. MCP clients can decompile binaries, list methods, classes, imports and exports, and rename methods and data. A headless mode uses PyGhidra to analyze a binary without the Ghidra GUI.

- **+** Works with any MCP client; stdio and streamable-http transports are both supported
- **+** Headless mode analyzes a binary through PyGhidra with no Ghidra GUI running
- **+** Install is a Ghidra extension zip plus a one-line uvx command
- **+** Ghidra host and port are configurable, so it can target a remote instance
- **−** Pinned to Ghidra 12.1.4; other versions are not listed as supported
- **−** Headless mode needs Python 3.10-3.13 and GHIDRA_INSTALL_DIR set
- **−** On macOS, headless mode requires building Ghidra's decompiler natives first
- **−** README describes only a few tool groups and has no full tool reference

<sub>no GPU · Needs Ghidra 12.1.4, uv or Python 3.10+, Java 21 (build from source), PyGhidra (headless mode) · Models: Any MCP client · port 8080 · [Repo](https://github.com/lauriewired/ghidramcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ghidramcp/)</sub>

<a name="serve-sim"></a>
### #&#8288;120 [serve-sim](https://github.com/evanbacon/serve-sim) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

**Streams and controls iOS Simulators from a browser for agent tools.**

serve-sim runs a Swift helper that captures a booted iOS, iPad or Watch simulator's framebuffer and serves it as an H.264 or MJPEG stream with a WebSocket control channel and React preview UI on port 3200. Its CLI sends gestures, text, recordings, accessibility dumps and camera feeds, so agent tools can drive the simulator locally, over a LAN or through a tunnel.

- **+** CLI covers taps by accessibility ref, typing, paste, recording and frame diffs for scripts and agents
- **+** Injects a synthetic camera feed (placeholder, file or webcam) into a chosen app without changing it
- **+** Remote access requires a token; host shell and .ipa install stay off unless --allow-exec is set
- **+** Starts with npx; no Xcode plugin or app instrumentation required
- **−** macOS on Apple Silicon only; the bundled helper does not run on Intel Macs
- **−** Xcode 27 keyboard input needs Device Hub frontmost and Accessibility permission
- **−** iPhone Duo support relies on private beta APIs and needs rechecking after SDK updates
- **−** With --allow-exec, a raw ssh -R or socat forward lets anyone reaching the port install apps

<sub>Needs macOS (Apple Silicon), Xcode command line tools (xcrun simctl), Node.js 20+ · port 3200 · [Repo](https://github.com/evanbacon/serve-sim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serve-sim/)</sub>

<a name="codexpro"></a>
### #&#8288;121 [codexpro](https://github.com/rebel0789/codexpro) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

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

<a name="openserp"></a>
### #&#8288;122 [openserp](https://github.com/karust/openserp) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**Self-hosted web search API and MCP server over Google, Bing and other engines.**

OpenSERP loads search results for Google, Bing, Yandex, Baidu, DuckDuckGo and Ecosia in Chromium and returns them as one JSON schema with source engine and rank. It exposes a REST API and a CLI, can attach page content as Markdown to the top results, and ships an MCP server plus JS and Python SDKs. No API keys are needed; you supply compute and proxies.

- **+** Six engines share one JSON schema; engine and rank survive multi-engine merge
- **+** extract=N attaches Markdown of top results; /extract/batch reads up to 20 URLs
- **+** Single Go binary or Docker image, with proxies, cache, retries and rate limits
- **+** Ready integrations: MCP for Claude Code and Cursor, Open WebUI provider, n8n node
- **−** Scrapes search pages with a browser, so engine layout changes or blocks can break results
- **−** Raw HTTP mode covers only Google, Yandex, Baidu and Ecosia
- **−** MCP server needs Node.js 18+ and a separately running OpenSERP server
- **−** Reliable Google scraping at volume likely needs your own proxies

<sub>no GPU · Docker + Compose · Needs Chromium, Node.js 18+ (MCP server), HTTP/SOCKS5 proxies (optional) · port 7000 · [Repo](https://github.com/karust/openserp) · [📖 Docs ↗](https://github.com/karust/openserp/blob/main/docs/openapi.yaml) · [🌐 Site ↗](https://openserp.org/cloud/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openserp/)</sub>

<a name="token-savior"></a>
### #&#8288;123 [token-savior](https://github.com/mibayy/token-savior) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Oct 2026</sub>

**MCP server for symbol-level code navigation, persistent memory and Bash output trimming.**

Token Savior is a Python MCP server that indexes a codebase by symbol (functions, classes, imports, call graph) so agents fetch pointers instead of whole files. It adds a SQLite WAL + FTS5 memory store re-injected across sessions, plus opt-in Bash hooks: 34 PostToolUse output compactors and a 10-rule PreToolUse command rewriter. The README's 97.9% tsbench score is self-reported and unverifiable; a later 8-task re-measure showed -45% cost.

- **+** Symbol index with call graph and structural editing that keeps the index in sync
- **+** Persistent memory in SQLite WAL + FTS5, optional vector search, re-injected next session
- **+** `ts init` merges hooks for Claude, Cursor, Gemini, Codex and OpenClaw with diff and backup
- **+** README openly withdraws a flawed benchmark and reports a re-measure with tool-use checks
- **−** Headline tsbench 97.9% cannot be reproduced; benchmark repo is not public
- **−** Re-measure on 8 tasks: -45% cost but +40% wall time from indexing
- **−** PostToolUse compactors do not shrink the current turn; only the rewriter does
- **−** Needs `alwaysLoad` on Claude Code, otherwise the model rarely calls its tools

<sub>no GPU · Needs Python 3.11+, SQLite, MCP-compatible client · [Repo](https://github.com/mibayy/token-savior) · [🌐 Site ↗](https://mibayy.github.io/token-savior/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/token-savior/)</sub>

<a name="ida-mcp-rs"></a>
### #&#8288;124 [ida-mcp-rs](https://github.com/blacktop/ida-mcp-rs) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 913 · MIT · Nov 2026</sub>

**Headless IDA Pro MCP server for reverse engineering with AI agents.**

A Rust MCP server that drives IDA Pro through idalib. It exposes tools for opening binaries, decompiling, xrefs, renaming, typing, patching and IDAPython scripting over stdio or HTTP. It has explicit support for universal Mach-O slice selection, dSYM/DWARF loading and dyld_shared_cache modules. It requires a licensed IDA Pro 9.5 install, with version-matched releases for older IDA.

- **+** Single-call tools for fat Mach-O slices, dSYM/DWARF and dyld_shared_cache loading
- **+** Exact-target edits, save_idb checkpoints and automatic replacement of crashed IDA workers
- **+** run_script keeps IDAPython state between calls and returns a trailing expression as JSON
- **+** 28-tool lean profile cost 25% less than the full set in the project's own benchmark
- **−** Needs a separately licensed IDA Pro 9.5; IDA is not included
- **−** Releases are pinned to IDA versions; a mismatch makes IDA-backed tools fail
- **−** Unsaved edits are lost on SDK crash, timeout or SIGKILL
- **−** Pseudocode tools need a Hex-Rays decompiler for the target processor

<sub>no GPU · Needs IDA Pro 9.5, Hex-Rays decompiler (for pseudocode tools), IDAPython (for run_script) · Models: Claude Code, Codex CLI, Gemini CLI, Cursor · [Repo](https://github.com/blacktop/ida-mcp-rs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ida-mcp-rs/)</sub>

<a name="reddit-mcp-buddy"></a>
### #&#8288;125 [reddit-mcp-buddy](https://github.com/karanb192/reddit-mcp-buddy) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 912 · MIT · Nov 2026</sub>

**MCP server for browsing and searching Reddit from AI assistants.**

TypeScript MCP server that exposes Reddit browsing, search, post and comment retrieval, user analysis and subreddit lookup as tools over stdio. It requires credentials for an already-approved Reddit API app, and optional posting tools can be enabled with REDDIT_BUDDY_WRITE. Reddit is closing public API access in stages through March 2027, so new users cannot get credentials.

- **+** Six read tools plus opt-in posting tools that stay hidden by default
- **+** Supports app-only, password-grant and refresh-token OAuth (--oauth flow)
- **+** NSFW filtering set per call or server-wide via REDDIT_BUDDY_NSFW
- **+** Installs via npx, a Claude Desktop .mcpb extension, or Docker
- **−** New users cannot use it: Reddit stopped issuing API access on 2026-10-31
- **−** Credential-free RSS fallback ends 2026-11-13; then every Reddit tool needs credentials
- **−** Access closes for unregistered apps from 2027-01-12, fully by March 2027
- **−** Write tools work over stdio only; the HTTP transport refuses to register them

<sub>no GPU · Docker · Needs Reddit API credentials (approved app), Node.js / npx · [Repo](https://github.com/karanb192/reddit-mcp-buddy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reddit-mcp-buddy/)</sub>

<a name="coolify-mcp"></a>
### #&#8288;126 [coolify-mcp](https://github.com/stumason/coolify-mcp) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 631 · MIT · Nov 2026</sub>

**MCP server for managing a self-hosted Coolify instance from AI clients.**

TypeScript MCP server that exposes 46 tools for Coolify v4 (v4.0 to v4.3): deploying, diagnosing, configuring and deleting apps, databases and services. It runs over stdio via npx or as an HTTP container with OAuth 2.1, and supports several Coolify instances. Destructive calls ask for human confirmation on clients that support elicitation, and secrets are masked.

- **+** Human confirmation on destructive calls, failing closed in HTTP mode
- **+** Doctor command checks config, reachability, token and Coolify version with fixes
- **+** Stdio and HTTP transports, plus one-click Claude Desktop .mcpb install
- **+** Multi-instance fleet mode; secrets masked and logs wrapped as untrusted data
- **−** Only useful with a Coolify v4 instance; tested range is v4.0 to v4.3
- **−** Local mode without elicitation relies on a confirm flag the model sets itself
- **−** Tool list costs about 8,900 tokens of context
- **−** Coolify now ships a built-in MCP server, which covers read-only use

<sub>no GPU · Docker · Needs Coolify v4 instance, Coolify API token, Node.js (npx) · [Repo](https://github.com/stumason/coolify-mcp) · [📖 Docs ↗](https://coolify-mcp.stumason.dev) · [🌐 Site ↗](https://coolify-mcp.stumason.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coolify-mcp/)</sub>

<a name="code2prompt"></a>
### #&#8288;127 [code2prompt](https://github.com/mufeedvh/code2prompt) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (75) · Freshness: active (86) · Maintenance: patchy (41) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

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

<a name="magic-mcp"></a>
### #&#8288;128 [magic-mcp](https://github.com/21st-dev/magic-mcp) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · ISC · Sep 2026</sub>

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

<a name="git-sim"></a>
### #&#8288;129 [git-sim](https://github.com/initialcommit-com/git-sim) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · GPL-2.0 · Oct 2026</sub>

**Simulate and visualize Git commands as shareable graphs before running them.**

git-sim is a Python CLI that takes a Git command (merge, rebase, reset and others), draws its effect on your repo as an interactive graph, and leaves the repo unchanged. It also has a live mode that records real Git operations, a preflight risk check, a VS Code extension, a Jupyter magic, a GitHub Action for PRs, and an MCP server and hook for AI agents.

- **+** Simulates commands without touching the repo; prefix git commands with git-sim
- **+** Preflight reports risk, lost commits and the undo command; wires into Claude Code, Cursor, Codex, Gemini CLI
- **+** Graph data sits in the URL fragment, so it is not sent to the server; --open-in local works offline
- **+** Output as link, embed, HTML, PNG, SVG or MP4; also VS Code, Jupyter and GitHub Action
- **−** Default viewer is hosted at initialcommit.com unless --open-in local is set
- **−** Public share links store graph data on initialcommit.com servers
- **−** Animated video output needs Manim; minimal Linux needs libEGL, libGL and fontconfig
- **−** GPL-2.0 license may limit embedding in proprietary software

<sub>no GPU · Docker · Needs Python 3.10-3.14, Git, Manim (for --animate), libEGL, libGL, fontconfig (Linux) · [Repo](https://github.com/initialcommit-com/git-sim) · [▶️ Demo ↗](https://initialcommit.com/tools/git-sim/viewer?demo=rebase) · [🌐 Site ↗](https://initialcommit.com/tools/git-sim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/git-sim/)</sub>

<a name="mcp2cli"></a>
### #&#8288;130 [mcp2cli](https://github.com/knowsuchagency/mcp2cli) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Nov 2026</sub>

**CLI that exposes MCP servers, OpenAPI specs and GraphQL endpoints as commands.**

mcp2cli builds a command-line interface at runtime from an MCP server (HTTP/SSE or stdio), an OpenAPI spec, or a GraphQL endpoint, with no code generation. Its compact `--list` output and usage-based ranking cut the tokens an agent spends on tool schemas. It also handles OAuth, named sessions that reuse one MCP connection, and saved "baked" configurations.

- **+** One tool covers MCP (HTTP/SSE, stdio), OpenAPI (JSON/YAML) and GraphQL sources
- **+** OAuth with PKCE, client credentials and a manual-callback mode for headless hosts
- **+** Persistent sessions keep one MCP connection alive across calls
- **+** Secrets can be read from env: or file: references instead of CLI arguments
- **−** Only MCP sources support `--schema`; `--spec` and `--graphql` reject it
- **−** Spec and tool-list caching has a 1-hour default TTL, so stale lists need `--refresh`
- **−** No tagged release published
- **−** Token-saving figures come from the project's own writeup, not the README itself

<sub>no GPU · Needs uv, mcp Python SDK (>=1.26,<3) · [Repo](https://github.com/knowsuchagency/mcp2cli) · [🌐 Site ↗](https://www.orangecountyai.com/blog/mcp2cli-one-cli-for-every-api-zero-wasted-tokens) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp2cli/)</sub>

<a name="ida-mcp"></a>
### #&#8288;131 [ida-mcp](https://github.com/hexrayssa/ida-mcp) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Oct 2026</sub>

**Official Hex-Rays MCP server for reverse engineering binaries in IDA.**

Exposes IDA databases to MCP-capable agents over stdio or Streamable HTTP, so an agent can be asked to reverse a binary. It runs headless through idalib, or opens files in the IDA GUI when the companion plugin is installed. Built on IDA Nexus, which lets several clients share the same database. Installation is automated through hcli, with plugins for Claude Code, Codex CLI, Copilot CLI, Pi and oh-my-pi.

- **+** Official Hex-Rays project, MIT licensed, with a PyPI release installable via uvx
- **+** Works headless via idalib or against an open IDA GUI session
- **+** Ready-made plugins for Claude Code, Codex CLI, Copilot CLI, Pi and oh-my-pi
- **+** Supports stdio and Streamable HTTP, plus a session dashboard and log export
- **−** Requires IDA 9.4 or higher with idalib, which is commercial software
- **−** Other IDA MCP servers should be disabled to avoid confusing agents
- **−** Needs Git, uv and Python 3.11+ on PATH

<sub>no GPU · Needs IDA 9.4+ with idalib, Python 3.11+, uv, Git, hcli (optional) · port 8737 · [Repo](https://github.com/hexrayssa/ida-mcp) · [📖 Docs ↗](https://hcli.docs.hex-rays.com/) · [🌐 Site ↗](https://hex-rays.com/blog/hex-rays-ida-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ida-mcp/)</sub>

<a name="coding-tools-mcp"></a>
### #&#8288;132 [coding-tools-mcp](https://github.com/xytom/coding-tools-mcp) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Oct 2026</sub>

**MCP server giving chat clients and agents sandboxed file, patch, exec and git tools.**

Python MCP server that exposes 18 tools (19 in dangerous mode) for reading and searching files, atomic multi-file patches, PTY-backed command execution, and git inspection, confined to one workspace root. Runs over stdio or Streamable HTTP on port 8765 and works with Claude Desktop, Claude Code, Codex, Cursor, Cline, VS Code, Windsurf and Gemini CLI. Permission modes (safe, trusted, dangerous) gate network, shell expansion and destructive commands.

- **+** Rejects absolute paths, .. traversal and symlink escapes; Landlock confinement on Linux
- **+** Three permission modes, with safe as the default
- **+** Runs via uvx or npx; works over stdio or Streamable HTTP
- **+** Bearer and OAuth 2.1 with PKCE built in for remote tunnel access
- **−** Not a complete OS sandbox; README says to use Docker or a VM for untrusted code
- **−** Landlock confinement is Linux only; other platforms get a warning
- **−** Anonymous telemetry is on by default and must be disabled by env var
- **−** npm package is only a launcher and still needs Python 3.11+ with uv or pipx

<sub>no GPU · Docker + Compose · Needs Python >= 3.11, uv or pipx (for the npm launcher), Docker (optional sandbox), cloudflared, ngrok or Dev Tunnel (optional remote access) · Models: Any MCP client (model-neutral) · port 8765 · [Repo](https://github.com/xytom/coding-tools-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coding-tools-mcp/)</sub>

<a name="jadx-ai-mcp"></a>
### #&#8288;133 [jadx-ai-mcp](https://github.com/zinja-coder/jadx-ai-mcp) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="oc"></a>
### #&#8288;134 [oc](https://github.com/only-cli/oc) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 698 · MIT · Nov 2026</sub>

**CLI that renders web pages as compact numbered text for coding agents.**

only-cli (`oc`) is a Node CLI that fetches a URL and prints a numbered, token-budgeted view (default 500 tokens) instead of raw HTML. Agents follow links with `oc do <n>` and read more with `find`, `read` and `next`. Requests impersonate Chrome, then Firefox, then native fetch, and about 40 site shortcuts cover docs, package registries, forums and code hosts. It also ships an agent skill and a Claude Code plugin.

- **+** Token-budgeted numbered output with find, read and next, so pages are not refetched
- **+** About 40 site shortcuts (GitHub, npm, PyPI, MDN, Hacker News) plus JSON API rendering
- **+** Browser-fingerprint impersonation with Chrome, Firefox, fetch fallback; no daemon or extension
- **+** Cookie sessions stored owner-only, HTTP(S) proxy and NO_PROXY support
- **−** Pages that render only with JavaScript are not supported; exits 2 on empty renders
- **−** Sites with hard bot challenges and no feed stay unreachable
- **−** Form commands `fill` and `submit` are listed as planned
- **−** `oc` name collides with the OpenShift CLI; needs npx or an alias

<sub>no GPU · Needs Node.js 20+, impers (libcurl-impersonate) · [Repo](https://github.com/only-cli/oc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oc/)</sub>

<a name="flocon"></a>
### #&#8288;135 [flocon](https://github.com/openflocon/flocon) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 391 · MIT · Nov 2026</sub>

**Desktop debugger for Android, iOS and Flutter apps with a built-in MCP server.**

Flocon is a desktop app that connects to a running mobile app through small SDKs for Android, Kotlin Multiplatform, iOS/macOS (Swift) and Flutter. It shows network calls (HTTP, GraphQL, gRPC), databases, preferences, analytics events, crashes and a timeline. It also exposes an MCP server at localhost:9042/mcp so agents such as Claude Code, Codex, Cursor and Gemini CLI can read that data, mock calls, simulate a slow network and open deeplinks.

- **+** One desktop app serves Android, KMP, iOS/macOS and Flutter SDKs through the same API
- **+** Agents can mock calls, throttle the network, open deeplinks and take screenshots
- **+** Network inspector covers HTTP, GraphQL and gRPC, with mocking and slowdown
- **+** Installers for macOS (Homebrew), Linux (.deb, .rpm) and Windows (.msi); MIT licensed
- **−** Requires adding an SDK dependency to each app you want to inspect
- **−** Screenshots, recordings and deeplinks need adb, so they are Android-oriented
- **−** Portable jar needs JDK 21; Swift SDK needs Xcode 16+ and iOS 15
- **−** Flocon 1.x users must follow a migration guide

<sub>no GPU · Needs JDK 21 (portable jar), adb (Android screenshots, recordings, deeplinks), Xcode 16+ (Swift SDK), Flutter 3.38.1+ (Flutter SDK) · port 9042 · [Repo](https://github.com/openflocon/flocon) · [📖 Docs ↗](https://openflocon.github.io/Flocon/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flocon/)</sub>

<a name="mcp-gsc"></a>
### #&#8288;136 [mcp-gsc](https://github.com/aminforou/mcp-gsc) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (44) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Nov 2026</sub>

**MCP server exposing Google Search Console analytics, indexing and sitemaps to AI clients.**

A Python MCP server that wraps the Google Search Console API as 20 tools: search analytics with country, device, query and page filters, period comparison, URL inspection, and sitemap management. It runs over stdio via uvx or a clone, authenticating with an OAuth desktop client or a service account. Add and delete site and delete sitemap tools stay disabled unless GSC_ALLOW_DESTRUCTIVE is set to true.

- **+** Installs with uvx; no clone or virtualenv needed
- **+** Read-only OAuth scope by default; write tools gated behind GSC_ALLOW_DESTRUCTIVE
- **+** Supports both OAuth and service account credentials
- **+** Optional SSE transport and Dockerfile for remote deployment
- **−** Requires creating a Google Cloud project and OAuth or service account credentials
- **−** Local stdio server; does not work in the claude.ai web interface
- **−** Clone install needs Python 3.11+ and fails silently on older versions
- **−** README promotes a hosted paid version with GA4 and Ads features

<sub>no GPU · Docker · Needs Google Search Console API, Google Cloud project with OAuth client or service account, uv (for uvx install) · port 3001 · [Repo](https://github.com/aminforou/mcp-gsc) · [🌐 Site ↗](https://www.advancedgsc.com/mcp?utm_source=github&utm_medium=readme&utm_campaign=mcp-gsc&utm_content=hero-callout) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-gsc/)</sub>

<a name="figma-mcp-bridge"></a>
### #&#8288;137 [figma-mcp-bridge](https://github.com/gethopp/figma-mcp-bridge) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 958 · MIT · Nov 2026</sub>

**Figma plugin and MCP server that reads and edits live Figma files locally.**

A Figma development plugin paired with an MCP server that talks to it over WebSocket, so AI tools can read document trees, styles, variables, prototype flows and screenshots without calling the Figma REST API. It also has write tools for creating and editing frames, text, fills, auto-layout and FigJam objects, plus an opt-in run_script tool. Several open files can be targeted by fileKey.

- **+** Avoids Figma API rate limits, which the README puts at 6 requests per month on free plans
- **+** Runs via npx with no binaries; configured as a standard MCP server entry
- **+** Over 50 tools covering reads, edits, prototype tracing, FigJam and multiple files by fileKey
- **+** run_script is off by default and delete_nodes requires confirm: true
- **−** Needs the Figma desktop app on macOS or Windows; browser Figma cannot import dev plugins
- **−** Plugin must be imported manually from a release manifest and run in each file
- **−** No components or instances, variables or styles authoring, or boolean operations
- **−** Leader HTTP endpoints have no authentication; bound to 127.0.0.1 unless overridden

<sub>no GPU · Needs Figma desktop app, Node.js (npx) · [Repo](https://github.com/gethopp/figma-mcp-bridge) · [▶️ Demo ↗](https://youtu.be/ouygIhFBx0g) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/figma-mcp-bridge/)</sub>

<a name="adobe-premiere-pro-mcp"></a>
### #&#8288;138 [adobe_premiere_pro_mcp](https://github.com/hetpatel-11/adobe_premiere_pro_mcp) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 945 · MIT · Oct 2026</sub>

**MCP server that drives Adobe Premiere Pro through a CEP panel.**

A local Node.js MCP server that exposes 283 catalog tools for editing Premiere Pro projects: ingest, sequences, timeline edits, effects, keyframes, captions, audio and export. The server generates ExtendScript, writes it to a bridge directory, and a CEP panel inside Premiere polls that directory and runs it. Only five tools are advertised by default; the rest are reached through search_tools and invoke_tool.

- **+** 283 tools covering projects, bins, timeline trims, effects, keyframes, audio and exports
- **+** Default tool list is five entries, with search_tools and invoke_tool to save context
- **+** npm CLI with --install-cep and --doctor, plus Claude Code and Codex plugins
- **+** Read-only verify_premiere_connection check before any edit
- **−** Premiere Pro, MCP client and server must all run on the same computer
- **−** UXP bridge is experimental; only the CEP panel is supported for production
- **−** Premiere 26 has no scripting API to remove effects
- **−** import_ae_comps is not advertised because .aep import can wedge the bridge

<sub>no GPU · Needs Adobe Premiere Pro 2020+, Node.js 20+, MCP Bridge (CEP) panel · Models: Any MCP client (Claude Desktop, Claude Code, Codex, GitHub Copilot in VS Code) · [Repo](https://github.com/hetpatel-11/adobe_premiere_pro_mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/adobe-premiere-pro-mcp/)</sub>

<a name="mcp-proxy"></a>
### #&#8288;139 [mcp-proxy](https://github.com/tbxark/mcp-proxy) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 747 · MIT · Nov 2026</sub>

**Go proxy that merges many MCP servers behind one HTTP endpoint.**

MCP Proxy aggregates tools, prompts and resources from several MCP servers and serves them through a single endpoint over SSE or streamable HTTP. Downstream servers can be stdio, SSE or streamable-HTTP clients. The proxy can also hold and refresh OAuth tokens for servers that need interactive authorization, such as Notion.

- **+** Aggregates tools, prompts and resources from many MCP servers into one endpoint
- **+** Accepts stdio, SSE and streamable-HTTP downstream servers
- **+** Holds and refreshes OAuth tokens once for all callers
- **+** Docker image includes npx and uvx; config can be loaded from a remote URL
- **−** Configuration, usage and auth details are in separate docs, not the README
- **−** Does not accept examples for individual third-party MCP services
- **−** No live demo; the only hosted tool is a Claude config converter

<sub>no GPU · Docker + Compose · Needs npx, uvx · port 9090 · [Repo](https://github.com/tbxark/mcp-proxy) · [🌐 Site ↗](https://tbxark.github.io/mcp-proxy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-proxy/)</sub>

<a name="shadcn-ui-mcp-server"></a>
### #&#8288;140 [shadcn-ui-mcp-server](https://github.com/jpisnice/shadcn-ui-mcp-server) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

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

<a name="ok-script"></a>
### #&#8288;141 [ok-script](https://github.com/ok-oldking/ok-script) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 865 · custom license · Nov 2026</sub>

**Python framework and MCP server for agent-written Windows and Android automations.**

ok-script lets a coding agent connect over MCP to a running Windows app, game or Android device, take screenshots, run and reload Python tasks, and read per-run logs. Finished tasks use OpenCV template matching, OCR or YOLO, run locally without the agent, and can be packaged with a desktop GUI into a Windows installer via PyAppify.

- **+** MCP tools cover screenshot, run_task, reload_tasks and get_run_status, with logs under logs/mcp/<run_id>
- **+** Saved tasks run without the agent or any LLM calls
- **+** Same task code targets Windows clients, Android emulators and ADB devices
- **+** Templates are managed as COCO annotations and scale to screen resolution
- **−** Custom license (Apache 2.0 plus Commons Clause) forbids resale and requires attribution links
- **−** Packaged installers and PyAppify flow target Windows only
- **−** Connected agent can execute Python with your account permissions
- **−** OpenCV variant must be chosen and installed separately; Qt, ADB and OCR are optional installs

<sub>Needs Python 3.11+, OpenCV, PySide6, adbutils, OnnxOCR, PyAppify · Models: PaddleOCR v5 via OnnxOCR, YOLO, OpenCV template matching · [Repo](https://github.com/ok-oldking/ok-script) · [🌐 Site ↗](https://ok-script.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ok-script/)</sub>

<a name="cursor-talk-to-figma-mcp"></a>
### #&#8288;142 [cursor-talk-to-figma-mcp](https://github.com/grab/cursor-talk-to-figma-mcp) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (74) · Freshness: active (88) · Maintenance: weak (17) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Jul 2026</sub>

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

<a name="probe"></a>
### #&#8288;143 [probe](https://github.com/probelabs/probe) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 743 · Apache-2.0 · Nov 2026</sub>

**AST-aware code search and extraction engine with MCP server and built-in agent.**

Probe is a Rust CLI that searches codebases with Elasticsearch-style boolean queries ranked by BM25, TF-IDF or hybrid, and returns whole functions or classes parsed with tree-sitter. It needs no index or embedding model. It exposes search, query, extract and symbols as MCP tools, a Node.js SDK and Vercel AI SDK tools. It also ships an agent that works with Anthropic, OpenAI, Google or Bedrock models.

- **+** No indexing or embedding service: search runs immediately and works offline
- **+** Returns complete AST blocks, with --max-tokens budget and session dedup
- **+** Same tools available via CLI, MCP, Node.js SDK and Vercel AI SDK
- **+** Deterministic results; search runs locally without API calls
- **−** No vector search, so queries rely on the LLM to expand vocabulary
- **−** Agent mode needs a provider API key or Claude Code/Codex auth
- **−** Language support limited to the listed tree-sitter grammars
- **−** Comparison claims against other tools come from the project's own README

<sub>no GPU · Docker + Compose · Needs Node.js (npx install path), LLM provider API key for agent mode (optional) · Models: Anthropic, OpenAI, Google, AWS Bedrock · [Repo](https://github.com/probelabs/probe) · [📖 Docs ↗](https://probelabs.com/probe) · [🌐 Site ↗](https://probelabs.com/probe) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/probe/)</sub>

<a name="projectatlas"></a>
### #&#8288;144 [projectatlas](https://github.com/styler-ai/projectatlas) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 514 · MIT · Nov 2026</sub>

**Local repository map and code graph for coding agents, via CLI and MCP.**

ProjectAtlas indexes a repository into a project-local SQLite database holding folder and file purposes, summaries, outlines and symbol relationships. Agents query it through the native Rust `atlas` CLI or an MCP server (Codex, Claude Code, OpenCode) to find where to read before opening source. Each Git worktree keeps its own map, and a Codex plugin adds session and subagent hooks.

- **+** Map stays local in per-checkout SQLite; no source headers or .purpose files required
- **+** Callers, imports, impact analysis, cycles and dead-code candidates, with unresolved references kept visible
- **+** Separate map per Git worktree, addressable by MCP alias, with hooks for subagents
- **+** Prebuilt binaries for Windows x64, Linux x64, macOS Intel and Apple Silicon
- **−** Token savings are historical fixture estimates, not provider-billed session counts
- **−** Optional 150-grammar parser pack is limited to Linux x64 and Windows x64
- **−** ABAP, COBOL, Fortran, Ruby and SQL navigation is only planned for 0.6.0
- **−** Index needs refreshing with `atlas watch` after edits to stay current

<sub>no GPU · Needs SQLite (project-local database) · [Repo](https://github.com/styler-ai/projectatlas) · [📖 Docs ↗](https://styler-ai.github.io/ProjectAtlas/) · [🌐 Site ↗](https://styler-ai.github.io/ProjectAtlas/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/projectatlas/)</sub>

<a name="auryn"></a>
### #&#8288;145 [auryn](https://github.com/falkordb/auryn) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 400 · MIT · Nov 2026</sub>

**MCP server that indexes your repo into a FalkorDB code graph for agents.**

Auryn parses a codebase in 16 languages plus live SQL and Oracle schemas into a graph of functions, types, tables and endpoints, stored in FalkorDB. Coding agents query it over MCP with tools like who_calls, impact_of, find_path and read-only Cypher, and cite file and line. Quickstart runs an embedded FalkorDB with a local viewer, and an installer registers the MCP server with detected agents.

- **+** Caller, impact and path queries return exact edges with file:line citations instead of grep matches
- **+** Incremental resync re-parses only changed files; README claims about 150x faster than full re-ingest on Django
- **+** Cross-language links: HTTP call to endpoint, ORM model to table, gRPC, events
- **+** Embedded FalkorDB quickstart needs no daemon; read tools use only GRAPH.RO_QUERY and no telemetry
- **−** Deep semantic analysis only for Python (Jedi) and C# (Roslyn); other languages are tree-sitter structural
- **−** Embedded database unsupported on native Windows and older-glibc Linux; needs a remote FalkorDB there
- **−** Benchmark figures come from one Django test with Claude Code, published by the project itself
- **−** Requires Python 3.12+; deep C# analysis needs the .NET SDK on PATH

<sub>no GPU · Needs FalkorDB (embedded or remote), Python 3.12+, .NET SDK (optional, deep C#) · port 8080 · [Repo](https://github.com/falkordb/auryn) · [🌐 Site ↗](https://www.falkordb.com/products/codegraph-auryn) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auryn/)</sub>

<a name="blender-ai-mcp-addon"></a>
### #&#8288;146 [blender-ai-mcp-addon](https://github.com/bookwjitchieni1986/blender-ai-mcp-addon) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (37) · Freshness: active (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Blender add-on with AI chat, a built-in MCP server and 21 scene tools.**

A Blender 4.2+ extension that lets an LLM inspect the scene, create and edit objects and materials, take viewport screenshots, search assets and export. It ships a companion Studio chat window, an authenticated Streamable HTTP MCP server for clients such as OpenCode, and an optional manager/worker/reviewer team mode. The release bundle targets Windows x64.

- **+** 21 scene tools covering inspection, creation, editing, screenshots, asset search and export
- **+** Connects OpenAI, Anthropic, Gemini, OpenRouter, OpenCode Zen, Ollama and custom endpoints
- **+** Approvals, cancellation and named undo steps for mutations in built-in chat
- **+** Team chain mode runs tasks sequentially with a review step and one retry
- **−** Release bundle targets Windows x64 only
- **−** execute_code validation is not a security sandbox
- **−** Chat history lasts only for the current session
- **−** External MCP clients handle their own approval policies

<sub>Needs Blender 4.2+, Windows x64, OpenCode (optional), Poly Haven, Sketchfab, Poly Pizza (optional) · Models: OpenAI, Anthropic Claude, Google Gemini, OpenRouter, OpenCode Zen · [Repo](https://github.com/bookwjitchieni1986/blender-ai-mcp-addon) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/blender-ai-mcp-addon/)</sub>

<a name="repobrain"></a>
### #&#8288;147 [repobrain](https://github.com/study8677/repobrain) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

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

<a name="js-reverse-mcp"></a>
### #&#8288;148 [js-reverse-mcp](https://github.com/zhizhuodemao/js-reverse-mcp) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · Apache-2.0 · Sep 2026</sub>

**MCP server for debugging page JavaScript, breakpoints and network from an AI agent.**

JS Reverse MCP exposes 24 tools that let an MCP client list and search page scripts, set breakpoints, step through code, evaluate in paused call frames, and inspect network and WebSocket traffic. Results can be saved to local files for later analysis. It drives Chrome through a maintained Patchright fork, with an optional CloakBrowser binary for sites that fingerprint browsers.

- **+** Breakpoints, stepping and call-frame evaluation, including text-based breakpoints for minified code
- **+** Exports script source and raw request data to files instead of filling chat context
- **+** Persistent login profile by default, with --isolated for a clean profile
- **+** --allowedRoots restricts which local directories the agent can read and write
- **−** Without --allowedRoots, local file access is unrestricted and only a startup warning is printed
- **−** --cloak downloads a ~200MB binary on first launch, silently unless pre-installed
- **−** Network and debugger domains stay inactive until a tool needs them, so first-load capture needs a reload
- **−** README is Chinese-first and carries sponsor advertising

<sub>no GPU · Needs Node.js 20.19+, Google Chrome (stable), Patchright fork (@zhizhuodemao/patchright), CloakBrowser (optional) · [Repo](https://github.com/zhizhuodemao/js-reverse-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/js-reverse-mcp/)</sub>

<a name="nitrostack"></a>
### #&#8288;149 [nitrostack](https://github.com/nitrocloudofficial/nitrostack) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (47) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · Apache-2.0 · Nov 2026</sub>

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

<a name="codanna"></a>
### #&#8288;150 [codanna](https://github.com/bartolli/codanna) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 762 · Apache-2.0 · Nov 2026</sub>

**Local MCP server and CLI for code search, call graphs and impact analysis.**

Codanna indexes a repository on disk under .codanna/ and serves symbol search, semantic search, call graphs, dependency tracking and impact analysis to MCP clients such as Claude Code, Cursor, Codex and Gemini. It runs as a stdio, HTTP or HTTPS server, or as a one-shot CLI (`codanna mcp ...`) for scripts and hooks. It is written in Rust, parses 15 languages, and also indexes markdown docs for RAG.

- **+** One semantic_search_with_context call returns matches with callers, callees and impact radius
- **+** Runs locally; embeddings use a local model, remote embeddings are opt-in
- **+** One-shot CLI works in hooks, scripts and CI without a daemon
- **+** Reports warm-server lookups under 10 ms; benchmark reproduction commands are published
- **−** Prebuilt releases from 0.17.1 do not support Intel Macs
- **−** Linux cargo install needs glibc 2.38+ and libstdc++ from GCC 13+
- **−** Windows support is experimental
- **−** Embedding generation during indexing is slower than parsing and scales with CPU cores

<sub>Needs ONNX Runtime (prebuilt), Rust 1.95+ and pkg-config (build from source only) · Models: Local embedding model (~150MB, downloaded on first use), Remote OpenAI-compatible embeddings (opt-in) · [Repo](https://github.com/bartolli/codanna) · [📖 Docs ↗](https://docs.codanna.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codanna/)</sub>

<a name="mcpjungle"></a>
### #&#8288;151 [mcpjungle](https://github.com/mcpjungle/mcpjungle) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (35) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MPL-2.0 · Nov 2026</sub>

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

<a name="mcp-google-map"></a>
### #&#8288;152 [mcp-google-map](https://github.com/cablate/mcp-google-map) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 505 · MIT · Oct 2026</sub>

**MCP server and CLI exposing 18 read-only Google Maps tools to agents.**

Wraps Google Maps Platform (Places, Routes, Geocoding, weather, air quality, elevation, timezone, static maps) as 18 read-only tools, available over MCP stdio, Streamable HTTP at /mcp, or a stateless `exec` CLI. It also ships three Skills (general map research, travel planning, local SEO) packaged as Codex and Claude Code plugins that call the CLI without an MCP server. Requires Node.js 22+ and your own Google Maps API key.

- **+** Same 18 tools via stdio, HTTP, or CLI; plugins need no MCP setup
- **+** GOOGLE_MAPS_ENABLED_TOOLS allowlist trims the tool list to save context
- **+** Composite tools: route optimization up to 25 stops, area exploration, local rank tracking
- **+** Per-session API key isolation via X-Google-Maps-API-Key header in HTTP mode
- **−** Needs a billing-enabled Google Cloud project; live calls may be billable
- **−** Read-only tools only; no write or booking actions
- **−** Weather availability is limited by region
- **−** Displaying reviews or photos requires you to handle Google attribution and storage rules

<sub>no GPU · Docker · Needs Node.js 22+, Google Maps Platform API key, Places API (New), Routes API, Geocoding API · port 3000 · [Repo](https://github.com/cablate/mcp-google-map) · [📖 Docs ↗](https://github.com/cablate/mcp-google-map/blob/main/skills/google-maps/references/tools-api.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-google-map/)</sub>

<a name="figma-context-mcp"></a>
### #&#8288;153 [figma-context-mcp](https://github.com/glips/figma-context-mcp) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (86) · Freshness: active (83) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Jun 2026</sub>

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

<a name="mysql-mcp-server"></a>
### #&#8288;154 [mysql_mcp_server](https://github.com/designcomputer/mysql_mcp_server) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (31) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

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

<a name="fetcher-mcp"></a>
### #&#8288;155 [fetcher-mcp](https://github.com/jae-jae/fetcher-mcp) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**MCP server that fetches JavaScript-rendered web pages via headless Playwright.**

Fetcher MCP exposes fetch_url, fetch_urls and browser_install tools that load pages in headless Chromium through Playwright and return Markdown, HTML or plain text. It can extract the main content with Readability, block images, stylesheets and fonts, and fetch several URLs in parallel tabs. It runs over stdio by default, or over Streamable HTTP, SSE and a REST API on a configurable port.

- **+** Executes JavaScript, so dynamic pages render before content is extracted
- **+** Readability extraction with Markdown, HTML or plain-text output
- **+** Parallel multi-URL fetching via fetch_urls using multiple tabs
- **+** Supports stdio, Streamable HTTP, SSE and REST, plus a visible-browser debug mode
- **−** HTTP and REST endpoints have no authentication, including browser_install
- **−** Private-IP blocking does not resolve hostnames or recheck redirects
- **−** Needs a separate Playwright Chromium install on first run with npx
- **−** No tagged releases

<sub>no GPU · Docker + Compose · Needs Node.js, Playwright Chromium · port 3000 · [Repo](https://github.com/jae-jae/fetcher-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fetcher-mcp/)</sub>

<a name="mcpm-sh"></a>
### #&#8288;156 [mcpm.sh](https://github.com/pathintegral-institute/mcpm.sh) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**CLI that installs MCP servers once and wires them into clients.**

MCPM is a Python CLI that keeps a single global list of MCP servers, installed from a central registry or added manually. Servers can be grouped into profiles, run over stdio or HTTP, shared through a tunnel, and enabled per client such as Claude Desktop, Cursor, Windsurf, VS Code and Cline. It also updates git-based servers and supports non-interactive use.

- **+** One global server list reused across Claude Desktop, Cursor, Windsurf, VS Code, Cline and others
- **+** Profiles group servers and can be run together over stdio or HTTP
- **+** Non-interactive mode via MCPM_NON_INTERACTIVE and JSON output, plus an llm.txt command guide
- **+** Installs via brew, pipx, uv, pip or an install script
- **−** Demo GIF still shows outdated v1 commands, per the README
- **−** Execution in Docker is listed as not yet implemented
- **−** Advanced access monitoring and analytics are still unchecked on the roadmap
- **−** GitHub release binary updates are not implemented yet

<sub>no GPU · Docker · Needs Python 3.10+ · port 6276 · [Repo](https://github.com/pathintegral-institute/mcpm.sh) · [🌐 Site ↗](https://mcpm.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcpm-sh/)</sub>

<a name="claude-task-master"></a>
### #&#8288;157 [claude-task-master](https://github.com/eyaltoledano/claude-task-master) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (91) · Freshness: recent (63) · Maintenance: weak (8) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Apr 2026</sub>

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

<a name="mcp-server-chart"></a>
### #&#8288;158 [mcp-server-chart](https://github.com/antvis/mcp-server-chart) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (61) · Freshness: active (92) · Maintenance: weak (24) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Aug 2026</sub>

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

<a name="rpa"></a>
### #&#8288;159 [rpa](https://github.com/a9t9/rpa) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (42) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · custom license · Sep 2026</sub>

**Browser and desktop automation extension with an MCP bridge for AI agents.**

Ui.Vision is a Manifest V3 browser extension for Chrome, Edge and Firefox that records and replays macros, with a uiv.* JavaScript API, Selenium IDE commands, OCR and image matching. The uivision-mcp-bridge package, installed with npx, lets MCP clients such as Claude Code, Claude Desktop and Cursor create, edit and run macros, then check logs and screenshots. Desktop automation needs the separate XModules components.

- **+** Runs in your existing browser session; installs from Chrome, Edge and Firefox stores
- **+** Visual OCR and image matching work where HTML selectors are unavailable
- **+** MCP bridge installer registers with supported clients via one npx command
- **+** Saved macros are reusable and can run without an AI agent
- **−** Desktop automation requires the separate XModules install
- **−** License is reported as NOASSERTION, so terms need checking
- **−** Macros run sequentially; the uiv.* API has no async or await
- **−** Repository README gives no hardware or resource requirements

<sub>Needs Chrome, Edge or Firefox, Node.js and npm (MCP bridge installer), Ui.Vision XModules (desktop automation) · [Repo](https://github.com/a9t9/rpa) · [📖 Docs ↗](https://ui.vision/ai/ai-system-prompt) · [🌐 Site ↗](https://ui.vision/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rpa/)</sub>

<a name="codemap"></a>
### #&#8288;160 [codemap](https://github.com/jordancoin/codemap) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (10) · Freshness: active (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 717 · MIT · Nov 2026</sub>

**Import-resolving dependency map and blast-radius checker for coding agents.**

codemap is a Go CLI that scans a repo, resolves imports using each ecosystem's real rules (go.mod, Cargo workspaces, package.json exports, tsconfig aliases), and reports hub files and who depends on a given file. Every answer carries a coverage status of complete, partial or unavailable. `codemap setup` wires hooks, MCP and skills into detected agents, and `codemap mcp` serves 19 tools over stdio.

- **+** Resolves imports via go.mod, Cargo, package.json exports and tsconfig paths, not string matching
- **+** Every dependency answer reports complete, partial or unavailable coverage
- **+** Single static binary; installs via Homebrew or Scoop, with a `codemap doctor` check
- **+** Hooks inject hub warnings at session start, before edits and at compaction
- **−** Build-system-aware resolution documented only for Go, Rust, JS and TS
- **−** `codemap find` is lexical only, with no semantic retrieval
- **−** Per-query coverage and per-edge provenance are still roadmap items
- **−** Go imports resolve at package level, so file-level importer counts are coarser

<sub>no GPU · [Repo](https://github.com/jordancoin/codemap) · [📖 Docs ↗](https://github.com/jordancoin/codemap/blob/main/docs/INSTALL.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codemap/)</sub>

<a name="camoufox-cli"></a>
### #&#8288;161 [camoufox-cli](https://github.com/bin-huang/camoufox-cli) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 365 · MIT · Nov 2026</sub>

**Shell CLI that drives a fingerprint-spoofing Camoufox Firefox for AI agents.**

camoufox-cli wraps the Camoufox anti-detect Firefox build in shell commands (open, snapshot, click, fill, eval, screenshot). A background daemon holds the browser and talks to the CLI over a Unix socket. Agents target elements by @ref from accessibility-tree snapshots. A skill entry file lets Claude Code, Cursor and Codex discover the usage guide.

- **+** Camoufox patches canvas, WebGL, audio, fonts and screen metrics at the C++ level
- **+** --persistent freezes fingerprint, OS and seeds so a profile looks like the same device
- **+** Named tabs share one login; named sessions run as isolated processes with separate cookies
- **+** Plain shell commands work with any agent, and the skill reads the guide for the installed version
- **−** Fingerprint layer only; IP reputation, request rate and behavior checks still apply
- **−** Unix socket daemon design; Windows support is not mentioned
- **−** Browser binary is downloaded from GitHub releases, which can hit rate limits
- **−** No MCP server; integration relies on the agent running shell commands

<sub>Needs Node.js 20.10+ or Python (pipx), Camoufox browser download, Playwright · [Repo](https://github.com/bin-huang/camoufox-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/camoufox-cli/)</sub>

<a name="automate"></a>
### #&#8288;162 [automate](https://github.com/yuruotong1/automate) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (58) · Freshness: active (97) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Sep 2026</sub>

**MCP server giving AI clients shared notes, files, reminders and memory.**

autoMate is a FastAPI service that stores notes, files, reminders and long-term memory in SQLite under ~/.automate/. It exposes them, plus shell, script, browser, desktop and 31 SaaS connectors, over MCP-over-HTTP at /mcp/. Claude Desktop, Cursor, Cline and OpenClaw can use it as a shared tool source, or you can use its built-in web chat with a 25-provider LLM catalog.

- **+** Notes, files and memory persist across different AI clients through one MCP endpoint
- **+** Installs via pip, standalone binaries, Docker, Chrome extension or PWA
- **+** Secrets encrypted with Fernet; server binds to 127.0.0.1 by default
- **+** Hybrid BM25 search (SQLite FTS5) across notes and files in one call
- **−** MCP bearer token grants access to shell.exec, so a leaked token allows command execution
- **−** IM channels like WeChat and Telegram need a separate OpenClaw gateway
- **−** Audio transcription is listed as a Pro tier feature tied to autoMate Cloud
- **−** Wide scope (desktop control, shell, 31 SaaS APIs) enlarges the surface to secure

<sub>no GPU · Docker · Needs Python, SQLite, Playwright (browser tools), OpenClaw (optional, for IM channels) · Models: OpenAI, Anthropic, Gemini, xAI Grok, Mistral · port 8765 · [Repo](https://github.com/yuruotong1/automate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/automate/)</sub>

<a name="jadx-mcp-server"></a>
### #&#8288;163 [jadx-mcp-server](https://github.com/zinja-coder/jadx-mcp-server) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 859 · Apache-2.0 · Oct 2026</sub>

**MCP server that lets LLMs inspect decompiled Android APKs in JADX-GUI.**

A Python MCP server that forwards tool calls over HTTP to the JADX-AI-MCP plugin running inside jadx-gui. It exposes about 25 tools for fetching class source, smali, manifest and resources, cross-references, comments, renames and debugger state. It runs over stdio or HTTP (default port 8651) and talks to the plugin on port 8650.

- **+** Covers class source, smali, manifest components, resources and xrefs, with pagination
- **+** Can write back to JADX: rename variables, add and list comments
- **+** Exposes jadx debugger stack frames, threads and variables to the model
- **+** Includes an example adapter for OpenAI-compatible endpoints such as Ollama and LiteLLM
- **−** Needs the separate JADX-AI-MCP plugin and a running jadx-gui to work
- **−** Tested only on Claude Desktop, per the README
- **−** HTTP mode has no authentication or TLS; remote binding needs a tunnel or firewall
- **−** Docker support and Hermes (React Native) support are unchecked on the roadmap

<sub>no GPU · Needs JADX-AI-MCP plugin, jadx-gui, Java 11+, Python 3.10+, uv · Models: Claude Desktop, OpenAI-compatible APIs via example client · port 8651 · [Repo](https://github.com/zinja-coder/jadx-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jadx-mcp-server/)</sub>

<a name="flutter-skill"></a>
### #&#8288;164 [flutter-skill](https://github.com/ai-dashboad/flutter-skill) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: patchy (50) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 413 · MIT · Sep 2026</sub>

**MCP server that lets AI agents tap, type and inspect running apps for E2E testing.**

flutter-skill is an MCP server (stdio) and HTTP CLI that connects AI agents such as Claude, Cursor and Windsurf to a running app. The agent can screenshot, read an accessibility-tree snapshot, tap, type, scroll and assert, without test code. It covers Flutter plus React Native, Electron, Tauri, Android, iOS, KMP, .NET MAUI and web via CDP, with SDKs added to the app in a few lines.

- **+** Covers 10 platforms, including Flutter, React Native, Electron, Tauri and plain web via CDP
- **+** Accessibility-tree snapshots cut tokens versus screenshots (README claims 87-99% fewer)
- **+** Exposes 253 MCP tools including visual regression, network mocking and a11y audits
- **+** Installs via npm, Homebrew, Scoop, pub.dev or Docker; works with any MCP client
- **−** Native platforms need an SDK added to the app, not fully zero-config
- **−** Benchmarks and test scores are self-reported, run against the project's own demo app
- **−** Flutter test score is 188/195; web CDP is 141/156, so some tools fail
- **−** Tool count is very large, which can bloat agent context

<sub>no GPU · Docker · Needs Node.js (npm install), Chrome (web/CDP mode), MCP-compatible AI client · [Repo](https://github.com/ai-dashboad/flutter-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flutter-skill/)</sub>

<a name="bb-browser"></a>
### #&#8288;165 [bb-browser](https://github.com/epiral/bb-browser) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: popular (70) · Freshness: recent (75) · Maintenance: weak (5) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · May 2026</sub>

**CLI and MCP server that lets agents drive your logged-in Chrome.**

bb-browser runs site adapters (one JS file per command) inside your real browser tab, using your existing cookies and login state. It ships 103 commands across 36 platforms, such as Twitter, Reddit, GitHub, arXiv and Zhihu, and also offers general automation (snapshot, click, fill, eval, network capture). Agents call it through a CLI or an MCP stdio server, and a local daemon talks to the browser over CDP.

- **+** Reuses your real logged-in browser, so no API keys or separate login flows
- **+** Community adapters are single JS files in the bb-sites repo, in three auth tiers
- **+** All commands support --json, --jq filtering and --tab for concurrent tabs
- **+** Works as both CLI and MCP server for Claude Code, Cursor and similar agents
- **−** Adapters call undocumented site endpoints and page internals, so site changes can break them
- **−** Acts with your personal accounts, so agent mistakes or prompt injection affect real logins
- **−** Needs a running local daemon and your Chrome session, which is awkward for headless servers
- **−** Daemon --host 0.0.0.0 option exposes browser control beyond localhost if misconfigured

<sub>no GPU · Docker · Needs Node.js 18+, Chrome (CDP) with bb-browser extension or daemon, OpenClaw (optional) · port 19824 · [Repo](https://github.com/epiral/bb-browser) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bb-browser/)</sub>

<a name="mcp-server-qdrant"></a>
### #&#8288;166 [mcp-server-qdrant](https://github.com/qdrant/mcp-server-qdrant) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (33) · Freshness: active (86) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Nov 2026</sub>

**MCP server that stores and searches semantic memories in Qdrant.**

Official Qdrant MCP server exposing two tools, `qdrant-store` and `qdrant-find`, so an MCP client can save text with optional JSON metadata and retrieve it by semantic search. It embeds with FastEmbed (default `sentence-transformers/all-MiniLM-L6-v2`) and connects to a Qdrant server or a local on-disk database. Tool descriptions are configurable, so it can act as a code-snippet store for Cursor, Windsurf or Claude Code.

- **+** Runs with a single `uvx mcp-server-qdrant` command, no install step
- **+** Supports stdio, SSE and streamable-http transports
- **+** Works with a remote Qdrant URL or a local path via QDRANT_LOCAL_PATH
- **+** Read-only mode and custom tool descriptions set through environment variables
- **−** Only FastEmbed embedding models are supported
- **−** Only two tools: store and find, no delete or collection management
- **−** Stores free text plus metadata; it does not index a repository itself
- **−** QDRANT_URL and QDRANT_LOCAL_PATH cannot be set together

<sub>Docker · Needs Qdrant (server or local path), FastEmbed · Models: FastEmbed models, sentence-transformers/all-MiniLM-L6-v2 (default) · port 8000 · [Repo](https://github.com/qdrant/mcp-server-qdrant) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-qdrant/)</sub>

<a name="coderunner"></a>
### #&#8288;167 [coderunner](https://github.com/instavm/coderunner) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 903 · Apache-2.0 · Nov 2026</sub>

**Local Apple-container sandbox that runs agent Python code via MCP.**

CodeRunner runs code written by AI agents inside an Apple container VM on Apple Silicon Macs, with a Jupyter kernel behind an MCP server on port 8222. Host folders are mounted under /workspace (read-only by default), and outbound network can be disabled. Tools cover Python execution, named sessions, Playwright page scraping and a small skills system.

- **+** VM-level isolation via apple/container; host mounts are read-only unless marked :rw
- **+** Bearer token auth generated at install; only GET /health is public
- **+** Named sessions give isolated Jupyter kernels, up to five concurrently
- **+** Documented configs for Claude Desktop, Claude Code, OpenCode, Gemini CLI, Kiro, OpenAI Agents
- **−** Requires macOS on Apple Silicon; Linux support via Firecracker is only on the roadmap
- **−** Outbound network is unrestricted by default; must set CODERUNNER_NETWORK=none
- **−** Python kernel state is lost on VM or server restart
- **−** Mount and resource limits are fixed at creation; changing them means recreating the container

<sub>no GPU · Docker + Compose · Needs apple/container, Python 3.10+, macOS on Apple Silicon · Models: Claude Desktop, Claude Code, OpenCode, OpenAI Agents, Gemini CLI · port 8222 · [Repo](https://github.com/instavm/coderunner) · [🌐 Site ↗](https://instavm.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coderunner/)</sub>

<a name="discord-mcp"></a>
### #&#8288;168 [discord-mcp](https://github.com/saseq/discord-mcp) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (8) · Freshness: active (94) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 621 · MIT · Oct 2026</sub>

**MCP server exposing Discord server management and messaging as tools.**

A Java (JDA) Model Context Protocol server that lets MCP clients drive a Discord bot. It exposes tools for messages, channels, categories, threads, forums, roles, moderation, webhooks, invites, emojis, voice channels and scheduled events. It runs as an HTTP server with endpoint /mcp on port 8085, with a legacy stdio mode.

- **+** Wide tool coverage: messaging, roles, moderation, threads, forums, webhooks, permission overwrites, events
- **+** HTTP singleton mode at :8085/mcp serves multiple clients from one container
- **+** Optional DISCORD_GUILD_ID makes guildId optional across all tools
- **+** Setup snippets for Claude Code, Codex CLI, Cursor, n8n, OpenClaw and Claude Desktop
- **−** Needs your own Discord bot token and a bot added to the server
- **−** Destructive tools (ban, kick, delete channel, delete role) are exposed with no stated confirmation or scoping
- **−** Message search scans only the latest 1000 messages, not a server-side index
- **−** Claude Desktop remote connectors need a public HTTPS endpoint; localhost does not work

<sub>no GPU · Docker + Compose · Needs Discord bot token, Docker or Java with Maven · port 8085 · [Repo](https://github.com/saseq/discord-mcp) · [📖 Docs ↗](https://github.com/SaseQ/discord-mcp/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/discord-mcp/)</sub>

<a name="minimax-mcp"></a>
### #&#8288;169 [minimax-mcp](https://github.com/minimax-ai/minimax-mcp) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (34) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**MCP server for MiniMax text-to-speech, voice cloning, image and video generation.**

Official MiniMax MCP server, run with uvx, that exposes the MiniMax API to MCP clients such as Claude Desktop, Cursor, Windsurf and OpenAI Agents. Tools cover text-to-speech, voice listing, cloning and design, video generation with status queries, and image generation and editing. It supports stdio and SSE transports, and outputs can be returned as URLs or downloaded locally.

- **+** Eight tools cover TTS, voice clone/design, video, image generation and image editing
- **+** Supports both stdio and SSE transports, so it can run locally or in the cloud
- **+** Configurable output: return URLs or download files to a local base path
- **+** Installs with a single uvx entry in the MCP client config
- **−** Requires a paid MiniMax API key; README warns tool use may incur costs
- **−** API key and host must match region (global vs mainland) or calls fail
- **−** Only wraps MiniMax services; no local model inference
- **−** No tagged releases; README points to a newer CLI as recommended

<sub>no GPU · Needs MiniMax API key, uv · Models: MiniMax-H3-Image, image-01, MiniMax-Hailuo-02 · [Repo](https://github.com/minimax-ai/minimax-mcp) · [🌐 Site ↗](https://www.minimax.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/minimax-mcp/)</sub>

<a name="ref-tools-mcp"></a>
### #&#8288;170 [ref-tools-mcp](https://github.com/ref-tools/ref-tools-mcp) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**MCP server that searches and reads documentation for coding agents.**

Ref MCP exposes two tools, ref_search_documentation and ref_read_url, so a coding agent can search public docs, GitHub, and private repos or PDFs, then read pages as markdown. It uses MCP session history to drop repeated search results and trims fetched pages to the most relevant ~5k tokens. This repo holds the legacy stdio server; the recommended streamable-HTTP endpoint is hosted at api.ref.tools and needs an API key.

- **+** Session-aware search never repeats earlier results, so agents can page and refine in one call
- **+** Page reads return the most relevant ~5k tokens instead of 20k+ raw fetches
- **+** Runs over stdio via npx or hosted streamable HTTP; Cursor install links provided
- **+** Offers OpenAI deep research tool names (search, fetch) alongside its own
- **−** Requires a Ref API key from signing up; search depends on the hosted service
- **−** Repo contains only the legacy stdio server, not the recommended HTTP one
- **−** Only two tools, limited to documentation search and URL reading
- **−** No self-hosted index or offline mode described

<sub>no GPU · Docker · Needs Ref API key (api.ref.tools), Node.js / npx · [Repo](https://github.com/ref-tools/ref-tools-mcp) · [🌐 Site ↗](https://ref.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ref-tools-mcp/)</sub>

<a name="git-mcp"></a>
### #&#8288;171 [git-mcp](https://github.com/idosal/git-mcp) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (77) · Freshness: recent (59) · Maintenance: weak (4) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · May 2026</sub>

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

<a name="drissionpage-mcp-server"></a>
### #&#8288;172 [drissionpage-mcp-server](https://github.com/jumodada/drissionpage-mcp-server) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 483 · custom license · Oct 2026</sub>

**MCP server exposing DrissionPage browser automation as 69 typed tools.**

A local stdio MCP server that wraps DrissionPage (Chromium over CDP) and exposes 69 typed tools for navigation, DOM extraction, cookies, network listening, screenshots and coordinate-based pointer control. It offers direct and a deterministic 24-step "natural" pointer path for visual-only surfaces. Setup snippets cover Codex, Claude Code, Claude Desktop and Cursor. Marked beta; version 0.9.0.

- **+** 69 typed tools covering tabs, frames, shadow DOM, cookies, storage and network listening
- **+** Deterministic pointer motion with failure-safe button release, plus coordinate click and drag
- **+** Secrets redacted by default in cookies, storage and headers; file I/O limited to configured root directories
- **+** CI enforces a 95% coverage floor with real Chrome integration tests
- **−** Marked beta; README says 0.9.0 was still a local candidate, not yet on PyPI
- **−** Needs a local Chromium/Chrome install and a Python 3.10+ environment
- **−** Challenge and site-specific workflows are left to the client or optional external Skills
- **−** License is flagged NOASSERTION by detection, though README badge says Apache 2.0

<sub>no GPU · Needs Python 3.10+, Chrome/Chromium, DrissionPage · Models: Any MCP client (Codex, Claude Code, Claude Desktop, Cursor) · [Repo](https://github.com/jumodada/drissionpage-mcp-server) · [▶️ Demo ↗](https://drissionpage-mcp.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/drissionpage-mcp-server/)</sub>

<a name="mcp-server-gateway"></a>
### #&#8288;173 [mcp-server-gateway](https://github.com/harish-gaggar/mcp-server-gateway) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 586 · custom license · Oct 2026</sub>

**MCP gateway with per-user OAuth, example MCP servers and a LangGraph agent.**

Reference stack for running an MCP gateway that proxies OAuth-authenticated, audited calls to example MCP servers for Artifactory, GitHub and Google Drive. It also includes a LangGraph agent (jfrog-agent) with SQLite-backed memory, a context optimizer and per-query tracking, plus a separate PII and secrets guard (agent-safety-kit). It is a blueprint to fork for restricted or air-gapped networks, not a hosted product.

- **+** Gateway logs every operation and runs OAuth per user before each MCP tool call
- **+** Ships three working example MCP servers: Artifactory, GitHub, Google Drive
- **+** Smoke-test and e2e scripts verify gateway-to-server routing after startup
- **+** Separate PII and secrets scrubber installable with pip, no Docker needed
- **−** README calls it a reference implementation and says APIs may change
- **−** Default open mode hides the GitHub namespace; OAuth needs extra config files
- **−** Reference agent is JFrog-specific and needs adapting for other tools
- **−** Five containers including Redis; first build can take several minutes

<sub>no GPU · Needs Docker Compose v2, Redis, Node.js 20+ (smoke tests), Python 3.10+, GitHub OAuth app (optional), Google OIDC (secure mode) · port 8090 · [Repo](https://github.com/harish-gaggar/mcp-server-gateway) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-gateway/)</sub>

<a name="mcp-server"></a>
### #&#8288;174 [mcp-server](https://github.com/portswigger/mcp-server) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (0) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21 · GPL-3.0 · Nov 2026</sub>

**Burp Suite extension that exposes Burp tools to AI clients over MCP.**

A Kotlin Burp Suite extension that runs an MCP server inside Burp, listening on 127.0.0.1:9876 by default. It serves Streamable HTTP at /mcp and legacy SSE at /, and bundles a stdio proxy jar for clients that only support stdio. It includes an installer for Claude Desktop and a Codex plugin with a skill.

- **+** Serves both Streamable HTTP (/mcp) and legacy SSE transports from the extension
- **+** Bundled stdio proxy jar covers clients without HTTP MCP support
- **+** Burp asks for approval before sending requests or reading proxy history
- **+** Installer for Claude Desktop and a Codex plugin with a usage skill
- **−** README documents building from source with Gradle, no prebuilt install steps
- **−** Requires Burp Suite plus Java and the jar command on PATH
- **−** Optional config-editing tools can modify Burp configuration files when enabled
- **−** Stdio setup needs manual Java path and proxy jar path

<sub>no GPU · Needs Burp Suite, Java, jar command, Gradle · Models: Claude Desktop, Codex, any MCP client · port 9876 · [Repo](https://github.com/portswigger/mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server/)</sub>

<a name="mcp-neo4j"></a>
### #&#8288;175 [mcp-neo4j](https://github.com/neo4j-contrib/mcp-neo4j) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (21) · Freshness: active (96) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 992 · MIT · Sep 2026</sub>

**MCP servers for querying Neo4j, storing memory, and managing Aura.**

Four Python MCP servers from Neo4j Labs: Cypher query execution with schema lookup, a knowledge-graph memory store, graph data modeling with Arrows.app import/export, and a Neo4j Aura instance manager. Each runs over STDIO, SSE or streamable HTTP, so they work with Claude Desktop, VS Code, Cursor, Windsurf and Gemini CLI.

- **+** Separate servers for querying, memory, data modeling and Aura management
- **+** STDIO, SSE and streamable HTTP transports, set by flag or environment variables
- **+** Cypher server returns the schema and runs both read and write queries
- **+** MIT license; cloud guide covers AWS ECS Fargate and Azure Container Apps
- **−** Labs program: no SLAs and no backwards-compatibility guarantees
- **−** Not supported by the Neo4j product team; a separate official server exists
- **−** Cypher server needs the APOC plugin enabled for schema inspection
- **−** No Docker or compose files detected in the repository

<sub>no GPU · Needs Neo4j database, APOC plugin (cypher server), Neo4j Aura account (aura-api server) · Models: Any MCP client (Claude Desktop, VS Code, Cursor, Windsurf, Gemini CLI) · [Repo](https://github.com/neo4j-contrib/mcp-neo4j) · [🌐 Site ↗](https://neo4j.com/labs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-neo4j/)</sub>

<a name="pal-mcp-server"></a>
### #&#8288;176 [pal-mcp-server](https://github.com/beehiveinnovations/pal-mcp-server) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: widely used (81) · Freshness: quiet (21) · Maintenance: weak (6) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Dec 2025</sub>

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

<a name="octocode"></a>
### #&#8288;177 [octocode](https://github.com/bgauryy/octocode) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (20) · Freshness: active (85) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 966 · MIT · Aug 2026</sub>

**Code research toolset for agents, as an MCP server and CLI.**

Octocode gives coding agents one set of tools for searching and reading code, both local files and external sources (GitHub repos, PRs, commits, issues, npm). It combines ripgrep, AST search, directory trees, minified reads and LSP navigation, backed by a prebuilt Rust engine. It runs over stdio as an MCP server or as a CLI that returns YAML, and redacts secrets before output reaches the model.

- **+** Same tools via MCP and CLI; 8 to 17 tools depending on flags
- **+** Minifies or skeletonizes code across 70+ languages to save tokens
- **+** Local AST search, LSP navigation and dead-code detection beside GitHub search
- **+** Scans output and redacts secrets before it reaches the model
- **−** GitHub tools need auth (OAuth, gh CLI or token) for private repos and rate limits
- **−** Local tools and clone are off by default on MCP; need env flags
- **−** Two tools need both ENABLE_* and ENABLE_TOOLS settings to register on MCP
- **−** LSP navigation depends on separately installed language servers

<sub>no GPU · Needs Node.js 20.12+, GitHub token (optional), Language servers for LSP tools · [Repo](https://github.com/bgauryy/octocode) · [📖 Docs ↗](https://github.com/bgauryy/octocode/blob/main/docs/OCTOCODE_TOOLS.md) · [🌐 Site ↗](https://octocode.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/octocode/)</sub>

<a name="gemini-mcp-tool"></a>
### #&#8288;178 [gemini-mcp-tool](https://github.com/jamubc/gemini-mcp-tool) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: known (45) · Freshness: active (82) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · custom license · Jun 2026</sub>

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

<a name="gemini-skill"></a>
### #&#8288;179 [gemini-skill](https://github.com/wjz-p/gemini-skill) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 835 · MIT · Nov 2026</sub>

**MCP server that drives the Gemini web UI via Chrome CDP for image generation.**

Node.js MCP server and library that automates gemini.google.com in a logged-in Chrome or Edge session over CDP, using puppeteer-extra stealth. It exposes tools for image generation, reference-image upload, full-size download with watermark removal, chat, model switching and session navigation. A background daemon keeps the browser alive and exits after 30 idle minutes. An OpenAI-compatible Atlas Cloud provider is also included.

- **+** Exposes about 20 gemini_* MCP tools; works from any stdio MCP client or as a JS library
- **+** Downloads full-size images and removes the Gemini watermark using sharp
- **+** Daemon auto-starts and reuses one browser with saved login; idle TTL set by DAEMON_TTL_MS
- **+** Selectors keep fallbacks for older Gemini UI versions
- **−** Depends on Gemini web DOM selectors, so UI changes can break it until patched
- **−** Image generation takes 60-120s; client timeout should be at least 180s
- **−** One browser instance per CDP port; parallel instances are an unchecked to-do
- **−** Stealth automation of the web UI may conflict with Google's terms of service

<sub>no GPU · Needs Node.js >= 18, Chrome, Edge or Chromium, Logged-in Google account, Atlas Cloud API key (optional) · Models: Gemini web (pro, flash, flash-lite), Atlas Cloud OpenAI-compatible API · [Repo](https://github.com/wjz-p/gemini-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-skill/)</sub>

<a name="mcp-for-argocd"></a>
### #&#8288;180 [mcp-for-argocd](https://github.com/argoproj-labs/mcp-for-argocd) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 608 · Apache-2.0 · Nov 2026</sub>

**MCP server that lets AI assistants query and manage Argo CD applications.**

TypeScript MCP server exposing Argo CD's API as tools: list, get, create, update, delete and sync applications, read resource trees, events and workload logs, and run resource actions. It runs over stdio (via npx) or HTTP, with an optional token registry for multiple Argo CD instances. A read-only mode disables the mutating tools.

- **+** Read-only mode (MCP_READ_ONLY) disables create, update, delete, sync and run_resource_action
- **+** API token read only from env or headers, never from tool arguments
- **+** Token registry file supports multiple Argo CD instances, each bound to its own base URL
- **+** HTTP listener binds loopback by default; non-loopback needs MCP_AUTH_TOKEN or an explicit flag
- **−** Mutating tools are enabled by default; read-only must be set explicitly
- **−** Self-signed certs are handled by disabling Node TLS verification globally
- **−** Covers only Argo CD applications, clusters and one AppProject getter; no wider project management
- **−** Stateful HTTP sessions break behind multiple replicas unless --stateless is used

<sub>no GPU · Docker · Needs Argo CD instance with API access, Argo CD API token, Node.js 18+ · port 3000 · [Repo](https://github.com/argoproj-labs/mcp-for-argocd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-for-argocd/)</sub>

<a name="ask-search"></a>
### #&#8288;181 [ask-search](https://github.com/ythx-101/ask-search) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (6) · Freshness: active (93) · Maintenance: weak (10) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 538 · MIT · Nov 2026</sub>

**Web search CLI and MCP server for agents, backed by SearxNG.**

ask-search wraps a self-hosted SearxNG instance in an `ask-search` CLI and a Python MCP server. It returns titles, URLs and snippets from Google, Bing, DuckDuckGo, Brave and others without a paid search API key. Tavily is an optional backend. It also ships an OpenClaw SKILL.md and a Docker Compose setup for SearxNG.

- **+** No search API key needed in default SearxNG mode
- **+** Same backend as CLI, MCP server (web_search, web_search_news) and OpenClaw skill
- **+** Optional Tavily backend via SEARCH_PROVIDER=tavily
- **+** Bundled Docker Compose and settings.yml with json format enabled
- **−** Returns only snippets and URLs; full page fetching is left to the agent
- **−** You must run and maintain a SearxNG container
- **−** Bot limiter may block requests; needs pass_ip tuning in limiter.toml
- **−** Tavily mode ignores --engines, --lang and --categories; native Windows untested

<sub>no GPU · Needs SearxNG, Docker Compose, Python 3.8+ (MCP server 3.10+), mcp package, curl, Tavily API (optional) · port 8080 · [Repo](https://github.com/ythx-101/ask-search) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ask-search/)</sub>

<a name="doris-mcp-server"></a>
### #&#8288;182 [doris-mcp-server](https://github.com/apache/doris-mcp-server) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: weak (12) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 360 · Apache-2.0 · Nov 2026</sub>

**Read-only MCP server exposing Apache Doris catalog, query, and cluster tools.**

Python MCP server that gives agents read-only access to Apache Doris over stdio or Streamable HTTP (MCP 2026-07-28). It groups 55 child capabilities into eight domain tools such as catalog, query, cluster, search and governance, discovered progressively. Queries are bounded by SQL shape, timeout, rows and bytes, and Doris RBAC stays the final authority.

- **+** Eight domain tools front 55 children, keeping the tool list short for hosts
- **+** Read-only runtime with bounded rows, bytes and timeout; Doris RBAC enforced
- **+** Supports static tokens, JWT, OAuth/OIDC; non-loopback HTTP requires auth
- **+** Flat exposure mode and legacy HTTP adapter cover older MCP hosts
- **−** Package classifier is Beta despite GA protocol compatibility
- **−** Read-only only; the doris_admin domain is reserved and not registered
- **−** Doris-backed OAuth is process-local; ADBC is off by default
- **−** Requires Python 3.12+ and Doris 2.0.0+ with FE MySQL port reachable

<sub>no GPU · Docker + Compose · Needs Apache Doris 2.0.0+, Python 3.12+ · port 3000 · [Repo](https://github.com/apache/doris-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/doris-mcp-server/)</sub>

<a name="mcp-server-docker"></a>
### #&#8288;183 [mcp-server-docker](https://github.com/ckreiling/mcp-server-docker) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (12) · Freshness: active (95) · Maintenance: weak (3) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 762 · GPL-3.0 · Aug 2026</sub>

**MCP server that manages Docker containers, images, networks and volumes from an LLM.**

A Python MCP server built on the Docker SDK that lets an MCP client such as Claude Desktop create, inspect and remove containers, images, networks and volumes. It includes a `docker_compose` prompt that runs a plan-and-apply loop, and exposes container logs and stats as resource templates. It connects to the local daemon, or to a remote one over SSH via DOCKER_HOST.

- **+** Covers containers, images, networks and volumes with named tools, plus logs and stats resources
- **+** docker_compose prompt shows a plan for approval before applying changes
- **+** Remote Docker engines supported through an ssh:// DOCKER_HOST
- **+** Test suite runs without a Docker daemon; installs with uvx
- **−** README warns against passing secrets such as API keys or passwords to containers
- **−** No support for --privileged or --cap-add/--cap-drop
- **−** No tools for Compose files; the compose prompt drives individual container tools
- **−** GPL-3.0 license may limit embedding in proprietary products

<sub>no GPU · Docker · Needs Docker daemon, uv, MCP client (e.g. Claude Desktop) · [Repo](https://github.com/ckreiling/mcp-server-docker) · [▶️ Demo ↗](https://github.com/user-attachments/assets/65e35e67-bce0-4449-af7e-9f4dd773b4b3) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-server-docker/)</sub>

<a name="openapi-mcp-server"></a>
### #&#8288;184 [openapi-mcp-server](https://github.com/janwilmake/openapi-mcp-server) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (17) · Freshness: active (81) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 906 · MIT · Jul 2026</sub>

**MCP server for searching and reading OpenAPI specs via oapis.org.**

A Model Context Protocol server, written in TypeScript and run with wrangler, that lets Claude Desktop or Cursor look up an OpenAPI spec through oapis.org. It resolves the spec identifier, fetches a plain-language summary, then returns details for the specific endpoints needed. A hosted instance is available at openapi-mcp.openapisearch.com/mcp.

- **+** Hosted MCP URL provided, so no local install is needed for most clients
- **+** Three-step flow returns plain-language summaries instead of raw spec dumps
- **+** Handles both JSON and YAML OpenAPI specs
- **+** MIT licensed; local dev with wrangler dev and MCP inspector
- **−** Depends on the oapis.org service for spec lookup and summaries
- **−** Tested only with Claude Desktop and Cursor, per the README
- **−** No tagged releases
- **−** Documentation is minimal: no tool list or self-hosting guide

<sub>no GPU · Needs oapis.org, Cloudflare Wrangler · [Repo](https://github.com/janwilmake/openapi-mcp-server) · [▶️ Demo ↗](https://x.com/janwilmake/status/1903497808134496583) · [🌐 Site ↗](https://openapi-mcp.openapisearch.com/mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openapi-mcp-server/)</sub>

<a name="mcp-google-sheets"></a>
### #&#8288;185 [mcp-google-sheets](https://github.com/xing5/mcp-google-sheets) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: niche (22) · Freshness: recent (72) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · May 2026</sub>

**MCP server exposing Google Sheets and Drive operations to MCP clients.**

Python MCP server that lets clients such as Claude Desktop read, write, create, share and chart Google Sheets through the Sheets and Drive APIs. It runs via `uvx mcp-google-sheets@latest` and authenticates with a service account, OAuth 2.0, or Base64 credentials in an environment variable. The README lists 19 tools, and an include-tools filter trims the roughly 13K tokens they use by default.

- **+** Covers read, write, batch update, copy, rename, sharing and charts in one server
- **+** Three auth modes: service account, OAuth 2.0, and Base64 credentials via env var
- **+** Tool filtering via --include-tools or ENABLED_TOOLS cuts context use
- **+** Starts with a single uvx command, no clone or install step
- **−** All 19 tools cost about 13K tokens of context unless filtered
- **−** Requires Google Cloud project setup with Sheets and Drive APIs enabled
- **−** Service account only sees Drive folders explicitly shared with it
- **−** Tool set is Sheets-only; no other Google Workspace apps

<sub>no GPU · Docker · Needs Google Sheets API, Google Drive API, uv, Google Cloud service account or OAuth credentials · [Repo](https://github.com/xing5/mcp-google-sheets) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-google-sheets/)</sub>

<a name="mantic-sh"></a>
### #&#8288;186 [mantic.sh](https://github.com/marcoaapfortes/mantic.sh) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: niche (7) · Freshness: active (88) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 552 · MIT · Jul 2026</sub>

**Local code search CLI and MCP server that ranks files by intent.**

Mantic is a TypeScript CLI and MCP server that ranks repository files for a query using path structure, filename and metadata scoring over `git ls-files`, rather than reading file contents. It also offers Tree-sitter go-to-definition and find-references, impact analysis, session context carryover, and optional local semantic reranking via transformers.js. It plugs into Claude Desktop, Cursor and VS Code as a stdio MCP server.

- **+** Runs locally via npx or stdio MCP; README states zero data egress
- **+** Ranks by path, CamelCase and filename matching, with directory boosting
- **+** Includes goto, references and impact analysis commands, also exposed as MCP tools
- **+** Shareable learned search patterns stored in .mantic/search-patterns.json
- **−** README's own benchmarks show it 2-10x slower than ripgrep on raw text search
- **−** Chromium-scale repo (481K files) takes about 2s per query versus 0.38s for ripgrep
- **−** Not suited to exact string matching; README recommends ripgrep for that
- **−** Benchmarks and the 4/5 assessment are self-reported, with no independent validation

<sub>no GPU · Needs Node.js, git · Models: transformers.js local embeddings (optional --semantic) · [Repo](https://github.com/marcoaapfortes/mantic.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mantic-sh/)</sub>

<a name="universal-db-mcp"></a>
### #&#8288;187 [universal-db-mcp](https://github.com/anarkh-lee/universal-db-mcp) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: niche (18) · Freshness: recent (52) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 945 · MIT · Mar 2026</sub>

**MCP and REST server that lets AI assistants query 17 databases.**

Node.js server that exposes MySQL, PostgreSQL, Redis, Oracle, SQL Server, MongoDB, SQLite and ten other databases to AI clients through MCP (stdio, SSE, Streamable HTTP) and a REST API. Tools cover query execution, schema and table info, sample data and enum values. It runs read-only by default, with configurable permission modes, schema caching and data masking.

- **+** Covers 17 databases, including Oracle, ClickHouse, TiDB and several Chinese domestic databases
- **+** Read-only by default, with safe, readwrite, full and custom permission modes
- **+** Offers stdio, SSE, Streamable HTTP and REST access from one package
- **+** Schema caching and masking of phone, email, ID card and bank card data
- **−** Database passwords are passed as CLI args, URL query strings or headers
- **−** Performance table gives no baseline, so the quoted speedups are unverified
- **−** Write and DDL access is one flag away, so it relies on read-only DB accounts
- **−** Requires Node.js 20 or newer

<sub>no GPU · Docker + Compose · Needs Node.js >= 20, A target database (MySQL, PostgreSQL, etc.) · port 3000 · [Repo](https://github.com/anarkh-lee/universal-db-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/universal-db-mcp/)</sub>

<a name="devdocs"></a>
### #&#8288;188 [devdocs](https://github.com/cyberagiinc/devdocs) <sub>score [20](../README.md#-how-we-rank "Score 20/100. Adoption: known (41) · Freshness: quiet (25) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Feb 2026</sub>

**Documentation crawler that serves scraped docs to LLMs through an MCP server.**

DevDocs crawls a documentation site to a chosen depth of 1 to 5 levels using Crawl4AI. It exports content as Markdown or JSON and exposes it through an MCP server with Table of Contents and Section Access tools, which Claude, Cline or Roo Code can query. The README states the public repo is not maintained and an enhanced internal version exists.

- **+** Crawls with selectable depth from 1 to 5 and discovers child URLs
- **+** Exports Markdown or JSON and serves the content through an MCP server
- **+** Docker start script brings up frontend, backend, MCP and Crawl4AI together
- **+** Apache-2.0 licensed and self-hosted, with no page limits stated
- **−** README says the public version is not maintained; no releases published
- **−** Windows support is marked experimental and untested
- **−** API access is listed as coming soon; roadmap items are unimplemented
- **−** README speed and pricing claims against Firecrawl are unsourced

<sub>no GPU · Docker + Compose · Needs Docker, Crawl4AI · Models: Claude (via MCP), Cline, Roo Code · port 3001 · [Repo](https://github.com/cyberagiinc/devdocs) · [🌐 Site ↗](https://www.cyberagi.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devdocs/)</sub>

<a name="apple-docs-mcp"></a>
### #&#8288;189 [apple-docs-mcp](https://github.com/kimsungwhee/apple-docs-mcp) <sub>score [20](../README.md#-how-we-rank "Score 20/100. Adoption: niche (30) · Freshness: slowing (37) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Mar 2026</sub>

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

<a name="vectorcode"></a>
### #&#8288;190 [vectorcode](https://github.com/davidyz/vectorcode) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: niche (16) · Freshness: quiet (24) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 875 · MIT · Dec 2025</sub>

**Code repository indexer that feeds relevant project context to coding LLMs.**

VectorCode indexes a code repository into a Chroma vector store and returns task-relevant chunks to inject into LLM prompts. It ships a Python CLI plus a Neovim plugin with a Lua API, and integrates with codecompanion.nvim and MCP. Chunking uses tree-sitter, and indexing respects .gitignore. The author describes it as beta, with breaking changes on minor version bumps.

- **+** Syntax-aware chunking via py-tree-sitter and tree-sitter-language-pack
- **+** Respects .gitignore and detects project root from .git or .vectorcode/
- **+** Neovim Lua API for building or extending AI plugins
- **+** Persistent local Chroma client, installable from PyPI
- **−** Beta quality; minor releases may remove features or config options
- **−** Remote Chromadb with authentication is not yet supported
- **−** Query rewriting is still an open TODO
- **−** Editor integrations center on Neovim; other editors rely on MCP

<sub>Needs ChromaDB, tree-sitter-language-pack · [Repo](https://github.com/davidyz/vectorcode) · [📖 Docs ↗](https://github.com/Davidyz/VectorCode/blob/main/docs/cli.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vectorcode/)</sub>

<a name="context-space"></a>
### #&#8288;191 [context-space](https://github.com/context-space/context-space) <sub>score [4](../README.md#-how-we-rank "Score 4/100. Adoption: niche (13) · Freshness: quiet (0) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 814 · AGPL-3.0 · Oct 2025</sub>

**MCP gateway with managed OAuth for GitHub, Slack, Notion and other services.**

Context Space is a Go backend that exposes third-party services to AI agents through one REST API and one aggregated MCP endpoint. It handles OAuth flows and stores credentials in HashiCorp Vault. The README lists 14+ integrations, including GitHub, Slack, Airtable, HubSpot, Notion, Spotify and Stripe, with one-line setup for Cursor and Claude Code.

- **+** Single MCP endpoint aggregates all connected services for Cursor and Claude Code
- **+** OAuth flows with credentials stored in HashiCorp Vault
- **+** Unified REST API with published docs for invoking service operations
- **+** Hosted instance available to try the integrations
- **−** AGPL-3.0 license, with a planned Apache 2.0 move that has no date
- **−** Memory, semantic retrieval and smart aggregation are roadmap items, not shipped
- **−** Only 14+ integrations; new services need code contributions
- **−** README has no self-hosting steps, and no Docker files were detected

<sub>no GPU · Needs HashiCorp Vault · [Repo](https://github.com/context-space/context-space) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-space/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
