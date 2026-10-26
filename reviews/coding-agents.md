# 🤖 Coding agents and AI editors reviews · Best of Vibe Coding

Agents, assistants and editors that read your repo, write code and run commands, including tools that turn designs and screenshots into code. Back to the [leaderboard](../README.md#-coding-agents-and-ai-editors).

<sub>🌐 Also on the web: [Coding agents and AI editors on archestack.com](https://archestack.com/best-of-vibe-coding/coding-agents/), each project on its own page.</sub>

<a name="claw-code"></a>
### 🥇 [claw-code](https://github.com/ultraworkers/claw-code) <sub>score [97](../README.md#-how-we-rank "Score 97/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 195k · MIT · Oct 2026</sub>

**Rust CLI coding agent harness using Anthropic and OpenAI-compatible APIs.**

Claw Code is a Rust implementation of the `claw` command-line coding agent, built from source with cargo. It runs one-shot prompts or interactive sessions using an API key, and the docs cover local OpenAI-compatible servers such as Ollama, llama.cpp and vLLM. The README describes the repo as an agent-managed exhibit, not the production project, and points to LazyCodex and Gajae-Code for real work.

- **+** `claw doctor` checks API key, model access and tool configuration after build
- **+** Docs cover local OpenAI-compatible providers: Ollama, llama.cpp, vLLM
- **+** Build steps documented for macOS, Linux and Windows PowerShell
- **+** MIT license; workspace test suite and deterministic mock-service parity harness
- **−** README says it is not the serious production project and points elsewhere
- **−** Build-from-source only; `cargo install claw-code` installs a deprecated stub
- **−** Requires an API key; Claude subscription login is not supported
- **−** No ACP/Zed daemon yet; `claw acp serve` only returns status

<sub>no GPU · Docker + Compose · Needs Rust toolchain (cargo), LLM API key · Models: Anthropic API, OpenAI-compatible APIs, Ollama, llama.cpp, vLLM · [Repo](https://github.com/ultraworkers/claw-code) · [📖 Docs ↗](https://github.com/ultraworkers/claw-code/blob/main/USAGE.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claw-code/)</sub>

<a name="codewhale"></a>
### 🥈 [codewhale](https://github.com/codewhale-hq/codewhale) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

**Terminal coding agent in Rust that works with 40+ model providers.**

Codewhale is a terminal coding agent that reads a repository, edits files and runs shell commands until a task is done or it needs input. It supports more than 40 built-in providers, any OpenAI-compatible endpoint, and local models through Ollama, vLLM or SGLang, with DeepSeek as the default. It also has a headless exec mode, a local web UI, a PR review command and an ACP server for editors.

- **+** /receipts lists changed files, commands run, web and MCP calls, and approvals
- **+** Plan, Work and Operate modes with Ask, Auto-Review and Full Access permissions
- **+** One engine behind the TUI, exec, local web UI, Runtime API and ACP over stdio
- **+** Reads AGENTS.md; opt-in import of CLAUDE.md and Cursor rules; supports MCP, skills, hooks
- **−** Telemetry is on by default; aggregate counts are sent until you disable it
- **−** No OS sandbox on Windows, and Full Access disables the sandbox everywhere
- **−** Some features, such as the one-step /undo and terminal workbar, are only in unreleased 0.10.2
- **−** exec --auto defaults to Full Access with no shell sandbox

<sub>GPU optional · Docker · Needs Git repository, Provider API key or local runtime (Ollama, vLLM, SGLang), bubblewrap (optional, Linux sandbox) · Models: DeepSeek, Anthropic, OpenAI, Google, Mistral · [Repo](https://github.com/codewhale-hq/codewhale) · [📖 Docs ↗](https://github.com/codewhale-hq/codewhale/blob/main/docs/README.md) · [🌐 Site ↗](https://codewhale.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codewhale/)</sub>

<a name="deepseek-reasonix"></a>
### 🥉 [deepseek-reasonix](https://github.com/esengine/deepseek-reasonix) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

**Coding agent for terminal, desktop, browser and editors, with a DeepSeek preset.**

Reasonix is a Go coding agent that reads a project folder, edits files, and runs commands and tests, showing each step. It ships as a desktop app (Studio), a terminal UI, a local web interface via `reasonix web`, and an ACP backend for editors. Providers are declared in `reasonix.toml`; DeepSeek is a built-in preset and any OpenAI-compatible endpoint is a config entry.

- **+** Desktop, TUI, web and ACP editor front ends share one local engine
- **+** Permission levels, plan mode and forbid rules that always apply
- **+** Rewind restores files changed by edit tools, per conversation turn
- **+** Static CGO-free Go binary, cross-compiled to six targets
- **−** Rewind does not cover changes made by shell commands
- **−** 2.x is moving quickly; 1.x is the stable line on older architecture
- **−** VS Code extension needs the 1.x CLI installed separately
- **−** Linux packages are download only, no package repository

<sub>no GPU · Needs Model provider API key, Go 1.25+ (build from source), Node 24+ and pnpm 10 (build Studio) · Models: DeepSeek (preset), OpenAI-compatible endpoints, MCP servers · [Repo](https://github.com/esengine/deepseek-reasonix) · [📖 Docs ↗](https://github.com/esengine/DeepSeek-Reasonix/blob/studio/docs/GUIDE.md) · [🌐 Site ↗](https://esengine.github.io/DeepSeek-Reasonix/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepseek-reasonix/)</sub>

<a name="t3code"></a>
### #&#8288;4 [t3code](https://github.com/pingdotgg/t3code) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Oct 2026</sub>

**Desktop, web and mobile front end for controlling local coding agent CLIs.**

T3 Code is a control surface for coding agents already installed and authenticated on your machine: Claude Code, Codex, Cursor, Grok Build, OpenCode and Google Antigravity. It runs a local server started with the `t3` command and is reached through a web app, an Electron desktop app, or iOS and Android apps for remote use. The README says the project is early and bugs are expected.

- **+** Drives six agent providers from one interface using your existing subscriptions
- **+** Clients for desktop (Electron), web, iOS and Android, with remote access to your machine
- **+** Installs via shell script, npx, winget, scoop, Homebrew, .deb or AUR
- **+** MIT licensed; can run as a background service with `t3 service install`
- **−** README says it is very early and to expect bugs
- **−** Mostly not accepting contributions; large features will not be merged
- **−** Needs at least one provider CLI installed and logged in beforehand
- **−** No docs site yet; docs are Markdown files in the repo

<sub>no GPU · Needs At least one of: Codex CLI, Claude Code, Cursor CLI, Grok Build CLI, OpenCode, Antigravity · Models: Claude Code, Codex, Cursor, Grok Build, OpenCode · [Repo](https://github.com/pingdotgg/t3code) · [▶️ Demo ↗](https://app.t3.codes) · [📖 Docs ↗](https://github.com/pingdotgg/t3code/tree/main/docs) · [🌐 Site ↗](https://t3.codes) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/t3code/)</sub>

<a name="pi"></a>
### #&#8288;5 [pi](https://github.com/earendil-works/pi) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 118k · MIT · Oct 2026</sub>

**Terminal coding agent with extensions, skills, and an SDK.**

Pi is a TypeScript coding agent CLI that runs in your project directory and connects to LLM providers through a login or API key. It is customized with extensions, skills, prompt templates and themes, shared as npm or git packages, and can be driven interactively, in print/JSON mode, over RPC, or through a TypeScript SDK. The monorepo also ships a multi-provider LLM API, an agent runtime and a terminal UI library.

- **+** Multiple interfaces: interactive CLI, print/JSON mode, RPC and a TypeScript SDK
- **+** Extensions, skills, prompt templates and themes ship as npm or git packages
- **+** Core libraries (pi-ai, pi-agent-core, pi-tui) are published as separate packages
- **+** Installer pins dependencies; Nix flake builds on Linux and macOS, ARM64 and x86-64
- **−** No built-in permission system; runs with the launching user's full permissions
- **−** Sub-agents and plan mode are intentionally omitted and must be added via packages
- **−** Requires Node.js 22.19 or newer
- **−** New contributors' issues and PRs are auto-closed by default

<sub>no GPU · Needs Node.js 22.19+, LLM provider API key or subscription · Models: OpenAI, Anthropic, Google · [Repo](https://github.com/earendil-works/pi) · [📖 Docs ↗](https://pi.dev/docs/latest) · [🌐 Site ↗](https://pi.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi/)</sub>

<a name="oh-my-openagent"></a>
### #&#8288;6 [oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 70k · custom license · Oct 2026</sub>

**Terminal coding agent with multi-model orchestration and git-backed memory.**

OmO installs a native `omo` command that runs a coding agent on senpi, a fork of pi. It supports sign-in to Claude, ChatGPT, Kimi and GLM subscriptions, a keyword (`ulw`, `mass ulw`) that fans a task out into a graph of parallel agents, and a memory layer stored as markdown in a git repository. Config lives in `~/.omo/omo.jsonc` with per-project overrides.

- **+** Per-model system prompts and subscription login for Claude, ChatGPT, Kimi and GLM
- **+** Memory stored as markdown in a git repo, with a cheap model advising the main agent
- **+** Native binary via install script, bun or npm; `omo setup` migrates from the OpenCode edition
- **+** Config, skills and prompts reload live; project .omo/omo.jsonc overrides user config
- **−** License is SUL-1.0, a non-standard license; check terms before commercial use
- **−** Primary install is a curl-pipe-to-bash script
- **−** README gives no RAM, GPU or system requirements
- **−** Reviews in the README are testimonials, not benchmarks

<sub>Needs Model provider account or API keys · Models: Claude, ChatGPT, Kimi, GLM · safety checks passed 10 of 12 · [Repo](https://github.com/code-yeongyu/oh-my-openagent) · [📖 Docs ↗](https://omo.dev/docs) · [🌐 Site ↗](https://omo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-openagent/)</sub>

<a name="goose"></a>
### #&#8288;7 [goose](https://github.com/aaif-goose/goose) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 56k · Apache-2.0 · Oct 2026</sub>

**Rust AI agent with desktop app, CLI and API, extended through MCP.**

goose is a general-purpose agent written in Rust that runs locally as a desktop app (macOS, Linux, Windows), a CLI, or an embeddable API. It connects to 15+ model providers, including Anthropic, OpenAI, Google, Ollama, OpenRouter, Azure and Bedrock, and to 70+ extensions over the Model Context Protocol. It is hosted by the Agentic AI Foundation at the Linux Foundation.

- **+** Desktop app, CLI and API from one Rust codebase
- **+** 15+ providers, including Ollama for local models
- **+** Can use existing Claude, ChatGPT or Gemini subscriptions via ACP
- **+** 70+ MCP extensions; custom distros with preset providers and branding
- **−** README gives no RAM, GPU or port requirements
- **−** CLI install is a curl-pipe-to-bash script
- **−** Scope is general-purpose, not focused solely on coding
- **−** README has no demo and little detail on the API

<sub>Docker · Needs LLM provider API key or ACP-linked subscription · Models: Anthropic, OpenAI, Google, Ollama, OpenRouter · [Repo](https://github.com/aaif-goose/goose) · [📖 Docs ↗](https://goose-docs.ai/docs/category/getting-started) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goose/)</sub>

<a name="archon"></a>
### #&#8288;8 [Archon](https://github.com/coleam00/archon) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

**YAML workflow engine that runs AI coding agents through fixed dev steps.**

Archon lets you define development processes (plan, implement, validate, review, PR) as YAML workflows in `.archon/workflows/`, mixing bash nodes with AI nodes, loops and approval gates. Each run gets its own git worktree. It runs from a CLI, web UI, Slack, Telegram, Discord or GitHub webhooks, using Claude, Codex or Pi, and ships an `sdlc` workflow pack.

- **+** Workflows are YAML committed to the repo, with repo files overriding bundled defaults
- **+** Each run gets its own git worktree, so parallel runs do not conflict
- **+** Deterministic bash nodes mix with AI nodes, loops and human approval gates
- **+** Ships sdlc pack: triage, investigate, plan, implement, review, validate, PR
- **−** Claude provider needs Claude Code installed separately; compiled binaries do not bundle it
- **−** Quick-install binary on x64 requires AVX2 CPUs
- **−** Visual workflow builder is labeled experimental and covers a bounded set of nodes
- **−** Sends anonymous telemetry events by default

<sub>no GPU · Docker + Compose · Needs Bun, Claude Code, GitHub CLI, SQLite or PostgreSQL · Models: Claude, Codex, Pi · [Repo](https://github.com/coleam00/archon) · [📖 Docs ↗](https://archon.diy/docs/) · [🌐 Site ↗](https://archon.diy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archon/)</sub>

<a name="opencode"></a>
### #&#8288;9 [opencode](https://github.com/anomalyco/opencode) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 222k · MIT · Oct 2026</sub>

**Terminal-based AI coding agent with build and plan modes.**

OpenCode is a coding agent that runs in the terminal, with a beta desktop app, and works on your repository. It ships two built-in agents switched with Tab: a full-access build agent and a read-only plan agent that denies edits and asks before running bash. A general subagent handles multistep searches and can be called with @general.

- **+** Read-only plan agent denies file edits and asks before bash commands
- **+** Installs via curl script, npm, Homebrew, pacman, mise or Nix
- **+** Desktop app builds for macOS, Windows and Linux (.deb, .rpm, AppImage)
- **+** MIT licensed, with a release published within the last week
- **−** README does not list supported model providers or local model options
- **−** Desktop app is labeled beta
- **−** README gives no hardware requirements; details are deferred to the docs
- **−** Two Homebrew formulas with different update cadence can confuse installs

<sub>[Repo](https://github.com/anomalyco/opencode) · [📖 Docs ↗](https://opencode.ai/docs) · [🌐 Site ↗](https://opencode.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencode/)</sub>

<a name="open-swe"></a>
### #&#8288;10 [Open SWE](https://github.com/langchain-ai/open-swe) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

**Agent that turns issues into pull requests, reviews PRs and monitors CI.**

Open SWE is a LangChain coding agent built on Deep Agents and LangGraph. It takes work from a dashboard, GitHub issues and PRs, Slack or Linear, implements changes in per-thread Linux sandboxes, and opens pull requests. It also reviews PRs, learns review preferences, and watches CI. The README says it is under active development and accepts no external issues or contributions.

- **+** Covers the full loop: implement, open PR, review, CI monitoring via /baby-sit, and follow-ups
- **+** Triggers from dashboard, GitHub, Slack, and Linear (via MCP)
- **+** Models, sandbox provider, skills, and MCP servers are configurable; local execution is supported
- **+** Persistent per-thread sandboxes reuse context; independent threads run in parallel
- **−** Deploying as-is requires Managed Deep Agents; otherwise the README advises forking and adapting
- **−** Breaking changes expected; no stability or compatibility guarantees
- **−** Not accepting issues or external contributions
- **−** Sandboxes normally get installation-wide GitHub App access; approvals only guard detected Git pushes

<sub>Docker + Compose · Needs Managed Deep Agents, LangSmith, GitHub App, Slack, Linear · [Repo](https://github.com/langchain-ai/open-swe) · [📖 Docs ↗](https://github.com/langchain-ai/open-swe/blob/main/docs/INSTALLATION.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-swe/)</sub>

<a name="cmux"></a>
### #&#8288;11 [cmux](https://github.com/manaflow-ai/cmux) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Oct 2026</sub>

**Native macOS terminal with vertical tabs and alerts for parallel coding agents.**

cmux is a Swift/AppKit macOS terminal built on libghostty. Its sidebar shows git branch, PR status, working directory and listening ports per workspace, and panes get a ring when an agent needs input, triggered by OSC 9/99/777 sequences or `cmux notify`. It also embeds a scriptable browser pane, SSH workspaces, and a CLI and socket API for automation.

- **+** Works with any agent that runs in a terminal, including Claude Code, Codex and OpenCode
- **+** Native Swift/AppKit app rather than Electron; reads existing Ghostty config
- **+** CLI and socket API to create workspaces, split panes, send keystrokes and drive the browser
- **+** Session restore with agent resume via hooks for Claude Code, Codex, OpenCode and others
- **−** macOS only; no Linux or Windows build
- **−** Agent resume needs hooks installed per agent with `cmux hooks setup`
- **−** Live process state is not restored unless you opt into local tmux or zellij
- **−** iOS companion app is beta, with early access tied to the Founders Edition

<sub>Needs macOS · [Repo](https://github.com/manaflow-ai/cmux) · [▶️ Demo ↗](https://www.youtube.com/watch?v=i-WxO5YUTOs) · [📖 Docs ↗](https://cmux.com/docs/getting-started) · [🌐 Site ↗](https://cmux.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cmux/)</sub>

<a name="paseo"></a>
### #&#8288;12 [paseo](https://github.com/getpaseo/paseo) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Oct 2026</sub>

**Desktop, mobile and CLI client that runs many coding agents in parallel worktrees.**

Paseo runs a local daemon that manages coding agent CLIs (Claude Code, Codex, Copilot, OpenCode, Pi, Antigravity, Muse Code) and exposes them to Electron desktop, Expo mobile and web clients and a `paseo` CLI. Each agent can work in its own git worktree, with diffs, terminals, pull requests and a built-in browser in one window. It also ships a TypeScript SDK, a plugin system and orchestration skills.

- **+** One interface over seven agent CLIs, with provider and model chosen per task
- **+** Each agent can run in its own git worktree, many in parallel
- **+** Same app on desktop, iOS, Android, web and CLI, plus a TypeScript SDK
- **+** No telemetry or forced login; optional end-to-end encrypted relay for pairing
- **−** Requires at least one agent CLI installed and configured with your own credentials
- **−** Docker image needs extending with the agent CLIs you use
- **−** Plugins run with access to the daemon machine; only trusted code should be installed
- **−** Maintained by one person, per the README

<sub>no GPU · Docker + Compose · Needs Claude Code, Codex, Copilot, OpenCode, Pi, Antigravity or Muse Code CLI (at least one), Node.js/npm for CLI install · Models: Claude Code, Codex, GitHub Copilot, OpenCode, Pi · port 6767 · [Repo](https://github.com/getpaseo/paseo) · [📖 Docs ↗](https://paseo.sh/docs) · [🌐 Site ↗](https://paseo.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/paseo/)</sub>

<a name="openchamber"></a>
### #&#8288;13 [OpenChamber](https://github.com/openchamber/openchamber) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Workspace for running and reviewing OpenCode agent sessions on desktop, web and mobile.**

OpenChamber is a front end for OpenCode coding agents, shipped as a desktop app (macOS, Windows, Linux), a web/PWA server via CLI, a VS Code extension, and iOS/Android clients. It adds session goals, multi-model parallel runs with optional worktrees, guided diff walkthroughs, an in-app preview, GitHub issue and PR context, and scheduled prompts.

- **+** Multi-run sends one task to up to five models, each in its own session or worktree
- **+** Same projects and sessions reachable from desktop, web/PWA, VS Code, iOS and Android
- **+** Remote access via QR-paired Private Relay, tunnels, LAN/VPN or SSH, without opening ports
- **+** Desktop build bundles the OpenCode CLI, so no separate install
- **−** CLI/Web and VS Code need a separately installed OpenCode CLI
- **−** Agent runtime is OpenCode only
- **−** CLI/Web install requires Node.js 24.14+
- **−** Feature changes must go through an Ideas discussion before a PR

<sub>no GPU · Docker + Compose · Needs OpenCode CLI, Node.js 24.14+ · Models: OpenCode providers · [Repo](https://github.com/openchamber/openchamber) · [📖 Docs ↗](https://github.com/openchamber/openchamber/blob/main/packages/docs/content/docs/quickstart.mdx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openchamber/)</sub>

<a name="qwen-code"></a>
### #&#8288;14 [qwen-code](https://github.com/qwenlm/qwen-code) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent for Qwen and other models, with IDE, desktop and chat clients.**

Qwen Code is a Node.js CLI coding agent, started with `qwen`, that reads a repository, edits files and runs commands. It talks to OpenAI, Anthropic, Gemini and Qwen APIs, or local models via Ollama or vLLM, and can switch providers at runtime. It also offers VS Code, Zed and JetBrains integrations, a desktop app, an experimental web UI and daemon, TypeScript, Python and Java SDKs, and Telegram, DingTalk, WeChat and Feishu channels.

- **+** Supports OpenAI, Anthropic, Gemini and Qwen APIs plus Ollama or vLLM, switchable at runtime
- **+** Headless `qwen -p` mode and TypeScript, Python and Java SDKs for scripts and CI
- **+** Includes SubAgents, MCP, hooks, plan mode, sandbox and git worktrees
- **+** IDE plugins for VS Code, Zed and JetBrains, plus chat channels and a desktop app
- **−** Web UI and `qwen serve` daemon are marked experimental
- **−** Requires Node.js 22+ when installed through npm
- **−** Install script is fetched from an Alibaba Cloud OSS bucket and piped to a shell
- **−** Parity claims with Claude Code come from the project's own comparison report

<sub>no GPU · Docker · Needs Node.js 22+ (npm install), LLM provider API key or local model server · Models: Qwen, OpenAI, Anthropic, Gemini, Ollama · [Repo](https://github.com/qwenlm/qwen-code) · [📖 Docs ↗](https://qwenlm.github.io/qwen-code-docs/en/users/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qwen-code/)</sub>

<a name="claudian"></a>
### #&#8288;15 [claudian](https://github.com/yishentu/claudian) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

**Obsidian plugin that runs coding agents like Claude Code and Codex in your vault.**

Claudian is an Obsidian desktop plugin that embeds existing coding-agent CLIs (Claude Code, Codex, Grok Build, OpenCode, Pi, DeepSeek Harness) in a chat sidebar, with the vault as the agent's working directory. Agents read, write, search and run commands in notes. It adds inline edit with diff preview, slash commands and skills, @mentions, MCP via each CLI's config, and cross-session messaging.

- **+** Supports six agent harnesses behind one UI, with model lists discovered from each provider
- **+** Inline edit with word-level diff preview directly in notes
- **+** Sessions can message, steer or start other sessions on any provider
- **+** README states no telemetry; network use limited to provider and MCP calls
- **−** Requires at least one separately installed agent CLI plus a subscription or API provider
- **−** Desktop only; needs Obsidian 1.13.0 or newer
- **−** Pull requests that add new providers are not accepted
- **−** Windows needs specific CLI paths; .cmd and .ps1 wrappers are not recommended

<sub>no GPU · Needs Obsidian 1.13.0+, Claude Code, Codex, Grok Build, OpenCode, Pi or DeepSeek Harness CLI, Node.js for npm-installed CLIs · Models: Claude (Anthropic), Codex (OpenAI), Grok (xAI), OpenCode providers, Pi · [Repo](https://github.com/yishentu/claudian) · [🌐 Site ↗](https://community.obsidian.md/plugins/realclaudian) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claudian/)</sub>

<a name="openhands"></a>
### #&#8288;16 [OpenHands](https://github.com/openhands/openhands) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 92k · MIT · Oct 2026</sub>

**Web control center for running and automating multiple coding agents.**

Agent Canvas is a TypeScript web UI that starts conversations with coding agents and connects to one or more Agent Server backends (local, Docker, VM or OpenHands Cloud). It runs the OpenHands agent by default and can drive Claude Code, Codex, Gemini CLI, Pi, OpenCode or any ACP-compatible agent. A paired automation server runs agents on a schedule or from webhooks such as Slack, GitHub and Linear.

- **+** Switches between local, remote and cloud Agent Server backends from one frontend
- **+** Supports OpenHands plus Claude Code, Codex, Gemini, Pi, OpenCode and any ACP agent
- **+** Scheduled and webhook-triggered automations with Slack, GitHub and Linear integrations
- **+** Optional per-conversation Docker containers isolate concurrent agents
- **−** Default npm and source installs give the agent full filesystem access on the host
- **−** Needs Node.js 24+ and uv for non-Docker installs
- **−** Logic is split across four repositories, which complicates contributing and debugging
- **−** Internet-facing use needs manual hardening per the self-hosting guide

<sub>no GPU · Docker · Needs Node.js 24+, uv, Docker (optional), OpenHands Agent Server, Automation Server (optional) · Models: Any LLM via LLM profiles, OpenHands, Claude Code, Codex, Gemini CLI · port 8000 · [Repo](https://github.com/openhands/openhands) · [📖 Docs ↗](https://docs.openhands.dev/openhands/usage/agent-canvas/backends) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openhands/)</sub>

<a name="herdr"></a>
### #&#8288;17 [herdr](https://github.com/herdrdev/herdr) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · Apache-2.0 · Oct 2026</sub>

**Terminal multiplexer that keeps coding agents running and shows which are blocked.**

herdr is a Rust terminal multiplexer for running several coding agents such as Claude Code, Codex, Cursor and opencode. A background server keeps panes alive when the client detaches or SSH drops, and each pane is marked working, blocked or idle. Agents can also drive it through a CLI and socket API, and saved SSH machines appear in the same window.

- **+** Panes keep running in a background server after detach or SSH disconnect
- **+** Per-pane working, blocked or idle status across local and saved SSH machines
- **+** Agents can spawn panes and prompt each other via CLI and socket API
- **+** Single Rust binary; installs via curl script, Homebrew, mise or PowerShell
- **−** After a server or machine restart, processes are lost; only layout and supported agent sessions resume
- **−** Resume works only for supported agents; the README does not list which
- **−** Windows support is described as beta in the docs link
- **−** Install is a curl-pipe-to-shell script by default

<sub>no GPU · [Repo](https://github.com/herdrdev/herdr) · [📖 Docs ↗](https://herdr.dev/docs/) · [🌐 Site ↗](https://herdr.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/herdr/)</sub>

<a name="agent-orchestrator"></a>
### #&#8288;18 [agent-orchestrator](https://github.com/orchestratorinc/agent-orchestrator) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Oct 2026</sub>

**Desktop app that runs coding agents in parallel worktrees with a Kanban view.**

Orchestrator.inc is a local desktop app with a background daemon that runs one coding agent per task, each in its own Git branch and worktree. A project-level orchestrator agent can split a plan into tasks and spawn workers. A Kanban board tracks each worker's session, pull request, CI and review state, and sends failures or review comments back to the owning agent.

- **+** Each Git-backed worker gets its own branch and worktree, avoiding branch collisions
- **+** Supports many agent CLIs, including Claude Code, Codex, Cursor, Aider, Gemini CLI and Goose
- **+** Kanban status is derived from session, PR, CI and review state
- **+** Installers for macOS, Windows and Linux (AppImage, deb, rpm); no CLI needed to start
- **−** Worker, Chat and reviewer support differs per agent; a capability matrix is linked
- **−** Agent CLIs must be installed and set up separately
- **−** macOS builds may trigger a Gatekeeper warning and need a manual Open
- **−** No Docker or server deployment; it is a local desktop workspace

<sub>no GPU · Needs Git, Coding agent CLIs · Models: Claude Code, Codex, Cursor, opencode, Aider · [Repo](https://github.com/orchestratorinc/agent-orchestrator) · [📖 Docs ↗](https://docs.orchestrator.inc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-orchestrator/)</sub>

<a name="orca"></a>
### #&#8288;19 [orca](https://github.com/stablyai/orca) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 106k · MIT · Oct 2026</sub>

**Desktop app that runs multiple CLI coding agents in parallel git worktrees.**

Orca is a desktop app for macOS, Windows and Linux that runs CLI coding agents such as Claude Code, Codex and OpenCode side by side, each in its own git worktree. It adds terminal splits, an embedded browser for sending UI elements into prompts, GitHub and Linear task views, diff annotation, SSH worktrees and a mobile companion app. A CLI lets agents script Orca itself.

- **+** Works with any CLI agent that runs in a terminal; 30+ are listed by name
- **+** Each agent gets an isolated git worktree, so parallel runs can be compared and merged
- **+** SSH worktrees run agents, editing and terminals on a remote machine
- **+** Builds for macOS, Windows and Linux, plus iOS and Android companion apps
- **−** Does not include an agent or model; CLI agents are installed and paid for separately
- **−** Collects anonymous usage telemetry; opt-out is described in the docs
- **−** Mobile companion depends on a relay to pair with the desktop host
- **−** README gives no RAM or system requirements

<sub>no GPU · Needs git, CLI coding agents (Claude Code, Codex, OpenCode, etc.) · Models: Claude Code, Codex, OpenCode, Pi, Cursor · [Repo](https://github.com/stablyai/orca) · [📖 Docs ↗](https://www.onorca.dev/docs/cli/overview) · [🌐 Site ↗](https://onorca.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orca/)</sub>

<a name="cline"></a>
### #&#8288;20 [cline](https://github.com/cline/cline) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 71k · Apache-2.0 · Oct 2026</sub>

**Coding agent for VS Code, JetBrains, terminal and desktop, with an SDK.**

Cline is a coding agent that edits files across a project and runs shell commands, reacting to their output, with approval prompts for each edit and command. It ships as a CLI, VS Code extension, JetBrains plugin, macOS/Windows desktop app and a Node.js SDK built on the same engine. It works with Anthropic, OpenAI, Gemini, Bedrock, Vertex, OpenRouter, Ollama, LM Studio and any OpenAI-compatible endpoint.

- **+** Plan and Act modes, with per-edit and per-command approval or optional auto-approve
- **+** Supports many providers, including local models via Ollama and LM Studio
- **+** Headless CLI takes piped input and emits JSON for CI/CD scripts
- **+** SDK, MCP servers, .clinerules, multi-agent teams and cron-scheduled agents for extension
- **−** JetBrains plugin source is not open-sourced
- **−** Diff review and checkpoints are described only for VS Code and JetBrains
- **−** Desktop app is macOS and Windows only
- **−** Needs a provider API key or local model server; no bundled model

<sub>no GPU · Needs Node.js (npm), LLM provider API or local model server · Models: Anthropic, OpenAI, Google Gemini, OpenRouter, Vercel AI Gateway · [Repo](https://github.com/cline/cline) · [📖 Docs ↗](https://docs.cline.bot) · [🌐 Site ↗](https://cline.bot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cline/)</sub>

<a name="prime-agent"></a>
### #&#8288;21 [prime-agent](https://github.com/primeintellect-ai/prime-agent) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Oct 2026</sub>

**Terminal coding and research agent built around a persistent Python REPL.**

Prime Agent is a Rust terminal agent that reads and edits a working directory, runs commands, and does its work through a persistent Python REPL. Subagents are spawned with rlm.spawn(), and sessions run under a daemon so they survive terminal disconnects. The /refine command stores small, reviewable updates to prompts, memories and skills, with rollback snapshots.

- **+** Daemon-backed sessions keep running after the terminal detaches and can be reattached
- **+** Built-in subagents via rlm.spawn(), plus direct messaging between running agents
- **+** Long-task controls: /goal, heartbeats, schedules, and bounded /autonomous mode with quality gates
- **+** /refine records harness changes as snapshots and leaves the base system prompt untouched
- **−** Not a sandbox: model-generated Python and commands run with your user permissions
- **−** Installed through a curl-pipe-to-shell script; no Docker image is provided
- **−** GitHub detects the license as NOASSERTION, though the README says MIT
- **−** Needs a subscription or API-key provider via /login; supported models are not listed

<sub>no GPU · Needs Subscription or API-key model provider · Models: prime-inference provider, Subscription or API-key providers via /login · [Repo](https://github.com/primeintellect-ai/prime-agent) · [🌐 Site ↗](https://primeintellect.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/prime-agent/)</sub>

<a name="omnigent"></a>
### #&#8288;22 [omnigent](https://github.com/omnigent-ai/omnigent) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

**Orchestration layer that runs Claude Code, Codex, Cursor and other coding agents together.**

Omnigent is a Python CLI and server that wraps coding-agent harnesses (Claude Code, Codex, Cursor, OpenCode, Hermes, Pi, plus YAML-defined custom agents) behind one session model. Sessions can mix agents, be shared with teammates, and be opened from terminal, a web UI on port 6767, a phone, or a macOS desktop app. It adds approval and spend policies and can run sessions in cloud sandboxes such as Modal, E2B, Daytona or Kubernetes. The project is marked alpha.

- **+** Mixes several agent harnesses in one session, e.g. one agent reviewing another's diff
- **+** Policies for approval prompts, spend caps and tool limits at server, agent or chat scope
- **+** Supports API keys, Claude/ChatGPT subscriptions and OpenAI/Anthropic-compatible gateways like Ollama
- **+** Many sandbox backends: Modal, Daytona, E2B, Kubernetes, Databricks and others via extras
- **−** Marked alpha status in the README
- **−** Native terminal wrappers need tmux; Linux also requires bubblewrap
- **−** Windows runs degraded: no terminal wrappers and no filesystem or network sandboxing
- **−** Needs Python 3.12+, Node 22+, uv and git, so the install footprint is large

<sub>no GPU · Docker + Compose · Needs Python 3.12+, uv, git, Node.js 22+, pnpm, tmux, bubblewrap (Linux) · Models: Anthropic API, OpenAI API, Claude subscription, ChatGPT subscription, OpenRouter · port 6767 · [Repo](https://github.com/omnigent-ai/omnigent) · [📖 Docs ↗](https://omnigent.ai/quickstart/install) · [🌐 Site ↗](https://omnigent.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omnigent/)</sub>

<a name="gemini-cli"></a>
### #&#8288;23 [gemini-cli](https://github.com/google-gemini/gemini-cli) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 108k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent that runs Gemini models against your local codebase.**

Gemini CLI is a TypeScript terminal agent that sends prompts to Gemini models and can read and edit files, run shell commands, and fetch web pages. It supports MCP servers, custom commands, GEMINI.md context files, and a non-interactive mode with JSON and stream-JSON output for scripts. The README notes it is not optimized for the latest Gemini models and that unpaid-tier and Google One users were moved to Antigravity CLI on June 18th, 2026.

- **+** Headless mode with --output-format json and stream-json for scripting and automation
- **+** Extensible through MCP servers in ~/.gemini/settings.json and custom extensions
- **+** Three auth routes: Google login, Gemini API key, or Vertex AI
- **+** Installs via npx, npm, Homebrew, MacPorts or conda; weekly preview and stable channels plus nightly
- **−** Gemini models only; no other model providers are listed in the README
- **−** README says it is not optimized for the latest Gemini models, including Gemini 4 Argon
- **−** Unpaid-tier and Google One users were replaced by Antigravity CLI on June 18th, 2026
- **−** Preview and nightly releases may contain regressions

<sub>no GPU · Docker · Needs Node.js, Gemini API key, Google account, or Vertex AI · Models: Gemini · [Repo](https://github.com/google-gemini/gemini-cli) · [📖 Docs ↗](https://geminicli.com/docs/) · [🌐 Site ↗](https://www.geminicli.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-cli/)</sub>

<a name="openinterpreter"></a>
### #&#8288;24 [openinterpreter](https://github.com/openinterpreter/openinterpreter) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 69k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent, a Codex fork tuned for low-cost models.**

Open Interpreter is a Rust fork of OpenAI's Codex that runs as a terminal coding agent. It can emulate other agent harnesses (claude-code, kimi-code, qwen-code, swe-agent and others) via /harness, so cheaper models are driven the way their providers recommend. It also runs as an ACP agent for editors and accepts the Codex exec protocol.

- **+** Switchable harness emulation: native, claude-code, kimi-code, qwen-code, swe-agent, minimal and more
- **+** Runs under native sandboxing on macOS, Linux and Windows
- **+** Works as an ACP agent via `interpreter acp`; Codex SDK users can swap the binary
- **+** Reads shared AGENTS.md and .agents/skills; supports MCP, hooks and permissions
- **−** Rewrite of the original Python project, which is now only a community fork
- **−** Built-in computer use relies on external tools: agent-browser and trycua
- **−** README gives no RAM, GPU or supported-model minimums
- **−** Install is a curl or PowerShell pipe-to-shell script; no Docker image

<sub>Needs agent-browser, trycua · Models: OpenAI-compatible Chat Completions providers, Kimi K3, DeepSeek, Z.AI GLM · [Repo](https://github.com/openinterpreter/openinterpreter) · [📖 Docs ↗](https://www.openinterpreter.com/docs/terminal) · [🌐 Site ↗](https://www.openinterpreter.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openinterpreter/)</sub>

<a name="openclaude"></a>
### #&#8288;25 [openclaude](https://github.com/twigpine/openclaude) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Oct 2026</sub>

**Terminal coding-agent CLI for OpenAI-compatible, Gemini, Codex and Ollama backends.**

OpenClaude is a TypeScript coding-agent CLI installed from npm (Node.js 22 or newer). It provides bash, file, grep, glob, agent, task, MCP and web tools with slash commands and streaming output. You switch between cloud and local model providers with `/provider` and saved profiles. It also has background sessions, session resume and fork, and a bundled VS Code extension.

- **+** Many providers: OpenAI-compatible /v1 servers, Gemini, GitHub Models, Codex OAuth, Ollama, Atomic Chat
- **+** Guided `/provider` setup with saved profiles instead of per-provider tooling
- **+** Background sessions via `--bg`, `ps`, `logs`, `kill`; conversations can be resumed or forked
- **+** Runs against local Ollama with no API key
- **−** License detected as NOASSERTION, while the README badge says MIT
- **−** `openclaude attach` does not reattach a terminal yet; it only points to logs
- **−** Fork branches conversation history only, with no filesystem or worktree isolation
- **−** Project .env files are not loaded; needs `--provider-env-file` or exported variables

<sub>GPU optional · Docker · Needs Node.js >=22, ripgrep, Bun (source builds only) · Models: OpenAI-compatible APIs, Gemini, GitHub Models, Codex, Ollama · [Repo](https://github.com/twigpine/openclaude) · [🌐 Site ↗](https://twigpine.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openclaude/)</sub>

<a name="jcode"></a>
### #&#8288;26 [jcode](https://github.com/1jehuang/jcode) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

**Rust terminal coding agent built to run many parallel sessions with low RAM.**

jcode is a Rust coding agent for the terminal that manages multiple agent sessions through a shared server. Agents in the same repo get notified when another agent edits a file they have read, and can message each other or spawn worker agents. It supports many providers, including Claude OAuth and OpenAI Codex OAuth, and has a self-dev mode where the agent edits and reloads its own source.

- **+** README benchmark: about 3.3 MB per additional headless session, versus 169 MB for Claude Code
- **+** Reported 19.1 ms time to first input; benchmark script is linked for reproduction
- **+** Server-managed swarm: file-change notices and DMs or broadcasts between agents in one repo
- **+** Supports Claude and OpenAI Codex OAuth plus other providers listed in the docs
- **−** Install is a curl-pipe-to-bash script; README documents only macOS and Linux
- **−** Self-dev mode lets the agent rewrite its own binary; the README has no safeguards section
- **−** Benchmark figures come from the author; the README compares against other tools without method detail
- **−** README leaves the self-dev writeup as a placeholder

<sub>no GPU · Models: Claude (OAuth), OpenAI Codex (OAuth), other providers listed in docs · [Repo](https://github.com/1jehuang/jcode) · [📖 Docs ↗](https://jcode.sh/docs) · [🌐 Site ↗](https://jcode.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jcode/)</sub>

<a name="atlas"></a>
### #&#8288;27 [atlas](https://github.com/pacifio/atlas) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · Apache-2.0 · Oct 2026</sub>

**Desktop app that links each git commit to the agent session behind it.**

Atlas is a Tauri desktop app (Rust backend) that runs Claude Code, Codex, its own native agent and ACP-registry agents side by side on one codebase. It records each session locally in SQLite and links commits to the session that produced them as checkpoints. A shared on-device memory index feeds context to every agent, so switching agents mid-task keeps the history.

- **+** Checkpoints link commits to prompts, tool calls and file changes, and survive amend and rebase
- **+** Shared memory lets Claude Code and Codex see each other's decisions, using on-device embeddings
- **+** Local by default: sessions in .atlas/sessions.db, secrets scrubbed before write, no account needed
- **+** Notes are markdown, sessions JSONL, so data stays usable outside the app
- **−** Officially supports only macOS 13+ and Windows 10+ x64; Linux is untested
- **−** Anonymous usage analytics are on by default and must be turned off
- **−** QA on long-tail ACP registry agents is still ongoing
- **−** Claude Code use requires installing the separate claude CLI

<sub>no GPU · Needs Bun and Rust (build from source), claude CLI (for Claude Code agent), SQLite (bundled checkpoint store) · Models: Claude Code, Codex, Atlas native agent, ACP registry agents (Cursor, OpenCode, Kilo Code) · [Repo](https://github.com/pacifio/atlas) · [📖 Docs ↗](https://docs.tryatlas.cc/) · [🌐 Site ↗](https://www.tryatlas.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/atlas/)</sub>

<a name="superplane"></a>
### #&#8288;28 [superplane](https://github.com/superplanehq/superplane) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · custom license · Oct 2026</sub>

**Workflow engine that sends backlog issues to coding agents and returns reviewed PRs.**

SuperPlane coordinates coding agents, source control, CI, review and approvals around a work-order model: an issue enters a backlog, passes through ordered automation lines, and ends as a pull request or other artifact. Automations are composed on a Canvas using integrations such as GitHub, GitLab, Claude, Cursor, OpenAI, Semaphore and Slack. Failed runs are sent back to the agent with context and can resume from preserved state.

- **+** Integrations cover GitHub, GitLab, Bitbucket, several CI systems, Claude, Cursor and OpenAI
- **+** Event history and execution state persist across retries, so failed runs can resume
- **+** Approval steps and shared guardrails apply to every run
- **+** Model choice is open, with cloud or on-prem deployment
- **−** README gives no install steps, RAM or port figures for self-hosting
- **−** Contributor setup is Docker-based; production deployment docs are not described in the README
- **−** Automatic selection of high-confidence issues is described without detail on how it works
- **−** Detected license is NOASSERTION, though the README states Apache 2.0

<sub>Docker + Compose · Needs Docker, GitHub or GitLab, coding agent provider (Claude, Cursor, OpenAI) · Models: Claude, Cursor, OpenAI, OpenRouter, Perplexity · [Repo](https://github.com/superplanehq/superplane) · [📖 Docs ↗](https://docs.superplane.com/) · [🌐 Site ↗](https://superplane.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superplane/)</sub>

<a name="codecompanion-nvim"></a>
### #&#8288;29 [codecompanion.nvim](https://github.com/olimorris/codecompanion.nvim) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · Apache-2.0 · Oct 2026</sub>

**Neovim plugin for chatting with LLMs and ACP coding agents.**

CodeCompanion adds a chat buffer, inline code transformations and an action palette to Neovim, backed by HTTP adapters for providers such as Anthropic, OpenAI, Gemini, Copilot and Ollama. It also connects to CLI agents like Claude Code, Codex and Gemini CLI through the Agent Client Protocol, and to MCP servers. It is written in Lua and installs through lazy.nvim or any other plugin manager.

- **+** Many built-in adapters, including Ollama, OpenRouter and Azure OpenAI, plus a custom adapter API
- **+** ACP support lets Claude Code, Codex, Gemini CLI and others run inside Neovim
- **+** Supports MCP, skills, rules files (CLAUDE.md, .cursor/rules) and custom prompts
- **+** Review UI to comment on and approve or reject agent code changes
- **−** Works only inside Neovim
- **−** Depends on plenary.nvim and nvim-treesitter being installed
- **−** Maintainer accepts contributions at his discretion
- **−** Hardware requirements for local models are not documented

<sub>Docker · Needs Neovim, plenary.nvim, nvim-treesitter · Models: Anthropic, OpenAI, Azure OpenAI, Google Gemini, GitHub Copilot · [Repo](https://github.com/olimorris/codecompanion.nvim) · [📖 Docs ↗](https://codecompanion.olimorris.dev) · [🌐 Site ↗](https://codecompanion.olimorris.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codecompanion-nvim/)</sub>

<a name="oh-my-pi"></a>
### #&#8288;30 [oh-my-pi](https://github.com/can1357/oh-my-pi) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · MIT · Oct 2026</sub>

**Terminal coding agent with LSP, debugger, subagents and hashline edits built in.**

oh-my-pi (omp) is a fork of Pi: a terminal coding agent written in TypeScript with a Rust core, running on Bun. It ships 31 built-in tools, including LSP and DAP debugging, AST edits, persistent Python/JS eval, a browser, and parallel subagents in isolated worktrees. It supports 60+ model providers and runs on macOS, Linux and Windows.

- **+** LSP and DAP tools let the agent rename via the language server and drive lldb, dlv or debugpy
- **+** Subagents fan out into isolated worktrees and return schema-validated results
- **+** Reads existing Cursor, Cline, Codex and Copilot rule formats without conversion
- **+** Runs natively on Windows; ripgrep, glob and bash utilities run in-process, no WSL
- **−** Large surface (31 tools, 16 URL schemes) means a long learning curve
- **−** Benchmark claims in the README come from the author's own blog post
- **−** Install script fetches prebuilt binaries from build.stencil.so by default
- **−** Alpine/musl needs libstdc++ and libgcc installed manually

<sub>no GPU · Docker · Needs Bun >= 1.3.14 (or prebuilt binary), LLM provider API access, Language servers and debug adapters optional · Models: 60+ providers, OpenAI Codex, Gemini, Grok, MiniMax · safety checks passed 13 of 17 · [Repo](https://github.com/can1357/oh-my-pi) · [📖 Docs ↗](https://github.com/can1357/oh-my-pi/blob/main/docs/lsp-config.md) · [🌐 Site ↗](https://omp.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-pi/)</sub>

<a name="crush"></a>
### #&#8288;31 [crush](https://github.com/charmbracelet/crush) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Oct 2026</sub>

**Terminal coding agent with LSP context, MCP support and switchable LLM providers.**

Crush is a Go terminal UI coding agent from Charm that works against a project directory, with per-project sessions. It connects to many providers (Anthropic, OpenAI, Gemini, Bedrock, Azure, OpenRouter, Ollama and others) and lets you switch models mid-session. It uses LSPs for extra context and MCP servers (http, stdio, sse) for added tools.

- **+** Switch LLMs mid-session keeping context; custom OpenAI- or Anthropic-compatible providers
- **+** Config is a Bash-style crushrc, project-local or global, with a built-in Bash interpreter on Windows
- **+** MCP over http, stdio and sse, with a built-in OAuth flow for HTTP and SSE servers
- **+** Packaged for Homebrew, npm, apt, yum, Winget, Scoop, Nix and go install; Linux, macOS, Windows, BSDs
- **−** License is detected as NOASSERTION, so terms need checking before use
- **−** Hooks support is described as preliminary
- **−** crushrc and crush.json run as trusted code, so untrusted project configs are risky
- **−** Default onboarding points to Charm's subscription-based Hyper provider; others need your own keys

<sub>no GPU · Needs LLM provider API key or local model server (e.g. Ollama), Optional LSP servers (e.g. gopls) · Models: Anthropic, OpenAI, Google Gemini, Amazon Bedrock, Azure OpenAI · [Repo](https://github.com/charmbracelet/crush) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/crush/)</sub>

<a name="kilocode"></a>
### #&#8288;32 [kilocode](https://github.com/kilo-org/kilocode) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

**Coding agent for VS Code, JetBrains and the terminal.**

Kilo Code is a coding agent that edits code across files from natural language. It ships as a VS Code extension, a JetBrains plugin and a CLI (`kilo`). It has Code, Plan, Ask and Debug agents plus custom agents, inline autocomplete, terminal and browser control, and access to 500+ models at provider rates. The CLI is a fork of OpenCode.

- **+** Runs in VS Code, JetBrains and a CLI installable via npm, curl, Homebrew or AUR
- **+** Separate Code, Plan, Ask and Debug agents, plus custom agents
- **+** `kilo run --auto` runs non-interactively for CI/CD pipelines
- **+** 500+ models with mid-task switching, billed at provider rates with no markup
- **−** README points to account signup for model access; local or self-hosted model setup is not described
- **−** `--auto` approves permission prompts unless a rule denies them, so use only in trusted environments
- **−** Cloud Agent and Code Reviews are hosted services at app.kilo.ai
- **−** CLI is a fork of OpenCode, so it depends on that codebase

<sub>no GPU · Needs Kilo account or model provider, VS Code, JetBrains IDE or terminal · Models: 500+ models via Kilo, GPT, Claude, Gemini, Grok · [Repo](https://github.com/kilo-org/kilocode) · [📖 Docs ↗](https://kilo.ai/docs) · [🌐 Site ↗](https://kilo.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kilocode/)</sub>

<a name="pi-desktop"></a>
### #&#8288;33 [pi-desktop](https://github.com/vastsa/pi-desktop) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · LGPL-3.0 · Oct 2026</sub>

**Desktop app that runs coding agents in persistent sessions with plugins.**

PI-Desktop is a desktop app for macOS, Windows and Linux that organizes agent work as projects and sessions, with Agent, Plan and Goal modes, Subagents and parallel Worker Sessions. It is built on the pi agent runtime and supports OpenAI, Anthropic, OpenAI-compatible APIs, Ollama and LM Studio. Plugins can add panels, widgets, tools, skills, themes and MCP servers. The README labels the 0.20.x line Early Preview.

- **+** Sessions persist across app launches, with branching, search and recovery of interrupted work
- **+** Model chosen per session: OpenAI, Anthropic, compatible gateways, Ollama, LM Studio
- **+** Imports local sessions from Claude Code, Codex, OpenCode and Pi
- **+** Local-first: no telemetry, no account, credentials kept in the OS Keychain
- **−** README labels the 0.20.x line as Early Preview
- **−** Desktop app only; no Docker image or server deployment
- **−** Agent engine depends on the pi runtime packages
- **−** LGPL-3.0 license may constrain some embedding or redistribution uses

<sub>no GPU · Needs pi-ai, pi-agent-core, pi-coding-agent, Node.js >=22.19 (build), pnpm >=10 (build), Rust toolchain (build) · Models: OpenAI, Anthropic, OpenAI-compatible APIs, Ollama, LM Studio · [Repo](https://github.com/vastsa/pi-desktop) · [📖 Docs ↗](https://pi-docs.aiuo.net/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-desktop/)</sub>

<a name="dsh-tui"></a>
### #&#8288;34 [dsh-tui](https://github.com/ccch1mneyyy/dsh-tui) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

**Interactive terminal UI for DeepSeek Harness, with Claude and Codex backends.**

dsh-TUI is a terminal interface for DeepSeek Harness (DSH) that shows streaming thinking, tool cards, a context bar, a TPS gauge and double-Esc rewind. It installs as a DSH plugin profile and starts with `dsh-tui` or `dst`. Experimental backends drive the Claude Code CLI through the Claude Agent SDK and the native Codex app-server. It can also import session histories from other agents.

- **+** Imports Claude Code, Codex, OMP, zcode and Grok Build sessions; idempotent, with dry-run
- **+** Shows context occupancy, TPS, cache hit rate, tokens and session cost estimate
- **+** Renders images (Kitty/Sixel), Mermaid diagrams and LaTeX math in the terminal
- **+** Task-complete notifications via OSC 777/9/99 or BEL, configurable in /settings
- **−** Public beta; Claude and Codex backends are labelled experimental
- **−** Requires DeepSeek Harness and Node.js; first run also needs pnpm
- **−** Claude backend lacks DSH-only commands such as /tree, /preset and /provider
- **−** Notifications under tmux need passthrough and focus-events settings

<sub>no GPU · Needs Node.js, deepseek-harness, pnpm, DEEPSEEK_API_KEY or account sign-in · Models: DeepSeek, ChatGPT/Codex, Claude, Grok · [Repo](https://github.com/ccch1mneyyy/dsh-tui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-tui/)</sub>

<a name="chat-on-steroids"></a>
### #&#8288;35 [chat-on-steroids](https://github.com/totec448-spec/chat-on-steroids) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

**Desktop app that lets ChatGPT edit local files and run terminals via MCP.**

Desktop app (Windows, macOS Apple silicon, Linux) that connects a ChatGPT conversation to local files, shell and desktop tools through a custom MCP server and a browser extension for Chrome, Edge or Brave. It adds worker sub-agents, Goal and Loop modes for long tasks, and Compact & Resume to carry history into a new chat. It drives the ChatGPT web UI rather than calling Codex or a public API.

- **+** Reuses an existing ChatGPT plan; no separate model API billing described
- **+** Workers keep context between tasks and run independent jobs in parallel
- **+** Prebuilt installers for Windows x64, macOS arm64 and Linux x64 (DEB)
- **+** MIT licensed, UI available in 12 languages
- **−** Automates the ChatGPT browser UI, which is not a public API; account restrictions possible
- **−** Windows and macOS builds are unsigned; macOS prompts for a password after each update
- **−** Setup requires a tunnel, restricted OpenAI API key and custom MCP app in ChatGPT
- **−** Locked to ChatGPT; needs a plan that supports custom MCP apps

<sub>no GPU · Needs ChatGPT account with custom MCP app support, Chrome 125+, Edge or Brave, OpenAI tunnel and restricted API key, Linux Secret Service keyring · Models: ChatGPT models (account-dependent) · [Repo](https://github.com/totec448-spec/chat-on-steroids) · [📖 Docs ↗](https://github.com/totec448-spec/chat-on-steroids/blob/main/docs/setup.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-on-steroids/)</sub>

<a name="deepcode"></a>
### #&#8288;36 [deepcode](https://github.com/hkuds/deepcode) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

**Coding agent with TUI, Desktop and Web clients over one local service.**

DeepCode is a Python coding agent that works in your repository and runs from a terminal UI, a native Desktop app or a browser workbench. All three connect to one local background service, so sessions, projects, models, skills, permissions and goals are shared. It also includes Paper2Code, which turns research papers into code, and works with cloud or local model providers.

- **+** TUI, Desktop and Web clients share sessions and running work through one local service
- **+** Sandboxed shell commands, permission controls, opt-in command screening and egress limits
- **+** Goals, skills, MCP servers, automations and parallel agents are built in
- **+** Messages are written to the session file as read, so a crash mid-turn keeps history
- **−** Requires Python 3.12+; no Docker or compose files detected
- **−** RAM and GPU requirements are not stated in the README
- **−** Frequent releases with behaviour changes; upgrades call for a runtime snapshot first
- **−** Background service and an awake computer are needed for detached tasks

<sub>no GPU · Needs Python 3.12+, LLM provider or local model server · Models: Cloud and local model providers, Amazon Bedrock, Opper, DeepSeek V4, GLM-5.2 · port 3081 · [Repo](https://github.com/hkuds/deepcode) · [🌐 Site ↗](https://hkuds.github.io/DeepCode/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepcode/)</sub>

<a name="emdash"></a>
### #&#8288;37 [emdash](https://github.com/generalaction/emdash) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · Apache-2.0 · Oct 2026</sub>

**Desktop app that runs CLI coding agents in parallel Git worktrees.**

Emdash is a desktop app that launches several coding agent CLIs at once, each task in its own Git worktree and branch. It detects installed agents such as Claude Code, Codex, Cursor, OpenCode and Amp, and lets you review diffs, open pull requests, check CI and merge. It works on local projects and on remote machines over SSH/SFTP.

- **+** Per-task Git worktree and branch isolates parallel agent runs
- **+** Detects installed agent CLIs automatically
- **+** Sends tickets from Linear, GitHub, Jira, GitLab and others into an agent
- **+** Remote projects over SSH/SFTP with credentials in the OS keychain
- **−** Orchestrates other agent CLIs; you install and authenticate them yourself
- **−** Installs hook entries in each agent's user-level config
- **−** Desktop only; no Docker image or browser-hosted server
- **−** Optional telemetry must be disabled in Settings or via TELEMETRY_ENABLED=false

<sub>no GPU · Needs Git, Agent CLIs (Claude Code, Codex, OpenCode, Amp, etc.), SSH for remote projects · Models: Claude Code, Codex, Cursor, OpenCode, Amp · [Repo](https://github.com/generalaction/emdash) · [📖 Docs ↗](https://emdash.sh/docs) · [🌐 Site ↗](https://emdash.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/emdash/)</sub>

<a name="codex"></a>
### #&#8288;38 [codex](https://github.com/openai/codex) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 131k · Apache-2.0 · Oct 2026</sub>

**OpenAI's terminal coding agent that runs locally.**

Codex CLI is a coding agent from OpenAI that runs in the terminal on your machine. It installs through a shell script, npm, Homebrew, or prebuilt release binaries for macOS and Linux, and it signs in with a ChatGPT plan or an API key. The same project also covers IDE extensions and a desktop app.

- **+** Prebuilt binaries for macOS and Linux on x86_64 and arm64
- **+** Multiple install paths: script, npm, Homebrew, or release archive
- **+** Sign-in with an existing ChatGPT Plus, Pro, Business, Edu, or Enterprise plan
- **+** Apache-2.0 license, written in Rust
- **−** README documents only OpenAI sign-in or API key; other model providers are not mentioned
- **−** API key use requires extra setup beyond the quickstart
- **−** RAM and disk requirements are unknown
- **−** Install scripts fetch from OpenAI-hosted release URLs by default

<sub>no GPU · Needs ChatGPT account or OpenAI API key · Models: OpenAI models · [Repo](https://github.com/openai/codex) · [📖 Docs ↗](https://developers.openai.com/codex) · [🌐 Site ↗](https://chatgpt.com/codex) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex/)</sub>

<a name="claudecodeui"></a>
### #&#8288;39 [claudecodeui](https://github.com/siteboon/claudecodeui) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · AGPL-3.0 · Oct 2026</sub>

**Web and mobile UI for Claude Code, Cursor CLI and Codex sessions.**

Runs a local web server (default http://localhost:3001) that wraps the Claude Code, Cursor CLI and Codex CLIs with a chat view, shell terminal, file explorer with editing, and Git staging and commits. It discovers existing sessions from ~/.claude and reads and writes the same MCP and permission config as the CLI. A plugin system adds custom tabs and Node.js backends.

- **+** Auto-discovers existing sessions from ~/.claude; no separate config to maintain
- **+** Covers three agent CLIs: Claude Code, Cursor CLI and Codex
- **+** Built-in file editor, Git explorer, shell terminal and MCP management
- **+** Plugin system with a starter template and several community plugins
- **−** AGPL-3.0: modified versions run as a network service must publish source
- **−** Requires your own Claude, Cursor or Codex subscription; it supplies no models
- **−** Team sharing and always-on hosting only in paid CloudCLI Cloud (from €7/month)
- **−** Docker sandbox mode is experimental and supports only Claude Code and Codex

<sub>no GPU · Docker · Needs Node.js 22+, Claude Code, Cursor CLI or Codex CLI, sbx CLI (sandbox mode only) · Models: Claude, GPT · port 3001 · [Repo](https://github.com/siteboon/claudecodeui) · [📖 Docs ↗](https://cloudcli.ai/docs) · [🌐 Site ↗](https://cloudcli.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claudecodeui/)</sub>

<a name="claurst"></a>
### #&#8288;40 [claurst](https://github.com/kuberwastaken/claurst) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · GPL-3.0 · Oct 2026</sub>

**Rust terminal coding agent with multi-provider routing, modeled on Claude Code.**

Claurst is a terminal coding agent written in Rust, started as a clean-room reimplementation of Claude Code's behavior and now routing to several providers, including Anthropic and a ChatGPT (Codex) subscription. It has a TUI, a headless mode with stream-json output, hooks, skills, AGENTS.md/CLAUDE.md loading, and an ACP server for editors such as Zed. Version 0.2.0 is labelled beta.

- **+** Prebuilt binaries for Linux, macOS and Windows; installs via script, npm or bun
- **+** Speaks Agent Client Protocol (`claurst acp`), so Zed and other ACP editors can drive it
- **+** Follows Claude Code's hooks contract, plus skills and AGENTS.md/CLAUDE.md instruction files
- **+** Headless mode emits typed stream-json events and structured answers via --json-schema
- **−** Beta (v0.2.0); README warns of rough edges in experimental features
- **−** Seatbelt shell sandbox is described for macOS only
- **−** Free Mode, /goal, /share and ultracode are flagged experimental
- **−** Default build needs ALSA for voice; headless systems must disable default features

<sub>no GPU · Needs Provider API key or ChatGPT subscription login, Rust toolchain (build from source only) · Models: Anthropic, ChatGPT (Codex) subscription, other providers via /connect · [Repo](https://github.com/kuberwastaken/claurst) · [📖 Docs ↗](https://claurst.kuber.studio/docs) · [🌐 Site ↗](https://claurst.kuber.studio) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claurst/)</sub>

<a name="gh-aw"></a>
### #&#8288;41 [gh-aw](https://github.com/github/gh-aw) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Oct 2026</sub>

**GitHub CLI extension that compiles Markdown agent workflows into GitHub Actions.**

gh-aw is a GitHub CLI extension. You write repository automation as Markdown with YAML frontmatter, and `gh aw compile` turns it into a `.lock.yml` GitHub Actions workflow that runs an AI agent. Built-in engines are GitHub Copilot, Claude Code, OpenAI Codex, Google Gemini and Pi. Agent jobs are read-only and sandboxed by default, and writes go through validated `safe-outputs` jobs.

- **+** Compiles to standard Actions workflows, so it runs alongside existing CI/CD
- **+** Supports Copilot, Claude Code, Codex, Gemini and Pi engines
- **+** Agent jobs are read-only by default; writes are applied by separate scoped safe-outputs jobs
- **+** Targets tasks like issue triage, PR review, CI failure investigation and doc maintenance
- **−** Runs only on GitHub Actions and GitHub repositories
- **−** README says use is at your own risk and needs careful human supervision
- **−** Releases >= 0.83.3, < 0.85.4 were retired over a security vulnerability
- **−** Permissions, tools and network access are configurable, so authors must review them

<sub>no GPU · Docker · Needs GitHub CLI, GitHub Actions · Models: GitHub Copilot, Claude Code, OpenAI Codex, Google Gemini, Pi · [Repo](https://github.com/github/gh-aw) · [📖 Docs ↗](https://github.github.com/gh-aw/) · [🌐 Site ↗](https://github.github.com/gh-aw/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gh-aw/)</sub>

<a name="happy"></a>
### #&#8288;42 [happy](https://github.com/slopus/happy) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

**Mobile app, CLI and relay server to control Claude Code and Codex remotely.**

Happy is an Expo mobile and web client, an npm CLI (`happy claude`, `happy codex`) that wraps the Claude Code and Codex harnesses, and a relay server for end-to-end encrypted sync. Sessions started in the terminal can be continued from a phone. The newer multi-model Happy Harness (Claude, Codex, Grok) lives in the separate desktop app and happy-agent repositories.

- **+** Continue terminal Claude Code and Codex sessions from iOS, Android or web
- **+** Mobile sync between devices is end-to-end encrypted via a relay server
- **+** MIT licensed; the relay server is in the repo for self-hosting
- **+** Reuses existing Claude, Codex and Grok subscriptions rather than adding billing
- **−** Multi-model Harness and multiplayer sessions are in other repos, not this one
- **−** Original CLI only wraps Claude Code and Codex, not Grok
- **−** README gives no self-hosting steps, ports or resource requirements
- **−** Needs an existing Claude or Codex subscription or install to be useful

<sub>no GPU · Docker · Needs Claude Code, Codex, Node.js and npm · Models: Claude, Codex, Grok · safety checks passed 9 of 11 · [Repo](https://github.com/slopus/happy) · [📖 Docs ↗](https://happy.engineering/welcome/) · [🌐 Site ↗](https://happy.engineering/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/happy/)</sub>

<a name="avante-nvim"></a>
### #&#8288;43 [avante.nvim](https://github.com/avante-corp/avante.nvim) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

**Neovim plugin that adds a Cursor-style AI chat and code-apply workflow.**

avante.nvim is a Lua Neovim plugin that lets you ask an LLM about the current file and apply suggested edits to your source with one command. It defaults to an agentic mode that uses tools, supports ACP agents such as codex and gemini, and reads project instructions from an avante.md file. Providers include Claude, OpenAI, Azure, Gemini, Cohere, Copilot, Mistral, DeepSeek, Ollama and llama-cpp.

- **+** Many providers: Claude, OpenAI, Gemini, Ollama, llama-cpp, Copilot and others
- **+** Supports ACP agents (codex, gemini) alongside its own agentic mode
- **+** Per-project instructions via avante.md in the repo root
- **+** Installs through lazy.nvim, Pack, rocks.nvim, vim-plug, mini.deps, Nix
- **−** README badge says Neovim 0.12+, the install note says 0.11+
- **−** Build step needs make with curl and tar, or cargo to build from source
- **−** Auto-approves all tool permissions by default in agentic mode
- **−** Auto-suggestions are experimental and costly; RAG needs extra setup

<sub>no GPU · Needs Neovim 0.11+, plenary.nvim, nui.nvim, mega.cmdparse, make, curl, tar (or cargo to build from source) · Models: claude, openai, azure, gemini, cohere · [Repo](https://github.com/avante-corp/avante.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/avante-nvim/)</sub>

<a name="forgecode"></a>
### #&#8288;44 [forgecode](https://github.com/tailcallhq/forgecode) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent with a ZSH plugin and multiple LLM providers.**

Forge is a Rust CLI coding agent that reads files, writes patches and runs commands from an interactive TUI, a one-shot `-p` mode, or a ZSH plugin using a `:` prefix. It ships three agents (forge, sage, muse) and supports custom agents, SKILL.md skills, AGENTS.md instructions, MCP configuration and AI-written commit messages. Provider credentials are set with `forge provider login`.

- **+** Three usage modes: interactive TUI, one-shot `-p` for scripts, and `:` prefix ZSH plugin
- **+** Built-in read-only (sage) and planning (muse) agents alongside the implementing agent
- **+** Custom agents, skills and commands defined as files at project or global level
- **+** `--sandbox` creates an isolated git worktree and branch for experiments
- **−** Semantic search sends file content to api.forgecode.dev unless a server URL is set
- **−** Installed via a `curl | sh` script; no Docker or compose files detected
- **−** Full list of supported providers and models is not in the visible README
- **−** Plugin workflow requires ZSH; other shells get only the CLI

<sub>no GPU · Needs LLM provider API credentials, ZSH (for plugin mode), git · Models: OpenAI, Anthropic, other LLM providers · [Repo](https://github.com/tailcallhq/forgecode) · [🌐 Site ↗](https://forgecode.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/forgecode/)</sub>

<a name="kirocrew"></a>
### #&#8288;45 [kirocrew](https://github.com/kirodotdev/kirocrew) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Oct 2026</sub>

**Persistent agent workspace with memory, schedules and unattended tasks.**

Kiro Crew is a Python Gateway that drives agent sessions through ACP harnesses (default kiro-cli) and keeps sessions, memory, lessons, schedules and task checkpoints across restarts. You reach it from a desktop app, web dashboard, CLI, or messaging channels such as Slack and Discord. It runs checkpointed long tasks, scheduled jobs, webhooks and subagents, gated by approvals and OS sandboxing.

- **+** Sessions, memory, schedules and task checkpoints survive Gateway restarts
- **+** Same agent state reachable from desktop, dashboard, CLI, Slack, Discord, Telegram and Teams
- **+** Approvals, OS sandboxing, credential redaction and audit events; dashboard binds to loopback by default
- **+** Extensible with MCP servers, markdown skills, hooks and installable Apps
- **−** Default backend needs kiro-cli installed and signed in separately
- **−** Sends a daily anonymous telemetry heartbeat by default; opt-out required
- **−** Source build needs Python 3.12+ and Node.js 22.12+
- **−** Self-learning and skill synthesis are described without any benchmarks in the README

<sub>no GPU · Docker + Compose · Needs kiro-cli, Python 3.12+, Node.js 22.12+ · Models: Kiro models via kiro-cli, Other ACP harnesses · port 5476 · [Repo](https://github.com/kirodotdev/kirocrew) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kirocrew/)</sub>

<a name="openrig"></a>
### #&#8288;46 [openrig](https://github.com/mvschwarz/openrig) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · Apache-2.0 · Oct 2026</sub>

**Define and run a persistent team of Claude Code and Codex agents from YAML.**

OpenRig is a Node.js CLI (`rig`) and daemon that launches Claude Code and Codex sessions in tmux as a named, persistent team described in YAML. You talk to a kernel operator or a lead agent, which coordinates seats such as builder, QA and reviewer. It ships three starting teams (starter, workshop, factory), a TUI dashboard and a message queue between seats.

- **+** Mixes Claude Code and Codex seats in one YAML-defined rig
- **+** Ships three preset teams: starter, workshop and factory
- **+** Includes a TUI dashboard and per-seat status and readiness via `rig ps`
- **+** Setup has a dry run that previews changes before applying
- **−** Writes hooks and trust settings into Claude and Codex config files, plus ~/.tmux.conf
- **−** Native Windows unsupported; WSL2 only, and automated tests do not run there
- **−** Requires Node.js 22 or 24 and tmux; distro Node on Linux may be too old
- **−** Needs an existing Claude Code or Codex login; starter team assumes both

<sub>no GPU · Docker · Needs Node.js 22 or 24, tmux, Claude Code or Codex CLI, Herdr (optional) · Models: Claude Code, Codex · [Repo](https://github.com/mvschwarz/openrig) · [🌐 Site ↗](https://openrig.dev/follow) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openrig/)</sub>

<a name="kimi-code"></a>
### #&#8288;47 [kimi-code](https://github.com/moonshotai/kimi-code) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · MIT · Oct 2026</sub>

**Terminal coding agent from Moonshot AI that edits code and runs shell commands.**

Kimi Code CLI is a terminal coding agent that reads and edits code, runs shell commands, searches files and fetches web pages. It defaults to Moonshot AI's Kimi models via OAuth or an API key, and can be configured for other compatible providers. It also supports MCP servers, plugins, subagents, lifecycle hooks, and an ACP mode for Zed and JetBrains.

- **+** Installs as a single binary with one script; no Node.js required
- **+** Built-in coder, explore and plan subagents run in isolated contexts
- **+** `kimi acp` lets Zed, JetBrains or other ACP clients drive a session
- **+** Lifecycle hooks can gate risky tool calls; MCP servers configurable via /mcp-config
- **−** Defaults to Moonshot AI's Kimi models; other providers need manual configuration
- **−** Windows requires Git for Windows, since it uses Git Bash as its shell
- **−** README does not list which non-Kimi providers are supported
- **−** Terminal only; editor use depends on ACP client support

<sub>no GPU · Needs Git for Windows (Windows only), Kimi Code OAuth or Moonshot AI Open Platform API key · Models: Moonshot AI Kimi models, other compatible providers · [Repo](https://github.com/moonshotai/kimi-code) · [📖 Docs ↗](https://moonshotai.github.io/kimi-code/en/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kimi-code/)</sub>

<a name="cindy"></a>
### #&#8288;48 [cindy](https://github.com/makecindy/cindy) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · Apache-2.0 · Oct 2026</sub>

**Agent client that runs Claude Code and Codex on your local files.**

Cindy is the open-source client (Electron desktop and Expo mobile apps in a pnpm monorepo) for an agent that works on your local files and logged-in apps. It wraps the Claude Code and Codex harnesses, lets you switch models and harnesses mid-task, and can drive a browser, computer and phone. The backend service is in a separate repository and is not included.

- **+** Mixes harnesses and models in one task while memory, skills and tools carry over
- **+** Accepts an existing Claude Code or Codex plan, your own API keys, or local models
- **+** Skip Sign-In mode runs local agents without a Cindy account
- **+** Apache-2.0 source with MCP, skills and scheduled automation
- **−** Backend is not open source; server-backed features need the hosted Cindy service
- **−** Defaults to Cindy's official cloud endpoints; no self-hosted server path documented
- **−** Official builds send TapDB analytics and a heartbeat; removing it needs code edits
- **−** Only Claude Code and Codex harnesses today; native harness and plugin marketplace unfinished

<sub>Needs Node.js 22.x, pnpm 10.x, Git LFS, Cindy cloud account (for server-backed features) · Models: Claude Code, Codex, Cindy hosted models, custom API keys, local models · [Repo](https://github.com/makecindy/cindy) · [🌐 Site ↗](https://cindy.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cindy/)</sub>

<a name="bb"></a>
### #&#8288;49 [bb](https://github.com/get-bb/bb) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Oct 2026</sub>

**Agentic IDE with desktop app, web app, CLI and HTTP API.**

bb is an agentic IDE written in TypeScript that runs work in threads you can follow live, steer, or hand off to another agent. It is driven through an Electron desktop app, a web UI on port 38886, a `bb` CLI or an HTTP API, and it uses the provider CLI you have already authenticated. It is marked as in active development, with workflows still changing.

- **+** Same functionality across desktop app, web app, CLI and HTTP API
- **+** Starts with one command: `npx bb-app@latest`
- **+** Reuses your already authenticated provider CLI instead of separate API setup
- **+** Opt-out telemetry (`BB_TELEMETRY=false`) that the README says excludes message content
- **−** Desktop app supports only Apple Silicon macOS; Linux and Windows builds are alpha
- **−** README says workflows and surfaces are still evolving
- **−** Server API is unauthenticated and permits command execution; remote modes need a trusted network
- **−** Native add-ons need install scripts allowed on npm 12 or later

<sub>Needs Node.js, npm, authenticated provider CLI, Git for Windows (native Windows) · Models: provider CLIs (unspecified) · port 38886 · [Repo](https://github.com/get-bb/bb) · [📖 Docs ↗](https://github.com/get-bb/bb/blob/main/docs/configuration.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bb/)</sub>

<a name="symphony"></a>
### #&#8288;50 [symphony](https://github.com/openai/symphony) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

**Spec and Elixir reference for agents that pick up Linear tasks and open PRs.**

Symphony watches a Linear board for work and spawns isolated agent runs for each task. Agents report proof of work such as CI status, PR review feedback, complexity analysis and walkthrough videos, and land the PR once accepted. The repo ships a language-agnostic SPEC.md and an experimental Elixir reference implementation.

- **+** Language-agnostic SPEC.md lets you implement it in any language
- **+** Each task runs as an isolated, autonomous implementation run
- **+** Agents attach proof of work: CI status, review feedback, walkthrough videos
- **+** Apache-2.0 licensed reference implementation in Elixir
- **−** Described as a low-key engineering preview for trusted environments only
- **−** Reference implementation is experimental
- **−** Expects codebases that have already adopted harness engineering
- **−** RAM, ports and model support are not stated in the main README

<sub>Needs Linear, Codex · Models: Codex · [Repo](https://github.com/openai/symphony) · [▶️ Demo ↗](https://player.vimeo.com/video/1186371009?h=5626e4b899) · [📖 Docs ↗](https://github.com/openai/symphony/blob/main/SPEC.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/symphony/)</sub>

<a name="mimo-code"></a>
### #&#8288;51 [mimo-code](https://github.com/xiaomimimo/mimo-code) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

**Terminal coding agent with persistent project memory and checkpointed context.**

MiMoCode is a terminal TUI coding assistant that reads and writes code, runs commands and manages Git. It keeps project memory in files backed by SQLite FTS5 and rebuilds context from checkpoints when the window fills. It also has subagents, a /goal stop-condition judge, JavaScript workflows and bundled skills, and connects to Xiaomi MiMo, Codex OAuth or any OpenAI-compatible provider.

- **+** Checkpoint-based context rebuild and cross-session memory (MEMORY.md, checkpoint.md, task logs)
- **+** Works with Xiaomi MiMo, Codex OAuth, Claude Code import, or any OpenAI-compatible API
- **+** Per-model compaction limit via /context-limit to avoid long-context price tiers
- **+** Three built-in workflows and about 20 bundled skills; custom ones load from .mimocode/
- **−** macOS Terminal.app is unsupported; iTerm2 or VS Code terminal required
- **−** Voice input needs a MiMo login and sox; the ASR model is only on MiMo's platform
- **−** TUI can lag over SSH; workaround is mimo serve remotely and mimo attach locally
- **−** Desktop app features, including computer control, are separate and international edition only

<sub>no GPU · Needs sox (voice input only), LLM provider API key or OAuth login · Models: Xiaomi MiMo-V2.6-Pro, MiMo-V2.6-Flash, OpenAI/Codex, Anthropic, xAI/Grok · [Repo](https://github.com/xiaomimimo/mimo-code) · [🌐 Site ↗](https://mimo.xiaomi.com/coder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mimo-code/)</sub>

<a name="gptme"></a>
### #&#8288;52 [gptme](https://github.com/gptme/gptme) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

**Terminal-based AI agent that runs shell, Python, browser and file tools.**

gptme is a Python CLI agent that executes shell commands and Python, edits files with patch tools, browses via Playwright and reads images. It works with Anthropic, OpenAI, Google, DeepSeek, OpenRouter, or local models through Ollama and OpenAI-compatible servers. It also ships a Textual TUI, a web UI with REST server, an MCP client and server, ACP support for Zed and JetBrains, and a scaffold for scheduled autonomous agents.

- **+** Provider-agnostic: hosted APIs, OpenRouter, or local Ollama, LM Studio, vLLM and llama.cpp
- **+** Acts as MCP client and server, and as an ACP agent in Zed and JetBrains
- **+** Plugins, skills, hooks and lessons extend behavior without forking
- **+** Runs headless via gptme service init with systemd timers for scheduled agents
- **−** Executes shell and Python locally; sandboxing (Docker, Wasmtime) is a separate option
- **−** RAG tool needs the separate gptme-rag package
- **−** Large surface area (TUI, web UI, server, desktop app) spread across several repos
- **−** Hosted gptme.ai cloud service exists; its terms and limits are unknown from the README

<sub>GPU optional · Compose · Needs Playwright (browser tool), Docker or Wasmtime (optional sandboxing), gptme-rag (optional, rag tool) · Models: Anthropic, OpenAI, Google Gemini, SpaceXAI Grok, DeepSeek · [Repo](https://github.com/gptme/gptme) · [▶️ Demo ↗](https://chat.gptme.org) · [📖 Docs ↗](https://gptme.org/docs/) · [🌐 Site ↗](https://gptme.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gptme/)</sub>

<a name="codeg"></a>
### #&#8288;53 [codeg](https://github.com/spacering-net/codeg) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Oct 2026</sub>

**Workspace that runs Claude Code, Codex, Gemini CLI and other agents in one UI.**

Codeg is a Rust-based workspace that talks to coding agents over the Agent Client Protocol and renders each as a structured conversation with tool cards, live diffs and permission prompts. It imports and searches session history that agent CLIs keep on disk, and runs queued to-dos unattended in separate git worktrees. It ships as a desktop app, a self-hosted server or Docker container, and iOS and Android clients.

- **+** Fifteen agents built in, including Claude Code, Codex, Gemini CLI and Cursor; other ACP agents can be added
- **+** Imports and searches agent session history on disk, and lets one agent read another's session
- **+** To-dos run in their own git worktree and branch, scheduled or on demand, then wait for review
- **+** Runs as desktop app, self-hosted server, Docker, mobile clients, or via Telegram, Lark and WeChat
- **−** Wraps third-party agents; each agent's own install, login and model access still apply
- **−** Computer Use is described as preview
- **−** Very broad scope (git client, office viewers, canvas, browser) makes it a large surface to adopt
- **−** Server memory, port and sizing requirements are not stated in the README excerpt

<sub>no GPU · Docker + Compose · Needs Agent CLIs such as Claude Code or Codex, Git · Models: Claude Code, Codex, Gemini CLI, OpenClaw, OpenCode · [Repo](https://github.com/spacering-net/codeg) · [📖 Docs ↗](https://docs.codeg.app) · [🌐 Site ↗](https://docs.codeg.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeg/)</sub>

<a name="maestro"></a>
### #&#8288;54 [maestro](https://github.com/runmaestro/maestro) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · AGPL-3.0 · Oct 2026</sub>

**Desktop app for running many coding agents in parallel with unattended playbooks.**

Maestro is a cross-platform desktop app that wraps CLI coding agents (Claude Code, Codex, OpenCode, Factory Droid, plus beta Copilot-CLI, Qwen3 Coder and Oh My Pi) and runs them side by side, each with its own workspace and history. Auto Run executes markdown checklists or free-text goals as playbooks, one fresh session per task, and git worktrees isolate parallel agents. A built-in web server gives phone access, and a maestro-cli runs playbooks headless.

- **+** Passes through existing Claude Code, Codex or OpenCode config, MCP tools, skills and auth unchanged
- **+** Auto Run playbooks start a fresh session per task, suited to long unattended runs
- **+** Git worktree sub-agents run in parallel on isolated branches, with PR creation from the app
- **+** maestro-cli runs playbooks from cron or CI with JSONL output
- **−** Needs at least one supported agent CLI installed and authenticated separately
- **−** AGPL-3.0 license may restrict use in proprietary products
- **−** Copilot-CLI, Qwen3 Coder and Oh My Pi support is beta; Gemini CLI not supported
- **−** Tasks are prompt and response, not interactive agent sessions

<sub>no GPU · Needs Claude Code, Codex, OpenCode or another supported agent CLI, Git (optional), Cloudflare tunnel (optional, remote access) · Models: Claude Code, OpenAI Codex, OpenCode, Factory Droid, Copilot-CLI (beta) · [Repo](https://github.com/runmaestro/maestro) · [📖 Docs ↗](https://docs.runmaestro.ai) · [🌐 Site ↗](https://runmaestro.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maestro/)</sub>

<a name="m3e-canvas"></a>
### #&#8288;55 [m3e-canvas](https://github.com/lnkiai/m3e-canvas) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · MIT · Oct 2026</sub>

**Browser canvas for sketching linked Material 3 screens and exporting an AI prompt.**

M3E Canvas is a static Next.js app where you drag Material 3 Expressive parts onto phone or desktop screens, link them with tap and swipe transitions, and preview the flow. The design is exported as a prompt in Japanese, English, Chinese or Korean, targeting Android or web, to paste into a coding tool such as Claude Code, Codex, Gemini CLI or Cursor. State is kept in localStorage; there is no backend.

- **+** No backend: static export, designs saved in browser localStorage
- **+** Tap and swipe navigation with transitions, plus a clickable preview
- **+** Prompt output in four languages for Android or web targets
- **+** Optional AI helper sends your own key straight to the provider
- **−** Phone browsers get a one-screen, buttons-only editor
- **−** Output is a text prompt, not generated code
- **−** Design lives in browser storage unless shared by link
- **−** Fonts load from Google Fonts at runtime

<sub>no GPU · Needs Node.js and npm (to build), Google Fonts · Models: OpenAI, Claude, Gemini, DeepSeek · port 3000 · [Repo](https://github.com/lnkiai/m3e-canvas) · [▶️ Demo ↗](https://lnkiai.github.io/m3e-canvas/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/m3e-canvas/)</sub>

<a name="hapi"></a>
### #&#8288;56 [hapi](https://github.com/tiann/hapi) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · AGPL-3.0 · Oct 2026</sub>

**Remote control for coding agent CLI sessions from phone or web.**

HAPI wraps official coding agent CLIs (Claude Code, Codex, Cursor Agent, OpenCode, Copilot and others) and runs a hub, so you can watch, approve and continue the same sessions from native iOS/Android apps, a web/PWA client or a Telegram Mini App. Sessions move between local terminal and remote without a restart. The hub can use an E2E encrypted relay, Cloudflare Tunnel or Tailscale.

- **+** Wraps the official CLIs of ten agents instead of replacing them
- **+** Approve agent requests from a phone; web terminal and file browser included
- **+** SwiftUI and Kotlin Compose native clients live in the same repo
- **+** Self-host via Cloudflare Tunnel or Tailscale, or use the WireGuard+TLS relay
- **−** AGPL-3.0 license restricts use in closed network services
- **−** Shared Codex sessions require Codex 0.154.0 or newer
- **−** Native apps are built from source; store availability is not stated
- **−** No Docker or compose files; building from source needs Bun 1.4.0

<sub>no GPU · Needs Bun 1.4.0 (build from source), Agent CLIs (Claude Code, Codex, etc.), Cloudflare Tunnel or Tailscale (optional) · Models: Claude Code, Codex, Cursor Agent, Grok Build, OpenCode · [Repo](https://github.com/tiann/hapi) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hapi/)</sub>

<a name="agent-of-empires"></a>
### #&#8288;57 [agent-of-empires](https://github.com/agent-of-empires/agent-of-empires) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Session manager that runs AI coding agents in parallel tmux sessions.**

Agent of Empires (aoe) is a Rust session manager for AI coding agents on Linux and macOS. Each agent runs in its own tmux session, optionally in a git worktree or a Docker, Podman or Apple Containers sandbox. You monitor sessions from a TUI, a web dashboard (`aoe serve`), the CLI or an HTTP API.

- **+** Sessions are tmux-backed, so agents survive closing the TUI or dropping SSH
- **+** Per-session git worktrees and multi-repo workspaces for parallel work across branches
- **+** Optional container sandboxing with Docker, Podman or Apple Containers
- **+** TUI, web dashboard with phone view, CLI and HTTP API all available
- **−** Requires tmux; Windows only works through WSL2
- **−** Does not provide an agent itself; you bring Claude Code or another CLI agent
- **−** Supported agent list is not in the README; it requires running `aoe agents`
- **−** Web dashboard port and auth setup are not documented in the README

<sub>no GPU · Docker · Needs tmux, Docker (optional, for sandboxing) · [Repo](https://github.com/agent-of-empires/agent-of-empires) · [📖 Docs ↗](https://www.agent-of-empires.com/docs/quick-start/) · [🌐 Site ↗](https://www.agent-of-empires.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-of-empires/)</sub>

<a name="autonomous-company"></a>
### #&#8288;58 [autonomous-company](https://github.com/maxmiksa/autonomous-company) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Loop that runs Claude Code or Codex CLI as a 14-role product team.**

Runs a continuous shell loop that calls Claude Code (default) or Codex CLI each cycle with a charter, 14 expert-persona role prompts and 30+ skills. State persists in memories/consensus.md between cycles. A local dashboard and Product Center on port 8810 show cycles, usage, budgets and logs, and the repo ships 22 example apps produced by the agents.

- **+** Runs as launchd or systemd --user daemon with restart, rate-limit wait and circuit breaker
- **+** Supports Claude Code and Codex CLI; Cursor and OpenAI-compatible adapters are optional
- **+** Local Product Center tracks usage and budgets, with four parallel projects by default
- **+** Includes 22 runnable example products with startup notes and limitations
- **−** Consumes model quota continuously; outcomes depend on engine and budget limits
- **−** Team creation depends on the model; workflow is prompt guidance, not enforced
- **−** Supports macOS and Windows via WSL2 only; no Docker or compose files
- **−** Steering means editing consensus.md after stopping; mid-cycle edits can conflict

<sub>no GPU · Needs Claude Code or Codex CLI, Python 3.10+, Git, make · Models: Claude Code, Codex CLI, Cursor (optional adapter), OpenAI-compatible (optional adapter) · port 8810 · [Repo](https://github.com/maxmiksa/autonomous-company) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autonomous-company/)</sub>

<a name="warp"></a>
### #&#8288;59 [warp](https://github.com/warpdotdev/warp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · AGPL-3.0 · Oct 2026</sub>

**Terminal-based development environment with a built-in coding agent.**

Warp is a Rust client that started as a terminal and now includes a built-in coding agent. It can also run third-party CLI agents such as Claude Code, Codex and Gemini CLI. The client source is public, and the repository is itself maintained partly by automated agents (Warp Factories).

- **+** Runs its own agent or external CLI agents (Claude Code, Codex, Gemini CLI)
- **+** Client source is public; build with ./script/bootstrap and ./script/run
- **+** UI framework crates (warpui_core, warpui) are MIT-licensed
- **+** Written in Rust; contribution flow and AGENTS.md engineering guide documented
- **−** Most code is AGPL-3.0, which constrains proprietary forks
- **−** README does not state supported models, RAM or GPU requirements
- **−** Factories automation is early access with a demo booking flow
- **−** README covers only the client; server-side components are not described

<sub>Docker · Models: GPT models, Claude Code, Codex, Gemini CLI · [Repo](https://github.com/warpdotdev/warp) · [▶️ Demo ↗](https://build.warp.dev) · [📖 Docs ↗](https://docs.warp.dev) · [🌐 Site ↗](https://www.warp.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/warp/)</sub>

<a name="munder-difflin"></a>
### #&#8288;60 [munder-difflin](https://github.com/harnessmd/munder-difflin) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · MIT · Oct 2026</sub>

**Desktop app that runs many terminal coding agents as a coordinated team.**

Electron desktop app that runs terminal agent CLIs (Claude Code, Codex, Gemini CLI, Grok, Kimi, Qwen, OpenCode, Crush, Copilot, Cursor, custom commands) in node-pty sessions. An orchestrator agent routes work between them through file-based mailboxes and shared markdown memory, shown as avatars on a Pixi.js office floor. Adds approval gates, a circuit breaker, per-agent budgets, a Monaco editor with git views and local dictation.

- **+** Wraps 12 named agent CLIs plus custom commands, using your existing subscriptions
- **+** Per-agent markdown memory, mailboxes and optional git worktrees to avoid branch collisions
- **+** Approval queue for spend, scope and destructive ops, plus a steer, constrain, stop circuit breaker
- **+** Supports BYOK keys and local models via Ollama, LM Studio or vLLM
- **−** Labeled pre-release (v0.5.3)
- **−** Stapler meeting transcription and the newer sidebar are in the paid Pro tier
- **−** Transcription is English only in 0.5.3
- **−** Desktop Electron app only; no Docker image or headless server mode

<sub>GPU optional · Needs Agent CLIs (claude, codex, etc.), git, uv, Node, MemPalace · Models: Claude Code, OpenAI Codex, Gemini CLI, Antigravity, Grok · [Repo](https://github.com/harnessmd/munder-difflin) · [🌐 Site ↗](https://harnessmd.com/download) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/munder-difflin/)</sub>

<a name="openevolve"></a>
### #&#8288;61 [openevolve](https://github.com/algorithmicsuperintelligence/openevolve) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · Apache-2.0 · Oct 2026</sub>

**Evolves programs with LLM mutations, scored by your own evaluator.**

OpenEvolve takes an initial program and an evaluator function, then repeatedly asks LLMs to rewrite the code. It keeps candidates in a MAP-Elites population split across islands. It works with OpenAI-compatible APIs, local servers such as Ollama, or the Claude Code, Copilot and Codex CLIs as backends. It runs from the command line or as a Python library.

- **+** MAP-Elites with multiple islands and migration, plus island-selector and population hooks
- **+** Works with OpenAI-compatible APIs, Ollama/vLLM, and Claude Code, Copilot or Codex CLIs
- **+** Usable as a CLI or a Python library with inline code and callable evaluators
- **+** Seeded by default (seed 42); cascade evaluation filters weak programs early
- **−** Needs a user-written evaluator; it does not work on an arbitrary repo by itself
- **−** LLM cost is real: README estimates $0.01-0.60 per iteration depending on model
- **−** Benchmark claims in the README are not backed by numbers beyond the examples
- **−** Quick start sets a Gemini key through OPENAI_API_KEY, which is confusing

<sub>no GPU · Docker · Needs Python 3.10+, LLM provider (OpenAI-compatible API or Claude Code/Copilot/Codex CLI) · Models: OpenAI, Google Gemini, Ollama, vLLM, OptiLLM · [Repo](https://github.com/algorithmicsuperintelligence/openevolve) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openevolve/)</sub>

<a name="codepilot"></a>
### #&#8288;62 [codepilot](https://github.com/op7418/codepilot) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · custom license · Sep 2026</sub>

**Desktop AI agent client for Claude Code workflows across many model providers.**

CodePilot is an Electron and Next.js desktop app that runs chat and coding sessions against 17+ providers, including Anthropic, OpenRouter, Bedrock, Vertex, Ollama and custom OpenAI- or Anthropic-compatible endpoints. It adds MCP server management, skills, session rewind, a git panel, and a remote bridge for Telegram, Feishu, Discord, QQ and WeChat. File editing and shell commands need the Claude Code CLI installed.

- **+** Switch among 17+ providers and models mid-conversation, including Ollama and custom endpoints
- **+** Manages MCP servers (stdio/sse/http) with runtime status, plus skills and a skills.sh marketplace
- **+** Session pause, resume and rewind to checkpoint, split-screen sessions, token and cost charts
- **+** Local SQLite storage; builds for macOS, Windows and Linux, with in-app updates on macOS and Windows
- **−** BSL-1.1 license: commercial use needs a separate license; converts to Apache 2.0 in 2029
- **−** File editing, terminal and git actions require the separate Claude Code CLI
- **−** Windows builds are unsigned and trigger SmartScreen; Linux updates are manual
- **−** Interface is English and Chinese only

<sub>no GPU · Needs Claude Code CLI (optional, for file editing and terminal), Node.js 18+ (build from source), Provider API keys · Models: Anthropic, OpenRouter, AWS Bedrock, Google Vertex AI, Ollama · port 3000 · [Repo](https://github.com/op7418/codepilot) · [📖 Docs ↗](https://www.codepilot.sh/docs) · [🌐 Site ↗](https://www.codepilot.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codepilot/)</sub>

<a name="maka"></a>
### #&#8288;63 [maka](https://github.com/apache/maka) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · Apache-2.0 · Oct 2026</sub>

**Desktop, TUI and CLI agent workspace with an append-only event log.**

Apache Maka (Incubating) is an Electron desktop app, TUI and CLI that run a coding agent against your own model. Every message, tool call and permission decision is stored as an append-only RuntimeEvent in local SQLite. Desktop, TUI, CLI and the eval package are clients of one Runtime Host, and the repo publishes benchmark runs with per-task results. Written in TypeScript; latest Apache release is 0.2.0.

- **+** Every model message, tool call and permission decision is kept in an append-only event log
- **+** Sessions, settings and run records stay local; models can be cloud API, local or gateway
- **+** Per-task benchmark results against other harnesses are published in docs/eval
- **+** One Runtime Host serves Desktop, TUI and CLI, with an MCP client and sandboxed file and shell tools
- **−** Windows and Linux builds are previews; macOS is the main platform
- **−** API keys are kept in a plaintext local file, readable only by your OS account
- **−** Incubating project; data formats and CLI commands may still change
- **−** Older JSONL transcripts and safeStorage credentials are not imported after upgrade

<sub>no GPU · Needs Node.js 22.19+ or 24+, npm, Git, ripgrep, Rust 1.98+ (only for peer builds) · Models: cloud APIs, local models, compatible gateways · [Repo](https://github.com/apache/maka) · [📖 Docs ↗](https://github.com/apache/maka/blob/main/docs/README.md) · [🌐 Site ↗](https://maka.apache.org/en/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maka/)</sub>

<a name="terax-ai"></a>
### #&#8288;64 [terax-ai](https://github.com/crynta/terax-ai) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · Apache-2.0 · Oct 2026</sub>

**Terminal-first desktop workspace with editor, git panel and agentic AI side-panel.**

Terax is a desktop app built on Tauri 2, Rust and React 19 that combines a PTY terminal, CodeMirror editor, file explorer, git graph and web preview. Its AI side-panel runs agents with approval-gated bash and file edits against your own API keys or local Ollama, LM Studio and MLX models. About 7-8 MB on disk, with no telemetry or account.

- **+** Many BYOK providers plus Ollama, LM Studio and MLX for local models
- **+** API keys go to the OS keychain; no telemetry or account
- **+** AI edit diffs can be accepted or rejected hunk by hunk
- **+** Runs on macOS, Linux and Windows, with WSL workspaces
- **−** README says v0.9.0 will replace xterm.js with libghostty and WebGPU, so internals will change
- **−** Language server support is opt-in and needs configuration
- **−** Desktop install only; no Docker or server mode
- **−** Author notes development time went to another product (Zephium)

<sub>GPU optional · Needs Rust (build from source), Node 22+ and pnpm (build from source), Tauri platform prerequisites (build from source) · Models: OpenAI, Anthropic, Google Gemini, Groq, xAI · [Repo](https://github.com/crynta/terax-ai) · [📖 Docs ↗](https://terax.app/docs) · [🌐 Site ↗](https://terax.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terax-ai/)</sub>

<a name="neo"></a>
### #&#8288;65 [neo](https://github.com/neomjs/neo) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Oct 2026</sub>

**Multi-threaded browser UI engine, maintained by a cross-model team of AI agents.**

Neo.mjs is a zero-dependency, build-free JavaScript application engine that runs app logic, VDOM diffing, data and canvas work in separate Web Workers. Its README frames it as one part of an agent setup: a Neural Link lets AI agents inspect and mutate a live app's state, while memory and review tooling lives in the sibling neo-agent-brain repo. This repo is the UI runtime, not the agent backend.

- **+** Off-main-thread design with App, VDom, Data, Canvas workers and SharedWorker for multi-window apps
- **+** Native ES modules with no transpilation and zero runtime dependencies
- **+** Neural Link exposes tools like get_component_tree and patch_code for agents to edit live apps
- **+** Project's own maintenance record is public: 900+ merged PRs reported for June 2026
- **−** Agent memory, knowledge base and orchestration are in separate repos, not this one
- **−** Fleet Manager (neo-agent-institution) is version 0.1.0 and awaits an outside operator's first run
- **−** Requires adopting the Actor Model and Workers; not a drop-in swap for other UI frameworks
- **−** README is mostly vision and claims; setup requirements for the agent stack are not stated here

<sub>Needs Node.js and npm (npx neo-app), neo-agent-brain (for agent features) · Models: Claude, Gemini, GPT, Kimi · [Repo](https://github.com/neomjs/neo) · [📖 Docs ↗](https://neomjs.com/#/learn/gettingstarted/Setup) · [🌐 Site ↗](https://neomjs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neo/)</sub>

<a name="cate"></a>
### #&#8288;66 [cate](https://github.com/0-ai-ug/cate) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Oct 2026</sub>

**Desktop IDE that lays out coding-agent terminals on an infinite canvas.**

Cate is a desktop app where terminals, Monaco editors, browsers and document viewers sit on a pannable canvas or in docked tabs. Terminals running Claude Code, Codex or other agent CLIs show running, waiting or finished state and notify you when input is needed. It creates git worktrees per branch so parallel agents stay separated.

- **+** Per-terminal agent status and notifications for turn end and permission prompts
- **+** One-step git worktree creation from a local branch, remote branch or open PR
- **+** Agent sessions reattach with scrollback and resume commands after restart
- **+** Prebuilt installers for macOS, Windows and Linux, plus a Homebrew cask
- **−** Status reporting works only with supported agent CLIs; the list is not given
- **−** Desktop app; no web or self-hosted server deployment is described
- **−** Ships no agent or model of its own; you bring the agent CLI
- **−** Remote pairing through Cate Connect is not documented in the README

<sub>no GPU · Needs git, agent CLIs such as Claude Code or Codex · [Repo](https://github.com/0-ai-ug/cate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cate/)</sub>

<a name="zeroshot"></a>
### #&#8288;67 [zeroshot](https://github.com/the-open-engine/zeroshot) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Runs coding agents through enforced review-and-repair graphs you define.**

zeroshot runs a worker agent, independent reviewers and repair loops as a graph with engine-enforced review gates and retry limits. Each node can use its own model and harness (Pi, Claude Code, Codex or Copilot), and graphs plus runtime settings can be saved as reusable profiles. Runs are logged to a SQLite ledger, and delivery can stay local or push, open a PR, or merge.

- **+** Review gates and retry limits are enforced by the engine, not by prompts
- **+** Per-node model and harness choice across Pi, Claude Code, Codex and Copilot
- **+** Events go to a durable SQLite ledger; failed runs can be restarted or resumed
- **+** Delivery levels: local, --push, --pr, --ship; self-hostable Docker target
- **−** Needs an installed, signed-in harness CLI such as Codex or Claude Code
- **−** PR and ship delivery supports GitHub only; local runs also need gh
- **−** Docker and cloud runs require an exact Git source
- **−** A passing run only means the configured checks accepted the work

<sub>no GPU · Docker · Needs Node.js 18+, Codex, Claude Code, GitHub Copilot or Pi CLI, GitHub CLI (gh) for local PR and ship runs · Models: Anthropic, OpenAI, Codex, GitHub Copilot, Pi · port 4173 · [Repo](https://github.com/the-open-engine/zeroshot) · [📖 Docs ↗](https://zeroshot.sh/docs/) · [🌐 Site ↗](https://zeroshot.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zeroshot/)</sub>

<a name="mistral-vibe"></a>
### #&#8288;68 [mistral-vibe](https://github.com/mistralai/mistral-vibe) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent from Mistral with file, shell and subagent tools.**

Mistral Vibe is a Python CLI that lets Mistral models read, edit and search a codebase and run shell commands from a chat prompt. It has approval-based agent profiles (ask, plan, accept-edits, auto-approve), subagents via a task tool, skills, slash commands and MCP server configuration. A programmatic mode (-p) adds limits on turns, cost, tokens and time, with JSON output and exit codes for scripting.

- **+** Scriptable -p mode with --max-turns, --max-price, --max-tokens, --time-limit and defined exit codes
- **+** Agent profiles control approvals: ask, plan (read-only), accept-edits (default), auto-approve
- **+** Supports subagents, custom skills, slash commands, MCP servers and custom agent files
- **+** Trust-folder prompt guards against running in unvetted directories
- **−** Officially supports UNIX only; Windows works but is not a target
- **−** Built around Mistral's models; other provider support is not stated in the visible README
- **−** Needs a modern terminal emulator; older terminals may render badly
- **−** Some features are experimental, such as --agent-socket

<sub>no GPU · Needs Python 3.12+, Mistral API key, uv (Windows install) · Models: Mistral models, Mistral Medium 3.5 (vision) · [Repo](https://github.com/mistralai/mistral-vibe) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mistral-vibe/)</sub>

<a name="atomic-agent"></a>
### #&#8288;69 [atomic-agent](https://github.com/atomicbot-ai/atomic-agent) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Local-first terminal agent that browses, edits files and runs approved commands.**

Atomic Agent is a TypeScript CLI/TUI agent that keeps its control loop, memory and sessions on your disk. It drives a browser via playwright-core, edits files, runs approval-gated shell commands, and connects to MCP servers. It targets a local llama.cpp server (managed or your own) with grammar-constrained tool calls, and also supports cloud providers and a Fusion mode that splits planning and work across models.

- **+** Runs on local llama.cpp models with GBNF-constrained tool calls; no API cost locally
- **+** Reports GAIA L1 69.8% vs Hermes 58.5% on the same local model
- **+** Memory in SQLite/FTS5 and plain-file state, with traces you can inspect
- **+** Imports sessions and skills from Claude Code, Codex, Pi, Hermes and OpenClaw
- **−** Developer preview: APIs, commands and config are still changing
- **−** No Intel Mac build; Windows on ARM runs x64 under emulation
- **−** Install is a curl-to-shell script; no Docker or compose files
- **−** Benchmark covers 53 tasks, with different agent versions per model row

<sub>GPU optional · Needs llama.cpp (llama-server), Chrome/Edge/Brave/Chromium (browser tools) · Models: GGUF via llama-server, OpenAI-compatible, OpenRouter, Gemini, Anthropic · [Repo](https://github.com/atomicbot-ai/atomic-agent) · [🌐 Site ↗](https://atomicagent.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/atomic-agent/)</sub>

<a name="nanocoder"></a>
### #&#8288;70 [nanocoder](https://github.com/nano-collective/nanocoder) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · custom license · Oct 2026</sub>

**Terminal coding agent that works with local or any OpenAI-compatible model.**

Nanocoder is a terminal coding agent written in TypeScript, installed through npm, Homebrew or Nix. It runs against local models via Ollama or any OpenAI-compatible API, and offers interactive and non-interactive modes, MCP server configuration, skills, hooks and PR review from the CLI. It is developed by the Nano Collective, a non-profit community group.

- **+** Provider-agnostic: Ollama locally, or OpenRouter, Requesty, Anthropic, Google via compatible APIs
- **+** Several modes (normal, auto-accept, yolo, plan, architect) selectable with --mode
- **+** Non-interactive `run` command and `review` command for branches or PRs
- **+** README states no paid tiers and no telemetry sending prompts
- **−** `nanocoder review` is diff-only and needs a TTY; output cannot be captured to a file
- **−** `worktree` command requires Git and an authenticated gh CLI
- **−** License is reported as NOASSERTION, so terms are unclear from metadata
- **−** Hardware requirements for local models are not documented in the README

<sub>GPU optional · Needs Node.js/npm, Ollama (for local models), Git and gh CLI (worktree command) · Models: Ollama, OpenAI-compatible APIs, OpenRouter, Requesty, Anthropic · [Repo](https://github.com/nano-collective/nanocoder) · [📖 Docs ↗](https://docs.nanocollective.org/nanocoder/docs) · [🌐 Site ↗](https://nanocollective.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nanocoder/)</sub>

<a name="supacode"></a>
### #&#8288;71 [supacode](https://github.com/supabitapp/supacode) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · custom license · Oct 2026</sub>

**Native macOS app that runs coding agents in parallel git worktrees.**

Supacode is a native macOS app, written in Swift, that gives each coding-agent task its own git worktree and a libghostty-rendered terminal. Sessions run under the zmx daemon, so they survive app quits and dropped SSH connections. It detects Claude, Codex and Copilot through installed hooks, shows busy, awaiting-input or idle state, and can be driven by a CLI and deeplinks.

- **+** One git worktree and one terminal per task, so parallel agents do not collide
- **+** Sessions persist via zmx across app restarts and, with zmx on the host, SSH drops
- **+** Live agent status badges and notifications for Claude, Codex and Copilot
- **+** supacode CLI and supacode:// deeplinks allow scripting and hotkey bindings
- **−** Requires macOS 26.0 or later; no Linux or Windows support
- **−** Building from source needs mise, submodules, and Xcode 26.3 on macOS 26.4+
- **−** Remote SSH repositories are Beta with some local-only features reduced
- **−** License not identified by tooling (NOASSERTION); README only points to a LICENSE file

<sub>Needs macOS 26.0+, git, zmx, mise, Xcode 26.3 (build, macOS 26.4+) · Models: Claude, Codex, Copilot · [Repo](https://github.com/supabitapp/supacode) · [🌐 Site ↗](https://supacode.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supacode/)</sub>

<a name="firstmate"></a>
### #&#8288;72 [firstmate](https://github.com/kunchenguid/firstmate) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · MIT · Oct 2026</sub>

**Agent distro that lets one chat agent dispatch parallel coding agents in git worktrees.**

firstmate is a cloned repo of AGENTS.md instructions, bundled skills and shell helper scripts. Launched inside a terminal coding agent such as Claude Code, Grok, Pi, Codex or Cursor Agent CLI, it becomes a single "first mate" you talk to. It spawns crewmate agents in tmux, Herdr, Zellij, cmux or Orca sessions, gives each a clean git worktree, supervises them with a bash watcher, and returns PRs, local merges or investigation reports.

- **+** Each task runs in its own treehouse or Orca worktree, so parallel work on one repo does not collide
- **+** Crewmates are visible tmux windows or Herdr tabs you can watch or type into
- **+** State is kept on disk, so a restarted session reconciles the fleet
- **+** Per-project modes: no-mistakes, direct-PR or local-only, with optional +yolo merge autonomy
- **−** Needs a separate primary harness (Claude Code, Grok, Pi, Codex, etc.); it is not standalone
- **−** Zellij, cmux and Orca backends are marked experimental
- **−** Supervision and turn-end guard behavior differs across harnesses; Codex and OpenCode carry more tradeoffs
- **−** Supports macOS and Linux only; GitHub CLI authentication is required

<sub>no GPU · Needs git, GitHub CLI (gh), tmux (default backend), treehouse, a supported agent harness (Claude Code, Grok, Pi, Codex, OpenCode, Cursor Agent CLI) · Models: Claude Code, Grok, Pi, Oh My Pi, Codex · [Repo](https://github.com/kunchenguid/firstmate) · [📖 Docs ↗](https://github.com/kunchenguid/firstmate/blob/main/docs/architecture.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/firstmate/)</sub>

<a name="jetbrains-cc-gui"></a>
### #&#8288;73 [jetbrains-cc-gui](https://github.com/zhukunpenglinyutong/jetbrains-cc-gui) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

**JetBrains IDE plugin providing a chat GUI for Claude Code, Codex and other CLIs.**

An IntelliJ platform plugin that wraps AI coding CLIs in a chat panel inside the IDE. It supports Claude Code and OpenAI Codex, plus several beta CLIs (Grok, Kimi, OpenCode, PI, OMP, DeepSeek Harness). Features include @file references, image input, conversation rewind, diff view, MCP servers, slash-command skills, permission controls and session history.

- **+** Single chat UI over Claude Code, Codex and six beta CLIs
- **+** Session history with search, favorites, export and usage statistics
- **+** Permission management, diff comparison and MCP server support
- **+** Provider management compatible with cc-switch
- **−** JetBrains IDEs only; no VS Code or standalone version
- **−** Most non-Claude, non-Codex engines are marked Beta
- **−** macOS scrolling lag may need a JCEF GPU-disable VM option
- **−** Requires the underlying CLIs and accounts; README does not document setup

<sub>no GPU · Docker · Needs IntelliJ IDEA / JetBrains IDE, Claude Code or other supported AI coding CLI, Node.js (ai-bridge, webview build) · Models: Claude Code, OpenAI Codex, Grok CLI, Kimi CLI, OpenCode · [Repo](https://github.com/zhukunpenglinyutong/jetbrains-cc-gui) · [🌐 Site ↗](https://plugins.jetbrains.com/plugin/29342-cc-gui-claude-or-codex-) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jetbrains-cc-gui/)</sub>

<a name="code-graph-rag"></a>
### #&#8288;74 [code-graph-rag](https://github.com/vitali87/code-graph-rag) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Oct 2026</sub>

**Tree-sitter code knowledge graph you query and edit in plain English.**

Parses a multi-language repository with Tree-sitter into a knowledge graph stored in an embedded SQLite file by default, with Memgraph and Neo4j as opt-in backends. A CLI agent (cgr) turns natural-language questions into Cypher, retrieves source, finds dead code, and applies AST-based edits with a diff preview. It also runs as an MCP server for Claude Code and other clients.

- **+** Embedded SQLite graph by default: no database server, Docker or cmake needed
- **+** 14 languages fully supported under one graph schema, plus an ast-grep tier for more
- **+** Optional compiler frontends (libclang, go/types, Roslyn, javac, Jedi) and runtime trace merging
- **+** Runs as an MCP server for Claude Code and other MCP clients
- **−** PyPI and GitHub releases follow every 50th version; newest code needs a git install
- **−** Needs Python 3.12+ and ripgrep; older system interpreters need manual pinning
- **−** --clean deletes every project in the shared graph, not only the current repo
- **−** Managed cloud and air-gapped deployments are sold as paid enterprise services

<sub>Docker · Needs Python 3.12+, ripgrep, Memgraph (optional), Neo4j (optional), Qdrant (optional) · [Repo](https://github.com/vitali87/code-graph-rag) · [📖 Docs ↗](https://docs.code-graph-rag.com) · [🌐 Site ↗](https://code-graph-rag.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-graph-rag/)</sub>

<a name="obsidian-agent-client"></a>
### #&#8288;75 [obsidian-agent-client](https://github.com/rait-09/obsidian-agent-client) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Sep 2026</sub>

**Obsidian plugin that chats with Claude Code, Codex, Gemini CLI and other ACP agents.**

Desktop-only Obsidian plugin that launches locally installed agents over the Agent Client Protocol and gives them a chat UI inside the vault. Notes are passed with `@` mentions, and agent edits appear as word-level diffs. Nine agent presets are included, and any ACP-compatible agent can be added as a custom entry.

- **+** Works with nine ACP agent presets plus custom ACP entries, no plugin update needed
- **+** Per-action permission prompts; auto-allow is off by default
- **+** Several agents can run in sidebar tabs, editor tabs, floating windows or embedded in notes
- **+** Agents reuse their own MCP servers, skills and slash commands without plugin configuration
- **−** Desktop-only; agents must be installed and authenticated separately
- **−** Agents keep full system access, including terminal commands, once permitted
- **−** Session resume and fork depend on the agent
- **−** Notes, mentions and attachments are sent to the agent's provider

<sub>no GPU · Needs Obsidian desktop, Locally installed ACP agent (e.g. Claude Code, Codex, Gemini CLI) · Models: Claude Code, Codex, Gemini CLI, Mistral Vibe, OpenCode · [Repo](https://github.com/rait-09/obsidian-agent-client) · [📖 Docs ↗](https://rait-09.github.io/obsidian-agent-client/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/obsidian-agent-client/)</sub>

<a name="happier"></a>
### #&#8288;76 [happier](https://github.com/happier-dev/happier) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Control Claude Code, Codex and OpenCode sessions from phone, desktop and browser.**

Happier is a multi-device client for running coding agents on your own machines. A daemon starts Claude Code, Codex, OpenCode, Pi and other ACP agents where your code lives, and an end-to-end encrypted relay syncs sessions to iOS, Android, desktop and web apps. It adds cross-agent subagents, git worktrees, diff review, an approvals inbox and an MCP server mode.

- **+** Session content is encrypted on-device before reaching the relay
- **+** Self-hosted relay runs the same features as the hosted one
- **+** Sessions can delegate to other agents, and agents can be switched mid-session
- **+** Mirrors existing Claude Code, Codex and OpenCode terminal sessions to every device
- **−** Relay still sees routing metadata such as session ids, timestamps and usage
- **−** Requires the daemon installed on each machine that runs agents
- **−** Voice assistant needs an ElevenLabs key or a local voice pipeline
- **−** Preview and dev channels can break; hosted cloud runs stable only

<sub>no GPU · Docker · Needs Claude Code, Codex, OpenCode or other ACP agent CLIs, Happier relay (hosted or self-hosted), ElevenLabs (optional, voice) · Models: Claude Code, Codex, OpenCode, Gemini CLI, Pi · [Repo](https://github.com/happier-dev/happier) · [▶️ Demo ↗](https://cloud.happier.dev) · [📖 Docs ↗](https://docs.happier.dev) · [🌐 Site ↗](https://happier.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/happier/)</sub>

<a name="xum"></a>
### #&#8288;77 [xum](https://github.com/coder/xum) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Oct 2026</sub>

**Desktop and server app for running many coding agents in isolated workspaces.**

Xum (formerly Mux) is a TypeScript app that runs several coding agents side by side. Each agent gets its own workspace: the local project directory, a git worktree, or a remote host over SSH. It uses a custom agent loop with Claude Code-style Plan/Exec modes and /compact, and shows git divergence, costs and agent status in one UI.

- **+** Three runtimes per workspace: local directory, git worktree, or SSH remote
- **+** Central git divergence view across parallel agent workspaces
- **+** Ollama for local models and OpenRouter for long-tail providers
- **+** Ships a VS Code extension and a responsive server-mode UI for mobile
- **−** AGPL-3.0 license may restrict use in proprietary or hosted products
- **−** Pre-built binaries listed only for macOS and Linux; no Windows build
- **−** Custom agent loop, so behavior differs from Claude Code despite similar UX
- **−** README gives no RAM, port or server-mode setup details

<sub>GPU optional · Docker + Compose · Needs git, SSH (for remote runtime), Ollama (optional), OpenRouter (optional) · Models: Anthropic Claude (sonnet-4, opus-4), OpenAI GPT-5, xAI Grok, Ollama, OpenRouter · [Repo](https://github.com/coder/xum) · [📖 Docs ↗](https://mux.coder.com) · [🌐 Site ↗](https://mux.coder.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xum/)</sub>

<a name="vibe-kanban"></a>
### #&#8288;78 [vibe-kanban](https://github.com/bloopai/vibe-kanban) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Oct 2026</sub>

**Kanban board that runs coding agents in per-issue git workspaces.**

Vibe Kanban pairs a kanban board for planning with workspaces where coding agents execute, each with its own branch, terminal and dev server. You review diffs, leave inline comments that go back to the agent, preview the app in a built-in browser, and open pull requests. The README announces the project is sunsetting.

- **+** Works with 10+ agents, including Claude Code, Codex, Gemini CLI, Copilot, Amp and Cursor
- **+** Starts with one command: npx vibe-kanban
- **+** Inline diff comments are sent straight to the agent
- **+** Built-in preview browser with devtools, inspect mode and device emulation
- **−** README states the project is sunsetting
- **−** Last release was 2026-04-24, months before the latest commit
- **−** Each coding agent must be installed and authenticated separately
- **−** Maintainers ask that PRs not be opened without prior discussion

<sub>no GPU · Docker · Needs Node.js >=20, Git, an authenticated coding agent CLI · Models: Claude Code, Codex, Gemini CLI, GitHub Copilot, Amp · [Repo](https://github.com/bloopai/vibe-kanban) · [📖 Docs ↗](https://vibekanban.com/docs) · [🌐 Site ↗](https://vibekanban.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-kanban/)</sub>

<a name="opencursor"></a>
### #&#8288;79 [opencursor](https://github.com/pawanosman/opencursor) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Sep 2026</sub>

**AI coding agent extension for VS Code with bring-your-own models.**

OpenCursor is a VS Code extension that adds an agent chat able to read and edit files, search code, run terminal commands and check browser behavior. It connects to subscription accounts, API keys, custom OpenAI- or Anthropic-compatible endpoints, or local Ollama and llama.cpp models. Edits can be reviewed per hunk and kept or undone, with permission controls for actions.

- **+** Many providers: OpenAI, Anthropic, Gemini, OpenRouter, DeepSeek, plus Claude Code and Copilot accounts
- **+** Local inference via Ollama or llama.cpp with GGUF download, plus local embeddings for code search
- **+** Per-hunk change review with Keep All and Undo All, and Ask, Plan and Agent modes
- **+** Supports MCP servers, hooks, skills, subagents and Git worktrees; MIT licensed
- **−** Runs only inside VS Code 1.96 or newer; no standalone editor or CLI
- **−** Account-based providers depend on third-party login flows that may change or be restricted
- **−** Some features download native runtimes or models on first use, which breaks offline setup
- **−** Web search, doc fetching, browser tools and remote workers need external services

<sub>GPU optional · Needs VS Code 1.96+, Node.js 22 and pnpm (build from source), Ollama or llama.cpp (optional, local models), Chrome or Edge (browser tools), Docker (optional, command execution) · Models: OpenAI, Anthropic, Google Gemini, OpenRouter, xAI · [Repo](https://github.com/pawanosman/opencursor) · [🌐 Site ↗](https://marketplace.visualstudio.com/items?itemName=pkrd.ocursor) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencursor/)</sub>

<a name="design-extract"></a>
### #&#8288;80 [design-extract](https://github.com/manavarya09/design-extract) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Oct 2026</sub>

**CLI that extracts a website's design system into tokens, Tailwind and Figma files.**

designlang drives a headless Chromium against a URL and reads colors, type, spacing, layout, motion and component structure from the live DOM. It writes 17+ files, including W3C DTCG tokens, a Tailwind config, a shadcn theme, Figma variables and prompt packs for v0, Lovable and Cursor. It also covers site-wide crawls, clone fidelity scoring, drift checks, a Claude Code plugin and a stdio MCP server.

- **+** Emits many formats per run: DTCG, Tailwind, shadcn CSS, Figma variables, typed React stubs
- **+** Measures clones with pixel diff plus motion comparison, with a --min flag usable as a CI gate
- **+** Ships a Claude Code plugin and an MCP server (designlang mcp) for agent use
- **+** Core extraction runs locally and deterministically; the API key is only needed for --smart
- **−** Needs a separate Chromium download via install-browser, or an installed Google Chrome
- **−** Authenticated pages need cookies or headers passed by hand
- **−** The README lists a very large command surface, which makes it hard to know where to start
- **−** --smart classification needs an external OpenAI-compatible or Anthropic API key

<sub>no GPU · Docker · Needs Node.js, Chromium via Playwright or Google Chrome, Optional: Atlas Cloud, OpenAI or Anthropic API key for --smart · Models: OpenAI-compatible chat API (Atlas Cloud), OpenAI, Anthropic · [Repo](https://github.com/manavarya09/design-extract) · [▶️ Demo ↗](https://designlang.app/watch) · [🌐 Site ↗](https://designlang.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/design-extract/)</sub>

<a name="openbitfun"></a>
### #&#8288;81 [openbitfun](https://github.com/gcwing/openbitfun) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Desktop agent workspace with phone remote control and agent-built Mini Apps.**

OpenBitFun is a Tauri desktop app (Windows, macOS, Linux) with a Rust agent runtime that handles session state, context and tool execution. It offers four harness modes, from Minimal for quick tasks to Creative for building Mini Apps, works on remote hosts over SSH, and can be controlled from a phone or browser through a Relay server you deploy. Agents extend via MCP, Skills and Hooks.

- **+** Rust runtime with persistent sessions, interruption recovery and context compression
- **+** Remote control from phone or browser; tasks keep running on the selected host
- **+** Extensible through MCP, Skills, Hooks, custom agents, skins and Mini Apps
- **+** README reports DeepSWE v1.1 pass rates of 64.6% (GLM-5.3-Flash) and 56.6% (DeepSeek-V4-Flash)
- **−** Cross-device sync and control require deploying your own Relay server
- **−** 1.0.0 is not data-compatible with 0.2.x; migration tool covers only 0.2.17-0.2.19
- **−** Only core code is MIT; third-party dependencies and assets keep their own licenses
- **−** README gives no RAM or GPU figures; community contact is a WeChat group

<sub>Compose · Needs Relay server (for cross-device sync), Node.js 22.12+ (source build), pnpm 10.15.0 (source build), Rust toolchain (source build), Tauri prerequisites (source build) · Models: GLM-5.3-Flash, DeepSeek-V4-Flash, MCP tools · [Repo](https://github.com/gcwing/openbitfun) · [📖 Docs ↗](https://playbook.openbitfun.com) · [🌐 Site ↗](https://openbitfun.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openbitfun/)</sub>

<a name="little-coder"></a>
### #&#8288;82 [little-coder](https://github.com/itayinbarr/little-coder) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · Apache-2.0 · Sep 2026</sub>

**Terminal coding agent tuned for small local models, built on pi.**

little-coder is a terminal coding agent that adds about 30 extensions and 30 skill markdown files to the pi agent runtime. It targets small local models, with Qwen3.6-35B-A3B on llama.cpp as the default, and also works with Ollama, LM Studio, other OpenAI-compatible servers and cloud providers. It includes plan mode, deep research, read-only sub-coders, background jobs and per-phase model selection.

- **+** Default setup runs Qwen3.6-35B-A3B on 8 GB VRAM by keeping MoE experts in RAM
- **+** Works with llama.cpp, Ollama, LM Studio, any OpenAI-compatible server and cloud providers
- **+** Small-model extensions auto-disable for large or cloud models; cold-start context is about 7k tokens
- **+** Separate plan and action models via /plan-model and /action-model; read-before-edit enforced
- **−** Requires Node.js 22.19+ even when installed with bun
- **−** Globally installed pi packages do not load unless you opt in via flag or env var
- **−** Dense Qwen3.8-27B measured about 6.4 tok/s on 8 GB VRAM versus about 44 for the MoE
- **−** Local setup means building llama.cpp and downloading a roughly 22 GB model yourself

<sub>GPU optional · Needs Node.js 22.19+, pi, llama.cpp, Ollama or LM Studio (for local models) · Models: llama.cpp (GGUF), Ollama, LM Studio, OpenAI-compatible servers, Anthropic · [Repo](https://github.com/itayinbarr/little-coder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/little-coder/)</sub>

<a name="org2"></a>
### #&#8288;83 [org2](https://github.com/org2ai/org2) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · AGPL-3.0 · Oct 2026</sub>

**Desktop app that runs coding agents and records replayable session trajectories.**

ORG-2 is a Tauri and Rust desktop app with its own native agent harness and launchers for 20+ coding agent CLIs, such as Claude Code, Codex and Aider. It records each session as a replayable trajectory, ingests history from other tools, and traces shipped lines back to the sessions that wrote them ("AI blame"). Teams can share sessions and comment on trajectories.

- **+** Replays messages, tool calls, file edits and command output on one timeline
- **+** Ingests and backfills session history from 10+ other apps and CLIs
- **+** AI blame traces code back to agent sessions and tool calls
- **+** Installers for macOS Apple Silicon, Windows and Linux; under 100MB on disk
- **−** Session sharing and group issues rely on self-hosted Supabase and are marked WIP
- **−** Issue and project alignment features are marked WIP
- **−** Computer Use is macOS only; the macOS build is Apple Silicon only
- **−** AGPL license may restrict use in closed-source products

<sub>no GPU · Needs Supabase (self-hosted, for collaboration, WIP), agent-browser (optional sidecar), peekaboo (optional, macOS), API keys or agent CLI subscriptions · Models: Claude Code, Codex, Cursor CLI, GitHub Copilot, Aider · [Repo](https://github.com/org2ai/org2) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/org2/)</sub>

<a name="nodeterm"></a>
### #&#8288;84 [nodeterm](https://github.com/eneskirca/nodeterm) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · custom license · Oct 2026</sub>

**Electron terminal manager with terminals and agents as nodes on a canvas.**

nodeterm places real terminals (xterm over tmux), coding-agent sessions, sticky notes, Monaco editors and diff views as draggable nodes on a pan/zoom canvas. Each project can also be shown as a kanban board whose cards are live sessions, with hook-driven RUNNING / NEEDS YOU status. It runs as an Electron desktop app or a self-hosted browser Server Edition, and pairs with an iOS companion app.

- **+** Sessions persist across app restarts and reboots via tmux; macOS build ships its own tmux
- **+** Agent status comes from hooks, not output scraping, with OS notifications and context meter
- **+** Supports Claude Code, Codex, Gemini, Copilot, opencode, Grok, Cursor and custom agents
- **+** Same renderer runs as desktop app or browser Server Edition; local Whisper dictation
- **−** License is BUSL-1.1 (source-available), not an OSI open-source license
- **−** Windows build is beta: unsigned installer, manual updates, no session continuity across restarts yet
- **−** Server Edition is single-user (password auth) and needs Node 22 plus tmux
- **−** Notch integration and the iOS companion app are Apple-only

<sub>no GPU · Docker · Needs tmux, Node.js 20+ (build from source), Node.js 22 (Server Edition), git · Models: Claude Code, Codex, Gemini, GitHub Copilot, opencode · port 8443 · [Repo](https://github.com/eneskirca/nodeterm) · [📖 Docs ↗](https://nodeterm.dev/docs) · [🌐 Site ↗](https://nodeterm.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nodeterm/)</sub>

<a name="ralph-claude-code"></a>
### #&#8288;85 [ralph-claude-code](https://github.com/frankbria/ralph-claude-code) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · MIT · Oct 2026</sub>

**Shell loop that reruns Claude Code until a task list is finished.**

Ralph is a set of shell commands that re-runs Claude Code in a loop against a PROMPT.md and a fix_plan.md task list until the work is done. It exits only when heuristic completion indicators and an explicit EXIT_SIGNAL both agree. It adds rate limiting (100 calls/hour by default), a circuit breaker, session resume and a tmux monitor. Projects are set up with ralph-enable, ralph-import or ralph-setup.

- **+** Dual-condition exit gate (indicators plus EXIT_SIGNAL) reduces premature stops
- **+** Rate limit, circuit breaker and 5-hour API limit handling for unattended runs
- **+** Imports tasks from PRDs, GitHub issues or beads; ralph-enable detects project type
- **+** Optional Docker and E2B sandbox execution; 784 tests reported
- **−** Tied to the claude CLI; multi-provider support is still in progress
- **−** Breaking changes between versions, including .ralph/ layout and .ralphrc parsing
- **−** No tagged releases on the repository
- **−** Exit detection relies partly on heuristics; loops consume API quota

<sub>no GPU · Docker · Needs Claude Code CLI, tmux, git, Docker (optional), E2B (optional) · Models: Claude (via Claude Code) · [Repo](https://github.com/frankbria/ralph-claude-code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph-claude-code/)</sub>

<a name="claude-code-action"></a>
### #&#8288;86 [claude-code-action](https://github.com/anthropics/claude-code-action) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (71) · Freshness: recent (80) · Maintenance: fair (75) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · MIT · Oct 2026</sub>

**GitHub Action that runs Claude Code on PRs and issues via @claude mentions.**

A GitHub Action that runs Claude Code on your own runner to answer questions, review PR changes and implement code changes. It triggers on @claude mentions, issue assignments or explicit prompts. It authenticates against the Anthropic API (API key or workload identity federation), Amazon Bedrock, Google Vertex AI or Microsoft Foundry, and can emit structured JSON as Action outputs.

- **+** Runs on your own GitHub runner; API calls go only to the provider you choose
- **+** Supports Anthropic API, Bedrock, Vertex AI and Microsoft Foundry authentication
- **+** Picks execution mode from workflow context: mention, assignment or automation prompt
- **+** Structured JSON outputs become GitHub Action outputs for downstream steps
- **−** Guided /install-github-app quickstart works only for direct Anthropic API users
- **−** Installing the GitHub app and adding secrets requires repository admin rights
- **−** README claims only simple fixes, refactors and features; larger change limits are unspecified
- **−** Last tagged release is 2025-08-26, well behind recent commits

<sub>no GPU · Needs GitHub Actions runner, Claude GitHub app, Anthropic API, Amazon Bedrock, Google Vertex AI or Microsoft Foundry · Models: Claude (Anthropic API), Amazon Bedrock, Google Vertex AI, Microsoft Foundry · [Repo](https://github.com/anthropics/claude-code-action) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-action/)</sub>

<a name="agent-teams-ai"></a>
### #&#8288;87 [agent-teams-ai](https://github.com/777genius/agent-teams-ai) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · AGPL-3.0 · Oct 2026</sub>

**Desktop app that runs teams of coding agents on a kanban board.**

Agent Teams AI is an Electron-style desktop app (TypeScript) that orchestrates multiple AI agents with distinct roles working in parallel on a kanban board. It drives Claude Code, Codex, OpenCode and other providers such as Cursor, GitHub Copilot, Z.AI, MiniMax and Kiro, and includes per-task logs, diff review, a terminal, and token budgets. Agents message each other, including across teams, and can run in separate git worktrees.

- **+** Kanban board with per-task logs, comments and agent-to-agent review in one app
- **+** Per-action tool approvals or fully autonomous mode, selectable per team
- **+** Token analytics with monthly token or cost budgets and alerts at 80% and 100%
- **+** Installers for macOS, Windows and Linux (.AppImage, .deb, .rpm, .pacman); free model needs no key
- **−** AGPL-3.0 license limits use in closed-source derivative services
- **−** Desktop only; no server or web deployment described in the README
- **−** Depends on third-party runtimes and subscriptions for most providers
- **−** Windows installer triggers SmartScreen; OpenCode may need admin rights on symlink errors

<sub>no GPU · Docker + Compose · Needs Claude Code, Codex or OpenCode runtime (optional), Provider subscription or API key (optional), git · Models: Claude Code, Codex, OpenCode, Cursor, SuperGrok · [Repo](https://github.com/777genius/agent-teams-ai) · [▶️ Demo ↗](https://agentteams.live/) · [🌐 Site ↗](https://agentteams.live/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-teams-ai/)</sub>

<a name="traycer"></a>
### #&#8288;88 [traycer](https://github.com/traycerai/traycer) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Desktop app that runs multiple coding agents in parallel with shared context.**

Traycer is a desktop app that connects to coding agents you already subscribe to, such as Claude Code, Codex, Cursor, OpenCode and Copilot, and runs several in parallel. It shares context across models and providers, lets you switch models within an agent, and supports agent-to-agent messaging. Shareable boards and ticket assignment cover team use.

- **+** Connects to 25+ existing coding agents, including Claude Code, Codex, Cursor and Copilot
- **+** Switch models within one agent while keeping the same context window
- **+** Native installers for macOS (arm64, x64), Linux (AppImage, deb, rpm) and Windows
- **+** Shareable boards, ticket assignment and real-time editing for teams
- **−** Agent-to-agent transcript reading and message delivery vary by user, host and runtime
- **−** Release builds may enable Sentry crash reporting and PostHog analytics
- **−** Privacy Mode is opt-in for individuals; with it off, prompts may be logged
- **−** Hardware requirements (RAM, GPU) are not documented in the README

<sub>Needs Coding agent subscriptions (Claude Code, Codex, Cursor, etc.) or Traycer inference subscription · Models: Claude Code, Codex, Cursor, OpenCode, GitHub Copilot · [Repo](https://github.com/traycerai/traycer) · [▶️ Demo ↗](https://youtu.be/doh2yz3ZFvU) · [📖 Docs ↗](https://docs.traycer.ai) · [🌐 Site ↗](https://traycer.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/traycer/)</sub>

<a name="wally"></a>
### #&#8288;89 [wally](https://github.com/runanywhereai/wally) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**CLI that launches coding agents preconfigured for a hosted or local model.**

Wally is a Rust command-line tool that opens a coding agent (OpenCode, Claude Code, Hermes, OpenClaw and others) already wired to a chosen model, installing the agent if missing. Models can be hosted (default glm-5.3-flash, billed to RunAnywhere credit) or open models downloaded and run locally without an account. It also offers terminal chat, an OpenAI-compatible API server, and a `decisions` command for scoring labels with the Eve model.

- **+** One command launches a coding agent and installs it first if it is missing
- **+** Runs hosted models or local open models; local use needs no account
- **+** Also provides terminal chat and an OpenAI-compatible API server
- **+** Supports macOS, Linux and Windows, including x64 and ARM64
- **−** Hosted models require a RunAnywhere login and are billed against its credit
- **−** Intel Macs unsupported; Linux needs glibc 2.39 or newer
- **−** Eve decision model is hosted by default; local use needs a separate checkpoint pull
- **−** Building from source needs CMake and a prebuilt RunAnywhere C++ desktop kit

<sub>Needs RunAnywhere account (hosted models only) · Models: glm-5.3-flash (hosted), clef-flash-9b (local), eve (decision model), open models via local download · [Repo](https://github.com/runanywhereai/wally) · [📖 Docs ↗](https://docs.runanywhere.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wally/)</sub>

<a name="screenshot-to-code"></a>
### #&#8288;90 [screenshot-to-code](https://github.com/abi/screenshot-to-code) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 81k · MIT · Oct 2026</sub>

**Turns screenshots and mockups into Tailwind, React or Vue code.**

Takes a screenshot, mockup, Figma export or screen recording and generates HTML with Tailwind or CSS, React, Vue, Bootstrap or Ionic code using Gemini 3, GPT-5.5 or Claude Opus models, with Replicate for image generation and background removal. Runs as a React/Vite frontend on port 5173 and a FastAPI backend on 7001, or via docker-compose. For developers prototyping UIs from designs.

- **+** Six output stacks including React, Vue, Bootstrap and Ionic with Tailwind
- **+** Video mode turns a screen recording into a working prototype (needs Gemini)
- **+** Optional headless Chromium lets the agent render and check its own output
- **+** docker-compose brings up frontend and backend with one env file
- **−** Requires at least one OpenAI, Anthropic or Gemini API key; no bundled local model
- **−** Ollama models are possible but the README calls the results poor quality
- **−** Replicate key must be set in backend/.env, not in the UI
- **−** Docker setup has no hot reload; file changes need a rebuild

<sub>no GPU · Compose · Needs OpenAI, Anthropic or Gemini API key, Replicate API key (optional), Playwright Chromium (optional preview) · Models: Gemini 3 Flash Preview, Gemini 3.1 Pro Preview, GPT-5.5, GPT-5.4 Mini, Claude Opus 4.6/4.8 · port 5173 · [Repo](https://github.com/abi/screenshot-to-code) · [▶️ Demo ↗](https://screenshottocode.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/screenshot-to-code/)</sub>

<a name="grok-build"></a>
### #&#8288;91 [grok-build](https://github.com/xai-org/grok-build) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

**Terminal coding agent from SpaceXAI with a full-screen TUI, written in Rust.**

Grok Build is the source for the `grok` CLI, a full-screen terminal agent that reads your codebase, edits files, runs shell commands and searches the web. It runs interactively, headlessly for scripts and CI, or inside editors through the Agent Client Protocol (ACP). The bundled user guide covers MCP servers, skills, plugins, hooks and sandboxing.

- **+** Three run modes: interactive TUI, headless for scripting and CI, and ACP for editors
- **+** Prebuilt binaries for macOS, Linux and Windows via a one-line install script
- **+** Supports MCP servers, skills, plugins and hooks, per the bundled user guide
- **+** Apache-2.0 first-party code, with third-party notices documented in the repo
- **−** External contributions are not accepted
- **−** Repo is synced periodically from a private monorepo, not developed in the open
- **−** Browser authentication on first launch; supported models are not listed in the README
- **−** Windows source builds are untested; building needs DotSlash and protoc

<sub>no GPU · Needs Rust toolchain (build from source), DotSlash (build from source), protoc (build from source) · [Repo](https://github.com/xai-org/grok-build) · [📖 Docs ↗](https://docs.x.ai/build/overview) · [🌐 Site ↗](https://x.ai/cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/grok-build/)</sub>

<a name="anus"></a>
### #&#8288;92 [anus](https://github.com/anus-dev/anus) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Oct 2026</sub>

**Terminal coding agent that routes requests across free-tier LLM APIs.**

ANUS is a terminal coding agent built on the pi engine. It reads code, edits files and runs shell commands, sending each request to the highest-ranked free model you have a key for and falling back to the next when one is rate-limited or fails mid-answer. The ranked list refreshes twice a day from anus.dev/free-models.json.

- **+** Automatic fallback across free models when one hits a rate limit or cuts off
- **+** Ignores paid keys in the shell unless ANUS_ENV_KEYS=1 is set
- **+** Keys, sessions and settings stay in ~/.anus/agent; sends data only to providers you configure
- **+** Installs with npm or a curl script; non-interactive mode via anus -p
- **−** Free tiers are capped, e.g. OpenRouter 50 requests a day without a $10 top-up
- **−** Some free providers may train on your prompts and code
- **−** Model quality varies by day, since routing depends on which free model is awake
- **−** Depends on a remote ranked list at anus.dev; free tiers change often

<sub>no GPU · Needs Node.js 22.19+, At least one free API key (OpenRouter, Gemini, Groq, Mistral or Cerebras) · Models: OpenRouter free models, Google Gemini, Groq, Cerebras, Mistral · [Repo](https://github.com/anus-dev/anus) · [🌐 Site ↗](https://anus.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/anus/)</sub>

<a name="zcode"></a>
### #&#8288;93 [zcode](https://github.com/zai-org/zcode) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · Apache-2.0 · Oct 2026</sub>

**AI coding workbench with desktop app, browser UI and terminal agent.**

ZCode is a TypeScript monorepo containing an Electron desktop client, a web client, an HTTP/WebSocket backend, and an agent CLI with a TUI. The packaged `zcode` command starts the TUI by default or a local web UI with `--web`. The README documents build and dev workflows in detail but does not list supported models or providers.

- **+** Desktop (Electron), browser and terminal TUI share one agent runtime and backend
- **+** `zcode --web` runs locally with no Electron; binds 127.0.0.1 by default
- **+** Token auth is generated automatically when listening on non-local addresses
- **+** Agent CLI source is in-repo, no submodule; UI plugin system documented
- **−** README is primarily in Chinese; English version is a separate file
- **−** Pinned toolchain: Node.js 24.14.0 and pnpm 10.33.2 required to build
- **−** Packaging the CLI needs a self-hosted download base URL set first
- **−** Supported models and providers are not listed in the README

<sub>Docker · Needs Node.js 24.14.0, pnpm 10.33.2, Electron (desktop) · port 3030 · [Repo](https://github.com/zai-org/zcode) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zcode/)</sub>

<a name="costrict"></a>
### #&#8288;94 [costrict](https://github.com/zgsm-ai/costrict) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Sep 2026</sub>

**AI coding assistant for VS Code, JetBrains and CLI with a spec-driven workflow.**

CoStrict is an AI coding assistant that runs as a VS Code extension, a JetBrains plugin and a CLI. Its Strict Mode walks through requirements analysis, architecture design, task planning and test generation. It also offers free-form chat coding, repository-wide RAG code review, MCP, skills and OpenSpec integration. It connects to Anthropic, OpenAI, OpenAI-compatible APIs and local models.

- **+** Strict Mode enforces requirements, design, task planning and test steps before code generation
- **+** Ships as VS Code extension, JetBrains plugin and CLI
- **+** Accepts Anthropic, OpenAI, OpenAI-compatible and local models, plus built-in free models
- **+** Supports MCP, skills and OpenSpec change proposals
- **−** JetBrains plugin lives in a separate repository
- **−** README gives no hardware requirements or deployment details; those are in external docs
- **−** Built on Roo Code and OpenCode, so features overlap with those projects
- **−** Built-in free models are not named and their limits are not described

<sub>Needs VS Code or JetBrains IDE · Models: Anthropic, OpenAI, OpenAI-compatible APIs, local models · [Repo](https://github.com/zgsm-ai/costrict) · [📖 Docs ↗](https://docs.costrict.ai/en/guide/installation) · [🌐 Site ↗](https://costrict.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/costrict/)</sub>

<a name="background-agents"></a>
### #&#8288;95 [Background Agents](https://github.com/colemurray/background-agents) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Self-hosted background coding agent that runs tasks in cloud sandboxes and opens PRs.**

Open-Inspect is an open-source implementation of Ramp's Inspect design. A Cloudflare Workers and Durable Objects control plane runs coding agents (OpenCode or Claude Agent harness) in sandboxes on Modal, Daytona, E2B or Vercel. Sessions start from a Next.js web UI, Slack, GitHub, Linear or webhooks, and can be scheduled or triggered by events. Commits are attributed to the prompting user.

- **+** Triggers from web, Slack, GitHub PRs, Linear issues, webhooks, cron and Sentry alerts
- **+** Multiplayer sessions with prompts attributed to authors in git commits
- **+** Parallel child sessions in separate sandboxes; one session can span up to 10 repos
- **+** Filesystem snapshots and prebuilt images rebuilt every 30 minutes for fast startup
- **−** Single-tenant only; multi-tenant needs per-tenant GitHub App installs and isolation work
- **−** Requires Cloudflare plus a sandbox provider account (Modal, Daytona, E2B or Vercel)
- **−** Credentials are cached on disk, so snapshots can retain them; grant removal does not revoke tokens
- **−** GitLab access uses one deployment-wide PAT rather than per-session tokens

<sub>no GPU · Compose · Needs Cloudflare Workers, Cloudflare Durable Objects, Cloudflare D1, GitHub App, Modal, Daytona, E2B or Vercel Sandbox · Models: Anthropic Claude, OpenAI Codex (ChatGPT subscription), xAI Grok (SuperGrok), OpenCode Zen and Go, Z.AI Coding Plan · [Repo](https://github.com/colemurray/background-agents) · [📖 Docs ↗](https://github.com/colemurray/background-agents/blob/main/docs/GETTING_STARTED.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/background-agents/)</sub>

<a name="tau"></a>
### #&#8288;96 [tau](https://github.com/huggingface/tau) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**Python terminal coding agent with a small, layered, readable codebase.**

Tau is a terminal coding agent that reads files, edits code and runs shell commands from a Textual TUI or a one-shot print mode. Sessions are stored as append-only JSONL under ~/.tau/sessions/. The code is split into three packages (tau_ai, tau_agent, tau_coding), so the agent harness can be reused as a library. It is also written as a teaching example of how coding agents are built.

- **+** Three-layer split lets the tau_agent harness run without the CLI or TUI
- **+** Durable JSONL sessions with resume, branching and compaction
- **+** Supports OpenAI, Anthropic, OpenRouter, Hugging Face and OpenAI-compatible endpoints
- **+** Reads AGENTS.md, .tau/ and .agents/ resources; supports skills and prompt templates
- **−** Only four built-in tools: read, write, edit and bash
- **−** README says it is under active development
- **−** Requires Python 3.12 or newer
- **−** README does not mention MCP support

<sub>no GPU · Needs Python 3.12+, uv (installed by the install script), model provider account or endpoint · Models: OpenAI, Anthropic, OpenAI Codex subscription, OpenRouter, Hugging Face · [Repo](https://github.com/huggingface/tau) · [📖 Docs ↗](https://twotimespi.dev/quickstart/) · [🌐 Site ↗](https://twotimespi.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tau/)</sub>

<a name="ovis"></a>
### #&#8288;97 [ovis](https://github.com/devswha/ovis) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Browser and phone client for herdr agent sessions, with chat and terminal views.**

Ovis is a herdr plugin that serves a web app and installable PWA for the Claude Code, Codex and other agent panes already running on your computer. It reads each agent's own transcript as a chat, turns supported approvals and questions into tappable cards, and keeps the live terminal one click away. It also sends push alerts, shows repository diffs and can attach other PCs over SSH.

- **+** Reads native session transcripts for Claude Code, Codex, omp, omo, gjc, pi and Hermes
- **+** Approvals and questions become cards, checked as current before the answer is sent
- **+** Phone PWA with push alerts, customizable key bar and QR pairing over Tailscale
- **+** Terminal stays attached to the same panes as herdr's TUI, so nothing is handed over
- **−** Works only with herdr 0.9.0+; no tmux or zellij support
- **−** Linux glibc and macOS only for the shell installer; no Alpine/musl or 32-bit ARM
- **−** Windows terminal is a screen mirror with fixed grid until herdr supports attach
- **−** Grok chat is Linux-only; Antigravity is experimental; unsupported sessions fall back to terminal

<sub>no GPU · Needs herdr 0.9.0+, Bun 1.4+, Node 18+ (not on Windows), Git, Tailscale (optional) · Models: Claude Code, Codex, OpenCode, omp, omo · port 7317 · [Repo](https://github.com/devswha/ovis) · [▶️ Demo ↗](https://ovis.sh/demo/) · [📖 Docs ↗](https://github.com/devswha/ovis/blob/main/docs/guide.md) · [🌐 Site ↗](https://ovis.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ovis/)</sub>

<a name="twinny"></a>
### #&#8288;98 [twinny](https://github.com/twinnydotdev/twinny) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**VS Code assistant for completion, chat and edits against your own model server.**

twinny is a VS Code extension that provides fill-in-the-middle completion, inline diff edits, chat with @-attached context, an experimental agent mode, workspace indexing and code review. It connects to local servers (Ollama, LM Studio, llama.cpp), paired devices, hosted APIs, or a shared twinny-server gateway for teams. It has no telemetry or sign-in; the gateway is free for five developers and paid per seat beyond that.

- **+** Works with Ollama, LM Studio, llama.cpp, OpenAI-compatible servers, and hosted APIs like OpenAI and Anthropic
- **+** No telemetry and no account; prompts go only to the server you configure
- **+** Inline edits shown as diffs with per-hunk accept or reject
- **+** Team gateway runs via npx with per-developer keys and usage metrics
- **−** VS Code only (1.93 or newer); no other editors mentioned
- **−** Agent mode is labelled experimental
- **−** Team policy, recording, plugins and SSO need a paid licence ($15 per seat per month)
- **−** Maintained by one person; README says provided as is

<sub>GPU optional · Needs VS Code 1.93+, Model server (Ollama, LM Studio, llama.cpp, or hosted API) · Models: Ollama, LM Studio, llama.cpp, OpenAI-compatible servers, OpenAI · [Repo](https://github.com/twinnydotdev/twinny) · [📖 Docs ↗](https://docs.twinny.dev/) · [🌐 Site ↗](https://twinny.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/twinny/)</sub>

<a name="claude-codex-bridge"></a>
### #&#8288;99 [claude_codex_bridge](https://github.com/seemseam/claude_codex_bridge) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (46) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · custom license · Oct 2026</sub>

**Terminal workspace running Codex, Claude, Gemini and other CLI agents side by side.**

CCB is a multi-agent terminal UI that mounts coding-agent CLIs (Codex, Claude, Gemini and 13 other families) in visible panes and lets them hand work to each other with /ask. A background daemon keeps project state alive, and per-agent FIFO queues avoid colliding with a human's draft. It also ships an Android remote-control app and an optional rich file-browser mode.

- **+** Supports 16 CLI agent families, mixed in one project via .ccb/ccb.config
- **+** Native interactive panes let you take over any agent directly
- **+** Queue mode holds agent replies while you type a draft (tested with Claude, Codex, OMP)
- **+** Android app offers voice input, file transfer and terminal access via Tailscale Serve or LAN
- **−** Draft protection is only recommended and tested for Claude, Codex and OMP in managed tmux panes
- **−** Queue mode is described as a first test version; Ctrl-C draft clearing can still interrupt
- **−** Native Windows support is beta, needs WezTerm, Git Bash and Herdr, with unsigned binaries
- **−** License is not identified (NOASSERTION) and the README excerpt does not state one

<sub>no GPU · Needs tmux, Provider CLIs (Codex, Claude, Gemini, etc.), npm, Python 3.10+ (Windows beta), WezTerm (rich mode, Windows beta), Tailscale (remote mobile access) · Models: Codex, Claude, Gemini, Pi, OMP · [Repo](https://github.com/seemseam/claude_codex_bridge) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-codex-bridge/)</sub>

<a name="monocode"></a>
### #&#8288;100 [monocode](https://github.com/hardbeat920/monocode) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Desktop GUI that runs installed coding agent CLIs in tabbed, split-pane sessions.**

MonoCode is a Tauri desktop app (TypeScript and Rust) that wraps coding agents you have already installed and signed in to, such as Claude Code, Codex, Cursor, OpenCode and Devin. Each tab is a session, panes can be split, and work can be organized by project with separate Git worktrees and in-app file editing and change review. It does not sell tokens, so usage goes through your existing agent subscriptions.

- **+** Supports eleven agents including Claude Code, Codex, Cursor, OpenCode and Devin from one interface
- **+** Uses your existing agent logins; the app does not resell tokens
- **+** Per-task Git worktrees and side-by-side split panes for parallel sessions
- **+** Prebuilt installers for macOS (Apple Silicon and Intel), Linux and Windows
- **−** Requires at least one supported agent installed and signed in beforehand
- **−** README calls the project early; Monos agents and remote sessions are experimental
- **−** Not a standalone agent; no model or provider support of its own
- **−** Linux needs extra dependencies; setup is documented separately

<sub>no GPU · Needs At least one supported coding agent CLI, installed and logged in, Node.js 20+ and Rust toolchain (build from source only) · Models: Claude Code, Codex, Cursor, Grok Build, OpenCode · [Repo](https://github.com/hardbeat920/monocode) · [📖 Docs ↗](https://github.com/hardbeat920/monocode/blob/main/docs/providers.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/monocode/)</sub>

<a name="nimbalyst"></a>
### #&#8288;101 [nimbalyst](https://github.com/nimbalyst/nimbalyst) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Desktop workspace for running and reviewing Codex and Claude Code sessions.**

Nimbalyst is an Electron desktop app for macOS, Windows and Linux that wraps coding agents (Codex, Claude Code, plus OpenCode and Copilot in alpha) in one UI. It runs parallel sessions in separate git worktrees and tracks them on a kanban board. It also provides WYSIWYG editors for markdown, mockups, Mermaid, Excalidraw and CSV, with red/green diff review of agent edits. An iOS companion app handles replies and approvals.

- **+** Parallel agent sessions, each isolated in its own git worktree
- **+** Accept or reject agent edits as diffs in rendered documents, not just raw code
- **+** Stores content as plain files in your git repo, no proprietary store
- **+** Extension SDK where built-in and custom editors share the same EditorHost contract
- **−** OpenCode and Copilot support is alpha
- **−** Collaboration sync server is a separate project, hosted at sync.nimbalyst.com
- **−** Sends anonymous PostHog analytics by default; opt-out is in Settings
- **−** Desktop app only, with no Docker or browser deployment

<sub>no GPU · Needs Codex or Claude Code CLI/account, Node 24 and pnpm (build from source only) · Models: Codex, Claude Code, OpenCode (alpha), GitHub Copilot (alpha), Gemini · [Repo](https://github.com/nimbalyst/nimbalyst) · [📖 Docs ↗](https://docs.nimbalyst.com/) · [🌐 Site ↗](https://nimbalyst.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nimbalyst/)</sub>

<a name="lody"></a>
### #&#8288;102 [lody](https://github.com/lodyai/lody) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Oct 2026</sub>

**Shared team workspace for dispatching and reviewing ACP-compatible coding agents.**

Lody connects machines you own to a shared workspace. Teammates can dispatch, watch and review coding-agent sessions (Claude Code, Codex, Kimi, OpenCode or any ACP agent) from desktop, mobile, web or CLI. Sessions can use separate Git worktrees and show diffs and PR/CI status. Machines connect with `npx lody daemon start`.

- **+** Works with any ACP-compatible agent, reusing existing local logins and subscriptions
- **+** Per-session Git worktrees, diffs, line comments and PR/CI status beside the conversation
- **+** Clients for desktop, iOS, Android, web and CLI; CLI commands support --json
- **+** Machines stay private until the owner shares them with the workspace
- **−** README does not document self-hosting; sign-in goes through a Lody link
- **−** Local-first sync is unfinished; the README says it is still moving toward it
- **−** E2EE library exists but is not yet wired into the product
- **−** No Docker or compose files; setup details live in external docs

<sub>no GPU · Needs Node.js (npx), ACP-compatible coding agent, Git, GitHub · Models: Claude Code, Codex, Kimi, OpenCode, ACP-compatible agents · [Repo](https://github.com/lodyai/lody) · [📖 Docs ↗](https://lody.ai/docs/) · [🌐 Site ↗](https://lody.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lody/)</sub>

<a name="omnirush-gui"></a>
### #&#8288;103 [omnirush-gui](https://github.com/omnirush-ai/omnirush-gui) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · custom license · Oct 2026</sub>

**Desktop coding agent app for macOS and Linux with a model picker.**

Electron-style desktop app that runs a coding agent against your local projects. It clones repos, branches, commits, pushes and opens or reviews pull requests through `gh`, with approval prompts for write and destructive commands. Prompts run only after signing in to an omnirush.ai account, though you can add your own OpenAI, Anthropic or other provider keys.

- **+** Per-chat model and effort selection (low, high, xhigh, max)
- **+** Skills and MCP servers added from a Library in Settings, shared across models
- **+** Git workflow support with approval prompts; destructive commands always ask
- **+** Packages for macOS arm64 and Linux x64/arm64 (deb, rpm, pacman, AppImage, tar.gz)
- **−** Requires an omnirush.ai account sign-in before any prompt runs
- **−** No build for Intel Macs or Windows
- **−** macOS builds are not notarized; first launch needs a manual override
- **−** License detected as NOASSERTION; README cites MIT with a separate ee/ license

<sub>no GPU · Needs omnirush.ai account, gh CLI (for pull request workflows), GTK runtime libraries (AppImage/tar.gz on Linux) · Models: GPT 6 Astra, GPT 6.1 Sol, OpenAI (own key), Anthropic (own key) · [Repo](https://github.com/omnirush-ai/omnirush-gui) · [🌐 Site ↗](https://omnirush.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omnirush-gui/)</sub>

<a name="holyclaude"></a>
### #&#8288;104 [holyclaude](https://github.com/coderluii/holyclaude) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

**Container image bundling Claude Code, a web UI, headless Chromium and other AI CLIs.**

HolyClaude is a Docker image that runs the official Claude Code CLI behind the CloudCLI web UI on port 3001. It bundles Chromium with Xvfb and Playwright, s6-overlay process supervision, 8 AI CLIs (including Gemini CLI, Codex, Cursor and OpenCode) and 50+ dev tools. Config and workspace are bind-mounted so auth and code survive rebuilds.

- **+** Runs the real Claude Code CLI; Max/Pro OAuth or an API key both work
- **+** Chromium, Xvfb and Playwright preconfigured, with shm_size set to 2g
- **+** amd64 and arm64 images, with full and slim tags plus pinned versions
- **+** Settings and workspace bind-mounted, so they survive container rebuilds
- **−** Compose template needs SYS_ADMIN, SYS_PTRACE and seccomp=unconfined, a weak isolation profile
- **−** Full image bundles many tools; compressed size not stated in the README
- **−** Kubernetes/Helm support is only planned
- **−** Accepted upstream vulnerabilities remain in dependency scans, per the README warning

<sub>no GPU · Docker + Compose · Needs Docker, Docker Compose, Anthropic account or API key · Models: Claude (Anthropic), OpenAI Codex, Gemini CLI, Cursor, OpenCode · port 3001 · [Repo](https://github.com/coderluii/holyclaude) · [📖 Docs ↗](https://github.com/CoderLuii/HolyClaude/blob/master/docs/configuration.md) · [🌐 Site ↗](https://holyclaude.coderluii.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/holyclaude/)</sub>

<a name="minimax-code"></a>
### #&#8288;105 [minimax-code](https://github.com/minimax-ai/minimax-code) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Terminal coding agent that edits code and runs tests with MiniMax or custom models.**

MiniMax Code (mcode) is a Node.js CLI and TUI agent that reads a project, edits files, runs shell commands and tests, and resumes sessions. It also runs headless (`mcode exec`) for CI and over ACP for editors. Models come from a MiniMax account or from custom providers using the openai-completions, openai-responses or anthropic-messages formats.

- **+** Three entry points: interactive TUI, headless `mcode exec` for CI, and ACP for editors
- **+** BYOK works without a MiniMax login via OpenAI- or Anthropic-style endpoints, including local servers
- **+** Permission modes, sandboxing, plan mode, subagents, skills and MCP support built in
- **+** Installer needs no sudo and sets up a compatible Node.js runtime if missing
- **−** Desktop app source is not included; repo covers only the TUI, headless CLI and ACP
- **−** Pull requests accepted only from repository collaborators
- **−** Search, media tools and managed connectors need a MiniMax account and credits
- **−** README says source is a 0.6.3 preview while npm is 0.6.9, so builds may differ

<sub>no GPU · Needs Node.js 22.19+, 24.2+, 25 or 26, pnpm 9.12.0 (source builds), MiniMax account or third-party model API · Models: MiniMax, openai-completions, openai-responses, anthropic-messages · [Repo](https://github.com/minimax-ai/minimax-code) · [📖 Docs ↗](https://agent.minimax.io/docs/cli/quick-start) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/minimax-code/)</sub>

<a name="nezha"></a>
### #&#8288;106 [nezha](https://github.com/hanshuaikang/nezha) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · GPL-3.0 · Sep 2026</sub>

**Desktop IDE for running Claude Code and Codex sessions across multiple projects.**

Nezha is a Tauri and React desktop app that wraps the native Claude Code and Codex CLIs in an embedded terminal. It groups sessions by project, notifies you when an agent needs input, and replays finished sessions. It also includes Git with Worktree support, AI-generated commit messages, a lightweight code and Markdown editor, and Skill management through symlinks.

- **+** Switches between Claude Code and Codex sessions across several projects in one window
- **+** Notifications and dock badge when an agent needs human input
- **+** Finished sessions are visualized and can be resumed
- **+** Built-in Git, Worktree support and review view; installer stated as 7 MB
- **−** Requires Claude Code or Codex installed separately
- **−** macOS installer is unsigned; needs an xattr command to open
- **−** README is mainly Chinese; English docs are in a separate file
- **−** GPL-3.0 license limits use in proprietary derivatives

<sub>no GPU · Needs Claude Code, Codex, Git · Models: Claude Code, Codex · [Repo](https://github.com/hanshuaikang/nezha) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nezha/)</sub>

<a name="zero"></a>
### #&#8288;107 [zero](https://github.com/twigpine/zero) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Oct 2026</sub>

**Terminal coding agent in Go with a TUI, headless exec mode and 25+ providers.**

Zero is a coding agent for the local terminal that inspects a repo, edits files and runs commands under a permission and sandbox policy. It offers an interactive TUI and a scriptable `zero exec` mode with text, JSON and stream-JSON I/O. Sessions are stored on disk, and it extends through MCP servers, skills, plugins, hooks and subagents.

- **+** Works with 25+ providers plus any OpenAI- or Anthropic-compatible endpoint, including Ollama and LM Studio
- **+** `zero exec` supports stream-JSON, isolated worktrees, spec-first runs and exit codes for CI
- **+** Writes, shell and network access are permission-gated; Linux sandbox uses Bubblewrap
- **+** Sessions stay on local disk, searchable, resumable and forkable; no telemetry upload
- **−** Linux native sandboxing requires Bubblewrap
- **−** Windows on ARM runs the x64 build under emulation
- **−** Source builds need Go 1.26.10+ and optional helper binaries for browser/terminal tools
- **−** README shows no hosted demo; docs are only in-repo markdown files

<sub>no GPU · Needs Bubblewrap (Linux sandbox), LLM provider API key or local Ollama/LM Studio · Models: OpenAI, Anthropic, Gemini, Groq, OpenRouter · [Repo](https://github.com/twigpine/zero) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zero/)</sub>

<a name="opencove"></a>
### #&#8288;108 [opencove](https://github.com/deadwavewave/opencove) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Desktop infinite canvas for running Claude Code, Codex, terminals, tasks and notes.**

OpenCove is an Electron app that places CLI agent sessions (Claude Code, Codex), PTY terminals, tasks and notes as nodes on one 2D canvas. Layout, viewport, terminal output and agent state persist across restarts, and projects can be isolated by directory or git worktree. It also ships an `opencove` CLI, a headless worker, and an experimental browser Web UI. The project is labeled alpha.

- **+** Runs several Claude Code or Codex sessions side by side on one canvas
- **+** Restores viewport, layout, terminal output and agent state after restart
- **+** Per-project isolation via directories and git worktrees
- **+** Desktop builds for macOS, Windows and Linux plus a standalone CLI/server installer with SHA256 check
- **−** Labeled alpha; nightly builds may have rough edges
- **−** macOS builds are not signed or notarized; Gatekeeper workaround needed
- **−** Web UI is experimental and LAN use needs a password and a built renderer
- **−** Needs Claude Code or Codex installed separately for full agent workflows

<sub>no GPU · Needs Node.js >= 22.12.0 (source build), pnpm 9.6.0 (source build), Claude Code or Codex CLI (recommended) · Models: Claude Code, Codex · [Repo](https://github.com/deadwavewave/opencove) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencove/)</sub>

<a name="aider-desk"></a>
### #&#8288;109 [aider-desk](https://github.com/hotovo/aider-desk) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Oct 2026</sub>

**Desktop app for steering AI coding agents with diff review and Git worktrees.**

AiderDesk is a TypeScript desktop app that began as a GUI for the Aider CLI and now includes its own agent mode. It organizes work into projects and tasks, gives each task an isolated Git worktree, and requires diff review and tool approval before changes or shell commands run. It connects to 30+ LLM providers, works as an MCP client and server, and supports TypeScript extensions.

- **+** Per-task Git worktrees keep AI experiments off the active local branch
- **+** Tool approval gates and diff review (side-by-side and unified) before changes apply
- **+** Extensions with 30+ lifecycle hooks, custom tools and React UI components
- **+** Chat history, task metadata and settings stored locally
- **−** README only points to Docker, npm, Homebrew and Scoop installs; steps are in external docs
- **−** RAM and GPU requirements are not stated
- **−** Broad feature set means more setup than a plain CLI agent
- **−** Voice control model requirements are not specified

<sub>Docker · Needs Aider CLI, LanceDB · Models: OpenAI, Anthropic, Gemini, DeepSeek, Ollama · [Repo](https://github.com/hotovo/aider-desk) · [📖 Docs ↗](https://aiderdesk.hotovo.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aider-desk/)</sub>

<a name="ghostex"></a>
### #&#8288;110 [ghostex](https://github.com/maddada/ghostex) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Native workspace for running many coding agents, with desktop and phone apps.**

Ghostex is a Rust/GPUI desktop app that wraps coding agents such as Claude Code, Codex, OpenCode and Gemini CLI in a chat view, terminal, embedded Chromium panes and an optional VS Code editor. Sessions persist across restarts. iOS and Android apps pair through Easy Connect or Tailscale to read transcripts and send prompts, and agents can open and steer other agents through the ghostex command.

- **+** Works with many agent CLIs: Claude Code, Codex, OpenCode, Pi, Gemini, Grok, Cursor, Copilot CLI
- **+** Sessions survive restarts; fuzzy search of all past prompts, also via gx f
- **+** Runs on macOS, Windows and Linux, with Android and iOS apps; brew, deb, rpm and AUR packages
- **+** Prompt queueing, worktree per task, split panes, and Markdown/HTML annotations sent back to the agent
- **−** iOS access is by TestFlight, requested through the project's Discord
- **−** Chromium is installed on first use of the browser or code editor
- **−** Several features depend on third-party parts such as CEF, code-server and Trycua
- **−** RAM requirements are not documented

<sub>Needs Chromium (CEF), Agent CLIs such as Claude Code or Codex, Tailscale (optional) · Models: Claude Code, Codex, OpenCode, Pi, Gemini CLI · [Repo](https://github.com/maddada/ghostex) · [🌐 Site ↗](https://ghostex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ghostex/)</sub>

<a name="openharness"></a>
### #&#8288;111 [openharness](https://github.com/autonomous-ai/openharness) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Desktop app that runs many coding agents across machines in tmux panes.**

Native desktop app (Flutter) and CLI that run Claude Code, Codex, Cursor, OpenCode and other agent CLIs in tmux sessions on your own machines. A per-machine daemon dials out and links machines over end-to-end encrypted WebRTC, with TURN and relay fallbacks. A Store adds domain harnesses such as Blender, KiCad and Typst, each with a live viewer.

- **+** Runs agent CLIs unmodified in tmux, using vendor transcripts and hooks rather than wrappers
- **+** End-to-end encryption (ChaCha20-Poly1305, X25519); relay forwards ciphertext only
- **+** Machines link by password with no SSH keys, Tailscale or open ports
- **+** Whole stack is MIT in one repo: app, CLI, daemon, relay and device firmware
- **−** Desktop app targets macOS and Linux only; no Windows build is listed
- **−** Building from source needs Node 20+, tmux, Xcode and Flutter 3.47+
- **−** Remote links depend on the vendor's relay and Cloudflare TURN as fallbacks
- **−** Agent Messages between harnesses is experimental and off by default

<sub>GPU optional · Needs tmux, Node.js 20+, Flutter 3.47+ (build from source), Xcode (build from source) · Models: Claude Code, Codex, Cursor, OpenCode, Hermes · [Repo](https://github.com/autonomous-ai/openharness) · [🌐 Site ↗](https://harness.autonomous.ai/desktop?utm_source=github&utm_medium=readme) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openharness/)</sub>

<a name="jean"></a>
### #&#8288;112 [jean](https://github.com/coollabsio/jean) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Oct 2026</sub>

**Desktop and headless workspace running parallel AI coding agents in git worktrees.**

Jean is a Tauri v2 desktop app, with a headless Linux `jean-server`, that runs CLI agents such as Claude, Codex, Cursor and OpenCode in parallel, one git worktree per task. It bundles a terminal, diff review with line comments, and GitHub, Linear and Sentry integrations. The UI is also served over HTTP/WebSocket with token auth, and the desktop app can combine local and remote servers in one sidebar.

- **+** Each task gets its own git worktree, so parallel agent sessions do not collide
- **+** Uses your existing agent CLIs and subscriptions; supports about ten backends
- **+** Headless jean-server with systemd installer, Docker image and browser access including phones
- **+** Desktop app shows local and remote servers together, with actions run on the owning server
- **−** Windows is marked not fully tested; Linux only community tested
- **−** jean-server supports Linux amd64 and arm64 only, glibc and OpenSSL 3
- **−** Antigravity backend and Mr. Robot issue automation are beta
- **−** Remote use needs your own network hardening, such as Tailscale, TLS and tokens

<sub>no GPU · Docker · Needs Agent CLIs (Claude, Codex, Cursor, OpenCode, etc.), git, Node.js and Rust (build from source) · Models: Claude, Codex, Cursor, OpenCode, Pi · port 3456 · [Repo](https://github.com/coollabsio/jean) · [🌐 Site ↗](https://jean.build) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jean/)</sub>

<a name="ante"></a>
### #&#8288;113 [ante](https://github.com/antigmalabs/ante) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent in a single Rust binary with built-in local inference.**

Ante is a terminal coding agent written in Rust, shipped as one executable with no runtime dependencies. It runs against 15 hosted-provider presets or a custom catalog entry, and can run fully offline on GGUF models through a managed llama.cpp. It also offers headless, server (stdio, socket, WebSocket) and Slack/Discord gateway modes, plus settings profiles that swap the system prompt and tool set.

- **+** Single Rust binary, about 15MB compressed, no runtime dependencies
- **+** Offline mode runs GGUF models via managed llama.cpp, no API key needed
- **+** Named profiles replace system prompt, tools, skills and memory per run
- **+** Terminal-Bench 2.1 results published with pinned builds and raw run logs
- **−** Beta preview: breaking changes and incomplete functionality expected
- **−** macOS and Linux only; Windows requires WSL
- **−** Prebuilt binary is under Binary Preview Terms, not Apache-2.0
- **−** /term orchestration requires tmux and the other agent CLIs installed

<sub>GPU optional · Needs tmux (for /term only) · Models: Anthropic, OpenAI, Google Gemini, Grok, DeepSeek · [Repo](https://github.com/antigmalabs/ante) · [📖 Docs ↗](https://docs.antigma.ai) · [🌐 Site ↗](https://antigma.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ante/)</sub>

<a name="zerostack"></a>
### #&#8288;114 [zerostack](https://github.com/gi-dellav/zerostack) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · GPL-3.0 · Oct 2026</sub>

**Terminal coding agent in Rust with permission modes and swappable prompts.**

zerostack is a terminal coding agent written in Rust, inspired by pi and opencode. It talks to OpenRouter, OpenAI, Anthropic, Gemini, Ollama and custom providers, and offers five permission modes, saved sessions, subagents and runtime-switchable system prompts such as code, plan and review. Memory, hooks, ACP, advisor and multimodal input are compile-time features, not in the default build.

- **+** README reports ~16MB average RAM, versus ~300MB for opencode, per its own measurements
- **+** Five permission modes with per-tool glob rules and doom-loop detection
- **+** Optional bubblewrap or zerobox sandbox masks ~/.ssh, ~/.aws and similar credential directories
- **+** Hooks use a settings.json format largely compatible with Claude Code hooks
- **−** Memory, hooks, ACP, advisor and multimodal need non-default cargo features
- **−** Windows support is untested, per the README
- **−** Sandbox falls back to unsandboxed bash if backend is missing, unless sandbox-required is set
- **−** GPL-3.0 license may limit embedding in proprietary products

<sub>no GPU · Needs bubblewrap (optional, for --sandbox), zerobox (optional, macOS sandbox), LLM provider API key · Models: OpenRouter, OpenAI, Anthropic, Gemini, Ollama · [Repo](https://github.com/gi-dellav/zerostack) · [📖 Docs ↗](https://github.com/gi-dellav/zerostack/blob/main/docs/GET_STARTED.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zerostack/)</sub>

<a name="continue"></a>
### #&#8288;115 [continue](https://github.com/continuedev/continue) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: widely used (90) · Freshness: active (98) · Maintenance: weak (22) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Jul 2026</sub>

**Coding agent as a CLI, VS Code extension and JetBrains plugin.**

Continue is a coding agent distributed as an npm CLI, a VS Code extension (Marketplace and OpenVSX) and a JetBrains plugin. The repository is read-only and no longer actively maintained; the final 2.0.0 release removed anonymous telemetry and authentication. The README does not list supported models or providers and points to docs.continue.dev for configuration.

- **+** Ships as CLI, VS Code extension and JetBrains plugin from one codebase
- **+** Final 2.0.0 release removed anonymous telemetry and authentication
- **+** Apache-2.0 license; extension available on OpenVSX as well as Marketplace
- **+** Source for each extension lives in its own directory (vscode, cli, intellij)
- **−** Repository is read-only and no longer actively maintained
- **−** README recommends the CLI over the JetBrains plugin
- **−** README does not list supported models or providers; docs needed
- **−** No Docker or compose setup

<sub>[Repo](https://github.com/continuedev/continue) · [📖 Docs ↗](https://docs.continue.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/continue/)</sub>

<a name="gastown"></a>
### #&#8288;116 [gastown](https://github.com/gastownhall/gastown) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: weak (22) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Oct 2026</sub>

**Orchestrates many coding agents across git repos with persistent work state.**

Gas Town is a Go CLI (gt) that manages a workspace of git repositories ("rigs") and runs multiple coding agents such as Claude Code, Codex, Copilot, Gemini and Cursor against them. Work is tracked as Beads issues grouped into convoys, with state kept in git worktree hooks so it survives agent restarts. A Mayor agent coordinates, while Witness and Deacon watchdogs and a Refinery merge queue handle health and merging.

- **+** 11 built-in agent presets, including claude, codex, copilot, gemini, cursor and opencode
- **+** Work state persists in git worktree hooks and the Beads ledger across restarts
- **+** Watchdogs detect stuck agents; a Bors-style bisecting queue merges finished work
- **+** Minimal mode tracks state without tmux while you run agents manually
- **−** Many project-specific terms (Mayor, polecats, rigs, convoys, wasteland) make the learning curve steep
- **−** Native install needs Git, Go, bd, Dolt, sqlite3 and tmux 3.0+
- **−** Full tmux workflows on Windows need WSL; native Windows is CLI-only
- **−** Copilot preset runs with --yolo, so autonomous agents need cost and safety care

<sub>no GPU · Docker + Compose · Needs Git 2.20+, Go 1.26.2+, Beads (bd) 0.57.0+, Dolt, tmux 3.0+, sqlite3, Claude Code CLI or another agent runtime · Models: Claude Code, GitHub Copilot, Codex, Gemini, Cursor · port 8080 · [Repo](https://github.com/gastownhall/gastown) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gastown/)</sub>

<a name="claude-squad"></a>
### #&#8288;117 [claude-squad](https://github.com/smtg-ai/claude-squad) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.7k · AGPL-3.0 · Aug 2026</sub>

**Terminal app that runs multiple coding agents in isolated git worktrees.**

Claude Squad is a Go terminal UI that launches several agent sessions at once: Claude Code by default, plus Codex, Gemini, Aider or any shell command. Each session runs in its own tmux session on a separate git worktree and branch, so parallel tasks do not conflict. You can preview output, review the diff, commit and push a branch, or pause and resume a session from one window.

- **+** Per-task git worktree and branch isolation avoids conflicts between parallel agents
- **+** Works with Claude Code, Codex, Gemini, Aider or any command via -p or named profiles
- **+** Built-in diff tab, plus commit/push and checkout/pause/resume keys
- **+** Installs as a single binary via Homebrew or install script
- **−** Requires tmux and the gh CLI to be installed
- **−** Auto-accept (-y) is marked experimental and documented only for Claude Code and Aider
- **−** Terminal UI only, no web interface
- **−** AGPL-3.0 license may restrict some commercial uses

<sub>no GPU · Needs tmux, gh, git · Models: Claude Code, Codex, Gemini CLI, Aider · [Repo](https://github.com/smtg-ai/claude-squad) · [🌐 Site ↗](https://smtg-ai.github.io/claude-squad/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-squad/)</sub>

<a name="zeron"></a>
### #&#8288;118 [zeron](https://github.com/zeronsh/zeron) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Desktop and CLI app for running and monitoring multiple coding agents locally.**

Zeron is a desktop app and Linux headless CLI that controls coding agents such as Claude Code, Codex, Cursor, Devin, Grok, Hermes, Pi and Antigravity. Sessions stay on the local device by default and no account is needed. Signing in optionally lets you start an agent on one device and follow or drive it from another.

- **+** Supports eight named agents (Claude Code, Codex, Cursor, Devin, Grok, Hermes, Pi, Antigravity) from one app
- **+** Local-only by default; no account or network needed, sessions stay on device
- **+** Headless Linux mode runs the engine as a boot-persistent background service
- **+** Desktop builds for macOS arm64, Windows x86_64 and Linux, with self-update
- **−** Headless CLI is Linux only
- **−** Synced devices can read and write each other's workspace files, so trust is required
- **−** macOS build is arm64 only per the README; Intel is not listed
- **−** Sync backend and hosting details are not described in the README

<sub>no GPU · Models: Claude Code, Codex, Cursor, Devin, Grok · [Repo](https://github.com/zeronsh/zeron) · [📖 Docs ↗](https://deepwiki.com/zeronsh/zeron) · [🌐 Site ↗](https://zeron.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zeron/)</sub>

<a name="ralph-orchestrator"></a>
### #&#8288;119 [ralph-orchestrator](https://github.com/mikeyobrien/ralph-orchestrator) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (40) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Rust CLI that loops coding agent CLIs until a task passes its checks.**

Ralph Orchestrator implements the Ralph Wiggum technique: it re-runs a coding agent CLI (Claude Code, Codex, Gemini CLI and others) until the agent emits LOOP_COMPLETE or an iteration limit is hit. Work is split across "hats", personas that coordinate through events, and gates such as tests, lint and typecheck reject incomplete output. It also has a Telegram human-in-the-loop bot, an MCP server over stdio, and an alpha web dashboard.

- **+** Supports 11 agent backends, including Claude Code, Codex, Gemini CLI, Kiro, Amp and Copilot CLI
- **+** Backpressure gates reject incomplete work using tests, lint and typecheck
- **+** Telegram integration lets agents block on questions and accept mid-loop guidance
- **+** Installs via npm, Cargo or a GitHub Releases script
- **−** Needs a separate agent CLI installed; it does not call models itself
- **−** Web dashboard is alpha with documented rough edges and breaking changes
- **−** Only 5 builtin hat presets: code-assist, debug, research, review, pdd-to-code-assist
- **−** MCP server is scoped to one workspace root, so multi-repo use needs one instance each

<sub>no GPU · Docker + Compose · Needs Rust 1.75+ (ralph-api), Node.js >= 18 and npm (web dashboard), An agent CLI such as Claude Code, Codex or Gemini CLI, Telegram bot token (optional) · Models: Claude Code, Kiro, Gemini CLI, Codex, Forge · port 3000 · [Repo](https://github.com/mikeyobrien/ralph-orchestrator) · [📖 Docs ↗](https://mikeyobrien.github.io/ralph-orchestrator/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph-orchestrator/)</sub>

<a name="ralph-tui"></a>
### #&#8288;120 [ralph-tui](https://github.com/subsy/ralph-tui) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Oct 2026</sub>

**Terminal UI that loops AI coding agents through a task list.**

Ralph TUI runs an autonomous loop around a coding agent CLI. It picks the highest-priority task from a prd.json file or a Beads epic, builds a prompt, runs the agent, detects completion and moves on. It supports Claude Code, OpenCode, Factory Droid, Cursor CLI, Gemini CLI, Codex and Kiro CLI, with session persistence and a remote listener for controlling instances on other machines.

- **+** Works with seven agent CLIs, including Claude Code, Codex, Gemini CLI and Kiro CLI
- **+** Sessions can be paused, resumed and recovered after a crash
- **+** Remote listener with token auth and audit log controls instances on other machines
- **+** Optional sandbox mode (bwrap on Linux, sandbox-exec on macOS) and headless runs
- **−** Only two task trackers: prd.json and Beads
- **−** Needs Bun and a separately installed agent CLI
- **−** Remote listener binds to 0.0.0.0 once a token is configured
- **−** Linux sandbox mode requires bwrap to be installed

<sub>no GPU · Needs Bun, A supported agent CLI (Claude Code, OpenCode, Codex, etc.), Beads (optional tracker), bwrap (optional, Linux sandbox) · Models: Claude Code, OpenCode, Factory Droid, Cursor CLI, Gemini CLI · [Repo](https://github.com/subsy/ralph-tui) · [📖 Docs ↗](https://ralph-tui.com/docs/getting-started/quick-start) · [🌐 Site ↗](https://ralph-tui.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph-tui/)</sub>

<a name="corecoder"></a>
### #&#8288;121 [corecoder](https://github.com/he-yufeng/corecoder) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Minimal Python coding agent written to be read and forked.**

CoreCoder is a working terminal coding agent in about 2,816 lines of Python (1,322 in the engine). It runs a tool loop with eight tools, three-tier context compaction, sub-agents, MCP stdio tools, plan mode, hooks and /undo. It is meant as a readable reference to study and fork, backed by eight source-reading essays, not as a daily driver.

- **+** Whole engine is small enough to read in one sitting, with a file-by-file code map
- **+** Works with any OpenAI-compatible endpoint; optional LiteLLM backend for other providers
- **+** Mutating tools ask for consent; -p mode refuses them unless --yes is passed
- **+** Eight bilingual essays walk through the actual code; 227 tests
- **−** Bash safety is a regex blacklist, not a sandbox; unsafe for untrusted input
- **−** No fallback model chain or hard dollar budget; retry is plain exponential backoff
- **−** Sub-agents run synchronously; no RAG; MCP client supports tools only
- **−** Author states it is not intended as a daily driver

<sub>no GPU · Needs Python 3.10+, LLM API key (OpenAI-compatible) · Models: OpenAI, DeepSeek, Ollama, OmniRoute, Kimi · [Repo](https://github.com/he-yufeng/corecoder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/corecoder/)</sub>

<a name="opencode-telegram-bot"></a>
### #&#8288;122 [opencode-telegram-bot](https://github.com/grinev/opencode-telegram-bot) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Telegram client for controlling a local OpenCode coding agent from your phone.**

A Node.js bot that connects to a local OpenCode server (V1 or V2) and the Telegram Bot API, so you can send prompts, switch models and agents, manage sessions, and answer permission requests from chat. It restricts access to one Telegram user ID and opens no inbound ports. It also supports voice prompts through a Whisper-compatible API, scheduled tasks, and file browsing.

- **+** Access limited to one whitelisted Telegram user ID; no open ports or exposed API
- **+** Covers sessions, model and agent switching, worktrees, revert/fork, and permission prompts in chat
- **+** Supports both OpenCode V1 and V2 servers via OPENCODE_SERVER_VERSION
- **+** Installs with npx or npm; 12 UI languages; macOS, Windows and Linux
- **−** Needs OpenCode running on the same machine; it does not work with other coding agents
- **−** Does not detect the OpenCode version; a wrong setting only shows as a log error
- **−** Sessions are not shared between OpenCode V1 and V2
- **−** README tracks main, so some described features may be missing from the npm release

<sub>no GPU · Docker + Compose · Needs Node.js 22.14+, OpenCode server, Telegram Bot token, Whisper-compatible API (optional, for voice) · Models: Any model configured in OpenCode · [Repo](https://github.com/grinev/opencode-telegram-bot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencode-telegram-bot/)</sub>

<a name="inferstep-atlas"></a>
### #&#8288;123 [atlas](https://github.com/inferstep/atlas) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Oct 2026</sub>

**Local coding agent that plans, tests and repairs code using small GGUF models.**

ATLAS is a terminal coding agent that runs a GGUF model through llama-server on your own GPU. A Go proxy drives a multi-phase pipeline of planning, diverse candidate generation, scoring, sandboxed testing and repair, with a Bubbletea TUI as the client. The README marks it experimental and lists known gaps in 3.1.x verification, with fixes planned for 3.2.0.

- **+** Runs fully local on a GGUF model; no hosted API or per-token fees
- **+** Sandbox compiles and tests candidates in Python, Rust, Go, C and Shell
- **+** Supports NVIDIA CUDA, AMD ROCm, Apple Metal and Vulkan (preview)
- **+** One-command bootstrap script, with a pinned-release install option
- **−** A failing V3 candidate can be written and reported as verified (3.1.0 to 3.1.6)
- **−** No current benchmark result; the V3.0 LiveCodeBench figure was withdrawn
- **−** Geometric Lens gives no usable signal with default settings in 3.1.3 to 3.1.6
- **−** Needs 16 GB+ VRAM; prebuilt CUDA image targets Blackwell, older GPUs need a rebuild

<sub>GPU required · Compose · Needs Docker or Podman, nvidia-container-toolkit (NVIDIA), llama-server, Python 3.9+ · Models: GGUF (Q6_K, Q4_K_M), Qwen3-14B · [Repo](https://github.com/inferstep/atlas) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/inferstep-atlas/)</sub>

<a name="agent-shell"></a>
### #&#8288;124 [agent-shell](https://github.com/xenodium/agent-shell) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · GPL-3.0 · Oct 2026</sub>

**Emacs client that runs ACP-compatible coding agents in native Emacs buffers.**

agent-shell is an Emacs package built on comint via shell-maker. It talks to coding agents over the Agent Client Protocol (using acp.el), so you use normal buffers and key bindings instead of terminal emulation. The README lists 23 agents, including Claude Agent, Codex, Gemini CLI, Goose, Cursor, Copilot and OpenCode, plus any other ACP agent.

- **+** Supports 23 named agents and any other ACP-speaking agent from one interface
- **+** Uses regular Emacs buffers and bindings, with no terminal emulation
- **+** Installable from MELPA; acp.el and shell-maker dependencies install automatically
- **+** Active ecosystem of add-on packages for queues, notifications, Org transcripts and sandboxing
- **−** Emacs only; each agent's CLI or ACP adapter must be installed separately
- **−** No tagged releases; versions are tracked only through MELPA and blog posts
- **−** Several agents need a paid subscription or API key, and some need recent CLI versions
- **−** GPL-3.0 license may constrain reuse in non-GPL code

<sub>no GPU · Needs Emacs, acp.el, shell-maker, Node.js/npm (for several agent adapters), an ACP-capable agent CLI · Models: Claude Agent, Codex, Gemini CLI, Goose, Grok Build · [Repo](https://github.com/xenodium/agent-shell) · [🌐 Site ↗](https://xenodium.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-shell/)</sub>

<a name="agtx"></a>
### #&#8288;125 [agtx](https://github.com/fynnfluegge/agtx) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

**Terminal kanban board that runs parallel coding agents in git worktrees.**

agtx is a Rust TUI that manages coding agent CLIs (Claude Code, Codex, Grok, Cursor, OpenCode, Gemini CLI, Copilot and others) as tasks on a kanban board. Each task runs in its own git worktree and tmux window, and different agents can handle different workflow phases with context handover. It also offers an optional mobile web view, an MCP server, spec-driven workflow plugins and an experimental orchestrator agent.

- **+** Supports nine agent CLIs, with a different agent configurable per workflow phase
- **+** Each task gets an isolated git worktree and tmux window with persistent session history
- **+** Checks Review tasks for merge conflicts via git merge-tree and sends the agent a fix skill
- **+** Mobile web app with live agent terminal; server runs only while agtx is serving
- **−** Requires tmux; the gh CLI is needed for PR operations
- **−** Orchestrator agent is marked experimental and needs a flag to enable
- **−** Mobile board needs a binary built with the serve feature
- **−** Served board can type into agents, so access relies on device pairing

<sub>no GPU · Docker · Needs tmux, git, gh (optional), Tailscale (optional, for remote mobile access) · Models: Claude Code, Codex, Grok, Cursor, OpenCode · [Repo](https://github.com/fynnfluegge/agtx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agtx/)</sub>

<a name="waku"></a>
### #&#8288;126 [waku](https://github.com/egoist/waku) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · GPL-3.0 · Oct 2026</sub>

**Native desktop app for running local coding agent CLIs side by side.**

Waku is a Rust desktop app built on GPUI that wraps installed coding agent CLIs such as Claude Code, Codex CLI, Cursor CLI, OpenCode and Amp. It manages projects and independent sessions, with model switching, queued or steered follow-ups, and Git-backed checkpoints. A standalone waku-daemon owns the SQLite task data and workspaces, and a browser client talks to it over WebSocket.

- **+** Supports nine agent CLIs, including Claude Code, Codex CLI, Cursor CLI, OpenCode and Pi
- **+** Stores projects, sessions and transcripts locally; no Waku account or remote service needed
- **+** Daemon uses an authenticated, versioned WebSocket protocol and is loopback-only by default
- **+** Runs on macOS, Linux (Wayland and X11) and Windows with self-updating installers
- **−** Needs at least one agent CLI installed and authenticated separately
- **−** Embedded browser and computer-use integration are macOS-only
- **−** Local folder picker and PTY unavailable when connected to an external daemon
- **−** GPL-3.0-only license may limit embedding in proprietary products

<sub>Needs At least one supported agent CLI (Amp, Claude Code, Codex CLI, Cursor CLI, Fx, Grok Build, Kimi Code, OpenCode, Pi), Rust 1.96+ and Bun (development only) · Models: Amp, Claude Code, Codex CLI, Cursor CLI, Fx · [Repo](https://github.com/egoist/waku) · [🌐 Site ↗](https://waku.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/waku/)</sub>

<a name="vibeyard"></a>
### #&#8288;127 [vibeyard](https://github.com/elirantutia/vibeyard) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Sep 2026</sub>

**Desktop app for running multiple Claude Code, Codex and Gemini CLI sessions.**

Vibeyard is a desktop app that wraps Claude Code, OpenAI Codex CLI and Gemini CLI in a workspace with one PTY per session, a swarm grid view, split panes and session resume. It adds a per-project kanban board, cost and context tracking, a session inspector, and an embedded browser tab that sends selected DOM elements to the agent as context.

- **+** Supports three CLIs: Claude Code, Codex CLI and Gemini CLI
- **+** Per-session cost, token and context window tracking with a session inspector
- **+** Kanban cards can spawn or resume CLI sessions and auto-move to Done
- **+** Installers for macOS, Linux and Windows, plus npm global install
- **−** Requires at least one supported CLI installed and authenticated separately
- **−** Only three providers supported; others are listed as coming soon
- **−** Building from source needs Node v24+
- **−** No docs site; the README is the only documentation

<sub>no GPU · Needs Claude Code, Codex CLI or Gemini CLI, Node v24+ (build from source) · Models: Claude Code, OpenAI Codex CLI, Gemini CLI · [Repo](https://github.com/elirantutia/vibeyard) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibeyard/)</sub>

<a name="mini-swe-agent"></a>
### #&#8288;128 [mini-swe-agent](https://github.com/swe-agent/mini-swe-agent) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.8k · MIT · Sep 2026</sub>

**Bash-only coding agent in about 100 lines of Python.**

mini-swe-agent is a minimal software engineering agent from the SWE-bench and SWE-agent team. It gives the model only bash, runs each action with subprocess.run, and keeps a linear message history. It ships a `mini` CLI, batch inference for SWE-bench, a trajectory browser and Python bindings, and reports over 74% on SWE-bench Verified.

- **+** Agent class is about 100 lines of Python, easy to read and modify
- **+** Runs locally or in docker/podman, singularity/apptainer, bubblewrap or contree
- **+** Works with any model via litellm, openrouter or portkey; no tool-calling required
- **+** Linear history means the trajectory equals the messages sent to the model
- **−** Bash is the only tool; no built-in editor, search or other specialised tools
- **−** Each action is stateless, with no persistent shell session between commands
- **−** v2 differs from v1, so existing users need the migration guide
- **−** No IDE integration; interfaces are a CLI and a Python API

<sub>no GPU · Needs Python, LLM provider API (litellm, openrouter or portkey) · Models: litellm, openrouter, portkey, /completion and /response endpoints · [Repo](https://github.com/swe-agent/mini-swe-agent) · [📖 Docs ↗](https://mini-swe-agent.com/latest/quickstart/) · [🌐 Site ↗](https://mini-swe-agent.com/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mini-swe-agent/)</sub>

<a name="longhorizon-harness"></a>
### #&#8288;129 [longhorizon-harness](https://github.com/amap-ml/longhorizon-harness) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Manager/Executor/Auditor loop that keeps Claude Code or Codex on long tasks.**

LongHorizon-Harness wraps existing agent CLIs (Claude Code, Codex, OpenCode, DeepSeek Harness) in a plan, act, verify, checkpoint loop. A Manager picks the next bounded step, an Executor runs it with fresh context, and an Auditor checks real files, UI and logs before progress is accepted. It ships a CLI and a browser workbench, and reports gains on WeaveBench, OSWorld 2.0 and Terminal-Bench 2.1.

- **+** Separate Auditor inspects actual files, logs and tests before a step counts as progress
- **+** Manager, Executor and Auditor can each use a different backend or model
- **+** Resumable runs stored under .lh-harness/runs, with follow-ups continuing the same run
- **+** README reports Terminal-Bench 2.1 69.7 to 77.2 with Qwen 3.7-Plus on Claude Code
- **−** macOS is the only tested platform; native Windows is blocked in v0.1.8, WSL2 needed
- **−** Requires a separate agent CLI (codex, claude, opencode or dsh) installed and authenticated
- **−** GUI use needs a computer-use plugin and OS permissions granted by hand on macOS
- **−** DeepSeek backend is CLI-only, returns only final answer, and exposes task text in process args

<sub>no GPU · Needs Python 3.10+, uv or pip, Node.js 20+, codex, claude, opencode or dsh CLI, computer-use plugin (optional) · Models: Claude, GPT, Qwen, DeepSeek · port 8799 · [Repo](https://github.com/amap-ml/longhorizon-harness) · [🌐 Site ↗](https://lh-harness.pages.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/longhorizon-harness/)</sub>

<a name="container-use"></a>
### #&#8288;130 [container-use](https://github.com/dagger/container-use) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (50) · Freshness: recent (79) · Maintenance: fair (54) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Aug 2026</sub>

**MCP server that gives each coding agent its own container and git branch.**

Container Use is an MCP server and CLI, written in Go on top of Dagger, that runs each coding agent in a fresh container tied to its own git branch. You add `container-use stdio` (alias `cu`) as an MCP server in Claude Code, Cursor, Goose, VSCode or another MCP-compatible agent. You can review command history and logs, open an agent's terminal, or `git checkout` its branch.

- **+** Per-agent container and git branch lets several agents run in parallel without conflicts
- **+** Full command history and logs, plus a terminal you can drop into to take over
- **+** Works with any MCP-compatible agent through one `container-use stdio` entry
- **+** Review uses plain git: check out the agent's branch
- **−** README labels it experimental and in early development
- **−** Built on Dagger; the README does not say what container runtime it needs
- **−** Last tagged release is 2025-08-19, well behind recent commits
- **−** Agent rules file is optional but must be appended to CLAUDE.md manually

<sub>no GPU · Needs Dagger, git, MCP-compatible agent · Models: any model via MCP-compatible agents · [Repo](https://github.com/dagger/container-use) · [📖 Docs ↗](https://container-use.com/quickstart) · [🌐 Site ↗](https://container-use.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/container-use/)</sub>

<a name="dmux"></a>
### #&#8288;131 [dmux](https://github.com/standardagents/dmux) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Aug 2026</sub>

**tmux manager that runs coding agents in separate git worktrees.**

dmux opens a tmux pane per task, each with its own git worktree and branch, and launches one or more agent CLIs (Claude Code, Codex, OpenCode, Gemini CLI and others) on a prompt. Finished panes can be merged into the main branch or pushed as a GitHub PR from a pane menu. It also offers a file browser, lifecycle hooks and multi-project sessions.

- **+** Each pane gets its own worktree and branch, so parallel agents do not conflict
- **+** Supports 11 agent CLIs including Claude Code, Codex, OpenCode, Gemini and Cursor
- **+** Merge or create GitHub PR from the pane menu; lifecycle hooks run on create and merge
- **+** Resumes terminals and tracked agent conversations when a pane is recreated
- **−** Requires tmux 3.0+, Node.js 18+ and Git 2.20+ installed
- **−** Needs at least one separate agent CLI installed and configured
- **−** macOS notifications only; no equivalent noted for other platforms
- **−** AI naming and summaries need an inference provider key or subscription login

<sub>no GPU · Needs tmux 3.0+, Node.js 18+, Git 2.20+, at least one agent CLI · Models: Claude Code, Codex, OpenCode, Cline CLI, Gemini CLI · [Repo](https://github.com/standardagents/dmux) · [📖 Docs ↗](https://dmux.ai) · [🌐 Site ↗](https://dmux.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dmux/)</sub>

<a name="gsd-pi"></a>
### #&#8288;132 [gsd-pi](https://github.com/open-gsd/gsd-pi) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Terminal coding agent that plans and verifies work in Git worktrees.**

GSD Pi is a local-first coding agent started with the `gsd` command. It breaks work into milestones, slices and tasks, and an auto mode plans, implements and verifies them in isolated Git worktrees. Project state is kept in `.gsd/` and a local database with markdown projections. A TUI is the default, and `gsd --web` opens a web interface.

- **+** Auto mode plans, implements, verifies and advances through milestones, slices and tasks
- **+** Git worktrees isolate implementation work from the main checkout
- **+** Works with API keys, OAuth providers and external CLIs such as Claude Code and Cursor Agent
- **+** `gsd quick --output-format json` gives structured output and meaningful exit codes for automation
- **−** Public history restarted at 1.0.0; older release notes are archived
- **−** README gives no RAM, hardware or supported Node.js version
- **−** Older unscoped `gsd-pi` installs need manual removal before migrating
- **−** Web UI port and deployment details are not in the README

<sub>no GPU · Docker + Compose · Needs Node.js, npm or pnpm, Git, Model provider API key, OAuth or CLI (e.g. Claude Code, cursor-agent) · Models: Claude Haiku 5.5 (default light tier), Cursor Agent (composer-2.5), Claude Code CLI, API-key and OAuth providers · [Repo](https://github.com/open-gsd/gsd-pi) · [📖 Docs ↗](https://github.com/open-gsd/gsd-pi/blob/main/docs/user-docs/getting-started.md) · [🌐 Site ↗](https://pi.opengsd.net/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gsd-pi/)</sub>

<a name="agentsmesh"></a>
### #&#8288;133 [agentsmesh](https://github.com/agentsmesh/agentsmesh) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (31) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · custom license · Sep 2026</sub>

**Control plane that schedules terminal coding agents across self-hosted runners.**

AgentsMesh runs terminal-based coding agents (Claude Code, Codex CLI, Gemini CLI, Aider, OpenCode, or custom) in isolated pods, each with its own Git worktree, on self-hosted runner daemons. A Go backend orchestrates runners over gRPC with mTLS, while terminal output streams through a separate relay to Web, Electron and iOS clients. It adds Autopilot control agents, pod channels and a Kanban ticket board.

- **+** Each agent pod gets its own Git worktree, branch and credentials, so concurrent agents do not collide
- **+** Runners are self-hosted daemons, so code stays on your machines; capacity set via max_concurrent_pods
- **+** Control plane (gRPC+mTLS) is split from terminal streaming through a stateless WebSocket relay
- **+** Works with any terminal agent; Web, Electron and iOS clients share one Rust core
- **−** BSL-1.1 license: production use requires a commercial license until 2030-02-28
- **−** Self-hosting needs PostgreSQL, Redis, MinIO, Traefik, backend and relay; heavy for small teams
- **−** README recommends the hosted service at agentsmesh.ai; self-host guide lives in a separate folder
- **−** Agents need your own API keys (BYOK); no models bundled

<sub>no GPU · Docker + Compose · Needs PostgreSQL, Redis, MinIO, Traefik, Docker · Models: Claude Code, Codex CLI, Gemini CLI, Aider, OpenCode · port 3000 · [Repo](https://github.com/agentsmesh/agentsmesh) · [📖 Docs ↗](https://agentsmesh.ai/docs) · [🌐 Site ↗](https://agentsmesh.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentsmesh/)</sub>

<a name="cli-agent-orchestrator"></a>
### #&#8288;134 [cli-agent-orchestrator](https://github.com/awslabs/cli-agent-orchestrator) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Oct 2026</sub>

**Supervisor agent that delegates work to multiple coding CLIs in tmux sessions.**

CAO runs a local cao-server and starts provider coding CLIs (Kiro CLI, Claude Code, Codex CLI, Cursor CLI and others) in isolated tmux sessions. A supervisor agent gets tools to delegate tasks to worker agents in parallel or in sequence. Agents stay full CLI processes with their own authentication, and a web UI at localhost:9889 shows the fleet.

- **+** Supports 12 provider CLIs, including Claude Code, Codex, Kiro, Copilot and Cursor
- **+** Workers keep native CLI auth and capabilities instead of being re-wrapped
- **+** Includes web UI, HTTP API, flows, memory, skills and tool restrictions
- **+** Kubernetes example for running supervisor and worker fleets on Amazon EKS
- **−** Requires tmux 3.3+ and at least one separately installed, authenticated provider CLI
- **−** Default provider is Kiro CLI; other providers need per-provider overrides
- **−** Agent plugins feature is gated off by default behind an environment variable
- **−** No Docker image or compose file; container use is via a devcontainer feature

<sub>no GPU · Needs Python 3.10+, tmux 3.3+, uv, a provider CLI (Kiro, Claude Code, Codex, etc.) · Models: Kiro CLI, Claude Code, Codex CLI, Antigravity CLI, Hermes · port 9889 · [Repo](https://github.com/awslabs/cli-agent-orchestrator) · [📖 Docs ↗](https://awslabs.github.io/cli-agent-orchestrator/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-agent-orchestrator/)</sub>

<a name="takt"></a>
### #&#8288;135 [takt](https://github.com/nrslib/takt) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**CLI that runs coding agents through YAML plan, implement, review and fix workflows.**

TAKT is a Node.js CLI that defines AI coding workflows in YAML: each step has a persona, permissions, and rules that decide the next step, such as a review-to-fix loop. Queued tasks run in isolated git worktrees with logs and reports under .takt/runs. It drives Claude, Codex, OpenCode, Pi, DeepSeek Harness, Cursor, Copilot CLI and Kiro as providers.

- **+** Review and fix loops are explicit YAML transitions, not prompt instructions
- **+** Queued tasks run in isolated worktrees, with logs and reports kept per run
- **+** Supports many providers: Claude, Codex, OpenCode, Pi, Cursor, Copilot CLI, Kiro
- **+** Ships MCP server (takt-mcp) and ACP agent (takt-acp) entrypoints
- **−** Requires Node.js 22.22.0 or later and a git repository with a commit
- **−** SDK providers need a separate `takt install <provider>` step
- **−** Web UI (`takt ui`) is labeled experimental
- **−** No tagged release; large workflow and config surface to learn

<sub>no GPU · Docker + Compose · Needs Node.js >=22.22.0, git, Provider CLI or SDK (Claude, Codex, OpenCode, Pi, Cursor, Copilot, Kiro), gh or glab (optional), tmux (claude-terminal only) · Models: Claude Agent SDK, Claude Code CLI, Codex SDK, OpenCode, Pi · port 20525 · [Repo](https://github.com/nrslib/takt) · [📖 Docs ↗](https://github.com/nrslib/takt/blob/main/docs/tutorial.md) · [🌐 Site ↗](https://nrslib.github.io/takt/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/takt/)</sub>

<a name="rune"></a>
### #&#8288;136 [rune](https://github.com/unstablebuild/rune) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · GPL-3.0 · Oct 2026</sub>

**Native GPU-rendered IDE and terminal multiplexer with a built-in agent.**

Rune is a native IDE and terminal multiplexer written in Go, rendering with OpenGL on Linux and Metal on macOS instead of Electron. It offers nine workspace slots, language intelligence for a documented list of languages, and a built-in agent or IDE skills for external agents. Rune instances connect over an end-to-end encrypted peer network built on headscale, and a headless node can serve workspaces to your other machines.

- **+** Native rendering pipeline (OpenGL on Linux, Metal on macOS), no Electron
- **+** Peer network lets you open remote workspaces via rune:// URLs
- **+** Headless node runs as a Docker container or a systemd, launchd, OpenRC or runit service
- **+** Packages install from official sources or directly from a Git repository
- **−** GPL-3.0 license may restrict embedding in proprietary products
- **−** Remote networking depends on the project's own headscale network
- **−** README lists only macOS and Linux install paths; Windows support unknown
- **−** Supported models and providers for the built-in agent are not stated

<sub>Docker · Needs headscale network (hosted by project) · [Repo](https://github.com/unstablebuild/rune) · [📖 Docs ↗](https://docs.rune.build/) · [🌐 Site ↗](https://rune.build) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rune/)</sub>

<a name="cccc"></a>
### #&#8288;137 [cccc](https://github.com/chesterra/cccc) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Oct 2026</sub>

**Daemon that coordinates multiple coding agent CLIs as a persistent group with a Web UI.**

CCCC is a Rust daemon that runs several coding agents (Claude Code, Codex CLI, Grok Build, OpenCode, Kilo and others) as one group. Messages go through an append-only ledger with separate stored, delivered, read and reply status. A Web UI, CLI, MCP tools and IM bridges all talk to the same daemon, and state lives in CCCC_HOME.

- **+** Append-only ledger.jsonl records messages for replay, with separate delivery, read and reply status
- **+** Supports about 20 agent runtimes plus a custom runtime for any command-line agent
- **+** Single native install: no database, message broker, Docker or Rust toolchain needed
- **+** Web UI, CLI, MCP and IM bridges share one daemon-owned state; SDKs for Python, npm and Rust
- **−** Prebuilt targets only Linux x86-64, Apple Silicon macOS and Windows x86-64; no Intel Mac after 0.4.37
- **−** Web-model runtimes like ChatGPT Web need a public HTTPS URL for the MCP connector
- **−** Voice features are experimental, and the global Secretary shares model history across Groups
- **−** Each agent CLI must be installed and signed in separately; default autonomy flags bypass approvals

<sub>no GPU · Docker + Compose · Needs Agent CLIs such as Claude Code or Codex CLI, installed and signed in separately · Models: Claude Code, Codex CLI, Grok Build, OpenCode, Kilo Code · port 8848 · [Repo](https://github.com/chesterra/cccc) · [📖 Docs ↗](https://chesterra.github.io/cccc/) · [🌐 Site ↗](https://chesterra.github.io/cccc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cccc/)</sub>

<a name="tmuxai"></a>
### #&#8288;138 [tmuxai](https://github.com/alvinunreal/tmuxai) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

**Terminal assistant that reads your tmux panes and runs commands in an exec pane.**

TmuxAI runs inside a tmux window with a chat pane, an exec pane and read-only context panes. It captures visible pane content, sends it with chat history to a configured model, and runs suggested commands in the exec pane after confirmation. It also has watch mode, knowledge bases, skills, context squashing and MCP tool support.

- **+** Reads context from all panes in the tmux window, no copy-paste needed
- **+** Commands need confirmation unless whitelisted; blacklist patterns and risk indicator included
- **+** Prepare mode tracks exit codes and command completion for bash, zsh and fish
- **+** Knowledge bases and SKILL.md skills load context on demand; /squash trims history
- **−** Requires tmux; targets Linux and macOS only
- **−** One TmuxAI instance per tmux window
- **−** Config lists openrouter, requesty, openai or azure; local models not documented
- **−** README says the command risk scoring is not exhaustive

<sub>no GPU · Needs tmux, LLM API key (openrouter, requesty, openai or azure) · Models: openrouter, requesty, openai, azure · [Repo](https://github.com/alvinunreal/tmuxai) · [🌐 Site ↗](https://tmuxai.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tmuxai/)</sub>

<a name="empryo"></a>
### #&#8288;139 [empryo](https://github.com/proxysoul/empryo) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Oct 2026</sub>

**Coding agent that maps your repo and edits code by symbol name.**

Empryo is a coding agent with desktop, terminal and headless modes that builds a map of a repository before editing. It replaces functions or classes by name, runs typecheck, lint and tests in the same turn, and keeps per-project memory of decisions and past bugs. This repository holds only the public SoulForge v2 core and engine; the Empryo v3 desktop app is developed privately.

- **+** Edits by function or class name instead of line ranges
- **+** Runs typecheck, lint and tests and fixes failures in the same turn
- **+** Per-project memory of decisions and past bugs
- **+** Same agent across desktop, terminal and headless CI
- **−** Repo is only the SoulForge v2 core; v3 app and newest features are private
- **−** Empryo v3 license forbids selling, hosting or bundling it without written permission
- **−** License detected as NOASSERTION; two separate licenses apply
- **−** README does not list supported models, providers or system requirements

<sub>[Repo](https://github.com/proxysoul/empryo) · [📖 Docs ↗](https://empryo.com/docs) · [🌐 Site ↗](https://empryo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/empryo/)</sub>

<a name="gentle-shell"></a>
### #&#8288;140 [gentle-shell](https://github.com/gentleman-programming/gentle-shell) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Coding-agent workspace for Pi with diff views, subagents and review.**

gentle-shell is a Pi-native package that turns a Pi coding-agent session into a workspace. It adds a live changes viewer across worktrees, subagent cards, per-role model profiles and a command palette. Its ODD workflow keeps small tasks inline and delegates to explorers, writers or verifiers only for named reasons.

- **+** Shows uncommitted changes across session and subagent worktrees in one diff viewer
- **+** Subagents run as separate processes with live model, token, cost and elapsed cards
- **+** Routing rules come with linked benchmark PRs and issues
- **+** Installers for macOS, Windows and Linux; one prefix bundles Pi, Gentle AI and Engram
- **−** Requires Pi; it is not a standalone agent
- **−** Benchmarks are single runs (n=1); the large task took about 3x longer than Codex CLI
- **−** Workflow concepts (ODD, RDD, 4R lenses) add a learning curve
- **−** Native review needs a filesystem honoring private POSIX modes; WSL DrvFS may fail

<sub>Needs Pi, Gentle AI v4.1.1, Engram, Git · Models: Provider models via Pi, Per-role model profiles · [Repo](https://github.com/gentleman-programming/gentle-shell) · [📖 Docs ↗](https://gentle-ai-wiki.gentlemanprogramming.com/) · [🌐 Site ↗](https://gentle-ai.gentlemanprogramming.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gentle-shell/)</sub>

<a name="thclaws"></a>
### #&#8288;141 [thclaws](https://github.com/thclaws/thclaws) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Oct 2026</sub>

**Native Rust coding agent with desktop GUI, CLI, and OpenAI-compatible server.**

thClaws is a single Rust binary that runs a coding and automation agent as a desktop app, a CLI REPL, a one-shot `-p` command, or a `--serve` web server. The server exposes OpenAI-compatible `/v1/chat/completions` and Anthropic-compatible `/v1/messages` endpoints. It supports 27 providers including Ollama, plus MCP servers, skills, hooks, scheduled jobs, and OS-level Bash confinement.

- **+** One binary covers desktop GUI, CLI REPL, non-interactive mode, and HTTP server
- **+** Catalogue lists 1,100+ models across 27 providers, plus Ollama for fully local use
- **+** Bash runs inside Seatbelt, Landlock, or bubblewrap confinement by default
- **+** Supports MCP, AGENTS.md, SKILL.md, hooks, plugins, cron scheduling, and multi-agent teams
- **−** Young project (started April 2026) with roughly weekly releases
- **−** v0.126.0 moves existing workspaces into .thclaws/bots/main/, breaking absolute paths
- **−** Discord, Slack, and WhatsApp bridges are not built yet
- **−** README badge says MIT OR Apache-2.0, while detected license is Apache-2.0

<sub>GPU optional · Docker + Compose · Needs LLM provider API key or local Ollama, Rust, Node.js 20+, pnpm 10+ (build from source only) · Models: Anthropic, OpenAI, Google Gemini, Ollama, LMStudio · port 7878 · [Repo](https://github.com/thclaws/thclaws) · [📖 Docs ↗](https://thclaws.ai/manual) · [🌐 Site ↗](https://thclaws.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/thclaws/)</sub>

<a name="loushang"></a>
### #&#8288;142 [loushang](https://github.com/zhnt/loushang) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent with persistent sessions and method-guided delivery.**

Loushang is a Python CLI and terminal workbench, `loushang code`, that runs coding turns against a model catalog with built-in tools, resumable sessions and project-level extensions. It also ships `loushang.ai`, an SDK with a model registry, streaming, tool calls and cost helpers. Work is structured through "methods" that define roles, phases and acceptance expectations.

- **+** Sessions can be resumed, forked, exported and diagnosed
- **+** Project-level Python extensions add hooks, tools, commands and resources
- **+** Reusable AI SDK with model registry, streaming and cost helpers
- **+** Apache-2.0 licensed with docs and examples for CLI and SDK
- **−** README calls it early development; recommended install is from source
- **−** No tagged release published
- **−** Supported providers and models are not listed in the README
- **−** Work, research and ppt surfaces are roadmap only

<sub>Needs uv, Python · [Repo](https://github.com/zhnt/loushang) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loushang/)</sub>

<a name="kode-cli"></a>
### #&#8288;143 [kode-cli](https://github.com/shareai-lab/kode-cli) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: weak (21) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent that edits files and runs commands across many model providers.**

Kode is a TypeScript CLI coding agent installed with npm. It reads your repo, edits files and runs shell commands, and routes work across configured models through main, task, compact and quick pointers. It reads AGENTS.md and legacy .claude directories, supports subagents, skills, plugin marketplaces and MCP servers, and can run as an ACP agent server.

- **+** Model profiles and pointers (main/task/compact/quick) with mid-session switching and YAML export
- **+** Reads AGENTS.md plus legacy .claude agents, skills and commands
- **+** No product telemetry by default; network use limited to features you invoke
- **+** Supports MCP servers, subagents, skill marketplaces and ACP mode for Zed/Toad
- **−** Runs in YOLO mode by default, skipping permission checks unless started with --safe
- **−** Linux bwrap sandbox applies only in safe mode or when enabled by env var
- **−** No tagged releases on the repository
- **−** README advises against older Q&A-tuned models such as GPT-4o

<sub>no GPU · Docker · Needs Node.js (or standalone Bun-compiled binary), ripgrep (bundled via optionalDependencies), bubblewrap (optional, Linux sandbox) · Models: Anthropic, OpenAI-compatible endpoints · [Repo](https://github.com/shareai-lab/kode-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kode-cli/)</sub>

<a name="golutra"></a>
### #&#8288;144 [golutra](https://github.com/golutra/golutra) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (49) · Freshness: active (80) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · custom license · May 2026</sub>

**Desktop app that runs and coordinates multiple coding-agent CLIs in parallel.**

golutra is a Tauri desktop app (Vue 3 frontend, Rust backend) for Windows, macOS and Linux that wraps existing agent CLIs such as Claude Code, Gemini CLI, Codex CLI, OpenCode, Qwen Code and OpenClaw. It runs several agents in parallel, lets you inspect their logs and inject prompts into their terminal streams, and supports importable workflow templates. Memory (EverOS) and MCP (golutra-mcp) integrations are separate projects.

- **+** Works with existing CLIs: Claude Code, Gemini CLI, Codex CLI, OpenCode, Qwen Code, OpenClaw, any CLI
- **+** Native desktop builds for Windows, macOS and Linux via Tauri
- **+** Workflow templates can be imported and exported in one step
- **+** Prompts can be injected directly into running agent terminal streams
- **−** BSL 1.1 license, not an OSI-approved open-source license
- **−** Roadmap items (CEO Agent, mobile control) are not yet implemented
- **−** README gives no system requirements or build instructions
- **−** Memory and MCP features depend on separate repositories

<sub>no GPU · Needs Agent CLIs such as Claude Code, Gemini CLI, Codex CLI, EverOS (optional memory layer), golutra-mcp (optional MCP connection) · Models: Claude Code, Gemini CLI, Codex CLI, OpenCode, Qwen Code · [Repo](https://github.com/golutra/golutra) · [🌐 Site ↗](https://www.golutra.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/golutra/)</sub>

<a name="agor"></a>
### #&#8288;145 [agor](https://github.com/preset-io/agor) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (14) · Freshness: active (97) · Maintenance: patchy (47) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Oct 2026</sub>

**Web workspace for teams running coding agents on isolated git branches.**

Agor is a web workspace that runs coding-agent CLIs and SDKs (Claude Code, Codex, Gemini, OpenCode, Copilot, Cursor beta) on separate git branches. Each branch gets its own working directory, dev server and conversation history, shown as cards on a shared 2D board with live cursors and comments. It adds persistent teammates with a knowledge base, a scheduler, Slack and GitHub gateways, and an MCP server.

- **+** Runs several agent runtimes interchangeably per session, using your own provider subscriptions
- **+** Per-branch working directory and dev server with automatically assigned ports to avoid collisions
- **+** Branch-scoped RBAC, per-user credentials, and per-prompt token and dollar accounting
- **+** Install via npm (agor-live) or Docker Compose; LibSQL or Postgres storage
- **−** BSL 1.1 license: source-available, not open source until conversion to Apache 2.0
- **−** Cannot be offered to third parties as a hosted or managed agent-orchestration service
- **−** Requires Node.js 22.12 or newer and Git; the daemon runs as a separate process
- **−** Cursor support and Cards are marked beta

<sub>no GPU · Docker + Compose · Needs Node.js >= 22.12, Git, LibSQL or Postgres, Agent CLIs/SDKs (Claude Code, Codex, Gemini, etc.) · Models: Claude Code, Codex, Gemini CLI, GitHub Copilot, OpenCode · port 5173 · [Repo](https://github.com/preset-io/agor) · [📖 Docs ↗](https://agor.live/guide/getting-started) · [🌐 Site ↗](https://agor.live/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agor/)</sub>

<a name="onlook"></a>
### #&#8288;146 [Onlook](https://github.com/onlook-dev/onlook) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (84) · Freshness: recent (75) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Jul 2026</sub>

**Visual editor that edits Next.js and Tailwind apps with AI.**

Browser-based editor that loads a Next.js and Tailwind project into a web container, renders it in an iframe and maps DOM elements back to source so you can drag, restyle and edit visually or through an AI chat. Built on Next.js, tRPC, Supabase, Drizzle and the Vercel AI SDK with OpenRouter for models and CodeSandbox for sandboxes. For designers and front-end developers working on Next.js codebases.

- **+** Edits map directly to code; right-click any element to open its source location
- **+** Branching, checkpoints and a real-time code editor beside the visual canvas
- **+** Apache-2.0 with Dockerfile and compose file for local runs
- **+** Figma-like layers, pages, brand tokens and asset management
- **−** Next.js plus Tailwind only; other frameworks are roadmap items, not supported
- **−** Depends on hosted services: Supabase, OpenRouter, CodeSandbox SDK, Freestyle
- **−** Team comments, MCP support and image references are unchecked roadmap items
- **−** Maintainers are moving to a hosted early-access product; last commit July 2026

<sub>no GPU · Docker + Compose · Needs Supabase (auth, database, storage), OpenRouter API key, CodeSandbox SDK, Bun · Models: OpenRouter-hosted models, Morph Fast Apply, Relace · README: alternative to Lovable, v0, Bolt.new, Replit · [Repo](https://github.com/onlook-dev/onlook) · [▶️ Demo ↗](https://onlook.com) · [📖 Docs ↗](https://docs.onlook.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/onlook/)</sub>

<a name="sidekick-nvim"></a>
### #&#8288;147 [sidekick.nvim](https://github.com/folke/sidekick.nvim) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (37) · Freshness: active (97) · Maintenance: patchy (41) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · Apache-2.0 · Sep 2026</sub>

**Neovim plugin for Copilot next-edit suggestions and a terminal for AI CLIs.**

sidekick.nvim shows Copilot LSP "Next Edit Suggestions" as inline and block diffs in Neovim, which you can step through hunk by hunk and apply. It also runs AI CLI tools (Claude, Codex, Gemini, Copilot CLI, aider, opencode and others) in a Neovim terminal, sends file, selection and diagnostics context to them, and can keep sessions alive through tmux or zellij.

- **+** Treesitter-highlighted diffs down to word or character level, with hunk-by-hunk navigation
- **+** Preconfigured for about a dozen AI CLIs, including Claude, Codex, Gemini and aider
- **+** Prompt templates with context variables such as {file}, {selection} and {diagnostics}
- **+** Reloads buffers when AI tools modify files; tmux and zellij session persistence
- **−** Next Edit Suggestions require the Copilot language server and a Copilot sign-in
- **−** Requires Neovim 0.11.2 or newer
- **−** Provides no model or agent of its own; CLI tools are installed separately
- **−** Optional pieces (snacks.nvim, treesitter-textobjects, lsof, ps) needed for full features

<sub>no GPU · Needs Neovim >= 0.11.2, copilot-language-server, nvim-lspconfig (lsp/copilot.lua), snacks.nvim (optional), tmux or zellij (optional), lsof and ps (optional) · Models: GitHub Copilot (Next Edit Suggestions), Claude CLI, Codex, Gemini, Grok · [Repo](https://github.com/folke/sidekick.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sidekick-nvim/)</sub>

<a name="tabby"></a>
### #&#8288;148 [Tabby](https://github.com/tabbyml/tabby) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: widely used (89) · Freshness: active (85) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Jun 2026</sub>

**Self-hosted code completion and chat server for IDEs.**

Serves code completion and chat to VS Code, Vim and JetBrains extensions from one self-contained binary with no external database. Runs local models such as StarCoder-1B and Qwen2-1.5B-Instruct on CUDA or Apple Metal, exposes an OpenAPI interface on port 8080, and adds an Answer Engine, repository and GitLab merge-request indexing and LDAP auth. For teams that want an on-premises Copilot alternative.

- **+** Single binary with embedded storage; no DBMS or cloud service required
- **+** One docker run command starts a server with completion and chat models
- **+** Repository context indexing, GitHub and GitLab integration, LDAP auth, usage reports
- **+** Live demo instance and documented extensions for VS Code, Vim and IntelliJ
- **−** Last commit June 2026; recent news points to the separate Pochi agent
- **−** License is non-standard (GitHub reports NOASSERTION); check terms before deploying
- **−** Model list and hardware guidance live only in the external docs
- **−** Building from source needs Rust, protobuf and OpenBLAS

<sub>GPU optional · Docker · Models: StarCoder-1B, Qwen2-1.5B-Instruct, CodeLlama 7B, CodeGemma, CodeQwen · port 8080 · README: alternative to GitHub Copilot · [Repo](https://github.com/tabbyml/tabby) · [▶️ Demo ↗](https://tabby.tabbyml.com) · [📖 Docs ↗](https://tabby.tabbyml.com/docs/welcome/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tabby/)</sub>

<a name="minuet-ai-nvim"></a>
### #&#8288;149 [minuet-ai.nvim](https://github.com/milanglacier/minuet-ai.nvim) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · GPL-3.0 · Oct 2026</sub>

**LLM code completion plugin for Neovim with FIM and chat-model support.**

Minuet is a Neovim plugin that requests code completions from LLM providers (OpenAI, Claude, Gemini, Codestral, Ollama, llama.cpp and OpenAI-compatible endpoints) using curl via vim.system. Results appear through virtual text, nvim-cmp, blink.cmp, or an in-process LSP server for built-in completion. It also has an experimental next-edit prediction mode called duet.

- **+** Works with hosted APIs and local servers such as Ollama and llama.cpp
- **+** Supports fill-in-the-middle and chat-model prompts for completion
- **+** Frontends: virtual text, nvim-cmp, blink.cmp, built-in LSP completion
- **+** No background binary; requests go through curl, with streaming support
- **−** Neovim only; needs 0.10+, and 0.11 or 0.12 for built-in and inline LSP completion
- **−** Requires an API key or a self-run local model server
- **−** Duet next-edit prediction is described as highly experimental
- **−** Built-in completion can mis-indent multi-line suggestions, notably in Python

<sub>GPU optional · Needs Neovim 0.10+, curl, LLM provider API key or local server (Ollama, llama.cpp), nvim-cmp or blink.cmp (optional) · Models: OpenAI, Claude, Gemini, Codestral, Mercury Coder · [Repo](https://github.com/milanglacier/minuet-ai.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/minuet-ai-nvim/)</sub>

<a name="opcode"></a>
### #&#8288;150 [opcode](https://github.com/winfunc/opcode) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (83) · Freshness: recent (80) · Maintenance: weak (15) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · AGPL-3.0 · Sep 2026</sub>

**Tauri desktop GUI for Claude Code projects, sessions and custom agents.**

opcode is a Tauri 2 desktop app (React frontend, Rust backend, SQLite) that sits on top of the Claude Code CLI. It browses projects and sessions under ~/.claude/projects/, runs custom agents as separate processes, and tracks token usage and cost. It also manages MCP servers, session checkpoints with a diff viewer, and CLAUDE.md files.

- **+** Checkpoints with branching timeline, fork and diff viewer for Claude Code sessions
- **+** Usage dashboard breaks down tokens and cost by model, project and date, with export
- **+** Reads existing ~/.claude data and can import MCP servers from Claude Desktop
- **+** Data stays local in SQLite; README states no telemetry
- **−** Requires the Claude Code CLI; README mentions only Claude models
- **−** README says prebuilt executables are not yet published; build needs Rust and Bun
- **−** AGPL-3.0 license may restrict use in some organizations
- **−** Last tagged release is 2025-08-31, older than recent commits

<sub>RAM ≥ 4 GB · no GPU · Needs Claude Code CLI, Rust 1.70+, Bun, Git · Models: Claude · [Repo](https://github.com/winfunc/opcode) · [🌐 Site ↗](https://asterisk.so/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opcode/)</sub>

<a name="aider"></a>
### #&#8288;151 [aider](https://github.com/aider-ai/aider) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: widely used (93) · Freshness: recent (61) · Maintenance: weak (18) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · Apache-2.0 · May 2026</sub>

**Terminal pair-programming tool that edits your git repo with LLMs.**

Aider runs in the terminal and edits files in an existing codebase through chat with a cloud or local LLM. It builds a map of the repository to give the model context, commits each change to git with a generated message, and can run linters and tests after edits and try to fix failures. It also accepts images, web pages and voice input, and can be triggered by comments in an editor.

- **+** Auto-commits every change to git, so diffs and undo use ordinary git tools
- **+** Connects to almost any LLM, including local models
- **+** Runs linters and tests after edits and attempts to fix reported failures
- **+** Repo map gives the model context across larger codebases
- **−** Terminal-first; no standalone GUI, IDE use relies on comment watching
- **−** Last tagged release is 2025-08-09, older than recent commits
- **−** Needs an LLM API key or a separately hosted local model
- **−** Installed via pip and aider-install; no Docker setup in the repo

<sub>no GPU · Docker · Needs LLM provider API key or local model server · Models: Claude 3.7 Sonnet, DeepSeek R1 and V3, OpenAI o1, o3-mini, GPT-4o, local models · [Repo](https://github.com/aider-ai/aider) · [📖 Docs ↗](https://aider.chat/docs/install.html) · [🌐 Site ↗](https://aider.chat/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aider/)</sub>

<a name="copilotforxcode"></a>
### #&#8288;152 [copilotforxcode](https://github.com/intitni/copilotforxcode) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (66) · Freshness: active (93) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Oct 2026</sub>

**Xcode source editor extension adding Copilot, Codeium and ChatGPT-based chat and edits.**

A macOS app and Xcode Source Editor Extension that adds code suggestions from GitHub Copilot or Codeium, a chat panel, and a prompt-to-code modification window inside Xcode. A background service app does the work and reads Xcode state through the Accessibility API. Custom commands with template arguments such as {{selected_code}} extend chat and modification.

- **+** Works inside Xcode itself: suggestions, chat panel and code modification from one extension
- **+** Suggestion providers: GitHub Copilot or Codeium; chat uses OpenAI or other configurable models
- **+** Custom commands with template arguments for selected code, language, file name and clipboard
- **+** Installable via Homebrew cask; chat has /shell and Shortcuts.app plugins
- **−** Setup is multi-step: extension enabling, Accessibility permission, accounts, key bindings
- **−** Requires Accessibility API and folder access permissions for the background service
- **−** Xcode state monitoring may fail, especially with multiple Xcode windows or displays
- **−** Needs a paid Copilot or Codeium account, or an OpenAI key, plus Node for Copilot

<sub>no GPU · Needs Xcode, macOS, Node (for GitHub Copilot language server), GitHub Copilot, Codeium or OpenAI account · Models: GitHub Copilot, Codeium, OpenAI, other LLMs · [Repo](https://github.com/intitni/copilotforxcode) · [📖 Docs ↗](https://copilotforxcode.intii.com/wiki) · [🌐 Site ↗](https://copilotforxcode.intii.com/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/copilotforxcode/)</sub>

<a name="swe-agent"></a>
### #&#8288;153 [swe-agent](https://github.com/swe-agent/swe-agent) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: widely used (81) · Freshness: recent (68) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Jul 2026</sub>

**Research agent that lets an LLM fix GitHub issues using tools.**

SWE-agent lets a language model such as GPT-4o or Claude Sonnet 4 autonomously use tools to fix issues in real GitHub repositories, find cybersecurity vulnerabilities, or run custom tasks. Behavior is governed by a single yaml file, and it can be run in batch mode for SWE-bench. The README says the maintainers now focus on mini-swe-agent, which supersedes it, and recommend using that instead.

- **+** Single yaml file configures agent behavior; documentation site covers install, usage and batch mode
- **+** Batch mode for benchmarking on SWE-bench
- **+** Works with the model of your choice, e.g. GPT-4o or Claude Sonnet 4
- **+** MIT license, built by Princeton and Stanford researchers with an accompanying paper
- **−** README says mini-swe-agent supersedes it and recommends using that instead
- **−** Last release was 2025-05-22, well behind recent commits
- **−** EnIGMA cybersecurity mode requires SWE-agent 0.7 until it is updated for 1.0
- **−** Built for research and benchmarks rather than daily IDE-style assistance

<sub>no GPU · Models: GPT-4o, Claude Sonnet 4, Claude 3.7 · [Repo](https://github.com/swe-agent/swe-agent) · [📖 Docs ↗](https://swe-agent.com/latest/) · [🌐 Site ↗](https://swe-agent.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/swe-agent/)</sub>

<a name="grok-cli"></a>
### #&#8288;154 [grok-cli](https://github.com/superagent-ai/grok-cli) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (45) · Freshness: active (81) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · May 2026</sub>

**Terminal coding agent for the xAI Grok API with sub-agents and Telegram control.**

grok-cli is a TypeScript terminal coding agent built on Bun and OpenTUI that talks to xAI's Grok API. It runs interactively or headless (`--prompt`, optional `--format json` event stream, xAI Batch API), with X and web search tools, sub-agents, MCP servers, skills, hooks and saved sessions. It can also be driven from Telegram, and run shell commands in a Shuru microVM sandbox on Apple Silicon.

- **+** Headless mode with newline-delimited JSON events and Batch API option suits CI and scripts
- **+** Supports MCP servers, Agent Skills, AGENTS.md and lifecycle hooks (17 events, exit code 2 blocks)
- **+** Custom sub-agents defined in user-settings.json alongside built-in explore, general, computer and verify
- **+** Telegram remote control with voice-note transcription through the Grok speech-to-text endpoint
- **−** Tied to the xAI Grok API and requires a Grok API key; no other providers documented
- **−** Sandbox mode needs macOS 14+ on Apple Silicon; unavailable on Intel Mac or Linux
- **−** Computer sub-agent targets macOS only and needs Accessibility permission
- **−** Community project, not affiliated with xAI; interactive UI documented for four terminal emulators

<sub>no GPU · Needs Grok API key (xAI), Bun, Telegram bot token (optional), Shuru (optional sandbox), agent-desktop (optional, macOS) · Models: grok-4.3, grok-4.20-non-reasoning, grok-4.20-multi-agent-0309 · [Repo](https://github.com/superagent-ai/grok-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/grok-cli/)</sub>

<a name="helmor"></a>
### #&#8288;155 [helmor](https://github.com/dohooo/helmor) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (6) · Freshness: active (99) · Maintenance: weak (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Jul 2026</sub>

**Desktop app that runs parallel coding agents in isolated git worktrees.**

Helmor is a desktop app for macOS and Windows that runs several coding agents at once, each in its own git worktree and branch. Diffs, a Monaco editor, terminals and PR actions for GitHub and GitLab sit beside the conversation. It also ships a `helmor` CLI and an MCP server, and stores its data locally under `~/helmor/`.

- **+** One git worktree and branch per task, so parallel agents do not collide
- **+** Supports Claude Code, Codex, Cursor, OpenCode and Kimi Code with your own logins or keys
- **+** CLI with --json output and a stdio MCP server let scripts or other agents drive it
- **+** Create PR/MR, merge, fix CI and resolve conflicts from the UI; GitHub and GitLab
- **−** Desktop only: macOS and Windows x64 listed, no Linux build mentioned
- **−** Mobile companion is experimental and relies on a Cloudflare tunnel
- **−** CLI is installed from Settings → Experimental
- **−** Plan mode and Slack/GitHub context are listed as not yet available

<sub>no GPU · Needs GitHub or GitLab account, Cloudflare tunnel (mobile companion, experimental) · Models: Claude Code, Codex, Cursor, OpenCode, Kimi Code · [Repo](https://github.com/dohooo/helmor) · [📖 Docs ↗](https://docs.helmor.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/helmor/)</sub>

<a name="core"></a>
### #&#8288;156 [core](https://github.com/opensumi/core) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: known (46) · Freshness: recent (71) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**TypeScript framework for building AI-native IDEs for web and Electron.**

OpenSumi is a TypeScript framework for assembling IDE products that run as a cloud IDE, in the browser, or on Electron. It acts as an MCP client with tool support, and the README links starter projects including a cloud IDE, an Electron desktop IDE and CodeFuse IDE. Development uses yarn, and docs are on opensumi.com.

- **+** Several starters: cloud IDE, Electron desktop IDE, lite web IDE, CodeBlitz
- **+** MCP client badge with tools support
- **+** MIT license; CI, E2E and coverage workflows are published
- **+** Used as the base of CodeFuse IDE, an AI IDE
- **−** Framework, not a ready-to-use IDE; you assemble and host the product yourself
- **−** README does not describe the AI features or supported models
- **−** Last tagged release is 2025-05-20, well before the latest commit
- **−** Dev setup may need extra system-level dependencies

<sub>Needs Node.js, yarn · [Repo](https://github.com/opensumi/core) · [▶️ Demo ↗](https://codeblitz.cloud.alipay.com/github/opensumi/core) · [📖 Docs ↗](https://opensumi.com) · [🌐 Site ↗](https://opensumi.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/core/)</sub>

<a name="toad"></a>
### #&#8288;157 [toad](https://github.com/batrachianai/toad) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: known (45) · Freshness: active (84) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · AGPL-3.0 · May 2026</sub>

**Terminal UI that runs coding agents over the Agent Client Protocol.**

Toad is a Python terminal UI that front-ends coding agents such as Claude, Gemini, Codex and OpenHands through the Agent Client Protocol. It includes a real persistent shell, a Markdown prompt editor, an @ fuzzy file picker, diff views, concurrent agent sessions and session resume. It can also be served in a browser with `toad serve`.

- **+** Works with many agents via ACP, with an in-UI agent browser and installer
- **+** Integrated shell keeps cwd and env vars, and supports interactive commands
- **+** Runs several agents from different providers at once, with session resume
- **+** Can be served as a web app with `toad serve`
- **−** No native Windows support; WSL is needed
- **−** AGPL-3.0 license; commercial license required for non-AGPL use
- **−** Model selection, MCP server UI and built-in editor are still on the roadmap
- **−** Default macOS terminal gives a reduced experience

<sub>no GPU · Needs uv, Python 3.14, xclip (Linux clipboard), a coding agent supporting ACP · Models: Claude, Gemini, Codex, OpenHands · [Repo](https://github.com/batrachianai/toad) · [🌐 Site ↗](https://willmcgugan.github.io/toad-released/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/toad/)</sub>

<a name="trae-agent"></a>
### #&#8288;158 [trae-agent](https://github.com/bytedance/trae-agent) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: popular (75) · Freshness: slowing (37) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Feb 2026</sub>

**Research-oriented CLI agent that runs software engineering tasks with LLM tools.**

Trae Agent is a Python CLI that takes a natural-language task and runs an LLM loop with bash, file-edit, sequential-thinking and task-done tools. It works with OpenAI, Anthropic, Google Gemini, Azure, OpenRouter, Doubao and Ollama, and can run tasks inside Docker containers. It records full trajectories to JSON and is built to be modified for agent research.

- **+** Many providers, including Ollama for local models, plus custom base_url support
- **+** Trajectory files log LLM calls, steps and tool use for debugging and analysis
- **+** Can run tasks in a new or existing Docker container, or one built from a Dockerfile
- **+** Optional MCP servers configured in YAML; modular code aimed at ablation studies
- **−** Terminal only; no IDE extension or web UI described
- **−** Installed from source with uv and Python 3.12+; no release published
- **−** Config is YAML with a legacy JSON format; tabs are not allowed
- **−** README says the project is still under active development

<sub>no GPU · Needs uv, Python 3.12+, LLM provider API key, Docker (optional) · Models: OpenAI, Anthropic, Google Gemini, Azure, OpenRouter · [Repo](https://github.com/bytedance/trae-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trae-agent/)</sub>

<a name="proxyai"></a>
### #&#8288;159 [proxyai](https://github.com/carlrobertoh/proxyai) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (24) · Freshness: active (84) · Maintenance: weak (5) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · May 2026</sub>

**JetBrains plugin for AI chat, autocomplete and code edits.**

ProxyAI is a Kotlin plugin for JetBrains IDEs that adds chat, inline autocomplete, next-edit suggestions and natural-language code edits. It connects to hosted providers such as OpenAI, Anthropic, Azure and Mistral, or to a self-hosted model for offline use. Suggested changes stream into the editor and can be reviewed in diff view before applying.

- **+** Chat can reference project files, folders, git history, web docs and images
- **+** Auto Apply streams edits into the editor with diff preview and accept or reject
- **+** Works with hosted providers or a self-hosted model for offline use
- **+** Also generates commit messages and name suggestions
- **−** Runs only inside JetBrains IDEs; no VS Code or standalone editor
- **−** Collects anonymous usage data, with user consent
- **−** README does not name supported self-hosted backends or model formats
- **−** Building from source needs git submodules and Gradle runIde

<sub>Needs JetBrains IDE, Gradle (build from source) · Models: OpenAI, Anthropic, Azure, Mistral, self-hosted models · README: alternative to GitHub Copilot · [Repo](https://github.com/carlrobertoh/proxyai) · [📖 Docs ↗](https://docs.tryproxy.io/features) · [🌐 Site ↗](https://plugins.jetbrains.com/plugin/21056-proxy-ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/proxyai/)</sub>

<a name="neovate-code"></a>
### #&#8288;160 [neovate-code](https://github.com/neovateai/neovate-code) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (15) · Freshness: recent (63) · Maintenance: weak (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Mar 2026</sub>

**Terminal coding agent that edits code, fixes bugs and writes tests.**

Neovate Code is a command-line coding agent installed from npm as @neovate/code and started with `neovate`. You describe a task in the terminal, review the proposed changes and approve tool calls. It reads API keys from environment variables for each provider, or you can sign in with `/login` and pick a model with `/model`.

- **+** Installs with one npm command; runs on macOS, Linux and Windows
- **+** Respects provider API key environment variables, with /login and /model for setup
- **+** Asks for approval on tool calls and shows proposed changes before applying
- **+** MIT license with a documented quickstart and contributing guide
- **−** README does not list supported providers or models
- **−** Requires Node.js and npm; the README gives no minimum version
- **−** No demo or screenshots of workflows beyond a single image
- **−** README does not describe plugins, MCP support or sandboxing

<sub>no GPU · Needs Node.js, npm, LLM provider API key · [Repo](https://github.com/neovateai/neovate-code) · [📖 Docs ↗](https://neovateai.dev/en/docs/quickstart) · [🌐 Site ↗](https://neovateai.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neovate-code/)</sub>

<a name="copilot-vim"></a>
### #&#8288;161 [copilot.vim](https://github.com/github/copilot.vim) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (74) · Freshness: quiet (27) · Maintenance: weak (2) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Jan 2026</sub>

**Inline GitHub Copilot code suggestions for Vim and Neovim.**

Vim and Neovim plugin that shows GitHub Copilot completions inline as you type, built from comments and method names. Suggestions are accepted with Tab. It needs Node.js and an active Copilot subscription, including the Free tier, and is set up with `:Copilot setup`.

- **+** Works in both Vim (9.0.0185 or newer) and Neovim
- **+** Installs with any plugin manager or a plain git clone into the pack directory
- **+** Inline suggestions accepted with Tab; built-in help via `:help copilot`
- **+** Copilot Free tier is available for sign-up
- **−** Requires a GitHub Copilot subscription and a connection to the hosted service
- **−** Needs Node.js (and NPM) installed separately
- **−** Inline completion only; the README mentions no repo-wide agent features
- **−** License not identified (NOASSERTION); README lists no supported models

<sub>no GPU · Needs Node.js, NPM, GitHub Copilot subscription, Vim 9.0.0185+ or Neovim · [Repo](https://github.com/github/copilot.vim) · [🌐 Site ↗](https://github.com/features/copilot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/copilot-vim/)</sub>

<a name="chatgpt-vscode"></a>
### #&#8288;162 [chatgpt-vscode](https://github.com/ai-genie/chatgpt-vscode) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (5) · Freshness: recent (70) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · ISC · Oct 2026</sub>

**VS Code extension for prompting OpenAI models on selected code.**

Genie is a VS Code extension that sends selected code to OpenAI GPT-4, GPT-3.5 or Codex models, or to Azure OpenAI deployments, using your own API key. It adds context-menu commands (explain, find bugs, add tests, optimize), a sidebar chat with streaming and on-disk history, a diff view of suggestions, and commit message generation. The repository holds documentation and issue tracking only.

- **+** Context-menu commands for explain, find bugs, add tests, optimize, with editable prompts
- **+** Supports Azure OpenAI deployments via the genieai.azure.url setting
- **+** Generates git commit messages, with configurable prompt and opt-out setting
- **+** Conversation history stored locally and exportable as Markdown
- **−** Only OpenAI and Azure OpenAI backends are documented; no local or other providers
- **−** Repository is for docs and bug reports; extension source is not included
- **−** Requires an OpenAI API key, billed separately from ChatGPT Plus
- **−** Conversation history is experimental and opt-in, with limitations noted in the README

<sub>no GPU · Needs Visual Studio Code, OpenAI API key or Azure OpenAI deployment · Models: gpt-4o, gpt-4-turbo, gpt-4, gpt-3.5-turbo, o1-mini · [Repo](https://github.com/ai-genie/chatgpt-vscode) · [🌐 Site ↗](https://marketplace.visualstudio.com/items?itemName=genieai.chatgpt-vscode) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chatgpt-vscode/)</sub>

<a name="octogent"></a>
### #&#8288;163 [octogent](https://github.com/hesamsheikh/octogent) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (11) · Freshness: recent (64) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Apr 2026</sub>

**Local UI that coordinates multiple Claude Code terminals with per-task context folders.**

Octogent runs several Claude Code sessions from a local web UI and API. Each job gets a "tentacle" folder holding CONTEXT.md, todo.md and notes, and a Claude Code agent can spawn child agents from todo items and message them. Terminals can share the main workspace or run in git worktrees on separate branches.

- **+** Scoped markdown context per job (CONTEXT.md, todo.md) that agents read and update
- **+** Spawns worker agents from todo checkbox items, with inter-agent messaging
- **+** Optional git worktree isolation on octogent/<id> branches
- **+** CLI commands to list, stop, kill and prune terminal sessions
- **−** Docs cover only Claude Code; startup needs the claude binary
- **−** Not published to npm; install requires building from a clone
- **−** PTY sessions do not survive an API restart and are marked stale
- **−** Described as a personal exploration; pull requests not currently being reviewed

<sub>no GPU · Needs Node.js 22+, claude (Claude Code CLI), git, gh, curl · Models: Claude Code · port 8787 · [Repo](https://github.com/hesamsheikh/octogent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/octogent/)</sub>

<a name="amazon-q-developer-cli"></a>
### #&#8288;164 [amazon-q-developer-cli](https://github.com/aws/amazon-q-developer-cli) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: niche (25) · Freshness: recent (62) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Apr 2026</sub>

**Terminal client for Amazon Q Developer chat, written in Rust, now unmaintained.**

Amazon Q Developer CLI is the Rust source for the `q` command, which lets you talk to Amazon Q Developer from the terminal. The repository is no longer actively maintained and gets only critical security fixes, since the product continues as the closed-source Kiro CLI. The README covers installation and a cargo-based contributor setup, but not the agent features themselves.

- **+** Open source Rust codebase under Apache-2.0 (dual MIT), buildable with cargo run --bin chat_cli
- **+** Installers for macOS (DMG, Homebrew) and Linux (Ubuntu/Debian, AppImage, alternative builds)
- **+** Includes docs and scripts directories for studying how the CLI is built
- **−** No longer actively maintained; only critical security fixes are accepted
- **−** Successor Kiro CLI is closed source, so new features will not land here
- **−** Requires an Amazon Q Developer login; README documents no other model backends
- **−** README has no feature list, model details or usage examples

<sub>no GPU · Needs Amazon Q Developer account (login), Rust toolchain (to build) · Models: unknown · [Repo](https://github.com/aws/amazon-q-developer-cli) · [📖 Docs ↗](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/command-line-installing.html) · [🌐 Site ↗](https://kiro.dev/cli/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/amazon-q-developer-cli/)</sub>

<a name="aiac"></a>
### #&#8288;165 [aiac](https://github.com/gofireflyio/aiac) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: known (48) · Freshness: slowing (38) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Mar 2026</sub>

**CLI that generates Terraform, Dockerfiles, k8s manifests and queries from prompts.**

aiac is a Go command line tool and library that sends a prompt such as "terraform for AWS EC2" to an LLM backend and extracts the code from the reply. It supports OpenAI (including Azure OpenAI), Amazon Bedrock and Ollama, configured as named backends in a TOML file. Output goes to stdout or files, with an interactive shell for retries and follow-ups.

- **+** Named backends in one TOML file, so staging and production providers can coexist
- **+** Works with OpenAI, Azure OpenAI, Amazon Bedrock and local Ollama
- **+** Quiet mode with file output and clipboard flags suits scripting
- **+** Usable as a Go library (libaiac) as well as a CLI
- **−** Does not read your repo or run commands; it only generates code from a prompt
- **−** Chat models only; completion models dropped in v5
- **−** Does not validate model names, and --list-models may show unusable models
- **−** Last release 2024-10-29; Ollama behind an authenticating proxy is unsupported

<sub>no GPU · Docker · Needs OpenAI API key, Amazon Bedrock account, or Ollama server · Models: OpenAI, Azure OpenAI, Amazon Bedrock, Ollama · [Repo](https://github.com/gofireflyio/aiac) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aiac/)</sub>

<a name="codemachine-cli"></a>
### #&#8288;166 [codemachine-cli](https://github.com/moazbuilds/codemachine-cli) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: known (33) · Freshness: recent (54) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Feb 2026</sub>

**CLI that chains AI coding agents into repeatable, multi-step workflows.**

CodeMachine is a TypeScript CLI, installed with npm, that runs AI coding CLIs such as Claude Code, Codex and Cursor through workflows you define once and rerun. It spawns each engine in its headless mode, passes context between steps, and can run several agents in parallel or over long periods. A default "Ali Workflow Builder" workflow helps you create your first workflow interactively.

- **+** Drives existing coding CLIs (Claude Code, Codex, Cursor) instead of replacing them
- **+** Supports multi-agent and parallel execution within one workflow
- **+** Workflows can run for hours or days with persistence handled by the tool
- **+** Covers interactive through fully autonomous orchestration patterns
- **−** Needs a separate coding agent CLI installed; it does not supply models itself
- **−** Depends on each engine's headless mode, so behavior follows those tools
- **−** README gives no system requirements, config format or workflow file examples
- **−** Full list of supported engines is not stated in the README

<sub>Compose · Needs Node.js/npm, AI coding CLI (Claude Code, Codex, Cursor) · Models: Claude Code, Codex, Cursor · [Repo](https://github.com/moazbuilds/codemachine-cli) · [▶️ Demo ↗](https://www.youtube.com/watch?v=G7OTG9iSvYw) · [📖 Docs ↗](https://docs.codemachine.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codemachine-cli/)</sub>

<a name="mle-agent"></a>
### #&#8288;167 [mle-agent](https://github.com/mlsysops/mle-agent) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (17) · Freshness: recent (65) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Jul 2026</sub>

**CLI agent that builds ML baselines and runs Kaggle tasks.**

MLE-Agent is a Python CLI that acts as a pairing agent for ML engineers. It plans an ML task from vague requirements, writes and runs code locally, debugs errors, and can search Arxiv and Papers with Code. It also has an auto mode for Kaggle competitions, an interactive chat, and a weekly report generator from GitHub or a local git repo.

- **+** Auto Kaggle mode runs data prep to submission without human input
- **+** Searches Arxiv and Papers with Code to inform solutions
- **+** Installs from PyPI with pip or uv; MIT license
- **+** Report command works from GitHub or a local git repo
- **−** Last tagged release is 2024-10-12; README milestones stop at 0.4.2
- **−** Many roadmap integrations (Hugging Face, MLflow, Wandb, S3) are unchecked
- **−** README names few models: Ollama Llama3, OpenAI, Claude 3.5 Sonnet, Mistral
- **−** Hardware needs and API key setup are not documented in the README

<sub>Needs Python, LLM provider or Ollama, Kaggle account (for Kaggle mode) · Models: OpenAI, Anthropic Claude, Ollama, Mistral · port 3000 · [Repo](https://github.com/mlsysops/mle-agent) · [📖 Docs ↗](https://mle-agent-site.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mle-agent/)</sub>

<a name="chatgpt-nvim"></a>
### #&#8288;168 [chatgpt.nvim](https://github.com/jackmort/chatgpt.nvim) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: known (49) · Freshness: quiet (20) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Jan 2026</sub>

**Neovim plugin for chat, code editing and actions via the OpenAI API.**

ChatGPT.nvim adds a chat window, an edit-with-instructions window and a set of ChatGPTRun actions (fix_bugs, add_tests, docstring, explain_diagnostic and others) to Neovim, backed by the OpenAI API. Custom actions are defined in a JSON file with templates, and Azure OpenAI and custom API hosts are supported. It calls the API through curl; the last tagged release is from January 2023, though commits continue into 2026.

- **+** Custom actions defined in JSON with template variables like {{input}}, {{filetype}} and {{diagnostic}}
- **+** API key can come from a command (api_key_cmd), such as 1Password or GPG, instead of an env var
- **+** Supports Azure OpenAI and a custom API host via config or environment variables
- **+** Inline @ references pull in LSP definitions or project files as prompt context
- **−** Only OpenAI-style APIs are documented; no local model or other provider setup is described
- **−** Does not run commands or work across the repo as an agent; it edits buffers and selections
- **−** Requires paid OpenAI API credits; a ChatGPT Plus subscription does not cover them
- **−** Last tagged release is 2023-01-08, so versioned installs are old; the README notes edit models are deprecated

<sub>no GPU · Needs Neovim, curl, nui.nvim, plenary.nvim, telescope.nvim, trouble.nvim (optional), OpenAI API key · Models: OpenAI GPT models (gpt-5-mini default), Azure OpenAI · [Repo](https://github.com/jackmort/chatgpt.nvim) · [▶️ Demo ↗](https://www.youtube.com/watch?v=7k0KZsheLP4) · [📖 Docs ↗](https://github.com/jackMort/ChatGPT.nvim/blob/main/lua/chatgpt/config.lua) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chatgpt-nvim/)</sub>

<a name="10x"></a>
### #&#8288;169 [10x](https://github.com/ntegrals/10x) <sub>score [10](../README.md#-how-we-rank "Score 10/100. Adoption: niche (8) · Freshness: quiet (26) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Jan 2026</sub>

**Terminal coding assistant that chains models in multi-step workflows.**

10x is an npm-installed CLI (10x-cli, TypeScript) for coding in the terminal. It runs multi-step workflows called Superpowers (/review, /pr, /refactor, /debug, /test) and routes each step to a fast or a smart model tier. It supports a bring-your-own OpenRouter key, project context in 10X.md, and custom workflows and skills as Markdown files.

- **+** Each workflow step can target a different model tier (superfast, fast, smart)
- **+** Custom workflows and skills are plain Markdown files in .10x/ or ~/.config/10x/
- **+** BYOK mode with an OpenRouter key; MIT licensed
- **+** Non-interactive mode via -x and session resume via --resume
- **−** The 'up to 20x faster' claim has no benchmark in the README and applies to the smallest tier
- **−** Non-BYOK hosting and pricing are not described in the README
- **−** No docs site, demo or release tags; only the README documents usage
- **−** README does not describe sandboxing or permission controls for command execution

<sub>no GPU · Needs Node.js/npm, OpenRouter API key (BYOK) · Models: GPT OSS 20B, Kimi K2 1T, Claude Opus 4 · [Repo](https://github.com/ntegrals/10x) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/10x/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
