# 🤖 Coding agents and assistants reviews · Best of Vibe Coding

Agents and assistants that read your repo, write code and run commands: CLIs, IDE extensions and self-hosted servers. Back to the [leaderboard](../README.md#-coding-agents-and-assistants).

<sub>🌐 Also on the web: [Coding agents and assistants on archestack.com](https://archestack.com/best-of-vibe-coding/coding-agents/), each project on its own page.</sub>

<a name="claw-code"></a>
### 🥇 [claw-code](https://github.com/ultraworkers/claw-code) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 195k · MIT · Oct 2026</sub>

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

<a name="opencode"></a>
### 🥈 [opencode](https://github.com/anomalyco/opencode) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 214k · MIT · Oct 2026</sub>

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
### 🥉 [pi](https://github.com/earendil-works/pi) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 115k · MIT · Oct 2026</sub>

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
### #&#8288;4 [oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 70k · custom license · Oct 2026</sub>

**Terminal coding agent that fans work out across many models.**

OmO is an `omo` command-line agent, built on senpi (a fork of pi), that reads a codebase, plans, and verifies each step. Typing `ulw` or `mass ulw` turns a job into a graph of parallel agents, each on a different model. Memory is kept as markdown files in a git repository, and `/login` covers Claude, ChatGPT, Kimi and GLM subscriptions.

- **+** Splits jobs across many agents and models in parallel with the `mass ulw` keyword
- **+** Memory stored as markdown in a git repo, so it is inspectable and versionable
- **+** Native binary installer with checksum verification, plus bun and npm packages
- **+** `omo setup` imports keys, MCP servers and skills from the OpenCode edition
- **−** License is SUL-1.0, not a standard OSI license; check terms before commercial use
- **−** Primary install path pipes a curl script into bash
- **−** README gives no RAM, token cost or hardware figures
- **−** Computer use is marked experimental

<sub>no GPU · Needs Model provider subscription or API keys, git (memory repository) · Models: Claude, ChatGPT, Kimi, GLM · safety checks passed 8 of 11 · [Repo](https://github.com/code-yeongyu/oh-my-openagent) · [📖 Docs ↗](https://omo.dev/docs) · [🌐 Site ↗](https://omo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-openagent/)</sub>

<a name="orca"></a>
### #&#8288;5 [orca](https://github.com/stablyai/orca) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 93k · MIT · Oct 2026</sub>

**Desktop app that runs CLI coding agents in parallel git worktrees.**

Orca is a desktop app for macOS, Windows and Linux that runs terminal-based coding agents such as Claude Code, Codex and OpenCode side by side, each in its own git worktree. It adds split terminals, an embedded browser with element picking, diff annotation, GitHub and Linear task views, SSH worktrees and a scriptable CLI. An iOS and Android companion app monitors agents and sends follow-ups.

- **+** Works with any CLI agent that runs in a terminal, with 30+ listed
- **+** Each agent gets an isolated git worktree, so parallel results can be compared
- **+** Supports remote worktrees over SSH with auto-reconnect and port forwarding
- **+** Orca CLI lets agents script worktree creation and browser actions
- **−** Does not include a model or agent; agent CLIs are installed and authenticated separately
- **−** Mobile app needs pairing with a running desktop host
- **−** Ships daily, so the README feature list lags behind the changelog
- **−** Collects anonymous usage telemetry, with an opt-out documented separately

<sub>no GPU · Needs git, CLI coding agents (Claude Code, Codex, OpenCode, etc.) · Models: Claude Code, Codex, OpenCode, Pi, Cursor · [Repo](https://github.com/stablyai/orca) · [📖 Docs ↗](https://www.onorca.dev/docs/cli/overview) · [🌐 Site ↗](https://onorca.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orca/)</sub>

<a name="openinterpreter"></a>
### #&#8288;6 [openinterpreter](https://github.com/openinterpreter/openinterpreter) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 69k · Apache-2.0 · Oct 2026</sub>

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

<a name="goose"></a>
### #&#8288;7 [goose](https://github.com/aaif-goose/goose) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 55k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;8 [herdr](https://github.com/herdrdev/herdr) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (94) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;9 [codewhale](https://github.com/codewhale-hq/codewhale) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

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
### #&#8288;10 [deepseek-reasonix](https://github.com/esengine/deepseek-reasonix) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

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

<a name="archon"></a>
### #&#8288;11 [Archon](https://github.com/coleam00/archon) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (94) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

**YAML workflow engine that runs coding agents in isolated worktrees.**

Defines development processes (plan, implement, validate, review, PR) as YAML workflows and runs them through Claude Code, Codex or Pi, each run in its own git worktree. Deterministic nodes mix with AI nodes and human approval gates; runs start from the CLI, a web console, Slack, Telegram, Discord or GitHub webhooks, with state in SQLite or PostgreSQL. For teams standardizing how agents ship code.

- **+** Every run isolated in a git worktree; parallel fixes without conflicts
- **+** Bundled sdlc pack: ship, triage, investigate, plan, deliver, review, validate, upkeep
- **+** Adapters for web, CLI, Slack, Telegram, Discord and GitHub webhooks
- **+** Telemetry documented field by field; DO_NOT_TRACK=1 or CI=true disables it
- **−** Requires Claude Code (or Codex, Pi) installed separately; binaries need CLAUDE_BIN_PATH
- **−** Anonymous telemetry is on by default
- **−** x64 quick-install binaries require AVX2; older CPUs must build from source
- **−** Workflows from v0.11.1 and earlier no longer ship and must be copied manually

<sub>no GPU · Docker + Compose · Needs Bun, Claude Code (or Codex or Pi), GitHub CLI, SQLite or PostgreSQL · Models: Claude Code, Codex, Pi · [Repo](https://github.com/coleam00/archon) · [📖 Docs ↗](https://archon.diy/docs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archon/)</sub>

<a name="gemini-cli"></a>
### #&#8288;12 [gemini-cli](https://github.com/google-gemini/gemini-cli) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 107k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;13 [OpenHands](https://github.com/openhands/openhands) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 91k · MIT · Oct 2026</sub>

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
### #&#8288;14 [cline](https://github.com/cline/cline) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (79) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 70k · Apache-2.0 · Oct 2026</sub>

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

<a name="codex"></a>
### #&#8288;15 [codex](https://github.com/openai/codex) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: fair (72) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 129k · Apache-2.0 · Oct 2026</sub>

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

<a name="cmux"></a>
### #&#8288;16 [cmux](https://github.com/manaflow-ai/cmux) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · custom license · Oct 2026</sub>

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

<a name="t3code"></a>
### #&#8288;17 [t3code](https://github.com/pingdotgg/t3code) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<a name="open-swe"></a>
### #&#8288;18 [Open SWE](https://github.com/langchain-ai/open-swe) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (100) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<a name="openclaude"></a>
### #&#8288;19 [openclaude](https://github.com/twigpine/openclaude) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Oct 2026</sub>

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

<a name="oh-my-pi"></a>
### #&#8288;20 [oh-my-pi](https://github.com/can1357/oh-my-pi) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

**Terminal coding agent with LSP, debugger, subagents and in-process tools.**

oh-my-pi (omp) is a terminal coding agent forked from Pi, written in TypeScript with a Rust core and run on Bun. It ships 31 built-in tools, including hashline content-hash edits, LSP and DAP debugger access, persistent Python/JS eval cells, parallel subagents in isolated worktrees, and in-process ripgrep and coreutils. It supports 60+ model providers and can run inside Zed over ACP.

- **+** LSP and DAP integration: renames go through the language server, debuggers can be stepped
- **+** Subagents run in isolated worktrees and return schema-validated results
- **+** In-process grep, glob and 58 coreutils; same binary on macOS, Linux and Windows
- **+** Reads existing Cursor, Cline, Codex and Copilot rule files without conversion
- **−** Benchmark gains cited come from the author's own blog post, not independent tests
- **−** Large tool surface (31 tools, 16 URL schemes) takes time to learn
- **−** Fork of Pi, so upstream changes are tracked separately
- **−** PR policy is a temporary trial and may return to vouch-only

<sub>no GPU · Docker · Needs Bun >= 1.3.14 (or prebuilt binary), LLM provider API access · Models: 60+ providers, Grok, Gemini, MiniMax, OpenAI Codex · safety checks passed 13 of 16 · [Repo](https://github.com/can1357/oh-my-pi) · [📖 Docs ↗](https://github.com/can1357/oh-my-pi/blob/main/docs/lsp-config.md) · [🌐 Site ↗](https://omp.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-pi/)</sub>

<a name="paseo"></a>
### #&#8288;21 [paseo](https://github.com/getpaseo/paseo) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · custom license · Oct 2026</sub>

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

<a name="kilocode"></a>
### #&#8288;22 [kilocode](https://github.com/kilo-org/kilocode) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<a name="symphony"></a>
### #&#8288;23 [symphony](https://github.com/openai/symphony) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

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

<a name="prime-agent"></a>
### #&#8288;24 [prime-agent](https://github.com/primeintellect-ai/prime-agent) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (98) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Oct 2026</sub>

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

<a name="crush"></a>
### #&#8288;25 [crush](https://github.com/charmbracelet/crush) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (76) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Oct 2026</sub>

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
### #&#8288;26 [qwen-code](https://github.com/qwenlm/qwen-code) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent with IDE, desktop, web and chat front ends.**

Qwen Code is a TypeScript coding agent that runs as the `qwen` CLI in your project, with subagents, MCP, hooks, plan mode, sandboxing and headless mode (`qwen -p`). It talks to OpenAI, Anthropic, Gemini and Qwen APIs, or local models via Ollama and vLLM. The same agent is exposed through VS Code, Zed and JetBrains plugins, a desktop app, an experimental `qwen serve` daemon, SDKs and chat channels.

- **+** Multi-protocol: OpenAI, Anthropic, Gemini, Qwen APIs, plus Ollama or vLLM, switchable at runtime
- **+** Many front ends: CLI, VS Code, Zed, JetBrains, desktop app, Telegram, DingTalk, WeChat, Feishu
- **+** TypeScript, Python and Java SDKs plus headless mode for CI and scripts
- **+** Apache-2.0; README lists SWE-bench Verified results across 7 versions
- **−** Web UI and `qwen serve` daemon are marked experimental
- **−** Requires Node.js 22+ for the npm install path
- **−** Benchmarks use Qwen 3.7 Max; results with other models are not reported
- **−** Default installer is a script piped to a shell, hosted on an Aliyun OSS bucket

<sub>GPU optional · Docker · Needs Node.js 22+ (npm install), LLM provider API key or local model server · Models: Qwen, OpenAI, Anthropic, Gemini, Ollama · [Repo](https://github.com/qwenlm/qwen-code) · [📖 Docs ↗](https://qwenlm.github.io/qwen-code-docs/en/users/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qwen-code/)</sub>

<a name="jcode"></a>
### #&#8288;27 [jcode](https://github.com/1jehuang/jcode) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (83) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

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

<a name="agent-orchestrator"></a>
### #&#8288;28 [agent-orchestrator](https://github.com/orchestratorinc/agent-orchestrator) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

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

<a name="openchamber"></a>
### #&#8288;29 [OpenChamber](https://github.com/openchamber/openchamber) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (97) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<a name="vibe-kanban"></a>
### #&#8288;30 [vibe-kanban](https://github.com/bloopai/vibe-kanban) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: weak (29) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

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

<a name="claudian"></a>
### #&#8288;31 [claudian](https://github.com/yishentu/claudian) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

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

<a name="warp"></a>
### #&#8288;32 [warp](https://github.com/warpdotdev/warp) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: patchy (44) · Easy to run: some setup (33) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 65k · AGPL-3.0 · Oct 2026</sub>

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

<a name="background-agents"></a>
### #&#8288;33 [Background Agents](https://github.com/colemurray/background-agents) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (53) · Easy to run: easy (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="mimo-code"></a>
### #&#8288;34 [mimo-code](https://github.com/xiaomimimo/mimo-code) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: easy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

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

<a name="happy"></a>
### #&#8288;35 [happy](https://github.com/slopus/happy) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Claude Code, Codex, Node.js and npm · Models: Claude, Codex, Grok · safety checks passed 6 of 8 · [Repo](https://github.com/slopus/happy) · [📖 Docs ↗](https://happy.engineering/welcome/) · [🌐 Site ↗](https://happy.engineering/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/happy/)</sub>

<a name="deepcode"></a>
### #&#8288;36 [deepcode](https://github.com/hkuds/deepcode) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

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

<a name="claudecodeui"></a>
### #&#8288;37 [claudecodeui](https://github.com/siteboon/claudecodeui) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · AGPL-3.0 · Oct 2026</sub>

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

<a name="continue"></a>
### #&#8288;38 [continue](https://github.com/continuedev/continue) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: patchy (36) · Easy to run: some setup (33) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Jul 2026</sub>

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
### #&#8288;39 [gastown](https://github.com/gastownhall/gastown) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (36) · Easy to run: easy (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Jul 2026</sub>

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

<a name="grok-build"></a>
### #&#8288;40 [grok-build](https://github.com/xai-org/grok-build) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (50) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Sep 2026</sub>

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

<a name="tabby"></a>
### #&#8288;41 [Tabby](https://github.com/tabbyml/tabby) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (67) · Freshness: active (89) · Maintenance: weak (12) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Jun 2026</sub>

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

<a name="opcode"></a>
### #&#8288;42 [opcode](https://github.com/winfunc/opcode) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (45) · Freshness: active (81) · Maintenance: weak (18) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · AGPL-3.0 · Sep 2026</sub>

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
### #&#8288;43 [aider](https://github.com/aider-ai/aider) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: popular (78) · Freshness: recent (65) · Maintenance: weak (18) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · Apache-2.0 · May 2026</sub>

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

<a name="swe-agent"></a>
### #&#8288;44 [swe-agent](https://github.com/swe-agent/swe-agent) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: known (39) · Freshness: recent (72) · Maintenance: weak (1) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Jul 2026</sub>

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

<a name="trae-agent"></a>
### #&#8288;45 [trae-agent](https://github.com/bytedance/trae-agent) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (25) · Freshness: slowing (41) · Maintenance: weak (1) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Feb 2026</sub>

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

<a name="copilot-vim"></a>
### #&#8288;46 [copilot.vim](https://github.com/github/copilot.vim) <sub>score [12](../README.md#-how-we-rank "Score 12/100. Adoption: niche (23) · Freshness: slowing (31) · Maintenance: weak (2) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Jan 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
