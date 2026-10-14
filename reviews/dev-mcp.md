# 🔌 MCP servers for developers reviews · Best of Vibe Coding

MCP servers that give coding agents tools: docs lookup, browsers, GitHub, databases and code navigation. Back to the [leaderboard](../README.md#-mcp-servers-for-developers).

<sub>🌐 Also on the web: [MCP servers for developers on archestack.com](https://archestack.com/best-of-vibe-coding/dev-mcp/), each project on its own page.</sub>

<a name="codegraph"></a>
### 🥇 [codegraph](https://github.com/colbymchenry/codegraph) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 74k · MIT · Oct 2026</sub>

**Local code knowledge graph served to coding agents over MCP.**

CodeGraph indexes a project into a local graph of symbols, call edges and dependencies under `.codegraph/`, then exposes it to coding agents through an MCP server. Agents can fetch relevant source, call paths and change impact in one call instead of grepping and reading files. `codegraph install` wires it into Claude Code, Cursor, Codex CLI, opencode, Gemini CLI, Kiro, GitHub Copilot and others, and auto-sync keeps the index current.

- **+** Runs locally; no Node.js needed, ships as a bundled installer or npm package
- **+** One `codegraph install` configures MCP for nine named agents and IDEs
- **+** Covers 30+ languages, including TypeScript, Python, Go, Rust, Java, C#, Swift
- **+** Watches files and updates the graph automatically; no manual re-index
- **−** README admits about 80% more retrieval context stays resident in long sessions
- **−** Published benchmarks are the author's, on 7 repos with one question each
- **−** No Docker or compose setup; install is via curl/PowerShell script or npm
- **−** Hosted CodeGraph platform is a waitlist product, separate from this repo

<sub>no GPU · safety checks passed 11 of 13 · [Repo](https://github.com/colbymchenry/codegraph) · [📖 Docs ↗](https://colbymchenry.github.io/codegraph/) · [🌐 Site ↗](https://getcodegraph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegraph/)</sub>

<a name="chrome-devtools-mcp"></a>
### 🥈 [chrome-devtools-mcp](https://github.com/chromedevtools/chrome-devtools-mcp) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 53k · Apache-2.0 · Oct 2026</sub>

**MCP server that lets coding agents drive and debug a live Chrome.**

chrome-devtools-mcp is an MCP server that gives coding agents such as Claude, Cursor and Copilot control of a live Chrome browser. It records performance traces through Chrome DevTools, inspects network requests and console messages with source-mapped stack traces, and automates page actions via puppeteer. A CLI is included for use without MCP, and a --slim mode exposes a smaller tool set.

- **+** Records DevTools performance traces and extracts insights from them
- **+** Puppeteer-based automation waits for action results automatically
- **+** Slim mode limits the exposed tools to basic browser tasks
- **+** Also ships a CLI for use without an MCP client
- **−** Usage statistics are sent to Google by default; opt out with --no-usage-statistics
- **−** Performance tools may send trace URLs to the Google CrUX API
- **−** Officially supports only Chrome and Chrome for Testing
- **−** Exposes all browser content to the connected MCP client

<sub>no GPU · Needs Node.js LTS, npm, Google Chrome (current stable) · safety checks passed 14 of 14 · [Repo](https://github.com/chromedevtools/chrome-devtools-mcp) · [📖 Docs ↗](https://github.com/chromedevtools/chrome-devtools-mcp/blob/main/docs/tool-reference.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chrome-devtools-mcp/)</sub>

<a name="codebase-memory-mcp"></a>
### 🥉 [codebase-memory-mcp](https://github.com/deusdata/codebase-memory-mcp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · MIT · Oct 2026</sub>

**MCP server that indexes codebases into a queryable knowledge graph.**

A native C executable that parses repositories with tree-sitter (162 languages) into a persistent graph of functions, classes, call chains, HTTP routes and cross-service links, and exposes it through 17 MCP tools. It adds semantic search with bundled embeddings, Cypher-like queries, dead code detection, git diff impact mapping and a built-in 3D graph UI. Processing is local, and `install` configures detected coding-agent clients.

- **+** Runs locally with no API key, hosted service or language runtime
- **+** Bundled embeddings enable semantic search without Ollama or Docker
- **+** Covers 162 languages; Hybrid LSP type resolution for 10 of them
- **+** Releases are VirusTotal-scanned and SLSA 3 attested
- **−** Updates require re-running the install script; `update` only prints the command
- **−** Defender may flag release binaries as a false positive, per the README
- **−** All active processes must share the exact same build and cache root
- **−** Watcher covers only git projects opened in MCP sessions, by default

<sub>no GPU · Models: nomic-embed-code (bundled, int8, 768d) · port 9749 · safety checks passed 10 of 13 · [Repo](https://github.com/deusdata/codebase-memory-mcp) · [📖 Docs ↗](https://github.com/DeusData/codebase-memory-mcp/blob/main/docs/CONFIGURATION.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codebase-memory-mcp/)</sub>

<a name="github-mcp-server"></a>
### #&#8288;4 [github-mcp-server](https://github.com/github/github-mcp-server) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

**MCP server exposing GitHub repos, issues, PRs and Actions to AI tools.**

Official GitHub MCP server, written in Go, that lets MCP hosts read code, manage issues and pull requests, inspect Actions runs and review security alerts. It runs either as a GitHub-hosted remote endpoint (api.githubcopilot.com/mcp/) or locally over stdio via the ghcr.io Docker image or a binary built with go build. Authentication is OAuth or a personal access token.

- **+** Hosted remote endpoint needs no local install; local Docker image and Go build also available
- **+** Supports OAuth login or PAT; PAT takes precedence when set
- **+** Works with GitHub Enterprise Cloud (ghe.com) and Enterprise Server via GITHUB_HOST
- **+** Install guides for VS Code, Claude, Cursor, Windsurf, Zed, Codex and others
- **−** Enterprise Server is not supported by the remote server; local server only
- **−** Remote OAuth needs each host to configure a GitHub App or OAuth App
- **−** Local Docker OAuth needs a fixed callback port (8085) published to loopback
- **−** Only talks to GitHub; no other forges or providers

<sub>no GPU · Docker · Needs GitHub API, Docker (optional) · safety checks passed 10 of 11 · [Repo](https://github.com/github/github-mcp-server) · [📖 Docs ↗](https://github.com/github/github-mcp-server/blob/main/docs/remote-server.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github-mcp-server/)</sub>

<a name="serena"></a>
### #&#8288;5 [serena](https://github.com/oraios/serena) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · custom license · Oct 2026</sub>

**MCP server giving coding agents symbol-level code search, editing and refactoring.**

Serena is an MCP server that gives a coding agent IDE-style tools: find symbol, find references, replace symbol body, rename, and a memory system. It uses language servers (over 40 languages) by default, or a paid JetBrains plugin that adds move, inline, type hierarchy and a debugger. It plugs into MCP clients such as Claude Code, Codex, Cursor and VSCode.

- **+** Symbol-level retrieval and editing instead of line numbers or text search
- **+** Language server backend is free and covers over 40 languages
- **+** Works with any MCP client, launched by command or run in HTTP mode
- **+** Layered YAML configuration: global, per-project, per-client contexts and modes
- **−** Move, inline, type hierarchy and debugging need the paid JetBrains plugin
- **−** Language server rename covers symbols only; some languages need extra installs
- **−** Application is GPL-3.0-or-later; only the SolidLSP component is MIT
- **−** Contributions require accepting a CLA

<sub>Docker + Compose · Needs uv, language servers (per language), JetBrains IDE plugin (optional, paid) · Models: Any LLM through MCP clients (Claude Code, Codex, Gemini-CLI, OpenCode, Cursor, VSCode, Claude Desktop) · [Repo](https://github.com/oraios/serena) · [📖 Docs ↗](https://oraios.github.io/serena/02-usage/000_intro.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serena/)</sub>

<a name="code-review-graph"></a>
### #&#8288;6 [code-review-graph](https://github.com/tirth8205/code-review-graph) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Python 3.10+, Tree-sitter, SQLite · Models: sentence-transformers (all-MiniLM-L6-v2), Google Gemini, MiniMax, Voyage AI, OpenAI-compatible endpoints · [Repo](https://github.com/tirth8205/code-review-graph) · [🌐 Site ↗](https://code-review-graph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-review-graph/)</sub>

<a name="context7"></a>
### #&#8288;7 [context7](https://github.com/upstash/context7) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 63k · MIT · Oct 2026</sub>

**Fetches current, version-specific library docs into coding agent prompts.**

Context7 looks up documentation and code examples for a named library and version, then returns them to the coding agent as context. It runs as an MCP server with two tools (resolve-library-id, query-docs) or as a ctx7 CLI plus skill. Setup is one command, npx ctx7 setup, which handles OAuth and API key generation. The hosted service at mcp.context7.com does the retrieval.

- **+** Two modes: MCP server, or ctx7 CLI with an installed skill
- **+** Library IDs like /vercel/next.js skip matching; version can be named in the prompt
- **+** npx ctx7 setup configures Cursor, Claude Code or opencode
- **+** Also ships a TypeScript SDK and Vercel AI SDK tools
- **−** API backend, parsing and crawling engines are private; repo has only the MCP server
- **−** Relies on the hosted service at mcp.context7.com; local run is a separate guide
- **−** Free API key recommended for higher rate limits; exact limits unknown
- **−** Docs are community-contributed; accuracy and security are not guaranteed

<sub>no GPU · Needs Node.js 18+, Context7 hosted API · safety checks passed 13 of 14 · [Repo](https://github.com/upstash/context7) · [📖 Docs ↗](https://context7.com/docs/clients/cli) · [🌐 Site ↗](https://context7.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context7/)</sub>

<a name="cli-anything"></a>
### #&#8288;8 [cli-anything](https://github.com/hkuds/cli-anything) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: patchy (43) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 52k · Apache-2.0 · Sep 2026</sub>

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

<sub>no GPU · Needs Python 3.10+, A supported AI coding agent (for generating new CLIs), Upstream apps the chosen CLI wraps (e.g. GIMP, Blender, LibreOffice) · safety checks passed 7 of 10 · [Repo](https://github.com/hkuds/cli-anything) · [📖 Docs ↗](https://arxiv.org/abs/2606.03854) · [🌐 Site ↗](https://hkuds.github.io/CLI-Anything/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-anything/)</sub>

<a name="claude-task-master"></a>
### #&#8288;9 [claude-task-master](https://github.com/eyaltoledano/claude-task-master) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (29) · Freshness: recent (77) · Maintenance: weak (4) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Apr 2026</sub>

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

<sub>no GPU · Needs Node.js, npm, AI provider API key or Claude Code/Codex CLI · Models: Anthropic, OpenAI, Google Gemini, Perplexity, xAI · [Repo](https://github.com/eyaltoledano/claude-task-master) · [📖 Docs ↗](https://tryhamster.com/docs/taskmaster) · [🌐 Site ↗](https://tryhamster.com/product/taskmaster) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-task-master/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
