# 🔌 MCP servers for developers reviews · Best of Vibe Coding

MCP servers that give coding agents tools: docs lookup, browsers, GitHub, databases and code navigation. Back to the [leaderboard](../README.md#-mcp-servers-for-developers).

<sub>🌐 Also on the web: [MCP servers for developers on archestack.com](https://archestack.com/best-of-vibe-coding/dev-mcp/), each project on its own page.</sub>

<a name="gitnexus"></a>
### 🥇 [gitnexus](https://github.com/abhigyanpatwari/gitnexus) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: very easy (83) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · custom license · Oct 2026</sub>

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
### 🥈 [codegraph](https://github.com/colbymchenry/codegraph) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 74k · MIT · Oct 2026</sub>

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

<a name="n8n-mcp"></a>
### 🥉 [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (93) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Oct 2026</sub>

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

<a name="serena"></a>
### #&#8288;4 [serena](https://github.com/oraios/serena) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · custom license · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs uv, language servers (per language), JetBrains IDE plugin (optional, paid) · Models: any MCP-capable client/LLM · safety checks passed 11 of 13 · [Repo](https://github.com/oraios/serena) · [📖 Docs ↗](https://oraios.github.io/serena/02-usage/000_intro.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serena/)</sub>

<a name="chrome-devtools-mcp"></a>
### #&#8288;5 [chrome-devtools-mcp](https://github.com/chromedevtools/chrome-devtools-mcp) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;6 [codebase-memory-mcp](https://github.com/deusdata/codebase-memory-mcp) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · MIT · Oct 2026</sub>

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

<sub>GPU optional · Models: Optional local model for CBM Lens chat, downloaded from Hugging Face · port 9749 · safety checks passed 12 of 15 · [Repo](https://github.com/deusdata/codebase-memory-mcp) · [📖 Docs ↗](https://github.com/DeusData/codebase-memory-mcp) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codebase-memory-mcp/)</sub>

<a name="github-mcp-server"></a>
### #&#8288;7 [github-mcp-server](https://github.com/github/github-mcp-server) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

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

<a name="code-review-graph"></a>
### #&#8288;8 [code-review-graph](https://github.com/tirth8205/code-review-graph) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Oct 2026</sub>

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

<a name="unity-mcp"></a>
### #&#8288;9 [unity-mcp](https://github.com/coplaydev/unity-mcp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: some setup (33) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

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

<a name="desktopcommandermcp"></a>
### #&#8288;10 [desktopcommandermcp](https://github.com/wonderwhy-er/desktopcommandermcp) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (77) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

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

<a name="context7"></a>
### #&#8288;11 [context7](https://github.com/upstash/context7) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 63k · MIT · Oct 2026</sub>

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

<a name="aos-ce"></a>
### #&#8288;12 [aos-ce](https://github.com/unicity-aos/aos-ce) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (82) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="ivanmurzak-unity-mcp"></a>
### #&#8288;13 [unity-mcp](https://github.com/ivanmurzak/unity-mcp) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="mobile-mcp"></a>
### #&#8288;14 [mobile-mcp](https://github.com/mobile-next/mobile-mcp) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · Apache-2.0 · Oct 2026</sub>

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

<a name="linkedin-mcp-server"></a>
### #&#8288;15 [linkedin-mcp-server](https://github.com/stickerdaniel/linkedin-mcp-server) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="repowise"></a>
### #&#8288;16 [repowise](https://github.com/repowise-dev/repowise) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · AGPL-3.0 · Oct 2026</sub>

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

<a name="dev-browser"></a>
### #&#8288;17 [dev-browser](https://github.com/sawyerhood/dev-browser) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (56) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · MIT · Sep 2026</sub>

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

<a name="agent-device"></a>
### #&#8288;18 [agent-device](https://github.com/callstack/agent-device) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

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

<a name="devspace"></a>
### #&#8288;19 [devspace](https://github.com/waishnav/devspace) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Sep 2026</sub>

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

<a name="google-workspace-mcp"></a>
### #&#8288;20 [google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="code2prompt"></a>
### #&#8288;21 [code2prompt](https://github.com/mufeedvh/code2prompt) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (37) · Freshness: active (89) · Maintenance: fair (53) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Sep 2026</sub>

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

<a name="artemis"></a>
### #&#8288;22 [artemis](https://github.com/google/artemis) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: patchy (39) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Sep 2026</sub>

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

<a name="mcp"></a>
### #&#8288;23 [mcp](https://github.com/awslabs/mcp) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="cursor-talk-to-figma-mcp"></a>
### #&#8288;24 [cursor-talk-to-figma-mcp](https://github.com/grab/cursor-talk-to-figma-mcp) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (34) · Freshness: active (100) · Maintenance: patchy (40) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Jul 2026</sub>

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

<a name="magic-mcp"></a>
### #&#8288;25 [magic-mcp](https://github.com/21st-dev/magic-mcp) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (69) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · ISC · Sep 2026</sub>

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

<a name="cli-anything"></a>
### #&#8288;26 [cli-anything](https://github.com/hkuds/cli-anything) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: patchy (42) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · Apache-2.0 · Sep 2026</sub>

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

<a name="figma-context-mcp"></a>
### #&#8288;27 [figma-context-mcp](https://github.com/glips/figma-context-mcp) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (65) · Freshness: active (93) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Jun 2026</sub>

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

<a name="claude-task-master"></a>
### #&#8288;28 [claude-task-master](https://github.com/eyaltoledano/claude-task-master) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: popular (74) · Freshness: recent (76) · Maintenance: weak (4) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Apr 2026</sub>

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

<a name="pal-mcp-server"></a>
### #&#8288;29 [pal-mcp-server](https://github.com/beehiveinnovations/pal-mcp-server) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (56) · Freshness: slowing (34) · Maintenance: weak (5) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Dec 2025</sub>

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

<a name="claude-context"></a>
### #&#8288;30 [claude-context](https://github.com/zilliztech/claude-context) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (59) · Freshness: active (98) · Maintenance: weak (3) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Jul 2026</sub>

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

<a name="git-mcp"></a>
### #&#8288;31 [git-mcp](https://github.com/idosal/git-mcp) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: known (44) · Freshness: recent (73) · Maintenance: weak (10) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · May 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
