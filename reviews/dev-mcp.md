# 🔌 MCP servers for developers reviews · Best of Vibe Coding

MCP servers that give coding agents tools: docs lookup, browsers, GitHub, databases and code navigation. Back to the [leaderboard](../README.md#-mcp-servers-for-developers).

<sub>🌐 Also on the web: [MCP servers for developers on archestack.com](https://archestack.com/best-of-vibe-coding/dev-mcp/), each project on its own page.</sub>

<a name="gitnexus"></a>
### 🥇 [gitnexus](https://github.com/abhigyanpatwari/gitnexus) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: very easy (83) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · custom license · Oct 2026</sub>

**Code knowledge graph exposed to coding agents through MCP tools.**

GitNexus indexes a repository with Tree-sitter into a LadybugDB graph of dependencies, call chains, clusters and execution flows. It serves that graph to agents such as Claude Code, Cursor and Codex through 19 MCP tools (impact, trace, query, rename, cypher and others), and installs skills and hooks. A browser Web UI offers graph exploration and chat.

- **+** Precomputes clusters and processes at index time, so impact returns callers and confidence in one call
- **+** One analyze command indexes, installs skills, registers Claude Code hooks and writes AGENTS.md/CLAUDE.md
- **+** setup auto-detects editors; Claude Code and Codex get MCP, skills and pre/post tool hooks
- **+** CLI indexing runs locally with native Tree-sitter and persistent LadybugDB storage
- **−** PolyForm Noncommercial license restricts commercial use
- **−** Web UI in-browser mode is limited to about 5k files
- **−** npx install can crash on npm 11; some grammars need a C++ toolchain or are skipped
- **−** Render deploy costs about $35/month and the token is the only access control

<sub>GPU optional · Docker + Compose · Needs Node.js, LadybugDB, Tree-sitter · Models: Claude Code, Cursor, Codex, Antigravity, Windsurf · [Repo](https://github.com/abhigyanpatwari/gitnexus) · [▶️ Demo ↗](https://gitnexus.vercel.app) · [🌐 Site ↗](https://gitnexus.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitnexus/)</sub>

<a name="codegraph"></a>
### 🥈 [codegraph](https://github.com/colbymchenry/codegraph) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (89) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 74k · MIT · Oct 2026</sub>

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

<sub>no GPU · safety checks passed 13 of 15 · [Repo](https://github.com/colbymchenry/codegraph) · [📖 Docs ↗](https://colbymchenry.github.io/codegraph/) · [🌐 Site ↗](https://getcodegraph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegraph/)</sub>

<a name="chrome-devtools-mcp"></a>
### 🥉 [chrome-devtools-mcp](https://github.com/chromedevtools/chrome-devtools-mcp) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js LTS, npm, Google Chrome (current stable) · safety checks passed 16 of 16 · [Repo](https://github.com/chromedevtools/chrome-devtools-mcp) · [📖 Docs ↗](https://github.com/chromedevtools/chrome-devtools-mcp/blob/main/docs/tool-reference.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chrome-devtools-mcp/)</sub>

<a name="codebase-memory-mcp"></a>
### #&#8288;4 [codebase-memory-mcp](https://github.com/deusdata/codebase-memory-mcp) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · MIT · Oct 2026</sub>

**Local MCP server that indexes code into a queryable knowledge graph.**

A native C MCP server that indexes functions, classes, imports and HTTP routes across 162 languages into a local graph, and exposes 17 tools (search, trace, impact analysis, Cypher queries, dead code detection) to coding agents such as Claude Code and Codex. Indexing and queries need no hosted service or API key. A browser UI, CBM Lens Beta, adds source reading, architecture maps and optional local chat, but it is only on main, not in v0.11.0.

- **+** Single native binary for macOS, Linux and Windows; no Docker, runtime or API key needed
- **+** 162 tree-sitter grammars compiled in; hybrid LSP type resolution for 13 languages
- **+** Reports Linux kernel (28M LOC) indexed in about 3 minutes
- **+** Installer configures 45 detected agent client surfaces automatically
- **−** CBM Lens Beta is only on main; the current release ships the older graph UI
- **−** Token savings (120x, 10x) come from the project's own benchmarks
- **−** Preprint reports lower answer quality than file-by-file exploration (83% vs 92%)
- **−** Installer rewrites agent configs and a shared daemon requires identical builds across sessions

<sub>no GPU · Needs Hugging Face (optional model download for Lens chat) · port 9749 · safety checks passed 12 of 15 · [Repo](https://github.com/deusdata/codebase-memory-mcp) · [📖 Docs ↗](https://github.com/DeusData/codebase-memory-mcp/blob/main/docs/CONFIGURATION.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codebase-memory-mcp/)</sub>

<a name="github-mcp-server"></a>
### #&#8288;5 [github-mcp-server](https://github.com/github/github-mcp-server) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs GitHub API, Docker (optional) · safety checks passed 13 of 14 · [Repo](https://github.com/github/github-mcp-server) · [📖 Docs ↗](https://github.com/github/github-mcp-server/blob/main/docs/remote-server.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github-mcp-server/)</sub>

<a name="serena"></a>
### #&#8288;6 [serena](https://github.com/oraios/serena) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · custom license · Oct 2026</sub>

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

<sub>Docker + Compose · Needs uv, language servers (per language), JetBrains IDE plugin (optional, paid) · Models: Any LLM through MCP clients (Claude Code, Codex, Gemini-CLI, OpenCode, Cursor, VSCode, Claude Desktop) · safety checks passed 11 of 13 · [Repo](https://github.com/oraios/serena) · [📖 Docs ↗](https://oraios.github.io/serena/02-usage/000_intro.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serena/)</sub>

<a name="code-review-graph"></a>
### #&#8288;7 [code-review-graph](https://github.com/tirth8205/code-review-graph) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Python 3.10+, Tree-sitter, SQLite · Models: sentence-transformers (all-MiniLM-L6-v2), Google Gemini, MiniMax, Voyage AI, OpenAI-compatible endpoints · safety checks passed 15 of 17 · [Repo](https://github.com/tirth8205/code-review-graph) · [🌐 Site ↗](https://code-review-graph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-review-graph/)</sub>

<a name="context7"></a>
### #&#8288;8 [context7](https://github.com/upstash/context7) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 63k · MIT · Oct 2026</sub>

**MCP server and CLI that fetch current library docs into coding-agent prompts.**

Context7 looks up version-specific documentation and code examples for a library and places them in the agent's context. It runs as an MCP server (tools resolve-library-id and query-docs) or as a ctx7 CLI plus a skill, with no MCP needed. The repo holds the MCP server, CLI and SDKs; the API backend, parsing and crawling engines are private.

- **+** Two modes: MCP server tools, or ctx7 CLI with an installed skill
- **+** One command, npx ctx7 setup, configures Cursor, Claude Code or OpenCode
- **+** Version-aware lookups; prompts can pin a library ID such as /vercel/next.js
- **+** Also ships a TypeScript SDK and Vercel AI SDK tools
- **−** API backend, parser and crawler are private; only client code is open
- **−** Depends on the hosted service at mcp.context7.com; local run is a separate guide
- **−** API key recommended for higher rate limits; the limits are not stated
- **−** Indexed docs are community-contributed; README gives no accuracy guarantee

<sub>no GPU · Needs Context7 hosted API (mcp.context7.com), Node.js 22.13+ for ctx7 CLI · safety checks passed 14 of 16 · [Repo](https://github.com/upstash/context7) · [📖 Docs ↗](https://context7.com/docs/resources/all-clients) · [🌐 Site ↗](https://context7.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context7/)</sub>

<a name="unity-mcp"></a>
### #&#8288;9 [unity-mcp](https://github.com/coplaydev/unity-mcp) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: some setup (33) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

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

<sub>Compose · Needs Unity 2021.3 LTS to 6.x, Python 3.10+, uv · Models: Any MCP client (Claude, Codex, Cursor, VS Code, Windsurf, Cline, Gemini CLI) · [Repo](https://github.com/coplaydev/unity-mcp) · [📖 Docs ↗](https://coplaydev.github.io/unity-mcp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unity-mcp/)</sub>

<a name="cli-anything"></a>
### #&#8288;10 [cli-anything](https://github.com/hkuds/cli-anything) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: patchy (43) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 53k · Apache-2.0 · Sep 2026</sub>

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

<sub>no GPU · Needs Python 3.10+, A supported AI coding agent (for generating new CLIs), Upstream apps the chosen CLI wraps (e.g. GIMP, Blender, LibreOffice) · safety checks passed 8 of 12 · [Repo](https://github.com/hkuds/cli-anything) · [📖 Docs ↗](https://arxiv.org/abs/2606.03854) · [🌐 Site ↗](https://hkuds.github.io/CLI-Anything/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-anything/)</sub>

<a name="artemis"></a>
### #&#8288;11 [artemis](https://github.com/google/artemis) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: patchy (39) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Sep 2026</sub>

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

<sub>Docker · Needs ADB, scrcpy, FFmpeg, uv, Python 3.12+, Android device or emulator with USB debugging · Models: Gemini, Claude, GPT-4o, Qwen-VL · port 8000 · [Repo](https://github.com/google/artemis) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/artemis/)</sub>

<a name="claude-task-master"></a>
### #&#8288;12 [claude-task-master](https://github.com/eyaltoledano/claude-task-master) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (51) · Freshness: recent (77) · Maintenance: weak (4) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Apr 2026</sub>

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

<sub>no GPU · Needs Node.js, npm, AI provider API key or Claude Code/Codex CLI · Models: Anthropic, OpenAI, Google Gemini, Perplexity, xAI · safety checks passed 11 of 16 · [Repo](https://github.com/eyaltoledano/claude-task-master) · [📖 Docs ↗](https://tryhamster.com/docs/taskmaster) · [🌐 Site ↗](https://tryhamster.com/product/taskmaster) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-task-master/)</sub>

<a name="figma-context-mcp"></a>
### #&#8288;13 [figma-context-mcp](https://github.com/glips/figma-context-mcp) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (38) · Freshness: active (94) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Jun 2026</sub>

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

<sub>no GPU · Needs Figma API, Figma personal access token, Node.js (npx) · [Repo](https://github.com/glips/figma-context-mcp) · [▶️ Demo ↗](https://youtu.be/6G9yb-LrEqg) · [📖 Docs ↗](https://www.framelink.ai/docs/quickstart) · [🌐 Site ↗](https://www.framelink.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/figma-context-mcp/)</sub>

<a name="claude-context"></a>
### #&#8288;14 [claude-context](https://github.com/zilliztech/claude-context) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (28) · Freshness: active (99) · Maintenance: weak (3) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Jul 2026</sub>

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

<sub>no GPU · Needs Node.js >= 20, Milvus or Zilliz Cloud, OpenAI API key (default embedding provider) · Models: OpenAI, VoyageAI, Ollama, Gemini · [Repo](https://github.com/zilliztech/claude-context) · [📖 Docs ↗](https://github.com/zilliztech/claude-context/tree/master/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-context/)</sub>

<a name="pal-mcp-server"></a>
### #&#8288;15 [pal-mcp-server](https://github.com/beehiveinnovations/pal-mcp-server) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (23) · Freshness: slowing (35) · Maintenance: weak (5) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Dec 2025</sub>

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

<sub>GPU optional · Docker + Compose · Needs Python 3.10+, Git, uv, Provider API key (Gemini, OpenAI, OpenRouter, Azure, X.AI, DIAL) or Ollama · Models: Gemini, OpenAI, Anthropic, Grok, Azure OpenAI · [Repo](https://github.com/beehiveinnovations/pal-mcp-server) · [📖 Docs ↗](https://github.com/BeehiveInnovations/pal-mcp-server/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pal-mcp-server/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
