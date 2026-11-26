# 🤖 Coding agents and AI editors reviews · Best of Vibe Coding

Agents, assistants and editors that read your repo, write code and run commands, including tools that turn designs and screenshots into code. Back to the [leaderboard](../README.md#-coding-agents-and-ai-editors).

<sub>🌐 Also on the web: [Coding agents and AI editors on archestack.com](https://archestack.com/best-of-vibe-coding/coding-agents/), each project on its own page.</sub>

<a name="claw-code"></a>
### 🥇 [claw-code](https://github.com/ultraworkers/claw-code) <sub>score [97](../README.md#-how-we-rank "Score 97/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 195k · MIT · Nov 2026</sub>

**Rust CLI coding agent harness for prompts and sessions via API keys.**

Claw Code is a Rust implementation of the `claw` CLI agent harness, built from source in the `rust/` workspace. It runs one-shot prompts or interactive sessions using an API key (Anthropic, OpenAI and others), and `claw doctor` checks key, model access and tool configuration. The README says the repo is an agent-maintained exhibit and points to LazyCodex or Gajae-Code for real work.

- **+** Rust workspace builds a single `claw` binary with prompt and interactive modes
- **+** `claw doctor` validates API key, model access and tool config after build
- **+** Docs cover local OpenAI-compatible providers (Ollama, llama.cpp, vLLM) and Windows PowerShell
- **+** Mock parity harness and `cargo test --workspace` test suite
- **−** README says it is not the serious production project and points to other tools
- **−** Build from source only; `cargo install claw-code` installs a deprecated stub
- **−** Requires an API key; Claude subscription login is not supported
- **−** No ACP/Zed daemon yet; `claw acp serve` only returns status

<sub>no GPU · Docker + Compose · Needs Rust toolchain (cargo), LLM API key · Models: Anthropic API, OpenAI API, OpenAI-compatible local servers (Ollama, llama.cpp, vLLM) · [Repo](https://github.com/ultraworkers/claw-code) · [📖 Docs ↗](https://github.com/ultraworkers/claw-code/blob/main/USAGE.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claw-code/)</sub>

<a name="t3code"></a>
### 🥈 [t3code](https://github.com/pingdotgg/t3code) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 80k · MIT · Nov 2026</sub>

**Desktop, web and mobile front end for controlling local coding agent CLIs.**

T3 Code is a control surface for coding agents already installed and logged in on your machine, including Claude Code, Codex, Cursor, Grok Build, OpenCode, Antigravity and fx. A local server started with `t3` backs an Electron desktop app, a web app, and iOS and Android apps for remote access. Other agents can connect to it over MCP.

- **+** Uses existing Claude, Codex, Cursor, OpenCode and other provider logins
- **+** Clients for desktop (Electron), web, iOS and Android, with documented remote access
- **+** Installs via curl script, npx, winget, scoop, Homebrew, AUR or nixpkgs
- **+** MIT licensed, with a stated aim that users can fork it
- **−** Maintainers call it very early and say to expect bugs
- **−** Mostly not accepting contributions; large features will not be considered
- **−** Needs at least one provider CLI installed and authenticated before use
- **−** No docs site; documentation is markdown files in the repo

<sub>no GPU · Needs At least one agent CLI: Codex, Claude Code, Cursor CLI, Grok Build, OpenCode or fx, Google sign-in for Antigravity · Models: Claude Code, Codex, Cursor, Grok Build, OpenCode · [Repo](https://github.com/pingdotgg/t3code) · [▶️ Demo ↗](https://app.t3.codes) · [📖 Docs ↗](https://github.com/pingdotgg/t3code/tree/main/docs) · [🌐 Site ↗](https://t3.codes) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/t3code/)</sub>

<a name="codewhale"></a>
### 🥉 [codewhale](https://github.com/codewhale-hq/codewhale) <sub>score [95](../README.md#-how-we-rank "Score 95/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Nov 2026</sub>

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

<a name="archon"></a>
### #&#8288;4 [Archon](https://github.com/coleam00/archon) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Nov 2026</sub>

**YAML workflow engine that runs Claude Code, Codex and Pi through gated steps.**

Archon runs YAML-defined workflows as graphs of agent prompts, bash commands, scripts, loops and human approval gates. It drives Claude Code, Codex and Pi through their own CLIs and SDKs rather than being a coding agent itself. A bundled sdlc pack takes a GitHub issue through planning, implementation, review and merge, with each run in its own git worktree.

- **+** Loop nodes can end on a bash exit code, such as a test command, not the agent's judgment
- **+** Approval pauses, per-run event log, transcripts and cost stored in SQLite or PostgreSQL
- **+** Each repository run gets its own git worktree, so runs can proceed in parallel
- **+** Plugin contracts for providers, forges, chat surfaces and workflow packs, installed from GitHub
- **−** Needs an existing Claude Code or Codex install and account; it does not include a model
- **−** SDLC pack reaches GitHub through a plugin; no other code host is maintained
- **−** Sends anonymous telemetry by default; opting out requires an environment variable
- **−** Bundled SDLC queues are not bound to schedules or events by default

<sub>no GPU · Docker + Compose · Needs Claude Code, Codex or Pi, git, SQLite or PostgreSQL, GitHub (for SDLC pack) · Models: Claude Code, Codex, Pi · [Repo](https://github.com/coleam00/archon) · [📖 Docs ↗](https://archon.diy/docs/) · [🌐 Site ↗](https://archon.diy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archon/)</sub>

<a name="oh-my-openagent"></a>
### #&#8288;5 [oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 71k · custom license · Nov 2026</sub>

**Terminal coding agent with multi-model routing and git-backed memory.**

OmO is an `omo` command-line coding agent built on senpi, a fork of pi. It routes tasks to different models, signs in with Claude, ChatGPT, Kimi and GLM subscriptions, and can fan a job out into a graph of parallel agents with `mass ulw`. Memory is kept as markdown files in a git repository, and a small model nudges the main agent based on past sessions.

- **+** Native binary installer for macOS, Linux and Windows; also on npm and bun as omo-ai
- **+** Mixes frontier and cheap models, with a tuned system prompt per model
- **+** Memory stored as markdown in a git repo, so it is inspectable and versionable
- **+** `omo setup` migrates provider keys, MCP servers and skills from the OpenCode edition
- **−** Custom license (SUL-1.0), not a standard OSI license
- **−** In-app bug reports can include session transcripts and device details
- **−** Computer use is marked experimental
- **−** Install is a curl-piped shell script from a project-run domain

<sub>no GPU · Needs Model provider account or API keys · Models: Claude, ChatGPT, Kimi, GLM · safety checks passed 10 of 12 · [Repo](https://github.com/code-yeongyu/oh-my-openagent) · [📖 Docs ↗](https://omo.dev/docs) · [🌐 Site ↗](https://omo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-openagent/)</sub>

<a name="goose"></a>
### #&#8288;6 [aaif-goose/goose](https://github.com/aaif-goose/goose) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 57k · Apache-2.0 · Nov 2026</sub>

**General-purpose agent with desktop app and CLI, plus Rust agent crates.**

goose is a Rust agent for coding, research, writing and automation, available as a desktop app (macOS, Linux, Windows) and a CLI. It connects tools through MCP, talks to over 85 model providers or loads local models in-process, and can run as `goose acp` to serve as an agent backend. The same repo ships oi-kit, an alpha set of Rust crates for composing custom agents.

- **+** Desktop app and CLI share one agent, with MCP extensions for tools and data
- **+** Over 85 providers, including Anthropic, OpenAI, Gemini, OpenRouter and Bedrock
- **+** Loads local models in-process, without Ollama or a separate inference server
- **+** `goose acp` runs the agent as a subprocess backend over ACP
- **−** oi-kit is alpha; docs must be matched to the dependency version
- **−** Python and Kotlin bindings cover only providers, streaming and compaction
- **−** Full agent runtime API is Rust only
- **−** README covers two products (oi-kit and goose), which blurs the entry point

<sub>GPU optional · Docker · Needs LLM provider account or supported local model · Models: Anthropic, OpenAI, Gemini, OpenRouter, Amazon Bedrock · [Repo](https://github.com/aaif-goose/goose) · [📖 Docs ↗](https://goose-docs.ai/docs/quickstart) · [🌐 Site ↗](https://goose-docs.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goose/)</sub>

<a name="pi"></a>
### #&#8288;7 [pi](https://github.com/earendil-works/pi) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 124k · MIT · Nov 2026</sub>

**Minimal terminal coding agent extensible with skills and packages.**

Pi is a TypeScript coding agent CLI that runs in a project directory. It can be used interactively, in print or JSON mode, over RPC, or through a TypeScript SDK. Behavior is customized with extensions, skills, prompt templates and themes, shared as npm or git packages. The monorepo also ships a multi-provider LLM API, an agent runtime and a terminal UI library.

- **+** Four usage modes: interactive, print/JSON, RPC, and a TypeScript SDK
- **+** Extensions, skills, prompt templates and themes ship as npm or git packages
- **+** Installer pins dependencies; npm install works with --ignore-scripts
- **+** Reusable libraries: pi-ai multi-provider LLM API, agent core, TUI
- **−** No built-in permission system; runs with the launching user's permissions
- **−** Sub-agents and plan mode are omitted; need packages or self-built code
- **−** Sandboxing needs external setup (Gondolin, Docker or OpenShell)
- **−** Issues and PRs from new contributors are auto-closed by default

<sub>no GPU · Needs Node.js 22.19+, LLM provider subscription or API key · Models: OpenAI, Anthropic, Google · [Repo](https://github.com/earendil-works/pi) · [📖 Docs ↗](https://pi.dev/docs/latest) · [🌐 Site ↗](https://pi.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi/)</sub>

<a name="paseo"></a>
### #&#8288;8 [paseo](https://github.com/getpaseo/paseo) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · custom license · Nov 2026</sub>

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

<a name="opensre"></a>
### #&#8288;9 [opensre](https://github.com/tracer-cloud/opensre) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · Apache-2.0 · Nov 2026</sub>

**CLI agent that investigates failed CI runs and pushes fixes to the PR branch.**

OpenSRE is a Python CLI agent that reads failing CI checks and logs, correlates them with commits, deploys, logs, metrics and traces, and runs a tool-calling loop to find the cause. It separates CI-caused failures from code-caused ones, pushes a fix to the PR branch for review, and can post summaries to Slack, PagerDuty or Telegram. It runs as an interactive shell, a headless `opensre ask` command, or an embedded Python API.

- **+** Integrates with 60+ services, including Datadog, Grafana, Kubernetes, GitHub, GitLab, Jenkins and PagerDuty
- **+** Supports Anthropic, OpenAI, Gemini, Bedrock, OpenRouter, NVIDIA NIM and local Ollama models
- **+** Usable three ways: interactive REPL, headless CLI for scripts and CI, and in-process Python API
- **+** Optional masking of sensitive identifiers before external LLM calls
- **−** Labeled public alpha; APIs and integrations may change
- **−** Interactive shell requires signing in to an account and starts on a hosted model
- **−** Python API requires a source checkout
- **−** Several deployment paths are tied to AWS, Railway or Vercel; Docker Compose setup is not provided

<sub>Docker · Needs LLM provider API key (or Ollama), Git repository, Postgres (optional, for shared gateway state) · Models: Anthropic, OpenAI, OpenAI Codex, Ollama, Google Gemini · [Repo](https://github.com/tracer-cloud/opensre) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opensre/)</sub>

<a name="opencode"></a>
### #&#8288;10 [opencode](https://github.com/anomalyco/opencode) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 229k · MIT · Nov 2026</sub>

**Terminal-based AI coding agent with build and plan modes.**

OpenCode is a coding agent that runs in the terminal, with a beta desktop app, and works on your repository. It ships two built-in agents switched with Tab: a full-access build agent and a read-only plan agent that denies edits and asks before running bash. A general subagent handles multistep searches and can be called with @general.

- **+** Read-only plan agent denies file edits and asks before bash commands
- **+** Installs via curl script, npm, Homebrew, pacman, mise or Nix
- **+** Desktop app builds for macOS, Windows and Linux (.deb, .rpm, AppImage)
- **+** MIT licensed, with a release published within the last week
- **−** Desktop app is labeled beta
- **−** README gives no hardware requirements; details are deferred to the docs
- **−** Two Homebrew formulas with different update cadence can confuse installs

<sub>[Repo](https://github.com/anomalyco/opencode) · [📖 Docs ↗](https://opencode.ai/docs) · [🌐 Site ↗](https://opencode.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencode/)</sub>

<a name="craft-anything"></a>
### #&#8288;11 [craft-anything](https://github.com/storytold/craft-anything) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Nov 2026</sub>

**Rust engine that inspects a website, app or game and has an agent rebuild it.**

Craft Anything studies a target (website, desktop or mobile app, game, file) with inspection tools, then drives a coding agent such as Claude Code to build a new project. It compares the build against the original, for example pages at three screen widths, and refines it. It ships as an egui desktop app, a CLI and an MCP server exposing 320 tools. The project is early alpha.

- **+** Compares each build with the original and lists mismatches before declaring it ready
- **+** Every one of 320 tools is both a CLI command and an MCP tool
- **+** Clean room mode refuses tools that read the original's code or files
- **+** Installers for Windows, macOS, Linux and FreeBSD, plus a WebAssembly file viewer
- **−** Early alpha; other coding agents and API-key builds are not yet run live
- **−** Needs a separately installed and signed-in coding agent, Claude Code first
- **−** Clean room is a tool rule, not an OS sandbox; the agent acts as you
- **−** Dependency installs run package scripts on your machine

<sub>no GPU · Needs Rust 1.97+ (to build from source), Claude Code or another ACP coding agent, Ghidra (optional, Deep mode), fal.ai key (optional, images and 3D) · Models: Claude Code, Codex (unverified), GitHub Copilot CLI (ACP), Grok Build (ACP), Anthropic API · [Repo](https://github.com/storytold/craft-anything) · [🌐 Site ↗](https://getartcraft.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/craft-anything/)</sub>

<a name="cmux"></a>
### #&#8288;12 [cmux](https://github.com/manaflow-ai/cmux) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Nov 2026</sub>

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

<a name="agent-orchestrator"></a>
### #&#8288;13 [agent-orchestrator](https://github.com/orchestratorinc/agent-orchestrator) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

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

<a name="openchamber"></a>
### #&#8288;14 [OpenChamber](https://github.com/openchamber/openchamber) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Nov 2026</sub>

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
### #&#8288;15 [qwen-code](https://github.com/qwenlm/qwen-code) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent for Qwen and other models, with IDE and SDK front ends.**

Qwen Code is a TypeScript CLI coding agent that reads a repository, edits files and runs commands, started with `qwen` in a project directory. It works with OpenAI, Anthropic, Gemini and Qwen APIs or local models via Ollama and vLLM, switchable at runtime. It also ships VS Code, Zed and JetBrains integrations, a desktop app, SDKs, and an experimental `qwen serve` daemon with a Web UI.

- **+** Multi-protocol: OpenAI, Anthropic, Gemini and Qwen APIs, plus Ollama or vLLM
- **+** Subagents, MCP, hooks, skills, plan mode and sandbox are built in
- **+** Headless `qwen -p` mode and TypeScript, Python and Java SDKs for CI and scripts
- **+** Reachable from IDE plugins, desktop app, Telegram, DingTalk, WeChat and Feishu
- **−** npm install path requires Node.js 22+
- **−** Daemon and Web UI are experimental; daemon has no auth by default
- **−** Install script is piped to a shell from an Alibaba Cloud OSS bucket
- **−** Main version and 1.0 Preview are separate tracks with separate setup

<sub>GPU optional · Docker · Needs Node.js 22+ (npm install), Model provider API key or Qwen account, or local Ollama/vLLM · Models: Qwen, OpenAI API, Anthropic API, Gemini API, Ollama · port 4170 · [Repo](https://github.com/qwenlm/qwen-code) · [📖 Docs ↗](https://qwenlm.github.io/qwen-code-docs/en/users/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qwen-code/)</sub>

<a name="codecompanion-nvim"></a>
### #&#8288;16 [codecompanion.nvim](https://github.com/olimorris/codecompanion.nvim) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · Apache-2.0 · Nov 2026</sub>

**Neovim plugin for chatting with LLMs and ACP coding agents.**

CodeCompanion is a Lua plugin that adds a chat buffer, inline code transformations and an action palette to Neovim. It talks to hosted and local LLMs (Anthropic, OpenAI, Gemini, Copilot, Ollama and others) and to CLI agents such as Claude Code, Codex and Gemini CLI through the Agent Client Protocol. It also supports MCP servers, skills, rules files and custom prompts.

- **+** Built-in adapters for 13 LLM providers, plus a documented custom adapter API
- **+** ACP support connects Claude Code, Codex, Gemini CLI, Goose, OpenCode and others inside Neovim
- **+** Also supports MCP, skills, and rules files like CLAUDE.md and .cursor/rules
- **+** Review agent edits with comments and approve/reject; multiple chats; image and PDF input
- **−** Neovim only; no standalone or other-editor version
- **−** Requires plenary.nvim and nvim-treesitter as dependencies
- **−** Contributions accepted at the maintainer's discretion; one primary maintainer
- **−** Install and configuration live in external docs, not the README

<sub>no GPU · Docker · Needs Neovim, plenary.nvim, nvim-treesitter · Models: Anthropic, OpenAI, Azure OpenAI, Google Gemini, GitHub Copilot · [Repo](https://github.com/olimorris/codecompanion.nvim) · [📖 Docs ↗](https://codecompanion.olimorris.dev) · [🌐 Site ↗](https://codecompanion.olimorris.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codecompanion-nvim/)</sub>

<a name="herdr"></a>
### #&#8288;17 [herdr](https://github.com/herdrdev/herdr) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 53k · Apache-2.0 · Nov 2026</sub>

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

<a name="oh-my-pi"></a>
### #&#8288;18 [oh-my-pi](https://github.com/can1357/oh-my-pi) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Nov 2026</sub>

**Terminal coding agent with LSP, debugger and subagents built in.**

oh-my-pi (omp) is a terminal coding agent forked from Pi, written in TypeScript on Bun with a Rust core. It ships 31 built-in tools, including LSP operations, DAP debugger control, in-process ripgrep and bash, parallel subagents in isolated worktrees, and hashline content-hash edits. It supports 60+ model providers and runs on macOS, Linux and Windows.

- **+** LSP and DAP integration: renames via workspace/willRenameFiles, lldb, dlv and debugpy sessions
- **+** Hashline edits reject stale anchors; README reports Grok 4 Fast output tokens down 61%
- **+** In-process ripgrep, glob and bash with coreutils; runs on Windows without WSL
- **+** Reads existing Cursor, Cline, Codex and Copilot rule files without conversion
- **−** Large surface (31 tools, 16 URL schemes, memory backends) means a steep learning curve
- **−** Benchmark figures come from the maintainers' own blog post, not independent evaluation
- **−** Prebuilt binary is fetched from build.stencil.so; musl Alpine needs libstdc++ and libgcc
- **−** Collab sharing goes through a hosted relay; self-hosting it is not described

<sub>no GPU · Docker · Needs Bun >= 1.4.4 (source install), LLM provider API access · Models: 60+ providers, OpenAI Codex, Gemini, Grok, MiniMax · safety checks passed 14 of 17 · [Repo](https://github.com/can1357/oh-my-pi) · [📖 Docs ↗](https://github.com/can1357/oh-my-pi/blob/main/docs/lsp-config.md) · [🌐 Site ↗](https://omp.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-pi/)</sub>

<a name="openclaude"></a>
### #&#8288;19 [openclaude](https://github.com/twigpine/openclaude) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · custom license · Nov 2026</sub>

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

<a name="onlook"></a>
### #&#8288;20 [Onlook](https://github.com/onlook-dev/onlook) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Nov 2026</sub>

**Desktop design canvas that runs your repo and edits it via Claude Code or Codex.**

Onlook is a local-first Electron desktop app that opens a Git repository, starts its dev server, and shows the running app in frames on an infinite canvas. It ships no model of its own: requests go to a connected Claude Code or ChatGPT/Codex account, which edits the real files. It also exports artifacts as HTML, PNG, JPEG or PDF.

- **+** Works on your existing Git repo and dev server, so any web framework it can run is supported
- **+** Uses a worktree copy, so the original folder is not modified
- **+** Source build needs no Onlook account, cloud keys or .env file
- **+** Exports self-contained HTML, PNG, JPEG and PDF; MCP connectors supported
- **−** Only macOS builds are published; Windows is a waitlist and Linux has no artifact
- **−** Requires your own Claude Code or ChatGPT/Codex plan; no built-in model
- **−** Official download has usage analytics on by default
- **−** Icons, brand marks and sounds are not under Apache-2.0 and must be replaced in forks

<sub>Needs Claude Code or ChatGPT/Codex account, Git, Bun (source build) · Models: Claude Code, ChatGPT/Codex · README: alternative to v0, Replit · [Repo](https://github.com/onlook-dev/onlook) · [▶️ Demo ↗](https://onlook.com) · [🌐 Site ↗](https://onlook.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/onlook/)</sub>

<a name="prime-agent"></a>
### #&#8288;21 [prime-agent](https://github.com/primeintellect-ai/prime-agent) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · custom license · Nov 2026</sub>

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

<a name="theia"></a>
### #&#8288;22 [theia](https://github.com/eclipse-theia/theia) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · EPL-2.0 · Nov 2026</sub>

**TypeScript framework for building cloud and desktop IDEs and tools.**

Eclipse Theia is a TypeScript framework for assembling browser-based or Electron desktop IDEs and custom developer tools. It supports the VS Code extension protocol, so VS Code-style extensions can run in applications built on it. Adopters compose their own product from Theia's extension mechanisms rather than forking a ready-made editor.

- **+** Targets both browser and Electron desktop apps from one architecture
- **+** Supports the VS Code extension protocol, with a published API compatibility report
- **+** Vendor-neutral Eclipse governance; SBOM published for every release
- **+** Own extension mechanism plus VS Code-style extensions for customization
- **−** A framework to assemble, not a ready-to-use IDE; the IDE is in theia-blueprint
- **−** README does not describe any AI or agent features
- **−** Building a product needs Theia-specific extension and composition knowledge
- **−** Dual-licensed EPL-2.0 with GPL-2.0 plus Classpath Exception as secondary license

<sub>[Repo](https://github.com/eclipse-theia/theia) · [📖 Docs ↗](https://theia-ide.org/docs/) · [🌐 Site ↗](http://www.theia-ide.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/theia/)</sub>

<a name="omnigent"></a>
### #&#8288;23 [omnigent](https://github.com/omnigent-ai/omnigent) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Nov 2026</sub>

**Orchestration layer that runs multiple coding agent CLIs in shared sessions.**

Omnigent is a Python CLI and local server that wraps coding agents such as Claude Code, Codex, Cursor, OpenCode, Goose and Kiro behind one session model. Sessions can be viewed from the terminal, a web UI on port 6767, a phone or a macOS desktop app. They can mix agents, run in cloud sandboxes (Modal, E2B, Daytona, Kubernetes and others), and be governed by approval, spend and tool policies. The README marks it alpha.

- **+** Supports about 15 agent harnesses, and one session can combine several of them
- **+** Policies can require approval, cap spend or limit tools per server, agent or chat
- **+** Runs sessions in a dozen sandbox providers including Modal, E2B, Daytona and Kubernetes
- **+** Same session is available in the terminal, browser, phone and macOS desktop app
- **−** Marked alpha in the README, so interfaces may change
- **−** Native Windows is degraded: no tmux wrappers, no filesystem or network sandboxing
- **−** Needs Python 3.12+, Node 22+, uv, git and tmux; Linux also needs bubblewrap
- **−** Several harnesses need their vendor CLI installed and signed in separately

<sub>no GPU · Docker + Compose · Needs Python 3.12+, uv, git, Node.js 22+, tmux, bubblewrap (Linux) · Models: Anthropic, OpenAI, Gemini, Databricks, Bedrock · port 6767 · [Repo](https://github.com/omnigent-ai/omnigent) · [📖 Docs ↗](https://omnigent.ai/docs/interact/desktop) · [🌐 Site ↗](https://omnigent.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omnigent/)</sub>

<a name="open-swe"></a>
### #&#8288;24 [Open SWE](https://github.com/langchain-ai/open-swe) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

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

<a name="orca"></a>
### #&#8288;25 [orca](https://github.com/stablyai/orca) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 140k · MIT · Nov 2026</sub>

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

<a name="zed"></a>
### #&#8288;26 [zed](https://github.com/zed-industries/zed) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 96k · custom license · Nov 2026</sub>

**Multiplayer code editor written in Rust, from the creators of Atom.**

Zed is a native, multiplayer code editor written in Rust by the creators of Atom and Tree-sitter. It installs on macOS, Linux and Windows from a download or a package manager. The README covers installation, build guides and licensing, and does not describe AI or agent features.

- **+** Native desktop builds for macOS, Linux and Windows
- **+** Built by the authors of Atom and Tree-sitter
- **+** Multiplayer editing is a core feature
- **+** Per-OS build guides included in the repo docs
- **−** No web version; it is only tracked in a GitHub discussion
- **−** Mixed licensing: mainly GPL-3.0-or-later, Apache-2.0 where marked
- **−** Building from source needs a Rust toolchain and per-OS setup
- **−** README does not document AI or agent features

<sub>Compose · [Repo](https://github.com/zed-industries/zed) · [📖 Docs ↗](https://zed.dev/docs/installation) · [🌐 Site ↗](https://zed.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zed/)</sub>

<a name="openhands"></a>
### #&#8288;27 [OpenHands](https://github.com/openhands/openhands) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 94k · MIT · Nov 2026</sub>

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

<a name="jcode"></a>
### #&#8288;28 [jcode](https://github.com/1jehuang/jcode) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Nov 2026</sub>

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

<a name="claudian"></a>
### #&#8288;29 [claudian](https://github.com/yishentu/claudian) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

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

<a name="superplane"></a>
### #&#8288;30 [superplane](https://github.com/superplanehq/superplane) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · custom license · Nov 2026</sub>

**Turns backlog issues into verified pull requests using coding agents.**

SuperPlane coordinates coding agents, source control, CI, review and approvals in one workflow. It assesses imported GitHub issues for agent suitability, refines a plan, has an agent implement it, sends failed checks back for correction, and adds an agent review with a merge-confidence assessment before a human decides. It runs as a hosted service or self-hosted.

- **+** Same workflow guardrails apply to every run; failures go back to the agent
- **+** Workflows can wait for tool events, call an agent, or ask a person to approve
- **+** Self-hosts on one Linux VM with Docker Compose or on Kubernetes
- **+** Engine is Apache 2.0 and the model choice is yours
- **−** README names only GitHub as the connected source control
- **−** Self-hosting details live only in external docs
- **−** Detected license is NOASSERTION, so check the LICENSE file

<sub>Docker + Compose · Needs GitHub, Docker Compose or Kubernetes · [Repo](https://github.com/superplanehq/superplane) · [▶️ Demo ↗](https://app.superplane.com/) · [📖 Docs ↗](https://docs.superplane.com/) · [🌐 Site ↗](https://superplane.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superplane/)</sub>

<a name="dsh-tui"></a>
### #&#8288;31 [dsh-tui](https://github.com/ccch1mneyyy/dsh-tui) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · MIT · Nov 2026</sub>

**Terminal UI front end for DeepSeek Harness with side panels and session management.**

dsh-TUI is a TypeScript terminal UI for DeepSeek Harness (DSH), installed from npm as a plugin and started with `dsh-tui` or `dst`. It adds streaming Markdown, tool cards, todo/goal panels, a context bar, a TPS gauge, session resume and rewind, image and Mermaid rendering, and account sign-in for several providers. It also has a headless CLI (`dst -p`, `dst run --json`) and is described as moving from a mounted plugin to a standalone app. Public beta.

- **+** Uses only DSH public exports; uninstalling leaves no patches behind
- **+** Session tools: resume, fork, double-Esc rewind, /compact, /export and a session manager
- **+** Headless CLI for automation: `dst -p`, `dst run --json`, `dst session list --json`
- **+** Renders images (Kitty/Sixel), Mermaid diagrams and LaTeX in the terminal
- **−** Requires DeepSeek Harness and Node.js; not usable on its own
- **−** Labeled public beta; the plugin-to-app architecture is still changing
- **−** Primary compatibility target is DSH 0.2.2-rc.5, a release candidate
- **−** Many features depend on terminal support (graphics, notifications, cursor effects)

<sub>Needs Node.js, deepseek-harness, pnpm, DEEPSEEK_API_KEY (API-key route) · Models: DeepSeek, ChatGPT/Codex, Claude, Grok · [Repo](https://github.com/ccch1mneyyy/dsh-tui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-tui/)</sub>

<a name="cline"></a>
### #&#8288;32 [cline](https://github.com/cline/cline) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 72k · Apache-2.0 · Nov 2026</sub>

**Coding agent for VS Code, JetBrains, terminal and desktop, with any model provider.**

Cline is a coding agent that edits files across a project, runs shell commands and reads their output, and asks for approval before each change unless auto-approve is on. It ships as a VS Code extension, JetBrains plugin, CLI (`npm i -g cline`), desktop app for macOS and Windows, and a Node.js SDK (`@cline/sdk`). It works with Anthropic, OpenAI, Gemini, OpenRouter, Bedrock, Vertex, Ollama, LM Studio and OpenAI-compatible endpoints.

- **+** Plan and Act modes with per-edit approval, diffs and checkpoints to undo changes in VS Code and JetBrains
- **+** Many providers, including local models via Ollama and LM Studio and any OpenAI-compatible API
- **+** Headless CLI with JSON output for CI/CD, plus cron-scheduled agents and multi-agent teams
- **+** MCP support and an SDK plugin system for custom tools and lifecycle hooks
- **−** JetBrains plugin source is not open-sourced
- **−** Diff review and checkpoints are described only for VS Code and JetBrains, not the CLI
- **−** Spans many surfaces (CLI, desktop, SDK, IDEs), so features differ by product
- **−** Needs a model provider API key or local model; no bundled model

<sub>GPU optional · Needs Model provider API or local runtime (Ollama, LM Studio), Node.js (npm install) · Models: Anthropic, OpenAI, Google Gemini, OpenRouter, Vercel AI Gateway · [Repo](https://github.com/cline/cline) · [📖 Docs ↗](https://docs.cline.bot) · [🌐 Site ↗](https://cline.bot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cline/)</sub>

<a name="crush"></a>
### #&#8288;33 [crush](https://github.com/charmbracelet/crush) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Nov 2026</sub>

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

<a name="paradev"></a>
### #&#8288;34 [paradev](https://github.com/paradevai/paradev) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · custom license · Nov 2026</sub>

**Desktop app that runs CLI coding agents in parallel Git worktrees.**

Paradev (formerly Superset) is a desktop app that gives each task its own Git worktree, branch and terminals, so Claude Code, Codex, OpenCode, Gemini CLI or any other CLI agent can work on one repository at once. It adds a diff and pull request review pane, a per-workspace browser preview and sidebar agent status. It is not an agent itself and does not proxy model calls.

- **+** Works with any CLI agent; about 20 are listed as fully supported
- **+** Per-task worktree, branch and terminals, with ports detected per workspace
- **+** In-app diff, commit, push and PR review with checks and threads
- **+** Ships a CLI, TypeScript SDK and MCP server for scripting workspaces
- **−** macOS is the main target; Linux AppImage is experimental and Windows is unavailable
- **−** Mobile app, remote hosts and automations require the Pro plan
- **−** Worktrees do not sandbox processes or prevent merge conflicts
- **−** License is reported as NOASSERTION, so terms need checking before use

<sub>no GPU · Compose · Needs Git, gh (optional), Your own CLI agent subscriptions or API keys, Docker (source development only) · Models: Claude Code, OpenAI Codex CLI, OpenCode, Gemini CLI, Cursor Agent · [Repo](https://github.com/paradevai/paradev) · [📖 Docs ↗](https://docs.paradev.com) · [🌐 Site ↗](https://paradev.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/paradev/)</sub>

<a name="atlas"></a>
### #&#8288;35 [pacifio/atlas](https://github.com/pacifio/atlas) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · Apache-2.0 · Nov 2026</sub>

**Desktop IDE and CLI that records coding-agent sessions and links them to commits.**

Atlas is a desktop app (macOS, Windows, Linux) and a separate CLI that run Claude Code, Codex and other ACP agents, record each session to a local .atlas/sessions.db, and link sessions to the commits they produced as checkpoints. It adds shared on-device agent memory, @ mentions, and an optional team timeline where members comment on each other's sessions. It also includes an editor, terminal, git and cost dashboards.

- **+** Commit-to-session links survive amend and rebase via patch-id reconciliation
- **+** Local mode works offline with no account; secrets are scrubbed before writing to disk
- **+** Shared memory lets Claude Code and Codex see each other's context
- **+** Runs Claude Code, Codex and other ACP registry agents side by side
- **−** Session capture is off until enabled per project
- **−** Team timeline, web app and Ask Atlas need an account and cloud sync
- **−** Claude Code and Codex get most support; other registry agents still in QA
- **−** CLI supports macOS and Linux only

<sub>no GPU · Needs Claude Code, Codex or another ACP agent, SQLite (.atlas/sessions.db) · Models: Claude Code, Codex, Cursor, Copilot, OpenCode · [Repo](https://github.com/pacifio/atlas) · [📖 Docs ↗](https://docs.tryatlas.cc/) · [🌐 Site ↗](https://www.tryatlas.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/atlas/)</sub>

<a name="pi-desktop"></a>
### #&#8288;36 [vastsa/pi-desktop](https://github.com/vastsa/pi-desktop) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · LGPL-3.0 · Nov 2026</sub>

**Desktop app for running coding agents in persistent sessions, with plugins.**

PI-Desktop is a desktop app for macOS, Windows and Linux that runs coding agents on local projects. Work is organized as projects and persistent sessions, with Agent, Plan and Goal modes, plus subagents and parallel worker sessions. Plugins add tools, panels, widgets, MCP servers and background services. It is built on the pi agent runtime and connects to OpenAI, Anthropic, compatible APIs, Ollama and LM Studio.

- **+** Sessions persist across app launches, with branching, search and recovery of interrupted work
- **+** Plugin API covers agent tools, panels, floating widgets, MCP servers and services, shipped as .piplug
- **+** Imports local sessions from Claude Code, Codex, OpenCode and Pi
- **+** Local-first: no telemetry, credentials in OS keychain, requests go directly to your provider
- **−** Desktop app only; no server, web UI or Docker deployment
- **−** Depends on the pi runtime packages (pi-ai, pi-agent-core, pi-coding-agent)
- **−** Building from source needs Node 22.19+, pnpm 10+ and a Rust toolchain
- **−** Linux packages require glibc 2.35 or newer

<sub>GPU optional · Needs Node.js >=22.19 (source build), pnpm >=10 (source build), Rust toolchain (source build) · Models: OpenAI, Anthropic, OpenAI-compatible APIs, Ollama, LM Studio · [Repo](https://github.com/vastsa/pi-desktop) · [📖 Docs ↗](https://pi-docs.aiuo.net/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-desktop/)</sub>

<a name="gemini-cli"></a>
### #&#8288;37 [gemini-cli](https://github.com/google-gemini/gemini-cli) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 109k · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent for Gemini Code Assist enterprise users.**

Gemini CLI (`gemini`) is a TypeScript terminal agent that reads and edits a codebase, runs shell commands, and can be scripted with `-p` and JSON or stream-JSON output. It extends through MCP servers in `~/.gemini/settings.json`, GEMINI.md context files, custom commands and extensions. The README now scopes it to Gemini Code Assist Standard/Enterprise and legacy paid API or Vertex keys; free and Google AI Pro/Ultra users moved to Antigravity CLI.

- **+** Headless mode with json and stream-json output for scripts and CI
- **+** MCP servers, custom commands, extensions and GEMINI.md context files for customization
- **+** Three auth paths: Google login with Cloud project, Gemini API key, Vertex AI
- **+** Installs via npx, npm, Homebrew, MacPorts or conda; stable, preview and nightly channels
- **−** No free tier or Google AI Pro/Ultra access since June 18, 2026; moved to Antigravity CLI
- **−** Not tuned for the Gemini 4 series, per the README
- **−** Not suitable for benchmarking Gemini models; harness gives unrepresentative scores
- **−** Only Gemini models are documented; no other providers listed

<sub>no GPU · Docker · Needs Node.js, Google Cloud project, Gemini API key or Vertex AI credentials · Models: Gemini (e.g. gemini-2.5-flash) · [Repo](https://github.com/google-gemini/gemini-cli) · [📖 Docs ↗](https://www.geminicli.com/docs/get-started) · [🌐 Site ↗](https://geminicli.com/docs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-cli/)</sub>

<a name="kilocode"></a>
### #&#8288;38 [kilocode](https://github.com/kilo-org/kilocode) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Nov 2026</sub>

**Coding agent for VS Code, JetBrains and the terminal with 500+ models.**

Kilo Code is a coding agent that runs as a VS Code extension, a JetBrains plugin, a CLI (`kilo`) and a hosted cloud agent. It has Code, Plan, Ask and Debug agents, inline autocomplete, terminal and browser control, and a marketplace for skills, MCP servers and plugins. The CLI is a fork of OpenCode, and `kilo run --auto` supports non-interactive CI use.

- **+** Same agent in VS Code, JetBrains, CLI and a web cloud agent
- **+** Separate Code, Plan, Ask and Debug agents, plus custom agents
- **+** Model switching mid-task; provider pricing with no markup, per README
- **+** `kilo run --auto` enables unattended runs in CI pipelines
- **−** `main` accepts only bug fixes; new features go to the `v2` branch
- **−** `--auto` auto-approves permissions unless denied; only safe in trusted environments
- **−** Cloud agent and code reviews depend on a Kilo account
- **−** CLI is an OpenCode fork, so it tracks upstream changes

<sub>no GPU · Needs VS Code, JetBrains IDE or terminal, LLM provider or Kilo account · Models: 500+ models via providers, OpenAI GPT, Anthropic Claude, Google Gemini, xAI Grok · [Repo](https://github.com/kilo-org/kilocode) · [▶️ Demo ↗](https://app.kilo.ai/cloud) · [📖 Docs ↗](https://kilo.ai/docs) · [🌐 Site ↗](https://kilo.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kilocode/)</sub>

<a name="m3e-canvas"></a>
### #&#8288;39 [m3e-canvas](https://github.com/lnkiai/m3e-canvas) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**Browser sketchpad for Material 3 Expressive screens that exports an AI coding prompt.**

M3E Canvas is a static Next.js app where you drag Material 3 Expressive parts onto phone or desktop screens, link them with transitions, and preview the tap-through flow. The design is turned into a text brief in Japanese, English, Chinese or Korean, which you paste into a tool such as Claude Code, Codex, Gemini CLI or Cursor. It does not generate code itself.

- **+** Runs fully in the browser with no account or server; designs autosave locally
- **+** Screen links with slide, fade or expand transitions, playable in a preview
- **+** Share links and an agent.md let a coding agent read or write a design
- **+** Optional AI drafting uses your own key, sent directly from browser to provider
- **−** Only produces a prompt; the app code comes from a separate coding tool
- **−** Limited to Material 3 Expressive parts, so other design systems are out
- **−** Full editor targets desktop browsers; phones get a reduced buttons-only editor
- **−** No tagged releases

<sub>no GPU · Needs Node.js and npm (to build locally), Optional API key for OpenAI, Claude, Gemini or DeepSeek · Models: OpenAI, Claude, Gemini, DeepSeek · port 3000 · [Repo](https://github.com/lnkiai/m3e-canvas) · [▶️ Demo ↗](https://lnkiai.github.io/m3e-canvas/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/m3e-canvas/)</sub>

<a name="emdash"></a>
### #&#8288;40 [generalaction/emdash](https://github.com/generalaction/emdash) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · Apache-2.0 · Nov 2026</sub>

**Desktop app that runs multiple coding agents in separate Git worktrees.**

Emdash Classic is an Electron-style desktop app for macOS, Windows and Linux that launches Claude Code, Codex, OpenCode and other agent CLIs in parallel, each in its own Git worktree and branch. It can work on local repos or remote machines over SSH/SFTP, and handles diff review, PR creation, CI checks and merging. Issues from Linear, GitHub, Jira and others can be sent to an agent.

- **+** Isolates each agent in its own Git worktree and branch
- **+** Auto-detects installed agent CLIs: Claude Code, Codex, Cursor, OpenCode, Amp, Devin, Copilot and more
- **+** Local-first: app state in local SQLite, code and chats not sent to Emdash servers
- **+** Remote projects over SSH/SFTP with agent, key or password auth; credentials in OS keychain
- **−** Needs separate agent CLIs installed and configured; it does not supply models
- **−** Writes lifecycle hook entries into agents' user config files
- **−** Team and cloud use is a separate product, not this app
- **−** Telemetry is on by default and must be disabled in Settings or by env var

<sub>no GPU · Needs Git, Agent provider CLIs (Claude Code, Codex, etc.), SSH for remote projects · Models: Claude Code, Codex, Cursor, OpenCode, Amp · [Repo](https://github.com/generalaction/emdash) · [📖 Docs ↗](https://emdash.com/docs) · [🌐 Site ↗](https://emdash.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/emdash/)</sub>

<a name="chat-on-steroids"></a>
### #&#8288;41 [chat-on-steroids](https://github.com/totec448-spec/chat-on-steroids) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Nov 2026</sub>

**Desktop app that lets ChatGPT edit local files and run commands via MCP.**

Chat On Steroids is an Electron-style desktop app (Windows, macOS, Linux) that connects your ChatGPT conversation to local tools over MCP, so ChatGPT can read and edit files, run tests and keep terminals open. A browser extension for Chrome, Edge or Brave drives the ChatGPT UI. It adds parallel workers, Goal/Loop modes, per-folder permissions and ntfy or Telegram notifications. It is an unofficial beta and does not call Codex directly.

- **+** Folder-level access control: choose which folders ChatGPT may touch and what it may do
- **+** Workers run independent jobs in parallel and keep context between tasks
- **+** Telegram bot can show status, pause or stop chats, and deny approvals remotely
- **+** Installers for Windows x64, macOS Apple silicon and Linux x64 DEB
- **−** Depends on automating the ChatGPT web UI, which is not a public API
- **−** Setup needs a tunnel, restricted API key and custom MCP app in ChatGPT
- **−** Windows and macOS builds are unsigned; macOS asks for a password after each update
- **−** Requires a ChatGPT plan that allows custom MCP apps; usage limits still apply

<sub>no GPU · Needs ChatGPT account with custom MCP app support, OpenAI tunnel and restricted API key, Chrome 125+, Edge or Brave with browser extension, Secret Service keyring (Linux) · Models: ChatGPT models available to your account · [Repo](https://github.com/totec448-spec/chat-on-steroids) · [📖 Docs ↗](https://github.com/totec448-spec/chat-on-steroids/blob/main/docs/setup.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-on-steroids/)</sub>

<a name="openinterpreter"></a>
### #&#8288;42 [openinterpreter](https://github.com/openinterpreter/openinterpreter) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 69k · Apache-2.0 · Nov 2026</sub>

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

<a name="gitbutler"></a>
### #&#8288;43 [gitbutler](https://github.com/gitbutlerapp/gitbutler) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

**Git client with stacked and parallel branches, as a desktop GUI and CLI.**

GitButler is a Git-based version control client, written in Rust, that works in an existing Git repo through a desktop GUI and a `but` CLI. It adds stacked and parallel branches, drag-and-drop commit editing, an operation log with undo, and conflicts that stay inside commits. It also opens pull requests on GitHub, GitLab and Bitbucket, generates commit messages with AI, and installs hooks or skills for coding agents.

- **+** Runs in any existing Git repo without migration
- **+** Stacked branches restack automatically when you amend or edit a commit
- **+** Operation log lets you undo or revert any operation
- **+** Both GUI and `but` CLI, with agent hooks and skills
- **−** Fair Source license, not OSI open source; converts to MIT after 2 years
- **−** Non-compete clause bars building a competing product with it
- **−** AI features are secondary; it is a Git client, not a coding agent
- **−** Parallel branches differ from the standard Git workflow, adding a learning curve

<sub>no GPU · Needs Git, GitHub, GitLab or Bitbucket (optional, forge integration) · [Repo](https://github.com/gitbutlerapp/gitbutler) · [📖 Docs ↗](https://docs.gitbutler.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitbutler/)</sub>

<a name="cindy"></a>
### #&#8288;44 [cindy](https://github.com/makecindy/cindy) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Nov 2026</sub>

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

<sub>Docker · Needs Node.js 22.x, pnpm 10.x, Git LFS, Cindy cloud account (for server-backed features) · Models: Claude Code, Codex, Cindy hosted models, custom API keys, local models · [Repo](https://github.com/makecindy/cindy) · [🌐 Site ↗](https://cindy.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cindy/)</sub>

<a name="openevolve"></a>
### #&#8288;45 [openevolve](https://github.com/algorithmicsuperintelligence/openevolve) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · Apache-2.0 · Nov 2026</sub>

**Evolutionary coding agent that mutates programs with LLMs against your scoring function.**

OpenEvolve is an open-source implementation of Google DeepMind's AlphaEvolve. It asks LLMs to mutate code between EVOLVE-BLOCK markers, scores each candidate with a user-written evaluator, and keeps diverse programs using MAP-Elites and island populations. It runs from a CLI or as a Python library, and ships examples such as circle packing, Metal kernels and symbolic regression.

- **+** MAP-Elites plus island populations with migration to keep candidate programs diverse
- **+** Works with any OpenAI-compatible API, or Claude Code, GitHub Copilot and Codex CLIs
- **+** Every component is seeded, so runs can be reproduced
- **+** Many worked examples: circle packing, Rust sort, MLX kernels, prompt optimization
- **−** Requires you to write an evaluator that scores candidates; no evaluator, no evolution
- **−** Cost depends on LLM calls across many iterations; no cost figures given
- **−** Quick start needs an API key and sets OPENAI_API_KEY even for Gemini
- **−** Targets scoreable optimization problems, not general repo editing or feature work

<sub>no GPU · Docker · Needs Python 3.10+, LLM API access (OpenAI-compatible) · Models: OpenAI-compatible APIs, Google Gemini, Claude Code CLI, GitHub Copilot CLI, Codex CLI · [Repo](https://github.com/algorithmicsuperintelligence/openevolve) · [📖 Docs ↗](https://github.com/algorithmicsuperintelligence/openevolve/blob/main/docs/how-it-works.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openevolve/)</sub>

<a name="gh-aw"></a>
### #&#8288;46 [gh-aw](https://github.com/github/gh-aw) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.7k · MIT · Nov 2026</sub>

**GitHub CLI extension that compiles Markdown agent workflows into Actions.**

gh-aw is a GitHub CLI extension where a workflow is Markdown with YAML frontmatter for triggers, permissions, tools and engine. `gh aw compile` validates it and generates a `.lock.yml` GitHub Actions workflow. Agent jobs run read-only and sandboxed, and writes go through validated `safe-outputs` jobs with scoped permissions. Engines include Copilot, Claude Code, Codex, Gemini and Pi.

- **+** Compiles to standard Actions workflows, so it runs on existing GitHub infrastructure
- **+** Agent jobs are read-only and sandboxed by default; writes pass through validated safe-outputs
- **+** Supports several engines: Copilot, Claude Code, OpenAI Codex, Gemini and Pi
- **+** Workflows are plain Markdown plus YAML frontmatter, reviewable in pull requests
- **−** Tied to GitHub Actions and the gh CLI; no other CI systems mentioned
- **−** README says use at your own risk and requires careful human supervision
- **−** Security advisory retired releases >= 0.83.3 and < 0.85.4
- **−** Each engine needs its own authentication, set up separately

<sub>no GPU · Docker · Needs GitHub CLI, GitHub Actions · Models: GitHub Copilot, Claude Code, OpenAI Codex, Google Gemini, Pi · [Repo](https://github.com/github/gh-aw) · [📖 Docs ↗](https://github.github.com/gh-aw/setup/quick-start/) · [🌐 Site ↗](https://github.github.com/gh-aw/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gh-aw/)</sub>

<a name="kirocrew"></a>
### #&#8288;47 [kirocrew](https://github.com/kirodotdev/kirocrew) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · Apache-2.0 · Nov 2026</sub>

**Persistent agent workspace with scheduled tasks, memory, and Slack/Discord access.**

Kiro Crew is a Python Gateway that runs agent sessions on your own machine or a remote host, driven by kiro-cli through ACP by default. It keeps sessions, memory, schedules and task checkpoints across restarts, and runs long tasks, recurring jobs and webhook-triggered work unattended. You reach it from a desktop app, web dashboard, CLI, Slack or Discord, and extend it with MCP servers, markdown skills, hooks and installable Apps.

- **+** Sessions, memory, schedules and checkpoints persist across Gateway restarts
- **+** Runs scheduled jobs, scripts and webhook-triggered work without a terminal open
- **+** Same state reachable from desktop app, dashboard, CLI, Slack and Discord
- **+** Approvals, OS sandboxing, credential redaction and audit events; dashboard binds to loopback
- **−** Default agent needs kiro-cli installed and signed in separately
- **−** Sends a daily anonymous heartbeat by default; opt-out via setting or env var
- **−** Source build needs Python 3.12+ and Node.js 22.12+
- **−** Windows is supported only through a separate native source install guide

<sub>Docker + Compose · Needs kiro-cli, Python 3.12+, Node.js 22.12+ (source build) · Models: Kiro models via kiro-cli (ACP), Other verified ACP harnesses · port 5476 · [Repo](https://github.com/kirodotdev/kirocrew) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kirocrew/)</sub>

<a name="agent-of-empires"></a>
### #&#8288;48 [agent-of-empires](https://github.com/agent-of-empires/agent-of-empires) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · MIT · Nov 2026</sub>

**Session manager for running AI coding agents in parallel with tmux.**

Agent of Empires (aoe) is a Rust session manager for AI coding agents on Linux and macOS. Each agent runs in a persistent tmux session, or a persistent worker in the structured view, with optional git worktree and Docker, Podman or Apple Containers isolation. It offers a TUI, a web dashboard that works on phones, a CLI and an HTTP API.

- **+** Sessions survive closing the TUI, SSH disconnects and terminal crashes
- **+** Git worktrees and multi-repo workspaces for parallel agents across branches
- **+** Container sandboxing with Docker, Podman or Apple Containers
- **+** TUI, web dashboard, CLI and HTTP API; installs via Homebrew or script
- **−** Windows only through WSL2, since it depends on tmux and POSIX processes
- **−** Supported agent list is not in the README; must run `aoe agents`
- **−** Manages agent sessions but does not write code; needs separate agent CLIs
- **−** Requires tmux installed on the host

<sub>no GPU · Docker · Needs tmux, Docker (optional) · [Repo](https://github.com/agent-of-empires/agent-of-empires) · [📖 Docs ↗](https://www.agent-of-empires.com/docs/quick-start/) · [🌐 Site ↗](https://www.agent-of-empires.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-of-empires/)</sub>

<a name="aicommits"></a>
### #&#8288;49 [aicommits](https://github.com/nutlope/aicommits) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · MIT · Oct 2026</sub>

**CLI that writes git commit messages from staged diffs using an LLM.**

aicommits is a Node.js CLI that reads your staged git changes and proposes a commit message, either directly via `aicommits` or through a `prepare-commit-msg` hook. It works with API providers (Together AI, OpenAI, Anthropic, Groq, xAI, OpenRouter, custom endpoints), local Ollama or LM Studio, or an existing Claude, Codex or OpenCode Go subscription. Output formats include plain, conventional, gitmoji and body variants.

- **+** Supports many providers, including local Ollama and LM Studio and any OpenAI-compatible endpoint
- **+** Can use a logged-in Claude or Codex CLI, so no API key is needed
- **+** Git hook mode keeps the normal `git commit` flow and opens the editor
- **+** Five message formats plus locale, custom prompt and multiple-candidate options
- **−** Requires Node.js 22 or newer
- **−** Hosted providers send staged diff content to a third party
- **−** Reasoning models may need `max-output-tokens` raised or they return no message
- **−** `--generate` with several candidates uses more tokens and costs more

<sub>no GPU · Needs Node.js 22+, LLM provider API key, or logged-in claude/codex CLI, or local Ollama/LM Studio · Models: Together AI, OpenAI, Anthropic, Claude Agent, Codex · [Repo](https://github.com/nutlope/aicommits) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aicommits/)</sub>

<a name="code-graph-rag"></a>
### #&#8288;50 [code-graph-rag](https://github.com/vitali87/code-graph-rag) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Nov 2026</sub>

**CLI that indexes a codebase into a graph for natural-language queries and edits.**

Code-Graph-RAG parses a multi-language repository with Tree-sitter into a knowledge graph stored in an embedded SQLite file by default. The `cgr` CLI turns natural-language questions into Cypher queries, retrieves source, applies AST-based edits with diff preview, and finds dead code. It also runs as an MCP server, and can merge runtime call traces into the graph.

- **+** Embedded SQLite graph by default, so no database server is needed
- **+** Fully supports 14 languages under one graph schema, including mixed-language monorepos
- **+** Compiler frontends and runtime traces (`cgr trace`) add facts static parsing misses
- **+** Exposes the graph to Claude Code and other clients through an MCP server
- **−** PyPI releases ship only every 50th version, so installs lag the newest git tag
- **−** Native extension limits installs to CPython 3.12+ on Linux, macOS and Windows x64
- **−** Ruby, Kotlin, Swift and others get only structural support via ast-grep
- **−** `--clean` deletes every project in the shared graph, not just the current repo

<sub>Docker · Needs Python 3.12+, ripgrep, Memgraph (optional), Neo4j (optional), Qdrant (optional, with Memgraph stack) · [Repo](https://github.com/vitali87/code-graph-rag) · [📖 Docs ↗](https://docs.code-graph-rag.com/) · [🌐 Site ↗](https://code-graph-rag.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-graph-rag/)</sub>

<a name="vibe-kanban"></a>
### #&#8288;51 [vibe-kanban](https://github.com/bloopai/vibe-kanban) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Nov 2026</sub>

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

<a name="avante-nvim"></a>
### #&#8288;52 [avante.nvim](https://github.com/avante-corp/avante.nvim) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Nov 2026</sub>

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

<a name="claudecodeui"></a>
### #&#8288;53 [claudecodeui](https://github.com/siteboon/claudecodeui) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · AGPL-3.0 · Nov 2026</sub>

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
### #&#8288;54 [claurst](https://github.com/kuberwastaken/claurst) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · GPL-3.0 · Nov 2026</sub>

**Rust terminal coding agent with multiple model providers and a TUI.**

Claurst is a terminal coding agent written in Rust, started as a clean-room reimplementation of Claude Code's behavior. It routes to multiple providers (Anthropic API key, ChatGPT/Codex subscription login), and offers a TUI, headless mode with stream-json output, hooks, skills, plugins, and an ACP server for editors such as Zed. Version 0.2.1 is labeled Beta.

- **+** Prebuilt single binary for Linux, macOS and Windows; also installable via npm or bun
- **+** Headless mode with stream-json events, --json-schema output and --resume
- **+** Speaks Agent Client Protocol (`claurst acp`) for Zed and other editors
- **+** Reads AGENTS.md/CLAUDE.md and skills, and follows Claude Code's hooks contract
- **−** Beta (v0.2.1); README warns of rough edges in experimental features
- **−** Free Mode, /goal, /share and ultracode are flagged experimental
- **−** Seatbelt Bash sandbox is described only for macOS
- **−** GPL-3.0 license may constrain embedding in proprietary products

<sub>no GPU · Needs Anthropic API key or ChatGPT (Codex) subscription, libasound2-dev (optional, for voice build) · Models: Anthropic, ChatGPT (Codex), multi-provider (others unspecified) · [Repo](https://github.com/kuberwastaken/claurst) · [📖 Docs ↗](https://claurst.kuber.studio/docs) · [🌐 Site ↗](https://claurst.kuber.studio) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claurst/)</sub>

<a name="bb"></a>
### #&#8288;55 [bb](https://github.com/get-bb/bb) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Nov 2026</sub>

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

<a name="athas"></a>
### #&#8288;56 [athas](https://github.com/athasdev/athas) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · AGPL-3.0 · Nov 2026</sub>

**Desktop code editor with Git, LSP, vim keybindings and AI agents.**

Athas is a desktop code editor built with Tauri (Rust backend, React frontend). It bundles syntax highlighting, LSP support, Git integration, an integrated terminal, vim keybindings, database viewers and AI agents. It installs via shell script, Homebrew, APT, DNF, or prebuilt packages for macOS, Windows and Linux.

- **+** Tauri build rather than Electron, so a native webview app
- **+** Packaged for Homebrew, APT, DNF, AppImage, .deb, .rpm and a Windows install script
- **+** LSP, Git, terminal, vim keybindings and database viewers in one editor
- **+** Enterprise policy controls: managed mode and extension allowlist
- **−** AGPL-3.0, and the project may also ship under commercial terms
- **−** Contributors must agree to a Contributor License and Feedback Agreement
- **−** Building from source needs Node.js 24, Bun 1.3.14 and Rust

<sub>Needs Node.js 24 (build), Bun 1.3.14 (build), Rust (build), WebKitGTK 4.1 (Linux tar.gz) · [Repo](https://github.com/athasdev/athas) · [📖 Docs ↗](https://athas.dev/docs) · [🌐 Site ↗](https://athas.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/athas/)</sub>

<a name="deepcode"></a>
### #&#8288;57 [deepcode](https://github.com/hkuds/deepcode) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Nov 2026</sub>

**Coding agent with TUI, Desktop and Web clients over one local service.**

DeepCode is a Python coding agent that works in your repository and runs from a terminal UI, a native Desktop app or a browser workbench. All three connect to one local background service, so sessions, projects, models, skills, permissions and goals are shared. It also includes Paper2Code, which turns research papers into code, and works with cloud or local model providers.

- **+** TUI, Desktop and Web clients share sessions and running work through one local service
- **+** Sandboxed shell commands, permission controls, opt-in command screening and egress limits
- **+** Goals, skills, MCP servers, automations and parallel agents are built in
- **+** Messages are written to the session file as read, so a crash mid-turn keeps history
- **−** Requires Python 3.12+; no Docker or compose files detected
- **−** Frequent releases with behaviour changes; upgrades call for a runtime snapshot first
- **−** Background service and an awake computer are needed for detached tasks

<sub>no GPU · Needs Python 3.12+, LLM provider or local model server · Models: Cloud and local model providers, Amazon Bedrock, Opper, DeepSeek V4, GLM-5.2 · port 3081 · [Repo](https://github.com/hkuds/deepcode) · [🌐 Site ↗](https://hkuds.github.io/DeepCode/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepcode/)</sub>

<a name="openrig"></a>
### #&#8288;58 [openrig](https://github.com/mvschwarz/openrig) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.0k · Apache-2.0 · Nov 2026</sub>

**Define and run a persistent team of Claude Code and Codex agents.**

OpenRig is a CLI (`rig`) and TUI that launches and manages teams of coding agents, with Claude Code and Codex seats in the same rig, running in tmux sessions. Teams are defined in YAML and booted with `rig up`. A kernel operator agent helps pick one of three teams (starter, workshop, factory) and coordinates work across seats.

- **+** Mixes Claude Code and Codex seats in one YAML-defined team
- **+** Ships three ready teams: starter, workshop and factory
- **+** Dashboard TUI shows seats with runtime, model, context and state
- **+** Needs only one signed-in provider to start
- **−** Setup edits ~/.tmux.conf, provider configs and hooks, and may install tmux or Herdr
- **−** Kernel defaults to broad permissions, including Codex full access with no approvals
- **−** Requires macOS or Linux (WSL2 on Windows) and Node.js 22 or 24
- **−** Only Claude Code and Codex are providers; OMP setup is unverified

<sub>no GPU · Docker · Needs Node.js 22 or 24, tmux, Claude Code or Codex (signed in), Herdr (optional) · Models: Claude Code, Codex · [Repo](https://github.com/mvschwarz/openrig) · [📖 Docs ↗](https://github.com/mvschwarz/openrig/blob/main/docs/reference/quickstart.md) · [🌐 Site ↗](https://openrig.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openrig/)</sub>

<a name="zcode"></a>
### #&#8288;59 [zcode](https://github.com/zai-org/zcode) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · Apache-2.0 · Nov 2026</sub>

**AI coding workbench with desktop app, browser UI and terminal agent.**

ZCode is a TypeScript monorepo with an Electron desktop client, a web client, an HTTP/WebSocket backend and an agent CLI with a TUI. The `zcode` command opens the TUI by default or serves the web UI with `--web`, bound to 127.0.0.1. Remote workspaces over SSH/WSL and a UI plugin system are included.

- **+** One agent backend serves desktop, browser and terminal front ends
- **+** Web mode binds to localhost and generates an access token on non-local hosts
- **+** Supports remote projects over SSH and WSL
- **+** Active releases: v3.18.1 on 2026-11-12
- **−** README is written in Chinese; English version is a separate file
- **−** Building the CLI package requires setting a download base URL
- **−** Pinned to Node.js 24.14.0 and pnpm 10.33.2
- **−** Local desktop builds are unsigned; macOS needs a quarantine workaround

<sub>no GPU · Docker · Needs Node.js 24.14.0, pnpm 10.33.2, Git · port 3030 · [Repo](https://github.com/zai-org/zcode) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zcode/)</sub>

<a name="codex"></a>
### #&#8288;60 [codex](https://github.com/openai/codex) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 137k · Apache-2.0 · Nov 2026</sub>

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

<a name="happy"></a>
### #&#8288;61 [happy](https://github.com/slopus/happy) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Nov 2026</sub>

**Mobile app and CLI for running Claude Code and Codex from your phone.**

Happy wraps the Claude Code and Codex harnesses in a terminal CLI (`npm install -g happy`, then `happy claude` or `happy codex`) and syncs sessions to native iOS, Android and web apps through an encrypted relay server. This repo holds the mobile apps, the original CLI, the relay server and a Cloudflare Worker for APNs/FCM push. The desktop app and multi-model harness live in separate repositories.

- **+** Continue a running Claude Code or Codex session from a phone
- **+** Device sync is end-to-end encrypted through a relay server
- **+** Native Swift iOS and Kotlin Android apps, plus a web build
- **+** MIT licensed, with relay server and push worker included
- **−** Original CLI covers only Claude Code and Codex
- **−** Multi-model sessions need the separate desktop app and agent runtime
- **−** Monorepo mixes Swift, Kotlin and TypeScript packages, which raises the cost of forking
- **−** Push delivery depends on a Cloudflare Worker you must deploy yourself

<sub>no GPU · Docker · Needs Node.js/npm, Claude Code or Codex, Cloudflare Workers (push server) · Models: Claude, Codex · safety checks passed 1 of 2 · [Repo](https://github.com/slopus/happy) · [📖 Docs ↗](https://happy.engineering/welcome/) · [🌐 Site ↗](https://happy.engineering/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/happy/)</sub>

<a name="claude-cage"></a>
### #&#8288;62 [claude-cage](https://github.com/lee-xeo/claude-cage) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.7k · MIT · Nov 2026</sub>

**Desktop app that runs Claude Code in an isolated VM behind your own proxy.**

Claude Cage is a Go desktop app that creates a macOS, Windows or Linux guest VM (via Lima) with its own network, timezone and language settings. It routes all guest traffic through a built-in Mihomo proxy and pauses outbound access when its network and isolation checks fail. Terminal, browser, editor and Claude Desktop sit in one workbench, with optional SSH VPS deployment, multi-account quota tracking and phone pairing.

- **+** No direct-connection fallback: guest goes offline if the proxy or critical checks fail
- **+** Guest OS choice: macOS, Windows or Linux VM, or a remote Linux VPS over SSH without KVM
- **+** Installer bundles the proxy core; no Go, Node.js, Docker or Clash needed
- **+** Shares only the default workspace and folders you open; host Claude login and SSH keys stay out
- **−** Supports only Apple Silicon Macs, Windows x64 and Debian/Ubuntu x86_64; no Intel Mac or ARM64 Windows/Linux
- **−** Projects share one guest's tools, accounts and filesystem; no per-project isolation
- **−** Needs your own proxy node; public UDP, IPv6 and ICMP are restricted
- **−** Docs are mainly Chinese; checks cannot guarantee against account restrictions

<sub>Docker + Compose · Needs Lima, Mihomo (bundled), Clash/Mihomo YAML proxy subscription, uv (source builds only) · Models: Claude (via Claude Code) · [Repo](https://github.com/lee-xeo/claude-cage) · [📖 Docs ↗](https://claude-cage.com/docs/) · [🌐 Site ↗](https://claude-cage.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-cage/)</sub>

<a name="thinkrail"></a>
### #&#8288;63 [thinkrail](https://github.com/jetbrains/thinkrail) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Nov 2026</sub>

**Desktop and browser IDE that runs the pi coding agent in git worktrees.**

ThinkRail wraps the pi coding agent in a workbench with Monaco editor tabs, terminals, diffs and PR status. Each workspace is a git worktree with its own branch, so several agent chats run in parallel without touching your checkout. It keeps project knowledge in SPEC.md files the agent reads and updates through spec_* tools, and supports MCP servers, Agent Skills and OpenAI-compatible model servers.

- **+** Git worktree workspaces let parallel agent sessions work without touching your checkout
- **+** Topbar tracks branch, PR, CI checks and review status, and can merge from the UI
- **+** Uses existing pi config, Agent Skills and MCP servers; no ThinkRail accounts
- **+** Connects any OpenAI-compatible server such as Ollama, vLLM, LiteLLM or llama.cpp
- **−** Agent engine is pi only; other coding agents are not supported
- **−** Sends usage analytics and error reports tied to an installation ID; extra sharing is opt-in
- **−** Linux builds and desktop installers are unsigned; macOS CLI is signed but not notarized
- **−** Full extension support is still planned, not shipped

<sub>no GPU · Needs git, pi coding agent, model provider (JetBrains AI or own credentials), Node.js >= 22.19 and Bun 1.4.4 (development only) · Models: JetBrains AI, any pi-supported provider, OpenAI-compatible servers (LiteLLM, sglang, vLLM, Ollama, LM Studio, llama.cpp) · [Repo](https://github.com/jetbrains/thinkrail) · [🌐 Site ↗](https://thinkrail.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/thinkrail/)</sub>

<a name="kimi-code"></a>
### #&#8288;64 [kimi-code](https://github.com/moonshotai/kimi-code) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · MIT · Nov 2026</sub>

**Terminal coding agent from Moonshot AI that edits code and runs shell commands.**

Kimi Code CLI is a terminal coding agent that reads and edits code, runs shell commands, searches files and fetches web pages. It defaults to Moonshot AI's Kimi models via OAuth or an API key, and can be configured for other compatible providers. It also supports MCP servers, plugins, subagents, lifecycle hooks, and an ACP mode for Zed and JetBrains.

- **+** Installs as a single binary with one script; no Node.js required
- **+** Built-in coder, explore and plan subagents run in isolated contexts
- **+** `kimi acp` lets Zed, JetBrains or other ACP clients drive a session
- **+** Lifecycle hooks can gate risky tool calls; MCP servers configurable via /mcp-config
- **−** Defaults to Moonshot AI's Kimi models; other providers need manual configuration
- **−** Windows requires Git for Windows, since it uses Git Bash as its shell
- **−** Terminal only; editor use depends on ACP client support

<sub>no GPU · Needs Git for Windows (Windows only), Kimi Code OAuth or Moonshot AI Open Platform API key · Models: Moonshot AI Kimi models, other compatible providers · [Repo](https://github.com/moonshotai/kimi-code) · [📖 Docs ↗](https://moonshotai.github.io/kimi-code/en/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kimi-code/)</sub>

<a name="coucou"></a>
### #&#8288;65 [coucou](https://github.com/louis-cfm/coucou) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Nov 2026</sub>

**Notch companion app that monitors AI coding agent sessions and approves permissions.**

Coucou is a Swift/SwiftUI macOS app (with Tauri builds for Windows and Linux, plus iPhone and Android companions) that shows live Claude Code, Cursor, Codex, Gemini CLI and other agent sessions in the notch. It lets you Allow/Deny permission requests and answer questions from there, and also offers chat with several providers and offline Parakeet dictation on the Mac.

- **+** Approve or deny Claude Code permissions and answer questions without switching to the terminal
- **+** Covers many agents: Claude Code, Cursor, Codex, Gemini CLI, OpenCode, Amp, and custom via coucou_agent tag
- **+** Runs on macOS 15+, Windows 10/11, Linux, iOS 18+ and Android 11+
- **+** No telemetry or account; API keys stored in the OS keychain
- **−** Dictation, notetaker, voice and many pills are macOS-only, some only in the GitHub build
- **−** iPhone app is TestFlight beta; iCloud sync requires the same Apple Account
- **−** Android link works only with the Windows or Linux app, not the Mac
- **−** Name, Mochi character and sounds are not MIT-licensed; only code is

<sub>no GPU · Needs Claude Code or other agent CLIs, iCloud (iPhone sync), FluidAudio (Parakeet dictation), Ollama or LM Studio (optional) · Models: Claude, Gemini, OpenAI, DeepSeek, Qwen · [Repo](https://github.com/louis-cfm/coucou) · [📖 Docs ↗](https://github.com/Louis-CFM/coucou/blob/main/docs/AGENTS.md) · [🌐 Site ↗](https://louisraille.fr/botan) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coucou/)</sub>

<a name="codepilot"></a>
### #&#8288;66 [codepilot](https://github.com/op7418/codepilot) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · custom license · Nov 2026</sub>

**Desktop client for chat and coding agents across many AI providers.**

CodePilot is an Electron and Next.js desktop app for macOS, Windows and Linux that runs chat and coding sessions against 17+ providers, including Anthropic, OpenRouter, Bedrock, Vertex, Ollama and custom OpenAI- or Anthropic-compatible endpoints. It adds MCP servers, skills, a persistent assistant workspace, a task scheduler and bridges to Telegram, Discord, Feishu, QQ and WeChat. Data is stored locally in SQLite.

- **+** Switch providers and models mid-conversation across 17+ providers plus custom endpoints
- **+** Session rewind to checkpoints, split-screen sessions, and token and cost charts
- **+** MCP servers over stdio, sse or http, with runtime status monitoring
- **+** Chat history stays local in SQLite; signed macOS builds update in-app
- **−** BSL-1.1 license: commercial use needs a separate license until the 2029-03-16 change date
- **−** File editing, terminal commands and git operations need the Claude Code CLI installed separately
- **−** Windows builds are unsigned, and Linux updates are manual downloads
- **−** Interface is English and Chinese only; image generation is limited to Gemini

<sub>Needs Node.js 24+ (build from source), Claude Code CLI (optional) · Models: Anthropic, OpenRouter, AWS Bedrock, Google Vertex AI, Ollama · port 3000 · [Repo](https://github.com/op7418/codepilot) · [📖 Docs ↗](https://www.codepilot.sh/docs) · [🌐 Site ↗](https://www.codepilot.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codepilot/)</sub>

<a name="maka"></a>
### #&#8288;67 [maka](https://github.com/apache/maka) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · Apache-2.0 · Nov 2026</sub>

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

<sub>no GPU · Needs Node.js 22.19+ or 24+, npm, Git, ripgrep, Rust 1.98+ (only for peer builds) · Models: cloud APIs, local models, compatible gateways · [Repo](https://github.com/apache/maka) · [🌐 Site ↗](https://maka.apache.org/en/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maka/)</sub>

<a name="codeg"></a>
### #&#8288;68 [codeg](https://github.com/spacering-net/codeg) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · Apache-2.0 · Nov 2026</sub>

**Workspace that runs many ACP coding agents in one chat UI.**

Codeg is a Rust desktop app and headless server that connects to twenty built-in coding agents (Claude Code, Codex, Gemini CLI, OpenCode, Cline and others), plus any ACP agent, over the Agent Client Protocol. It shows them as one structured conversation with live diffs. It adds session import and search, cross-agent delegation with @, scheduled to-dos in worktrees, a code editor, Git tools and a CLI for CI.

- **+** Twenty agents built in, and any agent from the ACP registry can be added
- **+** Imports and searches each agent's session history and can hand it to another agent
- **+** Desktop, server, Docker, iOS and Android clients, plus codeg-cli for scripts and CI
- **+** Unattended to-dos run in isolated Git worktrees for later review
- **−** Wraps third-party agents; each still needs its own runtime and account or API key
- **−** Server mode uses a single access token; no multi-user accounts are described
- **−** Computer Use is labelled preview
- **−** Wide scope (Office, canvas, chat bots) means a large surface to adopt

<sub>no GPU · Docker + Compose · Needs Agent Client Protocol agents (Claude Code, Codex, etc.) · Models: Agent Client Protocol agents · port 3080 · [Repo](https://github.com/spacering-net/codeg) · [📖 Docs ↗](https://docs.codeg.app) · [🌐 Site ↗](https://docs.codeg.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeg/)</sub>

<a name="copilot-lua"></a>
### #&#8288;69 [copilot.lua](https://github.com/zbirenbaum/copilot.lua) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Nov 2026</sub>

**Neovim plugin for GitHub Copilot inline suggestions, written in Lua.**

Pure Lua replacement for github/copilot.vim that runs the Copilot Language Server inside Neovim. It provides inline ghost-text suggestions, a split-window suggestion panel, and experimental next edit suggestions via copilot-lsp. The native server binary is downloaded and SHA-256 verified on first use, with a Node.js server as an alternative.

- **+** Inline suggestions, panel and experimental next edit suggestions in one plugin
- **+** Native server download is version-pinned, SHA-256 verified and cached
- **+** Can hide ghost text while nvim-cmp or blink.cmp menus are open
- **+** Per-filetype and per-buffer attach control via filetypes and should_attach
- **−** Requires a GitHub Copilot account; sign-in via :Copilot auth
- **−** Requires Neovim 0.11.0 or higher
- **−** Native binary covers glibc Linux, macOS and Windows; musl needs Node.js 22+
- **−** Next edit suggestions are experimental and need the separate copilot-lsp plugin

<sub>no GPU · Needs Neovim 0.11.0+, GitHub Copilot account, Node.js 22+ (only for nodejs server type), copilot-lsp (optional, for NES), curl, wget or PowerShell (first install) · Models: GitHub Copilot · [Repo](https://github.com/zbirenbaum/copilot.lua) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/copilot-lua/)</sub>

<a name="maestro"></a>
### #&#8288;70 [runmaestro/maestro](https://github.com/runmaestro/maestro) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · AGPL-3.0 · Nov 2026</sub>

**Desktop app for running multiple coding agents in parallel with playbook automation.**

Maestro is a cross-platform desktop app that manages several CLI coding agents (Claude Code, OpenAI Codex, OpenCode, Factory Droid, plus beta Copilot-CLI, Qwen3 Coder and Oh My Pi) side by side. It passes prompts through to the installed agent CLIs, so existing MCP tools, skills and auth carry over. Auto Run executes markdown checklists, one fresh session per task, and git worktrees isolate parallel agents on separate branches.

- **+** Reuses your installed agent CLIs' MCP tools, skills and auth without extra configuration
- **+** Auto Run playbooks run markdown task lists, each task in a fresh session
- **+** Git worktree sub-agents allow parallel work on isolated branches
- **+** Headless maestro-cli runs playbooks from cron or CI with JSONL output
- **−** Needs at least one supported agent CLI installed and authenticated separately
- **−** AGPL-3.0 license limits use in closed-source derivatives
- **−** Copilot-CLI, Qwen3 Coder and Oh My Pi support is beta; Gemini CLI unsupported
- **−** Tasks are prompt/response, not interactive sessions like the native agent CLIs

<sub>no GPU · Needs Claude Code, Codex, OpenCode, Factory Droid, Copilot-CLI, Qwen Code or Oh My Pi CLI, Git (optional), Cloudflare tunnel (optional, remote access) · Models: Claude Code, OpenAI Codex, OpenCode, Factory Droid, Copilot-CLI (beta) · [Repo](https://github.com/runmaestro/maestro) · [📖 Docs ↗](https://docs.runmaestro.ai) · [🌐 Site ↗](https://runmaestro.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maestro/)</sub>

<a name="autonomous-company"></a>
### #&#8288;71 [autonomous-company](https://github.com/maxmiksa/autonomous-company) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

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

<a name="mimo-code"></a>
### #&#8288;72 [mimo-code](https://github.com/xiaomimimo/mimo-code) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**Terminal coding assistant with persistent memory, subagents and workflows.**

MiMoCode is a terminal-native coding agent that reads and writes code, runs commands and manages Git. It keeps cross-session state in SQLite FTS5-backed memory files and checkpoints, and rebuilds context when the window fills. It adds build and plan agents, subagents, a /goal stop-condition judge, JavaScript workflows and bundled skills, and connects to Xiaomi MiMo, Codex OAuth or OpenAI-compatible providers.

- **+** Checkpoints, project memory and task tree restore context when sessions resume or compact
- **+** Deterministic JavaScript workflows: deep-research, fact-check and research-experiment ship built in
- **+** Connects via OAuth logins, catalog providers by API key, or any OpenAI-compatible endpoint
- **+** mimo serve and mimo attach let the TUI run locally against a remote server
- **−** Built-in macOS Terminal.app is unsupported; iTerm2 or VS Code terminal required
- **−** Voice input and the ASR model work only with a MiMo login or relay
- **−** Web search needs Exa enabled via env var or a separately configured MCP server
- **−** Install is a curl-pipe-to-shell script; no Docker or compose setup

<sub>no GPU · Needs sox (voice input), Exa API (optional web search), xsel (WSL clipboard) · Models: Xiaomi MiMo-V2.6-Pro, MiMo-V2.6-Flash, Codex (ChatGPT Pro/Plus) OAuth, Anthropic, OpenAI · port 4096 · [Repo](https://github.com/xiaomimimo/mimo-code) · [🌐 Site ↗](https://mimo.xiaomi.com/coder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mimo-code/)</sub>

<a name="munder-difflin"></a>
### #&#8288;73 [munder-difflin](https://github.com/harnessmd/munder-difflin) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.9k · MIT · Nov 2026</sub>

**Desktop app that runs many terminal coding agents as a coordinated team.**

Electron desktop app that wraps terminal agent CLIs (Claude Code, Codex, Gemini CLI, Grok, Qwen, OpenCode, Copilot CLI, Cursor and others) in node-pty sessions. An orchestrator agent routes tasks between them through a git-backed mailbox, shared memory and a task board, while agents appear as avatars on a 2D office floor. Some features, such as the Stapler meeting transcriber and the new sidebar, are in the paid Pro tier.

- **+** Wraps 12+ agent CLIs as real PTY processes, using subscriptions you already have
- **+** Per-agent markdown memory, mailboxes and optional git worktrees to avoid branch collisions
- **+** Human approval gates for spend and destructive ops, plus a circuit breaker for looping agents
- **+** Supports BYOK keys and local models via Ollama, LM Studio or vLLM
- **−** Pre-release status (v0.5.6); features and Pro scope are still changing
- **−** Pro tier costs $150/year after the launch offer ends (regional pricing from $100)
- **−** Needs each agent CLI installed and logged in separately; limited by their usage caps
- **−** Dictation and transcription are English only; UI languages limited to English, Chinese, Arabic

<sub>GPU optional · Needs Agent CLIs (claude, codex, etc.), git, Node, uv, MemPalace · Models: Claude Code, OpenAI Codex, Gemini CLI, Antigravity, Grok · [Repo](https://github.com/harnessmd/munder-difflin) · [📖 Docs ↗](https://munderdiffl.in/blog/how-to-install-and-use-munder-difflin/) · [🌐 Site ↗](https://harnessmd.com/download) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/munder-difflin/)</sub>

<a name="stagewise"></a>
### #&#8288;74 [stagewise](https://github.com/stagewise-io/stagewise) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · AGPL-3.0 · Nov 2026</sub>

**Desktop IDE with a built-in coding agent and browser access.**

stagewise is an IDE with a built-in coding agent that can read a browser tab's console and debugger. It can make temporary test changes to a page or connect to a codebase for permanent edits, and it can extract components, styles and color palettes from existing sites. Models come from your own API keys or subscriptions (Kimi, Qwen, MiniMax, Xiaomi MiMo, Mistral, OpenRouter) or from custom providers, including local inference.

- **+** Agent has access to the tab's console and debugger while editing
- **+** Bring your own key; custom providers and local inference can be registered
- **+** Can reverse-engineer a site's components, style system and color palettes
- **+** Integrates with other editors to view and apply code changes
- **−** Hosted stagewise account service is being sunset at the end of November 2026
- **−** AGPL-3.0; uses outside its terms require contacting the vendor for a license
- **−** Distributed as a downloaded app; no Docker or compose setup
- **−** No self-hosting, hardware or system requirements documented in the README

<sub>Needs Model provider API key or subscription · Models: Moonshot Kimi, Alibaba Qwen, MiniMax, Xiaomi MiMo, Mistral · [Repo](https://github.com/stagewise-io/stagewise) · [🌐 Site ↗](https://ade.stagewise.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/stagewise/)</sub>

<a name="hapi"></a>
### #&#8288;75 [hapi](https://github.com/tiann/hapi) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · AGPL-3.0 · Nov 2026</sub>

**Remote control for local Claude Code, Codex and other coding agent sessions.**

HAPI wraps official coding agent CLIs (Claude Code, Codex, Cursor Agent, OpenCode, Copilot and others) and runs a hub so you can watch, approve and continue sessions from a web/PWA client, native iOS/Android apps or a Telegram Mini App. The hub can expose itself through an end-to-end encrypted relay (WireGuard + TLS), Cloudflare Tunnel or Tailscale. Sessions can move between local terminal and remote without restarting.

- **+** Wraps the official agent CLIs, so the terminal workflow stays the same
- **+** Supports about ten agents behind one hub, including Claude Code, Codex and OpenCode
- **+** Web/PWA client is free and includes remote terminal and voice assistant
- **+** Self-hosted access via Cloudflare Tunnel or Tailscale as alternatives to the relay
- **−** Native iOS and Android apps are paid
- **−** AGPL-3.0 license limits use in closed network services
- **−** No Docker or Compose files provided; source build requires Bun 1.4.4
- **−** Shared Codex sessions require Codex 0.154.0 or newer

<sub>no GPU · Needs Bun 1.4.4 (build from source), Claude Code / Codex / other agent CLIs, Optional: Cloudflare Tunnel or Tailscale · Models: Claude Code, Codex, Cursor Agent, Grok Build, OpenCode · [Repo](https://github.com/tiann/hapi) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hapi/)</sub>

<a name="gptme"></a>
### #&#8288;76 [gptme](https://github.com/gptme/gptme) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Nov 2026</sub>

**Terminal AI agent that runs shell, Python, browser and file tools.**

gptme is a Python CLI agent that runs shell commands and Python, edits files with patch tools, browses via Playwright, and feeds output back to the model to self-correct. It works with Anthropic, OpenAI, Google, DeepSeek, OpenRouter and local servers such as Ollama, llama.cpp and vLLM. It also ships a Textual TUI, a web UI with REST server, an MCP client and server, and ACP support for Zed and JetBrains.

- **+** Provider-agnostic: hosted APIs, OpenRouter, or local via Ollama, LM Studio, vLLM, llama.cpp
- **+** Acts as both MCP client and MCP server, plus ACP for Zed and JetBrains
- **+** Plugins, skills, hooks and lessons extend it; sandboxed execution via Docker or Wasmtime
- **+** Runs headless for CI and systemd-scheduled agents via gptme service init
- **−** Runs code in your local environment by default; sandboxing is a separate option
- **−** RAG tool needs the separate gptme-rag package
- **−** Several features live in add-on repos (gptme-contrib, webui, agent template)

<sub>GPU optional · Compose · Needs Python, Playwright (browser tool), gptme-rag (rag tool), Ollama or OpenAI-compatible server (local models) · Models: Anthropic, OpenAI, Google Gemini, DeepSeek, OpenRouter · [Repo](https://github.com/gptme/gptme) · [▶️ Demo ↗](https://chat.gptme.org) · [📖 Docs ↗](https://gptme.org/docs/) · [🌐 Site ↗](https://gptme.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gptme/)</sub>

<a name="gnhf"></a>
### #&#8288;77 [gnhf](https://github.com/kunchenguid/gnhf) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Nov 2026</sub>

**Overnight loop that runs coding agent CLIs, one committed change per iteration.**

gnhf is a Node CLI that repeatedly invokes a coding agent (Claude by default, plus other agent CLIs and ACP targets) against a prompt inside a Git repo. Each iteration is committed on success or rolled back with git reset --hard on failure, and a shared notes.md carries context between iterations. Runs stop on caps for iterations, tokens, run time, or a natural-language stop condition.

- **+** Per-iteration unsigned commits and rollback on failure make each change easy to cherry-pick or revert
- **+** --worktree runs several agents on one repo in isolated worktrees and branches
- **+** Waits out Claude usage-limit windows and resumes; caps via --max-iterations, --max-tokens, --max-run-time
- **+** Resumes from an existing gnhf/ branch; run metadata stays in .gnhf/runs and is ignored locally
- **−** Requires a Git repository with a clean working tree to start
- **−** Supplies no model; needs a separate agent CLI and its credentials or subscription
- **−** README says local models report --stop-when conditions unreliably
- **−** Known Linux issue: no-commit worktrees can be left behind after systemd-inhibit re-exec

<sub>no GPU · Needs Node.js, Git, a coding agent CLI (claude, codex, copilot, opencode, pi, cursor) or ACP target · Models: claude, codex, copilot, opencode, pi · [Repo](https://github.com/kunchenguid/gnhf) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gnhf/)</sub>

<a name="dsh-tauri-deepseek-harness-desktop"></a>
### #&#8288;78 [dsh-tauri/deepseek-harness-desktop](https://github.com/dsh-tauri/deepseek-harness-desktop) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Nov 2026</sub>

**Tauri desktop client for DeepSeek Harness with plugin management and mobile pairing.**

Desktop wrapper for the upstream DeepSeek Harness (dsh) agent platform, built with Tauri 2 and React 19. It installs and updates the Node/pnpm runtime and Harness kernel itself, manages plugins and profiles, and exposes dsh and pnpm through managed CLI shims. An Android/iOS companion app connects to the desktop Harness over LAN or a Cloudflare tunnel.

- **+** No manual Node.js, pnpm or Docker install; runtime and kernel are managed in-app
- **+** Installers for Windows, macOS and Linux, plus Homebrew and Fedora Copr packages
- **+** Offline Bundle installers available; 12 built-in plugins, with local and community plugin install
- **+** Mobile app pairs by QR over LAN or Cloudflare tunnel
- **−** License is MIT plus an additional non-commercial clause
- **−** Only Harness kernel 0.2.1-rc.4 and later supported; plugin compatibility not guaranteed
- **−** Marked development preview; upstream dsh has breaking changes
- **−** dsh runs code locally; remote access is not read-only, so QR codes must stay private

<sub>Needs DeepSeek Harness (dsh) kernel 0.2.1-rc.4+, Git (for Git features), Cloudflare tunnel (optional, remote access) · [Repo](https://github.com/dsh-tauri/deepseek-harness-desktop) · [📖 Docs ↗](https://dshtauri.mintlify.site) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-tauri-deepseek-harness-desktop/)</sub>

<a name="ovis"></a>
### #&#8288;79 [devswha/ovis](https://github.com/devswha/ovis) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

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

<a name="zeroshot"></a>
### #&#8288;80 [zeroshot](https://github.com/the-open-engine/zeroshot) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

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

<a name="neo"></a>
### #&#8288;81 [neo](https://github.com/neomjs/neo) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Nov 2026</sub>

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

<a name="nanocoder"></a>
### #&#8288;82 [nanocoder](https://github.com/nano-collective/nanocoder) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · custom license · Nov 2026</sub>

**Terminal coding agent that works with local or any OpenAI-compatible model.**

Nanocoder is a terminal coding agent written in TypeScript, installed through npm, Homebrew or Nix. It runs against local models via Ollama or any OpenAI-compatible API, and offers interactive and non-interactive modes, MCP server configuration, skills, hooks and PR review from the CLI. It is developed by the Nano Collective, a non-profit community group.

- **+** Provider-agnostic: Ollama locally, or OpenRouter, Requesty, Anthropic, Google via compatible APIs
- **+** Several modes (normal, auto-accept, yolo, plan, architect) selectable with --mode
- **+** Non-interactive `run` command and `review` command for branches or PRs
- **+** README states no paid tiers and no telemetry sending prompts
- **−** `nanocoder review` is diff-only and needs a TTY; output cannot be captured to a file
- **−** `worktree` command requires Git and an authenticated gh CLI
- **−** License is reported as NOASSERTION, so terms are unclear from metadata

<sub>GPU optional · Needs Node.js/npm, Ollama (for local models), Git and gh CLI (worktree command) · Models: Ollama, OpenAI-compatible APIs, OpenRouter, Requesty, Anthropic · [Repo](https://github.com/nano-collective/nanocoder) · [📖 Docs ↗](https://docs.nanocollective.org/nanocoder/docs) · [🌐 Site ↗](https://nanocollective.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nanocoder/)</sub>

<a name="supacode"></a>
### #&#8288;83 [supacode](https://github.com/supabitapp/supacode) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · custom license · Nov 2026</sub>

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

<a name="agtx"></a>
### #&#8288;84 [agtx](https://github.com/fynnfluegge/agtx) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="symphony"></a>
### #&#8288;85 [symphony](https://github.com/openai/symphony) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

**Spec and Elixir reference for agents that pick up Linear tasks and open PRs.**

Symphony watches a Linear board for work and spawns isolated agent runs for each task. Agents report proof of work such as CI status, PR review feedback, complexity analysis and walkthrough videos, and land the PR once accepted. The repo ships a language-agnostic SPEC.md and an experimental Elixir reference implementation.

- **+** Language-agnostic SPEC.md lets you implement it in any language
- **+** Each task runs as an isolated, autonomous implementation run
- **+** Agents attach proof of work: CI status, review feedback, walkthrough videos
- **+** Apache-2.0 licensed reference implementation in Elixir
- **−** Described as a low-key engineering preview for trusted environments only
- **−** Reference implementation is experimental
- **−** Expects codebases that have already adopted harness engineering

<sub>Needs Linear, Codex · Models: Codex · [Repo](https://github.com/openai/symphony) · [▶️ Demo ↗](https://player.vimeo.com/video/1186371009?h=5626e4b899) · [📖 Docs ↗](https://github.com/openai/symphony/blob/main/SPEC.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/symphony/)</sub>

<a name="ralph-claude-code"></a>
### #&#8288;86 [ralph-claude-code](https://github.com/frankbria/ralph-claude-code) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · MIT · Nov 2026</sub>

**Bash loop that reruns Claude Code on a task list until done.**

Ralph is a set of shell commands that run Claude Code repeatedly against a project's PROMPT.md and fix_plan.md, following Geoffrey Huntley's "Ralph Wiggum" technique. It stops only when completion heuristics and an explicit EXIT_SIGNAL agree. It adds rate limiting (100 calls/hour by default), a circuit breaker, session resume and tmux monitoring, with optional Docker and E2B sandboxes.

- **+** Exit needs both completion indicators and an explicit EXIT_SIGNAL, reducing premature stops
- **+** Circuit breaker, hourly rate limit and 5-hour API limit handling guard against runaway loops
- **+** Imports tasks from PRD files, GitHub issues or beads; ralph-enable detects project type
- **+** Optional Docker or E2B sandbox, dry-run mode, git backup branches with rollback
- **−** Tied to the claude CLI; multi-provider support (Codex, Gemini, etc.) is still in progress
- **−** Unreleased change makes .ralphrc data-only, breaking files that relied on shell syntax
- **−** Exit detection relies partly on natural-language heuristics, so tuning may be needed
- **−** No tagged release; installs by cloning the repo and running install.sh

<sub>no GPU · Docker · Needs Claude Code CLI, tmux, Docker (optional sandbox), E2B (optional sandbox) · Models: Claude (via Claude Code) · [Repo](https://github.com/frankbria/ralph-claude-code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph-claude-code/)</sub>

<a name="puerts"></a>
### #&#8288;87 [puerts](https://github.com/tencent/puerts) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · custom license · Nov 2026</sub>

**Multi-language scripting for Unity and Unreal, with an in-editor LLM agent and MCP server.**

PuerTS embeds JavaScript/TypeScript (V8, QuickJS, Node.js) in Unity, Unreal and .NET, and since Unity 3.0 also Lua 5.4 and CPython, all behind one ScriptEnv API with C#/C++ interop. The Puerts.AI part adds a Unity Editor assistant, run as an in-editor agent or as an MCP server inside the Unity process, plus an agent framework usable at game runtime.

- **+** MCP server runs inside the Unity process and exposes a single tool, loading builtins on demand
- **+** Same ScriptEnv API across V8, QuickJS, Node.js, Lua and Python backends in Unity
- **+** Generates TypeScript declarations for typed access to engine APIs
- **+** Agent framework also runs at game runtime, with demo repos for NPCs and maze navigation
- **−** Puerts.AI and the MCP server are Unity only; Unreal supports only JS/TS
- **−** Primarily a scripting runtime; the AI tooling is a secondary component
- **−** Python backend is desktop only; no Android or iOS
- **−** QuickJS backend has no debugging support

<sub>Needs Unity or Unreal Engine or .NET, LLM provider for Puerts.AI · [Repo](https://github.com/tencent/puerts) · [📖 Docs ↗](https://puerts.github.io/en) · [🌐 Site ↗](https://puerts.github.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/puerts/)</sub>

<a name="openbitfun"></a>
### #&#8288;88 [openbitfun](https://github.com/gcwing/openbitfun) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Nov 2026</sub>

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

<a name="atomic-agent"></a>
### #&#8288;89 [atomic-agent](https://github.com/atomicbot-ai/atomic-agent) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Nov 2026</sub>

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

<sub>GPU optional · Docker + Compose · Needs llama.cpp (llama-server), Chrome/Edge/Brave/Chromium (browser tools) · Models: GGUF via llama-server, OpenAI-compatible, OpenRouter, Gemini, Anthropic · [Repo](https://github.com/atomicbot-ai/atomic-agent) · [🌐 Site ↗](https://atomicagent.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/atomic-agent/)</sub>

<a name="codenomad"></a>
### #&#8288;90 [codenomad](https://github.com/neuralnomadsai/codenomad) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

**Desktop and browser workspace for OpenCode V2 sessions and Git worktrees.**

CodeNomad is a UI for OpenCode V2 that runs as an Electron or Tauri desktop app, or as an npm-launched server you open in a browser. It adds project tabs, nested and forkable sessions, Git worktree management, file attachments, MCP and plugin controls, and web previews. It connects to OpenCode's shared background service, so sessions stay available to terminal clients.

- **+** Sessions live in OpenCode's shared service, so they survive closing tabs, windows or the backend
- **+** Git worktree support moves a session with its subsessions and shows Git changes
- **+** Desktop builds bundle Node and npm; the server runs with one npx command
- **+** Remote access via password-protected HTTPS or an OpenTunnel relay without opening ports
- **−** Requires OpenCode V2 (2.2.3 minimum); OpenCode V1 is not supported
- **−** Git is not bundled; worktrees and Git operations need it on the backend PATH
- **−** Server mode defaults to a self-signed HTTPS certificate, which triggers browser warnings
- **−** Linux builds are x64 only and tested on Ubuntu 24.04; macOS builds are not notarized

<sub>no GPU · Needs OpenCode V2 CLI (2.2.3+, 2.2.5 recommended), Git, Node.js 24 LTS (server and source builds only) · Models: Any provider configured in OpenCode · [Repo](https://github.com/neuralnomadsai/codenomad) · [📖 Docs ↗](https://neuralnomadsai.github.io/CodeNomad/) · [🌐 Site ↗](https://neuralnomadsai.github.io/CodeNomad/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codenomad/)</sub>

<a name="codync"></a>
### #&#8288;91 [codync](https://github.com/leepokai/codync) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

**Message your local coding agents as persistent bots from iPhone or desktop.**

Codync runs a Rust host (codync-host) on your computer that drives coding agents such as Claude Code, Codex, Cursor and Gemini over the Agent Client Protocol, exposing each as a named bot with its own project folder and approval policy. You chat with bots from a SwiftUI iPhone app, an Electron desktop app, or a terminal UI, with group chats, approval cards and push notifications. Remote access uses a direct connection, Tailscale, or an end-to-end encrypted Cloudflare relay.

- **+** Works with ~40 agents from the ACP registry; each bot picks its own
- **+** Runs agents on your existing subscriptions; no provider API calls with your login
- **+** Single static Rust host binary for macOS, Windows and Linux, with SQLite transcripts
- **+** Scriptable: codync-host send --wait --json returns structured results with exit codes
- **−** iPhone app is an App Store download and can lag host releases
- **−** Windows lacks remote screen, on-device speech and the Claude Code status line hook
- **−** Claude Code, Codex and Pi adapters need Node.js via npx
- **−** Remote access beyond your network needs the hosted Cloudflare relay and an account

<sub>no GPU · Needs Node.js (for Claude Code, Codex, Pi ACP adapters), Installed coding agents (Claude Code, Codex, etc.), Cloudflare relay (optional, remote access) · Models: Agent Client Protocol agents, Claude Code, Codex, Cursor, Gemini CLI · port 19222 · [Repo](https://github.com/leepokai/codync) · [📖 Docs ↗](https://www.codync.dev/docs) · [🌐 Site ↗](https://www.codync.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codync/)</sub>

<a name="cate"></a>
### #&#8288;92 [cate](https://github.com/0-ai-ug/cate) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Nov 2026</sub>

**Desktop IDE that lays out coding-agent terminals on an infinite canvas.**

Cate is a desktop app where terminals, Monaco editors, browsers and document viewers sit on a pannable canvas or in docked tabs. Terminals running Claude Code, Codex or other agent CLIs show running, waiting or finished state and notify you when input is needed. It creates git worktrees per branch so parallel agents stay separated.

- **+** Per-terminal agent status and notifications for turn end and permission prompts
- **+** One-step git worktree creation from a local branch, remote branch or open PR
- **+** Agent sessions reattach with scrollback and resume commands after restart
- **+** Prebuilt installers for macOS, Windows and Linux, plus a Homebrew cask
- **−** Status reporting works only with supported agent CLIs; the list is not given
- **−** Desktop app; no web or self-hosted server deployment is described
- **−** Ships no agent or model of its own; you bring the agent CLI

<sub>no GPU · Needs git, agent CLIs such as Claude Code or Codex · [Repo](https://github.com/0-ai-ug/cate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cate/)</sub>

<a name="xum"></a>
### #&#8288;93 [xum](https://github.com/coder/xum) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Nov 2026</sub>

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

<a name="github1s"></a>
### #&#8288;94 [github1s](https://github.com/conwnet/github1s) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

**Read-only VS Code in the browser for GitHub and GitLab repositories.**

GitHub1s opens a GitHub repository in a VS Code web interface when you add "1s" to the URL. You can browse files, search code, switch branches or tags, inspect commits and review pull or merge request diffs without cloning. A built-in AI chat sends code context to a model endpoint you configure.

- **+** Hosted at github1s.com: change the URL and browse, no install or clone
- **+** Also covers GitLab (gitlab1s.com) and npm packages (npmjs1s.com)
- **+** Public repositories need no sign-in; private ones use OAuth or an access token
- **+** AI chat can look up relevant code and answer follow-ups about a file or selection
- **−** Remote repositories are read-only, so no editing or running code
- **−** Search and navigation depend on upstream services and their rate limits
- **−** AI needs a model endpoint that accepts browser requests; code context is sent to it
- **−** Primarily an explorer; the AI chat is secondary to browsing

<sub>no GPU · Docker · Needs Sourcegraph, searchcode, OSS Insight, GitHub or GitLab APIs · Models: User-configured model endpoint that accepts browser requests · [Repo](https://github.com/conwnet/github1s) · [▶️ Demo ↗](https://github1s.com/conwnet/github1s) · [📖 Docs ↗](https://github.com/conwnet/github1s/blob/master/docs/usage.md) · [🌐 Site ↗](https://github1s.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github1s/)</sub>

<a name="terax-ai"></a>
### #&#8288;95 [terax-ai](https://github.com/crynta/terax-ai) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · Apache-2.0 · Nov 2026</sub>

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

<a name="forgecode"></a>
### #&#8288;96 [forgecode](https://github.com/tailcallhq/forgecode) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="mistral-vibe"></a>
### #&#8288;97 [mistral-vibe](https://github.com/mistralai/mistral-vibe) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent that reads, edits and runs commands in your repo.**

Mistral Vibe is a Python CLI coding agent from Mistral AI. You describe a task in the terminal, and it reads your code, edits files and runs commands, asking for approval before risky actions. Sign-in uses a Mistral account or an API key, and it also has a programmatic mode and use from other IDEs.

- **+** Installs with one curl script on macOS/Linux or `uv tool install` on any platform
- **+** Asks for approval before risky actions; permissions model is documented
- **+** Programmatic mode and use from other IDEs are documented
- **+** Telemetry can be turned off with `enable_telemetry = false` in config.toml
- **−** Does not accept pull requests; only bug reports and feature requests
- **−** Needs a GIL-enabled Python 3.12+; some Python versions break installs
- **−** Sign-in is a Mistral account or API key; other providers not stated
- **−** Telemetry and crash reporting are on unless disabled in config

<sub>no GPU · Needs Python 3.12+ (GIL build), uv (Windows install), Mistral account or API key · Models: Mistral models via Mistral API · [Repo](https://github.com/mistralai/mistral-vibe) · [📖 Docs ↗](https://docs.mistral.ai/vibe/code/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mistral-vibe/)</sub>

<a name="rewrite"></a>
### #&#8288;98 [rewrite](https://github.com/openrewrite/rewrite) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Nov 2026</sub>

**Recipe-based automated refactoring engine for Java and other languages.**

OpenRewrite parses source into a type-aware Lossless Semantic Tree and runs prepackaged recipes that apply framework migrations, security fixes and style changes. Maven and Gradle plugins run one recipe at a time against a single repository. Parsers cover Java, Kotlin, Groovy, JavaScript/TypeScript, Python and C#. The code is deterministic rewriting, not LLM-based; the commercial Moderne platform adds multi-repo runs and agent tooling.

- **+** Deterministic, type-aware recipes for framework migrations, security fixes and style cleanup
- **+** Maven and Gradle plugins run recipes directly on a repository
- **+** Recipes can be customized or written from scratch
- **+** Parsers for Java, Kotlin, Groovy, JavaScript/TypeScript, Python and C#
- **−** Tiered licensing: non-Java parsers and base recipes use the Moderne Source Available License
- **−** Proprietary recipes need a Moderne commercial license
- **−** Plugins run one recipe at a time on one repository; multi-repo needs Moderne CLI or platform
- **−** Not an LLM agent; agent integration comes through Moderne tools such as its MCP server

<sub>no GPU · Needs Maven or Gradle plugin (for Java) · [Repo](https://github.com/openrewrite/rewrite) · [📖 Docs ↗](https://docs.openrewrite.org) · [🌐 Site ↗](https://www.moderne.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rewrite/)</sub>

<a name="nodeterm"></a>
### #&#8288;99 [nodeterm](https://github.com/eneskirca/nodeterm) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · custom license · Nov 2026</sub>

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

<a name="happier"></a>
### #&#8288;100 [happier](https://github.com/happier-dev/happier) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Nov 2026</sub>

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

<a name="botmux"></a>
### #&#8288;101 [botmux](https://github.com/deepcoldy/botmux) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

**Daemon that runs AI coding CLIs from Feishu/Lark chat with streamed cards.**

botmux is a daemon that listens for Feishu/Lark messages and starts a separate CLI process per session. It bridges existing coding CLIs such as claude-code, codex, cursor and opencode rather than reimplementing them, streams each turn back as a live card, and offers a writable browser terminal. It ships as a self-contained binary for Linux and macOS.

- **+** Bridges the real CLI process, so its hooks, memory and MCP keep working
- **+** 20+ built-in adapters, switchable per bot via cliId or /cli per session
- **+** Self-contained binary; install and run need no local Node
- **+** Several bots with different CLIs can share one group via @mention routing
- **−** Tied to Feishu/Lark as the only chat front end
- **−** Windows only through WSL2; Linux and macOS supported natively
- **−** README and most docs are written mainly in Chinese
- **−** Adapters may need updates when a CLI changes flags or resume behavior

<sub>no GPU · Needs Feishu/Lark app, tmux (optional, for session attach) · Models: claude-code, codex, cursor, opencode, copilot · [Repo](https://github.com/deepcoldy/botmux) · [📖 Docs ↗](https://deepcoldy.github.io/botmux/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/botmux/)</sub>

<a name="traycer"></a>
### #&#8288;102 [traycer](https://github.com/traycerai/traycer) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2026</sub>

**Desktop app that runs multiple coding agents in parallel with shared context.**

Traycer is a desktop app that connects to coding agents you already subscribe to, such as Claude Code, Codex, Cursor, OpenCode and Copilot, and runs several in parallel. It shares context across models and providers, lets you switch models within an agent, and supports agent-to-agent messaging. Shareable boards and ticket assignment cover team use.

- **+** Connects to 25+ existing coding agents, including Claude Code, Codex, Cursor and Copilot
- **+** Switch models within one agent while keeping the same context window
- **+** Native installers for macOS (arm64, x64), Linux (AppImage, deb, rpm) and Windows
- **+** Shareable boards, ticket assignment and real-time editing for teams
- **−** Agent-to-agent transcript reading and message delivery vary by user, host and runtime
- **−** Release builds may enable Sentry crash reporting and PostHog analytics
- **−** Privacy Mode is opt-in for individuals; with it off, prompts may be logged

<sub>Needs Coding agent subscriptions (Claude Code, Codex, Cursor, etc.) or Traycer inference subscription · Models: Claude Code, Codex, Cursor, OpenCode, GitHub Copilot · [Repo](https://github.com/traycerai/traycer) · [▶️ Demo ↗](https://youtu.be/doh2yz3ZFvU) · [📖 Docs ↗](https://docs.traycer.ai) · [🌐 Site ↗](https://traycer.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/traycer/)</sub>

<a name="wally"></a>
### #&#8288;103 [wally](https://github.com/runanywhereai/wally) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

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

<a name="agent-deck"></a>
### #&#8288;104 [agent-deck](https://github.com/asheshgoplani/agent-deck) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Nov 2026</sub>

**Terminal UI that manages many AI coding agent sessions in one place.**

Agent Deck is a Go terminal UI that tracks Claude Code, OpenCode, Codex, Gemini CLI and Pi sessions and shows which are running, waiting or done. It adds groups, search, session forking, git worktrees, cost tracking, and per-session MCP and skill attachment. A conductor session can supervise the others and report through Telegram, Slack, Discord or Mattermost.

- **+** Single view of session status across several agent CLIs
- **+** Per-session MCP and skill toggling without hand-editing config files
- **+** Per-group and per-conductor Claude account config, plus switching a session's account
- **+** Installs via curl script, Homebrew or go install
- **−** Supports macOS, Linux and WSL only; no native Windows
- **−** Conductor notifications need a bot token and a setup wizard
- **−** Many keybindings and seven config precedence layers to learn
- **−** Forking works only for supported session types

<sub>no GPU · Needs tmux, Claude Code, OpenCode, Codex, Gemini CLI or Pi · Models: Claude Code, OpenCode, Codex, Gemini CLI, Pi · port 8420 · [Repo](https://github.com/asheshgoplani/agent-deck) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-deck/)</sub>

<a name="warp"></a>
### #&#8288;105 [warp](https://github.com/warpdotdev/warp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · AGPL-3.0 · Nov 2026</sub>

**Terminal-based development environment with a built-in coding agent.**

Warp is a Rust client that started as a terminal and now includes a built-in coding agent. It can also run third-party CLI agents such as Claude Code, Codex and Gemini CLI. The client source is public, and the repository is itself maintained partly by automated agents (Warp Factories).

- **+** Runs its own agent or external CLI agents (Claude Code, Codex, Gemini CLI)
- **+** Client source is public; build with ./script/bootstrap and ./script/run
- **+** UI framework crates (warpui_core, warpui) are MIT-licensed
- **+** Written in Rust; contribution flow and AGENTS.md engineering guide documented
- **−** Most code is AGPL-3.0, which constrains proprietary forks
- **−** Factories automation is early access with a demo booking flow
- **−** README covers only the client; server-side components are not described

<sub>Docker · Models: GPT models, Claude Code, Codex, Gemini CLI · [Repo](https://github.com/warpdotdev/warp) · [▶️ Demo ↗](https://build.warp.dev) · [📖 Docs ↗](https://docs.warp.dev) · [🌐 Site ↗](https://www.warp.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/warp/)</sub>

<a name="firstmate"></a>
### #&#8288;106 [firstmate](https://github.com/kunchenguid/firstmate) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Nov 2026</sub>

**Agent distro where one chat agent runs parallel coding agents.**

firstmate is a cloned repo of instructions (AGENTS.md), skills and shell helper scripts. Launched inside a terminal coding agent such as Claude Code, Grok or Pi, it turns that session into a "first mate" that spawns crewmate agents in tmux or Herdr windows, each in its own git worktree. A bash watcher supervises them, and you get back PRs, local merges or investigation reports.

- **+** Each task gets an isolated git worktree, so parallel work on one repo does not collide
- **+** Per-project modes: no-mistakes, direct-PR or local-only, with optional +yolo merge autonomy
- **+** State lives on disk and in the session backend, so sessions recover after a restart
- **+** Works with many primary harnesses and session backends, including tmux, Herdr, Zellij and Orca
- **−** Needs an existing agent harness and gh login; not usable standalone
- **−** Most backends other than tmux and Herdr are marked experimental
- **−** Codex and OpenCode carry more supervision tradeoffs than the three co-primary harnesses
- **−** macOS and Linux only; no tagged releases

<sub>no GPU · Needs git, GitHub CLI (gh), tmux (default backend), treehouse, a supported agent harness (Claude Code, Grok, Pi, Codex, etc.) · Models: Claude Code, Grok, Pi, Oh My Pi, Codex · [Repo](https://github.com/kunchenguid/firstmate) · [📖 Docs ↗](https://github.com/kunchenguid/firstmate/blob/main/docs/architecture.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/firstmate/)</sub>

<a name="design-extract"></a>
### #&#8288;107 [design-extract](https://github.com/manavarya09/design-extract) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Nov 2026</sub>

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

<a name="eac-desktop"></a>
### #&#8288;108 [eac-desktop](https://github.com/ebony-vinyl/eac-desktop) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Nov 2026</sub>

**Tauri desktop app that runs the DeepSeek Harness agent with a local Web UI.**

EAC-Desktop packages DeepSeek Harness (dsh) as a native desktop app. A Rust/Tauri shell starts a Node sidecar over stdio JSON-RPC, which launches the dsh kernel and opens its Web UI in a window. It bundles Node, npm and pnpm runtimes, tracks per-session file changes with restore, and adds a plugin market and swappable skins.

- **+** Bundles Node, npm and pnpm runtimes, so no separate Node install is needed
- **+** Per-channel DPX environments keep profiles, sessions and workspace data separate
- **+** Session file-change view with restore, plus snapshot and rollback for plugins
- **+** Installers for Windows x64, Linux (AppImage, deb) and macOS arm64
- **−** README says DPX gives no filesystem sandbox; absolute paths follow OS permissions
- **−** Linux (v5.3.6) and macOS (v5.1.0) builds trail Windows v6.0.0
- **−** Skin sources include CC BY-NC-SA 4.0 content, which limits redistribution
- **−** Source build needs submodules, Node 24, pnpm 11.7.0, Rust and network access

<sub>no GPU · Needs DeepSeek Harness (dsh) kernel, dsh-dpx, Tauri, Node.js 24 and pnpm 11.7.0 (source builds), Rust stable (source builds) · Models: Provider-configured models via DeepSeek Harness · [Repo](https://github.com/ebony-vinyl/eac-desktop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eac-desktop/)</sub>

<a name="ralph-orchestrator"></a>
### #&#8288;109 [ralph-orchestrator](https://github.com/mikeyobrien/ralph-orchestrator) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Nov 2026</sub>

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

<a name="gentle-shell"></a>
### #&#8288;110 [gentle-shell](https://github.com/gentleman-programming/gentle-shell) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

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

<a name="agent-teams-ai"></a>
### #&#8288;111 [agent-teams-ai](https://github.com/777genius/agent-teams-ai) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · AGPL-3.0 · Nov 2026</sub>

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

<a name="org2"></a>
### #&#8288;112 [org2](https://github.com/org2ai/org2) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · AGPL-3.0 · Oct 2026</sub>

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

<a name="obsidian-agent-client"></a>
### #&#8288;113 [obsidian-agent-client](https://github.com/rait-09/obsidian-agent-client) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

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

<a name="lody"></a>
### #&#8288;114 [lody](https://github.com/lodyai/lody) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Nov 2026</sub>

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

<a name="ghostex"></a>
### #&#8288;115 [ghostex](https://github.com/maddada/ghostex) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Native workspace for running many coding agents, with desktop and phone apps.**

Ghostex is a Rust/GPUI desktop app that wraps coding agents such as Claude Code, Codex, OpenCode and Gemini CLI in a chat view, terminal, embedded Chromium panes and an optional VS Code editor. Sessions persist across restarts. iOS and Android apps pair through Easy Connect or Tailscale to read transcripts and send prompts, and agents can open and steer other agents through the ghostex command.

- **+** Works with many agent CLIs: Claude Code, Codex, OpenCode, Pi, Gemini, Grok, Cursor, Copilot CLI
- **+** Sessions survive restarts; fuzzy search of all past prompts, also via gx f
- **+** Runs on macOS, Windows and Linux, with Android and iOS apps; brew, deb, rpm and AUR packages
- **+** Prompt queueing, worktree per task, split panes, and Markdown/HTML annotations sent back to the agent
- **−** iOS access is by TestFlight, requested through the project's Discord
- **−** Chromium is installed on first use of the browser or code editor
- **−** Several features depend on third-party parts such as CEF, code-server and Trycua

<sub>Needs Chromium (CEF), Agent CLIs such as Claude Code or Codex, Tailscale (optional) · Models: Claude Code, Codex, OpenCode, Pi, Gemini CLI · [Repo](https://github.com/maddada/ghostex) · [🌐 Site ↗](https://ghostex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ghostex/)</sub>

<a name="mysti"></a>
### #&#8288;116 [mysti](https://github.com/deepmyst/mysti) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**VS Code extension that coordinates Claude Code, Codex and other coding agents.**

Mysti is a VS Code extension that puts several coding agents in one conversation. You address agents with @mentions to get independent answers, or chain them with "then" so one agent reviews another's finished work. It ships 16 provider adapters plus a coordinator, Brainstorm discussion modes, Canvas previews and checkpoints. It is still labelled beta.

- **+** 16 provider adapters, including Claude Code, Codex, Gemini CLI, Copilot CLI, Ollama and OpenRouter
- **+** @mentions give parallel opinions; an explicit 'then' hands one agent's result to another
- **+** Context via file mentions, @problems diagnostics and @git changes
- **+** Brainstorm strategies: Quick, Debate, Red Team, Perspectives, Delphi
- **−** Beta: native provider/account coverage and long-duration testing are incomplete
- **−** Ollama and LocalAI show tool proposals but do not execute them
- **−** Composer attachments are not forwarded to explicitly assigned collaborators
- **−** No model access included; each provider bills its own usage per agent

<sub>no GPU · Needs VS Code 1.86+, At least one configured provider (Claude Code, Codex, Ollama, OpenRouter, etc.) · Models: Claude Code, OpenAI Codex, Gemini CLI, GitHub Copilot CLI, Cline · [Repo](https://github.com/deepmyst/mysti) · [▶️ Demo ↗](https://github.com/DeepMyst/Mysti/blob/main/docs/DEMO_GALLERY.md) · [📖 Docs ↗](https://github.com/DeepMyst/Mysti/blob/main/docs/README.md) · [🌐 Site ↗](https://marketplace.visualstudio.com/items?itemName=DeepMyst.mysti) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mysti/)</sub>

<a name="freebuff"></a>
### #&#8288;117 [freebuff](https://github.com/codebuffai/freebuff) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent with free hosted models, supported by text ads.**

Freebuff is a multi-agent coding tool installed with `npm install -g freebuff` and run inside a project directory. File-finding, editing and review agents work on the repo using a catalog of hosted models (DeepSeek, MiMo, GLM, Solar, GPT, Gemini), paid for in daily hours rather than API keys. The same brand also covers a desktop app, web app builder, GitHub cloud agents and a chat product, built on the Codebuff framework.

- **+** No API key or subscription; free allowance of 5 hours a day in limited-access regions
- **+** Specialized agents for file finding, editing, research and review
- **+** Desktop app isolates parallel agents and can run local Claude Code and Codex
- **+** Apache-2.0 TypeScript monorepo built on the Codebuff SDK
- **−** Models are hosted by Freebuff; free tier is funded by text ads
- **−** Messages and traces may be used for ad personalization and, for some models, AI training
- **−** Outside supported regions or on VPN: 4 to 5 hours a day and fewer models
- **−** Local development needs Docker and a configured .env.local

<sub>no GPU · Needs Node.js/npm, Freebuff hosted model service, Docker (contributor setup only), Bun (contributor setup only) · Models: DeepSeek V4.1 Flash, MiMo v2.6, GLM 5.3 Flash, Solar Mini 4, Solar Pro 4 · [Repo](https://github.com/codebuffai/freebuff) · [📖 Docs ↗](https://codebuff.com/docs) · [🌐 Site ↗](https://freebuff.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/freebuff/)</sub>

<a name="jetbrains-cc-gui"></a>
### #&#8288;118 [jetbrains-cc-gui](https://github.com/zhukunpenglinyutong/jetbrains-cc-gui) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

**JetBrains IDE plugin giving Claude Code, Codex and other coding CLIs a chat UI.**

CC GUI is an IntelliJ IDEA plugin, written mainly in Java with a webview frontend and an ai-bridge Node layer, that wraps coding CLIs such as Claude Code, OpenAI Codex, Grok CLI, Kimi CLI and OpenCode in an in-IDE chat panel. It adds @file references, image input, diff review of edits, permission modes, session history and MCP server support.

- **+** Supports several CLIs (Claude Code, Codex, Grok, Kimi, OpenCode) from one panel
- **+** Permission modes with per-command allow/deny and a diff view for edits
- **+** Searchable session history with favorites, export and usage statistics
- **+** Provider management is compatible with cc-switch
- **−** Tied to JetBrains IDEs; no VS Code or standalone version
- **−** Needs the underlying CLIs and their accounts or API keys separately
- **−** Built plugin package is about 40MB
- **−** macOS scrolling can lag unless JCEF GPU acceleration is disabled

<sub>no GPU · Docker · Needs IntelliJ IDEA / JetBrains IDE, Node.js (ai-bridge), Claude Code or other supported coding CLIs · Models: Claude Code, OpenAI Codex, Grok CLI, Kimi CLI, OpenCode · [Repo](https://github.com/zhukunpenglinyutong/jetbrains-cc-gui) · [🌐 Site ↗](https://plugins.jetbrains.com/plugin/29342-cc-gui-claude-or-codex-) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jetbrains-cc-gui/)</sub>

<a name="reverse-api-engineer"></a>
### #&#8288;119 [reverse-api-engineer](https://github.com/kalil0321/reverse-api-engineer) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Nov 2026</sub>

**CLI that captures site traffic and generates typed API clients from it.**

Reverse API Engineer records a website's network traffic to a HAR file, either while you browse or while an AI agent drives the browser. A configured model then reads the traffic and writes an API client in Python, JavaScript, TypeScript, Go, Java, C#, PHP, Ruby, C or PowerShell. It also ships a skill for Claude Code, Codex, Cursor and OpenCode, plus scriptable subcommands with JSON output.

- **+** Generates clients in 10 languages from captured HAR traffic
- **+** Manual, agent, engineer and collector modes cover different capture workflows
- **+** Scriptable subcommands with --json output and documented exit codes
- **+** Works with Claude, OpenCode, Cursor and Copilot SDKs, plus Ollama via OpenCode
- **−** Agent mode needs an API key; RAM and GPU needs are unknown
- **−** Chrome-mcp runs save no HAR, so engineer cannot regenerate them
- **−** Sites with aggressive bot detection may block capture
- **−** No Intel macOS or 32-bit Windows support; generated code needs review before running

<sub>no GPU · Needs Python 3.11+, Node.js 20+ (npx), Playwright Chromium (manual mode), Chrome 146+ (chrome-mcp headed), Claude, OpenCode, Cursor or Copilot SDK · Models: Claude Sonnet, Claude Opus, Claude Haiku, OpenCode providers, Ollama · [Repo](https://github.com/kalil0321/reverse-api-engineer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reverse-api-engineer/)</sub>

<a name="openharness"></a>
### #&#8288;120 [openharness](https://github.com/autonomous-ai/openharness) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

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

<a name="tianshu-harness"></a>
### #&#8288;121 [tianshu-harness](https://github.com/huiliyi37/tianshu-harness) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Oct 2026</sub>

**Terminal coding agent runtime with task contracts and evidence-gated delivery.**

Tianshu Harness is a TypeScript coding-agent runtime with a terminal TUI, a desktop app and a VS Code extension sharing one core. A supervision layer called CVM keeps a per-task contract and runs 75 hook modules across five turn phases. A deliver_task gate reports RED, YELLOW or GREEN based on verification evidence. It ships 25 provider presets plus OpenAI-compatible endpoints, and is built around prefix caching.

- **+** Per-task TaskContract held by the runtime, so goals do not depend on chat history
- **+** Delivery gate separates commit, targeted tests (run_tests) and independent review (review_changes)
- **+** 25 provider presets plus any OpenAI-compatible endpoint such as Ollama or vLLM
- **+** Frozen-prefix cache design; README reports 99.3-99.6% hit rate on 5 DeepSeek sessions
- **−** CLI requires Node 24.22.1+ or 26.12.1+; other versions are rejected at startup
- **−** Repo is a synced projection; desktop app and some advanced code are not included
- **−** Published cache and A/B results cover mainly DeepSeek; the behavior pilot is 5 tasks, one model
- **−** README and most docs are in Chinese; the English README is a separate file

<sub>no GPU · Needs Node.js 24.22.1+ or 26.12.1+ (CLI), LLM provider API key or OpenAI-compatible endpoint · Models: DeepSeek, Claude, Codex (GPT), Gemini, GLM · [Repo](https://github.com/huiliyi37/tianshu-harness) · [📖 Docs ↗](https://github.com/huiliyi37/tianshu-harness/blob/main/docs/user-guide.md) · [🌐 Site ↗](https://tianshuharness.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tianshu-harness/)</sub>

<a name="bernstein"></a>
### #&#8288;122 [bernstein](https://github.com/sipyourdrink-ltd/bernstein) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**Deterministic orchestrator that runs CLI coding agents in parallel git worktrees.**

Bernstein is a Python CLI that decomposes a goal into tasks with one LLM call, then schedules them with plain Python rather than a model. Each coding task runs in its own git worktree behind merge gates, using Claude Code, Codex, Gemini CLI or 50+ other CLI agent adapters. Runs are recorded in a replay journal and lineage spine, with optional HMAC-chained audit logs and signed receipts that can be verified offline. The README marks it beta and solo-maintained.

- **+** Scheduler is plain Python with no LLM in the coordination loop, so plans replay
- **+** Signed run receipts verify offline with `bernstein verify receipt` and a pinned public key
- **+** 50+ CLI agent adapters plus a generic `--prompt` wrapper
- **+** File-based state under `.sdd/`, no SaaS hop or third-party data plane
- **−** Marked beta and solo-maintained; minor versions may change interfaces
- **−** Needs a separately installed and authenticated CLI agent; `bernstein doctor` checks this
- **−** HMAC audit chain is opt-in via `BERNSTEIN_AUDIT=1` or `--audit`
- **−** Stricter filesystem isolation is opt-in; with worktrees disabled, tasks share one checkout

<sub>no GPU · Docker + Compose · Needs git, a CLI coding agent (Claude Code, Codex, Gemini CLI, etc.), Python 3.12+ · Models: Claude Code, Codex, Gemini CLI, 50+ CLI agent adapters · [Repo](https://github.com/sipyourdrink-ltd/bernstein) · [📖 Docs ↗](https://docs.bernstein.run/) · [🌐 Site ↗](https://bernstein.run) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bernstein/)</sub>

<a name="anus"></a>
### #&#8288;123 [anus](https://github.com/anus-dev/anus) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Nov 2026</sub>

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

<a name="desktop-cc-gui"></a>
### #&#8288;124 [desktop-cc-gui](https://github.com/zhukunpenglinyutong/desktop-cc-gui) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

**Desktop GUI for Claude Code, Codex CLI and nine other coding CLIs.**

ccgui is a Tauri 2, React and Rust desktop app that puts eleven command-line coding agents (Claude Code, Codex CLI, Kimi, Grok, OpenCode, Qoder, MiniMax Code and others) behind one chat interface. Each engine has its own protocol adapter in the Rust backend. The app adds a file tree, PTY terminal, Git panel, provider-channel config and a plugin SDK, with installers for macOS, Windows and Linux.

- **+** Eleven engines in one UI, each with a dedicated Rust protocol adapter
- **+** Writes provider channels to each CLI's native config; CC Switch import for Claude, Codex, Grok
- **+** Built-in file tree, PTY terminal, Git panel and CodeMirror editor
- **+** Installers for macOS (aarch64), Windows (NSIS) and Linux (AppImage, rpm)
- **−** Needs the underlying CLIs installed and configured separately; not a standalone agent
- **−** Feature support varies by engine; team mode is unsupported on all of them
- **−** MiniMax Code has no provider channels or MCP/Skills sync yet
- **−** Only a macOS Apple Silicon installer is listed; no Intel macOS build

<sub>no GPU · Needs Supported engine CLIs (Claude Code, Codex CLI, etc.), Node.js 22.13+ and pnpm 10 (build from source), Rust stable (build from source) · Models: Claude Code, Codex CLI, Kimi CLI, Grok CLI, Pi CLI · port 1420 · [Repo](https://github.com/zhukunpenglinyutong/desktop-cc-gui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/desktop-cc-gui/)</sub>

<a name="nimbalyst"></a>
### #&#8288;125 [nimbalyst](https://github.com/nimbalyst/nimbalyst) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Nov 2026</sub>

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

<a name="chorus"></a>
### #&#8288;126 [chorus](https://github.com/chorus-aidlc/chorus) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · AGPL-3.0 · Nov 2026</sub>

**Coordinates teams of coding agents and humans through an idea-to-task pipeline.**

Chorus is a Next.js server that runs an AI-DLC workflow: agents draft proposals, documents and task DAGs, and humans review before work executes. It tracks session lifecycle and task state, applies per-agent permissions, and connects clients such as Claude Code, Codex, Kiro, Pi and Hermes over MCP. It starts locally with embedded PGlite and can move to external PostgreSQL.

- **+** Two-command local start with embedded PGlite, no Docker or database setup
- **+** Fine-grained, configurable permissions per agent and human, with no fixed roles
- **+** Connects many agent clients over MCP, with a setup wizard in Settings
- **+** Optional daemon wakes local agents on assigned tasks, with live Kanban and graph views
- **−** AGPL-3.0 license restricts closed-source hosted or modified use
- **−** Quick Start pins npm version 0.21.0 while the README lists v0.24.0
- **−** Orchestrates other agents; it does not write code itself
- **−** Multi-agent or production use needs external PostgreSQL, Docker or AWS setup

<sub>no GPU · Docker + Compose · Needs PostgreSQL 17 (embedded PGlite by default), Redis 7 (optional) · port 8637 · [Repo](https://github.com/chorus-aidlc/chorus) · [📖 Docs ↗](https://doc.chorus-ai.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chorus/)</sub>

<a name="screenshot-to-code"></a>
### #&#8288;127 [screenshot-to-code](https://github.com/abi/screenshot-to-code) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 81k · MIT · Nov 2026</sub>

**Turns screenshots, mockups and screen recordings into HTML, React or Vue code.**

A React/Vite frontend and FastAPI backend that send a screenshot, Figma design or screen recording to a vision model and return code in HTML+Tailwind, HTML+CSS, React+Tailwind, Vue+Tailwind, Bootstrap or Ionic+Tailwind. It needs at least one OpenAI, Anthropic or Gemini key, and optionally uses Replicate for image generation and editing. A hosted version is also available.

- **+** Supports six output stacks, including React, Vue, Bootstrap and Ionic with Tailwind
- **+** Accepts screen recordings as input, not just static screenshots (video mode needs Gemini)
- **+** Works with OpenAI, Anthropic or Gemini keys and picks a model mix by available keys
- **+** Optional headless Chromium preview lets the agent check its own rendered page
- **−** Needs paid third-party API keys; Ollama local models are described as poor quality
- **−** Asset extraction, video mode and image editing need Gemini and Replicate keys beyond one provider
- **−** Docker setup does not rebuild on file changes, so it is unsuitable for development
- **−** No tagged releases; manual setup needs Poetry, pnpm and a Playwright Chromium install

<sub>no GPU · Compose · Needs OpenAI, Anthropic or Gemini API key, Replicate API key (recommended), Playwright Chromium (optional), Poetry, pnpm · Models: GPT-5.5, GPT-5.4 Mini, Claude Opus, Gemini 3 Flash, Gemini 3.1 Pro · port 5173 · [Repo](https://github.com/abi/screenshot-to-code) · [▶️ Demo ↗](https://screenshottocode.com) · [🌐 Site ↗](https://screenshottocode.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/screenshot-to-code/)</sub>

<a name="opencursor"></a>
### #&#8288;128 [opencursor](https://github.com/pawanosman/opencursor) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

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

<a name="omnirush-gui"></a>
### #&#8288;129 [omnirush-gui](https://github.com/omnirush-ai/omnirush-gui) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · custom license · Nov 2026</sub>

**Desktop coding agent app for macOS and Linux, backed by an omnirush.ai account.**

Electron-style desktop app (TypeScript) that runs a coding agent against your local projects. It uses models from your omnirush.ai account, with GPT 6 Astra as default and a per-chat model and effort picker. It handles git and gh workflows, skills, and local MCP servers, with approval prompts for write and destructive commands.

- **+** Git workflows built in: clone, branch, worktrees, commit, push, and PRs via gh
- **+** Approval prompts: write commands ask once per session, destructive ones always ask
- **+** Packages for macOS arm64 and Linux x64/arm64: deb, rpm, pacman, AppImage, tar.gz
- **+** Releases ship SHA256SUMS.txt and the app updates itself in place on most installs
- **−** Requires an omnirush.ai account sign-in; prompts do not run without one
- **−** Your own provider keys are not supported, so no local or self-hosted models
- **−** Remote and account-linked MCP servers are not supported; only a fixed local list
- **−** No Intel Mac or Windows build; macOS builds are not notarized

<sub>no GPU · Needs omnirush.ai account, gh (for pull request workflows) · Models: GPT 6 Astra, GPT 6.1 Sol, models in omnirush.ai account catalog · [Repo](https://github.com/omnirush-ai/omnirush-gui) · [🌐 Site ↗](https://omnirush.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omnirush-gui/)</sub>

<a name="abtop"></a>
### #&#8288;130 [abtop](https://github.com/graykode/abtop) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Sep 2026</sub>

**btop-style terminal monitor for Claude Code, Codex CLI and OpenCode sessions.**

abtop is a Rust TUI that discovers running Claude Code, Codex CLI and OpenCode sessions from local process and file state. It shows per-session token usage, context window %, rate limits, git status, child processes and open ports, and can kill orphaned ports. It also offers a `--json` snapshot and a library crate for scripts and other local tools.

- **+** Read-only; needs no API keys or auth, reads local files and process metadata
- **+** Tracks Claude Code, Codex CLI and OpenCode in one view on macOS, Linux and Windows
- **+** `--json` output and a Rust library crate let other tools reuse the data
- **+** Enter jumps to an agent's terminal pane; orphan ports can be killed with one key
- **−** OpenCode lacks context %, current task and rate limit data; Codex lacks subagents
- **−** OpenCode monitoring requires the `sqlite3` CLI on PATH
- **−** Terminal jump supports only cmux, tmux and iTerm2 (iTerm2 on macOS)
- **−** Session summaries call `claude --print`, which makes an API call on your quota

<sub>no GPU · Needs sqlite3 (for OpenCode sessions), tmux, cmux or iTerm2 (optional, terminal jump) · [Repo](https://github.com/graykode/abtop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/abtop/)</sub>

<a name="zeron"></a>
### #&#8288;131 [zeron](https://github.com/zeronsh/zeron) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Nov 2026</sub>

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

<a name="claude-codex-bridge"></a>
### #&#8288;132 [claude_codex_bridge](https://github.com/seemseam/claude_codex_bridge) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · custom license · Nov 2026</sub>

**Terminal workspace that runs and links Codex, Claude, Gemini and other coding CLIs.**

CCB opens a terminal workspace where several coding CLI agents (Codex, Claude, Gemini, OpenCode, Kimi and others, 16 families listed) run in visible panes. Agents delegate to each other with /ask, using per-agent FIFO message queues, and a background daemon keeps project state alive. Layout is set in .ccb/ccb.config or a local config UI, and an Android app can control projects remotely.

- **+** Supports 16 CLI agent families in one workspace, with direct takeover of any pane
- **+** Per-agent FIFO queues keep returned results from interrupting a running turn
- **+** Daemon keeps project state alive after the foreground UI closes
- **+** Android app offers voice input, file transfer and terminal access; gateway binds to loopback by default
- **−** Draft protection in message queues is tested mainly with Claude, Codex and OMP in tmux
- **−** Queue deadline clearing uses Ctrl-C and can still interrupt simultaneous typing
- **−** Windows support is beta with unsigned binaries; ccb update is diagnostic-only there
- **−** License is reported as NOASSERTION, so reuse terms need checking

<sub>no GPU · Needs npm, tmux, Provider CLIs (Codex, Claude, Gemini, etc.), WezTerm (rich mode, Windows), Tailscale (remote mobile access), Python 3.10+ (Windows beta), Herdr 0.8.0+ (Windows beta) · Models: Codex, Claude, Gemini, OpenCode, Kimi · [Repo](https://github.com/seemseam/claude_codex_bridge) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-codex-bridge/)</sub>

<a name="echobird"></a>
### #&#8288;133 [echobird](https://github.com/edison7009/echobird) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Nov 2026</sub>

**Desktop app that installs coding CLIs and switches their models.**

EchoBird is a Tauri and Rust desktop app that installs coding tools such as Claude Code, Codex CLI, Aider and OpenCode, and rewrites each tool's native config file to switch models. It includes a Smart Router that puts up to 20 model APIs behind one local endpoint with priority-ordered failover, multi-account switching with quota display, and bundled vLLM, SGLang and llama.cpp runtimes. Desktop source is public only through v6.4.9.

- **+** Writes native tool config files, so model switching needs no manual TOML or JSON editing
- **+** Smart Router serves OpenAI Chat Completions and Anthropic Messages with ordered failover
- **+** Saved ChatGPT, Codex CLI and Claude Code accounts with 5-hour and 7-day quota view
- **+** Builds for Windows, macOS (Apple Silicon) and Linux x64/arm64
- **−** Desktop source after v6.4.9 is private; repo holds site, docs and releases
- **−** Smart Router lacks the Responses API, so Codex CLI third-party models cannot use it
- **−** Router follows fixed priority only and does not rotate saved login accounts
- **−** README carries sponsor API reseller promotions; the install path pipes a script to shell

<sub>GPU optional · Models: OpenAI, Anthropic, vLLM, SGLang, llama.cpp · [Repo](https://github.com/edison7009/echobird) · [🌐 Site ↗](https://echobird.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/echobird/)</sub>

<a name="background-agents"></a>
### #&#8288;134 [Background Agents](https://github.com/open-inspect/background-agents) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Nov 2026</sub>

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

<sub>no GPU · Compose · Needs Cloudflare Workers, Cloudflare Durable Objects, Cloudflare D1, GitHub App, Modal, Daytona, E2B or Vercel Sandbox · Models: Anthropic Claude, OpenAI Codex (ChatGPT subscription), xAI Grok (SuperGrok), OpenCode Zen and Go, Z.AI Coding Plan · [Repo](https://github.com/open-inspect/background-agents) · [📖 Docs ↗](https://github.com/open-inspect/background-agents/blob/main/docs/GETTING_STARTED.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/background-agents/)</sub>

<a name="tau"></a>
### #&#8288;135 [tau](https://github.com/huggingface/tau) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Nov 2026</sub>

**Python terminal coding agent with a small, layered, readable codebase.**

Tau is a terminal coding agent that reads files, edits code and runs shell commands from a Textual TUI or a one-shot print mode. Sessions are stored as append-only JSONL under ~/.tau/sessions/. The code is split into three packages (tau_ai, tau_agent, tau_coding), so the agent harness can be reused as a library. It is also written as a teaching example of how coding agents are built.

- **+** Three-layer split lets the tau_agent harness run without the CLI or TUI
- **+** Durable JSONL sessions with resume, branching and compaction
- **+** Supports OpenAI, Anthropic, OpenRouter, Hugging Face and OpenAI-compatible endpoints
- **+** Reads AGENTS.md, .tau/ and .agents/ resources; supports skills and prompt templates
- **−** Only four built-in tools: read, write, edit and bash
- **−** README says it is under active development
- **−** Requires Python 3.12 or newer

<sub>no GPU · Needs Python 3.12+, uv (installed by the install script), model provider account or endpoint · Models: OpenAI, Anthropic, OpenAI Codex subscription, OpenRouter, Hugging Face · [Repo](https://github.com/huggingface/tau) · [📖 Docs ↗](https://twotimespi.dev/quickstart/) · [🌐 Site ↗](https://twotimespi.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tau/)</sub>

<a name="agentsmesh"></a>
### #&#8288;136 [agentsmesh](https://github.com/agentsmesh/agentsmesh) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (46) · Freshness: active (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · custom license · Sep 2026</sub>

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

<sub>no GPU · Needs PostgreSQL, Redis, MinIO, Traefik, Docker · Models: Claude Code, Codex CLI, Gemini CLI, Aider, OpenCode · port 3000 · [Repo](https://github.com/agentsmesh/agentsmesh) · [📖 Docs ↗](https://agentsmesh.ai/docs) · [🌐 Site ↗](https://agentsmesh.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentsmesh/)</sub>

<a name="opencode-telegram-bot"></a>
### #&#8288;137 [opencode-telegram-bot](https://github.com/grinev/opencode-telegram-bot) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

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

<a name="kandev"></a>
### #&#8288;138 [kandev](https://github.com/kdlbs/kandev) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · AGPL-3.0 · Nov 2026</sub>

**Kanban board that runs coding agent CLIs in parallel git worktrees.**

Kandev is a Go server with an embedded web UI that manages tasks on kanban or pipeline views and runs coding agent CLIs (Claude Code, Codex, Copilot, Gemini CLI and others) against them in parallel. Each task gets its own git worktree, and output is reviewed in a workspace with an editor, terminal, browser preview and git changes panel. Agents can run locally, in Docker, over SSH, in Kubernetes Pods or on sprites.dev.

- **+** Supports 20+ agent CLIs, mostly via ACP, and can mix agents per workflow step
- **+** Git worktrees isolate concurrent tasks; multi-repo tasks get one worktree per repo
- **+** Executors include local, Docker, SSH, Kubernetes and sprites.dev, with reusable profiles
- **+** Native Go binary with embedded frontend and SQLite; installs via Homebrew, Scoop or npx
- **−** AGPL-3.0 license may restrict use in proprietary or hosted products
- **−** Office mode (persistent agent teams) is experimental and off by default
- **−** Agent CLIs must be installed separately; Cursor integration requires Cursor Pro
- **−** Orchestrates other agents rather than being one, so needs their accounts and keys

<sub>no GPU · Docker · Needs Agent CLIs (Claude Code, Codex, etc.), Docker (optional), Node.js (only for npx launch) · Models: Claude Code, Codex, GitHub Copilot, Gemini CLI, OpenCode · [Repo](https://github.com/kdlbs/kandev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kandev/)</sub>

<a name="ccpocket"></a>
### #&#8288;139 [ccpocket](https://github.com/k9i-0/ccpocket) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Mobile chat client for running Codex and Claude sessions on your own machine.**

CC Pocket is a Flutter app for iOS, Android, macOS, Linux and Windows that talks to a Node.js Bridge Server running on your own machine, which drives the Codex or Claude CLI. You start tasks, approve steps, browse files, review diffs and commit from the phone. Code stays on the host; the app connects by QR code, mDNS, manual ws:// URL or Tailscale.

- **+** Supports both Codex and Claude sessions, and can resume CLI sessions from the app
- **+** Includes file browser, code and image diffs, staging, commit, push and git worktrees
- **+** Queues outgoing messages offline and recovers missed streaming updates after reconnect
- **+** MIT licensed, with Bridge sync, approval flow and viewers designed to be reused in forks
- **−** Requires a separate always-on host with Node.js 22.19.0+ and an agent CLI installed
- **−** Linux and Windows desktop builds are experimental
- **−** Claude subscription auth needs explicit opt-in via BRIDGE_ALLOW_CLAUDE_OAUTH=1; API key is the default
- **−** On macOS the Bridge goes offline when the Mac sleeps

<sub>no GPU · Needs Node.js 22.19.0+, Codex CLI or Claude Code CLI, Tailscale (optional, for remote access), Flutter (for development) · Models: Codex, Claude · port 8765 · [Repo](https://github.com/k9i-0/ccpocket) · [📖 Docs ↗](https://k9i-0.github.io/ccpocket/architecture/) · [🌐 Site ↗](https://k9i-0.github.io/ccpocket/install/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ccpocket/)</sub>

<a name="claude-code-action"></a>
### #&#8288;140 [claude-code-action](https://github.com/anthropics/claude-code-action) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (78) · Freshness: recent (77) · Maintenance: fair (70) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Nov 2026</sub>

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

<a name="monocode"></a>
### #&#8288;141 [monocode](https://github.com/hardbeat920/monocode) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Nov 2026</sub>

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

<a name="little-coder"></a>
### #&#8288;142 [little-coder](https://github.com/itayinbarr/little-coder) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (50) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · Apache-2.0 · Sep 2026</sub>

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

<a name="holyclaude"></a>
### #&#8288;143 [holyclaude](https://github.com/coderluii/holyclaude) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

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
### #&#8288;144 [minimax-code](https://github.com/minimax-ai/minimax-code) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Nov 2026</sub>

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

<a name="zero"></a>
### #&#8288;145 [zero](https://github.com/twigpine/zero) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

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

<a name="zerostack"></a>
### #&#8288;146 [zerostack](https://github.com/gi-dellav/zerostack) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · GPL-3.0 · Nov 2026</sub>

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

<a name="aider-desk"></a>
### #&#8288;147 [aider-desk](https://github.com/hotovo/aider-desk) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Nov 2026</sub>

**Desktop app for steering AI coding agents with diff review and Git worktrees.**

AiderDesk is a TypeScript desktop app that began as a GUI for the Aider CLI and now includes its own agent mode. It organizes work into projects and tasks, gives each task an isolated Git worktree, and requires diff review and tool approval before changes or shell commands run. It connects to 30+ LLM providers, works as an MCP client and server, and supports TypeScript extensions.

- **+** Per-task Git worktrees keep AI experiments off the active local branch
- **+** Tool approval gates and diff review (side-by-side and unified) before changes apply
- **+** Extensions with 30+ lifecycle hooks, custom tools and React UI components
- **+** Chat history, task metadata and settings stored locally
- **−** README only points to Docker, npm, Homebrew and Scoop installs; steps are in external docs
- **−** Broad feature set means more setup than a plain CLI agent

<sub>Docker · Needs Aider CLI, LanceDB · Models: OpenAI, Anthropic, Gemini, DeepSeek, Ollama · [Repo](https://github.com/hotovo/aider-desk) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aider-desk/)</sub>

<a name="waveterm"></a>
### #&#8288;148 [waveterm](https://github.com/wavetermdev/waveterm) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (89) · Freshness: active (96) · Maintenance: patchy (37) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · Apache-2.0 · Oct 2026</sub>

**Cross-platform terminal with a built-in AI assistant and durable SSH sessions.**

Wave is a desktop terminal for macOS, Linux and Windows that puts terminals, a file editor, previews, a web browser and an AI chat in draggable blocks. Wave AI reads terminal output and can read, write and edit files with backups and user approval. It uses your own keys for OpenAI, Claude, Gemini or Azure, or local models through Ollama and LM Studio.

- **+** Works with OpenAI, Claude, Gemini, Azure, Ollama and LM Studio; no account required
- **+** SSH sessions reconnect automatically after network drops and Wave restarts
- **+** File edits by the AI keep automatic backups and need user approval
- **+** `wsh` CLI copies files between local and remote hosts and pipes output to the AI
- **−** AI command execution is listed as coming soon, so it cannot run commands yet
- **−** Desktop app only; no Docker image or web deployment
- **−** Included AI credits are a free beta, with terms after the beta unknown
- **−** Requires glibc 2.28 or later on Linux, and macOS 11 or later

<sub>Models: OpenAI, Claude, Gemini, Azure, Perplexity · [Repo](https://github.com/wavetermdev/waveterm) · [📖 Docs ↗](https://docs.waveterm.dev) · [🌐 Site ↗](https://www.waveterm.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/waveterm/)</sub>

<a name="mitosis"></a>
### #&#8288;149 [mitosis](https://github.com/builderio/mitosis) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**Compiler that turns one component source into React, Vue, Angular, Svelte and more.**

Mitosis compiles components written once in a JSX-like syntax into native code for React, Vue, Angular, Svelte, Solid, Alpine, Qwik and other frameworks. It is aimed at design systems that must ship across frameworks, and it includes a Figma integration for syncing design components to code. Projects are scaffolded with `npm create @builder.io/mitosis@latest`, and a browser playground is available.

- **+** Emits native framework code instead of wrapping web components
- **+** Targets React, Vue, Angular, Svelte, Solid, Alpine and Qwik from one source
- **+** Figma integration to sync design system components into code
- **+** Online playground and npm scaffolding command for quick trials
- **−** Not an AI tool; fit in this list is loose, only design-to-code overlaps
- **−** Components must be written in Mitosis syntax, which limits framework-specific features

<sub>no GPU · Needs Node.js, npm · [Repo](https://github.com/builderio/mitosis) · [▶️ Demo ↗](https://mitosis.builder.io/playground) · [📖 Docs ↗](https://mitosis.builder.io/docs) · [🌐 Site ↗](https://mitosis.builder.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mitosis/)</sub>

<a name="genericagent"></a>
### #&#8288;150 [genericagent](https://github.com/lsdefine/genericagent) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**Minimal Python agent that controls browser, terminal and files, and saves skills.**

GenericAgent is a Python agent framework with a roughly 100-line agent loop and 9 atomic tools (code execution, file read/write/patch, web scan, browser JS, ask-user, two memory tools). It drives a real Chrome session through a local WebSocket server and extension, plus keyboard/mouse, screen vision and ADB. Finished tasks are written into a layered memory (L0-L4) as reusable skills. Frontends are a terminal UI, a Streamlit UI, and Telegram, Discord and Lark bots.

- **+** Core is about 3K lines; base install needs only requests plus four small packages
- **+** Uses a real persistent Chrome session, keeping logins; README reports passing several bot-detection tests
- **+** Layered memory turns finished tasks into reusable skills; README claims under 30K context
- **+** Terminal, Streamlit, Telegram, Discord and Lark frontends; Claude, Gemini, Kimi, MiniMax supported
- **−** Gives an LLM broad control of the local machine, including code execution and input
- **−** Python 3.14 is incompatible; README requires 3.11 or 3.12
- **−** Pre-installed SOPs are written in Chinese and were tuned on Windows
- **−** OCR, vision and computer use need agent-driven setup; web tools need a manual extension install

<sub>no GPU · Needs Python 3.11 or 3.12, Chrome/Chromium with bundled extension, LLM API key · Models: Claude, Gemini, Kimi, MiniMax · [Repo](https://github.com/lsdefine/genericagent) · [📖 Docs ↗](https://github.com/lsdefine/GenericAgent/blob/main/docs/installation.md) · [🌐 Site ↗](https://gaagent.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/genericagent/)</sub>

<a name="ante"></a>
### #&#8288;151 [ante](https://github.com/antigmalabs/ante) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

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

<a name="corecoder"></a>
### #&#8288;152 [corecoder](https://github.com/he-yufeng/corecoder) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

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

<a name="cloudroom"></a>
### #&#8288;153 [cloudroom](https://github.com/davidondrej/cloudroom) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Nov 2026</sub>

**Runs Claude Code, Codex, and other coding agent CLIs in cloud sandboxes.**

Cloudroom runs coding agent harnesses (Claude Code, Codex, Pi, OpenCode and others) as their own CLIs, each in an isolated sandbox on its own Git branch. A Rust core service handles the sandbox, process, queue, recorded history and recovery, and a desktop app built on BB connects to it. Running sessions can be teleported between a Mac and the cloud with the same chat, model and effort.

- **+** Supports 7 harnesses over 4 native protocols, each keeping its own agent loop and login
- **+** Teleport moves a running session between Mac and cloud, preserving chat, model and effort
- **+** Self-hostable Rust core with documented HTTP API, installable via script on Ubuntu 24.04
- **+** One sandbox and Git branch per agent thread
- **−** Agents run without approval prompts; README advises one machine per trusted user
- **−** Self-host install script officially targets Ubuntu 24.04 only
- **−** Building the core needs Rust 1.89+; desktop app is a separate build
- **−** API listens only on localhost unless you put it behind HTTPS yourself

<sub>no GPU · Needs Rust 1.89+ (build from source), Ubuntu 24.04 (self-host install script) · Models: Claude Code, Codex, Pi, OpenCode · [Repo](https://github.com/davidondrej/cloudroom) · [📖 Docs ↗](https://github.com/davidondrej/cloudroom/blob/main/core/docs/setup.md) · [🌐 Site ↗](https://www.cloudroom.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloudroom/)</sub>

<a name="opencove"></a>
### #&#8288;154 [opencove](https://github.com/deadwavewave/opencove) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (37) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Nov 2026</sub>

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

<a name="pideck"></a>
### #&#8288;155 [pideck](https://github.com/ayuayue/pideck) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Electron desktop app for managing pi, DSH and ACP coding agent sessions.**

PiDeck is an Electron and TypeScript desktop shell that runs one `pi --mode rpc` process per session across multiple local projects. It also embeds the DeepSeek Harness (DSH) host and acts as an ACP client for external agent CLIs, with 15 presets. It adds a file tree, Git panel, built-in terminal, visual editing of pi's models.json, auth.json and settings.json, and import of Codex and Claude sessions.

- **+** One window for pi, DSH and ACP sessions, with 15 ACP CLI presets such as Gemini CLI and Codex CLI
- **+** Does not fork pi: sessions and tools stay native, communicating over stdio JSON-RPC
- **+** Edits pi config files visually and tests provider connections
- **+** Ships Windows, macOS and Linux installers, plus a LAN web UI for phone clients
- **−** Requires a separately installed `pi` CLI on PATH with providers already configured
- **−** README labels the project experimental
- **−** Sends anonymous heartbeat usage stats by default; opt-out is in settings
- **−** README mixes in unrelated promotion (reseller shop, sponsor QR codes) and is mostly in Chinese

<sub>no GPU · Needs pi CLI, Node.js 20+ (source builds), npm · Models: pi providers via models.json, DeepSeek models (DSH), ACP CLIs (Gemini, Claude, Codex, Kimi, Qwen, etc.), OpenAI-compatible image generation · [Repo](https://github.com/ayuayue/pideck) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pideck/)</sub>

<a name="sidecar"></a>
### #&#8288;156 [sidecar](https://github.com/marcus/sidecar) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Oct 2026</sub>

**Terminal workspace for running coding agents beside git, files and tasks.**

Sidecar is a Go terminal UI that hosts coding agents (Claude Code, Codex, Gemini, Cursor, OpenCode, Pi) in embedded tmux-backed terminals. Split panes show git diffs, a file browser, td task issues, and Jira or GitHub resources next to the agent. It also manages git worktrees, a cross-project Sessions screen, and CLI commands for opening panes, layouts and notifications.

- **+** Hosts several agents (Claude, Codex, Gemini, Cursor, OpenCode, Pi) in one shell
- **+** Sessions screen shows agent status across all configured projects
- **+** Agents can drive panes via `sidecar open`, `layout` and `notify post`
- **+** Runs locally with no telemetry; only GitHub version checks
- **−** Terminal UI only; setup checks expect tmux and truecolor support
- **−** Jira and GitHub panes need separate add-on executables
- **−** Task view depends on the author's separate td tool
- **−** Supports macOS, Linux or WSL only; no native Windows

<sub>no GPU · Needs tmux, td (optional), sidecar-jira (optional), sidecar-github (optional), Go 1.26+ (build from source) · [Repo](https://github.com/marcus/sidecar) · [📖 Docs ↗](https://marcus.github.io/sidecar/docs/intro) · [🌐 Site ↗](https://marcus.github.io/sidecar/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sidecar/)</sub>

<a name="repoprompt-ce"></a>
### #&#8288;157 [repoprompt-ce](https://github.com/repoprompt/repoprompt-ce) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 998 · Apache-2.0 · Nov 2026</sub>

**Native macOS app that builds code context and orchestrates CLI coding agents.**

RepoPrompt CE is a Swift macOS app that assembles prompts from selected files, CodeMaps, file trees and Git diffs, then hands them to AI models or CLI agents. It also ships an MCP server so external MCP clients can search repos, curate context and run agent sessions. Worktrees are managed by the app, and workspaces can span multiple roots.

- **+** Context Builder lets an agent pick relevant files within a token budget
- **+** Bundled MCP server exposes repo search and context curation to external clients
- **+** Multi-root workspaces and app-managed worktrees with .worktreeinclude file copying
- **+** Installable as a signed, notarized app via a Homebrew cask
- **−** Requires macOS 26 or later; no Linux or Windows support
- **−** Building from source needs full Xcode 26 and Python 3
- **−** Ad-hoc debug builds do not persist saved API keys across launches
- **−** Local production build is self-signed, not notarized, and not redistributable

<sub>no GPU · Needs macOS 26+, Xcode 26 (source builds), Python 3 (launcher scripts), Homebrew (optional install) · Models: unknown · [Repo](https://github.com/repoprompt/repoprompt-ce) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repoprompt-ce/)</sub>

<a name="wegent"></a>
### #&#8288;158 [wegent](https://github.com/wecode-ai/wegent) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 894 · Apache-2.0 · Nov 2026</sub>

**Issue-based workspace where team members and AI agents share tasks and deliverables.**

Wegent ties people, AI agents and personal stand-ins to the same Issue, with linked tasks, discussion and deliverables kept together. It ships an Electron desktop app (Wework) that drives Codex on local projects with diffs and test output, plus a self-hosted Next.js web app and Backend for shared projects, models, knowledge and remote executors.

- **+** Desktop app runs local coding tasks without Backend login, showing diffs, commands and test results
- **+** Tracks assignment, execution, discussion and deliverables per Issue across members and agents
- **+** Tasks can run locally, on remote work machines, or on server-managed executors
- **+** One-line standalone install script serves the web app on port 3000
- **−** Large multi-service monorepo (Python, Rust, TypeScript), heavy to self-host and modify
- **−** Personal stand-ins are Beta and need source authorization, a model and an execution device
- **−** AI lead conversations require experimental features to be enabled
- **−** Local coding path is built around Codex; other agent runtimes are not described

<sub>Docker + Compose · Needs Docker (self-hosting), Node.js 22.15+ and pnpm (development) · port 3000 · [Repo](https://github.com/wecode-ai/wegent) · [📖 Docs ↗](https://wecode-ai.github.io/wegent-docs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wegent/)</sub>

<a name="twinny"></a>
### #&#8288;159 [twinny](https://github.com/twinnydotdev/twinny) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Nov 2026</sub>

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

<a name="tmuxai"></a>
### #&#8288;160 [tmuxai](https://github.com/alvinunreal/tmuxai) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="waku"></a>
### #&#8288;161 [waku](https://github.com/egoist/waku) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · GPL-3.0 · Oct 2026</sub>

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

<a name="jean"></a>
### #&#8288;162 [jean](https://github.com/coollabsio/jean) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Nov 2026</sub>

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

<a name="optio"></a>
### #&#8288;163 [optio](https://github.com/jonwiggins/optio) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Orchestrates coding agents on Kubernetes or your own machines, with mobile apps.**

Optio runs coding agents (Claude Code, Codex, Copilot, Gemini, Cursor, OpenCode and others) as tasks in Kubernetes pods or on paired local machines. Work starts from a prompt, a schedule, or one of fifteen trigger types such as GitHub, Slack, PagerDuty or webhooks, and issue-to-PR runs follow CI and review. It has a web UI, native iOS and Android clients, and a Helm chart for production.

- **+** Supports eight agent runtimes plus plain shell commands, chosen per piece of work
- **+** Fifteen trigger types including GitHub, GitLab, Slack, Linear, Jira, PagerDuty, Sentry, Jenkins
- **+** Helm chart with managed Postgres/Redis, existing Secrets, and horizontally scaled API replicas
- **+** Native SwiftUI iOS and Jetpack Compose Android apps with widgets and notifications
- **−** Requires Kubernetes, even for the local setup via Docker Desktop
- **−** Pods in the same pool are mutually trusted; not a boundary for hostile tenants
- **−** Shared sessions expose the session's credentials and environment to collaborators
- **−** Agents still call external model providers; self-hosting does not make them local

<sub>no GPU · Docker + Compose · Needs Kubernetes, PostgreSQL, Redis · Models: Claude Code, OpenAI Codex, GitHub Copilot, Google Gemini, Cursor · port 30310 · [Repo](https://github.com/jonwiggins/optio) · [📖 Docs ↗](https://optio.host/docs/) · [🌐 Site ↗](https://optio.host) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/optio/)</sub>

<a name="wesight"></a>
### #&#8288;164 [wesight](https://github.com/freestylefly/wesight) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 976 · MIT · Nov 2026</sub>

**Electron desktop console for running local coding agent CLIs in one chat UI.**

WeSight is an Electron app (React, Redux Toolkit, SQLite) that installs or reuses local agent CLIs such as Claude Code, Codex, Kimi Code, OpenClaw, Hermes Agent, OpenCode, Qwen Code and DeepSeek-TUI, plus a built-in runtime. It adds a shared chat with tool and diff panels, one model-provider config, Feishu IM routing, a SkillHub marketplace, scheduled tasks, and a per-call runtime dashboard.

- **+** Supports nine engines, including Claude Code, Codex, OpenCode and Qwen Code, from one workspace
- **+** Runtime dashboard records engine, model, tokens, TTFT, TPS, tool latency and steps per call
- **+** Can reuse existing local CLI accounts and config or manage providers centrally, including Ollama
- **+** Signed and notarized macOS builds plus a Windows x64 installer; local data in SQLite
- **−** Windows installer is unsigned and triggers SmartScreen warnings
- **−** One-click CLI install is described only for macOS
- **−** IM routing is documented only for Feishu
- **−** Development requires Node.js >=24 <25; no Linux release is listed

<sub>no GPU · Needs Node.js >=24 <25 (development), npm, Local agent CLIs (optional) · Models: OpenAI, Anthropic Claude, Google Gemini, DeepSeek, Qwen · port 5175 · [Repo](https://github.com/freestylefly/wesight) · [🌐 Site ↗](https://wesight.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wesight/)</sub>

<a name="codeman"></a>
### #&#8288;165 [codeman](https://github.com/ark0n/codeman) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 852 · MIT · Nov 2026</sub>

**Web dashboard that runs and monitors AI coding CLIs in tmux sessions.**

Codeman spawns Claude Code, OpenCode, Codex, Gemini, Copilot CLI and other coding agents inside persistent tmux sessions and streams the terminal to a browser, including a touch-optimized mobile UI. It re-prompts idle agents, resumes after usage limits reset, and runs scheduled jobs. Sessions can run locally, in Docker or over SSH, and an MCP server lets one agent start others and collect their answers.

- **+** Supports eleven agent CLIs plus a plain shell, chosen per session
- **+** tmux persistence keeps agents running across restarts and network drops
- **+** Mobile terminal with local echo, QR login and push notifications
- **+** Loopback-only by default; optional multi-user mode and Tailscale exposure
- **−** Requires tmux, so Windows users must run it under WSL
- **−** Installer compiles node-pty from source on Linux, needing a build toolchain
- **−** Mac app does not self-update; the DMG must be replaced manually
- **−** Needs at least one agent CLI installed separately

<sub>no GPU · Docker + Compose · Needs Node.js 22+, tmux, at least one AI coding CLI · Models: Claude Code, OpenCode, Codex, Antigravity, Gemini CLI · port 3000 · [Repo](https://github.com/ark0n/codeman) · [📖 Docs ↗](https://github.com/Ark0N/Codeman/wiki/Installation) · [🌐 Site ↗](https://getcodeman.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeman/)</sub>

<a name="pilot"></a>
### #&#8288;166 [pilot](https://github.com/qf-studio/pilot) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 744 · custom license · Nov 2026</sub>

**Go daemon that turns labeled tickets into pull requests using Claude Code.**

Pilot polls GitHub, GitLab or Azure DevOps, or takes Linear, Jira and Asana webhooks, then runs Claude Code to plan, implement, test and open a PR for each ticket. It also accepts tasks over a Telegram bot and shows queue, cost and autopilot status in a terminal dashboard. Autopilot modes (dev, stage, prod) control CI waiting, auto-merge and human approval.

- **+** Takes tickets from GitHub, GitLab, Azure DevOps, Linear, Jira and Asana
- **+** Autopilot modes set CI waiting, auto-merge or human approval per environment
- **+** Budget limits with hard enforcement; token and cost metrics persisted in SQLite
- **+** Runs Claude Code via Anthropic key, Bedrock or Vertex; OpenCode backend also supported
- **−** Requires Claude Code CLI 2.1.17+; no standalone model runtime
- **−** BSL 1.1 license, not OSI open source; competing SaaS needs a license
- **−** README says it is not suited to large architectural or security-critical changes
- **−** Model routing is described only for Claude models; other providers unclear

<sub>no GPU · Docker + Compose · Needs Claude Code CLI 2.1.17+, GitHub token, Go 1.22+ (build only), SQLite, OpenAI API key (optional, voice transcription) · Models: Claude (Haiku, Opus 4.6), AWS Bedrock, Google Vertex AI, OpenCode backend · port 9090 · [Repo](https://github.com/qf-studio/pilot) · [📖 Docs ↗](https://docs.pilotcloud.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pilot/)</sub>

<a name="termio"></a>
### #&#8288;167 [termio](https://github.com/termio-sh/termio) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 669 · MIT · Nov 2026</sub>

**macOS terminal app that runs and monitors multiple CLI coding agents.**

Termio is a native macOS terminal (Swift) for running CLI coding agents such as Claude Code, Codex, OpenCode and Cursor side by side. It installs each agent's hooks to report working, idle or needs-you status, and keeps sessions alive in a daemon, termiod, so quitting the app only detaches. Sessions can run on a remote Linux host over SSH and be mirrored on an iPhone companion app.

- **+** Sessions persist in the termiod daemon, so closing the app does not kill agents
- **+** Per-agent hooks report working, idle or needs-you in sidebar, tray and phone
- **+** Remote sessions over SSH use ~/.ssh/config and one binary in ~/.local/bin
- **+** CLI (termio session spawn/send/read/watch) lets agents control sibling sessions
- **−** Desktop app is macOS 14+ only; Windows, Android, web and TUI clients are roadmap items
- **−** iPhone companion is a TestFlight beta
- **−** Does not run models itself; agent CLIs must be installed and configured separately
- **−** Changes pane is read-only; commit and push stay in the terminal

<sub>no GPU · Needs macOS 14+, Agent CLIs (Claude Code, Codex, etc.), SSH access to a Linux host (for remote use) · [Repo](https://github.com/termio-sh/termio) · [📖 Docs ↗](https://termio.sh/docs) · [🌐 Site ↗](https://termio.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/termio/)</sub>

<a name="golutra"></a>
### #&#8288;168 [golutra](https://github.com/golutra/golutra) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · custom license · Nov 2026</sub>

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

<a name="inferstep-atlas"></a>
### #&#8288;169 [inferstep/atlas](https://github.com/inferstep/atlas) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · AGPL-3.0 · Oct 2026</sub>

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
### #&#8288;170 [agent-shell](https://github.com/xenodium/agent-shell) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · GPL-3.0 · Nov 2026</sub>

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

<a name="ralphex"></a>
### #&#8288;171 [ralphex](https://github.com/umputun/ralphex) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (34) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

**CLI that runs Claude Code or codex through a markdown plan, with reviews.**

ralphex is a single Go binary run from a git repository root. It reads a markdown plan, executes each task in a fresh Claude Code or codex session, runs the plan's validation commands, and commits. It then runs a multi-agent review pipeline (5 agents, optional external codex review, 2 agents) and moves the finished plan to completed/.

- **+** Fresh session per task keeps context small during long plans
- **+** Review-only and external-only modes work on branches made outside ralphex
- **+** --worktree flag runs several plans in parallel on one repo
- **+** Optional web dashboard (--serve) and Telegram, Email, Slack, webhook notifications
- **−** Default mode uses claude --print, which falls under Anthropic's separate Agent SDK credit pool
- **−** Needs Claude Code or codex CLI installed; codex mode requires codex 0.130.0 or newer
- **−** Pause and manual break via Ctrl+\ are not available on Windows
- **−** Wrappers that avoid claude --print are unofficial and may break if Anthropic blocks them

<sub>no GPU · Docker + Compose · Needs Claude Code CLI or codex CLI, git · Models: Claude (via Claude Code), OpenAI codex (default gpt-5.6-sol), custom external review scripts · [Repo](https://github.com/umputun/ralphex) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralphex/)</sub>

<a name="thclaws"></a>
### #&#8288;172 [thclaws](https://github.com/thclaws/thclaws) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Nov 2026</sub>

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

<a name="parallel-code"></a>
### #&#8288;173 [parallel-code](https://github.com/johannesjo/parallel-code) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Desktop app that runs coding agents in parallel git worktrees.**

Electron and SolidJS desktop app that creates a branch and git worktree per task and starts a terminal coding agent in it. Claude Code, Codex, OpenCode, Copilot and Antigravity CLIs run side by side on one board sorted by what needs attention. A diff viewer sends inline comments back to the agent, and finishing a task merges the branch or pushes it for a PR.

- **+** Mixes agents from different vendors on one board, each using its own CLI login
- **+** Per-task branch and worktree, with optional per-project Docker sandbox
- **+** Built-in diff review with inline comments and optional second-model review
- **+** Phone UI via QR code over Wi-Fi or Tailscale, plus an Android app
- **−** Agents run locally only; nothing continues while the computer is off
- **−** Packaged builds for macOS and Linux only; Windows needs a source build
- **−** Requires at least one separate agent CLI installed and authenticated
- **−** Docker sandboxes are not available for Antigravity

<sub>no GPU · Docker · Needs git, Claude Code, Codex CLI, OpenCode, Copilot CLI or Antigravity CLI, Node.js 22.12+ (build from source), Docker (optional) · Models: Claude Code, Codex CLI, OpenCode, Copilot CLI, Antigravity CLI · port 7777 · [Repo](https://github.com/johannesjo/parallel-code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/parallel-code/)</sub>

<a name="hax"></a>
### #&#8288;174 [hax](https://github.com/oleksandrchekhovskyi/hax) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Terminal coding agent in C with first-class local model support.**

hax is a coding agent that runs in the terminal as a single native C binary. It talks to OpenAI, Anthropic, Codex, OpenRouter, DeepSeek, llama.cpp, Ollama and custom endpoints, and auto-discovers the model when pointed at a llama-server. It keeps native terminal scrollback, offers a transcript view (Ctrl+T) and optional wire traces, and deliberately omits MCP, plugins and permission prompts.

- **+** Single native binary using only a few MB of memory
- **+** Auto-discovers llama.cpp model and capabilities without a provider config block
- **+** Transcript view and optional wire trace show what was sent to the model
- **+** Clean stdout in -p one-shot mode; plain-text config and session files
- **−** No built-in MCP, plugin runtime or IDE panels by design
- **−** No per-command permission prompts
- **−** Windows only via WSL; BSDs build from source only
- **−** Web search and MCP need separate Python companion tools

<sub>no GPU · Needs libcurl, jansson, meson, ninja, pkg-config, fzf (optional) · Models: OpenAI, Anthropic, Codex, OpenRouter, OpenCode Zen/Go · [Repo](https://github.com/oleksandrchekhovskyi/hax) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hax/)</sub>

<a name="cyrus"></a>
### #&#8288;175 [cyrus](https://github.com/cyrusagents/cyrus) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 915 · Apache-2.0 · Nov 2026</sub>

**Turns issues assigned in Linear, GitHub, GitLab or Slack into coding agent runs.**

Cyrus watches issues assigned to it in Linear, GitHub, GitLab or Slack, creates an isolated Git worktree per issue, and runs a Claude Code, Codex, Cursor, Gemini or Opencode session on it. Agent activity is streamed back to Linear or GitHub, including dropdown selects and approvals. It is bring-your-own-keys and runs on a machine you control, with a free community self-hosted path and paid Pro/Team plans.

- **+** One Git worktree per issue keeps concurrent agent sessions isolated
- **+** Works with five agent runtimes: Claude Code, Codex, Cursor, Gemini, Opencode
- **+** Community option is fully self-hosted with your own Linear, GitHub and Slack apps
- **+** Guided /cyrus-setup skill handles onboarding; npm install for the paid path
- **−** Community setup requires creating your own Linear OAuth app, GitHub App and Slack App
- **−** Paid self-hosted mode relies on Cyrus cloud for networking and integrations
- **−** Requires your own model API keys or subscriptions
- **−** Needs a persistent process (tmux, pm2 or systemd) to keep running

<sub>no GPU · Needs Node.js/npm, Git, Linear, GitHub, GitLab or Slack account, GitHub or GitLab CLI for PRs/MRs, Cloudflare Tunnel (optional) · Models: Claude Code, Codex, Cursor, Gemini, Opencode · [Repo](https://github.com/cyrusagents/cyrus) · [📖 Docs ↗](https://github.com/cyrusagents/cyrus/blob/main/docs/SELF_HOSTING.md) · [🌐 Site ↗](https://app.atcyrus.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cyrus/)</sub>

<a name="grok-build"></a>
### #&#8288;176 [grok-build](https://github.com/xai-org/grok-build) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Sep 2026</sub>

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

<a name="gastown"></a>
### #&#8288;177 [gastown](https://github.com/gastownhall/gastown) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: weak (27) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

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

<a name="rune"></a>
### #&#8288;178 [rune](https://github.com/unstablebuild/rune) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · GPL-3.0 · Nov 2026</sub>

**Native GPU-rendered IDE and terminal multiplexer with a built-in agent.**

Rune is a native IDE and terminal multiplexer written in Go, rendering with OpenGL on Linux and Metal on macOS instead of Electron. It offers nine workspace slots, language intelligence for a documented list of languages, and a built-in agent or IDE skills for external agents. Rune instances connect over an end-to-end encrypted peer network built on headscale, and a headless node can serve workspaces to your other machines.

- **+** Native rendering pipeline (OpenGL on Linux, Metal on macOS), no Electron
- **+** Peer network lets you open remote workspaces via rune:// URLs
- **+** Headless node runs as a Docker container or a systemd, launchd, OpenRC or runit service
- **+** Packages install from official sources or directly from a Git repository
- **−** GPL-3.0 license may restrict embedding in proprietary products
- **−** Remote networking depends on the project's own headscale network
- **−** README lists only macOS and Linux install paths; Windows support unknown

<sub>Docker · Needs headscale network (hosted by project) · [Repo](https://github.com/unstablebuild/rune) · [📖 Docs ↗](https://docs.rune.build/) · [🌐 Site ↗](https://rune.build) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rune/)</sub>

<a name="maki"></a>
### #&#8288;179 [maki](https://github.com/tontinton/maki) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

**Terminal coding agent in Rust that minimizes context-window token use.**

Maki is a single-binary Rust coding agent with a ratatui TUI. It reduces token spend with a tree-sitter `index` tool for file skeletons, a sandboxed `code_execution` tool, deferred MCP tool loading, and subagents that return only summaries. It supports about 18 providers, Lua plugins, headless stream-json output compatible with Claude Code, and ACP for editors like Zed.

- **+** Context-saving tools: tree-sitter index, code_execution sandbox, deferred MCP tools via tool_search
- **+** Parses bash commands with tree-sitter so `git diff && rm -rf /` asks for both permissions
- **+** Many providers, including Ollama and llama.cpp for local models, plus custom OpenAI/Anthropic-compatible ones
- **+** Lua plugin system where builtin tools are plugins; hooks, headless mode and ACP supported
- **−** Rewind restores chat history only; code changes are not rewound
- **−** Anthropic OAuth is not supported; an API key is required
- **−** Token-saving figures in the README come from the author's own usage
- **−** Bash output filtering depends on optional rtk; native filtering is only planned

<sub>no GPU · Needs rtk (optional) · Models: Anthropic, OpenAI, xAI, Google Gemini, GitHub Copilot · [Repo](https://github.com/tontinton/maki) · [📖 Docs ↗](https://maki.sh/docs) · [🌐 Site ↗](https://maki.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/maki/)</sub>

<a name="gsd-pi"></a>
### #&#8288;180 [gsd-pi](https://github.com/open-gsd/gsd-pi) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

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

<a name="orbital"></a>
### #&#8288;181 [orbital](https://github.com/zqiren/orbital) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · GPL-3.0 · Nov 2026</sub>

**Project agent that shares context across Claude Code, Codex and Gemini CLI.**

Orbital is a Windows and macOS desktop app that runs a project agent over a local workspace folder. It keeps state, decisions, lessons and a task queue as plain files (PROJECT_STATE.md, DECISIONS.md, LESSONS.md, queue.json) and delegates work to Claude Code, Codex, Gemini CLI, Cursor and other CLI agents. When one agent hits a usage limit, another can continue from the same project context.

- **+** Context lives as plain files in the project folder, readable by any agent
- **+** Dispatches to Claude Code (SDK), Codex (app-server), Cursor (ACP), and Gemini CLI or Aider (PTY)
- **+** Queued tasks must end Completed or Blocked; agents that stop without a verdict are re-prompted
- **+** Runs locally with your own API key; installers need no Python or Node
- **−** GPL-3.0 license limits embedding in proprietary products
- **−** Installers only for Windows and macOS; no Linux build or Docker image mentioned
- **−** Full autonomy is on the roadmap; today it is scheduler-driven
- **−** Delegating needs the worker agent CLIs installed and signed in separately

<sub>no GPU · Needs LLM provider API key, Claude Code, Codex, Gemini CLI or other agent CLIs (optional workers) · Models: DeepSeek, Anthropic, OpenAI, Moonshot · [Repo](https://github.com/zqiren/orbital) · [📖 Docs ↗](https://orbital.top/en/guide/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orbital/)</sub>

<a name="cezar"></a>
### #&#8288;182 [cezar](https://github.com/open-mercato/cezar) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Web cockpit that runs coding agent CLIs in parallel git worktrees.**

Cezar is a Node app that launches your installed coding agent CLIs (Claude Code, Codex, OpenCode, Gemini CLI and others) on tasks, each in its own git worktree, and streams steps, tool calls, tokens and cost to a browser UI. Workflows are YAML files mixing agent steps and shell checks with retry on failure. It also supports GitHub issue launch, scheduled automations, Jira/Linear, and child task dispatch. State is stored as plain files in .ai/cezar/.

- **+** Uses your existing agent CLI logins; no API key needed for most supported agents
- **+** Per-task git worktrees with queueing let several agents run at once
- **+** Workflows are YAML; each step can use a different agent runner
- **+** No database; state is plain files in .ai/cezar/
- **−** Requires at least one separately installed and logged-in agent CLI
- **−** Gemini CLI needs an API key, Vertex AI or Workspace licence
- **−** Parent task limited to four child tasks in flight
- **−** Server mode setup guides cover only Ubuntu VPS and macOS with ngrok

<sub>no GPU · Needs Node 20+, Agent CLI (Claude Code, Codex, OpenCode, etc.), git (optional), gh (optional) · Models: Claude Code, Codex, GitHub Copilot CLI, Cursor Agent, Gemini CLI · port 4321 · [Repo](https://github.com/open-mercato/cezar) · [▶️ Demo ↗](https://www.youtube.com/watch?v=nNLJm9gArnE) · [📖 Docs ↗](https://github.com/open-mercato/cezar/blob/main/docs/reference.md) · [🌐 Site ↗](https://cezar.run/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cezar/)</sub>

<a name="phi"></a>
### #&#8288;183 [phi](https://github.com/pulseaiclub/phi) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Terminal coding agent in Go with diff review and sub-agents.**

phi is a terminal UI coding agent written in Go that gives the model read, write, edit, bash, grep, find and ls tools. It talks to OpenAI, OpenAI Responses, Anthropic and Gemini APIs, plus OpenAI-compatible endpoints, and adds sub-agents, MCP, SKILL.md skills and PXB extensions. It also has an in-TUI git diff review with line notes, a code viewer, and a headless `phi run` mode with JSONL output.

- **+** Static Go binary of about 15 MB, with no Node, Python or Electron runtime
- **+** In-TUI /diff review lets you leave line notes and send them to the agent
- **+** Headless `phi run` with JSONL events, session resume and tool scoping via --tools
- **+** Per-directory JSONL sessions with fork, plus per-role models for sub-agents
- **−** Footprint timings and sizes measured only on macOS arm64 and not re-run since first published
- **−** Comparison charts against other harnesses use published figures, not a same-machine benchmark
- **−** Needs an external model API key; no local model runtime is described
- **−** README opens with sponsor ads for API resellers, which adds noise to the docs

<sub>no GPU · Needs LLM API key (OpenAI, Anthropic, Gemini or compatible), git, fd and ripgrep (auto-downloaded) · Models: OpenAI, OpenAI Responses, Anthropic, Gemini, OpenAI-compatible endpoints · [Repo](https://github.com/pulseaiclub/phi) · [📖 Docs ↗](https://pulseaiclub.github.io/docs/getting-started/) · [🌐 Site ↗](https://pulseaiclub.github.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/phi/)</sub>

<a name="pi-agent-desktop"></a>
### #&#8288;184 [pi-agent-desktop](https://github.com/abcwyc/pi-agent-desktop) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 945 · MIT · Nov 2026</sub>

**Desktop app for browsing and running pi agent sessions on macOS, Windows, Linux.**

Tauri desktop wrapper around the pi coding agent and the pi-web interface. It bundles a Next.js server and Node.js runtime, reads existing sessions and credentials from ~/.pi/agent, and shows tool calls, context usage and cost live. It adds session branching, Git worktree switching, file previews, cron-style scheduled prompts and signed in-app upgrades.

- **+** Bundles Node.js and the Next.js server, so no separate runtime or terminal is needed
- **+** Reuses existing ~/.pi/agent sessions, models and auth; PI_CODING_AGENT_DIR overrides the path
- **+** Scheduled prompts run in new sessions, default to read-only tools, and catch up after sleep
- **+** Upgrades ship as one signed build containing pi, pi-web and the desktop app together
- **−** macOS build is not Developer ID signed or notarized, so Gatekeeper blocks first launch
- **−** Does not install a global pi CLI; that must be installed separately
- **−** Scheduled tasks only run while the app is open
- **−** LAN mode exposes shell access over plain HTTP; needs a password and HTTPS or VPN

<sub>Docker + Compose · Needs pi (bundled), Microsoft WebView2 (Windows, installer fetches it), WebKitGTK 4.1 and GTK 3 (Linux) · Models: Models and OAuth/API keys configured through pi, Custom model configuration · port 30141 · [Repo](https://github.com/abcwyc/pi-agent-desktop) · [📖 Docs ↗](https://github.com/abcwyc/pi-agent-desktop/blob/main/docs/desktop-updates.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-agent-desktop/)</sub>

<a name="vtcode"></a>
### #&#8288;185 [vtcode](https://github.com/vinhnx/vtcode) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 917 · Apache-2.0 · Nov 2026</sub>

**Rust terminal coding agent with a macOS desktop app.**

VT Code is a coding agent written in Rust that runs as a terminal TUI and as a native macOS app sharing the same runloop, providers and sandboxing. It plans read-only, shows turn diffs, runs headless tasks with resume, and extends through MCP, skills, plugins and hooks. Models come from hosted or local providers, with keys kept in the OS keyring or an encrypted file.

- **+** Read-only planning and turn-diff review before changes are applied
- **+** Headless exec with resume, snapshots, revert and scheduled recurring tasks
- **+** Extends via MCP, skills, plugins, hooks, subagents and ACP editor integration
- **+** Installs via curl script, Homebrew, cargo or a Windows PowerShell script
- **−** Desktop app is macOS 15+ only; the cask ships Apple Silicon builds
- **−** Ad hoc-signed desktop builds need manual approval in System Settings on first launch
- **−** Source builds require Rust 1.100.0+ (edition 2024)
- **−** Headless exec needs workspace trust, or VTCODE_TRUST_WORKSPACE set for non-TTY runs

<sub>Docker · Needs Rust 1.100.0+ (source builds only), LLM provider API key or login · Models: OpenAI, ChatGPT login, GitHub Copilot, hosted providers, local providers · [Repo](https://github.com/vinhnx/vtcode) · [📖 Docs ↗](https://github.com/vinhnx/vtcode/blob/main/docs/index.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vtcode/)</sub>

<a name="ai-maestro"></a>
### #&#8288;186 [ai-maestro](https://github.com/23blocks-os/ai-maestro) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 858 · MIT · Nov 2026</sub>

**Dashboard for running and messaging many coding agents across machines.**

AI Maestro is a Next.js/TypeScript dashboard and service that launches and monitors terminal-based coding agents (Claude Code, Codex, Grok Build, plus Pi, OpenClaw, Copilot CLI) over tmux, Docker, AWS EC2 or ECS Fargate. Machines join a peer mesh with no central server, and agents message each other through the Agent Messaging Protocol. It adds per-agent long-term memory, Kanban boards, a secrets vault, and chat cards for approvals.

- **+** Peer mesh across machines with no central server; headless workers use about 100MB RAM
- **+** Works with Claude Code, Codex and Grok Build, and launches any terminal agent
- **+** Secrets vault: agents use credentials by name and output is scrubbed
- **+** MIT licensed, no account or telemetry; also ships a Claude Code plugin with 14 skills
- **−** Needs 4 GB RAM to build (2 GB plus swap); Node.js 24 and tmux required
- **−** Chat history and approval cards only for Claude Code, Codex and Grok Build
- **−** Lip-sync for agent faces needs OpenAI or ElevenLabs voice and an API key
- **−** Agents get separate clones, not shared worktrees, so repos sync through git

<sub>RAM ≥ 4 GB · no GPU · Docker · Needs Node.js 24, tmux, Claude Code 2.1.287+ (optional, for mods), AWS (optional, for EC2/ECS) · Models: Claude Code, Codex, Grok Build, Pi, OpenClaw · port 23000 · [Repo](https://github.com/23blocks-os/ai-maestro) · [📖 Docs ↗](https://aimaestro.sh) · [🌐 Site ↗](https://getaimaestro.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-maestro/)</sub>

<a name="pullboard"></a>
### #&#8288;187 [pullboard](https://github.com/pullboard-dev/pullboard) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 850 · MIT · Nov 2026</sub>

**Spec-driven task board that coordinates and cross-checks coding agents in a git repo.**

Pullboard is a Node CLI that keeps a work queue inside .git and assigns items to coding agents, each in its own worktree. Work is frozen against approved rows in SPEC.md, a second agent verifies the exact commit, and accepted items land on main with a receipt. It works with Claude Code and Codex, and provides an MCP server and a local web view.

- **+** A separate verifier agent checks each submitted commit; rejects go back with a reason
- **+** Board is one file in .git; no external database or service required
- **+** Per-agent worktree lanes with atomic claims keep parallel agents out of each other's files
- **+** Runners execute tests and landing on other machines, posting signed receipts
- **−** Does not run models itself; needs Claude Code, Codex or another MCP client
- **−** Spec rows, doctrine and review roles add overhead for small projects
- **−** Scale figures come from the project's own board, not independent users
- **−** Phone access uses a relay through pullboard.dev; a self-hosted relay is not described

<sub>no GPU · Needs git, Node 22.13+ · Models: Claude Code, Codex, any MCP client · [Repo](https://github.com/pullboard-dev/pullboard) · [▶️ Demo ↗](https://pullboard.dev/live/) · [🌐 Site ↗](https://pullboard.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pullboard/)</sub>

<a name="codeaf"></a>
### #&#8288;188 [codeaf](https://github.com/agent-field/codeaf) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 841 · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent that splits requests into parallel tasks on open models.**

CodeAF is a Go coding agent that runs from one terminal window across all projects on a machine. It splits chat requests into tasks, each in its own repo copy and branch, then tests them and lands passing work on your branch, never main. It picks worker, planner and checker models per task, and has a headless mode (`codeaf do`) for CI and scripts.

- **+** Single Go binary, 53 MB on disk, about 27 MB RAM per added session
- **+** Tasks run in separate repo copies and branches; passing work never lands on main
- **+** Per-task model crew with spend limits ($5 default) and open-weight-only option
- **+** Headless do, exec and run commands print JSON and exit codes for CI
- **−** Marked early preview; README warns of rough edges
- **−** Anonymous telemetry is on by default and must be turned off
- **−** Benchmark results are self-published and use one model, DeepSeek V4 Flash
- **−** Remote access without ssh depends on a hosted relay that is not live yet

<sub>no GPU · Docker + Compose · Needs Provider API key (OpenRouter, DeepSeek, etc.) or Ollama, ssh for remote hosts · Models: OpenRouter, DeepSeek, GLM, Kimi, MiniMax · [Repo](https://github.com/agent-field/codeaf) · [📖 Docs ↗](https://github.com/Agent-Field/codeaf/blob/main/docs/GUIDE.md) · [🌐 Site ↗](https://agentfield.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeaf/)</sub>

<a name="frontman"></a>
### #&#8288;189 [frontman](https://github.com/frontman-ai/frontman) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 743 · custom license · Nov 2026</sub>

**Browser overlay where you click a UI element and an AI edits its source.**

Frontman is a dev-mode plugin for Next.js, Astro and Vite (React, Vue, Svelte) that adds a chat overlay at /frontman on your local dev server. You click an element and describe the change. The agent uses the live DOM, computed CSS, component tree, source maps and server logs to edit the source files, with hot reload. It uses your own LLM API key and a separate Elixir/Phoenix server.

- **+** Reads rendered page context (computed CSS, component tree, source maps), not only source files
- **+** One install command each for Next.js, Astro and Vite, including Turbopack
- **+** Dev-only: production builds strip Frontman out
- **+** BYOK with OpenAI, Anthropic, OpenRouter, Fireworks AI, NVIDIA, Google and xAI
- **−** Supports only Next.js, Astro and Vite; Remix, Nuxt, SolidStart, Qwik are listed as coming soon
- **−** Split license: Apache 2.0 for libs, AGPL-3.0 for the server
- **−** Self-hosting is from source; packaging is described as still evolving
- **−** Free trial is five uses; no setup details for the Elixir server in the README

<sub>no GPU · Needs Node.js 22.19+ (Astro), Elixir/Phoenix server, LLM provider API key · Models: OpenAI, Anthropic, OpenRouter, Fireworks AI, NVIDIA · [Repo](https://github.com/frontman-ai/frontman) · [▶️ Demo ↗](https://www.youtube.com/watch?v=-4GD1GYwH8Y) · [📖 Docs ↗](https://frontman.sh/docs/) · [🌐 Site ↗](https://frontman.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frontman/)</sub>

<a name="dev-3-0"></a>
### #&#8288;190 [dev-3.0](https://github.com/h0x91b/dev-3.0) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 337 · Apache-2.0 · Nov 2026</sub>

**Kanban board that runs each task as a coding agent in its own git worktree.**

dev-3.0 is a desktop app (macOS, Windows) and a headless Linux CLI with a browser UI. Each Kanban card creates a git worktree, a tmux session and an agent such as Claude Code, Codex, Gemini CLI, Cursor Agent or opencode. A diff review panel sends inline comments back to the agent as a prompt, and `dev3 remote` serves the UI to a browser or phone.

- **+** One worktree and tmux session per task, so parallel agents do not touch each other's files
- **+** Supports Claude Code, Codex, Gemini CLI, Cursor Agent, opencode and custom CLI agents
- **+** Built-in diff viewer with inline comments exported back to the agent as a prompt
- **+** `dev3 remote` serves the full UI over Cloudflare tunnel, LAN or SSH forward
- **−** Sends usage telemetry to GA4 and PostHog by default; opt-out via setting or env var
- **−** Windows build is described as new, possibly rough, and unsigned
- **−** No embedded editor and no manual git staging, by design
- **−** Needs a separate agent CLI installed and configured; the app does not run models itself

<sub>no GPU · Docker + Compose · Needs git, tmux, Homebrew (macOS/Linux install), agent CLIs (Claude Code, Codex, Gemini CLI, Cursor Agent, opencode) · Models: Claude Code, Codex, Gemini CLI, Cursor Agent, opencode · [Repo](https://github.com/h0x91b/dev-3.0) · [📖 Docs ↗](https://dev3.h0x91b.com/first-task.html) · [🌐 Site ↗](https://dev3.h0x91b.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dev-3-0/)</sub>

<a name="costrict"></a>
### #&#8288;191 [costrict](https://github.com/zgsm-ai/costrict) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Sep 2026</sub>

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

<a name="codeapp"></a>
### #&#8288;192 [codeapp](https://github.com/thebaselab/codeapp) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Nov 2026</sub>

**Native iPad code editor with local terminal, Git and built-in language runtimes.**

Code App is a Swift iPadOS app that uses monaco-editor and native code to imitate the VS Code editing experience. It bundles Git, a terminal with 70+ commands, and local runtimes for Python, C/C++ (clang via WebAssembly), Node, PHP and Java. The README does not mention any AI features, so it fits this list only as an editor.

- **+** Runs Python 3.9.2, Node 18.19.0, PHP 8.3.2, Clang 14 and OpenJDK 8 on-device
- **+** Git clone, commit, diff, push and pull built in, plus SSH support
- **+** MIT licensed, with runtime source repositories listed for each bundled language
- **+** Distributed through the App Store and TestFlight
- **−** No AI assistant or agent features are described in the README
- **−** Apple-only: building requires Xcode and a downloadFrameworks.sh step
- **−** LSP support is limited to Python and Java
- **−** Bundled runtimes are old versions, such as Python 3.9 and OpenJDK 8

<sub>Needs Xcode, iPadOS · [Repo](https://github.com/thebaselab/codeapp) · [📖 Docs ↗](https://code.thebaselab.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeapp/)</sub>

<a name="ralph-tui"></a>
### #&#8288;193 [ralph-tui](https://github.com/subsy/ralph-tui) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (47) · Freshness: active (99) · Maintenance: fair (54) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

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

<a name="nezha"></a>
### #&#8288;194 [nezha](https://github.com/hanshuaikang/nezha) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · GPL-3.0 · Sep 2026</sub>

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

<a name="cli-agent-orchestrator"></a>
### #&#8288;195 [cli-agent-orchestrator](https://github.com/awslabs/cli-agent-orchestrator) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (37) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="cccc"></a>
### #&#8288;196 [cccc](https://github.com/chesterra/cccc) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Nov 2026</sub>

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

<a name="momo-code"></a>
### #&#8288;197 [momo-code](https://github.com/momozi1996/momo-code) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · custom license · Oct 2026</sub>

**Terminal coding agent built on opencode with experience-based self-improvement loops.**

Momo Code is a Node.js CLI coding agent built on opencode. It runs an interactive REPL or one-shot tasks against 25+ LLM providers, including any OpenAI-compatible endpoint. It adds a tactic-learning loop (/evolve), proposal-based self-refinement (/refine), LoRA fine-tuning (/fine-tune), recursive subagents and DAG task graphs. v2.0 integrates the Pi agent framework as an npm dependency and is labeled experimental.

- **+** Supports 25+ providers plus custom OpenAI-compatible endpoints via MOMO_CUSTOM_* env vars
- **+** Self-refinement proposals need human approval before they are applied
- **+** Budget rails and a ~/.momo/STOP file halt the self-evolution loop
- **+** Subagent and DAG graph runs persist state and can resume after restart
- **−** README marks v2.0 as experimental with an architecture upgrade in progress
- **−** Scope is broad (physics sim, voice, optimization), which adds surface area to audit
- **−** Install pipes a curl script to bash; npm package is not yet published
- **−** README shows version 1.0.0 output alongside v2.0 claims; license is unidentified

<sub>GPU optional · Needs Node.js >= 22.19.0, git, curl, LLM provider API key, Python with genesis-world (for /sim), sounddevice and scipy (for /voice) · Models: Claude, GPT-4, Gemini, Deepseek, Zhipu GLM · port 4097 · [Repo](https://github.com/momozi1996/momo-code) · [🌐 Site ↗](https://momozi.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/momo-code/)</sub>

<a name="eca"></a>
### #&#8288;198 [eca](https://github.com/editor-code-assistant/eca) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Editor-agnostic AI coding assistant server speaking an LSP-style protocol.**

ECA is a Clojure server that editors spawn with `eca server` and talk to over stdin/stdout, similar to a language server. It handles chat, rewrite and completion against the LLM provider you configure, with tool calls, subagents, MCP resources and prompts, and OpenTelemetry export. Plugins exist for Emacs, VS Code, Neovim, IntelliJ, a desktop app and a CLI.

- **+** One config.json works the same across Emacs, VS Code, Neovim, IntelliJ, desktop and CLI
- **+** Documented protocol lets other editors integrate without reimplementing tool-call handling
- **+** Supports OpenAI, Anthropic, Copilot and Ollama local models, plus custom providers
- **+** Configurable agents and subagents with separate models, tools and behaviors
- **−** Needs a separate editor plugin; the server alone has no UI
- **−** Requires configuring at least one model or provider before use
- **−** Server written in Clojure, which may deter contributors from other ecosystems
- **−** No Docker image or compose file provided

<sub>no GPU · Needs LLM provider account or local Ollama, Editor plugin · Models: OpenAI, Anthropic, GitHub Copilot, Ollama, custom providers · [Repo](https://github.com/editor-code-assistant/eca) · [📖 Docs ↗](https://eca.dev/config/introduction) · [🌐 Site ↗](https://eca.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eca/)</sub>

<a name="luvus"></a>
### #&#8288;199 [luvus](https://github.com/rizriyz/luvus) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · Apache-2.0 · Nov 2026</sub>

**Terminal workspace that tracks and orchestrates AI coding agents across panes.**

Luvus is a Rust terminal multiplexer with persistent sessions, split panes and tabs, and automatic detection of coding agents such as Claude Code, Codex, opencode and Gemini. It shows each agent's state (blocked, working, done, idle) with tokens and cost. It also adds git worktree orchestration, a Git/GitHub dashboard, SSH remote machines and an optional read-only web client.

- **+** Live status for about 20 agents needs no agent-side integration
- **+** Background server keeps panes and sessions alive, including on SSH remotes
- **+** Worktree orchestration with task queues, quality gates and merging
- **+** Installs by Homebrew, shell script or PowerShell on macOS, Linux, FreeBSD, Windows
- **−** Session resume and precise hook events vary by agent; several have neither
- **−** Web client phone access needs a separately trusted TLS tunnel
- **−** Supervises agents you install; it does not run models itself
- **−** Ctrl+Space conflicts with the macOS input source shortcut until disabled

<sub>no GPU · Needs git, gh, ssh · [Repo](https://github.com/rizriyz/luvus) · [📖 Docs ↗](https://luvus.dev/docs/) · [🌐 Site ↗](https://luvus.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/luvus/)</sub>

<a name="juggler"></a>
### #&#8288;200 [juggler](https://github.com/juggler-ai/juggler) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 871 · AGPL-3.0 · Nov 2026</sub>

**Desktop and browser workbench for inspecting and steering AI coding agents.**

Juggler is a Go-based desktop app and headless server that runs coding agents against a project and shows the session as a navigable tree of threads and tool calls. Each recorded model transaction can be opened to see the system prompt, messages, tool schemas, usage and stop reason. It works with Claude Code, Codex, Copilot, Gemini, Ollama and other providers, and the server can run remotely with the app or a browser as clients.

- **+** Opens any recorded LLM call to show prompt, tool schemas, tokens, cache use and timing
- **+** One server per machine; desktop app and several browsers share a live session
- **+** Provider-neutral: hosted APIs, installed agent CLIs or Ollama, switchable mid-conversation
- **+** JavaScript extensions; SDK, bundled extensions and examples are Apache-2.0
- **−** Core app is AGPL-3.0; modified hosted versions must be released under AGPL
- **−** WAN access modes exist only in official binaries, not in source builds
- **−** LAN access has no password, so it suits trusted networks only
- **−** Building from source needs Go 1.27+, submodules and GTK/WebKitGTK on Linux

<sub>GPU optional · Needs Go 1.27+ (build only), GTK4 and WebKitGTK (Linux), Model provider API key or subscription · Models: Anthropic/Claude Code, OpenAI/Codex, GitHub Copilot, Google Gemini, Mistral · port 3939 · [Repo](https://github.com/juggler-ai/juggler) · [📖 Docs ↗](https://github.com/juggler-ai/juggler/blob/main/docs/extension_guide.md) · [🌐 Site ↗](https://juggler.studio) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/juggler/)</sub>

<a name="pi-bolt"></a>
### #&#8288;201 [pi-bolt](https://github.com/opensec-git/pi-bolt) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 871 · MIT · Nov 2026</sub>

**Ahead-of-time compiled native build of the Pi terminal coding agent.**

Pi-Bolt is the Pi coding agent compiled ahead of time into a single native executable for Linux x86-64/ARM64, macOS on Apple silicon, Windows x64 and Android (Termux). It keeps Pi's commands, sessions, settings, providers and extensions, and needs no Node.js or Bun. It can also run as an ACP agent in editors (--acp) or as an MCP server (--mcp).

- **+** Single executable; no Node.js, Bun or npm needed at runtime
- **+** Reads existing ~/.pi/agent config and runs Pi extensions unchanged
- **+** README benchmarks vs Pi on Node 24: 41 ms start, 117 MB after 40 prompts
- **+** Runs as an ACP editor agent or an MCP server for other agents
- **−** Default build has no JIT, so extensions loaded at run time are interpreted
- **−** Extensions using bun:ffi need the separate JIT build
- **−** pi-bolt compile for baking in extensions works only on Linux and macOS
- **−** macOS support is Apple silicon only; no Intel Mac build listed

<sub>no GPU · Needs Model provider account (connect with /login), glibc 2.17+ on Linux, or musl with libstdc++, Termux glibc on Android · Models: Providers supported by Pi · [Repo](https://github.com/opensec-git/pi-bolt) · [📖 Docs ↗](https://pi-bolt.opensec.in/docs/installation.html) · [🌐 Site ↗](https://pi-bolt.opensec.in) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-bolt/)</sub>

<a name="repo2rlenv"></a>
### #&#8288;202 [repo2rlenv](https://github.com/huggingface/repo2rlenv) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 812 · Apache-2.0 · Nov 2026</sub>

**Generates verifiable Harbor RL tasks from repos, PRs and agent trajectories.**

Repo2RLEnv converts GitHub repositories, merged PRs, recorded agent sessions and task seeds into Harbor tasks. Each task has an instruction, a starting environment, a verifier and a reference solution. It ships pipelines such as pr_diff, pr_runtime and commit_runtime, plus Tasksmith, a LangGraph agent that designs tasks. Tasks are reviewed and labeled unverified, verified, needs_repair or blocked, and Harbor runs the agents.

- **+** Many pipelines: PR diff, runtime tests, CVE patches, trajectories, SWE-smith and R2E recipes
- **+** Tasks carry evidence labels and a quality loop that checks the reference and baseline
- **+** Published datasets on the Hub, including 50 verified tasks from Hugging Face ML libraries
- **+** Outputs Harbor task format, so tasks run with Harbor-supported agents
- **−** pr_diff grading needs a model judge; if it is unavailable, trials are left ungraded
- **−** Tasksmith and research recipes need Modal or Daytona workers to execute code
- **−** Requires Python 3.12+ and an authenticated GitHub CLI
- **−** Generated tasks are not automatically suitable for training; older datasets lack newer fixes

<sub>GPU optional · Needs Python 3.12+, GitHub CLI, Harbor, Docker, Modal or Daytona, Anthropic API · Models: Anthropic (judge), LangGraph with Pi or OpenCode · [Repo](https://github.com/huggingface/repo2rlenv) · [📖 Docs ↗](https://huggingface.github.io/Repo2RLEnv/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repo2rlenv/)</sub>

<a name="loki-mode"></a>
### #&#8288;203 [loki-mode](https://github.com/asklokesh/loki-mode) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · custom license · Nov 2026</sub>

**CLI agent that turns a task or issue into a PR with a signed receipt.**

Loki Mode is a Shell and Bun-based CLI that drives Claude Code (or opencode) through a contract, tests-first, implement, verify loop. It ends in a defined outcome such as VERIFIED or BLOCKED, opens a pull request, and seals an Ed25519-signed receipt that `loki verify` re-checks offline. It also ships a local Control Plane UI, a 48-tool MCP server and a Claude Code plugin.

- **+** Signed receipt per run, re-checkable offline with `loki verify` and distinct exit codes
- **+** Takes tasks, PRD files, or GitHub, GitLab and Jira issues and opens a PR
- **+** Spend cap via --max-cost or budgets.per_run; PR lists what was not proven
- **+** Local model routes: Ollama, LM Studio, llama.cpp, vLLM, OpenRouter via opencode
- **−** BUSL-1.1 license: commercial use needs separate arrangement until Apache 2.0 in 2030
- **−** Full feature set requires Claude Code; codex, aider, cline and gemini providers were removed
- **−** macOS and Linux only; Windows is not supported
- **−** Needs Node.js 20+, Git and curl; default spend cap is $100 with an API key

<sub>no GPU · Docker + Compose · Needs Claude Code CLI or ANTHROPIC_API_KEY, Node.js 20+, Git 2.x, curl, Bun 1.3+ (bundled in npm package) · Models: Claude (Claude Code, Anthropic Agent SDK), OpenRouter, Ollama, LM Studio, llama.cpp · port 47821 · [Repo](https://github.com/asklokesh/loki-mode) · [📖 Docs ↗](https://github.com/asklokesh/loki-mode/blob/main/docs/QUICKSTART.md) · [🌐 Site ↗](https://www.autonomi.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loki-mode/)</sub>

<a name="pydantic-deepagents"></a>
### #&#8288;204 [pydantic-deepagents](https://github.com/vstorm-co/pydantic-deepagents) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Oct 2026</sub>

**Terminal coding assistant and Python agent framework on Pydantic AI.**

A Claude Code-style terminal assistant that works with any tool-calling model, plus the Python framework behind it. create_deep_agent() gives a model a filesystem, shell, planning, memory, sub-agents, MCP client and an optional Docker sandbox. It also offers Live Run Forking, which splits a run into isolated branches and merges the winner by AI judge, test results or vote.

- **+** Same harness works as a TUI (pydantic-deep) and as a Python library
- **+** Supports Anthropic, OpenAI, OpenRouter, Gemini, Ollama or any OpenAI-compatible endpoint
- **+** Run forking with copy-on-write overlays, per-branch budgets and a test-command merge hook
- **+** Headless `pydantic-deep run` for CI, plus MCP client, hooks and USD budget limits
- **−** Comparison table and uniqueness claims are self-reported by the authors
- **−** Many capabilities are opt-in flags that need configuration
- **−** Browser automation needs the separate pydantic-deep[browser] extra
- **−** Docker sandbox needs a local Docker install; not bundled

<sub>no GPU · Needs Python 3.10+, Pydantic AI, LLM provider API key or Ollama, Docker (optional, sandbox), Playwright (optional, browser) · Models: Anthropic, OpenAI, OpenRouter, Google Gemini, Ollama · README: alternative to Claude Code · [Repo](https://github.com/vstorm-co/pydantic-deepagents) · [📖 Docs ↗](https://vstorm-co.github.io/pydantic-deepagents/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pydantic-deepagents/)</sub>

<a name="snow-cli"></a>
### #&#8288;205 [snow-cli](https://github.com/mayday-wpf/snow-cli) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · custom license · Nov 2026</sub>

**Terminal coding agent with MCP, LSP, sub-agents, hooks and headless mode.**

Snow CLI is a TypeScript terminal coding agent built on Ink and installed through npm (`npm install -g snow-ai`, then `snow`). It supports MCP servers, LSP-based code navigation, sub-agents, hooks, Claude Code-compatible skills, async background tasks and a headless mode. It also has an SSE server mode and VSCode and JetBrains extensions.

- **+** Headless and SSE server modes allow scripting and integration with other clients
- **+** Reads Claude Code skills and supports MCP, LSP, hooks and custom sub-agents
- **+** VSCode and JetBrains extensions plus a separate desktop client, Snow App
- **+** Docs cover installation, configuration and each major feature in separate guides
- **−** License is not identified (NOASSERTION), so reuse terms need a manual check
- **−** Requires Node.js 18 or newer and an external model API key or relay
- **−** README is mostly sponsors and relay links, with little technical overview

<sub>no GPU · Needs Node.js >= 18, npm >= 8.3.0, LLM API endpoint · [Repo](https://github.com/mayday-wpf/snow-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/snow-cli/)</sub>

<a name="gooey-pi"></a>
### #&#8288;206 [gooey-pi](https://github.com/am-will/gooey-pi) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 982 · MIT · Oct 2026</sub>

**Electron desktop GUI for the Pi, OMP and Prime Agent coding harnesses.**

GooeyPi is an Electron desktop app that wraps the Pi, OMP and Prime Agent coding-agent CLIs in one workspace for macOS, Linux and Windows. It adds session management, Git diffs and commits, integrated terminals, an in-app browser agents can drive, scheduled runs and voice dictation. Each harness keeps its own models, logins and sessions.

- **+** Switches between Pi, OMP and Prime Agent without stopping work running in another harness
- **+** Built-in Git review, terminal tabs, file browser and agent-controllable in-app browser
- **+** Provider credentials stay in each harness; voice keys use OS secure storage
- **+** Scheduled one-time or recurring runs, plus local whisper.cpp dictation with no API key
- **−** Requires at least one of Pi, OMP or Prime Agent installed separately
- **−** macOS 14 Sonoma or later required on Mac
- **−** Network MCP servers are read-only in the app; only local stdio MCP is managed
- **−** Remote SSH hosts are only a design proposal, not implemented

<sub>no GPU · Needs Pi, OMP or Prime Agent CLI, Node.js 24.15.0+ and npm 12.0.2+ (source builds), whisper.cpp (optional), CUA Driver (optional) · Models: Models via the Pi, OMP or Prime harness, OpenAI-compatible endpoints, OpenAI, Groq, Deepgram dictation · [Repo](https://github.com/am-will/gooey-pi) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gooey-pi/)</sub>

<a name="pi-web"></a>
### #&#8288;207 [pi-web](https://github.com/jmfederico/pi-web) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 965 · MIT · Nov 2026</sub>

**Web UI for running Pi Coding Agent sessions on a remote machine.**

PI WEB is a Node.js runtime and browser interface for Pi Coding Agent. Sessions run in real workspaces or Git worktrees on your computer or server and keep running after you disconnect. It offers file inspection, terminals and plugins in one UI, and can register remote machines to supervise several hosts.

- **+** Sessions persist on the host when the browser disconnects
- **+** Supports Git worktrees as separate workspaces per session
- **+** Can register remote machines and manage them from one UI
- **+** CLI covers install, doctor, status, logs, restart and update
- **−** Built only for Pi Coding Agent, not other coding agents
- **−** Not a sandbox or multi-tenant; assumes trusted users and repos
- **−** Must not face the public internet; needs VPN, tunnel or auth proxy
- **−** Bun is supported on a limited basis; Node.js is the recommended runtime

<sub>no GPU · Docker + Compose · Needs Node.js 22.19.0+, npm, Pi Coding Agent, git, node-pty · port 8504 · [Repo](https://github.com/jmfederico/pi-web) · [📖 Docs ↗](https://pi-web.dev/install) · [🌐 Site ↗](https://pi-web.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-web/)</sub>

<a name="michaelkinsy-pig"></a>
### #&#8288;208 [michaelkinsy/pig](https://github.com/michaelkinsy/pig) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 898 · MIT · Nov 2026</sub>

**Go port of the Pi terminal coding agent, shipped as one native binary.**

PiG reimplements Pi, a minimal terminal coding agent, in Go as a single binary that needs no Node.js. It runs Pi's TypeScript extensions unchanged and also supports extensions written in Go, Rust or Python. Extensions, skills and prompts can be bundled into a Piglet, a named agent that can be built into its own executable. It is a pre-stable 0.x release checked against Pi 1.5.0.

- **+** Single native Go binary; no Node.js needed to run the agent itself
- **+** Runs Pi TypeScript extensions unchanged, plus Go, Rust and Python extension SDKs
- **+** Behavior checked against pinned Pi 1.5.0 with parity scenarios and a public coverage report
- **+** Installs via curl script, npm, go install, Nix or release archives
- **−** Pre-stable 0.x; edge cases still being hardened against Pi behavior
- **−** No security sandbox; tools and shell commands run with your user permissions
- **−** Windows support is a preview; Nix flake verified only on x86_64-linux
- **−** Omits Pi's remote Session, telemetry and evaluation packages; not endorsed by Pi maintainers

<sub>no GPU · Needs Provider API key or subscription login (e.g. OPENAI_API_KEY) · Models: Providers via API key or subscription login (OpenAI named as an example) · [Repo](https://github.com/michaelkinsy/pig) · [📖 Docs ↗](https://pi-in-go.dev/docs/latest) · [🌐 Site ↗](https://pi-in-go.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/michaelkinsy-pig/)</sub>

<a name="pi-pocket"></a>
### #&#8288;209 [pi-pocket](https://github.com/tannermidd/pi-pocket) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 898 · MIT · Nov 2026</sub>

**Web and phone UI for running Pi coding agent sessions on your own machine.**

Pi Pocket is a Node.js server and web app that hosts sessions of the Pi coding agent on your computer, so you can review diffs, queue follow-ups and approve actions from a phone. It supports shared sessions with teammates, subagents, scheduled and resumable runs, and a Relay connector for Discord, Slack, Telegram and Matrix. Remote access works over LAN, Tailscale or a Cloudflare tunnel.

- **+** Runs on your own machine and project; no cloud VM required
- **+** Multiplayer sessions: teammates can watch or steer, and phone review works
- **+** Relay connector opens the connection from your machine, so no public server is needed
- **+** Install options include npm, Windows .exe, macOS .pkg, Docker/Podman, Nix and systemd
- **−** Anyone with steering access can run commands as your user; invites do not limit file access
- **−** Git worktrees isolate files but are not sandboxes
- **−** Pi CLI extensions do not run unchanged; it has its own extension API
- **−** One server process owns the database; built-in browser needs Chromium on the host

<sub>no GPU · Docker + Compose · Needs Node.js 22.19+, Chromium-based browser (built-in browser), Git for Windows (Windows shell tools) · Models: Providers connected in-app or via existing Pi sign-in · [Repo](https://github.com/tannermidd/pi-pocket) · [📖 Docs ↗](https://tannermidd.github.io/pi-pocket/docs/) · [🌐 Site ↗](https://tannermidd.github.io/pi-pocket/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-pocket/)</sub>

<a name="alphacode"></a>
### #&#8288;210 [alphacode](https://github.com/dragonked2/alphacode) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 681 · MIT · Nov 2026</sub>

**Rust terminal coding agent that edits files, runs tests and drives Firefox.**

AlphaCode is a terminal coding agent written in Rust. It reads a repository, plans, edits files, runs commands and tests, and reports what it verified. It can also drive a Firefox session through a browser extension and control desktop apps. It works with a built-in free model or providers such as Claude, GPT, Gemini, Ollama and any OpenAI-compatible endpoint.

- **+** Native Rust binary; README reports about 28 MB RAM for one session
- **+** Built-in free model, or many providers including Ollama and LM Studio
- **+** Sessions are saved to disk and resume after crashes or dropped SSH connections
- **+** Extends via skills, MCP servers and hooks; swarm mode runs parallel agents
- **−** Browser automation supports Firefox only, through a separate extension
- **−** Installs via curl-pipe-to-bash or PowerShell script; no Docker image
- **−** Terms and limits of the built-in free AI are not detailed in the visible README
- **−** RAM, benchmark and comparison figures come from the project's own README

<sub>no GPU · Needs Firefox with AlphaCode Browser Agent extension (optional) · Models: Claude, GPT, Gemini, DeepSeek, GitHub Copilot · [Repo](https://github.com/dragonked2/alphacode) · [🌐 Site ↗](https://alphacli.github.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/alphacode/)</sub>

<a name="beluga"></a>
### #&#8288;211 [beluga](https://github.com/beluga-labs/beluga) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 605 · MIT · Nov 2026</sub>

**Desktop app running one Claude Code agent per git worktree, in parallel.**

Beluga is a desktop app (macOS, Linux, Windows) that creates a worktree, branch and Claude Code agent for each task and runs them side by side. It renders tables, charts and diagrams in chat and runs scheduled or event-triggered agent jobs (Sentinel). Your agent can also ask a friend's agent to act on their Mac after approval.

- **+** Separate worktree, branch and agent per task; main folder stays untouched
- **+** Scratch tab shows screenshots and test logs while the agent is still running
- **+** Sentinel triggers on schedules or GitHub, Stripe, Sentry and webhook events; starts paused
- **+** Friend agent requests are end-to-end encrypted, need approval, and use no server
- **−** Requires a Claude Code login; other model providers are not mentioned
- **−** Mac and Windows installers are unsigned or not notarized, so first launch needs an override
- **−** macOS build is Apple Silicon only; friend features are described for Macs
- **−** Remote use depends on SSH or a server install; no Docker setup

<sub>no GPU · Needs Claude Code, Git for Windows (Windows only) · Models: Claude (via Claude Code) · [Repo](https://github.com/beluga-labs/beluga) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beluga/)</sub>

<a name="mini-swe-agent"></a>
### #&#8288;212 [mini-swe-agent](https://github.com/swe-agent/mini-swe-agent) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: weak (14) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Sep 2026</sub>

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

<a name="px0"></a>
### #&#8288;213 [px0](https://github.com/px0-ai/px0) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

**Browser-based IDE for reviewing PRs and diffs of AI-written code.**

px0 is a single Go binary that serves a browser UI for reviewing pull requests from GitHub, GitLab, Gitea/Forgejo and Bitbucket Cloud, browsing local repos, and making quick edits. Threads anchored to code ranges can be dispatched to local agents such as Claude Code, Codex, Aider or Goose. It can run headless on a remote host with `-host 0.0.0.0`.

- **+** Single static Go binary; no Node, Electron or CGO at runtime
- **+** Server daemon uses about 20-30 MB RAM, per the README's benchmarks
- **+** Reviews PRs from four hosts and hands threads to seven agent CLIs
- **+** Remote mode needs no SSH keys or remote daemon, only a reachable port
- **−** No built-in authentication; anyone reaching the port can edit workspace files
- **−** Workbench mode lets anyone with access browse any directory px0 can read
- **−** Does not run models itself; agent features require separate local CLIs
- **−** Building from source needs Go 1.24+ and Node.js or Bun

<sub>no GPU · Docker · Needs Local AI coding CLIs (optional), Git · Models: Claude Code, Cursor Agent, Antigravity, OpenCode, Codex · [Repo](https://github.com/px0-ai/px0) · [📖 Docs ↗](https://px0.ai/docs) · [🌐 Site ↗](https://px0.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/px0/)</sub>

<a name="takt"></a>
### #&#8288;214 [takt](https://github.com/nrslib/takt) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

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

<a name="vibeyard"></a>
### #&#8288;215 [vibeyard](https://github.com/elirantutia/vibeyard) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

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

<a name="fanbox"></a>
### #&#8288;216 [fanbox](https://github.com/alchaincyf/fanbox) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Desktop file browser with embedded terminal for running and reviewing coding agents.**

FanBox is an Electron app for macOS (Apple Silicon) that pairs a local file browser and previewer with an embedded node-pty/xterm.js terminal for running Claude Code, Codex and nine other agent CLIs. It lights up files as agents write them, shows per-round diffs with per-file restore and whole-round rollback, and lists past agent sessions per project with resume. A dependency-free web mode (node server.js, port 4567) covers browsing and preview only.

- **+** Per-round diff panel with single-file restore, whole-round rollback and replay timeline
- **+** Launches 11 agent CLIs; Claude Code and Codex get official hooks for exact state events
- **+** Backend listens on loopback only; write endpoints need a per-launch random token
- **+** Signed, notarized dmg; web mode needs no dependencies or build
- **−** Official build is macOS Apple Silicon only; Windows ports are unofficial community forks
- **−** Web mode has no terminal or editors; those require Electron
- **−** Usage panel and update checks contact Claude, Codex and GitHub endpoints
- **−** Resume, hooks and usage features target Claude Code and Codex; others use heuristics

<sub>no GPU · Needs Electron, node-pty, xterm.js, Claude Code or Codex CLI · Models: Claude Code, Codex, DeepSeek Harness, Hermes Agent, OpenClaw · port 4567 · [Repo](https://github.com/alchaincyf/fanbox) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fanbox/)</sub>

<a name="dscode"></a>
### #&#8288;217 [dscode](https://github.com/qiz029/dscode) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Terminal coding agent whose sessions can see and hand tasks to each other.**

DSCODE is a terminal coding agent for macOS and Linux built on DeepSeek Harness. A local background host owns sessions, so several terminals or scripts can attach to one session, and the agent can list, read and message other sessions. It also has version-checked file edits, a separate read-only reviewer for diffs, `dscode exec` for CI, and an optional remote runtime over TCP.

- **+** Background host keeps sessions alive after a terminal closes and lets terminals share one
- **+** Agent-to-agent messaging with persisted mailbox, retry de-duplication and a finite budget
- **+** Separate read-only model reviews diffs; default workspace-write sandbox with optional Auto review
- **+** Bundled Node.js; `dscode exec` supports scripts and CI with --json and --resume
- **−** No Windows support; Linux needs glibc, so Alpine/musl is unsupported
- **−** Remote runtime is token-authenticated but unencrypted; needs VPN, LAN or SSH tunnel
- **−** Linux sandboxing needs bubblewrap; otherwise Landlock, or sandboxed commands are refused
- **−** Antigravity Gemini provider access is noted as not yet verified live

<sub>no GPU · Docker · Needs Git, bubblewrap (Linux), Google Chrome (browser tasks) · Models: DeepSeek, OpenAI/ChatGPT, Antigravity Gemini, OpenRouter, OpenCode Go · [Repo](https://github.com/qiz029/dscode) · [📖 Docs ↗](https://github.com/qiz029/dscode/blob/main/docs/demo.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dscode/)</sub>

<a name="deepseek-harness-desktop"></a>
### #&#8288;218 [ningbainb/deepseek-harness-desktop](https://github.com/ningbainb/deepseek-harness-desktop) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 961 · BSD-3-Clause · Nov 2026</sub>

**Desktop client for the DeepSeek DSH runtime with Git, task board and SSH.**

Community-maintained Electron app that wraps the official DSH Runtime and Web UI as an AI coding workbench for Windows, macOS and Linux. It adds chat-driven code edits, file preview, Git/SCM, a task board with cron scheduling, Skills and plugins, SSH/SFTP, and phone remote control. It is not an official DeepSeek client.

- **+** Windows installer bundles Node.js, DSH, pnpm and MinGit; no separate setup
- **+** Task board runs real DSH agent sessions with cron scheduling and recorded evidence
- **+** Built-in SSH terminal, SFTP, port forwarding, and phone remote control via QR code
- **+** Imports Claude Code and Codex projects read-only; browser and computer use default off
- **−** Installers are unsigned; macOS build is not notarized and needs an xattr workaround
- **−** macOS (arm64, 13+) and Linux (x64) builds are Preview; macOS has no auto-update
- **−** README is primarily Chinese; English version is in a separate file
- **−** Official packages include anonymous usage telemetry, though opt-out is documented

<sub>Needs Git (macOS and Linux), Linux graphical session with sandbox · Models: DeepSeek, OpenAI Codex (ChatGPT OAuth), third-party APIs · [Repo](https://github.com/ningbainb/deepseek-harness-desktop) · [📖 Docs ↗](https://github.com/ningbainb/deepseek-harness-desktop/blob/HEAD/docs/desktop.md) · [🌐 Site ↗](https://1521003.xyz/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepseek-harness-desktop/)</sub>

<a name="helix"></a>
### #&#8288;219 [helix](https://github.com/helixml/helix) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 834 · custom license · Nov 2026</sub>

**Self-hosted fleet of coding agents with a spec-driven Kanban board.**

Helix runs many coding agents (Claude Code, Codex, Gemini CLI, Qwen Code, any ACP agent) in parallel, each in its own isolated sandbox with a streaming desktop. Work moves through a Kanban board: an agent writes a spec, you approve it, and it implements the change and opens a pull request on GitHub, GitLab or Azure DevOps. It also bundles RAG, MCP tool support, tracing, OIDC and RBAC.

- **+** Each agent gets an isolated desktop with browser, terminal and filesystem, viewable live
- **+** Switch agent harness mid-task; context carries over to the new agent
- **+** Accepts any OpenAI-compatible endpoint, including self-hosted vLLM, and runs air-gapped
- **+** Includes multi-tenancy, OIDC SSO, RBAC, token and cost tracing
- **−** Non-OSI license: free only for personal, educational, or under $10M revenue and 250 staff
- **−** Forbids using the code to build a competing product
- **−** Broad scope (RAG, billing, notifications) makes the stack heavier than a single agent CLI
- **−** Existing Docker installs ship PostgreSQL 12, which is end-of-life and needs a manual upgrade

<sub>GPU optional · Docker + Compose · Needs Docker, PostgreSQL, Git hosting (GitHub, GitLab or Azure DevOps) · Models: OpenAI, Anthropic, Anthropic on Vertex AI, Anthropic on AWS Bedrock, vLLM · port 8080 · [Repo](https://github.com/helixml/helix) · [▶️ Demo ↗](https://app.helix.ml/) · [📖 Docs ↗](https://helix.ml/docs) · [🌐 Site ↗](https://helix.ml) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/helix/)</sub>

<a name="tastecode"></a>
### #&#8288;220 [tastecode](https://github.com/leonxlnx/tastecode) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 649 · Apache-2.0 · Nov 2026</sub>

**Desktop app that runs Codex, Claude Code and Grok agents with a Design Mode.**

TasteCode is a desktop workspace, written in TypeScript, that puts Codex, Claude Code and Grok in one app. Orchestration, project state, terminal, diffs, checkpoints and history stay on the local machine, and it drives the provider CLIs you have already signed in to. Design Mode inspects and edits web interfaces. It is an early beta (0.5.1).

- **+** Three agent providers in one app: Codex, Claude Code and Grok
- **+** State, history and checkpoints stay local; credentials remain with the provider CLI or OS store
- **+** Built-in terminal, browser preview, git context and readable diffs
- **+** Controls a provider lacks are hidden or degraded rather than faked
- **−** Early beta; the README warns of bugs and changing behavior
- **−** Prebuilt installers only for Windows x64 and macOS Apple Silicon; no Linux build listed
- **−** Requires at least one provider CLI installed and signed in separately
- **−** Windows build is unsigned and triggers a SmartScreen warning

<sub>Needs Codex, Claude Code or Grok CLI (signed in), Git, Node 24 LTS and pnpm (development only) · Models: Codex, Claude Code, Grok · [Repo](https://github.com/leonxlnx/tastecode) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tastecode/)</sub>

<a name="mobius"></a>
### #&#8288;221 [mobius](https://github.com/citizenhicks/mobius) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 632 · Apache-2.0 · Nov 2026</sub>

**Rust runtime for coding agents with gateway, terminal client and macOS app.**

möbius is a Rust agent framework plus a headless gateway that runs coding agents (Bots) with sandboxed file and shell tools. A terminal client and a native macOS app, with an iPhone and iPad app in TestFlight beta, attach to the same gateway and share one conversation stream. The framework crate can also be embedded to build your own agent or frontend.

- **+** Commands run in Seatbelt (macOS) or Bubblewrap (Linux) and fail closed if unavailable
- **+** Same chat continues across terminal, Mac and iPhone through one gateway
- **+** Reported 48.9% fewer tokens than Codex CLI on 20 Terminal-Bench tasks, with lower peak RAM
- **+** Embeddable crate with pluggable models, sandboxes, checkpoint storage and middleware
- **−** MCP and app connectors are not yet supported
- **−** Prebuilt binaries only for Apple Silicon macOS and x86_64 Linux
- **−** Same benchmark pass rate as Codex (3 of 20) with 17.9% more agent time
- **−** Remote access needs the gateway machine awake; default tunnel address changes on restart

<sub>no GPU · Needs Bubblewrap (Linux sandbox), cloudflared (optional, Quick Connect), Rust 1.100.0+ (cargo install) · Models: OpenAI, Codex, Anthropic, DeepSeek, Kimi · [Repo](https://github.com/citizenhicks/mobius) · [📖 Docs ↗](https://mobius.thinkingsand.dev/how) · [🌐 Site ↗](https://mobius.thinkingsand.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mobius/)</sub>

<a name="kode-cli"></a>
### #&#8288;222 [kode-cli](https://github.com/shareai-lab/kode-cli) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="xed-editor"></a>
### #&#8288;223 [xed-editor](https://github.com/xed-editor/xed-editor) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · GPL-3.0 · Nov 2026</sub>

**Android text and code editor with LSP, built-in terminal and extensions.**

Xed-Editor is a Kotlin text editor for Android with syntax highlighting, LSP-based code intelligence, project-wide tools and an Ubuntu-rootfs terminal. It ships in two flavors: a community build with an extension store (themes, icon packs) and a Play Store build without it. It is a general mobile code editor and has no built-in AI features.

- **+** LSP code intelligence and syntax highlighting in a native Android editor
- **+** Built-in terminal backed by an Ubuntu rootfs
- **+** Extension support for themes and icon packs in the community flavor
- **+** Distributed via F-Droid, IzzyOnDroid, Google Play and GitHub releases
- **−** README describes no AI or coding-agent features
- **−** Play Store flavor excludes extensions and supports arm64-v8a only
- **−** Community flavor downloads the terminal rootfs over the network
- **−** GPL-3.0 license limits use as a closed-source base

<sub>no GPU · Docker · Needs Android device, JDK 21 and Android SDK (to build) · [Repo](https://github.com/xed-editor/xed-editor) · [🌐 Site ↗](https://xed-editor.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xed-editor/)</sub>

<a name="empryo"></a>
### #&#8288;224 [empryo](https://github.com/proxysoul/empryo) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · custom license · Nov 2026</sub>

**Coding agent that maps your repo and edits code by symbol name.**

Empryo is a coding agent with desktop, terminal and headless modes that builds a map of a repository before editing. It replaces functions or classes by name, runs typecheck, lint and tests in the same turn, and keeps per-project memory of decisions and past bugs. This repository holds only the public SoulForge v2 core and engine; the Empryo v3 desktop app is developed privately.

- **+** Edits by function or class name instead of line ranges
- **+** Runs typecheck, lint and tests and fixes failures in the same turn
- **+** Per-project memory of decisions and past bugs
- **+** Same agent across desktop, terminal and headless CI
- **−** Repo is only the SoulForge v2 core; v3 app and newest features are private
- **−** Empryo v3 license forbids selling, hosting or bundling it without written permission
- **−** License detected as NOASSERTION; two separate licenses apply

<sub>[Repo](https://github.com/proxysoul/empryo) · [📖 Docs ↗](https://empryo.com/docs) · [🌐 Site ↗](https://empryo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/empryo/)</sub>

<a name="llama-vscode"></a>
### #&#8288;225 [llama.vscode](https://github.com/ggml-org/llama.vscode) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**VS Code extension for local FIM completion, chat and agentic coding on llama.cpp.**

llama.vscode is a VS Code extension that sends fill-in-the-middle completion requests to a local llama.cpp server, with a ring context built from open and edited files. It also includes a chat view and Llama Agent, which works with local models or external ones such as OpenRouter and can use MCP servers installed in VS Code. Models are grouped into envs that can be selected, imported and exported together.

- **+** Completion runs locally on llama.cpp, with documented settings for under 8GB up to 64GB+ VRAM
- **+** Ring context from open files and yanked text, with cache reuse for large contexts
- **+** Envs switch whole model sets (completion, chat, embeddings, tools) in one step
- **+** Agent can use MCP servers installed in VS Code and external providers like OpenRouter
- **−** Completion requires FIM-compatible models, which limits model choice
- **−** CPU-only setups are documented as significantly lower quality
- **−** Tied to VS Code; Vim/Neovim needs the separate llama.vim plugin
- **−** Agent ships 9 internal tools; custom tools must be written in JavaScript

<sub>GPU optional · Needs VS Code, llama.cpp · Models: GGUF, FIM models (Qwen2.5-Coder), gpt-oss 20B, OpenRouter, Hugging Face downloads · port 8012 · [Repo](https://github.com/ggml-org/llama.vscode) · [📖 Docs ↗](https://github.com/ggml-org/llama.vscode/wiki) · [🌐 Site ↗](https://marketplace.visualstudio.com/items?itemName=ggml-org.llama-vscode) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llama-vscode/)</sub>

<a name="parrot-nvim"></a>
### #&#8288;226 [parrot.nvim](https://github.com/frankroeder/parrot.nvim) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 792 · custom license · Nov 2026</sub>

**Neovim plugin for LLM chat buffers and inline rewrite, append and prepend edits.**

parrot.nvim is a Lua plugin for Neovim 0.11+ that streams LLM responses into native buffers. It offers markdown chat sessions saved as files, plus visual-selection commands (PrtRewrite, PrtAppend, PrtPrepend, PrtRetry) with an optional diff preview. It talks to OpenAI, Anthropic, Gemini, xAI, ollama and custom OpenAI-compatible endpoints, and can connect to agent backends over ACP.

- **+** Chats are plain markdown files, stored in a configurable directory
- **+** Separate chat and command model selection, switchable with PrtModel
- **+** API keys can come from env vars, shell commands or password manager CLIs
- **+** No background requests or ghost-text completions; you control what is sent
- **−** Requires Neovim 0.11+; the latest release dropped plenary as a breaking change
- **−** No autonomous agent loop; agent use depends on an external ACP backend
- **−** Interactive commands only see the selection if you add template placeholders
- **−** No inline ghost-text completion

<sub>no GPU · Needs Neovim 0.11+, fzf-lua (optional), ripgrep (optional), telescope.nvim (optional) · Models: OpenAI, Anthropic, Google Gemini, xAI, Ollama · [Repo](https://github.com/frankroeder/parrot.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/parrot-nvim/)</sub>

<a name="timon"></a>
### #&#8288;227 [timon](https://github.com/ai-timon/timon) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 775 · AGPL-3.0 · Nov 2026</sub>

**Local orchestrator that dispatches coding tasks to agent CLIs you already use.**

Timon is a desktop and background-service app that splits a request into tasks and hands them to agent CLIs such as Claude Code, Codex, Copilot CLI, Grok, opencode, Pi and Hermes. Each task runs in its own git worktree and moves through code, review by a second model, and merge on a Kanban board. It runs on your own machine using your existing CLI subscriptions, with state in SQLite and permission prompts before pushes or deletions.

- **+** Each task gets its own git worktree, reviewed by a second model before merge
- **+** Uses existing agent CLI logins; the README says it never calls token-billed APIs
- **+** Quota fallbacks move work to another backend when a subscription runs out
- **+** Signed plugins install without a restart; SDK and templates are MIT
- **−** Needs at least one agent CLI already installed and signed in
- **−** Multi-user roles, groups and per-person permissions are only in the paid Pro tier
- **−** AGPL-3.0 core; plugin exception is described in a separate LICENSING.md
- **−** macOS build targets Apple silicon only; Windows and Linux are x64 only

<sub>no GPU · Compose · Needs Node.js 22 (bundled by installer), Git, Agent CLI signed in (claude, codex, copilot, grok, opencode, pi or hermes-acp), SQLite · Models: Claude Code, Codex, GitHub Copilot CLI, Grok CLI, opencode · [Repo](https://github.com/ai-timon/timon) · [📖 Docs ↗](https://docs.timon-ai.com) · [🌐 Site ↗](https://timon-ai.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/timon/)</sub>

<a name="diri"></a>
### #&#8288;228 [diri](https://github.com/cristicretu/diri) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 501 · AGPL-3.0 · Nov 2026</sub>

**Native Mac app that runs many coding agent CLIs side by side.**

diri is a Rust and GPUI desktop app that runs Claude Code, Codex, Cursor, Gemini, OpenCode and other agent CLIs in parallel terminals, locally or over SSH. It shows each session as working, waiting or done, and keeps sessions alive across app restarts. It also offers per-task Git worktrees, a built-in MCP server for spawning agents, notes, and scheduled runs.

- **+** Each terminal has its own holder process, so agents survive quitting or updating the app
- **+** Per-task Git worktrees keep parallel agents apart, with diffs and PR checks alongside
- **+** Remote sessions bootstrap a helper over SSH; no tmux or sudo needed on the server
- **+** New agents are added as JSON manifests, no code changes required
- **−** Deepest status and resume support is only for Claude Code and Codex
- **−** Linux support is beta, Ubuntu x86_64 only, and not every release ships packages
- **−** Main build requires macOS 15 or newer
- **−** AGPL-3.0 license may restrict some commercial use

<sub>no GPU · Needs Agent CLIs you already use, Git, SSH for remote hosts · Models: Claude Code, Codex, Cursor, Gemini, OpenCode · [Repo](https://github.com/cristicretu/diri) · [📖 Docs ↗](https://diri.sh/docs/) · [🌐 Site ↗](https://diri.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diri/)</sub>

<a name="continue"></a>
### #&#8288;229 [continue](https://github.com/continuedev/continue) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (94) · Freshness: active (90) · Maintenance: weak (22) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · Apache-2.0 · Jul 2026</sub>

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

<a name="loushang"></a>
### #&#8288;230 [loushang](https://github.com/zhnt/loushang) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent with persistent sessions and method-guided delivery.**

Loushang is a Python CLI and terminal workbench, `loushang code`, that runs coding turns against a model catalog with built-in tools, resumable sessions and project-level extensions. It also ships `loushang.ai`, an SDK with a model registry, streaming, tool calls and cost helpers. Work is structured through "methods" that define roles, phases and acceptance expectations.

- **+** Sessions can be resumed, forked, exported and diagnosed
- **+** Project-level Python extensions add hooks, tools, commands and resources
- **+** Reusable AI SDK with model registry, streaming and cost helpers
- **+** Apache-2.0 licensed with docs and examples for CLI and SDK
- **−** README calls it early development; recommended install is from source
- **−** No tagged release published
- **−** Work, research and ppt surfaces are roadmap only

<sub>Needs uv, Python · [Repo](https://github.com/zhnt/loushang) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loushang/)</sub>

<a name="wu"></a>
### #&#8288;231 [wu](https://github.com/dstrml/wu) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 841 · custom license · Nov 2026</sub>

**Native Rust code editor forked from Zed, with built-in coding agents.**

Wu is a GPU-rendered desktop code editor written in Rust, forked from Zed and diverging heavily from it. It integrates Claude Code, Codex and OpenCode as built-in agents and sends no telemetry or usage data. Installers exist for macOS, Windows and Linux (x86-64 and AArch64).

- **+** Native GPU rendering, no Electron or webviews
- **+** Built-in support for Claude Code, Codex and OpenCode
- **+** No account required and no telemetry
- **+** Prebuilt installers for macOS, Windows and Linux, including AArch64
- **−** Heavily diverged Zed fork, so Zed docs and extensions may not match
- **−** Build instructions defer to Zed's docs, with no Wu-specific steps
- **−** Mixed GPL-3.0-or-later and Apache-2.0 licensing, detected as NOASSERTION
- **−** Memory claims link to benchmarks; README gives no RAM or GPU requirements

<sub>Needs Claude Code, Codex, OpenCode · [Repo](https://github.com/dstrml/wu) · [📖 Docs ↗](https://wu.dstrml.org) · [🌐 Site ↗](https://wu.dstrml.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wu/)</sub>

<a name="distill"></a>
### #&#8288;232 [distill](https://github.com/samuelfaj/distill) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 782 · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent that splits work between a main model and a cheaper worker.**

Distill is a Rust coding agent harness with a TUI. A main model plans and reviews, an optional cheaper worker model runs delegated tasks, and a utility model handles extraction and summaries. It works with Grok, Claude and Codex subscriptions and any OpenAI-compatible model, with modes UltraSave, UltraFast, UltraCode, Auto and Normal.

- **+** Three model tiers (main, worker, utility), each set with an effort level or auto
- **+** Five execution modes with published cost and time per mode on one voxel prompt
- **+** Works with Grok, Claude and Codex subscriptions and OpenAI-compatible endpoints
- **+** BENCHMARKS.md lists methodology, cost bounds, reproduction commands and source JSON
- **−** Caveman terse-prose and Ponytail rules are always on, with no off switch
- **−** Install is a curl-pipe-to-shell script that edits your shell rc file
- **−** Savings claims come from the author's own benchmarks, not independent runs
- **−** Setup steps include an OpenRouter login plus a subscription login

<sub>Needs OpenRouter account, Grok, Claude or Codex subscription, or an OpenAI-compatible endpoint · Models: Grok, Claude, Codex, OpenAI-compatible models, OpenRouter · [Repo](https://github.com/samuelfaj/distill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/distill/)</sub>

<a name="genesis"></a>
### #&#8288;233 [genesis](https://github.com/emi-group/genesis) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 779 · AGPL-3.0 · Nov 2026</sub>

**Recursive multi-agent coding system that builds software from one objective.**

Genesis is an Elixir/OTP runtime where manager agents split an objective into tasks and executor agents implement and validate changes in isolated Git worktrees. It ships as a Tauri desktop app with a Phoenix LiveView dashboard, or as a headless server, and exposes a local MCP endpoint so other coding agents can submit tasks. Runtime data is stored in SQLite and software versions in Git.

- **+** Isolated Git worktrees per task, with accepted results merged into main
- **+** Provider profiles with per-account concurrency, peak-hour schedules and rate-limit backoff
- **+** Local MCP endpoint for task submission, progress, messaging and cancellation
- **+** Desktop dashboard can drive agents on a remote server over an SSH tunnel
- **−** Headless server has no built-in authentication; remote access needs an SSH tunnel
- **−** AGPL-3.0 license and a contributor license agreement for pull requests
- **−** Building from source needs Elixir 1.20.4 and Erlang/OTP 29
- **−** Needs external model provider credentials; no local model support is documented

<sub>no GPU · Needs Git, LLM provider API key or OAuth subscription, Elixir 1.20.4 and Erlang/OTP 29 (source builds) · Models: OpenAI (API key), Subscription OAuth providers · port 9999 · [Repo](https://github.com/emi-group/genesis) · [📖 Docs ↗](https://genesis.evox.group/getting-started/) · [🌐 Site ↗](https://genesis.evox.group/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/genesis/)</sub>

<a name="agent"></a>
### #&#8288;234 [agentiloop/agent](https://github.com/agentiloop/agent) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 658 · custom license · Nov 2026</sub>

**Native macOS Swift app that runs an LLM agent loop to control your Mac.**

AgentiLoop Agent is a SwiftUI app for macOS 14.6+ that connects 23 LLM providers, plus on-device Apple Intelligence, to a task loop. The loop reads and edits code, builds Xcode projects, runs shell commands as the user or root, and drives Mac apps through the Accessibility API. It also supports MCP servers, sub-agents, voice activation and iMessage remote control.

- **+** Supports 23 providers including Ollama, vLLM and LM Studio, with automatic fallback on 429 or timeout
- **+** Signed, notarized release binary; installs via Homebrew cask without building from source
- **+** Desktop automation through Accessibility, AppleScript, JXA and runtime-compiled Swift AgentScripts
- **+** Edits are snapshotted, with per-edit rollback and whole-task rewind
- **−** macOS only; the Rust and Go CLIs for Windows and Linux are separate repositories
- **−** Source builds are ad-hoc signed, so the Launch Agent and Daemon helpers do not register
- **−** Local models are impractical without 64-128GB Apple Silicon, per the README
- **−** License is not identified by detection (NOASSERTION), so reuse terms need manual checking

<sub>GPU optional · Needs macOS 14.6+, Xcode (source builds only), LLM provider API key or local Ollama/vLLM/LM Studio · Models: Claude, OpenAI, Codex, Gemini, Grok · [Repo](https://github.com/agentiloop/agent) · [📖 Docs ↗](https://github.com/AgentiLoop/Agent/blob/main/docs/TECHNICAL.md) · [🌐 Site ↗](https://agentiloop.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent/)</sub>

<a name="muxin"></a>
### #&#8288;235 [muxin](https://github.com/lumarylabsllc/muxin) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 475 · Apache-2.0 · Nov 2026</sub>

**Native desktop app for running agent sessions and tasks across your own machines.**

Muxin is a Rust desktop app (GPUI) for macOS, Linux and Windows that connects to your machines over ssh and a small remote agent. It opens persistent terminal sessions for Claude Code, Codex, Gemini CLI and other agent CLIs, runs containerized "boxes", streams Linux desktops, copies files, and manages GitHub self-hosted runners. The same features are exposed through an MCP server (`muxin mcp`) and `--json` CLI commands.

- **+** Sessions for 12+ agent CLIs stay running on the remote machine after the app closes
- **+** Reuses system ssh, ~/.ssh/config, gh login and optionally Tailscale; no extra server to set up
- **+** Every feature is available via MCP server and scriptable CLI with --json
- **+** Headless build with no GUI libraries for servers and CI boxes
- **−** Windows installer is unsigned and triggers a SmartScreen warning
- **−** Linux builds need glibc 2.35 or newer
- **−** A Mac desktop session needs Accessibility permission to forward system shortcuts
- **−** It manages agent CLIs rather than being a coding agent itself

<sub>no GPU · Needs ssh, gh (GitHub CLI), Tailscale (optional), Docker (for boxes) · Models: Claude Code, Codex, OpenCode, Gemini CLI, Amp · [Repo](https://github.com/lumarylabsllc/muxin) · [🌐 Site ↗](https://muxin.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/muxin/)</sub>

<a name="keel"></a>
### #&#8288;236 [keel](https://github.com/xing-shuyin/keel) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 403 · MIT · Nov 2026</sub>

**Browser and desktop workspace for pi, Claude Code, and Codex coding agents.**

Keel (pi-web-ui) is a Node.js web workspace that hosts coding-agent engines (pi, DSH, Claude Code, Codex) with parallel conversations, a file browser and editor, terminal, and Git diff view. It adds a canvas for chaining task steps with approval branches, plus Skills, MCP servers, and plugins. It runs from npm, as an Electron app, a Windows portable build, or in Docker.

- **+** Supports pi, DSH, Claude Code, and Codex engines in one UI
- **+** Built-in file editor, terminal, and Git status and diff beside chat
- **+** Install with npm install -g keel-agent, then run keel .
- **+** Ships as web, Electron desktop, Windows portable, or background service
- **−** Features and session formats vary by engine; native CLI sessions lack some chat features
- **−** Requires Node.js 22.19.0 or later
- **−** Model provider and credentials must be configured separately after install
- **−** Some docs and community links are in Chinese or on QQ

<sub>no GPU · Docker + Compose · Needs Node.js 22.19.0+ · Models: pi, DSH, Claude Code, Codex · port 8787 · [Repo](https://github.com/xing-shuyin/keel) · [📖 Docs ↗](https://xing-shuyin.github.io/pi-web-ui-site/docs.html) · [🌐 Site ↗](https://xing-shuyin.github.io/pi-web-ui-site/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/keel/)</sub>

<a name="pi-harness"></a>
### #&#8288;237 [pi-harness](https://github.com/wangmiaozero/pi-harness) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 362 · AGPL-3.0 · Nov 2026</sub>

**Desktop app for running, tracing and coordinating Pi coding agents.**

Pi-Harness is a desktop workspace built around the Pi Coding Agent, which still executes every run. It adds run history with trace, replay and evaluation, tool policies, budgets and checkpoints, plus multi-agent teams with a task DAG and git worktree isolation. It also includes file editing, Git tools, a project architecture map and a browser for Claude Code, Codex, Cursor and Gemini CLI histories.

- **+** Records runs with trace, replay, compare and per-run token, cost and duration stats
- **+** Checkpoints allow resume, fork or retry; policies and budgets limit tools and spend
- **+** Agent teams use task dependencies, review gates and worktrees to keep changes separate
- **+** Installers for macOS, Windows and Linux bundle Pi and Node.js; Pi sessions stay usable outside
- **−** Built around Pi Coding Agent; not a standalone agent
- **−** AGPL-3.0 license may constrain embedding or modified redistribution
- **−** macOS builds are ad-hoc signed and Windows installers unsigned; no in-app auto-install
- **−** Architecture map analyzes JS, TS and Vue imports; other languages get file-level index only

<sub>no GPU · Needs Pi Coding Agent (bundled in installers), Node.js (bundled in installers) · Models: ChatGPT subscription sign-in, API-key providers (Pi-compatible, custom endpoints), Claude, Gemini, DeepSeek · [Repo](https://github.com/wangmiaozero/pi-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-harness/)</sub>

<a name="opcode"></a>
### #&#8288;238 [opcode](https://github.com/winfunc/opcode) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (88) · Freshness: recent (77) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · AGPL-3.0 · Nov 2026</sub>

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

<a name="claude-squad"></a>
### #&#8288;239 [claude-squad](https://github.com/smtg-ai/claude-squad) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · AGPL-3.0 · Nov 2026</sub>

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

<a name="longhorizon-harness"></a>
### #&#8288;240 [longhorizon-harness](https://github.com/amap-ml/longhorizon-harness) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2026</sub>

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

<a name="agor"></a>
### #&#8288;241 [agor](https://github.com/preset-io/agor) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (33) · Freshness: active (95) · Maintenance: patchy (49) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Nov 2026</sub>

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

<a name="kander"></a>
### #&#8288;242 [kander](https://github.com/dualface/kander) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 338 · MIT · Nov 2026</sub>

**Terminal kanban that runs parallel coding agents with independent review gates.**

Kander is a Go terminal kanban board that dispatches task cards to coding agents (Codex, Claude, Grok, Cursor, Pi), each in its own Git worktree and tmux/herdr container. It schedules around branch and file overlaps and puts finished work through two independent review stages before a card closes. It can import GitHub issues by reusing local `gh` credentials.

- **+** Git worktree isolation per agent, with scheduling that avoids branch and file overlap
- **+** Review is separate from execution, with a completion gate before a card is done
- **+** Imports GitHub issues via local `gh` login; never reads or stores a token
- **+** Ships as a single binary via Homebrew, Linux tarball or Windows zip
- **−** Needs at least one separate agent CLI (Codex, Claude, Grok, Cursor or Pi) installed
- **−** Terminal UI only; no web interface is described
- **−** Production figures in the README come from the author's own projects
- **−** Tasks start through agents that have Kander rules loaded, which adds setup

<sub>no GPU · Needs Git, Codex, Claude, Grok, Cursor or Pi, tmux or herdr, GitHub CLI (optional) · Models: Codex, Claude, Grok, Cursor, Pi · [Repo](https://github.com/dualface/kander) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kander/)</sub>

<a name="auto-dev"></a>
### #&#8288;243 [auto-dev](https://github.com/phodal/auto-dev) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (62) · Freshness: active (91) · Maintenance: patchy (40) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MPL-2.0 · Sep 2026</sub>

**Kotlin Multiplatform coding agent for IntelliJ, VS Code, CLI, desktop and mobile.**

AutoDev Xiuper is an alpha multi-agent platform written in Kotlin Multiplatform. It ships a coding agent with file system, grep/glob, shell, web fetch and MCP tools, plus agents for document queries, code review, natural-language database queries and runnable artifacts. It runs as an IntelliJ IDEA plugin, VS Code extension, npm CLI, desktop and Android app, web app, and a Ktor server.

- **+** Same agent runtime across IntelliJ, VS Code, CLI, desktop, Android and web
- **+** Reads AGENTS.md from the project hierarchy and loads Claude Skills, MCP and A2A
- **+** Supports OpenAI, Anthropic, Google, DeepSeek and Ollama models
- **+** Includes PR review, pre-push review and NL-to-SQL agents beyond coding
- **−** Labelled Alpha; the web agent is experimental
- **−** iOS requires building from source
- **−** VS Code, iOS and landing web modules are not in the root Gradle graph
- **−** Last tagged release is from February 2026, well behind recent commits

<sub>Needs LLM provider API or Ollama, JetBrains IDE or VS Code (for plugins), npm (for CLI) · Models: OpenAI, Anthropic, Google, DeepSeek, Ollama · [Repo](https://github.com/phodal/auto-dev) · [▶️ Demo ↗](https://web.xiuper.com/) · [🌐 Site ↗](https://xiuper.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auto-dev/)</sub>

<a name="overalls"></a>
### #&#8288;244 [overalls](https://github.com/ghuntley/overalls) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Nov 2026</sub>

**Self-hosted persistent microVM dev machines with a built-in coding agent.**

Overalls is a self-hosted platform that runs development machines as persistent Firecracker microVMs (NixOS, Ubuntu or Windows). Each keeps its disk, name and address across stop, start, resize, clone and move. It has its own agent that keeps working after you disconnect, and Claude Code and Codex come pre-installed with no API keys on the machine. The README labels it a research preview.

- **+** Persistent microVMs keep disk, name and address through stop, resize, clone and move
- **+** Agent threads keep running after you disconnect and wake stopped machines
- **+** Claude Code and Codex pre-installed, no API keys on machine, per-token accounting
- **+** Access via browser, SSH, VS Code, overalls CLI or mobile app
- **−** Research preview; README says not for consumption
- **−** No hosted version; you install and operate it yourself
- **−** Hardware requirements and install steps are only on the website, not the README
- **−** No tagged release published

<sub>Needs Firecracker, NixOS · Models: Claude Code, Codex · [Repo](https://github.com/ghuntley/overalls) · [📖 Docs ↗](https://overalls.dev/self-host/) · [🌐 Site ↗](https://overalls.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/overalls/)</sub>

<a name="aidermacs"></a>
### #&#8288;245 [aidermacs](https://github.com/matthewzmd/aidermacs) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 936 · Apache-2.0 · Nov 2026</sub>

**Emacs package that runs Aider for AI pair programming inside Emacs.**

Aidermacs is an Emacs Lisp front end for the Aider CLI. It starts per-project Aider sessions from a Magit-style transient menu, in a comint or vterm buffer. It manages files added to the chat, switches between code, ask and architect modes, and shows AI edits in Ediff. Remote files work through Tramp.

- **+** Shows AI edits in built-in Ediff so you can accept or reject them
- **+** Architect mode can use separate reasoning and editor models
- **+** Works on remote files over Tramp (SSH, Docker)
- **+** Installs from MELPA or NonGNU ELPA; auto-commits are off by default
- **−** Needs a separate Aider or aider-ce install; it only wraps the CLI
- **−** File watching via AI comments in source files works only with the vterm backend
- **−** An .aider.conf.yml file overrides many Aidermacs model and commit settings
- **−** Architect mode is described as experimental

<sub>no GPU · Needs Emacs >= 26.1, Aider or aider-ce, Transient, vterm (optional) · Models: OpenAI, Anthropic, DeepSeek, Google Gemini, OpenRouter · [Repo](https://github.com/matthewzmd/aidermacs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aidermacs/)</sub>

<a name="coi"></a>
### #&#8288;246 [coi](https://github.com/coipond/coi) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 792 · MIT · Nov 2026</sub>

**Runs AI coding agents in isolated Incus system containers with threat monitoring.**

coi launches coding agents (Claude Code, Codex, opencode, opencode2, pi, omp, goose) inside an Incus system container with root, systemd and Docker, mounting your project at /workspace. Host SSH keys, tokens and environment variables stay out unless explicitly granted. Kernel-level monitoring auto-pauses or kills the container on suspicious activity, and nftables egress control has open, restricted and allowlist modes.

- **+** Host credentials and env vars are excluded by default; startup lists every grant
- **+** Auto-pauses on HIGH and auto-kills on CRITICAL threat events; JSONL audit log for a SIEM
- **+** Reusable TOML profiles with inheritance, plus a built-in hardened preset
- **+** Headless mode propagates exit codes for cron and CI; parallel isolated slots per project
- **−** Requires Linux with Incus; macOS only through Colima/Lima
- **−** Codex, opencode, omp and goose must be enabled in build config before coi build
- **−** First base image build takes about 5-10 minutes
- **−** Aider and Cursor support is listed as upcoming, not available

<sub>no GPU · Needs Incus, Colima/Lima (macOS) · Models: Claude Code, Codex CLI, opencode, opencode2, pi · [Repo](https://github.com/coipond/coi) · [📖 Docs ↗](https://github.com/coipond/coi/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coi/)</sub>

<a name="dsh-superagent-prototype"></a>
### #&#8288;247 [dsh-superagent-prototype](https://github.com/deepseek-ai/dsh-superagent-prototype) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Oct 2026</sub>

**Agent that takes GitHub requests for one repo and replies with pull requests.**

dsh-superagent is a coding agent for a single GitHub repository, packaged as a bundle for DeepSeek Harness. It listens to GitHub and optionally Feishu, opens a work item when an allowed user asks, works in its own agent session and directory, and answers in the original conversation, for example with a pull request. A web panel lists items that need a person.

- **+** Acts only on request or team-written rules; authorization is documented in docs/002
- **+** Each work item runs in its own agent session and directory
- **+** Numbered docs cover domain model, execution, prompts, panel and deployment
- **+** Cookbook documents adding a new event Source
- **−** Labeled a research prototype, not production-ready, and may contain bugs
- **−** Requires DeepSeek Harness as the runtime
- **−** Scoped to one GitHub repository per deployment
- **−** Some designs from the linked article are not implemented

<sub>Needs DeepSeek Harness, GitHub, Feishu (optional) · [Repo](https://github.com/deepseek-ai/dsh-superagent-prototype) · [🌐 Site ↗](https://www.deepseek.com/en/harness/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-superagent-prototype/)</sub>

<a name="altimate-code"></a>
### #&#8288;248 [altimate-code](https://github.com/altimateai/altimate-code) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 823 · MIT · Nov 2026</sub>

**Terminal agent for data engineering with deterministic SQL, lineage and dbt tools.**

A fork of OpenCode that adds data-engineering tooling: SQL anti-pattern detection, column-level lineage, dbt test and model generation, FinOps reports, and cross-warehouse data diffs. It runs as a TUI, as a plugin under Claude Code or Codex, or in CI for dbt pull request and GitLab MR review. It connects to 13 warehouse types and works with many LLM providers, including Ollama.

- **+** Analysis is parser-based, with benchmark methodology published for 1,077 SQL queries and 500 lineage queries
- **+** Connects to Snowflake, BigQuery, Databricks, Postgres, Redshift, ClickHouse, MongoDB and more
- **+** Analyst mode is read-only and enforces SELECT-only against live connections
- **+** Installs as an npm package or standalone binary; works with Claude Code and Codex plugins
- **−** Free default provider, Altimate Base, logs requests and may use them for training
- **−** Standalone binary unsupported on Alpine (musl) and Windows ARM64
- **−** Fork of OpenCode, so it tracks upstream changes and carries upstream fix markers
- **−** Benchmark figures are self-reported by the project, not independently verified

<sub>no GPU · Needs LLM provider or API key, Data warehouse credentials (optional), dbt (optional) · Models: Anthropic, OpenAI, Google Gemini, Amazon Bedrock, Azure OpenAI · [Repo](https://github.com/altimateai/altimate-code) · [▶️ Demo ↗](https://github.com/AltimateAI/dbt-pr-review-demo/pulls) · [📖 Docs ↗](https://help.altimate.ai/code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/altimate-code/)</sub>

<a name="wrongstack"></a>
### #&#8288;249 [wrongstack](https://github.com/wrongstack/wrongstack) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 435 · MIT · Nov 2026</sub>

**Open-source TypeScript coding agent with persistent project memory and delegation.**

WrongStack is a standalone coding agent written in TypeScript, with its own kernel, provider transports, tool executor and permission policy. A leader agent works directly or delegates to specialist agents, using SAGE (SQLite/FTS5 project memory), a Kanban board, a shared mailbox and Chimera diff review. It runs as REPL, TUI, WebUI, VibeUI, HQ and a desktop app, and installs as a single binary.

- **+** Long-term memory in SQLite/FTS5, anchored to files, symbols and commits and re-verified
- **+** REPL, TUI, WebUI, desktop and HQ share the same sessions and memory
- **+** Self-contained binary install; no Node.js needed on macOS or Linux
- **+** Works as an ACP agent for editors via `wstack acp`
- **−** Many subsystems (Brain, SAGE, Kanban, Chimera, HQ) add a steep learning curve
- **−** Install is a curl-pipe-to-shell script from the project's own domain
- **−** Linux desktop updates go through the package manager, not in place

<sub>Docker + Compose · Models: models.dev provider catalog, API keys, subscription sign-in, ACP agents · [Repo](https://github.com/wrongstack/wrongstack) · [🌐 Site ↗](https://wrongstack.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wrongstack/)</sub>

<a name="foreman"></a>
### #&#8288;250 [foreman](https://github.com/thruwire/foreman) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 835 · MIT · Oct 2026</sub>

**Supervisor that scores coding-agent runs and steers, stops, retries or finishes them.**

Foreman is a Python asyncio runtime that runs coding agents (Codex, OpenCode, Hermes, Deep Agents dcode) on a job and watches them with a decision model. It sends bounded evidence (diff, output tails, test results, AGENTS.md) to Jev or OpenAI's Decisions API and gets probabilities back. A Python policy then picks continue, steer, stop, retry, verify, finish or escalate.

- **+** Supervision loop runs concurrently, so the worker keeps working while Foreman assesses it
- **+** Checks, thresholds and evidence are configurable per responsibility in TOML files
- **+** Supports Codex, OpenCode, Hermes and Deep Agents workers, plus Pi and Codex hooks
- **+** Deterministic demo and tests run with no API key, network or agent CLI
- **−** Runs one coding worker at a time
- **−** Live steering only works with the Codex App Server backend; others stop or retry
- **−** Real runs need a TypeSafe, OpenRouter or OpenAI key for the decision model
- **−** Pi supervision needs a separate TypeScript bridge installed

<sub>no GPU · Needs Python 3.11+, TypeSafe, OpenRouter or OpenAI API key, Codex CLI, OpenCode, Hermes or dcode CLI · Models: Jev (TypeSafe), OpenAI Decisions API, OpenRouter · [Repo](https://github.com/thruwire/foreman) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/foreman/)</sub>

<a name="dinotty"></a>
### #&#8288;251 [dinotty](https://github.com/xichan96/dinotty) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 742 · MIT · Nov 2026</sub>

**Self-hosted web terminal with persistent sessions for running coding agents across devices.**

Dinotty is a Rust server with a Vue 3 frontend that runs a server-side virtual terminal (VTE parser plus PTY), so sessions survive disconnects and can be resumed from phone, tablet or desktop browser. It provides split panes, SSH with SFTP, a file browser, Git change indicators, web preview and hot-reloadable JS plugins, aimed at running Claude Code, opencode, Codex or OpenClaw. A built-in MCP server and an HTTP Open API allow external control.

- **+** PTY and screen state live on the server; refresh or reconnect restores the session
- **+** Text-only transport, about 1-10 KB/s typical, usable on 3G/4G
- **+** Built-in SSH/SFTP, file browser, Git diff marks, web preview and split panes
- **+** Hot-reload JS plugins, plus built-in MCP server and HTTP Open API
- **−** macOS app is unsigned; needs xattr -cr to open
- **−** Windows has no installer; run the server .exe or build from source
- **−** Plugin development guide is only available in Chinese
- **−** Not a coding agent itself; only hosts agents you install separately

<sub>no GPU · Docker + Compose · port 8999 · [Repo](https://github.com/xichan96/dinotty) · [📖 Docs ↗](https://xichan96.github.io/dinotty/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dinotty/)</sub>

<a name="swival"></a>
### #&#8288;252 [swival](https://github.com/swival/swival) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 363 · MIT · Nov 2026</sub>

**Python coding agent that works with local and hosted models.**

Swival is a command-line coding agent written in Python that runs against local models or online services without changing tools. It keeps working notes, resumes interrupted sessions, and has a goal mode for longer jobs. Optional features include a review step that retries on problems, a built-in security audit, and encryption of supported API keys and tokens before text reaches the model.

- **+** Same agent for local and online models; first-run setup guide connects the model
- **+** One option adds a review step, optionally run by a different model
- **+** Can encrypt supported keys and tokens, and filter private details, before sending
- **+** Session resume and saved notes support longer jobs; usable from Python code
- **−** Install command pins Python 3.14, which many systems do not ship by default
- **−** README names no specific providers or model formats
- **−** No Docker image or compose file provided
- **−** Secret encryption covers only supported keys and tokens, not arbitrary secrets

<sub>Needs uv or Homebrew, Python 3.14 · Models: local models, online services · [Repo](https://github.com/swival/swival) · [📖 Docs ↗](https://swival.dev/pages/getting-started.html) · [🌐 Site ↗](https://swival.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/swival/)</sub>

<a name="vibetunnel"></a>
### #&#8288;253 [vibetunnel](https://github.com/amantus-ai/vibetunnel) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (64) · Freshness: active (92) · Maintenance: weak (13) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Aug 2026</sub>

**Browser-based terminal for running and monitoring CLI agents remotely.**

VibeTunnel runs a TypeScript/Node.js server that proxies terminal sessions to a web UI built with Lit and ghostty-web, served on port 4020. The `vt` wrapper forwards any command, such as a coding agent, to the browser, and sessions are recorded in asciinema format. It ships as a macOS menu bar app for Apple Silicon or an npm package for Linux and headless systems.

- **+** `vt` command forwards any CLI command or shell alias to the browser
- **+** Remote access via Tailscale Serve/Funnel, ngrok, Cloudflare, Pinggy or Pangolin
- **+** Auth modes: system/PAM, env-var credentials, Ed25519 SSH keys
- **+** Git follow mode keeps the main checkout on the branch an agent uses in a worktree
- **−** Native macOS app requires Apple Silicon; Intel Macs only get the npm package
- **−** Windows is not supported
- **−** iOS app is work in progress and not recommended for production
- **−** npm package supports only Node.js 22.12 through 24.x

<sub>no GPU · Needs Node.js 22.12-24.x (npm package), Tailscale (optional), ngrok (optional), cloudflared (optional) · port 4020 · [Repo](https://github.com/amantus-ai/vibetunnel) · [📖 Docs ↗](https://docs.vibetunnel.sh) · [🌐 Site ↗](https://vibetunnel.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibetunnel/)</sub>

<a name="sidekick-nvim"></a>
### #&#8288;254 [sidekick.nvim](https://github.com/folke/sidekick.nvim) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (50) · Freshness: active (94) · Maintenance: patchy (39) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · Apache-2.0 · Sep 2026</sub>

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

<a name="minuet-ai-nvim"></a>
### #&#8288;255 [minuet-ai.nvim](https://github.com/milanglacier/minuet-ai.nvim) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · GPL-3.0 · Nov 2026</sub>

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

<a name="goraven"></a>
### #&#8288;256 [goraven](https://github.com/8treenet/goraven) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 856 · Apache-2.0 · Nov 2026</sub>

**Self-hosted multi-user agent workspace with tools, RAG and skills.**

GoRaven is a Go server with a React frontend that gives each team member an isolated agent workspace. Agents read and write files, run shell commands, call MCP tools, and retrieve from a shared RAG knowledge base. Admins manage model quotas and tool permissions, and teams share a skill library and lifecycle plugin hooks.

- **+** Per-user isolated workspaces with admin control of model quotas, tools and data access
- **+** Shared skill marketplace and plugin hooks on conversations, tool calls and SSE events
- **+** Works with OpenAI, Claude, DeepSeek, Qwen, GLM or any compatible API
- **+** Docker image bundles Go, Node.js, Python and Git; setup wizard on port 8000
- **−** Building from source means setting up Go, Node.js and Python yourself
- **−** Deliberately has no agent memory or self-evolution feature
- **−** No sandboxing details given for agent shell execution
- **−** Built as a team server, not a starter template to fork

<sub>no GPU · Needs Docker · Models: OpenAI, Claude, DeepSeek, Qwen, GLM · port 8000 · [Repo](https://github.com/8treenet/goraven) · [▶️ Demo ↗](https://preview.goraven.dev) · [🌐 Site ↗](https://goraven.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goraven/)</sub>

<a name="happyclaw"></a>
### #&#8288;257 [happyclaw](https://github.com/riba2534/happyclaw) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 848 · MIT · Nov 2026</sub>

**Multi-user web and chat-app workbench that runs Claude Code agents long-term.**

HappyClaw wraps the Claude Agent SDK and Claude Code runtime in a multi-user Node.js service. Agents work in isolated workspaces, either on the host or in non-root Docker containers, and are reachable from a web UI/PWA and eight messaging channels (Feishu, Telegram, QQ, DingTalk, WeChat, WeCom, Discord, WhatsApp). It adds scheduled automations, per-workspace memory, Skills/MCP/Plugins management, usage tracking and RBAC.

- **+** Uses the pinned Claude Code runtime and Agent SDK instead of reimplementing the tool loop
- **+** Eight IM channels with multi-account support and explicit per-session binding
- **+** Host or Docker execution per workspace; members are forced into containers
- **+** Scheduled automations with stop conditions, quiet mode and missed-run tracking
- **−** Single-user host mode gives the agent full host filesystem access
- **−** Docker needed for multi-user deployment; agent image pulled from Docker Hub
- **−** README is Chinese-first; English docs not evident
- **−** No tagged releases; runs from git clone with make start

<sub>no GPU · Needs Node.js 22+, npm, GNU Make, Docker (multi-user/container workspaces), SQLite · Models: Anthropic (API key or Claude subscription), ChatGPT subscription, DeepSeek, Zhipu GLM, Kimi · port 3000 · [Repo](https://github.com/riba2534/happyclaw) · [🌐 Site ↗](https://happyclaw.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/happyclaw/)</sub>

<a name="tim-agent"></a>
### #&#8288;258 [tim-agent](https://github.com/tim-today/tim-agent) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 409 · MIT · Nov 2026</sub>

**Phone-browser access to Claude Code, Codex and Gemini CLI sessions on your PC.**

Tim-Agent is a Go program that runs official coding-agent CLIs (Claude Code, Codex, Gemini, Opcode, Pi) in a local PTY and shares the terminal over a password-protected web page on port 20996. You scan a QR code from a phone to continue the same live session in a mobile browser. It also uploads phone photos and office documents to the PC for the agent, and stores per-project deploy settings in a local vault.

- **+** Drives the unmodified official CLIs, so their updates apply without changes
- **+** Runs locally; asks for no API keys and needs no cloud relay
- **+** Same live session is shared between desktop and phone browser, with PWA install
- **+** Deploy credentials kept in ~/.tim-agent/vault/ with 0600 permissions, not in the repo
- **−** Remote access depends on LAN, Tailscale or FRP set up separately
- **−** Attachments limited to images and office documents; code files, zips and videos are excluded
- **−** Does not implement an agent itself; requires the CLIs installed and authenticated
- **−** Security of the web terminal rests on a single shared password

<sub>no GPU · Needs Claude Code, Codex, Gemini, Opcode or Pi CLI, Tailscale or FRP (optional, for remote access) · Models: Claude Code, OpenAI Codex, Gemini CLI, Opcode, Pi · port 20996 · [Repo](https://github.com/tim-today/tim-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tim-agent/)</sub>

<a name="opencommit"></a>
### #&#8288;259 [opencommit](https://github.com/di-sukharev/opencommit) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (73) · Freshness: recent (70) · Maintenance: patchy (36) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · MIT · Nov 2026</sub>

**CLI that writes git commit messages from staged diffs using an LLM.**

OpenCommit is an npm-installed CLI (`oco`) that sends your staged diff to an LLM and commits with the generated message. It supports OpenAI, Anthropic, Azure, Gemini, Ollama, llama.cpp, Flowise, DeepSeek and OpenRouter, and can run as a prepare-commit-msg hook or a GitHub Action that rewrites commit messages on push.

- **+** Works with local models via Ollama or llama.cpp, so diffs need not leave your machine
- **+** prepare-commit-msg hook integrates with IDE source control and allows editing before commit
- **+** Per-repo .env and global ~/.opencommit config, plus .opencommitignore to exclude files from the prompt
- **+** Supports conventional-commit or commitlint prompt modules, GitMoji, and multiple output languages
- **−** GitHub Action is marked beta and rewrites history via rebase, changing commit SHAs
- **−** Last tagged release is from 2023-05-21 despite recent commits
- **−** Default input limit is 4096 tokens, so large diffs may need tuning
- **−** README contradicts itself on default model: gpt-4o-mini in config, 3.5-turbo in payments

<sub>no GPU · Needs Node.js, npm, git, LLM provider API key or local Ollama/llama.cpp server · Models: OpenAI, Anthropic, Azure OpenAI, Gemini, Ollama · [Repo](https://github.com/di-sukharev/opencommit) · [🌐 Site ↗](https://www.npmjs.com/package/opencommit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencommit/)</sub>

<a name="dlyzzt-pi-desktop"></a>
### #&#8288;260 [dlyzzt/pi-desktop](https://github.com/dlyzzt/pi-desktop) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 358 · Apache-2.0 · Nov 2026</sub>

**Electron desktop app for the Pi Coding Agent with built-in browser.**

Pi Agent Desktop is an Electron and React app that wraps the Pi Coding Agent in a GUI with sessions, project files, Git worktrees, MCP servers, Skills and Plugins. It adds an embedded Chromium browser the agent can drive, managed dev-server processes, and WeChat, Telegram and Feishu/Lark channels. It reads existing Pi CLI data from ~/.pi/agent/ and ships installers for macOS, Windows x64 and Linux x64.

- **+** Reuses Pi CLI sessions and config from ~/.pi/agent/, no migration needed
- **+** Browser, process and tool permissions are separate, with per-session grants and confirmations
- **+** Auto model routing between a fast and a strong model, with optional decision model
- **+** No internal TCP port for UI or control; Renderer uses Electron sandbox and strict CSP
- **−** Managed background processes are not a sandbox; children get the agent's local file and network access
- **−** Private-network protection in the browser is partial; Strict mode rejects requests without a network sandbox
- **−** No Windows ARM64 or 32-bit builds; Linux is AppImage only with manual updates
- **−** Main README is in Chinese; the English version is in a separate file

<sub>no GPU · Needs Node.js 22.19+ (source builds only), Model provider API key or OAuth login · Models: Pi Coding Agent providers (API key, subscription, OAuth), OpenRouter, OpenAI, Azure, MCP servers (stdio, Streamable HTTP) · [Repo](https://github.com/dlyzzt/pi-desktop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dlyzzt-pi-desktop/)</sub>

<a name="byteask-cli"></a>
### #&#8288;261 [byteask/cli](https://github.com/byteask/cli) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 968 · Apache-2.0 · Nov 2026</sub>

**Terminal coding agent forked from Codex CLI, with C and C++ debugging tools.**

ByteAsk CLI is a Rust fork of OpenAI Codex CLI that reads your repo, runs commands in a sandbox and asks for approval of each change. It adds C and C++ tools: clang-tidy, cppcheck, sanitizer builds, gdb/lldb, rr, perf and struct layout. Models can come from a ByteAsk account, your own OpenAI, Anthropic or Gemini key, a ChatGPT plan, or any OpenAI-compatible endpoint.

- **+** Native C/C++ tools: sanitizers, gdb/lldb, rr, perf, clang-tidy, cppcheck
- **+** Works with own key, ChatGPT plan, or OpenAI-compatible endpoints like vLLM and Ollama
- **+** Non-interactive `byteask exec` and `byteask review` for scripts and CI
- **+** Follows Codex CLI config format and manages MCP servers
- **−** Prebuilt binaries only for Linux x86_64/arm64, Apple silicon macOS, Windows x86_64
- **−** Releases up to v0.2.4 were built before the source was published
- **−** ByteAsk account mode routes code context through the hosted gateway
- **−** Sends usage records to ByteAsk unless BYTEASK_NO_TELEMETRY=1 is set

<sub>no GPU · Needs gdb or lldb, clang-tidy, cppcheck, rr, perf · Models: OpenAI, Anthropic, Gemini, ChatGPT Plus/Pro, OpenAI-compatible endpoints (vLLM, Ollama) · [Repo](https://github.com/byteask/cli) · [📖 Docs ↗](https://github.com/ByteAsk/cli/blob/main/docs/byteask/usage.md) · [🌐 Site ↗](https://byteask.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/byteask-cli/)</sub>

<a name="metaharness"></a>
### #&#8288;262 [metaharness](https://github.com/ruvnet/metaharness) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 764 · MIT · Nov 2026</sub>

**Generator that scaffolds a repo-specific agent harness as an npm package.**

MetaHarness generates an npm-publishable agent harness for a repo from a GitHub URL or a template, using the `npx metaharness` CLI or a browser Studio. The output includes agents, skills, slash commands, an MCP server with a default-deny policy, scoped memory and signed provenance. It targets ten hosts, including Claude Code, Codex, Copilot, OpenCode and GitHub Actions, and has 19 vertical templates.

- **+** One scaffold targets ten hosts, including Claude Code, Codex, Copilot, OpenCode and GitHub Actions
- **+** MCP output is default-deny: no network, no shell, no file-write, audit on
- **+** `score` and `analyze-repo` read a repo without executing it
- **+** `mcp-scan` statically flags shell/network grants and wildcard permissions in agent tools
- **−** It generates harnesses rather than running agents, so you still need a host and a model
- **−** Several packages (ARC-AGI-3, AVO) are private or experimental, with performance claims unproven
- **−** README is long and dense with ADR references, so the core workflow is hard to find
- **−** Darwin Mode evolution is validated mainly on SWE-bench Lite; broader gains are not shown

<sub>no GPU · Needs Node.js, npm · Models: Model-agnostic, GLM/Qwen LoRA tuning via weight-eft (GPU-gated) · [Repo](https://github.com/ruvnet/metaharness) · [▶️ Demo ↗](https://ruvnet.github.io/metaharness/) · [📖 Docs ↗](https://github.com/ruvnet/metaharness/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://ruvnet.github.io/metaharness/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/metaharness/)</sub>

<a name="swe-af"></a>
### #&#8288;263 [swe-af](https://github.com/agent-field/swe-af) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Multi-agent runtime that plans, codes, reviews and merges repo changes.**

SWE-AF runs on the AgentField control plane and registers a `swe-planner` node. A `build` call with a goal and a repo URL or path starts planning, coding, review, QA and merge agents, each coder in its own git worktree. Failed issues go through retry, issue-advisor and DAG-replanning loops. Runtimes include AForge, Claude Code, OpenCode, Codex and Command Code, and one build can change several repos.

- **+** Three nested control loops: coder retry, issue advisor, and replanning of the remaining DAG
- **+** Per-role model mapping (coder, qa, architect) across Claude, OpenRouter, OpenAI and Google
- **+** Parallel coders in isolated git worktrees; checkpointed builds can resume with resume_build
- **+** Multi-repo builds with primary and dependency roles in a single call
- **−** Requires an AgentField control plane plus an LLM provider key; not standalone
- **−** Labeled public beta and has no tagged release
- **−** Cost scales with agent count: the example PR used 79 invocations and $19.23
- **−** Command Code runtime is not supported on the Go node

<sub>no GPU · Docker + Compose · Needs AgentField control plane (af), Python 3.12+, LLM provider API key (Anthropic, OpenRouter, OpenAI or Google), GH_TOKEN for private repos and PRs, PostgreSQL (Railway deploy) · Models: Claude, OpenRouter models, OpenAI Codex, Google, MiniMax · port 8080 · [Repo](https://github.com/agent-field/swe-af) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/swe-af/)</sub>

<a name="imcodes"></a>
### #&#8288;264 [imcodes](https://github.com/im4codes/imcodes) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 965 · custom license · Nov 2026</sub>

**Web and mobile control layer for coding agents, with shared memory.**

IM.codes lets you reach terminal-based coding agents (Claude Code, Codex, Gemini CLI, Copilot, Cursor, OpenCode and others) from a browser, iOS app or Apple Watch. It adds cross-provider shared memory, a managed MCP server for memory, messaging and cron, supervised auto-continue, and OpenSpec Auto Deliver runs. It also enrolls other machines as Controlled Nodes for scoped commands and Windows remote desktop.

- **+** Works across many agent CLIs with one shared memory layer and managed MCP tool surface
- **+** Remote terminal, file browser, git diffs and localhost preview from phone or browser
- **+** Supervision and Auto Deliver fail closed and never stage, commit or push code
- **+** Controlled Nodes have per-node credentials and owner-revocable execution access
- **−** Author states no warranty, SLA or stability, security or compatibility guarantees
- **−** Remote desktop works only on Windows nodes; macOS and Linux support is planned
- **−** Enterprise shared context is described as not fully production-tested
- **−** Server-side memory recall uses pgvector; self-hosting steps are not in the visible README

<sub>no GPU · Compose · Needs Postgres with pgvector (server-side memory recall), Chrome DevTools Protocol (browser automation), Open Computer Use · Models: Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor · [Repo](https://github.com/im4codes/imcodes) · [▶️ Demo ↗](https://app.im.codes) · [🌐 Site ↗](https://im.codes) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/imcodes/)</sub>

<a name="baize"></a>
### #&#8288;265 [baize](https://github.com/xu123-bob/baize) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 654 · MIT · Nov 2026</sub>

**Terminal coding agent that redacts PII before sending prompts to the LLM.**

Baize is a Python CLI coding agent with bash, file editing, search, web fetch, skills, subagents, hooks and MCP support. Before each request it replaces 30+ types of sensitive data (phones, emails, API keys, DB strings) with random placeholders, restores them in the response, and redacts session files and logs on disk. It works with DeepSeek, Qwen, Kimi, GLM, OpenAI-compatible endpoints and local Ollama.

- **+** Reversible placeholder redaction of 30+ PII types, also applied to session files and audit logs
- **+** Switches between DeepSeek, Qwen, Kimi, GLM, OpenAI and Ollama by editing one config line
- **+** Extensible with skills, subagents, shell/Python hooks and MCP servers
- **+** Command allowlist and path-escape checks restrict actions to the working directory
- **−** Command allowlist limits shell commands to a small set such as ls, cat, grep, git, python3
- **−** SPSS analysis needs a licensed local IBM SPSS install and works mainly on Windows
- **−** Install steps are Windows-centric and API keys must be edited by hand in .env
- **−** Web/Docker deployment is described briefly, with no stated port

<sub>GPU optional · Needs Python 3.10+, Ollama (optional, local models), Docker (optional, web deployment), IBM SPSS Statistics (optional), Microsoft ODBC Driver 18 (optional, SQL Server) · Models: DeepSeek, Qwen, Kimi, GLM, OpenAI · [Repo](https://github.com/xu123-bob/baize) · [🌐 Site ↗](https://baize-agent-website.pages.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/baize/)</sub>

<a name="hyperfide-oss"></a>
### #&#8288;266 [hyperfide-oss](https://github.com/sidiora-labs/hyperfide-oss) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 622 · Apache-2.0 · Nov 2026</sub>

**Single-binary agent workflow engine with code graph, spec tasks and memory.**

Hyperfide is a single `hyperfide` CLI that indexes a repository into a local SQLite graph (symbols, calls, routes, full-text search) and pairs it with a spec-driven task board, snapshots and an agent memory. It exposes these over a built-in MCP server with 71 tools, and `hyperfide fleet up` supervises Codex or Claude Code agents in worktrees until work is qualified and merged. The core loop runs locally with no telemetry; a few opt-in commands call external models.

- **+** Local SQLite graph and memory under .codegraph/, no telemetry in the core loop
- **+** Built-in MCP server with 71 tools, plus `hyperfide integrate` for host configs
- **+** `spec done` is gated by verify_cmd and graph checks, not self-reported
- **+** Fleet supervisor is crash-resumable and checks branch drift before merge
- **−** Large command surface and spec format (kvx) to learn before the loop pays off
- **−** Language coverage varies from native extraction to file-only tracking
- **−** Jev, changelog highlights and recap need external API keys (OpenRouter, Centra)
- **−** Fleet mode drives only Codex CLI or Claude Code agents

<sub>no GPU · Needs Node 22.19.0 and pnpm 9.15 (dev), SQLite, Codex CLI or Claude Code (fleet), gh (fleet pr, checkpoint), OPENROUTER_API_KEY (optional, Jev), CENTRA_API_KEY (optional, changelog, recap) · Models: Codex CLI, Claude Code, OpenRouter (Jev) · [Repo](https://github.com/sidiora-labs/hyperfide-oss) · [📖 Docs ↗](https://github.com/sidiora-labs/hyperfide-oss/blob/main/docs/hyperfide/platform.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hyperfide-oss/)</sub>

<a name="facadecode"></a>
### #&#8288;267 [facadecode](https://github.com/y5ez3g/facadecode) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 564 · MIT · Nov 2026</sub>

**VS Code extension that runs and coordinates multiple coding agent CLIs.**

Facade Code is a VS Code extension, plus a preview VS Code fork, that runs native agent CLIs (Claude Code, Codex, Antigravity, Muse Code, OpenCode, Pi) in editor terminal tabs with a status card per agent. Agents can start, message and control each other through MCP and a terminal protocol, across windows and over Remote SSH. It uses each CLI's own sign-in and plan.

- **+** Supports six agent CLIs using their own accounts and plans
- **+** Agents can start, message and read terminals of other agents via MCP
- **+** Agent mesh spans multiple windows and Remote SSH machines
- **+** Per-agent Git worktrees; agents keep running through window reloads
- **−** Agents run without approval prompts by default (yolo enabled)
- **−** Requires separately installed and signed-in agent CLIs
- **−** Standalone IDE is a preview and a fork that shares no settings with VS Code
- **−** Binaries for macOS Apple silicon, Linux x64 and Windows x64 only

<sub>no GPU · Needs VS Code, Claude Code, Codex, Antigravity, Muse Code, OpenCode, Pi · Models: Claude Code, Codex, Antigravity, Muse Code, OpenCode · [Repo](https://github.com/y5ez3g/facadecode) · [▶️ Demo ↗](https://facadecode.com) · [🌐 Site ↗](https://facadecode.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/facadecode/)</sub>

<a name="github-copilotforxcode"></a>
### #&#8288;268 [github/copilotforxcode](https://github.com/github/copilotforxcode) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: weak (9) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Sep 2026</sub>

**GitHub Copilot chat, agent mode and completions inside Xcode.**

A macOS host app plus Xcode Source Editor extension that adds GitHub Copilot inline completions, chat and an agent mode to Xcode. Agent mode can edit files, run terminal commands, search the codebase and call configured MCP tools. It requires a GitHub account and signs in with a device code flow.

- **+** Lives in Xcode's Editor menu with configurable key bindings; tab accepts suggestions
- **+** Agent mode edits files, runs terminal commands and supports user-configured MCP tools
- **+** Installs via Homebrew cask or dmg, with in-app update checks
- **+** MIT-licensed client with a release in August 2026
- **−** Needs a GitHub account; the Copilot service behind it is hosted, not self-hostable
- **−** Requires Background, Accessibility and Xcode Source Editor Extension permissions
- **−** Xcode must be restarted after each update
- **−** Xcode's Predictive code completion should be disabled to avoid conflicts

<sub>no GPU · Needs GitHub account, GitHub Copilot service, macOS 13+, Xcode 14+ · [Repo](https://github.com/github/copilotforxcode) · [🌐 Site ↗](https://github.com/features/copilot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/github-copilotforxcode/)</sub>

<a name="clawcodex"></a>
### #&#8288;269 [clawcodex](https://github.com/agentforce314/clawcodex) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 927 · MIT · Nov 2026</sub>

**Python rebuild of Claude Code with TUI, web UI and desktop app.**

ClawCodex is a coding agent CLI that reads a repo, edits files and runs commands, ported from the TypeScript Claude Code reference into Python. The TUI, a browser UI (`clawcodex web`, port 8081) and an Electron desktop app share one in-process agent core and session store. It supports about 30 providers, multi-agent teams under a session supervisor, a `--nano` minimal mode and `/eco` output compression.

- **+** Sessions, config and permissions shared across TUI, web UI and desktop app
- **+** About 30 providers; fusion models add image input to text-only models
- **+** Reports 72/89 on Terminal-Bench 2.1 with Claude Opus 5 (single run)
- **+** Multi-agent teams with a supervisor, concurrency and depth limits
- **−** Teams are in-process only, one per workspace, no automatic crash recovery
- **−** Full Access permission is the default; change it with /permissions
- **−** Benchmark is the maintainers' own k=1 run, compared against k=5 board averages
- **−** Fast release churn; README is dense with release notes

<sub>no GPU · Needs Python 3.10+, uv, Git Bash (Windows), LLM provider API key, Tavily API key (optional, WebSearch) · Models: DeepSeek, Anthropic Claude, OpenAI, OpenRouter, Groq · port 8081 · [Repo](https://github.com/agentforce314/clawcodex) · [🌐 Site ↗](https://clawcodex.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/clawcodex/)</sub>

<a name="smithers"></a>
### #&#8288;270 [smithers](https://github.com/smithersai/smithers) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 451 · MIT · Nov 2026</sub>

**Runs repo-defined flows that turn issues into tested changes for review.**

Smithers is a CLI and set of npm libraries that run flows stored beside your code to turn issues into tested changes for review. When enabled, it also keeps the project wiki current. A hosted app at smithers.sh lets you browse a repo, chat about it and inspect runs.

- **+** Flows are defined in the repo next to the code they maintain
- **+** `smthrs init change` scaffolds a starter flow from npm install
- **+** Optional wiki upkeep in addition to issue-to-change automation
- **+** MIT licensed, written in TypeScript
- **−** Needs Node.js 22.19+; certified only on Linux with Node 26.4.0
- **−** CLI installs from the `next` tag, and the README refers to a release candidate
- **−** Scaffolded flow must be edited and a model credential set before first run

<sub>Needs Node.js 22.19+, Model credential required by the flow's model field, GitHub account (hosted app sign-in) · [Repo](https://github.com/smithersai/smithers) · [▶️ Demo ↗](https://smithers.sh/smithersai/smithers) · [📖 Docs ↗](https://smithers.sh/docs/) · [🌐 Site ↗](https://smithers.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/smithers/)</sub>

<a name="tabby"></a>
### #&#8288;271 [Tabby](https://github.com/tabbyml/tabby) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (93) · Freshness: recent (75) · Maintenance: weak (8) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · custom license · Jun 2026</sub>

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

<a name="continuous-claude"></a>
### #&#8288;272 [continuous-claude](https://github.com/anandchowdhary/continuous-claude) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (31) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Shell loop that runs Claude Code or Codex through branch, PR, CI and merge.**

A Bash script (with a PowerShell port) that repeatedly invokes Claude Code or Codex CLI on a prompt. Each iteration creates a branch, commits, opens a GitHub PR with gh, waits for checks and reviews, then merges or discards the work. A SHARED_TASK_NOTES.md file carries context between iterations, and runs stop on limits for runs, cost or duration, or after repeated completion signals.

- **+** Respects GitHub branch protection, required checks and code owner approval before merging
- **+** Stops on run count, USD cost or duration limits, with stall and rate-limit throttling flags
- **+** Supports Claude Code and Codex, with an optional separate provider for reviewer passes
- **+** Git worktree flag allows parallel loops on the same repository
- **−** Full PR automation requires GitHub; Gitea and other forges are not supported
- **−** Failed iterations close the PR and discard the work, which costs tokens
- **−** PowerShell runner lacks worktrees, self-update and automatic CI/comment retry
- **−** Codex cost budgets need token rates passed manually, since Codex reports no USD cost

<sub>no GPU · Needs Claude Code CLI or Codex CLI, GitHub CLI (gh), jq (Bash runner), Git · Models: Claude Code, Codex CLI · [Repo](https://github.com/anandchowdhary/continuous-claude) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/continuous-claude/)</sub>

<a name="arbor"></a>
### #&#8288;273 [arbor](https://github.com/ruc-nlpir/arbor) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**Research agent that grows a hypothesis tree to optimize code against a benchmark.**

Arbor runs a Coordinator and Executor agent loop that proposes hypotheses, edits code in isolated git worktrees, and runs experiments against a user-supplied benchmark. Changes merge into a per-run trunk only if they clear a configurable margin on a held-out test split. It ships as a Python CLI, a keyless MCP server, and a Codex/Claude Code skill suite.

- **+** Held-out test split gates merges, with a configurable margin against overfitting
- **+** Each Executor works in its own git worktree; main is untouched until you merge
- **+** Keyless mode runs inside Claude Code or Codex using the host model
- **+** Offline replay demo and a CPU-only NumPy example task need no API key
- **−** Needs a runnable eval script, dev/test data, and a clean git repo
- **−** Native runtime requires an LLM provider key or local model
- **−** Headline benchmark gains are the authors' own results, not independently checked
- **−** Keyless MCP server is an optional extra with a separate install

<sub>no GPU · Needs Python >=3.10, Git, LLM provider API key or local model (Ollama) · Models: Anthropic, OpenAI Responses API, OpenAI-compatible via LiteLLM (DeepSeek, Gemini, Qwen, vLLM, Ollama) · port 8765 · [Repo](https://github.com/ruc-nlpir/arbor) · [▶️ Demo ↗](https://RUC-NLPIR.github.io/Arbor/demo.html) · [📖 Docs ↗](https://RUC-NLPIR.github.io/Arbor/docs/) · [🌐 Site ↗](https://RUC-NLPIR.github.io/Arbor/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/arbor/)</sub>

<a name="easy-agent"></a>
### #&#8288;274 [easy-agent](https://github.com/conardli/easy-agent) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Terminal coding agent with permission rules and optional OS-level shell sandbox.**

Easy Agent (`eagent`) is a Node.js terminal agent that reads a repository, edits files, and runs shell commands, with each risky action checked against allow/ask/deny rules and workspace trust. It supports Anthropic, OpenAI-compatible, Gemini and local models such as Ollama, and extends through MCP, skills, hooks and plugins. It also runs headless with JSON/NDJSON output, as an SDK, and over JSON-RPC or ACP.

- **+** Layered permissions: deny rules win, workspace trust, plan mode, fail-closed Seatbelt/bubblewrap sandbox
- **+** Headless -p mode with JSON/NDJSON output, plus SDK, JSON-RPC and ACP for Zed/JetBrains
- **+** Anthropic, OpenAI-compatible, Gemini and Ollama profiles configured in settings.json
- **+** No telemetry; /rewind restores files from checkpoints
- **−** Shell sandbox unavailable on Windows; an enabled fail-closed sandbox blocks PowerShell
- **−** Linux sandbox needs bubblewrap, socat, rg and unprivileged user namespaces
- **−** Not accepting external pull requests yet
- **−** Requires Node.js 22 or newer; no tagged release on GitHub

<sub>no GPU · Needs Node.js 22+, npm, model provider credentials, bubblewrap, socat, rg (Linux sandbox), rg (macOS sandbox) · Models: Anthropic, OpenAI-compatible, Gemini, Ollama and other local models · [Repo](https://github.com/conardli/easy-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/easy-agent/)</sub>

<a name="fractal"></a>
### #&#8288;275 [fractal](https://github.com/plasma-ai/fractal) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 799 · Apache-2.0 · Oct 2026</sub>

**Tree of autonomous coding-agent loops, each in its own git worktree.**

Fractal runs autonomous agent loops as a tree: each node iterates toward a goal in its own git worktree and can spawn child nodes for separable subtasks. It drives Claude Code, Codex, Grok Build, OpenCode or Oh My Pi, with caps on iterations, depth, children, cost and time. Run state and cost go to a local SQLite database, viewable in a terminal UI.

- **+** Per-node caps on iterations, depth, children, cost and time bound each loop
- **+** Supports five agent backends, plus OpenRouter routing for Claude and Codex
- **+** All runs, steps and costs tracked in one local SQLite database
- **+** Terminal UI dashboard lets an operator steer or stop nodes live
- **−** Agents run with approval prompts disabled by default, using your credentials
- **−** Worktrees isolate only the git branch, not filesystem or network
- **−** Default mode needs tmux; headless mode is the fallback
- **−** No release published; requires a supported agent CLI installed separately

<sub>no GPU · Needs git, tmux, SQLite, plasma-wiki, agent CLI (Claude Code, Codex, Grok Build, OpenCode or Oh My Pi) · Models: Claude Code, Codex, Grok Build, OpenCode, Oh My Pi · [Repo](https://github.com/plasma-ai/fractal) · [📖 Docs ↗](https://docs.plasma.ai/fractal) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fractal/)</sub>

<a name="devo"></a>
### #&#8288;276 [devo](https://github.com/7df-lab/devo) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 347 · MIT · Nov 2026</sub>

**Rust coding agent with a persistent Python workspace and child agents.**

Devo is a terminal TUI/CLI and desktop agent built on a local Rust runtime. Its `ipython` tool keeps Python variables across calls, and the agent can spawn child agents with their own sessions, models and reasoning levels. It connects to OpenAI-compatible Chat Completions, OpenAI-compatible Responses, or Anthropic Messages endpoints, and supports MCP, skills and resumable sessions.

- **+** Persistent Python state across tool calls lets the agent filter and reuse large outputs
- **+** Child agents get their own sessions and can pick a different model and thinking level
- **+** Works with OpenAI-style and Anthropic APIs; catalog includes DeepSeek, Qwen, Kimi, GLM, MiniMax
- **+** Ships as desktop app and terminal CLI, with MCP, skills and session resume
- **−** Pre-1.0: README warns APIs and configuration may change
- **−** Python kernels run as trusted user-privileged processes, not OS-isolated
- **−** Installed via curl-pipe-to-shell scripts; no Docker image
- **−** Windows shell commands require Git for Windows and a one-time sandbox setup

<sub>no GPU · Needs Git for Windows (Windows only), model provider API endpoint · Models: OpenAI-compatible Chat Completions, OpenAI-compatible Responses, Anthropic Messages, DeepSeek, Qwen · [Repo](https://github.com/7df-lab/devo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devo/)</sub>

<a name="copilotforxcode"></a>
### #&#8288;277 [intitni/copilotforxcode](https://github.com/intitni/copilotforxcode) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (74) · Freshness: active (90) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Oct 2026</sub>

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

<a name="autokernel"></a>
### #&#8288;278 [autokernel](https://github.com/rightnow-ai/autokernel) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**Agent loop that profiles PyTorch models and optimizes Triton or CUDA kernels.**

AutoKernel profiles a PyTorch model with torch.profiler, extracts the top bottleneck kernels as standalone Triton or CUDA C++ files, and has a coding agent edit, benchmark and keep or revert each one. A fixed bench.py runs 5-stage correctness checks and roofline analysis, and verify.py checks end-to-end results. It also includes KernelBench integration and decode-step and TTFT benchmark scripts for serving engines.

- **+** Fixed benchmark with 5-stage correctness checks gates each agent edit before it is kept
- **+** Orchestrator picks the next kernel using Amdahl's law across profiled bottlenecks
- **+** Starter Triton and CUDA C++ kernels for 10 op types, plus GPT-2, LLaMA, BERT models
- **+** Includes KernelBench bridge and decode-step and long-prompt TTFT benchmarks
- **−** Requires an NVIDIA GPU; tested only on H100, A100 and RTX 4090
- **−** Needs an external coding agent such as Claude or Codex to drive program.md
- **−** Each experiment takes about 90 seconds, so gains depend on long unattended runs
- **−** No tagged release; used by cloning the repo and running scripts

<sub>GPU required · Needs uv, PyTorch, Triton, Coding agent (Claude, Codex or similar) · Models: PyTorch models, GPT-2, LLaMA, BERT, HuggingFace transformers (optional extra) · [Repo](https://github.com/rightnow-ai/autokernel) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autokernel/)</sub>

<a name="agentbox"></a>
### #&#8288;279 [agentbox](https://github.com/savannahfeder/agentbox) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 462 · GPL-3.0 · Nov 2026</sub>

**Inbox app that runs many Claude Code and Codex agents in parallel git worktrees.**

Agentbox is an Electron desktop app, also runnable in a browser via `npx agentbox-app`, that spawns one headless Claude Code or Codex session per task, each in its own git worktree and branch. Finished or stuck agents show up as inbox rows with a short summary and numbered options, answered by keyboard. Tasks are ordered by project rank and Urgent/High/Medium/Low tags, and an optional paid-tier-free-trial cloud mode runs agents on remote Linux machines.

- **+** Each agent gets its own git worktree and branch, so parallel agents do not touch the same files
- **+** Uses your existing Claude Code or Codex login; no server or account required
- **+** Priority queue with maxConcurrentSessions; only your own tags affect ordering
- **+** Telemetry is off in source builds and can be disabled in released copies
- **−** Requires Claude Code or Codex installed and signed in; no other agents are supported
- **−** Default sessionArgs grant only store tools; editing code needs a manual config opt-in
- **−** Released builds send usage counts to PostHog unless you turn them off
- **−** Agentcloud is a hosted service; the README gives no pricing beyond a free trial

<sub>no GPU · Needs Claude Code or Codex CLI, Node 22.18+ (source or browser), git, make and C++ compiler on Linux for terminal (optional) · Models: Claude Code, Codex · [Repo](https://github.com/savannahfeder/agentbox) · [🌐 Site ↗](https://agentbox.ac) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentbox/)</sub>

<a name="yylo"></a>
### #&#8288;280 [yylo](https://github.com/yylo-dev/yylo) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (0) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 69 · MIT · Nov 2026</sub>

**CLI that runs coding agents in loops with typed task and merge tracking.**

YYLO is a Node.js CLI (yy, yylo, ypl) that launches coding agents such as Pi and Claude Code, repeats them in bounded loops, and wraps the results in typed task, validation, merge and release-readiness commands. Provider credentials stay external. Validation runs produce content-addressed evidence, and records and benchmarks are delegated to the separate Ledger and Benchmark CLIs.

- **+** Bounded loops: -i limits agent iterations, yy loop -n limits outer workflow steps
- **+** Typed task, merge land and merge project commands with expected-old ref updates
- **+** Strict machine output via --format json|ndjson --raw with a versioned envelope
- **+** Read-only watch and doctor workspace commands inspect state without changing it
- **−** Needs a separately installed agent (e.g. Pi) and provider credentials to do real work
- **−** Ledger and Benchmark are separate installs; Ledger must be exactly 0.4.0 for this source
- **−** Skills come from a separate repo and need network access to install
- **−** Large command surface; source targets 0.2.16 while stable npm is 0.2.2

<sub>no GPU · Needs Node.js 20.10+, npm, Git, Pi coding agent (optional), YYLO Ledger 0.4.0, YYLO Benchmark, yylo-skills ^2.1.2 · Models: Pi (multiple providers), Claude Code (yy cc) · [Repo](https://github.com/yylo-dev/yylo) · [🌐 Site ↗](https://www.npmjs.com/package/%40yylo%2Fcli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yylo/)</sub>

<a name="aideml"></a>
### #&#8288;281 [aideml](https://github.com/wecoai/aideml) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (36) · Freshness: active (83) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**LLM agent that drafts, runs and iterates ML code via tree search.**

AIDE ML is a Python package that takes a dataset, a plain-English goal and a metric, then runs an LLM-driven tree search over generated scripts, executing and scoring each one. It saves the top-scoring script and an HTML solution tree to logs/. It runs from a CLI, a Python API or a Streamlit UI, and works with OpenAI, Anthropic, Gemini, OpenRouter or local OpenAI-compatible endpoints.

- **+** Tree search over code, backed by an arXiv paper and used in MLE-Bench
- **+** Writes best_solution.py and an HTML solution-tree visualiser per run
- **+** OpenAI, Anthropic, Gemini, OpenRouter, or local models via OPENAI_BASE_URL
- **+** MIT license; pip install aideml; CLI, Python API and Streamlit UI
- **−** Fully local runs lose quality; feedback model defaults to gpt-4.1-mini
- **−** Streamlit web UI requires cloning the repo, not just pip install
- **−** Research reference build; broader features are in the paid Weco product
- **−** Executes LLM-generated code locally; sandboxing is not described

<sub>Docker · Needs LLM API key (OpenAI, Anthropic, Gemini or OpenRouter) or local OpenAI-compatible server, Python 3.10+ · Models: OpenAI, Anthropic, Gemini, OpenRouter, Ollama / OpenAI-compatible · [Repo](https://github.com/wecoai/aideml) · [🌐 Site ↗](https://weco.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aideml/)</sub>

<a name="codeagent"></a>
### #&#8288;282 [codeagent](https://github.com/harvil1/codeagent) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Oct 2026</sub>

**Terminal coding agent in Python, modeled on Claude Code, with Chinese comments.**

CodeAgent is a terminal coding assistant that reads code, edits files, runs commands and fetches web pages from natural-language instructions. It connects to any OpenAI-compatible or Anthropic-protocol endpoint (default DeepSeek) and can route compression and memory work to a cheaper auxiliary model. It adds approval panels, long-term memory, skills learned from conversation traces, sub-agents and a workflow engine.

- **+** Works with OpenAI-compatible and Anthropic endpoints; API key via env var or settings.json
- **+** Approval panel for risky commands, plus secret scanning, SSRF guard and optional bwrap sandbox on Linux
- **+** Sub-agents with worktree isolation, team mode, cron tasks, hooks and /rewind checkpoints
- **+** MCP support via project .mcp.json, plus skills and a plugin marketplace through /plugin
- **−** Windows is the primary tested platform; macOS is described as not fully verified
- **−** No tagged release; install is git clone plus uv sync
- **−** README and code comments are mainly Chinese, with a separate English README
- **−** No docs site; documentation is the README and code comments

<sub>no GPU · Needs Python 3.11+, uv, LLM API key (DeepSeek, OpenAI, Anthropic, OpenRouter or ZhipuAI) · Models: DeepSeek, OpenAI-compatible endpoints, Anthropic, OpenRouter, ZhipuAI · [Repo](https://github.com/harvil1/codeagent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codeagent/)</sub>

<a name="aider"></a>
### #&#8288;283 [aider](https://github.com/aider-ai/aider) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: widely used (96) · Freshness: recent (51) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · Apache-2.0 · May 2026</sub>

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

<a name="minicode"></a>
### #&#8288;284 [minicode](https://github.com/liumengxuan04/minicode) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Small terminal coding assistant modeled on Claude Code's agent loop.**

MiniCode is a TypeScript terminal coding agent that runs a model-tool-model loop in a full-screen TUI, with review-before-write file edits and path and command permission checks. It supports up to 3 read-only sub-agents, /goal and /loop workflows, session resume and compaction, SKILL.md skills, and MCP over stdio or HTTP. The codebase is kept small so it can be read and modified as a reference implementation.

- **+** Review-before-write edits with path and command permission checks
- **+** Per-project sessions with resume, fork, auto-compact and context collapse
- **+** Supports MCP (stdio and remote HTTP) and local SKILL.md skills
- **+** Small codebase with architecture docs; ports exist in Rust, Python, Go and Java
- **−** Install is a git clone plus npm script; no published release
- **−** Installer asks for an Anthropic base URL and token; other providers undocumented
- **−** Sub-agents are read-only; only the root agent edits code
- **−** README carries sponsor promotion for a third-party API reseller

<sub>no GPU · Needs Node.js, npm, Anthropic-compatible API endpoint and token · Models: Anthropic-compatible API (configurable model name and base URL) · [Repo](https://github.com/liumengxuan04/minicode) · [📖 Docs ↗](https://github.com/LiuMengxuan04/MiniCode/blob/main/USAGE.md) · [🌐 Site ↗](https://liumengxuan04.github.io/MiniCode/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/minicode/)</sub>

<a name="claude-code-agent-farm"></a>
### #&#8288;285 [claude_code_agent_farm](https://github.com/dicklesworthstone/claude_code_agent_farm) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 925 · custom license · Sep 2026</sub>

**Runs parallel Claude Code sessions in tmux to fix lint errors and apply stack guides.**

A Python orchestrator that launches 20+ Claude Code sessions (up to 50 via max_agents) in tmux panes. It feeds them chunks of type-checker and linter output, or a per-stack guide to implement step by step, and agents work through them in parallel. A third workflow has agents claim files through lock files in a /coordination/ directory. It ships 34 stack configs, per-stack prompts, a monitoring dashboard with auto-restart, and tool setup scripts.

- **+** Ships 34 per-stack configs with prompts and 31 stack guides
- **+** Monitors context use and idle state, restarts agents, writes JSON monitor state
- **+** Cooperating workflow uses lock files and a work registry, with stale-lock handling after 2 hours
- **+** doctor command checks the setup before a run; config values are overridable from the CLI
- **−** Requires launching Claude Code with --dangerously-skip-permissions via the cc alias
- **−** Health checks and context resets assume Claude Code; other CLIs get degraded support
- **−** Conflict avoidance in the cooperating workflow comes from the prompt, not enforced code
- **−** Custom license (MIT plus OpenAI/Anthropic rider), detected as NOASSERTION

<sub>no GPU · Needs Python 3.13+, uv, tmux, git, Claude Code CLI, direnv (optional) · Models: Claude Code, OpenCode (limited), OpenAI Codex CLI (limited) · [Repo](https://github.com/dicklesworthstone/claude_code_agent_farm) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-agent-farm/)</sub>

<a name="dmux"></a>
### #&#8288;286 [dmux](https://github.com/standardagents/dmux) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: known (39) · Freshness: active (97) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Aug 2026</sub>

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

<a name="meta-harness"></a>
### #&#8288;287 [meta-harness](https://github.com/stanford-iris-lab/meta-harness) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: known (39) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Framework that searches for better harness code around a fixed LLM.**

Meta-Harness automates search over task-specific harnesses, the code that decides what a fixed base model stores, retrieves and sees. A coding agent (Claude Code in the examples) proposes harness changes, which are evaluated and logged. The repo includes two paper experiments: memory-system search for text classification and scaffold evolution for Terminal-Bench 2.0.

- **+** Includes two runnable reference experiments from the paper, with uv-based quick-start commands
- **+** ONBOARDING.md guides a coding assistant to produce a domain_spec.md for a new domain
- **+** Proposer agent is swappable by adapting the claude_wrapper.py scripts
- **+** Optimized Terminal-Bench 2 harness is published in a separate artifact repo
- **−** Release note says code was only verified to run, not tested further
- **−** Examples assume Claude Code as proposer; other agents need a custom wrapper
- **−** No tagged release; research code rather than a packaged library
- **−** A new domain requires writing your own harness and evaluation

<sub>Needs uv, Claude Code · Models: Claude Code (proposer agent) · [Repo](https://github.com/stanford-iris-lab/meta-harness) · [🌐 Site ↗](https://yoonholee.com/meta-harness/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/meta-harness/)</sub>

<a name="claude-code-chat"></a>
### #&#8288;288 [claude-code-chat](https://github.com/andrepimenta/claude-code-chat) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · custom license · Sep 2026</sub>

**VS Code and Cursor chat panel that fronts the Claude Code CLI.**

A VS Code extension that wraps the Claude Code CLI in a chat panel, with inline diffs, permission prompts, and Git-based checkpoints to roll back edits. It also includes a marketplace for installing MCP servers, skills and plugins, and can switch models, including 150+ through OpenCredits. It works in Cursor and under WSL.

- **+** Git-based checkpoints let you restore code to an earlier conversation state
- **+** Inline diffs, with a button to open VS Code's native side-by-side diff
- **+** Per-tool permission dialogs with always-allow patterns; YOLO mode skips them
- **+** Installs MCP servers to .mcp.json or ~/.claude.json, skills to .claude/skills/
- **−** Needs the Claude Code CLI and a Claude API key or Pro/Max plan
- **−** Non-Claude models go through OpenCredits, a separate provider
- **−** License is not identified by automated detection; the README only points to a LICENSE file
- **−** Tied to VS Code 1.80+ or compatible editors; no standalone app

<sub>no GPU · Needs Claude Code CLI, VS Code 1.80+ or Cursor, Node.js 18+, Claude API key or Pro/Max subscription, Git · Models: Claude Opus, Claude Sonnet, OpenCredits models (GPT, Gemini, MiniMax, Kimi, GLM, DeepSeek) · [Repo](https://github.com/andrepimenta/claude-code-chat) · [🌐 Site ↗](https://marketplace.visualstudio.com/items?itemName=andrepimenta.claude-code-chat) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-chat/)</sub>

<a name="figmatocode"></a>
### #&#8288;289 [figmatocode](https://github.com/bernaferrari/figmatocode) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (66) · Freshness: active (92) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · GPL-3.0 · Aug 2026</sub>

**Figma plugin that converts selections to HTML, Tailwind, Flutter or SwiftUI code.**

A Figma plugin that deterministically converts a selected frame, component or layer into HTML, React, Svelte, styled-components, Tailwind (3 or 4), Flutter or SwiftUI code. It runs inside Figma's plugin sandbox with no AI model and no network access, and can export small starter projects (Vite, Next.js, static HTML, Flutter, SwiftUI). It works in Design and Dev Mode and shows warnings where a target cannot express a design detail.

- **+** Manifest allows no network domains and requests no permissions, so designs are not uploaded
- **+** Covers HTML, React, Svelte, Tailwind 3/4, Flutter and SwiftUI from one selection
- **+** Runs in Design and Dev Mode with no account or generation limits
- **+** Shows conversion warnings instead of silently guessing unsupported details
- **−** No AI inference: no semantics, interactions, state or accessibility are generated
- **−** Cannot read or sync with an existing codebase or components
- **−** Vector support is optional on web and limited on native targets
- **−** GPL-3.0 license; large selections use more memory and process slowly

<sub>no GPU · Needs Figma, Node.js 24+ (development), pnpm 11 (development) · port 3000 · [Repo](https://github.com/bernaferrari/figmatocode) · [▶️ Demo ↗](https://figma-to-code-plugin.vercel.app/#preview) · [🌐 Site ↗](https://figma-to-code-plugin.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/figmatocode/)</sub>

<a name="container-use"></a>
### #&#8288;290 [container-use](https://github.com/dagger/container-use) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (60) · Freshness: recent (72) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Aug 2026</sub>

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

<a name="vibe-figma"></a>
### #&#8288;291 [vibe_figma](https://github.com/vibeflowing-inc/vibe_figma) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 852 · AGPL-3.0 · Oct 2026</sub>

**CLI and REST API that convert Figma frames into React and Tailwind components.**

VibeFigma fetches a Figma frame through the official Figma API using a personal access token and generates React/TypeScript components with Tailwind classes. It runs as an npx CLI (interactive or flag-driven), as a REST API server (POST /v1/api/vibe-figma, default port 3000), and as a Claude Code skill. An optional AI cleanup pass uses a Google Generative AI key.

- **+** Runs with a single npx command; no install needed for the CLI
- **+** Output paths, Tailwind, responsive, absolute positioning and fonts are set by flag
- **+** Also ships a REST API server and a Claude Code skill
- **+** Uses the official Figma API rather than screenshots
- **−** Optional --clean cleanup requires a Google Generative AI API key
- **−** AGPL-3.0 license restricts use in closed-source network services
- **−** Output is React with Tailwind or plain CSS; no other frameworks listed
- **−** No tagged releases on the repository

<sub>no GPU · Docker · Needs Figma personal access token, Google Generative AI API key (optional, for --clean), Bun (for API server) · Models: Google Generative AI (optional code cleanup) · port 3000 · [Repo](https://github.com/vibeflowing-inc/vibe_figma) · [▶️ Demo ↗](https://ui.vibeflow.ai) · [🌐 Site ↗](https://ui.vibeflow.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-figma/)</sub>

<a name="zhikuncode"></a>
### #&#8288;292 [zhikuncode](https://github.com/zhikunqingtao/zhikuncode) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 549 · MIT · Nov 2026</sub>

**Browser coding-agent workbench with sub-agents, tool approvals and phone access.**

ZhikunCode is a self-hosted browser workbench where a model reads a project, edits files and runs commands, with sub-agents, context management and approval prompts. The runtime is Java, with a React front end and a Python capability service and CLI. You choose the model API. A script can open a password-protected temporary HTTPS tunnel so a phone can continue sessions on the same instance.

- **+** Sub-agent task split, tool approvals and run verification in one browser UI
- **+** Model API is your choice; the runtime is self-hosted
- **+** Phone can resume existing sessions and handle approvals without a native app
- **+** Public case studies with logs, evidence files and recorded sessions
- **−** Three-part stack (Java, React, Python) is heavier to run than a single CLI
- **−** Phone access needs the host computer to stay online and awake
- **−** SWE-bench Lite 56.0% result has reference-fix exposure in public trajectories
- **−** README is mostly Chinese; English docs live in a separate file

<sub>Docker + Compose · Needs Model API provider, Python capability service · Models: Kimi K3, GLM-5.2 · [Repo](https://github.com/zhikunqingtao/zhikuncode) · [📖 Docs ↗](https://github.com/zhikunqingtao/zhikuncode/blob/main/docs/README_EN.md) · [🌐 Site ↗](https://zhikunqingtao.github.io/zhikuncode/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zhikuncode/)</sub>

<a name="49-ide"></a>
### #&#8288;293 [49-ide](https://github.com/49-agents/49-ide) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: weak (22) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 586 · custom license · Sep 2026</sub>

**Infinite-canvas workspace for tmux terminals and coding agents across machines.**

49 Agents IDE places real tmux terminals (via ttyd), a Monaco editor, a git graph, Beads issue tables and markdown notes as panes on one zoomable canvas. Agents on multiple machines connect to a single relay without SSH, and panes show Claude status and permission notifications. The server runs locally on port 1071 with no login, or you can use the hosted version.

- **+** Connects agents from several machines to one canvas without SSH
- **+** Real tmux sessions via ttyd keep your shell config and scrollback
- **+** Self-hosted local setup needs no account, login or token
- **+** Broadcast input sends keystrokes to several terminals at once
- **−** BSL 1.1 license, not OSI open source; converts to MIT only on 2030-02-26
- **−** Status and usage features are described mainly for Claude; other agents are unclear
- **−** macOS desktop app is not notarized and needs an xattr workaround
- **−** Terminal I/O passes through a relay, hosted unless you self-host

<sub>no GPU · Needs tmux, ttyd · port 1071 · [Repo](https://github.com/49-agents/49-ide) · [▶️ Demo ↗](https://app.49agents.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/49-ide/)</sub>

<a name="velocity"></a>
### #&#8288;294 [velocity](https://github.com/ishandutta2007/velocity) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 572 · GPL-2.0 · Nov 2026</sub>

**Web IDE for delegating coding tasks to parallel agents on any LLM.**

Open Velocity is an early-stage, web-based agent-first IDE meant to route coding agents to GPT-4, Claude, Gemini, Llama or Deepseek. The implemented part is a TypeScript backend core (newcore/) with a 14-table SQLite layer, a message bus, file-level locks and per-call cost caps for multi-agent swarms. Much of the feature list is described as vision, and the project is marked experimental.

- **+** Swarm backend tracks parent-child agents, with a shared whiteboard message bus
- **+** File-level locks stop parallel agents from colliding on the same file edits
- **+** Records token counts and cost per LLM call, with a MAX_COST_USD swarm ceiling
- **+** Agent memory snapshots allow restore after failures; CLI includes db:backup
- **−** Most headline features are labeled 'the Vision', not implemented
- **−** README says MIT but detected license is GPL-2.0; the conflict is unresolved
- **−** Disclaimer says experimental and not for production use
- **−** No release published; no concrete provider setup documented

<sub>no GPU · Compose · Needs Docker, Docker Compose, Node.js 20+, Python 3.11+, LLM provider API keys · Models: GPT-4, Claude 3.5, Gemini 1.5 Pro, Llama 3, Deepseek · port 3000 · [Repo](https://github.com/ishandutta2007/velocity) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/velocity/)</sub>

<a name="superdesign"></a>
### #&#8288;295 [superdesign](https://github.com/superdesigndev/superdesign) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: popular (73) · Freshness: recent (78) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · custom license · Jun 2026</sub>

**VS Code and Cursor extension that generates UI mockups from prompts.**

SuperDesign is an IDE extension for VS Code, Cursor and Windsurf that generates UI mockups, components and wireframes from natural-language prompts and previews them on a canvas in the editor. Designs are saved locally in `.superdesign/`, and it adds rules so Claude Code or Cursor can design into the canvas. This repo is the original 2025 extension and is no longer maintained; the product is now a web app.

- **+** Runs inside VS Code, Cursor and Windsurf with a design canvas sidebar
- **+** Designs are stored locally in the .superdesign/ folder
- **+** Accepts OpenAI-compatible endpoints, e.g. LM Studio at http://127.0.0.1:1234/v1
- **+** Can reuse a Claude Code or Cursor subscription via rules it installs
- **−** README states the repo is no longer actively maintained
- **−** Active product is a separate web app at superdesign.dev, not this code
- **−** License is reported as NOASSERTION, so reuse terms are unclear
- **−** No tagged releases in the repository

<sub>no GPU · Needs VS Code, Cursor or Windsurf, AI provider API key or OpenAI-compatible server · Models: Claude Code, Cursor, OpenAI-compatible servers (LM Studio) · [Repo](https://github.com/superdesigndev/superdesign) · [▶️ Demo ↗](https://youtu.be/INv6oZDhhUM) · [📖 Docs ↗](https://www.superdesign.dev/ide-extension) · [🌐 Site ↗](https://www.superdesign.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superdesign/)</sub>

<a name="sidex"></a>
### #&#8288;296 [sidex](https://github.com/sidenai/sidex) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: popular (53) · Freshness: active (95) · Maintenance: weak (2) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Aug 2026</sub>

**VS Code workbench ported from Electron to Tauri, with a built-in coding agent.**

SideX ports the VS Code TypeScript workbench to Tauri 2, using a Rust backend and the OS native webview instead of bundled Chromium. It includes Monaco, a PTY terminal, Git, and Open VSX extension installs. A built-in coding agent runs as a local Go server on loopback and uses a model provider you configure, such as Anthropic, OpenAI-compatible APIs, or local servers like Ollama.

- **+** Uses the system webview, no bundled Chromium; README shows 16.4 MB vs 797.8 MB on macOS
- **+** Agent needs no account; keys come from Settings, env vars, CLI logins, or local servers
- **+** Agent server binds to 127.0.0.1 and refuses non-loopback binds without explicit opt-in
- **+** MIT licensed; extensions install from Open VSX
- **−** Extension host and debugger are still in progress
- **−** No pre-built binaries; must build with Rust, Node, and Go 1.26+
- **−** Agent server is a separate manual build; chat panel stays disconnected without it
- **−** RAM savings mostly tested on macOS; Windows WebView2 memory can look higher

<sub>no GPU · Needs Rust, Node.js, Tauri 2, Go 1.26+ (agent server), Open VSX · Models: Anthropic Messages API, OpenAI-compatible /chat/completions, Ollama, LM Studio, llama.cpp · [Repo](https://github.com/sidenai/sidex) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sidex/)</sub>

<a name="multi-agent-shogun"></a>
### #&#8288;297 [multi-agent-shogun](https://github.com/yohey-w/multi-agent-shogun) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (32) · Freshness: active (94) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Aug 2026</sub>

**tmux orchestrator for parallel coding-agent CLIs in a Shogun/Karo/Ashigaru hierarchy.**

Shell scripts that launch one Shogun, one Karo, seven Ashigaru workers and one Gunshi strategist as separate coding-agent CLIs in tmux panes. Agents coordinate through YAML files on disk rather than API calls. It supports Claude Code, Codex, Copilot, Kimi, OpenCode, Cursor and Antigravity, and adds a dashboard.md progress file and an Android SSH companion app.

- **+** Coordination uses plain YAML files and tmux, so no orchestration API calls or extra infrastructure
- **+** Supports seven agent CLIs, with instruction files generated per CLI from shared templates
- **+** Every agent runs in a visible tmux pane; instructions and reports are readable files
- **+** Android app offers SSH terminal, voice input and a 9-pane agent grid
- **−** Needs tmux and bash 4+; Windows requires WSL2
- **−** Setup runs Claude Code with --dangerously-skip-permissions and bypass-permission prompts
- **−** Android companion only; no iOS client
- **−** Author has moved to a single-agent successor, kagemusha, though this project still works

<sub>no GPU · Needs tmux, bash 4+, Node.js 20+, at least one supported agent CLI, WSL2 (Windows) · Models: Claude Code, OpenAI Codex, GitHub Copilot, Kimi Code, OpenCode · [Repo](https://github.com/yohey-w/multi-agent-shogun) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/multi-agent-shogun/)</sub>

<a name="helmor"></a>
### #&#8288;298 [helmor](https://github.com/dohooo/helmor) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (30) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Jul 2026</sub>

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

<sub>no GPU · Needs GitHub or GitLab account, Cloudflare tunnel (mobile companion, experimental) · Models: Claude Code, Codex, Cursor, OpenCode, Kimi Code · [Repo](https://github.com/dohooo/helmor) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/helmor/)</sub>

<a name="squad"></a>
### #&#8288;299 [squad](https://github.com/bradygaster/squad) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (0) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9 · MIT · Nov 2026</sub>

**CLI that scaffolds a persistent team of AI agents inside a repo.**

Squad installs a team of role-based agents (lead, frontend, backend, tester) as files under .squad/ in your repo, driven mainly through GitHub Copilot. Agents run in parallel and record decisions and per-agent history in markdown committed to git. A watch mode (Ralph) polls issues and dispatches agents, and the team can be projected into Claude Code, Cursor, Codex, Kiro and OpenCode.

- **+** Team state, decisions and agent history live as markdown in git, so clones share them
- **+** Same team can be projected into Claude Code, Cursor, Codex, Kiro, OpenCode and Antigravity
- **+** Watch mode triages GitHub issues on an interval, with tiered error recovery and overnight pause
- **+** Installs via npm, Homebrew, WinGet or a standalone script that bundles Node.js
- **−** Primary workflow depends on GitHub Copilot and the gh CLI
- **−** Recommended Copilot run uses --yolo, which skips per-tool approval prompts
- **−** SDK-first TypeScript config mode is experimental with known bugs
- **−** Interactive shell is deprecated; per-agent model choice does not work in VS Code

<sub>no GPU · Docker · Needs GitHub Copilot, GitHub CLI (gh), Node.js 22.5+ (npm install), git · Models: GitHub Copilot models · [Repo](https://github.com/bradygaster/squad) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/squad/)</sub>

<a name="swe-agent"></a>
### #&#8288;300 [swe-agent](https://github.com/swe-agent/swe-agent) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: widely used (87) · Freshness: recent (59) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Jul 2026</sub>

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

<a name="dao-code"></a>
### #&#8288;301 [dao-code](https://github.com/tigicion/dao-code) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 788 · MIT · Oct 2026</sub>

**Terminal coding agent tuned for DeepSeek V4 with prefix-cache-aware cost control.**

Dao Code (command `dao`) is a TypeScript terminal coding agent that reads code, edits files and runs shell commands behind an approval gate. It targets DeepSeek V4 with 1M context and keeps the system prefix byte-stable to hit DeepSeek's prefix cache; memory and reflection run as cache-reusing forks. It reads Claude Code formats for settings, skills, hooks and MCP configs.

- **+** Reports 95.8% cache hit and ¥1.07 total over 7 real OSS bug-fix tasks, with logs
- **+** Reads Claude Code formats: settings.json, SKILL.md, hooks.json, mcp.json
- **+** Shadow-git checkpoints with /restore, plus crash recovery via `dao -c`
- **+** Layered allow/ask/deny permissions, auto mode and a managed enterprise policy layer
- **−** Built around DeepSeek V4; other providers are not documented in the visible README
- **−** Cost and benchmark figures are self-reported by the author
- **−** Chinese-first design, with a separate zh-CN README
- **−** Terminal UI only; no web or IDE interface described

<sub>no GPU · Needs DeepSeek API key, Node.js >= 20 (npm install; standalone binaries need no Node) · Models: deepseek-v4-pro, deepseek-flash · [Repo](https://github.com/tigicion/dao-code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dao-code/)</sub>

<a name="llm-nvim"></a>
### #&#8288;302 [llm.nvim](https://github.com/huggingface/llm.nvim) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**Neovim plugin for ghost-text code completion backed by llm-ls.**

llm.nvim is a Lua Neovim plugin that shows Copilot-style ghost-text completions by sending requests through the llm-ls language server. It talks to the Hugging Face Inference API, Ollama, OpenAI-compatible endpoints or TGI, and trims each prompt to the configured context window using the tokenizers library. It supports fill-in-the-middle prompts for models such as StarCoder and CodeLlama.

- **+** Four backends: Hugging Face Inference API, Ollama, OpenAI-compatible, TGI
- **+** Prompts sized to context_window using real tokenizers, with a character-count fallback
- **+** Configurable fill-in-the-middle tokens per model, with StarCoder and CodeLlama examples
- **+** Installs via packer, lazy.nvim or vim-plug; llm-ls auto-downloaded or via Mason
- **−** Completion only; the README documents no chat, edit or agent features
- **−** Requires the llm-ls binary, downloaded from GitHub releases on first load
- **−** Hugging Face free Inference API tier is rate limited; PRO plan suggested
- **−** No tagged releases; default llm-ls version pinned at 0.5.3

<sub>Needs Neovim, llm-ls, Hugging Face Inference API, Ollama, OpenAI-compatible server or TGI · Models: bigcode/starcoder, bigcode/starcoder2-15b, codellama/CodeLlama-13b-hf, Ollama models, OpenAI-compatible endpoints · [Repo](https://github.com/huggingface/llm.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llm-nvim/)</sub>

<a name="codexmonitor"></a>
### #&#8288;303 [codexmonitor](https://github.com/dimillian/codexmonitor) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (61) · Freshness: recent (55) · Maintenance: weak (11) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Mar 2026</sub>

**Tauri desktop app for running multiple Codex agents across local workspaces.**

CodexMonitor is a Tauri desktop app that spawns one `codex app-server` per workspace and shows threads, diffs, git state and GitHub issues/PRs in one UI. It supports git worktree and clone agents, a prompt library, Whisper dictation, and an optional remote daemon so Codex can run on another machine, with a work-in-progress iOS client over Tailscale.

- **+** Runs one codex app-server per workspace, with thread resume and unread/running tracking
- **+** Built-in git panel: staged/unstaged diffs, branches, commit log, and GitHub issues/PRs via gh
- **+** Remote daemon mode with a headless daemonctl CLI and Tailscale host detection
- **+** Worktree and clone agents keep parallel tasks isolated under the app data directory
- **−** Requires the Codex CLI; no other coding agents are listed
- **−** README documents only source builds, no prebuilt install steps
- **−** iOS support is marked WIP; terminal and dictation are unavailable on mobile
- **−** Source build needs Node, Rust and CMake, plus LLVM/Clang on Windows

<sub>Needs Codex CLI, Node.js, npm, Rust toolchain, CMake, Git, GitHub CLI (optional), LLVM/Clang (Windows), Tailscale (optional, remote/iOS) · Models: Codex (via codex app-server) · [Repo](https://github.com/dimillian/codexmonitor) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codexmonitor/)</sub>

<a name="core"></a>
### #&#8288;304 [opensumi/core](https://github.com/opensumi/core) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (56) · Freshness: recent (70) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="grok-cli"></a>
### #&#8288;305 [grok-cli](https://github.com/superagent-ai/grok-cli) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (55) · Freshness: recent (72) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · May 2026</sub>

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

<a name="vim-ai"></a>
### #&#8288;306 [vim-ai](https://github.com/madox2/vim-ai) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Oct 2026</sub>

**Vim and Neovim plugin for AI completion, in-place editing and chat.**

vim-ai adds :AI, :AIEdit, :AIChat and :AIImage commands to Vim and Neovim, sending prompts or visual selections to OpenAI's API. It can target any OpenAI-compatible endpoint (OpenRouter, LiteLLM, local servers) and supports third-party provider plugins such as Google Gemini. Chats live in editable .aichat buffers that can include files and command output, and reusable prompts are defined as roles in an .ini file.

- **+** Works on selections or ranges, so only text you pick is sent to the API
- **+** Custom endpoint_url and auth_type allow any OpenAI-compatible server, including local ones
- **+** Roles in .ini files and .aichat files make prompts reusable and combinable
- **+** Chat files can include globbed files, images and command output
- **−** Not an agent: no repo-wide context or tool use beyond exec sections in chat
- **−** Requires Vim or Neovim built with python3 support
- **−** Gemini and other non-OpenAI APIs need a proxy or a separate provider plugin
- **−** Defaults assume an OpenAI API key billed per token; no bundled local model

<sub>no GPU · Needs Vim or Neovim with python3, OpenAI API key or OpenAI-compatible endpoint · Models: OpenAI chat models, OpenAI image generation, OpenAI-compatible APIs (OpenRouter, LiteLLM), Gemini via provider plugin · [Repo](https://github.com/madox2/vim-ai) · [📖 Docs ↗](https://github.com/madox2/vim-ai/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vim-ai/)</sub>

<a name="codegen"></a>
### #&#8288;307 [codegen](https://github.com/salesforce/codegen) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (65) · Freshness: recent (68) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Jun 2026</sub>

**Open code-generation LLMs (CodeGen1, 2, 2.5) from Salesforce Research.**

Model release for the CodeGen1, CodeGen2 and CodeGen2.5 families of code LLMs, ranging from 350M to 16B parameters and published on the Hugging Face Hub. Models load through the transformers AutoModelForCausalLM API, and CodeGen2 adds infill sampling. Training and fine-tuning code is in the separate Jaxformer repository. The README labels the release research-only.

- **+** Loads with standard Hugging Face transformers calls, no custom server needed
- **+** Sizes from 350M to 16B, plus a 7B CodeGen2.5 model
- **+** CodeGen2 supports infill sampling, not only left-to-right completion
- **+** Paper-backed (ICLR 2023), with training code in the Jaxformer repo
- **−** Models date from 2022 to 2023; newest release in the news is July 2023
- **−** README states research-only use, not evaluated for all downstream purposes
- **−** Not an agent or editor: no repo awareness, tools or command execution
- **−** CodeGen2 and CodeGen2.5 examples require trust_remote_code=True

<sub>Needs Hugging Face transformers, PyTorch · Models: CodeGen1 (350M-16B), CodeGen2, CodeGen2.5 7B, Hugging Face Hub · [Repo](https://github.com/salesforce/codegen) · [🌐 Site ↗](https://www.salesforceairesearch.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegen/)</sub>

<a name="collab-public"></a>
### #&#8288;308 [collab-public](https://github.com/collabs-inc/collab-public) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (52) · Freshness: active (81) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · custom license · Jun 2026</sub>

**Desktop workspace that arranges agent terminals and files on an infinite canvas.**

Collaborator is an Electron desktop app for macOS, Windows and Linux that places terminal tiles, markdown notes, code editors and images on a pan-and-zoom canvas. Terminals start in the active workspace folder and are meant for running whatever CLI agent you choose. Files are bound to disk paths and reload on external changes, and all state is stored as JSON in ~/.collaborator/.

- **+** Terminals, Monaco code editor and markdown notes sit side by side on one canvas
- **+** Runs on macOS, Windows (PowerShell and WSL2) and Linux
- **+** Local files and local JSON state; no account required
- **+** File tiles track renames and reload when agents edit files on disk
- **−** Ships no agent of its own; you launch third-party agents in a terminal
- **−** README calls it early-stage and in active development
- **−** Anonymous usage analytics are collected via PostHog
- **−** License is not identified (NOASSERTION), so reuse terms need checking

<sub>no GPU · Needs Node.js 22+ (development), Bun (development), node-pty sidecar, PostHog (analytics) · [Repo](https://github.com/collabs-inc/collab-public) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/collab-public/)</sub>

<a name="integuru"></a>
### #&#8288;309 [integuru](https://github.com/integuru-ai/integuru) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (64) · Freshness: recent (66) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · AGPL-3.0 · May 2026</sub>

**Agent that turns recorded browser traffic into Python code calling internal web endpoints.**

Integuru v0 reads a HAR file and cookies captured from a logged-in browser session, plus a prompt such as "download utility bills". It builds a dependency graph of the requests behind that action and generates runnable Python that calls those internal endpoints. This repo is the original release; the maintainers say the current version is hosted at integuru.com.

- **+** Builds a request dependency graph so dynamic URL parameters are traced to the requests that supply them
- **+** Includes create_har.py to record the HAR and cookies from a browser session
- **+** CLI with options for HAR path, cookie path, max steps and code generation
- **+** Works with 2FA sites by reusing post-login cookies and tokens
- **−** Repo is the earliest version; the maintainers point to a newer hosted product
- **−** Input variables work only for graph generation, not code generation
- **−** Requires OpenAI API access; no other model providers listed
- **−** AGPL-3.0 license may restrict use in closed-source services

<sub>no GPU · Needs OpenAI API key, Poetry, Python 3.12, Browser for HAR capture · Models: gpt-4o, o3-mini, o1, o1-mini, o1-preview · [Repo](https://github.com/integuru-ai/integuru) · [▶️ Demo ↗](https://www.youtube.com/watch?v=7OJ4w5BCpQ0) · [🌐 Site ↗](https://www.integuru.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/integuru/)</sub>

<a name="toad"></a>
### #&#8288;310 [toad](https://github.com/batrachianai/toad) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (54) · Freshness: recent (76) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · AGPL-3.0 · May 2026</sub>

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

<a name="proxyai"></a>
### #&#8288;311 [proxyai](https://github.com/carlrobertoh/proxyai) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: known (41) · Freshness: recent (74) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · May 2026</sub>

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

<sub>Needs JetBrains IDE, Gradle (build from source) · Models: OpenAI, Anthropic, Azure, Mistral, self-hosted models · README: alternative to GitHub Copilot · [Repo](https://github.com/carlrobertoh/proxyai) · [🌐 Site ↗](https://plugins.jetbrains.com/plugin/21056-proxy-ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/proxyai/)</sub>

<a name="hermes-desktop"></a>
### #&#8288;312 [dodo-reach/hermes-desktop](https://github.com/dodo-reach/hermes-desktop) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: known (42) · Freshness: active (82) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Jun 2026</sub>

**Native macOS app for managing Hermes Agent sessions, Kanban, cron and skills.**

A Swift macOS app that works against a Hermes Agent install on the same Mac or over SSH. It reads the host's real sessions, Kanban, cron jobs, skills, files and usage, and embeds a local or SSH terminal plus a hosted `hermes --tui` chat. It keeps no mirror or gateway; state stays on the Hermes host.

- **+** Reads Hermes state in place; no gateway API, daemon or sync mirror needed
- **+** Same views work locally or over SSH, across multiple Hermes profiles
- **+** Files and skills saves are blocked if the host copy changed since opening
- **+** Universal build for Apple Silicon and Intel; builds from source with one script
- **−** macOS 14+ only; no Windows or Linux client
- **−** Release build is ad-hoc signed and not notarized, so Gatekeeper warns
- **−** Useful only with an existing Hermes Agent install; Kanban needs upstream support
- **−** SSH mode requires non-interactive auth and python3 on the remote host

<sub>no GPU · Needs Hermes Agent, python3, hermes CLI, SSH (for remote hosts) · [Repo](https://github.com/dodo-reach/hermes-desktop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hermes-desktop/)</sub>

<a name="chatgpt-vscode"></a>
### #&#8288;313 [chatgpt-vscode](https://github.com/ai-genie/chatgpt-vscode) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (29) · Freshness: recent (70) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · ISC · Oct 2026</sub>

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

<a name="deeptide"></a>
### #&#8288;314 [deeptide](https://github.com/paean-ai/deeptide) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (24) · Freshness: active (98) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Aug 2026</sub>

**Terminal coding agent for DeepSeek, with Rust CLI and desktop GUI.**

DeepTide is a terminal coding agent that defaults to the DeepSeek API and can use other Anthropic-compatible endpoints via a base URL and key. The repo covers a Swift macOS app, a Bun-based CLI that forwards to Zero CLI, and a Rust CLI (deeptide-rs) with an egui desktop GUI. It also holds a local DeepSeek V4 Flash Metal runtime (ds4) and a local OpenAI/Anthropic-compatible gateway (dsgo).

- **+** Rust CLI is a single native binary with no runtime, about 10 MB on disk
- **+** Ships 30+ built-in tools, hooks, MCP servers, sub-agents and markdown slash commands
- **+** GUI and CLI share the same settings.json and session store
- **+** Includes local inference source (ds4 and dsgo) for running DeepSeek V4 Flash on Mac
- **−** The deeptide npm package is a thin redirect to Zero CLI and needs Bun at runtime
- **−** Native macOS app is installed from a signed build via a curl script
- **−** CLI configuration docs live in the upstream Zero CLI repo, not here
- **−** Local runtime targets Metal on macOS; larger quants need 128 GB or more of memory

<sub>GPU optional · Needs Bun (for the deeptide npm CLI), DeepSeek API key or other Anthropic-compatible provider · Models: DeepSeek, Anthropic-protocol endpoints, Zhipu GLM, Qwen, Moonshot · [Repo](https://github.com/paean-ai/deeptide) · [🌐 Site ↗](https://deeptide.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deeptide/)</sub>

<a name="ai-doc-gen"></a>
### #&#8288;315 [ai-doc-gen](https://github.com/divar-ir/ai-doc-gen) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (11) · Freshness: active (86) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 772 · MIT · Jul 2026</sub>

**Multi-agent CLI that analyzes a repo and writes README, CLAUDE.md and AGENTS.md.**

Runs five concurrent pydantic-ai agents over a repository to analyze structure, dependencies, data flow, request flow and APIs, saving results to .ai/docs/. Generation commands then produce a README.md plus CLAUDE.md, AGENTS.md and Cursor rules. It works with any OpenAI-compatible endpoint, can run as a GitLab cronjob that opens merge requests, and also installs as a Claude Code plugin with three skills.

- **+** Writes CLAUDE.md, AGENTS.md and .cursor/rules alongside the README from the same analysis
- **+** Any OpenAI-compatible endpoint, with per-agent model and base URL settings
- **+** GitLab cronjob mode opens merge requests for recently active projects; Helm chart included
- **+** Retry client with exponential backoff and Retry-After handling; OpenTelemetry tracing with optional Langfuse
- **−** Requires Python 3.13, which many environments do not ship by default
- **−** Automated merge request mode supports GitLab only; GitHub is not mentioned
- **−** No tagged releases; install is from a git clone
- **−** Output quality depends on the chosen LLM; no evaluation or accuracy figures given

<sub>no GPU · Docker · Needs Python 3.13, Git, OpenAI-compatible LLM API, GitLab (cronjob mode, optional), Langfuse (optional) · Models: OpenAI-compatible APIs, OpenRouter, Anthropic-compatible gateways, local models · [Repo](https://github.com/divar-ir/ai-doc-gen) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-doc-gen/)</sub>

<a name="neovate-code"></a>
### #&#8288;316 [neovate-code](https://github.com/neovateai/neovate-code) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: known (35) · Freshness: recent (52) · Maintenance: weak (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Mar 2026</sub>

**Terminal coding agent that edits code, fixes bugs and writes tests.**

Neovate Code is a command-line coding agent installed from npm as @neovate/code and started with `neovate`. You describe a task in the terminal, review the proposed changes and approve tool calls. It reads API keys from environment variables for each provider, or you can sign in with `/login` and pick a model with `/model`.

- **+** Installs with one npm command; runs on macOS, Linux and Windows
- **+** Respects provider API key environment variables, with /login and /model for setup
- **+** Asks for approval on tool calls and shows proposed changes before applying
- **+** MIT license with a documented quickstart and contributing guide
- **−** Requires Node.js and npm; the README gives no minimum version
- **−** No demo or screenshots of workflows beyond a single image
- **−** README does not describe plugins, MCP support or sandboxing

<sub>no GPU · Needs Node.js, npm, LLM provider API key · [Repo](https://github.com/neovateai/neovate-code) · [📖 Docs ↗](https://neovateai.dev/en/docs/quickstart) · [🌐 Site ↗](https://neovateai.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neovate-code/)</sub>

<a name="termcanvas"></a>
### #&#8288;317 [termcanvas](https://github.com/blueberrycongee/termcanvas) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (3) · Freshness: recent (77) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 421 · MIT · May 2026</sub>

**Electron app that lays out terminals and coding agents on an infinite canvas.**

TermCanvas is a desktop app that arranges shell, lazygit, tmux and AI agent terminals on a pannable, zoomable canvas, organized as Project, Worktree, Terminal to match git worktrees. It supports Claude Code, Codex, Kimi, Gemini and OpenCode with status indicators, session replay and inline diffs. It bundles two CLIs: termcanvas for canvas control, and hydra for Lead-driven multi-agent workflows over git worktrees.

- **+** Worktrees are auto-detected and each one maps to a group of terminals on the canvas
- **+** Status dot per terminal shows whether an agent is thinking, awaiting input, idle or done
- **+** Hydra workflows gate on validated result.json files stored in repo-local .hydra/ directories
- **+** Builds for macOS, Linux and Windows; includes usage and cost tracking for Claude and Codex
- **−** Hydra role-driven workflows currently target only Claude and Codex
- **−** macOS builds are unsigned and may need xattr -cr to launch
- **−** Desktop Electron app only; cloud runtime and remote agents are roadmap items
- **−** Cross-device usage sync requires signing in, backed by Supabase

<sub>Needs pnpm (build from source), Supabase (optional sign-in and sync), Claude Code, Codex, Kimi, Gemini or OpenCode CLIs · Models: Claude Code, Codex, Kimi, Gemini, OpenCode · [Repo](https://github.com/blueberrycongee/termcanvas) · [🌐 Site ↗](https://website-ten-mu-37.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/termcanvas/)</sub>

<a name="trae-agent"></a>
### #&#8288;318 [trae-agent](https://github.com/bytedance/trae-agent) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: widely used (82) · Freshness: quiet (26) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Feb 2026</sub>

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

<a name="octogent"></a>
### #&#8288;319 [octogent](https://github.com/hesamsheikh/octogent) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: known (32) · Freshness: recent (53) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Apr 2026</sub>

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

<a name="supercoder"></a>
### #&#8288;320 [supercoder](https://github.com/transformeroptimus/supercoder) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (21) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Jul 2026</sub>

**Local desktop coding agent in Rust and Tauri with optional graph-based code search.**

SuperCoder is a Tauri 2 and React desktop app over a pure-Rust agent crate, offering Ask, Plan and Coding modes, subagents, skills, tool approval, checkpoints with rewind, and diff review. It talks directly to OpenAI chat-completions and Anthropic Messages APIs using your own key. An optional Go Context Engine indexes a repo with tree-sitter into Qdrant, FalkorDB and BM25 for codebase search.

- **+** Requests go straight from your machine to the provider you configure, with no vendor backend
- **+** Works with just an LLM key; the Context Engine is optional
- **+** Native OpenAI and Anthropic API support without a translation proxy
- **+** Agent core is a separate Rust crate, with the desktop app as a thin adapter
- **−** No prebuilt binaries yet; must build from source with Rust, Tauri prerequisites and Node 20+
- **−** Context Engine needs Docker Compose plus Qdrant, FalkorDB and a server-side embedding key
- **−** Only two provider API formats supported; broader support is on the roadmap
- **−** Original 2024 v1 pipeline is frozen and unmaintained

<sub>no GPU · Needs Rust, Tauri 2 prerequisites, Node.js 20+, Docker Compose (optional, Context Engine), Qdrant (optional), FalkorDB (optional), OpenAI API key for embeddings (optional) · Models: OpenAI chat-completions API, Anthropic Messages API · [Repo](https://github.com/transformeroptimus/supercoder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supercoder/)</sub>

<a name="browser-agent"></a>
### #&#8288;321 [browser-agent](https://github.com/magnitudedev/browser-agent) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: popular (60) · Freshness: slowing (40) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Feb 2026</sub>

**Vision-based browser agent and test runner driven by natural language.**

Magnitude is a TypeScript framework that controls a browser through a visually grounded LLM, which returns pixel coordinates for mouse and keyboard actions instead of relying on DOM element labels. It exposes act and extract calls, with extraction validated against zod schemas, and ships a test runner with visual assertions for web apps. The README reports 94% on WebVoyager.

- **+** Vision-first: model outputs pixel coordinates, so it does not depend on DOM structure
- **+** Mixes high-level tasks and low-level actions in one act() API
- **+** Structured extraction validated against zod schemas
- **+** Includes a test runner with visual assertions and CI docs
- **−** Needs a large visually grounded model; Claude Sonnet 4 recommended, Qwen-2.5VL 72B supported
- **−** Deterministic runs via native caching are marked in progress
- **−** No Docker or compose setup provided
- **−** Desktop and VM control is described as future work, not available

<sub>Needs Node.js, Visually grounded LLM (Claude Sonnet 4 or Qwen-2.5VL 72B) · Models: Claude Sonnet 4, Qwen-2.5VL 72B · [Repo](https://github.com/magnitudedev/browser-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browser-agent/)</sub>

<a name="amazon-q-developer-cli"></a>
### #&#8288;322 [amazon-q-developer-cli](https://github.com/aws/amazon-q-developer-cli) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: known (42) · Freshness: recent (52) · Maintenance: weak (8) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Apr 2026</sub>

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

<a name="copilot-vim"></a>
### #&#8288;323 [copilot.vim](https://github.com/github/copilot.vim) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: widely used (81) · Freshness: quiet (16) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Jan 2026</sub>

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

<a name="mle-agent"></a>
### #&#8288;324 [mle-agent](https://github.com/mlsysops/mle-agent) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (35) · Freshness: recent (58) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Jul 2026</sub>

**CLI agent that builds ML baselines and runs Kaggle tasks.**

MLE-Agent is a Python CLI that acts as a pairing agent for ML engineers. It plans an ML task from vague requirements, writes and runs code locally, debugs errors, and can search Arxiv and Papers with Code. It also has an auto mode for Kaggle competitions, an interactive chat, and a weekly report generator from GitHub or a local git repo.

- **+** Auto Kaggle mode runs data prep to submission without human input
- **+** Searches Arxiv and Papers with Code to inform solutions
- **+** Installs from PyPI with pip or uv; MIT license
- **+** Report command works from GitHub or a local git repo
- **−** Last tagged release is 2024-10-12; README milestones stop at 0.4.2
- **−** Many roadmap integrations (Hugging Face, MLflow, Wandb, S3) are unchecked
- **−** README names few models: Ollama Llama3, OpenAI, Claude 3.5 Sonnet, Mistral

<sub>Needs Python, LLM provider or Ollama, Kaggle account (for Kaggle mode) · Models: OpenAI, Anthropic Claude, Ollama, Mistral · port 3000 · [Repo](https://github.com/mlsysops/mle-agent) · [📖 Docs ↗](https://mle-agent-site.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mle-agent/)</sub>

<a name="codemachine-cli"></a>
### #&#8288;325 [codemachine-cli](https://github.com/moazbuilds/codemachine-cli) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: known (48) · Freshness: slowing (43) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Feb 2026</sub>

**CLI that chains AI coding agents into repeatable, multi-step workflows.**

CodeMachine is a TypeScript CLI, installed with npm, that runs AI coding CLIs such as Claude Code, Codex and Cursor through workflows you define once and rerun. It spawns each engine in its headless mode, passes context between steps, and can run several agents in parallel or over long periods. A default "Ali Workflow Builder" workflow helps you create your first workflow interactively.

- **+** Drives existing coding CLIs (Claude Code, Codex, Cursor) instead of replacing them
- **+** Supports multi-agent and parallel execution within one workflow
- **+** Workflows can run for hours or days with persistence handled by the tool
- **+** Covers interactive through fully autonomous orchestration patterns
- **−** Needs a separate coding agent CLI installed; it does not supply models itself
- **−** Depends on each engine's headless mode, so behavior follows those tools
- **−** README gives no system requirements, config format or workflow file examples

<sub>Compose · Needs Node.js/npm, AI coding CLI (Claude Code, Codex, Cursor) · Models: Claude Code, Codex, Cursor · [Repo](https://github.com/moazbuilds/codemachine-cli) · [▶️ Demo ↗](https://www.youtube.com/watch?v=G7OTG9iSvYw) · [📖 Docs ↗](https://docs.codemachine.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codemachine-cli/)</sub>

<a name="inferoa"></a>
### #&#8288;326 [inferoa](https://github.com/agentic-in/inferoa) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (7) · Freshness: active (82) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 570 · Apache-2.0 · Jun 2026</sub>

**Terminal coding agent with a durable /loop mode and prefix-cache-aware context.**

Inferoa is a TypeScript terminal (TUI) agent harness installed from npm. Its /loop command carries an objective across tasks, verification and recovery until the work is proven, while /plan and /tokenmaxxing expose plans and token and cache pressure. It builds on vLLM, vLLM Semantic Router, CodeGraph and RTK for serving, model routing and context reduction.

- **+** /loop keeps objective, attempts, verification evidence and decisions across loop tasks
- **+** Prompt epochs and deterministic tool schemas aim to preserve reusable prefix cache
- **+** Routes models by cost, privacy and capability via vLLM Semantic Router
- **+** npm install with interactive setup for endpoint, model and vault-backed API key
- **−** README installs the @dev tag, which tracks main rather than a stable release
- **−** No benchmarks or measured token or cache savings in the README
- **−** Routing and self-hosted serving depend on separately run vLLM components
- **−** Terminal-only interface; no web UI or editor integration described

<sub>GPU optional · Needs Node.js/npm, vLLM (optional), vLLM Semantic Router (optional), vLLM Omni (optional), CodeGraph, RTK · Models: Configurable model endpoints via inferoa setup, Self-hosted vLLM, Multimodal via vLLM Omni · [Repo](https://github.com/agentic-in/inferoa) · [📖 Docs ↗](https://inferoa.agentic-in.ai/docs/intro) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/inferoa/)</sub>

<a name="aiac"></a>
### #&#8288;327 [aiac](https://github.com/gofireflyio/aiac) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: popular (57) · Freshness: slowing (30) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Mar 2026</sub>

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

<a name="ai-shell"></a>
### #&#8288;328 [ai-shell](https://github.com/builderio/ai-shell) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: popular (67) · Freshness: quiet (15) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Jan 2026</sub>

**CLI that turns natural-language prompts into shell commands via OpenAI.**

AI Shell is an npm-installed CLI (`ai <prompt>`) that sends a plain-language request to OpenAI and returns a suggested shell command with an explanation. You can run it, revise it with another prompt, or cancel. It also has a chat mode, a silent flag to skip explanations, a configurable API endpoint, and 14 interface languages.

- **+** Run, revise or cancel step before any generated command executes
- **+** OPENAI_API_ENDPOINT setting allows proxies or compatible endpoints
- **+** Interactive `ai config` UI and 14 interface languages
- **+** One global npm install; Node.js v14 minimum
- **−** Requires an OpenAI API key with billing; no local model support documented
- **−** Prompts go to a remote API, so it does not work offline
- **−** No tagged releases; last commit 2026-01-05
- **−** Generated commands can be wrong; the confirmation step is the only safeguard

<sub>no GPU · Needs OpenAI API key, Node.js >= 14 · Models: OpenAI (default gpt-4o-mini) · [Repo](https://github.com/builderio/ai-shell) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-shell/)</sub>

<a name="async"></a>
### #&#8288;329 [async](https://github.com/x-man-git/async) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (5) · Freshness: recent (73) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 476 · Apache-2.0 · May 2026</sub>

**Electron desktop IDE with a built-in agent loop, Git and terminal.**

Async IDE is an Electron + React + Monaco desktop app, not a VS Code fork, where an agent runs multi-round tool calls (Read, Write, Edit, Grep, shell) with approval gates. It has Agent, Plan, Ask and Debug modes, a multi-agent Team mode, MCP support, and Telegram, Slack, Discord and Feishu bot bridges. Models are BYOK: Anthropic, OpenAI, Gemini or any OpenAI-compatible endpoint. Threads and settings are stored locally as JSON.

- **+** Supports Anthropic, OpenAI, Gemini and OpenAI-compatible endpoints such as Ollama and vLLM
- **+** Team mode with lead, specialist and reviewer agents, plus Plan mode review before execution
- **+** Bot bridges for Telegram, Slack, Discord and Feishu reuse the desktop agent runtime
- **+** Threads, settings and plans stored locally as JSON and Markdown
- **−** No prebuilt installers mentioned; run from source with npm install and npm run desktop
- **−** No VS Code extension ecosystem, since it is not a VS Code fork
- **−** LSP integration is documented only for TypeScript Language Server
- **−** API keys are kept in plain settings.json on disk

<sub>no GPU · Needs Node.js >= 18, npm >= 9, Git (recommended) · Models: Anthropic, OpenAI, Gemini, OpenAI-compatible endpoints (Ollama, vLLM) · [Repo](https://github.com/x-man-git/async) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/async/)</sub>

<a name="coffee"></a>
### #&#8288;330 [coffee](https://github.com/coframe/coffee) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: known (34) · Freshness: slowing (44) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Mar 2026</sub>

**Watches React files and generates or edits components from inline prompts.**

Coffee runs next to your React project and watches js/jsx/ts/tsx files for a `<Coffee>` component or a `coffee` prop. When it finds one, it sends the parent code, existing child code and your prompt to the OpenAI chat completions API and writes the generated component to disk. A `pour="Name.tsx"` prop replaces the placeholder with an import of the generated file.

- **+** Same prompt-in-JSX workflow for creating new components and editing existing ones
- **+** Editor-agnostic: watches files on save, so it works with any IDE
- **+** Agent code runs inside a Docker container, isolated from the host
- **+** `pour` prop turns a generated component into a normal imported file
- **−** Only React is supported; Vue and Svelte are unchecked TODO items
- **−** Requires an OpenAI API key; no other model providers are listed
- **−** Custom prompts, custom agents and prettier formatting are still TODO
- **−** README calls generation slow; no release published, last commit March 2026

<sub>no GPU · Needs Docker, OpenAI API key · Models: OpenAI chat completions · [Repo](https://github.com/coframe/coffee) · [🌐 Site ↗](https://coframe.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coffee/)</sub>

<a name="chatgpt-nvim"></a>
### #&#8288;331 [chatgpt.nvim](https://github.com/jackmort/chatgpt.nvim) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: popular (58) · Freshness: quiet (12) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Jan 2026</sub>

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

<a name="lemonai"></a>
### #&#8288;332 [lemonai](https://github.com/hexdocom/lemonai) <sub>score [20](../README.md#-how-we-rank "Score 20/100. Adoption: known (35) · Freshness: slowing (31) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · custom license · Feb 2026</sub>

**General-purpose local AI agent with a Docker sandbox and HTML editor.**

Lemon AI is a Manus-style general agent that plans tasks, browses the web, writes and runs code, and produces research reports or data analysis. Code runs inside a Docker-based VM sandbox. It can use local models through Ollama or vLLM, or cloud APIs such as Claude, GPT, Gemini and Grok. A built-in editor lets you click an element in a generated HTML page and have the agent change it.

- **+** Code execution runs in a Docker sandbox, separate from host files
- **+** Works with local models via Ollama or vLLM, or with cloud APIs
- **+** Click-to-edit HTML editor refines generated pages without full regeneration
- **+** Setup is a single docker run command; README recommends 4GB RAM
- **−** Custom license: Apache 2.0 plus extra restrictions; commercial use needs a separate license
- **−** Requires the host Docker socket mounted into the container
- **−** The 10x cheaper cost claim has no benchmark or method in the README
- **−** README links point to inconsistent repo names and doc sites

<sub>RAM ≥ 4 GB · GPU optional · Docker + Compose · Needs Docker, Ollama or vLLM (for local models) · Models: Ollama, vLLM, DeepSeek, Kimi, Qwen · port 5005 · [Repo](https://github.com/hexdocom/lemonai) · [📖 Docs ↗](https://lemon-11.gitbook.io/lemonai) · [🌐 Site ↗](https://lemonai.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lemonai/)</sub>

<a name="sleepless-agent"></a>
### #&#8288;333 [sleepless-agent](https://github.com/context-machine-lab/sleepless-agent) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: niche (14) · Freshness: slowing (43) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 842 · MIT · Mar 2026</sub>

**Daemon that runs queued tasks through Claude Code overnight, via Slack or CLI.**

Sleepless Agent is a Python daemon that wraps the Claude Code CLI through its Python Agent SDK and works through a SQLite-backed task queue. Tasks arrive from Slack slash commands or the `sle` CLI and run in isolated workspaces, and serious tasks get a feature branch and a pull request. It tracks Claude Code plan usage against day and night thresholds and can auto-generate tasks when idle.

- **+** Each task runs in its own workspace directory, so tasks can run in parallel
- **+** Creates feature branches and opens PRs for serious tasks via git and gh
- **+** Usage-aware scheduling with day (95%) and night (96%) thresholds
- **+** Slack is optional; the sle CLI covers every command
- **−** Requires a Claude Code CLI login; no other model providers mentioned
- **−** Only one release (0.1.0, Oct 2025); roadmap items still unchecked
- **−** No Docker or compose files; service install is via systemd or launchd make targets
- **−** Must edit config.yaml (e.g. git.remote_repo_url) before first run

<sub>no GPU · Needs Python 3.11+, Claude Code CLI (Node.js), Git, gh CLI (optional), Slack app with Socket Mode (optional), SQLite · Models: Claude (via Claude Code CLI) · [Repo](https://github.com/context-machine-lab/sleepless-agent) · [📖 Docs ↗](https://context-machine-lab.github.io/sleepless-agent/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sleepless-agent/)</sub>

<a name="10x"></a>
### #&#8288;334 [10x](https://github.com/ntegrals/10x) <sub>score [14](../README.md#-how-we-rank "Score 14/100. Adoption: known (31) · Freshness: quiet (15) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Jan 2026</sub>

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

<a name="typedai"></a>
### #&#8288;335 [typedai](https://github.com/trafficguard/typedai) <sub>score [13](../README.md#-how-we-rank "Score 13/100. Adoption: niche (27) · Freshness: quiet (7) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Dec 2025</sub>

**TypeScript platform for autonomous agents, code editing and PR review.**

TypedAI is a TypeScript platform for running LLM agents, workflows and chatbots, with a CLI (`ai`, `aid`) and a web UI. It bundles an autonomous agent, a code-editing agent with compile/lint/test loops, a GitLab merge request reviewer, a Slack chatbot and a chat interface. Function-calling schemas are generated from decorated class methods instead of zod or JSON definitions.

- **+** Code agent auto-detects compile, test and lint, then loops to fix failures
- **+** Function schemas generated from @func decorators on typed class methods
- **+** Supports many providers: OpenAI, Anthropic, Gemini, Groq, DeepSeek, Ollama, OpenRouter and more
- **+** OpenTelemetry tracing and configurable human-in-the-loop for budget and questions
- **−** Multi-user SSO relies on Google Cloud IAP; Terraform and other auth options are still planned
- **−** Code review agent is documented only for GitLab merge requests
- **−** Last release is 2025-06-09, well behind recent commits
- **−** Scale-to-zero deployment targets Firestore and Cloud Run, tying hosted setups to Google Cloud

<sub>no GPU · Docker + Compose · Needs LLM provider API keys, Firestore (cloud deployment), Google Cloud IAP (multi-user SSO) · Models: OpenAI, Anthropic, Vertex, Gemini, Groq · [Repo](https://github.com/trafficguard/typedai) · [📖 Docs ↗](https://typedai.dev/setup/) · [🌐 Site ↗](https://typedai.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typedai/)</sub>

<a name="hephaestus"></a>
### #&#8288;336 [hephaestus](https://github.com/ido-levi/hephaestus) <sub>score [11](../README.md#-how-we-rank "Score 11/100. Adoption: niche (27) · Freshness: quiet (1) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · custom license · Nov 2025</sub>

**Multi-agent orchestrator where agents spawn tasks across phases on a Kanban board.**

Hephaestus runs CLI coding agents (Claude Code, OpenCode, Droid, Codex) in isolated tmux sessions. You define phase types such as analysis, implementation and validation, and agents create new tickets in any phase as they discover work. A Guardian process monitors agents against phase instructions, and a web UI shows the Kanban board and dependency graph. Hephaestus Dev adds five preset software-development workflows. Status is alpha.

- **+** Agents create tasks in any phase, so workflows branch without predefined instructions
- **+** Isolated tmux sessions per agent, coordinated by Kanban tickets with blocking dependencies
- **+** Works with Claude Code, OpenCode, Droid or Codex as the agent CLI
- **+** Ships five preset dev workflows: PRD-to-software, bug fix, repo indexing, features, docs
- **−** Alpha status and no tagged release
- **−** AGPL-3.0 per the README, which restricts closed-source network use
- **−** Heavy setup: tmux, Docker for Qdrant, Node.js, git repo and several API keys
- **−** Setup validation script is macOS only

<sub>no GPU · Docker + Compose · Needs tmux, Git, Docker, Qdrant, Node.js, npm, Claude Code, OpenCode, Droid or Codex CLI · Models: OpenAI, Anthropic, OpenRouter, Azure OpenAI, Google AI Studio · [Repo](https://github.com/ido-levi/hephaestus) · [📖 Docs ↗](https://ido-levi.github.io/Hephaestus/docs/getting-started/quick-start) · [🌐 Site ↗](https://ido-levi.github.io/Hephaestus/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hephaestus/)</sub>

<a name="gptstudio"></a>
### #&#8288;337 [gptstudio](https://github.com/michelnivard/gptstudio) <sub>score [9](../README.md#-how-we-rank "Score 9/100. Adoption: niche (20) · Freshness: quiet (10) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 988 · custom license · Jan 2026</sub>

**RStudio addins and Shiny chat app for using LLMs inside R projects.**

gptstudio is an R package that adds LLM chat and text-editing addins to RStudio. Selected text or code, or a prompt typed into its built-in Shiny apps, is sent to a configured provider such as OpenAI, Anthropic, Google AI Studio, Azure OpenAI, Cohere, Perplexity, HuggingFace or a local Ollama server. Install from CRAN or GitHub and set an API key in .Renviron.

- **+** Supports seven hosted providers plus local models through Ollama
- **+** Installs from CRAN with install.packages, or from GitHub with pak
- **+** Shares only highlighted text or prompts unless other features are enabled
- **+** Per-provider setup articles on the project documentation site
- **−** Lifecycle badge marks it experimental
- **−** Last release 2024-05-21; model lists in the README are dated
- **−** Tied to RStudio and R; no other editor is mentioned
- **−** Default OpenAI setup needs an API key and paid account

<sub>no GPU · Needs R, RStudio, API key for chosen provider, Ollama (optional, for local models) · Models: OpenAI, Anthropic, HuggingFace, Ollama, Perplexity · [Repo](https://github.com/michelnivard/gptstudio) · [📖 Docs ↗](https://michelnivard.github.io/gptstudio/articles/openai.html) · [🌐 Site ↗](https://michelnivard.github.io/gptstudio/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gptstudio/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
