# 🤖 Coding agents and AI editors reviews · Best of Vibe Coding

Agents, assistants and editors that read your repo, write code and run commands, including tools that turn designs and screenshots into code. Back to the [leaderboard](../README.md#-coding-agents-and-ai-editors).

<sub>🌐 Also on the web: [Coding agents and AI editors on archestack.com](https://archestack.com/best-of-vibe-coding/coding-agents/), each project on its own page.</sub>

<a name="claw-code"></a>
### 🥇 [claw-code](https://github.com/ultraworkers/claw-code) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 195k · MIT · Oct 2026</sub>

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

<a name="archon"></a>
### 🥈 [Archon](https://github.com/coleam00/archon) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<a name="open-swe"></a>
### 🥉 [Open SWE](https://github.com/langchain-ai/open-swe) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (100) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

**LangChain coding agent that plans, implements and reviews pull requests.**

LangGraph-based agent that investigates a repository, implements changes in a per-thread Linux sandbox, validates them and opens a pull request, then reviews PRs and watches CI with /baby-sit. Work starts from a dashboard, GitHub issues or PR comments, Slack or Linear. Deploys into your infrastructure with a backend, dashboard, GitHub and Slack apps, for teams building an internal coding-agent service.

- **+** Covers build, review, investigate and operate flows, with subagents for parallel work
- **+** Durable execution and thread state via LangGraph; sandboxes persist per thread
- **+** Configurable models, reasoning effort, skills, MCP integrations and sandbox providers
- **+** Push approvals gate detected git pushes; PR chat excludes mutation tools
- **−** Production standalone Agent Server deployments require a license key
- **−** Maintainers are not accepting issues or contributions; breaking changes expected
- **−** LangSmith is the default sandbox and tracing provider; alternatives need configuration
- **−** CLI mode executes commands locally as you, with no sandbox isolation

<sub>no GPU · Docker + Compose · Needs LangSmith (default sandbox and tracing), GitHub App, Slack app (optional), model provider credentials · Models: configurable LLM providers · [Repo](https://github.com/langchain-ai/open-swe) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-swe/)</sub>

<a name="opencode"></a>
### #&#8288;4 [opencode](https://github.com/anomalyco/opencode) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 217k · MIT · Oct 2026</sub>

**Terminal coding agent with build and plan modes, plus a desktop app.**

OpenCode is an AI coding agent that runs in the terminal and as a beta desktop app for macOS, Windows and Linux. It ships a full-access build agent, a read-only plan agent that asks before running bash commands, and a general subagent invoked with @general. It installs through a curl script, npm, Homebrew, Scoop, Chocolatey, pacman, mise or nix.

- **+** Read-only plan agent denies file edits by default and asks before bash commands
- **+** Many install paths: curl script, npm, brew, scoop, choco, pacman, mise, nix
- **+** Switch between build and plan agents with the Tab key
- **+** MIT licensed, with desktop installers for macOS, Windows and Linux
- **−** README does not list supported model providers or formats
- **−** Desktop app is marked BETA
- **−** README gives no hardware requirements; configuration is only in external docs
- **−** Primary install command pipes a curl script into bash

<sub>[Repo](https://github.com/anomalyco/opencode) · [📖 Docs ↗](https://opencode.ai/docs) · [🌐 Site ↗](https://opencode.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencode/)</sub>

<a name="pi"></a>
### #&#8288;5 [pi](https://github.com/earendil-works/pi) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 116k · MIT · Oct 2026</sub>

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
### #&#8288;6 [oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 70k · custom license · Oct 2026</sub>

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
### #&#8288;7 [goose](https://github.com/aaif-goose/goose) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 55k · Apache-2.0 · Oct 2026</sub>

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

<a name="herdr"></a>
### #&#8288;8 [herdr](https://github.com/herdrdev/herdr) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (93) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 45k · Apache-2.0 · Oct 2026</sub>

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

<a name="codewhale"></a>
### #&#8288;9 [codewhale](https://github.com/codewhale-hq/codewhale) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

**Terminal coding agent in Rust that works with hosted or local models.**

Codewhale is a coding agent that reads a project, edits files, runs commands and checks its own work from a terminal UI. It supports over 40 built-in provider routes plus any OpenAI-compatible endpoint, Ollama, vLLM and SGLang. The same local engine also serves headless `exec` runs, a local browser client, PR review and an HTTP runtime API.

- **+** Over 40 built-in provider routes plus OpenAI-compatible endpoints, Ollama, vLLM and SGLang
- **+** Plan, Work and Operate modes with Ask, Auto-Review and Full Access postures
- **+** `/undo`, `/restore` and `/receipts` recover changes and list files, commands and approvals
- **+** Headless `exec --auto` and `review --pr N` for scripts and CI
- **−** Usage telemetry is on by default and must be disabled with a config command
- **−** OS sandbox only on macOS (Seatbelt) and Linux with bubblewrap installed
- **−** Native desktop app is still being built; VS Code extension is community-maintained
- **−** Computer Use plugin must be reviewed and enabled manually before use

<sub>GPU optional · Docker · Needs Ollama, vLLM or SGLang (optional, for local models), bubblewrap (optional, Linux sandbox) · Models: Anthropic, DeepSeek, Google, Mistral, Moonshot · [Repo](https://github.com/codewhale-hq/codewhale) · [📖 Docs ↗](https://github.com/codewhale-hq/codewhale/blob/main/docs/README.md) · [🌐 Site ↗](https://codewhale.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codewhale/)</sub>

<a name="deepseek-reasonix"></a>
### #&#8288;10 [deepseek-reasonix](https://github.com/esengine/deepseek-reasonix) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

**Coding agent for terminal, desktop, browser and VS Code, with DeepSeek preset.**

Reasonix is a Go coding agent that reads a project folder, edits files and runs commands and tests, showing each step. Models are set in reasonix.toml: a DeepSeek preset is built in and any OpenAI-compatible endpoint is a config entry. It ships as the Studio desktop app, a CLI/TUI, a local web UI (`reasonix web`), and a VS Code extension or ACP connection for other editors.

- **+** Any OpenAI-compatible provider is a config entry; DeepSeek ships as a preset
- **+** Permission levels and plan mode; forbid rules always apply
- **+** Rewind by conversation turn without touching git history
- **+** Static single binary (CGO_ENABLED=0), cross-compiled to six targets
- **−** Rewind covers only files its edit tools changed, not shell command effects
- **−** 2.x line is still moving quickly; 1.x is the stable branch
- **−** VS Code extension requires installing the 1.x CLI separately
- **−** Model provider receives what the agent reads; no local model setup documented

<sub>no GPU · Needs Model provider API key, Go 1.25+ (build from source), Node 24+ and pnpm 10 (build Studio) · Models: DeepSeek, OpenAI-compatible endpoints, MCP servers · [Repo](https://github.com/esengine/deepseek-reasonix) · [📖 Docs ↗](https://github.com/esengine/DeepSeek-Reasonix/blob/studio/docs/GUIDE.md) · [🌐 Site ↗](https://esengine.github.io/DeepSeek-Reasonix/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepseek-reasonix/)</sub>

<a name="orca"></a>
### #&#8288;11 [orca](https://github.com/stablyai/orca) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 97k · MIT · Oct 2026</sub>

**Desktop app that runs CLI coding agents in parallel git worktrees.**

Orca is a desktop app for macOS, Windows and Linux that runs CLI coding agents such as Claude Code, Codex and OpenCode side by side, each in its own git worktree. It bundles terminal splits, a VS Code-style editor, an embedded browser, GitHub and Linear task views, diff annotation and SSH remote worktrees. A mobile companion app and an `orca` CLI let you monitor and script agents.

- **+** Works with any agent that runs in a terminal; dozens are listed
- **+** Each task gets an isolated git worktree, so parallel runs do not collide
- **+** Runs agents on remote machines over SSH with auto-reconnect and port forwarding
- **+** MIT licensed, with builds for macOS, Windows and Linux plus Homebrew and AUR installs
- **−** Does not include an agent or model; you install and sign in to CLI agents yourself
- **−** Desktop app only; no web or server deployment is described
- **−** Collects anonymous usage telemetry; opt-out is documented separately
- **−** README says features ship daily and its list lags, so behavior changes quickly

<sub>no GPU · Needs git, CLI coding agents (Claude Code, Codex, OpenCode, etc.) · Models: Claude Code, Codex, OpenCode, Pi, Cursor · [Repo](https://github.com/stablyai/orca) · [📖 Docs ↗](https://www.onorca.dev/docs/cli/overview) · [🌐 Site ↗](https://onorca.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orca/)</sub>

<a name="openinterpreter"></a>
### #&#8288;12 [openinterpreter](https://github.com/openinterpreter/openinterpreter) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 69k · Apache-2.0 · Oct 2026</sub>

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

<a name="t3code"></a>
### #&#8288;13 [t3code](https://github.com/pingdotgg/t3code) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (89) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<a name="gemini-cli"></a>
### #&#8288;14 [gemini-cli](https://github.com/google-gemini/gemini-cli) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 107k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent that runs Gemini models with file, shell and MCP tools.**

Gemini CLI is a TypeScript terminal agent, installed from npm, Homebrew, MacPorts or conda, that sends prompts to Gemini models and can edit files, run shell commands, fetch web pages and ground answers with Google Search. It supports MCP servers, GEMINI.md context files, conversation checkpointing, a headless mode with JSON and stream-JSON output, and a GitHub Action for PR review and issue triage.

- **+** Free tier with Google login: 60 requests/min, 1,000 requests/day
- **+** 1M token context window with Gemini 3 models
- **+** Headless mode emits plain text, JSON or newline-delimited stream-JSON
- **+** Auth via Google login, Gemini API key or Vertex AI
- **−** Only talks to Gemini models; no other providers listed in the README
- **−** Needs a Google account, API key or Vertex AI credentials; no local models
- **−** Preview and nightly channels may contain regressions
- **−** Free-tier quotas and terms are governed by Google, not the project

<sub>no GPU · Docker · Needs Node.js, Gemini API, Google account login or Vertex AI · Models: Gemini 3, Gemini 2.5 Flash · [Repo](https://github.com/google-gemini/gemini-cli) · [📖 Docs ↗](https://geminicli.com/docs/) · [🌐 Site ↗](https://geminicli.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-cli/)</sub>

<a name="openhands"></a>
### #&#8288;15 [OpenHands](https://github.com/openhands/openhands) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 91k · MIT · Oct 2026</sub>

**Web control center for running coding agents and scheduled automations.**

Agent Canvas is a web frontend that starts conversations with coding agents and switches between multiple Agent Server backends: local, Docker, VM or OpenHands Cloud. It runs the OpenHands agent by default and can use Claude Code, Codex, Gemini CLI, Pi, OpenCode or any ACP-compatible agent. A paired Automation Server runs agents on a schedule or on webhook events, with Slack, GitHub and Linear integrations.

- **+** Works with OpenHands, Claude Code, Codex, Gemini, Pi, OpenCode or any ACP agent
- **+** One UI switches between local, remote and cloud Agent Server backends
- **+** Scheduled and webhook-triggered automations with Slack, GitHub and Linear
- **+** Option to run each conversation in its own Docker container
- **−** Marked beta in the README
- **−** Non-Docker install gives the agent full filesystem access on the host
- **−** Needs Node.js 24+ and uv for npm or source installs
- **−** Automation backend is a separate repo; internet-facing setups need manual hardening

<sub>no GPU · Docker · Needs Node.js 24+, uv, Docker (optional) · Models: Any LLM (LLM profiles), OpenHands, Claude Code, Codex, Gemini CLI · port 8000 · [Repo](https://github.com/openhands/openhands) · [📖 Docs ↗](https://docs.openhands.dev/openhands/usage/agent-canvas/backends) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openhands/)</sub>

<a name="cline"></a>
### #&#8288;16 [cline](https://github.com/cline/cline) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (80) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 71k · Apache-2.0 · Oct 2026</sub>

**Coding agent for VS Code, JetBrains, terminal and desktop.**

Cline is a coding agent that reads a project, edits files across it, and runs shell commands while watching the output. It ships as a VS Code extension, JetBrains plugin, CLI with headless mode, macOS/Windows desktop app, and a Node.js SDK. Edits and commands need approval by default, with Plan and Act modes, checkpoints, and optional auto-approve.

- **+** Same agent engine across VS Code, JetBrains, CLI, desktop app and SDK
- **+** Works with Anthropic, OpenAI, Gemini, Bedrock, Vertex, OpenRouter, Ollama and LM Studio
- **+** Headless CLI accepts piped input and emits JSON for CI/CD scripts
- **+** Supports MCP servers, SDK plugins, cron-scheduled agents and multi-agent teams
- **−** JetBrains plugin source is not open-sourced
- **−** VS Code extension code is still migrating to the new layout
- **−** Hosted model providers need your own API keys; local models via Ollama or LM Studio
- **−** Diff review and checkpoints are described only for VS Code and JetBrains

<sub>Needs Node.js, VS Code or JetBrains IDE (for extensions), LLM provider API key or local model server · Models: Anthropic, OpenAI, Google Gemini, OpenRouter, Vercel AI Gateway · [Repo](https://github.com/cline/cline) · [📖 Docs ↗](https://docs.cline.bot) · [🌐 Site ↗](https://cline.bot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cline/)</sub>

<a name="cmux"></a>
### #&#8288;17 [cmux](https://github.com/manaflow-ai/cmux) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Oct 2026</sub>

**Native macOS terminal with vertical tabs and agent notifications.**

cmux is a Swift/AppKit macOS terminal built on libghostty that reads your existing Ghostty config. It adds a sidebar showing git branch, PR status, working directory and ports per workspace, plus notification rings driven by OSC 9/99/777 sequences or `cmux notify` from agent hooks. It also has an in-app scriptable browser, SSH workspaces, and a CLI and Unix socket API.

- **+** Native Swift/AppKit app, not Electron; libghostty rendering and reads existing Ghostty config
- **+** Works with any agent that runs in a terminal; hooks for Claude Code, Codex, OpenCode and others
- **+** Everything scriptable through CLI and Unix socket, including browser automation and split panes
- **+** Session restore of layout, scrollback and supported agent sessions via `cmux hooks setup`
- **−** macOS only; no Linux or Windows build
- **−** License detected as NOASSERTION; README says GPL, so check terms
- **−** Does not checkpoint live processes; needs opt-in tmux or zellij for detach/reattach
- **−** iOS companion is beta, with early access tied to the Founders Edition

<sub>Needs libghostty, Sparkle (auto-update) · Models: Claude Code, Codex, OpenCode, Gemini CLI, Amp · [Repo](https://github.com/manaflow-ai/cmux) · [▶️ Demo ↗](https://www.youtube.com/watch?v=i-WxO5YUTOs) · [📖 Docs ↗](https://cmux.com/docs/getting-started) · [🌐 Site ↗](https://cmux.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cmux/)</sub>

<a name="paseo"></a>
### #&#8288;18 [paseo](https://github.com/getpaseo/paseo) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · custom license · Oct 2026</sub>

**Desktop, mobile and CLI client that runs many coding agents in parallel worktrees.**

Paseo runs a local daemon that manages Claude Code, Codex, Copilot, OpenCode, Pi, Antigravity and Muse Code agents, with Electron desktop, Expo mobile/web and CLI clients connecting to it. Each agent can run in its own git worktree, with an editor, terminals, diffs, pull requests and a built-in browser in one window. It also has a plugin system, a TypeScript SDK and orchestration skills.

- **+** One interface across seven agent CLIs, switchable per task
- **+** Per-agent git worktrees allow parallel runs on one or several machines
- **+** Same app on iOS, Android, desktop, web and CLI, plus a TypeScript SDK
- **+** No telemetry, tracking or forced log-in stated
- **−** Requires at least one agent CLI installed and configured with your own credentials
- **−** Plugins run with access to the daemon machine; trust is on the user
- **−** Docker image needs extending with the agent CLIs you use
- **−** Maintained by a single person, per the README

<sub>no GPU · Docker + Compose · Needs Agent CLI (Claude Code, Codex, Copilot, OpenCode, Pi, Antigravity or Muse Code), Node.js/npm for CLI install, Git · Models: Claude Code, Codex, GitHub Copilot, OpenCode, Pi · port 6767 · [Repo](https://github.com/getpaseo/paseo) · [📖 Docs ↗](https://paseo.sh/docs) · [🌐 Site ↗](https://paseo.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/paseo/)</sub>

<a name="openchamber"></a>
### #&#8288;19 [OpenChamber](https://github.com/openchamber/openchamber) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Workspace for running and reviewing OpenCode agent sessions across devices.**

OpenChamber is a front end for the OpenCode CLI that starts coding-agent sessions, shows diffs, and carries work through review and merge. It ships as a desktop app, a Node.js CLI serving a web/PWA UI, a VS Code extension, and iOS/Android clients sharing the same projects and sessions. It adds multi-model runs, goal-driven sessions, scheduled prompts, and GitHub issue and PR context.

- **+** Same sessions reachable from desktop, web/PWA, VS Code, iOS and Android
- **+** Multi-run sends one task to up to five models, each optionally in its own worktree
- **+** Remote access via E2E-encrypted Private Relay, LAN/VPN, Cloudflare/Ngrok tunnels or SSH
- **+** Desktop build bundles the OpenCode CLI, so no separate install is needed
- **−** CLI/Web and VS Code require a separately installed OpenCode CLI
- **−** Agent runtime is tied to OpenCode; no other agent backends are listed
- **−** CLI requires Node.js 24.14 or newer
- **−** Feature changes must go through an Ideas discussion before a PR

<sub>no GPU · Docker + Compose · Needs OpenCode CLI, Node.js 24.14+ · Models: Providers configured in OpenCode · [Repo](https://github.com/openchamber/openchamber) · [📖 Docs ↗](https://github.com/openchamber/openchamber/blob/main/packages/docs/content/docs/quickstart.mdx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openchamber/)</sub>

<a name="superplane"></a>
### #&#8288;20 [superplane](https://github.com/superplanehq/superplane) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · custom license · Oct 2026</sub>

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

<a name="oh-my-pi"></a>
### #&#8288;21 [oh-my-pi](https://github.com/can1357/oh-my-pi) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (83) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Bun >= 1.3.14 (or prebuilt binary), LLM provider API access, Language servers and debug adapters optional · Models: 60+ providers, OpenAI Codex, Gemini, Grok, MiniMax · safety checks passed 14 of 17 · [Repo](https://github.com/can1357/oh-my-pi) · [📖 Docs ↗](https://github.com/can1357/oh-my-pi/blob/main/docs/lsp-config.md) · [🌐 Site ↗](https://omp.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-pi/)</sub>

<a name="openclaude"></a>
### #&#8288;22 [openclaude](https://github.com/twigpine/openclaude) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (89) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Oct 2026</sub>

**Terminal coding-agent CLI that works with cloud and local LLM providers.**

OpenClaude is a Node.js terminal coding agent with bash, file edit, grep, glob, sub-agent, task, MCP and web tools. It connects to OpenAI-compatible APIs, Gemini, GitHub Models, Codex, Ollama, Atomic Chat and many gateways, with provider profiles saved through `/provider`. It also supports background sessions, session resume and fork, and a bundled VS Code extension.

- **+** Many providers behind one CLI, including local Ollama and Atomic Chat
- **+** Guided `/provider` setup with saved profiles; also configurable via env vars
- **+** Background sessions via `--bg`, with ps, logs and kill commands
- **+** Resume and fork conversations; bundled VS Code extension
- **−** License not clearly detected: badge says MIT, detected value is NOASSERTION
- **−** `openclaude attach` does not yet reattach a background session terminal
- **−** Does not read ~/.claude config, so Claude Code settings need manual migration
- **−** Requires Node.js 22 or newer for npm installs

<sub>GPU optional · Docker · Needs Node.js >=22, ripgrep, LLM provider API key or local Ollama · Models: OpenAI-compatible, Gemini, GitHub Models, Codex, Ollama · [Repo](https://github.com/twigpine/openclaude) · [🌐 Site ↗](https://twigpine.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openclaude/)</sub>

<a name="prime-agent"></a>
### #&#8288;23 [prime-agent](https://github.com/primeintellect-ai/prime-agent) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Oct 2026</sub>

**Terminal coding and research agent built around a persistent Python REPL.**

Prime Agent is a Rust-based terminal agent for coding and long-running research work. The model acts through a persistent Python REPL, where subagents are spawned with `rlm.spawn(...)`, and `/refine` stores small, reviewable updates to prompts, memories and skills. Sessions run under a background daemon, so they survive terminal disconnects and can be reattached.

- **+** Daemon-backed sessions keep running after terminal detach; reattach with `prime-agent attach`
- **+** Built-in subagents via `rlm.spawn(...)` for parallel or background work
- **+** `/refine` keeps history and snapshots with rollback, and never rewrites the base system prompt
- **+** Long-run controls: `/goal`, heartbeats, schedules, and `/autonomous` with turn, token and time budgets
- **−** Not a security sandbox: runs model-generated Python and commands with your user permissions
- **−** License detected as NOASSERTION, while the README states MIT
- **−** Installed via curl-pipe-to-shell script; no Docker or compose setup
- **−** Supported model providers are not listed; README only mentions `/login`

<sub>Needs subscription or API-key model provider · [Repo](https://github.com/primeintellect-ai/prime-agent) · [🌐 Site ↗](https://primeintellect.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/prime-agent/)</sub>

<a name="agent-orchestrator"></a>
### #&#8288;24 [agent-orchestrator](https://github.com/orchestratorinc/agent-orchestrator) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

**Desktop app that runs parallel coding agents in git worktrees with a Kanban view.**

Orchestrator.inc is a local desktop app with a background daemon that runs multiple coding agents side by side, each in its own branch and git worktree. A project-level orchestrator agent can plan work and spawn workers. A Kanban board tracks each worker's pull request, CI and review state, and can send failures or review comments back to the owning agent.

- **+** Each Git-backed worker gets its own branch and worktree, avoiding branch collisions
- **+** Supports 30+ agent harnesses, including Claude Code, Codex, Cursor, Aider, Gemini CLI and Goose
- **+** Kanban status is derived from session, PR, CI and review state
- **+** Desktop installers for macOS (arm64, Intel), Windows and Linux (AppImage, deb, rpm); no CLI needed
- **−** Desktop app only; no Docker or server deployment is documented
- **−** Worker, Chat and reviewer support differs per agent; a separate capability matrix is needed
- **−** macOS may block first launch and require right-click Open
- **−** Agent CLIs must be installed and configured separately; RAM requirements are unknown

<sub>no GPU · Needs Git, Agent CLIs (Claude Code, Codex, etc.) · Models: Claude Code, Codex, Cursor, opencode, Aider · [Repo](https://github.com/orchestratorinc/agent-orchestrator) · [📖 Docs ↗](https://docs.orchestrator.inc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-orchestrator/)</sub>

<a name="kilocode"></a>
### #&#8288;25 [kilocode](https://github.com/kilo-org/kilocode) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (89) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<a name="jcode"></a>
### #&#8288;26 [jcode](https://github.com/1jehuang/jcode) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (83) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

**Rust terminal coding agent with a shared daemon for multi-agent swarms.**

jcode is a Rust coding agent for the terminal that runs multiple sessions against one shared server. Agents in the same repo are notified when another agent edits a file they read, and they can message each other or spawn worker agents. The README reports 14 ms time to first frame and about 3.1 MB extra RAM per headless session, measured against Claude Code, Codex CLI and others.

- **+** Sessions share one daemon; README reports ~3.1 MB per added headless session vs ~164 MB for Claude Code
- **+** Swarm tool: agents in one repo get edit notifications, DMs and broadcasts, and can spawn workers
- **+** Can resume sessions from Codex, Claude Code, OpenCode and pi
- **+** Built-in browser tool via Firefox Agent Bridge; Claude and OpenAI Codex OAuth supported
- **−** Benchmarks are the author's own, run on one Linux machine, with differing versions between tables
- **−** Local embeddings raise single-session RAM from 27.8 MB to 167.1 MB
- **−** Self-dev mode is recommended only with a frontier model; weaker models can break the codebase
- **−** Browser automation needs separate Firefox Agent Bridge setup; provider list is only on the docs site

<sub>no GPU · Needs Firefox Agent Bridge (optional, for browser tool) · Models: Claude (OAuth), OpenAI Codex (OAuth), Other providers listed in docs · [Repo](https://github.com/1jehuang/jcode) · [📖 Docs ↗](https://jcode.sh/docs) · [🌐 Site ↗](https://jcode.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jcode/)</sub>

<a name="codex"></a>
### #&#8288;27 [codex](https://github.com/openai/codex) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (72) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 130k · Apache-2.0 · Oct 2026</sub>

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

<a name="crush"></a>
### #&#8288;28 [crush](https://github.com/charmbracelet/crush) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (76) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Oct 2026</sub>

**Terminal coding agent with multi-provider LLMs, LSP context and MCP support.**

Crush is a Go terminal UI coding agent that keeps per-project sessions and lets you switch LLMs mid-session without losing context. It connects to providers such as Anthropic, OpenAI, Gemini, Bedrock, Azure and OpenRouter, or to any OpenAI- or Anthropic-compatible endpoint such as Ollama. It uses LSPs for code context and MCP servers (stdio, http, sse) for extra tools, configured through a Bash-style crushrc file.

- **+** Switch models mid-session while keeping context
- **+** Runs on macOS, Linux, Windows, Android and the BSDs, with many package managers
- **+** MCP over stdio, http and sse, including a built-in OAuth flow
- **+** Config is a crushrc script run by a built-in Bash interpreter, same on every OS
- **−** License is reported as NOASSERTION, so terms need checking before use
- **−** crushrc and crush.json are trusted code; untrusted project configs can run commands
- **−** Hooks support is described as preliminary
- **−** Setup nudges toward Charm's subscription Hyper provider

<sub>no GPU · Needs LLM provider API key or local model server (e.g. Ollama), Optional LSP servers (e.g. gopls), Optional MCP servers · Models: Anthropic, OpenAI, Google Gemini, Amazon Bedrock, Azure OpenAI · [Repo](https://github.com/charmbracelet/crush) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/crush/)</sub>

<a name="qwen-code"></a>
### #&#8288;29 [qwen-code](https://github.com/qwenlm/qwen-code) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;30 [claudian](https://github.com/yishentu/claudian) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

**Obsidian plugin that runs coding agents like Claude Code in your vault.**

Claudian is an Obsidian plugin that embeds CLI coding agents (Claude Code, Codex, Grok Build, OpenCode, Pi, DeepSeek Harness) in a sidebar chat, using the vault as the working directory. Agents can read, write, edit, search and run commands on vault files. It adds inline edit with diff preview, slash commands and skills, @mentions, MCP via each CLI's config, and cross-session messaging.

- **+** Supports six agent harnesses behind one UI, with models discovered from each provider
- **+** Inline edit shows word-level diffs on selected text or at the cursor
- **+** No telemetry; network use limited to provider calls, MCP endpoints and a 127.0.0.1 listener
- **+** Agents can message, steer or start other sessions on any provider
- **−** Requires at least one separately installed agent CLI plus a subscription or API provider
- **−** Desktop only; needs Obsidian 1.13.0 or newer
- **−** Pull requests that add new providers are not accepted
- **−** CLI detection can fail when Obsidian is launched from the Dock; needs PATH or env workarounds

<sub>no GPU · Needs Obsidian 1.13.0+, Claude Code, Codex, Grok Build, OpenCode, Pi or DeepSeek Harness CLI, Subscription or API provider · Models: Claude Code, Codex, Grok Build, OpenCode, Pi · [Repo](https://github.com/yishentu/claudian) · [🌐 Site ↗](https://community.obsidian.md/plugins/realclaudian) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claudian/)</sub>

<a name="vibe-kanban"></a>
### #&#8288;31 [vibe-kanban](https://github.com/bloopai/vibe-kanban) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: weak (29) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

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

<a name="symphony"></a>
### #&#8288;32 [symphony](https://github.com/openai/symphony) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (78) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

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

<a name="avante-nvim"></a>
### #&#8288;33 [avante.nvim](https://github.com/avante-corp/avante.nvim) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

**Neovim plugin that adds Cursor-style AI chat and code edits inside the editor.**

avante.nvim is a Lua Neovim plugin with a Rust-built component. It opens a chat sidebar that answers questions about the current file and applies suggested changes to source files. It supports an agentic mode with tools, ACP agents such as codex and gemini, and many model providers. A per-project avante.md file supplies instructions.

- **+** Runs inside Neovim; suggested changes can be applied to files with one command
- **+** Supports many providers: openai, anthropic, mistral, deepseek, ollama, llama-cpp, copilot
- **+** ACP support lets external agents like codex and gemini drive edits
- **+** Project-level avante.md instructions file; optional local RAG service
- **−** Requires Neovim 0.11+ (badge says 0.12+); README is inconsistent on version
- **−** Install needs a build step: make with curl and tar, or cargo to build from source
- **−** Auto-suggestions are marked experimental and costly because of high request frequency
- **−** Tool permissions are auto-approved by default (auto_approve_tool_permissions = true)

<sub>no GPU · Needs Neovim 0.11+, plenary.nvim, nui.nvim, mega.cmdparse, curl and tar, or cargo, provider API key or local model server · Models: claude, openai, azure, gemini, cohere · [Repo](https://github.com/avante-corp/avante.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/avante-nvim/)</sub>

<a name="claurst"></a>
### #&#8288;34 [claurst](https://github.com/kuberwastaken/claurst) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · GPL-3.0 · Oct 2026</sub>

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

<a name="pi-desktop"></a>
### #&#8288;35 [pi-desktop](https://github.com/vastsa/pi-desktop) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (93) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · LGPL-3.0 · Oct 2026</sub>

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

<a name="omnigent"></a>
### #&#8288;36 [omnigent](https://github.com/omnigent-ai/omnigent) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

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

<a name="terax-ai"></a>
### #&#8288;37 [terax-ai](https://github.com/crynta/terax-ai) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (75) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · Apache-2.0 · Oct 2026</sub>

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

<a name="emdash"></a>
### #&#8288;38 [emdash](https://github.com/generalaction/emdash) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="chat-on-steroids"></a>
### #&#8288;39 [chat-on-steroids](https://github.com/totec448-spec/chat-on-steroids) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Oct 2026</sub>

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

<a name="mimo-code"></a>
### #&#8288;40 [mimo-code](https://github.com/xiaomimimo/mimo-code) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

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

<a name="atlas"></a>
### #&#8288;41 [atlas](https://github.com/pacifio/atlas) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (50) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="forgecode"></a>
### #&#8288;42 [forgecode](https://github.com/tailcallhq/forgecode) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (93) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="gh-aw"></a>
### #&#8288;43 [gh-aw](https://github.com/github/gh-aw) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="dsh-tui"></a>
### #&#8288;44 [dsh-tui](https://github.com/ccch1mneyyy/dsh-tui) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (94) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · MIT · Oct 2026</sub>

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

<a name="deepcode"></a>
### #&#8288;45 [deepcode](https://github.com/hkuds/deepcode) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

**Coding agent with TUI, Desktop and Web clients over one local service.**

DeepCode is a coding agent that works in your repository from a terminal UI, a native desktop app or a browser workbench, all connected to one shared local background service. Projects, sessions, models, skills, permissions, goals and automations are shared across clients. It also includes a Paper2Code pipeline that turns research papers into code. Models are user-configured, with provider templates including Opper and Amazon Bedrock.

- **+** Three clients (TUI, Desktop, Web) share sessions and approvals through one local service
- **+** Sandboxed commands, with opt-in egress limits, command screening and OS keychain key storage
- **+** Goal loops, parallel agents, reusable skills, MCP support and automations are built in
- **+** Bring your own cloud or local model, with per-session context caps and /compact
- **−** No Docker or compose files detected; install is through a Python runtime
- **−** Requires Python 3.12 or newer
- **−** Frequent releases with behavior changes across TUI, Desktop and Web
- **−** RAM and hardware requirements are not stated in the README excerpt

<sub>no GPU · Needs Python 3.12+, LLM provider or local model server · Models: Amazon Bedrock, Opper, DeepSeek V4, GLM-5.2, custom model servers · port 3081 · [Repo](https://github.com/hkuds/deepcode) · [🌐 Site ↗](https://hkuds.github.io/DeepCode/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepcode/)</sub>

<a name="kimi-code"></a>
### #&#8288;46 [kimi-code](https://github.com/moonshotai/kimi-code) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · MIT · Oct 2026</sub>

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

<a name="codecompanion-nvim"></a>
### #&#8288;47 [codecompanion.nvim](https://github.com/olimorris/codecompanion.nvim) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (100) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="kirocrew"></a>
### #&#8288;48 [kirocrew](https://github.com/kirodotdev/kirocrew) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="happy"></a>
### #&#8288;49 [happy](https://github.com/slopus/happy) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<a name="claudecodeui"></a>
### #&#8288;50 [claudecodeui](https://github.com/siteboon/claudecodeui) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · AGPL-3.0 · Oct 2026</sub>

**Web and mobile UI for Claude Code, Cursor CLI and Codex sessions.**

Runs a local Node.js server (default port 3001) that gives a browser front end to Claude Code, Cursor CLI and Codex. It auto-discovers existing sessions from ~/.claude and adds chat, a shell terminal, a file explorer with editing, and a Git view for staging, committing and switching branches. MCP settings are read from and written to the same Claude Code config, and a plugin system adds custom tabs.

- **+** Auto-discovers existing sessions and shares MCP and permission config with native Claude Code
- **+** Covers three agent CLIs: Claude Code, Cursor CLI and Codex
- **+** Built-in file editor, Git explorer and shell terminal alongside chat
- **+** Plugin system with a starter template for adding tabs and backend services
- **−** AGPL-3.0: modified versions run as a network service must publish source
- **−** Requires your own Claude, Cursor or Codex subscription; it supplies no models
- **−** Self-hosted host machine must stay on; team sharing is only in paid CloudCLI Cloud
- **−** Docker sandbox mode is experimental and supports only Claude Code and Codex

<sub>no GPU · Docker · Needs Node.js 22+, Claude Code, Cursor CLI or Codex CLI, sbx CLI (sandbox mode only) · Models: Claude, GPT · port 3001 · [Repo](https://github.com/siteboon/claudecodeui) · [📖 Docs ↗](https://cloudcli.ai/docs) · [🌐 Site ↗](https://cloudcli.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claudecodeui/)</sub>

<a name="openrig"></a>
### #&#8288;51 [openrig](https://github.com/mvschwarz/openrig) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (89) · Easy to run: easy (50) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="bb"></a>
### #&#8288;52 [bb](https://github.com/get-bb/bb) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

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

<a name="gptme"></a>
### #&#8288;53 [gptme](https://github.com/gptme/gptme) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (100) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

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

<a name="screenshot-to-code"></a>
### #&#8288;54 [screenshot-to-code](https://github.com/abi/screenshot-to-code) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: patchy (33) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 80k · MIT · Oct 2026</sub>

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

<a name="warp"></a>
### #&#8288;55 [warp](https://github.com/warpdotdev/warp) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: patchy (45) · Easy to run: some setup (33) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · AGPL-3.0 · Oct 2026</sub>

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
### #&#8288;56 [munder-difflin](https://github.com/harnessmd/munder-difflin) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (46) · Freshness: active (100) · Maintenance: fair (78) · Easy to run: easy (50) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · MIT · Oct 2026</sub>

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

<a name="codepilot"></a>
### #&#8288;57 [codepilot](https://github.com/op7418/codepilot) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · custom license · Sep 2026</sub>

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

<a name="hapi"></a>
### #&#8288;58 [hapi](https://github.com/tiann/hapi) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · AGPL-3.0 · Oct 2026</sub>

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

<a name="codeg"></a>
### #&#8288;59 [codeg](https://github.com/spacering-net/codeg) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;60 [maestro](https://github.com/runmaestro/maestro) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · AGPL-3.0 · Oct 2026</sub>

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

<a name="openevolve"></a>
### #&#8288;61 [openevolve](https://github.com/algorithmicsuperintelligence/openevolve) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (74) · Easy to run: easy (50) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="agent-of-empires"></a>
### #&#8288;62 [agent-of-empires](https://github.com/agent-of-empires/agent-of-empires) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="code-graph-rag"></a>
### #&#8288;63 [code-graph-rag](https://github.com/vitali87/code-graph-rag) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Oct 2026</sub>

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

<a name="mistral-vibe"></a>
### #&#8288;64 [mistral-vibe](https://github.com/mistralai/mistral-vibe) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (78) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · Apache-2.0 · Oct 2026</sub>

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

<a name="background-agents"></a>
### #&#8288;65 [Background Agents](https://github.com/colemurray/background-agents) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (53) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Background coding agents on cloud sandboxes with Slack, GitHub and Linear triggers.**

Runs coding sessions in cloud sandboxes coordinated by a Cloudflare Workers control plane, driven from a web UI, Slack, GitHub PR comments, Linear issues or webhooks. Sessions use OpenCode or the Claude Agent harness with Anthropic, OpenAI, xAI, DeepSeek or Z.AI models, with multiplayer editing, commit attribution, child sessions and cron or event automations. For single-tenant engineering orgs.

- **+** Snapshot restore, prebuilt images and proactive warming for fast session starts
- **+** Automations from cron, Sentry alerts, GitHub workflow runs and inbound webhooks
- **+** Secrets encrypted with AES-256-GCM and scoped globally, per repo or per environment
- **+** Browser automation, code-server and a web terminal inside each sandbox
- **−** Single-tenant only; all users must be trusted members of one organization
- **−** Control plane requires Cloudflare Workers, Durable Objects and D1
- **−** Sandboxes run on third-party providers (Modal, Daytona, E2B, OpenComputer, Vercel)
- **−** Cached credentials can persist in snapshots; grant removal does not revoke tokens

<sub>no GPU · Compose · Needs Cloudflare Workers, Durable Objects and D1, Sandbox provider (Modal, Daytona, E2B, OpenComputer or Vercel Sandbox), GitHub App, Slack and Linear apps (optional) · Models: Anthropic Claude (API key or subscription), OpenAI Codex via ChatGPT subscription, xAI Grok via SuperGrok, OpenCode Zen and Go, Z.AI Coding Plan · [Repo](https://github.com/colemurray/background-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/background-agents/)</sub>

<a name="onlook"></a>
### #&#8288;66 [Onlook](https://github.com/onlook-dev/onlook) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (72) · Freshness: recent (77) · Maintenance: weak (12) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Jul 2026</sub>

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

<a name="gastown"></a>
### #&#8288;67 [gastown](https://github.com/gastownhall/gastown) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: weak (29) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Jul 2026</sub>

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

<a name="zcode"></a>
### #&#8288;68 [zcode](https://github.com/zai-org/zcode) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (51) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="grok-build"></a>
### #&#8288;69 [grok-build](https://github.com/xai-org/grok-build) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (50) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Sep 2026</sub>

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

<a name="ralph-claude-code"></a>
### #&#8288;70 [ralph-claude-code](https://github.com/frankbria/ralph-claude-code) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: fair (53) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · MIT · Oct 2026</sub>

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
### #&#8288;71 [claude-code-action](https://github.com/anthropics/claude-code-action) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (49) · Freshness: active (80) · Maintenance: fair (75) · Easy to run: some setup (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · MIT · Oct 2026</sub>

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

<a name="claude-squad"></a>
### #&#8288;72 [claude-squad](https://github.com/smtg-ai/claude-squad) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (45) · Freshness: active (100) · Maintenance: patchy (48) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · AGPL-3.0 · Aug 2026</sub>

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

<a name="jetbrains-cc-gui"></a>
### #&#8288;73 [jetbrains-cc-gui](https://github.com/zhukunpenglinyutong/jetbrains-cc-gui) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (79) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Oct 2026</sub>

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

<a name="claude-codex-bridge"></a>
### #&#8288;74 [claude_codex_bridge](https://github.com/seemseam/claude_codex_bridge) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (82) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · custom license · Oct 2026</sub>

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

<a name="continue"></a>
### #&#8288;75 [continue](https://github.com/continuedev/continue) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: weak (22) · Easy to run: some setup (33) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Jul 2026</sub>

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

<a name="omnirush-gui"></a>
### #&#8288;76 [omnirush-gui](https://github.com/omnirush-ai/omnirush-gui) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (67) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · custom license · Oct 2026</sub>

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

<a name="mini-swe-agent"></a>
### #&#8288;77 [mini-swe-agent](https://github.com/swe-agent/mini-swe-agent) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (46) · Freshness: active (100) · Maintenance: patchy (41) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · MIT · Sep 2026</sub>

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

<a name="tabby"></a>
### #&#8288;78 [Tabby](https://github.com/tabbyml/tabby) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (81) · Freshness: active (87) · Maintenance: weak (11) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Jun 2026</sub>

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

<a name="anus"></a>
### #&#8288;79 [anus](https://github.com/anus-dev/anus) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (67) · Easy to run: some setup (33) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

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

<a name="container-use"></a>
### #&#8288;80 [container-use](https://github.com/dagger/container-use) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (19) · Freshness: recent (80) · Maintenance: fair (54) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Aug 2026</sub>

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

<a name="opcode"></a>
### #&#8288;81 [opcode](https://github.com/winfunc/opcode) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (69) · Freshness: active (81) · Maintenance: weak (18) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · AGPL-3.0 · Sep 2026</sub>

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

<a name="m3e-canvas"></a>
### #&#8288;82 [m3e-canvas](https://github.com/lnkiai/m3e-canvas) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (62) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · MIT · Oct 2026</sub>

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

<a name="firstmate"></a>
### #&#8288;83 [firstmate](https://github.com/kunchenguid/firstmate) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (48) · Easy to run: hard (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.1k · MIT · Oct 2026</sub>

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

<a name="aider"></a>
### #&#8288;84 [aider](https://github.com/aider-ai/aider) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: widely used (88) · Freshness: recent (63) · Maintenance: weak (17) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · Apache-2.0 · May 2026</sub>

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

<a name="kode-cli"></a>
### #&#8288;85 [kode-cli](https://github.com/shareai-lab/kode-cli) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: weak (30) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Oct 2026</sub>

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

<a name="swe-agent"></a>
### #&#8288;86 [swe-agent](https://github.com/swe-agent/swe-agent) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (66) · Freshness: recent (71) · Maintenance: weak (1) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Jul 2026</sub>

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
### #&#8288;87 [grok-cli](https://github.com/superagent-ai/grok-cli) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (13) · Freshness: active (83) · Maintenance: weak (0) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · May 2026</sub>

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

<a name="trae-agent"></a>
### #&#8288;88 [trae-agent](https://github.com/bytedance/trae-agent) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (57) · Freshness: slowing (40) · Maintenance: weak (1) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Feb 2026</sub>

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

<a name="toad"></a>
### #&#8288;89 [toad](https://github.com/batrachianai/toad) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: niche (12) · Freshness: active (86) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · AGPL-3.0 · May 2026</sub>

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

<a name="copilotforxcode"></a>
### #&#8288;90 [copilotforxcode](https://github.com/intitni/copilotforxcode) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: known (44) · Freshness: recent (51) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Feb 2026</sub>

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

<a name="aiac"></a>
### #&#8288;91 [aiac](https://github.com/gofireflyio/aiac) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: niche (16) · Freshness: slowing (40) · Maintenance: weak (0) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Mar 2026</sub>

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

<a name="copilot-vim"></a>
### #&#8288;92 [copilot.vim](https://github.com/github/copilot.vim) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: popular (55) · Freshness: quiet (30) · Maintenance: weak (2) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Jan 2026</sub>

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

<a name="chatgpt-nvim"></a>
### #&#8288;93 [chatgpt.nvim](https://github.com/jackmort/chatgpt.nvim) <sub>score [18](../README.md#-how-we-rank "Score 18/100. Adoption: niche (18) · Freshness: quiet (22) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Jan 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
