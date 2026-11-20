# 🧩 Agent and MCP starters reviews · Best of Vibe Coding

Agent backends and UIs to fork (LangGraph, ADK, OpenAI Agents SDK, Cloudflare Agents) and templates for MCP servers and chat-host apps. Back to the [leaderboard](../README.md#-agent-and-mcp-starters).

<sub>🌐 Also on the web: [Agent and MCP starters on archestack.com](https://archestack.com/best-of-vibe-coding/agents/), each project on its own page.</sub>

<a name="deepseek-harness"></a>
### 🥇 [deepseek-harness](https://github.com/deepseek-ai/deepseek-harness) <sub>score [98](../README.md#-how-we-rank "Score 98/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 284k · MIT · Nov 2026</sub>

**Plugin-based agent harness from DeepSeek with a local Web UI.**

DeepSeek Harness (`dsh`) is a TypeScript agent harness built on the Cordis plugin framework, where every component is a plugin. It runs via `npx @deepseek-ai/dsh web` or from a source checkout with pnpm, and serves a Web UI at 127.0.0.1:3080 by default. It is a developer preview, and the README warns of compatibility-breaking changes.

- **+** Starts with one npx command; no Docker or database mentioned
- **+** Everything-is-a-plugin design on Cordis, with a dsh-plugin topic for discovery
- **+** MIT license, documentation site and third-party license notices
- **+** Web UI binds to 127.0.0.1 by default; --no-open skips the browser
- **−** Developer preview; README warns of compatibility-breaking changes
- **−** No tagged release published
- **−** Safety notice must be read before running; its contents are not in the README

<sub>TypeScript · Needs Node.js, pnpm (source build) · [Repo](https://github.com/deepseek-ai/deepseek-harness) · [📖 Docs ↗](https://deepseek-harness.github.io/deepseek-harness/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepseek-harness/)</sub>

<a name="composio"></a>
### 🥈 [composio](https://github.com/composiohq/composio) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

**TypeScript and Python SDKs that give agents authenticated tools across 1000+ apps.**

Composio is an SDK monorepo (TypeScript, Python, and a CLI) that creates per-user sessions exposing pre-authenticated toolkits to an agent. Sessions default to meta tools that discover, authenticate and execute app tools at runtime, and can also be served through a hosted MCP endpoint. Provider adapters convert the tools to the formats of OpenAI, Anthropic, LangChain, Vercel AI SDK, Google ADK, CrewAI and others.

- **+** Adapters for about 16 frameworks, including OpenAI Agents, Claude Agent SDK, LangChain and Mastra
- **+** Per-user sessions handle authentication, so the agent does not manage OAuth flows
- **+** Meta tools load tools at runtime instead of putting hundreds of definitions in context
- **+** Each session can also be exposed as a hosted MCP URL for Claude, Cursor or other clients
- **−** Requires a COMPOSIO_API_KEY from the hosted dashboard; the README documents no self-hosted option
- **−** The SDK is open source, but toolkits and auth run through Composio's service
- **−** Provider coverage is uneven: Vercel and Mastra are TypeScript only, CrewAI and AutoGen Python only
- **−** Pi provider is experimental and ships from a separate package

<sub>TypeScript, OpenAI, Anthropic, Google GenAI, LangChain · Needs Composio API key (hosted service), Node 22+ for TypeScript SDK, Python 3.10+ for Python SDK · [Repo](https://github.com/composiohq/composio) · [📖 Docs ↗](https://docs.composio.dev) · [🌐 Site ↗](https://composio.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/composio/)</sub>

<a name="conductor-oss-conductor"></a>
### 🥉 [conductor](https://github.com/conductor-oss/conductor) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Nov 2026</sub>

**Durable workflow engine that orchestrates microservices and LLM agents from JSON.**

Conductor is a Java workflow orchestration server, originally from Netflix, that persists every task and runs versioned JSON workflow graphs. Workers in Java, Python, Go, JavaScript, C#, Ruby or Rust poll for tasks, while built-in tasks cover LLM chat, MCP tool discovery and calls, human approval, loops, forks and sub-workflows. It runs on Redis, Postgres or MySQL, with Elasticsearch or OpenSearch for indexing.

- **+** Every step is persisted, with retry, restart, rerun, pause and terminate controls on executions
- **+** Workflows are versioned JSON; running executions stay pinned to the version they started on
- **+** Native LLM_CHAT_COMPLETE, LIST_MCP_TOOLS and CALL_MCP_TOOL tasks for agent loops
- **+** Multiple persistence backends (Redis, Postgres, MySQL) and polyglot worker SDKs
- **−** Requires Java 25+ and a separate index store such as Elasticsearch or OpenSearch
- **−** Orchestration is declarative JSON, not code, which suits some teams less than code-first engines
- **−** Ruby and Rust SDKs are marked incubating
- **−** Not a ready-made agent app; you build agents by composing workflow tasks

<sub>Java, OpenAI (via llmProvider) · Needs Java 25+, Node.js 16+ (CLI), Redis, Postgres or MySQL, Elasticsearch or OpenSearch · Docker · [Repo](https://github.com/conductor-oss/conductor) · [📖 Docs ↗](https://docs.conductor-oss.org) · [🌐 Site ↗](https://conductor-oss.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/conductor-oss-conductor/)</sub>

<a name="mcp-use"></a>
### #&#8288;4 [mcp-use](https://github.com/mcp-use/mcp-use) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**TypeScript framework for building MCP servers with React Views and an Inspector.**

mcp-use is a TypeScript framework for writing MCP servers with Zod-typed tools and React Views bound to those tools, so they render as interactive apps in ChatGPT and Claude. It ships a browser Inspector at /mcp/inspector, a headless CLI client with View screenshots, and tunneling for testing against hosted clients. It builds on the official TypeScript SDK v2 and deploys to Manufact or self-hosted.

- **+** Zod schemas flow from tool input and output into React View props
- **+** Built-in Inspector, tunnel (mcp-use dev --tunnel) and View screenshot CLI
- **+** Scaffold via npx create-mcp-use-app gives a running server and Inspector
- **+** MIT licensed; separate client, agent and Python packages exist
- **−** Benchmark comparisons in the README are published by the project itself
- **−** Managed deploy, observability and evals tie into the commercial Manufact platform
- **−** v2 is a breaking change; v1 projects need migration
- **−** Server framework is TypeScript; Python support is a separate package

<sub>TypeScript · Needs Node.js, npm, zod, React · safety checks passed 14 of 18 · [Repo](https://github.com/mcp-use/mcp-use) · [▶️ Demo ↗](https://inspector.mcp-use.com/inspector) · [📖 Docs ↗](https://docs.mcp-use.com/v2/typescript/getting-started/welcome) · [🌐 Site ↗](https://mcp-use.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-use/)</sub>

<a name="a2ui"></a>
### #&#8288;5 [a2ui](https://github.com/a2ui-project/a2ui) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Nov 2026</sub>

**Protocol and renderers for agents to stream native UI instead of text.**

A2UI is a generative UI framework where agents emit UI as schema-validated data rather than code. It ships a streaming transport protocol, agent SDKs for Python, TypeScript and Dart, and native renderers for React, Angular, Lit, Flutter and SwiftUI. The host app controls which components the agent may use through a widget catalog.

- **+** UI is validated data against a schema, with no executable code from the agent
- **+** Renderers for React, Angular, Lit, Flutter and SwiftUI from one protocol
- **+** Agent SDKs in Python, TypeScript and Dart, with A2A and ADK connectors
- **+** Browser Composer and Theater let you try it without installing
- **−** Library and protocol only; no runnable full app without the quickstart
- **−** Protocol v1.1, sandboxed logic and templates are still roadmap items
- **−** Jetpack Compose is cited as a target but is not in the package list

<sub>TypeScript, LLM-agnostic (model-independent inference formats) · [Repo](https://github.com/a2ui-project/a2ui) · [▶️ Demo ↗](https://a2ui-project.github.io/composer/) · [📖 Docs ↗](https://a2ui.org/quickstart/) · [🌐 Site ↗](https://a2ui.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/a2ui/)</sub>

<a name="agent-autoloop"></a>
### #&#8288;6 [agent-autoloop](https://github.com/kkkkhazix/agent-autoloop) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Nov 2026</sub>

**Background scheduler that runs CLI agents on events and asks you only when unsure.**

Agent Autoloop is a zero-runtime-dependency Node hub that dispatches events (cron, GitHub/GitLab webhooks, HTTP) to command-line agents such as Claude Code, Codex, ACP agents or any command, per rules in rules.json. When an agent needs a decision, the process exits and a card goes to Feishu, DingTalk, WeCom, Slack, Discord or desktop notification. After you answer, the original session resumes. Ships recipes for daily briefs, issue handling, alert triage and a PR delivery pipeline.

- **+** Waiting for approval uses no agent process and no tokens; the session resumes after you answer
- **+** Any CLI agent that takes a prompt and prints a reply connects with one config line
- **+** Append-only event log; the `why` command explains any run; crash and simulation tests included
- **+** Event text is passed as data files, not prompts; events cannot set cwd, agent or access
- **−** No web UI; status and answers go through CLI commands and chat cards
- **−** README is Chinese first; English version is in a separate file
- **−** Webhook channels and several agent commands only tested against mock servers or docs, not live services
- **−** Text-channel approvals need hub.publicUrl set to an address your phone can reach

<sub>TypeScript, Claude Code, Codex, ACP agents (Gemini CLI, OpenCode), DeepSeek Harness · Needs Node 24+, Git, A logged-in CLI agent (Claude Code, Codex, etc.), curl (macOS/Linux install) · [Repo](https://github.com/kkkkhazix/agent-autoloop) · [📖 Docs ↗](https://github.com/KKKKhazix/agent-autoloop/blob/main/skills/agent-autoloop/SKILL.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-autoloop/)</sub>

<a name="mirage"></a>
### #&#8288;7 [mirage](https://github.com/strukto-ai/mirage) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Nov 2026</sub>

**Virtual shell that mounts S3, Slack and Gmail as one filesystem for agents.**

Mirage gives AI agents a single Unix-style shell over mounted services such as S3, Google Drive, Slack, Gmail and Redis. Commands like grep, ls and jq work across mounts, and each command is routed to an in-process, sandboxed (E2B) or remote runtime. Per-agent profiles allow, ask, deny or hide commands and paths, and a policy script can block actions before they run. Python and TypeScript SDKs exist.

- **+** One filesystem and shell across S3, Drive, Slack, Gmail and Redis, so pipes work across services
- **+** Profiles can hide paths entirely, so they are absent from the agent's view
- **+** Workspace uses about 100 KB and each session about 10 KB, per the README
- **+** Routes commands between in-process and sandbox runtimes such as Monty and E2B
- **−** Marked preview status, so APIs may change
- **−** Each mount needs its own credentials and config in code
- **−** Libraries like numpy need an external sandbox such as E2B
- **−** Virtual CLIs listed are only git, slack and ntn

<sub>TypeScript · Needs E2B (optional sandbox runtime), Credentials for mounted services (S3, Slack, Gmail) · Docker · env example file · [Repo](https://github.com/strukto-ai/mirage) · [📖 Docs ↗](https://docs.mirage.strukto.ai) · [🌐 Site ↗](https://www.strukto.ai/mirage) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mirage/)</sub>

<a name="computer"></a>
### #&#8288;8 [computer](https://github.com/cloudflare/computer) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.9k · MIT · Nov 2026</sub>

**Durable Object SQLite filesystem with container, shell and JS execution backends.**

A TypeScript library that keeps a virtual filesystem in a Cloudflare Durable Object, with SQLite as the authoritative state. Code runs against it through `workspace.runtime.exec`, which selects a backend: a FUSE-mounted Linux container (`computerd`), a just-bash shell in a Dynamic Worker, or an ECMAScript module in a Dynamic Worker. The repo includes examples for agents, MCP, and Cloudflare Artifacts.

- **+** One `runtime.exec` entry point across container, isolate shell and codemode backends
- **+** Isolate backends read the Workspace over Workers RPC, with no second store or sync
- **+** Many runnable examples: MCP, pi, TanStack AI, Think agents, egress policies
- **+** Filesystem usable on its own, with no execution backend configured
- **−** Container backend and `computerd` are experimental and not for production
- **−** Tied to Cloudflare Workers, Durable Objects and Dynamic Workers
- **−** Design spec in `docs/` is forward-looking, not a description of current code
- **−** Unsolicited pull requests are not accepted

<sub>TypeScript · Needs Cloudflare Workers, Durable Objects, Dynamic Workers, Cloudflare Containers · [Repo](https://github.com/cloudflare/computer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/computer/)</sub>

<a name="agentteams"></a>
### #&#8288;9 [agentteams](https://github.com/agentscope-ai/agentteams) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · Apache-2.0 · Nov 2026</sub>

**Coordinates a Manager agent and Worker agents in Matrix rooms.**

AgentTeams runs a Manager agent and multiple Worker agents (OpenClaw, QwenPaw, Hermes, experimental DeepSeek Harness), each in its own container, inside Matrix rooms where humans can watch and intervene. It bundles a Higress AI gateway that holds real credentials, a Tuwunel Matrix server with Element Web, and MinIO shared storage. It installs locally via script or on Kubernetes via Helm.

- **+** Workers hold only gateway tokens; real API keys and GitHub PATs stay in Higress
- **+** Mixes several agent runtimes in one Matrix room with human intervention
- **+** One-command local installer plus a Helm chart for Kubernetes 1.24+
- **+** Built-in Matrix server and Element Web, so no Slack or DingTalk bot setup
- **−** Runs a full stack: gateway, Matrix server, MinIO, controller, Manager and Worker containers
- **−** Default install pipes a remote shell script to bash
- **−** Helm images default to a China-region registry
- **−** Manager supports only OpenClaw or QwenPaw; DeepSeek Harness Worker is experimental

<sub>Go, OpenAI-compatible APIs, Qwen · Needs Docker, OrbStack or Podman, Higress AI gateway, Tuwunel (Matrix), Element Web, MinIO, Kubernetes 1.24+ and Helm 3.7+ (cluster install) · [Repo](https://github.com/agentscope-ai/agentteams) · [📖 Docs ↗](https://github.com/agentscope-ai/AgentTeams/blob/main/docs/quickstart.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentteams/)</sub>

<a name="soduwork"></a>
### #&#8288;10 [soduwork](https://github.com/mdiri-ai/soduwork) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Nov 2026</sub>

**Team workspace that routes requests to agent harnesses with AI review.**

SoduWork is a Hub, admin console and desktop client that dispatches requests to agent harnesses such as Pi, OpenCode, Qwen Code, Kimi Code and Codex. Each request carries acceptance criteria, a separate AI review checks them, and a person signs off. Working methods can be saved as versioned, reviewable plugins shared across a team. The README describes it as a public beta.

- **+** Mixes harnesses and models per step, with a different model reviewing the work
- **+** Plugins are versioned, reviewed before sharing, and can be granted or revoked
- **+** Roles, usage and cost tracking, and an audit log are built in
- **+** Docker deploy script starts Hub, admin console and PostgreSQL on one server
- **−** Public beta; README advises evaluating before production use
- **−** Running from source needs Python 3.12+, Node.js 22.19+ and Git
- **−** Hub usage accounting and update polling cannot be disabled
- **−** Runners are not a general sandbox; isolation depends on harness and environment

<sub>JavaScript, OpenAI-compatible chat models, DeepSeek, Codex (own OpenAI account), self-hosted models · Needs Python 3.12+, Node.js 22.19+, Git, PostgreSQL (Docker deploy) · [Repo](https://github.com/mdiri-ai/soduwork) · [▶️ Demo ↗](https://soduwork.ai) · [📖 Docs ↗](https://dev.soduwork.ai) · [🌐 Site ↗](https://soduwork.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/soduwork/)</sub>

<a name="epicenter"></a>
### #&#8288;11 [epicenter](https://github.com/epicenterhq/epicenter) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (68) · Freshness: active (88) · Maintenance: healthy (87) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · custom license · Nov 2026</sub>

**Personal data runtime that serves Markdown-backed app actions to CLI and MCP.**

Epicenter keeps one person's app data as Markdown files in a private Git repository (the "home") on a computer you control. `epicenter serve` imports the home's `epicenter.ts` and exposes every app's actions to the `epicenter` command and to MCP clients. The repo ships no apps besides Whispering, a separate speech-to-text app, so you write the first app yourself.

- **+** Records are plain Markdown in Git, readable and versioned without the tool
- **+** Same actions are exposed to the CLI and to MCP clients from one process
- **+** No sign-in or sync layer; devices reach the single copy over your private network
- **+** Runs on Bun and Git; no AI account required
- **−** Ships no apps; you author your own inside apps in TypeScript
- **−** `@epicenter/app` is a developer preview and not yet on npm
- **−** Routines and browser pages for apps are not built yet
- **−** `serve` has no auth; access control depends on your tailnet or network

<sub>TypeScript · Needs Bun, Git, Rust (Whispering desktop build only) · [Repo](https://github.com/epicenterhq/epicenter) · [🌐 Site ↗](https://epicenter.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/epicenter/)</sub>

<a name="docker-agent"></a>
### #&#8288;12 [docker-agent](https://github.com/docker/docker-agent) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · Apache-2.0 · Nov 2026</sub>

**Docker CLI plugin that runs multi-agent teams defined in YAML.**

docker-agent is a Go CLI plugin (`docker agent run agent.yaml`) that runs agents declared in YAML: model, instructions, and toolsets, including any MCP server. Agents can delegate to other agents, and configs can be pushed to and pulled from OCI registries. It supports OpenAI, Anthropic, Gemini, AWS Bedrock, Mistral, xAI and Docker Model Runner, plus built-in RAG with BM25, embeddings and reranking.

- **+** Agents, tools and models declared in versionable YAML, no code required
- **+** Works with local, remote or Docker-based MCP servers as toolsets
- **+** Agent configs can be shared through any OCI registry
- **+** Many providers supported, plus local models via Docker Model Runner
- **−** Collects anonymous usage telemetry; opt-out details are only in the docs
- **−** Needs a cloud provider API key or Docker Model Runner to do anything
- **−** Configuration is YAML-centric; custom logic needs MCP tools rather than code hooks

<sub>Go, OpenAI, Anthropic, Gemini, AWS Bedrock · Needs Docker CLI (plugin), LLM provider API key or Docker Model Runner, MCP servers (optional), OCI registry (optional) · Docker · [Repo](https://github.com/docker/docker-agent) · [📖 Docs ↗](https://docker.github.io/docker-agent/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/docker-agent/)</sub>

<a name="skybridge"></a>
### #&#8288;13 [skybridge](https://github.com/alpic-ai/skybridge) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

**React framework for building MCP Apps with interactive UI views.**

Skybridge is a TypeScript framework for building MCP servers that render interactive React views inside Claude, ChatGPT, VS Code and other UI-enabled MCP clients. It provides a dev server with a local emulator, hot module reload and a tunnel, plus React hooks and end-to-end type inference from tool definitions to views. A CLI, an agent skill and example apps are included.

- **+** Type inference from MCP tool definitions through to React views
- **+** Dev server with local emulator, hot module reload and tunnel to Claude and ChatGPT
- **+** Abstracts differences between MCP clients so one app targets several hosts
- **+** Many runnable examples with live demos, including six OAuth provider integrations
- **−** Tied to React and TypeScript; no other frontend stack is mentioned
- **−** Permanent tunnel, analytics and directory submission help are tied to the Alpic hosted service
- **−** Only useful with MCP clients that support UI views
- **−** No Docker image or compose file; self-hosting means a Node.js platform

<sub>TypeScript · Needs Node.js, npm · [Repo](https://github.com/alpic-ai/skybridge) · [▶️ Demo ↗](https://everything.skybridge.tech/try) · [📖 Docs ↗](https://docs.skybridge.tech) · [🌐 Site ↗](https://alpic.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skybridge/)</sub>

<a name="mercury-agent"></a>
### #&#8288;14 [mercury-agent](https://github.com/cosmicstack-labs/mercury-agent) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Nov 2026</sub>

**Personal agent daemon with permissioned tools, local memory and chat-app access.**

Mercury Agent is a TypeScript agent that runs as one background process on your machine and is reachable from a terminal UI, Telegram, Discord, Slack, Signal and a local web dashboard. It has about 50 built-in tools (files, shell, git, GitHub, fetch, scheduler), a per-folder permission and approval layer, and SQLite-based memory. It also includes a coding mode and persistent scheduled bots.

- **+** Permission layer: shell blocklist, per-folder scopes, approval prompts and SSRF-guarded fetches
- **+** One daemon shared by all channels, with crash recovery and a login service on each OS
- **+** Memory stays local in SQLite with FTS5; daily token budget enforced per turn
- **+** Many providers with automatic fallback, including Ollama and LM Studio for local models
- **−** No Docker or Compose setup; installs as a host binary or npm package
- **−** Community skills are not audited; the README tells users to review them first
- **−** Release binaries are unsigned; macOS builds need your own codesign and notarization
- **−** Built as a personal single-owner agent, not a multi-tenant backend to fork

<sub>TypeScript, DeepSeek, OpenAI, Anthropic, Grok · Needs Node.js 22+ (npm install only), signal-cli (Signal channel), LLM provider API key or local Ollama/LM Studio · env example file · [Repo](https://github.com/cosmicstack-labs/mercury-agent) · [📖 Docs ↗](https://mercuryagent.sh/docs) · [🌐 Site ↗](https://mercuryagent.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mercury-agent/)</sub>

<a name="agentconnect"></a>
### #&#8288;15 [agentconnect](https://github.com/agentconnect-md/agentconnect) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Nov 2026</sub>

**Platform for teams and multiple coding agents to work together in chat and Git tools.**

AgentConnect connects agent runtimes such as Claude Code, Codex, Grok Build, DeepSeek, Pi and other ACP-compatible agents to Slack, Teams, Google Chat, Lark, Discord, Telegram and WeChat, and to GitHub, GitLab, Gitea, Azure DevOps and Linear. Agents get roles, memory, skills and shared Knowledge, can call each other, and start work from messages, issues, pull requests, webhooks or schedules. The stack is a web console, control plane, relay and PostgreSQL, run with Docker Compose or a Helm chart.

- **+** Runs several agent runtimes side by side, including any ACP-compatible agent
- **+** Covers many chat platforms and Git hosts: Slack, Teams, Telegram, GitHub, GitLab, Gitea
- **+** Docker Compose quick start plus an official Helm chart on OCI
- **+** Per-agent runtime, model, workspace, tools and visibility permissions
- **−** Default Compose stack uses local no-auth mode, suitable only for evaluation
- **−** Real deployments need Logto auth and provider app setup on top of Compose
- **−** Routing Decisions depend on Jev, a separate TypeSafe product
- **−** Several moving parts: console, control plane, relay, daemons, PostgreSQL

<sub>TypeScript, Claude Code, Codex, Grok Build, DeepSeek · Needs PostgreSQL, Logto (browser authentication), Jev (agent routing and model selection) · Docker · env example file · [Repo](https://github.com/agentconnect-md/agentconnect) · [▶️ Demo ↗](https://app.agentconnect.md) · [📖 Docs ↗](https://www.agentconnect.md/docs) · [🌐 Site ↗](https://www.agentconnect.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentconnect/)</sub>

<a name="neuron-ai"></a>
### #&#8288;16 [neuron-ai](https://github.com/neuron-core/neuron-ai) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Nov 2026</sub>

**PHP framework for building LLM agents, RAG pipelines and workflows.**

Neuron is a Composer package that provides an Agent class with chat memory, tools, MCP connectors and structured output into PHP classes, plus a RAG class that takes a vector store and an embeddings provider. A separate Workflow component handles event-driven flows with human-in-the-loop. It supports 16 LLM providers, including Anthropic, OpenAI, Gemini, Ollama and AWS Bedrock.

- **+** Provider switch is a one-line change across Anthropic, OpenAI, Gemini, Ollama, Bedrock and others
- **+** Same Workflow component covers single agents and multi-agent flows with human approval
- **+** Ships agent skills and an MCP server so coding assistants can write Neuron code
- **+** Built-in MySQL toolkit runs SELECT queries in read-only transactions
- **−** PHP only, requires PHP 8.1 or newer
- **−** Read-only MySQL tool can still read anything the connection user can read
- **−** README spends more space on newsletter and ecosystem than on internals
- **−** RAG example depends on external services such as Pinecone and Voyage

<sub>PHP, Anthropic, OpenAI, Azure OpenAI, OpenAI-compatible APIs · Needs PHP ^8.1, Composer, LLM provider API key · Docker · env example file · [Repo](https://github.com/neuron-core/neuron-ai) · [📖 Docs ↗](https://docs.neuron-ai.dev/) · [🌐 Site ↗](https://neuron-ai.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neuron-ai/)</sub>

<a name="google-adk-recipes"></a>
### #&#8288;17 [adk-recipes](https://github.com/google/adk-recipes) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Nov 2026</sub>

**Runnable Agent Development Kit recipes, from single patterns to deployable agents.**

A recipe collection for Google's Agent Development Kit: core/ holds single-pattern agents (OAuth flows, session memory, guardrails, RAG), contrib/ holds deployable vertical agents targeting Agent Engine, Cloud Run and Gemini Enterprise, and plugins/ holds skills packaged with SKILL.md and EVAL.yaml. Each recipe has its own README; ADK SDKs exist for Python, TypeScript, Go, Java and Kotlin. For teams standardizing on ADK and Google Cloud.

- **+** Core recipes isolate one pattern each, so they lift cleanly into your project
- **+** Vertical agents include deploy paths to Agent Engine and Cloud Run
- **+** Recipe checklist and handbook define a contribution standard; tests and AGENTS.md included
- **+** Committed within the last day
- **−** Root README is an index; no single app, no shared setup
- **−** Gemini and Google Cloud are the assumed model and deploy target
- **−** README states recipes are demonstrations, not for production use
- **−** Mixed languages and maturity across folders

<sub>Python, google, google-adk · Needs google-adk, google-api-key-or-vertex-ai · [Repo](https://github.com/google/adk-recipes) · [📖 Docs ↗](https://adk.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-adk-recipes/)</sub>

<a name="xmcp"></a>
### #&#8288;18 [xmcp](https://github.com/basementstudio/xmcp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

**TypeScript framework for building MCP servers from one file per tool.**

xmcp is a TypeScript framework for writing MCP servers where each tool, prompt or resource is a file exporting a Zod schema, metadata and a function. It handles protocol, validation and transport, serving over HTTP or STDIO from the same code. It also provides adapters for Next.js, Express, NestJS, Hono and other frameworks, plus auth and payment integrations.

- **+** File system routing registers tools, prompts and resources with no configuration
- **+** Same code serves over HTTP or STDIO
- **+** Adapters for Next.js, Express, NestJS, Fastify, Hono, Nuxt, SvelteKit, Astro and more
- **+** Auth integrations include Better Auth, Clerk, Auth0, WorkOS and Supabase
- **−** TypeScript and Node.js only; no other language support
- **−** Tool schemas are written with Zod
- **−** No Docker or compose files in the repo
- **−** MCP Apps widgets are built with React

<sub>TypeScript · Needs Node.js · [Repo](https://github.com/basementstudio/xmcp) · [📖 Docs ↗](https://xmcp.dev/docs) · [🌐 Site ↗](https://xmcp.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/xmcp/)</sub>

<a name="agent-swarm"></a>
### #&#8288;19 [agent-swarm](https://github.com/desplega-ai/agent-swarm) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Lead agent that delegates tasks to Claude Code or Codex workers in containers.**

Agent Swarm runs a lead agent that takes tasks from Slack, GitHub/GitLab, email, or an API and delegates them to worker agents, each in its own Docker container. Workers use harnesses such as Claude Code, Codex, opencode, or Cursor, and share persistent memory with vector search, identity files, schedules, and workflows. Deploy with Docker Compose (reference file runs 1 lead and 11 workers), a Helm chart, or a one-line installer.

- **+** Supports many harnesses: Claude Code, Codex, pi, opencode, Cursor, Amp, Grok, Devin, ACP
- **+** Ships Compose, Helm chart, Railway template, and cloud-init deployment options
- **+** Integrates Slack, GitHub, GitLab, Linear, Jira, Azure DevOps, email, Telegram, Discord
- **+** Persistent memory with hybrid search, plus schema-validated task results and deferred tasks
- **−** Reference deployment needs at least 4 vCPU, 8 GB RAM and 40 GB disk
- **−** Default example runs 12 agents, so token spend can grow quickly
- **−** Installer exposes the API through a public tunnel unless --no-tunnel is passed
- **−** Repo changes daily; older workers need MULTI_RUNTIME_ENABLED=false after upgrades

<sub>TypeScript, Claude Code, Codex, pi, opencode · Needs Docker, Docker Compose v2, Bun (installer), Slack/GitHub/other integrations (optional) · Docker · env example file · [Repo](https://github.com/desplega-ai/agent-swarm) · [📖 Docs ↗](https://docs.agent-swarm.dev) · [🌐 Site ↗](https://agent-swarm.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-swarm/)</sub>

<a name="penguin-harness"></a>
### #&#8288;20 [penguin-harness](https://github.com/prism-shadow/penguin-harness) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Nov 2026</sub>

**Agent framework that evolves an agent's prompts, skills and tools against benchmarks.**

PenguinHarness runs agents with a small toolset and keeps the model fixed while it evolves the harness (prompts, Skills, tools, hooks) over scored rounds. Five RSI algorithms (default, OPRO, APE, ACE, AWM) ship as plugins and run on built-in Harbor benchmarks in Docker, with each candidate snapshotted as a version. It ships as a desktop app, Web App, CLI and TypeScript SDK, and can also generate agent apps from a prompt.

- **+** Five RSI algorithms run on the same benchmarks, scoreboard and per-version snapshots
- **+** Desktop app, Web App, CLI and SDK share one engine and the ~/.penguin/data directory
- **+** Works with many providers plus custom OpenAI-protocol endpoints, including local models
- **+** Agents can run on remote machines over ssh and drive Chrome through an extension
- **−** Benchmarks run as Harbor tasks in Docker, so self-evolution needs Docker
- **−** Cost and accuracy claims come from the project's own suite, not independent runs
- **−** Company-level self-evolution and OpenShell integration are still unchecked roadmap items

<sub>TypeScript, OpenAI, Anthropic, Google Gemini, OpenRouter · Needs Node >= 24 (npm install), Docker (benchmarks), Model provider API key · Docker · env example file · [Repo](https://github.com/prism-shadow/penguin-harness) · [📖 Docs ↗](https://penguin.ooo/docs/) · [🌐 Site ↗](https://penguin.ooo/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/penguin-harness/)</sub>

<a name="rivet-dev-agents"></a>
### #&#8288;21 [agents](https://github.com/rivet-dev/agents) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

**Runs coding agents as durable Rivet Actors or in sandboxes over HTTP.**

Rivet's agent infrastructure repo holds two projects. Rivet Agents runs agents such as Pi as durable Rivet Actors via the @rivet-dev/pi and @rivet-dev/sandbox-adapter packages. Sandbox Agent runs coding agents inside sandboxes and controls them over HTTP. Both ship on one version line.

- **+** Agents run as durable Rivet Actors via published npm packages
- **+** Sandbox Agent exposes sandboxed coding agents over HTTP
- **+** Single version line across npm packages, crates and binaries
- **+** Apache-2.0 license, active commits and releases in October 2026
- **−** README is a pointer table; setup and examples live in external docs
- **−** No Docker or Compose files detected in the repo
- **−** Two distinct projects in one repo, so scope is less focused

<sub>TypeScript · Needs Rivet Actors · [Repo](https://github.com/rivet-dev/agents) · [📖 Docs ↗](https://rivet.dev/agents/docs) · [🌐 Site ↗](https://rivet.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rivet-dev-agents/)</sub>

<a name="hello-halo"></a>
### #&#8288;22 [hello-halo](https://github.com/openkursar/hello-halo) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (43) · Freshness: active (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · custom license · Nov 2026</sub>

**Desktop AI workbench with scheduled agent teams and phone or IM handoff.**

Halo is a desktop app (TypeScript) for chat, coding, documents and research, with a canvas, browser and terminal beside the conversation. It adds "Digital Humans", scheduled or event-driven agents that can be grouped into teams, including teams spread across several computers. Work can be handed off from a phone, remote web, Feishu, WeChat or WeCom.

- **+** Runs Claude Code, Codex, its own Halo SDK or DeepSeek dsh as the agent engine
- **+** Accepts any Anthropic/OpenAI-compatible API or several ChatGPT, Claude and Copilot logins
- **+** Installers for macOS, Windows, Linux and an Android remote client; no server to deploy
- **+** Connects MCP servers and Skills; creates Word, Excel, PowerPoint and PDF files
- **−** Linux build does not include the AI terminal yet
- **−** iOS remote client must be built from source
- **−** Desktop app, not a template or library to fork into your own product
- **−** Cross-computer teams need Remote Access on the LAN or a configured relay gateway

<sub>TypeScript, Anthropic API, OpenAI-compatible API, ChatGPT, Claude · Needs Anthropic/OpenAI-compatible API key or ChatGPT/Claude/Copilot account · [Repo](https://github.com/openkursar/hello-halo) · [📖 Docs ↗](https://hello-halo.cc/) · [🌐 Site ↗](https://hello-halo.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hello-halo/)</sub>

<a name="agenticx"></a>
### #&#8288;23 [agenticx](https://github.com/demondamon/agenticx) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Python multi-agent framework with an Electron desktop client and Go gateway.**

AgenticX is a Python agent SDK and `agx` CLI with a FastAPI/SSE Studio server, covering a ReAct loop, graph workflows, MCP and A2A, memory, knowledge bases and sandboxed code execution. It also ships Near Desktop, an Electron app that talks to a local `agx serve`, and an Enterprise edition with a Go AI Gateway for auth, quota, audit and model relay.

- **+** Core install is about 27 lightweight dependencies; torch and others are optional extras
- **+** 15+ LLM providers including OpenAI, Anthropic, Ollama, Gemini, with failover routing
- **+** Supports MCP, A2A, AG-UI and OpenAPI tools, plus Docker, Microsandbox and subprocess sandboxes
- **+** Ships a desktop client and an enterprise gateway with audit, not just a library
- **−** Very broad scope; some storage adapters are placeholders or not wired into Studio
- **−** Studio path does not yet route every operation through the full SafetyLayer
- **−** Enterprise Cluster Agent Runtime is only planned; Edge Agent is an MVP
- **−** Near Desktop and Enterprise use independent runtime paths today

<sub>Python, OpenAI, Anthropic, Ollama, Gemini · Needs Python 3.10+, Redis (optional), PostgreSQL or MySQL (Enterprise), Chroma (Desktop knowledge base default), Docker or Microsandbox (optional sandbox) · Docker · [Repo](https://github.com/demondamon/agenticx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agenticx/)</sub>

<a name="antigravity-sdk-python"></a>
### #&#8288;24 [antigravity-sdk-python](https://github.com/google-antigravity/antigravity-sdk-python) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (63) · Freshness: active (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Oct 2026</sub>

**Python SDK for building Gemini-backed agents with tools, hooks and MCP.**

A Python SDK that wraps an agentic loop around Gemini, running through a compiled runtime binary shipped in platform-specific PyPI wheels. It offers an Agent class, a lower-level Conversation API, custom Python tools, MCP servers, a policy and hook system, and triggers. It can target the Gemini API, Vertex AI, or local Gemma 4 models through LiteRT-LM.

- **+** Declarative policies (deny, allow, ask_user) gate tool calls; run_command is denied by default
- **+** Supports Gemini API key, Vertex AI express mode, and Vertex with ADC
- **+** Offline local mode with Gemma 4 via LiteRT-LM
- **+** Python functions register as tools; MCP stdio servers and timed triggers are supported
- **−** Needs a compiled binary from PyPI wheels; cloning the repo is not enough
- **−** Local mode is only tested with one .litertlm file; others may fail or not work
- **−** Local mode recommends at least 24GB of VRAM or shared memory
- **−** Built around Gemini; no other hosted model providers are documented

<sub>Python, Gemini, Gemma 4 26B-A4B (LiteRT-LM) · Needs Gemini API key or Vertex AI credentials, compiled runtime binary (PyPI wheel), litert-lm (local models only) · [Repo](https://github.com/google-antigravity/antigravity-sdk-python) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/antigravity-sdk-python/)</sub>

<a name="rome"></a>
### #&#8288;25 [rome](https://github.com/rome-os/rome) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 907 · MIT · Nov 2026</sub>

**Agent runtime where agents build and keep installable apps and actions.**

Rome is a TypeScript pnpm monorepo with an agent runtime, a web dashboard and an app model. Agents can scaffold git-tracked Rome Apps (an app.yaml manifest plus actions, agents, skills, hooks, web UI and a private database) that are reused in later tasks. It runs from a Docker quickstart on port 7663 or on the Rome Cloud preview, and connects to Telegram, Discord and WhatsApp.

- **+** Apps, actions and skills are stored as git-tracked source code, not hidden model state
- **+** Public SDKs for apps: @rome-os/app-runtime and @rome-os/app-web-sdk
- **+** Actions can pause for approval, and every run is recorded
- **+** One-script Docker quickstart; state lives in named volumes and survives upgrades
- **−** Docker images default to romeos.cc and also run a signer container for Rome Cloud
- **−** Rome Cloud is a preview; the Mac app does not run Rome locally
- **−** README says the dev setup is not the final production self-hosting distribution
- **−** First-run onboarding is open to whoever reaches it first if exposed beyond loopback

<sub>TypeScript · Needs Docker, Docker Compose, Node.js 24+ (development), pnpm 11.6 (development) · Docker · [Repo](https://github.com/rome-os/rome) · [📖 Docs ↗](https://romeos.cc/docs/rome) · [🌐 Site ↗](https://romeos.cc/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rome/)</sub>

<a name="kohakuterrarium"></a>
### #&#8288;26 [kohakuterrarium](https://github.com/kohaku-lab/kohakuterrarium) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 556 · custom license · Nov 2026</sub>

**Python framework for building agents from tools, triggers and sub-agents.**

KohakuTerrarium is a Python framework where an agent (a "creature") is a controller loop plus input, output, tools, triggers and sub-agents, defined in a config file or custom modules. A Terrarium engine hosts many creatures wired through channels, with session persistence, resume, and CLI, TUI, web and desktop surfaces. The separate kt-biome pack supplies ready-made agents such as a software-engineering creature.

- **+** Agents embed as awaitable Python objects with typed TurnResult and timeouts that cancel
- **+** Sessions are persisted and searchable; resume with `kt resume` or Terrarium.resume
- **+** MCP stdio and streamable-HTTP servers, with four meta-tools to keep prompts small
- **+** Providers include Codex OAuth, OpenAI, Anthropic, Gemini and any OpenAI-compatible API
- **−** Custom license (KohakuTerrarium-1.0, detected as NOASSERTION); check terms before commercial use
- **−** Ready-made agents live in a separate kt-biome package
- **−** Source install needs a manual npm build of the web frontend
- **−** README says it is not suited to sub-50 ms per-operation latency

<sub>Python, Codex OAuth, OpenAI, OpenRouter, Anthropic · Needs Python 3.10+ (3.12+ recommended), LLM provider account or API key, Node/npm for source frontend build · Docker · [Repo](https://github.com/kohaku-lab/kohakuterrarium) · [📖 Docs ↗](https://terrarium.kohaku-lab.org) · [🌐 Site ↗](https://terrarium.kohaku-lab.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kohakuterrarium/)</sub>

<a name="frontieragent"></a>
### #&#8288;27 [frontieragent](https://github.com/apodexai/frontieragent) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · Apache-2.0 · Nov 2026</sub>

**Terminal agent runtime with single-agent and parallel sub-agent research workflows.**

FrontierAgent is a Python terminal UI and agent runtime for long-horizon research and file-based work. It has two modes: a stateful ReAct agent, and an Agent Team where a coordinator delegates to parallel sub-agents through a task board. Shell and file tools run in a task-scoped sandbox with /inputs, /workspace and /outputs, with diff approval, checkpoints and /revert. It also bundles a benchmark runner for BrowseComp, HLE, GDPval and others.

- **+** Agent Team mode with live task board and bounded parallel sub-agents
- **+** Read-only /inputs, writable /workspace and /outputs; mutations need approval and are revertable
- **+** Works with any OpenAI-compatible endpoint; optional keyless Parallel MCP for web search
- **+** Bundled benchmark harness with resumable runs and per-failure reruns
- **−** Aimed at research and file deliverables rather than code editing in an IDE
- **−** Agent Team concurrency multiplies with runner concurrency, raising simultaneous model calls
- **−** Prebuilt GHCR image is private and needs docker login; otherwise build from source
- **−** Local SGLang serving depends on pinned NVIDIA driver and CUDA tracks

<sub>Python, OpenAI-compatible endpoints, Apodex-1.1, SGLang-served models · Needs Python 3.12, uv, OpenAI-compatible model endpoint, Serper or Jina API keys (optional), Docker (optional), SGLang (optional) · Docker · env example file · [Repo](https://github.com/apodexai/frontieragent) · [🌐 Site ↗](https://www.apodex.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frontieragent/)</sub>

<a name="bindu"></a>
### #&#8288;28 [bindu](https://github.com/getbindu/bindu) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: weak (22) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · custom license · Sep 2026</sub>

**Wraps an agent handler with DID identity, A2A protocol and x402 payments.**

Bindu exposes an existing agent as an A2A JSON-RPC service on port 3773 through a single bindufy() call. It adds a DID-based Ed25519 identity, optional mTLS via step-ca, OAuth2 via Ory Hydra, and x402 USDC payments on EVM chains. SDKs exist for Python, TypeScript and Kotlin over a shared gRPC core, and the handler can use any framework.

- **+** Framework-agnostic: tested with Agno, CrewAI, LangChain, LangGraph, AG2 and others
- **+** Three auth layers together: mTLS, Hydra OAuth2 and DID body signatures
- **+** x402 USDC payments with 5 chains preconfigured, other EVM chains via config
- **+** Python, TypeScript and Kotlin SDKs share one gRPC core
- **−** Full security stack depends on step-ca and Ory Hydra, which you must run
- **−** Postgres and Redis are needed for storage and scheduler features
- **−** README points to a known-issues file to read before production use
- **−** Detected license is NOASSERTION, while the README says Apache 2.0

<sub>Python, OpenAI, OpenRouter, MiniMax, OpenAI-compatible APIs · Needs Python 3.12+, uv, Smallstep step-ca, Ory Hydra, PostgreSQL, Redis, LLM provider API key · [Repo](https://github.com/getbindu/bindu) · [▶️ Demo ↗](https://www.youtube.com/watch?v=qppafMuw_KI) · [📖 Docs ↗](https://docs.getbindu.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bindu/)</sub>

<a name="opencrabs"></a>
### #&#8288;29 [opencrabs](https://github.com/opencrabs/opencrabs) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Rust terminal AI agent with multi-provider LLM support and local memory.**

OpenCrabs is a single Rust binary that runs an LLM agent in a Ratatui terminal UI. It calls providers directly over HTTPS (Anthropic, OpenAI, Copilot, OpenRouter, Gemini, local Ollama or LM Studio and others), with fallback chains, prompt caching and auto-compaction. State is kept in local SQLite with a 3-tier memory, cron jobs, a /goal loop and an A2A protocol.

- **+** Single 34-36 MB binary with no Node runtime; data stays in ~/.opencrabs
- **+** Many providers plus fallback chains and any OpenAI-compatible local endpoint
- **+** Hybrid FTS5 and vector memory search with published benchmark reports
- **+** Local whisper.cpp speech-to-text; README states zero telemetry
- **−** Large feature surface (A2A, cron, epistemic engine) makes configuration heavy
- **−** No Docker image or compose file detected; install is binary or source build
- **−** Benchmarks and framework comparisons are self-reported by the project
- **−** Terminal-first; no web UI is described in the visible README

<sub>Rust, Anthropic Claude, OpenAI, GitHub Copilot, OpenRouter · Needs SQLite (embedded), LLM provider API or local LLM server · [Repo](https://github.com/opencrabs/opencrabs) · [📖 Docs ↗](https://docs.opencrabs.com) · [🌐 Site ↗](https://opencrabs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencrabs/)</sub>

<a name="mcp-typescript-template"></a>
### #&#8288;30 [mcp-typescript-template](https://github.com/nickytonline/mcp-typescript-template) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (0) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 61 · MIT · Oct 2026</sub>

**TypeScript starter for remote MCP servers over HTTP with Express and Effect.**

A degit-able template for building stateless, remote MCP servers on Node 24.11+ using the MCP TypeScript SDK, Express and Effect. It ships two example tools (echo and elicit_echo) with typed input and output schemas, plus an example Agent Skill published through the MCP Skills extension. Build, test, lint and format run through the Vite+ vp CLI.

- **+** Example tools cover structured output, annotations and MCP elicitation with accept/decline/cancel handling
- **+** Stateless per-request server following the MCP 2026-07-28 spec, with fallback for older clients
- **+** Includes Dockerfile, compose file with health check, and in-memory client/server integration tests
- **+** Bundles an example Agent Skill served via skills/list, skills/get and resources/read
- **−** Requires Node.js 24.11 or newer; Vite+ does not run on earlier Node 24 releases
- **−** Tool code is written in Effect, which adds a learning curve for teams not using it
- **−** HTTP transport only; the README mentions no stdio transport
- **−** No auth or database included; only two toy example tools

<sub>TypeScript · Needs Node.js 24.11+, Express, Effect, @modelcontextprotocol/server, Vite+ · GitHub template · Docker · [Repo](https://github.com/nickytonline/mcp-typescript-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-typescript-template/)</sub>

<a name="ai-town"></a>
### #&#8288;31 [ai-town](https://github.com/a16z-infra/ai-town) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**Simulated pixel-art town where LLM characters chat, remember and socialize.**

AI Town is a TypeScript starter for a Generative Agents-style simulation: AI characters move around a PixiJS map, hold conversations and keep vector-searched memories. Convex provides the game engine, database and vector search. The LLM defaults to llama3 with mxbai-embed-large via Ollama, and OpenAI, Together.ai or any OpenAI-compatible API can be configured instead.

- **+** Convex backend supplies shared state, transactions, simulation engine and vector search in one stack
- **+** Runs fully local with Ollama, or with OpenAI, Together.ai or any OpenAI-compatible endpoint
- **+** Characters, spritesheets and Tiled maps are editable through data files and a conversion script
- **+** Docker Compose setup with self-hosted Convex and dashboard; Fly.io instructions also included
- **−** Changing LLM provider or embedding model requires wiping the database, since vector dimensions must match
- **−** Editing characters requires wiping all tables and re-uploading data to Convex
- **−** Clerk auth was removed from the default code and must be restored by reverting a commit
- **−** Simulation pauses after 5 minutes of idle browser unless the cron is disabled

<sub>TypeScript, Ollama (llama3, mxbai-embed-large), OpenAI, Together.ai, OpenAI-compatible APIs · Needs Convex, Ollama, Node.js 18, Clerk (optional), Replicate (optional) · Docker · sign-in: Clerk · [Repo](https://github.com/a16z-infra/ai-town) · [▶️ Demo ↗](https://www.convex.dev/ai-town) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-town/)</sub>

<a name="commonly"></a>
### #&#8288;32 [commonly](https://github.com/team-commonly/commonly) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Nov 2026</sub>

**Shared team workspace where people and their own agents talk in one pod.**

Commonly is a chat workspace where teammates join a pod by link and @mention agents, each a named member with an owner. You connect your own Claude Code, Codex or OpenCode through the `commonly` CLI, and agents file and claim tasks on a shared board. Connectors are granted per pod and per agent. Self-host runs MongoDB and PostgreSQL via Docker Compose.

- **+** Connects your own Claude Code, Codex or OpenCode via an npm CLI
- **+** Connector grants are scoped per pod and agent; read-only grants expose only read actions
- **+** Shared task board where a connected agent claims a card under its own name
- **+** One-command self-host with ./install.sh runs MongoDB and PostgreSQL locally
- **−** Hosted agents are not available in self-hosted installs; only agents you bring
- **−** Self-host is local-only: no TLS or public domain from the default install
- **−** Linux needs bubblewrap; own-login Claude Code path on Linux is verified in CI only
- **−** Native Windows runs Claude Code with --unsandboxed and no connector grants

<sub>JavaScript, Claude Code, Codex, OpenCode · Needs Docker, Docker Compose v2, MongoDB, PostgreSQL, bubblewrap (Linux agents) · env example file · [Repo](https://github.com/team-commonly/commonly) · [▶️ Demo ↗](https://commonly.me) · [📖 Docs ↗](https://docs.commonly.me/quickstart) · [🌐 Site ↗](https://commonly.me) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/commonly/)</sub>

<a name="pipelex"></a>
### #&#8288;33 [pipelex](https://github.com/pipelex/pipelex) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 951 · custom license · Nov 2026</sub>

**Runtime for typed, multi-step AI methods written as .mthds files.**

Pipelex is a Python runtime that reads declarative .mthds files (the MTHDS standard) and runs them as chained LLM, OCR and image-generation steps with typed inputs and outputs. Methods run from the CLI, Python, a TypeScript SDK, REST API, MCP or n8n, on the hosted Pipelex API or locally with your own provider keys or local models. A plugin for Claude Code and Codex helps write the methods.

- **+** Declarative .mthds files with typed concepts, reusable across models and providers
- **+** Runs from CLI, Python, TypeScript SDK, REST API, MCP or n8n
- **+** Works with OpenAI, Anthropic, Google, Mistral, Bedrock, plus Ollama, vLLM, LM Studio, llama.cpp
- **+** Runs locally with own keys or on the hosted API with no provider account
- **−** Elastic License 2.0 is source-available, not OSI open source
- **−** Hosted path and plugin workflow require a Pipelex account and API key
- **−** Plugin hook and tools require Node.js on PATH
- **−** Anonymous usage statistics are on by default and must be disabled manually

<sub>Python, OpenAI, Azure OpenAI, Anthropic, Google Gemini/Vertex · Needs Python, uv, Node.js (for plugin), Pipelex API key or provider API keys · env example file · [Repo](https://github.com/pipelex/pipelex) · [▶️ Demo ↗](https://go.pipelex.com/demo) · [📖 Docs ↗](https://docs.pipelex.com/) · [🌐 Site ↗](https://www.pipelex.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pipelex/)</sub>

<a name="nasiko"></a>
### #&#8288;34 [nasiko](https://github.com/nasiko-labs/nasiko) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (86) · Freshness: active (92) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Nov 2026</sub>

**Control plane that tracks cost and routes LLM calls for coding agents.**

Nasiko is a single Rust server and CLI that discovers installed coding harnesses (Claude Code, Codex, OpenCode, Cursor CLI), reports their sessions and spend, and can route their LLM calls to a provider you configure. It also deploys A2A-speaking agents into Docker behind one proxy, with an MCP gateway, flow limits, ACLs and OTel traces. State lives in Postgres, Redis and S3-compatible storage.

- **+** Read-only `nasiko agents discover` changes no settings, needs no account, sends nothing off-machine
- **+** Routes Anthropic-format Claude Code traffic to an OpenAI key, decoupling protocol from provider
- **+** Agents get short-lived tokens, so no agent or log sees a real API key
- **+** Cost and traces per agent and model via gen_ai OTel span attributes
- **−** Cursor CLI supports discovery and reporting only; LLM routing is not yet available
- **−** Routing edits global per-user config, affecting every Claude Code or OpenCode process
- **−** Needs Postgres, Redis and S3 backing services plus a running control plane
- **−** OpenCode routing applies only to new sessions; existing sessions keep their model

<sub>Rust, OpenAI, Anthropic · Needs Docker, Postgres, Redis, S3 (RustFS), OTel Collector (optional), Tempo (optional), Loki (optional), Rust toolchain (for CLI) · env example file · [Repo](https://github.com/nasiko-labs/nasiko) · [📖 Docs ↗](https://docs.nasiko.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nasiko/)</sub>

<a name="open-agent-email"></a>
### #&#8288;35 [open-agent-email](https://github.com/anil-matcha/open-agent-email) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (46) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Oct 2026</sub>

**Self-hosted email inboxes for AI agents with an approval gate.**

Runs a FastAPI server with its own SMTP listener on port 25 that gives each agent a real address, threaded mailbox and API. Incoming mail is checked for SPF, DKIM and DMARC and scanned for prompt injection. Outgoing mail goes through a relay you configure (SES, Resend, SendGrid, Postmark, Gmail) and can be held until a person approves it. Agents connect through REST, webhooks, WebSocket, Python and TypeScript SDKs, a CLI, or 96 MCP tools.

- **+** Approval gate with emailed approve/reject links, expiry and per-message history
- **+** Per-inbox API keys with read-only, send and review-only scopes
- **+** Many integration paths: REST, signed webhooks, WebSocket, SDKs without dependencies, CLI, MCP
- **+** SQLite by default, PostgreSQL supported; includes dashboard and Alembic migrations
- **−** Single-user: one admin key, no customer accounts or multi-tenancy yet
- **−** Receiving from large providers and off-host backups still in progress
- **−** Receiving internet mail requires a public host, MX record and open port 25
- **−** Delivery and bounce tracking is built only for Amazon SES

<sub>Python · Needs SMTP relay (e.g. Amazon SES), PostgreSQL (optional), Node.js (dashboard) · [Repo](https://github.com/anil-matcha/open-agent-email) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-agent-email/)</sub>

<a name="ms-agent"></a>
### #&#8288;36 [ms-agent](https://github.com/modelscope/ms-agent) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (65) · Freshness: active (95) · Maintenance: patchy (40) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · Apache-2.0 · Nov 2026</sub>

**Python agent framework with CLI, TUI and WebUI, skills, sub-agents and MCP.**

MS-Agent is a Python SDK and harness for long-running agents. It handles planning, permissions, context compression, project memory and cron jobs, and supports sub-agents, sequential or DAG workflows, Agent Skills and MCP tools. The same agent logic runs from a CLI, a terminal UI or a browser WebUI, and the repo ships example apps for deep research, code generation and video generation.

- **+** One Python SDK drives CLI, TUI and WebUI, so agent logic is reused across interfaces
- **+** Context compaction, project memory and cron scheduling target long-running tasks
- **+** Supports MCP, ACP/A2A, Agent Skills and DAG or sequential multi-agent workflows
- **+** Bundled apps: deep research, Code Genesis, FinResearch, Singularity Cinema
- **−** WebUI must be installed from source; needs Python 3.12+, Node.js 22.22.0+, pnpm and uv
- **−** No Docker or compose files detected in the repo
- **−** Default provider is ModelScope and needs an API key from its token page
- **−** README is dominated by a long news log; the many bundled apps make scope broad

<sub>Python, ModelScope, multiple model providers, Anthropic API format, multimodal input (image, video) · Needs Python 3.12+ (WebUI), Node.js 22.22.0+, pnpm 10.17.1, uv 0.5+, LLM provider API key (ModelScope by default) · Docker · env example file · [Repo](https://github.com/modelscope/ms-agent) · [▶️ Demo ↗](https://modelscope.cn/mcp/playground) · [📖 Docs ↗](https://ms-agent-en.readthedocs.io) · [🌐 Site ↗](https://modelscope.github.io/ms-agent/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ms-agent/)</sub>

<a name="opengenerativeui"></a>
### #&#8288;37 [OpenGenerativeUI](https://github.com/copilotkit/openintelligentui) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Oct 2026</sub>

**Chat interface that answers with generated interactive UI, charts, maps and tools.**

A Next.js and CopilotKit chat frontend backed by a Python Deep Agent (FastAPI). For each turn the agent returns text, a native component, or custom HTML/CSS/JS streamed into a sandboxed iframe. A router model (Jev) picks A2UI for basic tables and Open Generative UI for charts, diagrams, calculators and maps. It is meant to be cloned and adapted rather than used as-is.

- **+** Generated UI runs in an isolated iframe with a validated host bridge for follow-ups
- **+** Visitors can supply their own keys, held in browser memory only, not storage
- **+** Optional standalone MCP server with HTTP, stdio and Docker configuration
- **+** MIT licensed, with a documented architecture and launch verification workflow
- **−** Needs both an OpenAI key and a TYPESAFE_API_KEY for the Jev router
- **−** Provider failures are surfaced; no fallback to another model or router
- **−** Output varies per run because the router chooses the presentation
- **−** Setup needs Node 22+, pnpm 9+, Python 3.12+ and uv; no release published

<sub>TypeScript, OpenAI chat-latest, jev-latest · Needs OpenAI API, Jev router (TYPESAFE_API_KEY), Node.js 22+, pnpm 9+, Python 3.12+, uv · Docker · env example file · [Repo](https://github.com/copilotkit/openintelligentui) · [📖 Docs ↗](https://github.com/CopilotKit/OpenIntelligentUI/blob/main/docs/README.md) · [🌐 Site ↗](https://copilotkit.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opengenerativeui/)</sub>

<a name="relay"></a>
### #&#8288;38 [relay](https://github.com/agentworkforce/relay) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (21) · Freshness: active (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 887 · Apache-2.0 · Oct 2026</sub>

**Messaging and enforced workflows for teams running several coding agents.**

Agent Relay connects coding agents such as Claude Code and Codex through shared channels, threads, DMs and search, including across machines. It exposes GitHub, Linear, Notion and Slack as a virtual filesystem, captures sessions for team search, and defines multi-step flows in TypeScript with deterministic checks and human gates. Setup is `npx -y agent-relay init` on Node.js 22 or newer.

- **+** Works alongside Claude Code and Codex without replacing them
- **+** Flows put required steps and human gates in TypeScript, not prompts
- **+** Agents on different machines share channels, DMs, files and search
- **+** Self-hosting options exist for each component, with a guide
- **−** Shared sessions and wider cross-agent communication need the paid desktop app
- **−** Shared Sessions MCP requires Cloud login
- **−** Team setup defaults to a hosted service via init --hosted
- **−** Integrations, session capture and flows live in separate repositories

<sub>TypeScript, Claude Code, Codex · Needs Node.js 22+ · [Repo](https://github.com/agentworkforce/relay) · [📖 Docs ↗](https://agentrelay.com/docs) · [🌐 Site ↗](https://agentrelay.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/relay/)</sub>

<a name="unla"></a>
### #&#8288;39 [unla](https://github.com/amoylab/unla) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (49) · Freshness: active (100) · Maintenance: weak (28) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Oct 2026</sub>

**Gateway that exposes REST APIs and existing MCP servers as MCP endpoints.**

Unla is a Go gateway that turns REST APIs into MCP servers through YAML configuration, and also proxies existing MCP servers. It serves MCP over SSE and Streamable HTTP, and includes a web UI for adding servers and a chat page for testing. Config can be stored on disk, SQLite, PostgreSQL or MySQL, and synced across replicas.

- **+** Converts REST APIs to MCP servers from YAML, with no changes to the backend
- **+** Supports SSE and Streamable HTTP, plus text, image and audio responses
- **+** Config persists to disk, SQLite, PostgreSQL or MySQL, with hot-reload and versioning
- **+** Multi-replica operation with sync over OS signals, HTTP or Redis PubSub; Helm supported
- **−** gRPC and WebSocket conversion are unchecked on the roadmap
- **−** Grouping and aggregating multiple MCP servers is not yet implemented
- **−** README warns backward compatibility is not guaranteed and docs may lag releases
- **−** Only auth feature listed is OAuth pre-authentication for MCP servers

<sub>TypeScript · Needs SQLite, PostgreSQL or MySQL (optional), Redis (optional, config sync) · env example file · [Repo](https://github.com/amoylab/unla) · [📖 Docs ↗](https://docs.unla.amoylab.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unla/)</sub>

<a name="exo"></a>
### #&#8288;40 [exo](https://github.com/exoharness/exo) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (41) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Nov 2026</sub>

**Runtime that hosts Codex, Claude Code or Pi agents behind an API.**

Exo is a Rust runtime that turns a markdown agent definition into a hosted agent with durable conversations, sandboxes, a credential vault and network policies. It separates harness behavior (compaction, tool calling, planning) from infrastructure, and supports Codex, Claude Code and Pi out of the box. It is positioned as a self-hostable alternative to Claude Managed Agents and OpenAI's Agents API.

- **+** Agent defined in one markdown file with harness, model and credential fields
- **+** Harness and model agnostic: Codex, Claude Code and Pi supported, custom harnesses extendable
- **+** Credential substitution and granular network policies for unsupervised agent runs
- **+** Durable history and environments let clients disconnect and resume
- **−** README says docs are under construction and some documented features are unimplemented
- **−** Installation instructions not written; only a development setup from the repo
- **−** No tagged release yet
- **−** Exo-side code models Codex and Claude Code event lifecycles, adding complexity

<sub>Rust, Codex harness, Claude Code harness, Pi harness, OpenAI · Needs Model provider API key (e.g. OPENAI_API_KEY) · env example file · [Repo](https://github.com/exoharness/exo) · [📖 Docs ↗](https://exoharness.ai/docs) · [🌐 Site ↗](https://exoharness.ai/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/exo/)</sub>

<a name="innovation-lab-examples"></a>
### #&#8288;41 [innovation-lab-examples](https://github.com/fetchai/innovation-lab-examples) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

**Collection of 80+ runnable Python agent examples built on Fetch.ai uAgents.**

A monorepo of self-contained Python agent projects, each with its own README, requirements and .env.example. Examples cover uAgents on Agentverse, ASI:One, A2A, MCP servers, Stripe, FET and Skyfire payments, RAG, and CrewAI, Google ADK, AG2, LangChain and LlamaIndex integrations. A root Dockerfile and setup.sh run any single example.

- **+** Each folder is self-contained with its own dependencies and env template
- **+** Covers many frameworks: CrewAI, Google ADK, AG2, LangChain, LlamaIndex, Pydantic AI
- **+** Includes payment examples using Stripe, FET and Skyfire
- **+** Root Dockerfile and setup.sh run any example by name
- **−** Tightly coupled to the Fetch.ai uAgents, Agentverse and ASI:One ecosystem
- **−** Most examples need third-party API keys (ASI:One, OpenAI, Stripe, etc.)
- **−** Not a single app; depth and quality vary per example
- **−** README and badge say Apache 2.0, detected license is MIT

<sub>Python, ASI:One, OpenAI, Anthropic Claude, Google Gemini · Needs Python 3.10+, ASI:One API key, Agentverse, OpenAI/Anthropic/Gemini keys (per example), Stripe (some examples) · Docker · [Repo](https://github.com/fetchai/innovation-lab-examples) · [📖 Docs ↗](https://innovationlab.fetch.ai/resources/docs/intro) · [🌐 Site ↗](https://fetch.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/innovation-lab-examples/)</sub>

<a name="agents-universe"></a>
### #&#8288;42 [agents-universe](https://github.com/agents-universe/agents-universe) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (19) · Freshness: active (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 861 · Apache-2.0 · Nov 2026</sub>

**Self-hosted multi-agent platform with Product Owner, Tech Lead and QA roles.**

Vue 3 and FastAPI platform that ships 10 built-in agents (Product Owner, Tech Lead, QA, office documents, data analysis, pentesting and others) over Anthropic, OpenAI, Azure OpenAI and Gemini. Agents load project knowledge as full files with no vector search, plan tasks, and run inside a two-layer sandbox. Tech Lead can clone a repo, write code, run tests and open a PR from a Jira card.

- **+** Per-user LLM keys stored with AES-256-GCM; automatic routing between model tiers
- **+** Database selectable via DATABASE_URL: SQL Server, PostgreSQL, MySQL or SQLite
- **+** Skills, workflows and knowledge are plain markdown files, so they can be committed and reused
- **+** Scheduled cron tasks run Playwright scripts without spending tokens
- **−** Default setup uses SQL Server and Redis; first Docker build takes about 10-30 minutes
- **−** AUTH_BYPASS_ENABLED defaults to true; production needs it off and OAuth SSO configured
- **−** Full knowledge loading is bounded by a token budget; extra files are read on demand
- **−** README is mostly in Chinese; workflows lean on Jira and Confluence

<sub>Python, Anthropic, OpenAI, Azure OpenAI, Google Gemini · Needs Docker Compose, SQL Server (or PostgreSQL/MySQL/SQLite), Redis 7, Playwright (Chromium) · Docker · [Repo](https://github.com/agents-universe/agents-universe) · [▶️ Demo ↗](https://agents-universe.com) · [🌐 Site ↗](https://agents-universe.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents-universe/)</sub>

<a name="create-context-graph"></a>
### #&#8288;43 [create-context-graph](https://github.com/neo4j-labs/create-context-graph) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 749 · Apache-2.0 · Oct 2026</sub>

**CLI that scaffolds domain-specific FastAPI and Next.js apps on a Neo4j graph.**

An interactive CLI (uvx or npx) that generates a full-stack app from a domain ontology: a FastAPI backend with an agent, and a Next.js frontend with streaming chat, graph visualization and a document browser. You pick one of 27 industry domains or describe a custom one, plus one of eight agent frameworks. Memory runs on hosted NAMS or self-hosted Neo4j, and data can be imported from sources such as GitHub, Slack and Jira.

- **+** Eight agent frameworks selectable at scaffold time, including PydanticAI, LangGraph, CrewAI and Google ADK
- **+** 27 prebuilt domain ontologies with sample data, plus LLM-generated custom domains
- **+** Twelve import connectors, including GitHub, Slack, Jira, Linear, Claude Code and ChatGPT exports
- **+** Optional MCP server config so Claude Desktop can query the same graph
- **−** Experimental Neo4j Labs project, not officially supported
- **−** Default NAMS backend needs a hosted API key and cannot write native edges
- **−** On NAMS, GDS endpoints and arbitrary Cypher writes return 501
- **−** No tagged release published

<sub>Python, Anthropic, OpenAI, Google Gemini, LiteLLM providers (Bedrock, Vertex AI, Ollama, Groq, Together) · Needs Neo4j 5+ (self-hosted) or NAMS hosted memory, Python 3.11+, Node.js 18+, Anthropic, OpenAI or Google API key · [Repo](https://github.com/neo4j-labs/create-context-graph) · [📖 Docs ↗](https://create-context-graph.dev/) · [🌐 Site ↗](https://create-context-graph.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/create-context-graph/)</sub>

<a name="deuz-sdk"></a>
### #&#8288;44 [deuz-sdk](https://github.com/deuz-ai/deuz-sdk) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 508 · MIT · Oct 2026</sub>

**TypeScript SDK for model calls, agents and multi-agent swarms.**

Deuz SDK (@deuz-sdk/core) is a TypeScript library with zero required runtime dependencies. It covers model calls with streaming, structured output and tool calls, plus native agents and swarms persisted to SQLite, Postgres or Redis. Version 2.4 adds versioned memory, a context compiler, a goal supervisor and a preview Docker sandbox, all off until configured.

- **+** Core has zero required runtime dependencies; integrations use optional peers
- **+** Swarms persist to SQLite, Postgres or Redis, with resumable runs and crash recovery
- **+** Includes MCP server, A2A, realtime voice, batch requests and optional React bindings
- **+** 23 examples; 07-22 run without an API key or network
- **−** Nothing in 2.4 was run against a real model provider, only scripted models
- **−** Docker sandbox runner and headless mode are marked preview
- **−** Without a lease provider, each swarm or agent run must be driven from one process
- **−** Requires Node.js 22+ or an edge runtime with Web APIs

<sub>TypeScript, Anthropic, multiple providers · Needs Node.js 22+, SQLite, Postgres or Redis (optional), Docker (optional sandbox) · [Repo](https://github.com/deuz-ai/deuz-sdk) · [📖 Docs ↗](https://deuz-sdk.tech/docs) · [🌐 Site ↗](https://deuz-sdk.tech/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deuz-sdk/)</sub>

<a name="commerce-agents"></a>
### #&#8288;45 [commerce-agents](https://github.com/anthropics/commerce-agents) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · Apache-2.0 · Aug 2026</sub>

**Reference shopping and merchant agents for commerce, built on Claude.**

Python reference implementation of two Claude agents: a customer-facing shopping agent and a staff-facing merchant agent. Each is defined once (prompt, skills, tool contracts, gates) and runs on the Messages API, the Claude Agent SDK, or Managed Agents. Four fictional verticals (retail, travel, telecom, entertainment) ship with web storefronts and portals; you implement StorefrontBackend or MerchantBackend over your own systems.

- **+** Same prompt, skills and tool contracts run on Messages API, Agent SDK and Managed Agents
- **+** Merchant writes are staged until a person approves; checkout is handed off to the host
- **+** Four runnable verticals with storefront and portal web apps via scripts/run_demo.py
- **+** Includes a Claude Code plugin that scaffolds and reviews commerce agents
- **−** Not maintained and does not accept contributions, per the README
- **−** Example hosts have no authentication; MCP servers bind to loopback only
- **−** Requires an Anthropic API key; other platforms are covered only in docs/deployment.md
- **−** No MCP connectors ship; you write backend methods for every system

<sub>Python, Claude · Needs Anthropic API key, Python 3.11+, Node 22 · env example file · [Repo](https://github.com/anthropics/commerce-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/commerce-agents/)</sub>

<a name="personal-agent-template"></a>
### #&#8288;46 [personal-agent-template](https://github.com/vercel-labs/personal-agent-template) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 497 · MIT · Nov 2026</sub>

**Nuxt and Eve personal agent with web chat, Slack, GitHub, Linear and memory.**

A forkable template for a personal agent built on the Eve agent framework and Nuxt. The same agent answers in a web chat and in Slack, calls GitHub and Linear tools, and keeps a per-user memory document in Vercel Blob. Auth uses Better Auth, and data lives in PostgreSQL through NuxtHub and Drizzle.

- **+** One agent serves web chat and Slack, with Slack linked to the web profile
- **+** Per-user memory recalled before each turn, outside history, so it survives compaction
- **+** GitHub tools require durable approval on writes
- **+** Includes email/password auth, Postgres migrations and a daily summary skill
- **−** Tied to Eve, Nuxt and Vercel services (Connect, Blob, Sandbox Drive)
- **−** Memory storage needs a Vercel Blob store attached before deploying
- **−** Linear and Slack integrations depend on Vercel Connect
- **−** No Docker or compose files; self-hosting needs Node.js 24+ and pnpm

<sub>TypeScript · Needs Node.js 24+, pnpm, PostgreSQL (NuxtHub), Vercel Blob, Vercel Connect, Better Auth, Eve · GitHub template · env example file · sign-in: Better Auth · [Repo](https://github.com/vercel-labs/personal-agent-template) · [📖 Docs ↗](https://github.com/vercel-labs/personal-agent-template/blob/main/docs/CUSTOMIZATION.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/personal-agent-template/)</sub>

<a name="shepherd"></a>
### #&#8288;47 [shepherd](https://github.com/shepherd-agents/shepherd) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Sep 2026</sub>

**Python runtime that records agent runs as reviewable, reversible traces.**

Shepherd is a Python framework where a task is a bodiless function whose signature and docstring define what a sandboxed agent (e.g. Claude via the claude CLI) must do. Agent output is held as a retained changeset that you inspect, then select, apply, release or discard. Write permissions come from type annotations such as May[GitRepo, ReadOnly], enforced by macOS Seatbelt or Linux Landlock. The project is in early alpha.

- **+** Agent writes land as retained outputs; nothing touches your files until you accept
- **+** Per-repository ReadOnly/ReadWrite grants declared in the signature, enforced at the syscall
- **+** Offline quickstart with a deterministic provider needs no API key
- **+** Three-way merge of a candidate onto a workspace that has moved on
- **−** Early alpha; README warns APIs may change between releases
- **−** Windows unsupported; WSL required
- **−** Linux Landlock enforcement runs only in a privileged container
- **−** Grants are whole-profile per binding; sub-path grants not supported yet

<sub>Python, Claude (via claude CLI, subscription or ANTHROPIC_API_KEY), deterministic offline provider · Needs Python 3.11+, claude CLI (for the agent quickstart) · Docker · env example file · [Repo](https://github.com/shepherd-agents/shepherd) · [📖 Docs ↗](https://docs.shepherd-agents.ai/) · [🌐 Site ↗](https://shepherd-agents.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shepherd/)</sub>

<a name="tinyfish-cookbook"></a>
### #&#8288;48 [tinyfish-cookbook](https://github.com/tinyfish-io/tinyfish-cookbook) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (50) · Freshness: active (100) · Maintenance: weak (28) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Nov 2026</sub>

**Example apps and n8n workflows built on the TinyFish web agent API.**

A monorepo of standalone recipes that call TinyFish's hosted Search, Fetch, Agent and Browser endpoints. Most are small web apps (price comparison, tutor and scholarship finders, supply-chain tracking) with live Vercel demos, plus three n8n workflows and a use-tinyfish agent skill. The README also documents the REST API, MCP server, CLI and Python/TypeScript SDKs.

- **+** Dozens of standalone recipes, many with live demos you can try before cloning
- **+** Covers REST, MCP server URL, CLI, Python and TypeScript SDKs with curl examples
- **+** Includes importable n8n workflows and an installable agent skill for coding agents
- **+** MIT licensed; Search and Fetch endpoints are free per the README
- **−** Every recipe depends on the hosted TinyFish API and a key; nothing runs offline
- **−** Agent and Browser endpoints are metered, so costs scale with usage
- **−** Recipes are separate projects of varying maturity; the README disclaims maintenance and security fixes
- **−** No release tags and no shared template; each recipe sets up its own stack

<sub>TypeScript · Needs TinyFish API key, TinyFish hosted Search/Fetch/Agent/Browser API, Vercel (for demos), n8n (for workflows) · [Repo](https://github.com/tinyfish-io/tinyfish-cookbook) · [▶️ Demo ↗](https://cookbook-viet-bike-scout.vercel.app/) · [📖 Docs ↗](https://docs.tinyfish.ai/) · [🌐 Site ↗](https://tinyfish.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tinyfish-cookbook/)</sub>

<a name="openai-cua-sample-app"></a>
### #&#8288;49 [openai-cua-sample-app](https://github.com/openai/openai-cua-sample-app) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (44) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Reference computer-use agents using Playwright (JS) and PyAutoGUI (Python).**

Two sample computer-use agents built on the OpenAI Responses API. The JavaScript agent writes code against Playwright to drive a browser; the Python agent uses PyAutoGUI to control a real desktop through screenshots, mouse and keystrokes. Both share a web console and three fake labs (kanban, paint, booking) for testing, plus SDK examples using ComputerToolset.

- **+** Two implementations of the same loop, in TypeScript and Python, for direct comparison
- **+** Bundled labs (kanban, paint, booking) with Replay JSON and a screenshot timeline per run
- **+** SDK examples run in a headless Chromium context with outbound page requests blocked
- **+** Persistent worker keeps state between model calls, reducing round trips
- **−** No OS sandbox: generated code runs with your user permissions
- **−** Python agent controls your real mouse and keyboard; crashes can leave input held
- **−** Requires an OpenAI API key and paid calls; no other model providers documented
- **−** Sample code, not a production runtime; lacks OpenAI's action-review controls

<sub>TypeScript, OpenAI models via Responses API · Needs OpenAI API key, Node.js 22.20.0, pnpm 10.26.0, Playwright, uv (Python app), Python 3.10+ (Python app) · env example file · [Repo](https://github.com/openai/openai-cua-sample-app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-cua-sample-app/)</sub>

<a name="opentag"></a>
### #&#8288;50 [OpenTag](https://github.com/copilotkit/opentag) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (32) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Nov 2026</sub>

**Slack and Teams knowledge agent on LangGraph and CopilotKit Channels.**

A deployable Slack and Teams agent in two services: a Node runtime (CopilotRuntime with embedded Channels) and a Python LangGraph deep agent speaking AG-UI. It ships web research, optional GitHub, PostHog, Linear and Notion MCP tools, native Slack charts and a LangGraph interrupt that pauses before Linear or Notion writes, with Slack ingress through a CopilotKit Intelligence managed channel. For teams that want an on-call style bot in chat.

- **+** Approval gate before writes is a resumable LangGraph interrupt, not a prompt rule
- **+** Railway config and an AWS ECS Fargate deployment are both in the repo
- **+** AGENT_URL accepts any AG-UI agent; the runtime does not care about the framework
- **+** Published container images; tests and AGENTS.md included
- **−** Slack and Teams delivery depends on hosted CopilotKit Intelligence unless you build a runner
- **−** Two languages and two processes: Node 22 plus Python 3.12 with uv
- **−** OpenAI is the only documented model provider
- **−** Setup has several Slack-specific failure modes the README spends pages on

<sub>Python, openai, langgraph, ag-ui, copilotkit · Needs copilotkit-intelligence-account, openai-api-key, slack-workspace, uv · Docker · env example file · [Repo](https://github.com/copilotkit/opentag) · [📖 Docs ↗](https://docs.copilotkit.ai/channels) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opentag/)</sub>

<a name="eve-software-factory-template"></a>
### #&#8288;51 [eve-software-factory-template](https://github.com/vercel-labs/eve-software-factory-template) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (30) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Multi-agent pipeline that turns GitHub or Linear issues into reviewed draft PRs.**

Foreman is an eve-based agent pipeline that takes tasks from GitHub issues, Linear, @mentions or an HTTP intake API. It runs each through triage, research, analysis, implementation and independent review, each in its own sandbox, and opens a draft pull request on the repo set in FACTORY_REPO. Humans review and merge.

- **+** Separate sandboxed agents per stage; Reviewer sees only the pushed branch, not Implementer reasoning
- **+** Intake via GitHub label, @mention, Linear agent sessions, or HTTP API with retry-safe externalId
- **+** Restricted sandbox egress and per-command scoped tokens; no token stored inside a sandbox
- **+** Diagnoses red CI on its own PRs and pushes fixes only to factory/ branches
- **−** Tied to Vercel: Connect connectors, Blob store and eve deploy are the documented path
- **−** Setup needs a GitHub App with specific permissions plus mandatory branch protection
- **−** Install scripts are off in sandboxes by default, which can cause failing builds or tests
- **−** Works on one repository per deployment, set by FACTORY_REPO

<sub>TypeScript · Needs Vercel, Vercel Blob, GitHub App, Linear (optional), eve · GitHub template · env example file · [Repo](https://github.com/vercel-labs/eve-software-factory-template) · [📖 Docs ↗](https://ask-foreman.dev/docs) · [🌐 Site ↗](https://ask-foreman.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eve-software-factory-template/)</sub>

<a name="echo-agent"></a>
### #&#8288;52 [echo-agent](https://github.com/fuyuxiang/echo-agent) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Nov 2026</sub>

**Self-hosted Python agent runtime with layered memory and a Tauri desktop app.**

Echo Agent is a Python 3.11+ agent runtime installed from PyPI, with a terminal mode, a Gateway serving a Dashboard and HTTP/WebSocket API, and message channels. It keeps Working, Episodic, Semantic and Archival memory with BM25 plus optional vector recall, and can generate skill candidates from execution traces. The repo also ships EchoAgent Desktop, a Tauri app with an embedded Rust engine, Theia IDE and browser and computer control.

- **+** Four-tier memory with BM25 and optional vector search fused by RRF
- **+** Skill evolution gates candidates through validation, risk checks and isolated evaluation, with manual rollback
- **+** Gateway offers Dashboard, HTTP/WebSocket API, CLI/TUI, webhooks and cron triggers
- **+** Tool calls pass permission policy and approval; supports MCP, Skills and Plugins
- **−** README states current code is PolyForm Noncommercial; commercial use needs separate permission
- **−** Desktop and Runtime use different engines (Rust vs Python) with separate config, sessions and memory
- **−** Skill evolution is off by default and must be configured
- **−** Embedding the runtime is source-level only; README advises pinning versions

<sub>Python, Remote model services via API key, Model routing with fallback · Needs Python 3.11+, LLM provider API key · [Repo](https://github.com/fuyuxiang/echo-agent) · [📖 Docs ↗](https://fuyuxiang.github.io/echo-agent/) · [🌐 Site ↗](http://www.ojlab.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/echo-agent/)</sub>

<a name="golf"></a>
### #&#8288;53 [golf](https://github.com/golf-mcp/golf) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 842 · Apache-2.0 · Sep 2026</sub>

**Python framework that compiles tool, resource and prompt files into an MCP server.**

Golf builds an MCP server from a directory of Python files: each file in tools/, resources/ or prompts/ defines one component, and the component ID is derived from its path. It targets FastMCP 4.0.0 and MCP 2026-07-28, with legacy client compatibility. Authentication (JWT, OAuth server mode, static dev tokens) is configured in auth.py, and OpenTelemetry tracing is switched on through golf.json or environment variables.

- **+** File-per-component layout; tool schemas inferred from function signatures and Pydantic models
- **+** Auth options in auth.py: JWT with JWKS, OAuth 2.0 server mode, static dev tokens
- **+** Optional OpenTelemetry tracing, with a detailed_tracing flag for input/output capture
- **+** Supports streamable-http and stdio transports; targets MCP 2026-07-28 with legacy compatibility
- **−** Collects anonymous CLI usage telemetry by default; opt-out needed
- **−** v0.2.0 auth API is a breaking change from v0.1.x
- **−** Under MCP 2026-07-28, elicit and sample need InputRequiredResult return handling in tools
- **−** SSE transport is deprecated; no Docker or compose files provided

<sub>Python · Needs Python 3.10+, FastMCP 4.0.0 · [Repo](https://github.com/golf-mcp/golf) · [📖 Docs ↗](https://docs.golf.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/golf/)</sub>

<a name="azure-ai-travel-agents"></a>
### #&#8288;54 [azure-ai-travel-agents](https://github.com/azure-samples/azure-ai-travel-agents) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 483 · MIT · Nov 2026</sub>

**Travel-agency multi-agent sample using MCP servers in four languages.**

Reference app where agents extract customer preferences, recommend destinations and plan itineraries, calling tools exposed as MCP servers written in Python, Node.js, Java and .NET. Three interchangeable orchestrators are provided: LangChain.js, LlamaIndex.TS and Microsoft Agent Framework (Python). It runs locally with Docker Model Runner and Phi4 14B, or deploys to Azure Container Apps with `azd up`.

- **+** Three orchestrators (LangChain.js, LlamaIndex.TS, Microsoft Agent Framework) over the same MCP tools
- **+** MCP server examples in Python, Node.js, Java and .NET
- **+** OpenTelemetry tracing viewable in Aspire Dashboard
- **+** One-command Azure deploy with `azd up`; MIT license
- **−** Sample app, not a reusable framework; the domain is fixed to travel
- **−** Local preview needs Phi4 14B (about 7.8 GB download, 16 GB RAM minimum)
- **−** Local GPU acceleration only on Apple Silicon and NVIDIA GPUs on Windows
- **−** Deployment path is tied to Azure; no release published

<sub>TypeScript, Phi4 14B (Docker Model Runner), Azure OpenAI, Microsoft Foundry · Needs Docker, Docker Model Runner, Node.js 22+, Azure Container Apps, Azure OpenAI or Microsoft Foundry · [Repo](https://github.com/azure-samples/azure-ai-travel-agents) · [📖 Docs ↗](https://github.com/Azure-Samples/azure-ai-travel-agents/blob/main/docs/advanced-setup.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-ai-travel-agents/)</sub>

<a name="mcp-ui"></a>
### #&#8288;55 [mcp-ui](https://github.com/mcp-ui-org/mcp-ui) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (70) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · Apache-2.0 · Jul 2026</sub>

**SDK for returning interactive UI from MCP tools and rendering it in hosts.**

mcp-ui implements the MCP Apps standard for UI over MCP. Server packages (TypeScript, Ruby, Python) build `ui://` resources that tools link to via `_meta.ui.resourceUri`. The TypeScript client provides `AppRenderer` and a legacy `UIResourceRenderer`, which show the UI in a sandboxed iframe and report UI actions back to the host.

- **+** Server SDKs in TypeScript, Ruby and Python; client SDK in TypeScript
- **+** Supports both MCP Apps hosts and legacy MCP-UI hosts
- **+** Remote code runs in a sandboxed iframe
- **+** Apps SDK adapter for ChatGPT's window.openai; Web Component also available
- **−** Client renderers are TypeScript only; no native or other-language host SDKs
- **−** Several legacy hosts have partial or no UI action support
- **−** Roadmap items such as component libraries and declarative UI are unfinished
- **−** ChatGPT needs the adapter rather than working natively

<sub>TypeScript · Needs @modelcontextprotocol/ext-apps, @modelcontextprotocol/sdk · [Repo](https://github.com/mcp-ui-org/mcp-ui) · [▶️ Demo ↗](https://scira-mcp-chat-git-main-idosals-projects.vercel.app/) · [📖 Docs ↗](https://mcpui.dev/guide/server/typescript/walkthrough) · [🌐 Site ↗](https://mcpui.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-ui/)</sub>

<a name="knowledge-agent-template"></a>
### #&#8288;56 [knowledge-agent-template](https://github.com/vercel-labs/knowledge-agent-template) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Nuxt knowledge agent that greps a synced snapshot repo instead of embedding.**

A Nuxt monorepo where the agent answers by running grep, find and cat inside a pooled Vercel Sandbox holding a snapshot repo synced from GitHub repos, YouTube transcripts or custom sources by Vercel Workflow; there is no vector store. The same agent serves web chat, a GitHub bot and a Discord bot through Chat SDK adapters, with Better Auth (GitHub OAuth), an admin panel and a model router by question complexity. For teams whose docs already live in repos.

- **+** No embeddings or vector DB; retrieval is deterministic and explainable
- **+** Admin panel with usage, errors, source sync and an admin agent over internal stats
- **+** Chat, GitHub and Discord share one agent; a new platform is one adapter file
- **+** Tests included; AGENTS.md and local skills for add-source and add-tool
- **−** Built on Vercel Sandbox, Workflow and AI Gateway; self-hosting means replacing all three
- **−** Sandbox is shared and read-only; no per-user private sources
- **−** Auth is GitHub OAuth only
- **−** bun is the documented toolchain

<sub>TypeScript, ai-gateway, ai-sdk · Needs vercel-sandbox, vercel-workflow, ai-gateway-api-key, github-app · [Repo](https://github.com/vercel-labs/knowledge-agent-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/knowledge-agent-template/)</sub>

<a name="react-agent"></a>
### #&#8288;57 [react-agent](https://github.com/langchain-ai/react-agent) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 863 · MIT · Nov 2026</sub>

**Minimal Python LangGraph ReAct agent with Tavily, ready for Studio.**

A single-graph Python template: a ReAct loop in src/react_agent/graph.py that reasons, calls Tavily search, observes and repeats, with the model set by a provider/model-name string (default claude-sonnet-4-5-20250929, OpenAI as the alternative). Prompts, tools and runtime context are each one file; it opens in LangGraph Studio and deploys to LangGraph Platform. For Python developers who want the smallest LangGraph agent to extend.

- **+** Three files to change: tools.py, prompts.py, graph.py
- **+** Model switch is a provider/model string in runtime context
- **+** Unit tests in CI; Studio hot reload and time travel work out of the box
- **−** Only one tool (Tavily) and no UI; the chat surface is Studio
- **−** No persistence configuration beyond what LangGraph Platform provides
- **−** README still mentions Claude 3 Sonnet in one place; check defaults

<sub>Python, langgraph, anthropic, openai · Needs anthropic-or-openai-api-key, tavily-api-key, langgraph-cli · GitHub template · env example file · [Repo](https://github.com/langchain-ai/react-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-agent/)</sub>

<a name="data-enrichment"></a>
### #&#8288;58 [data-enrichment](https://github.com/langchain-ai/data-enrichment) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 261 · MIT · Nov 2026</sub>

**LangGraph agent that researches the web to fill your JSON schema.**

A Python LangGraph graph that takes a research topic and a JSON extraction_schema, searches with Tavily, reads pages, fills the schema and checks the result for completeness before returning. The model is a provider/model string (default claude-3-5-sonnet-20240620, OpenAI supported), and it runs in LangGraph Studio or through the LangGraph API. For teams building lead or dataset enrichment pipelines.

- **+** Schema-driven output: change the JSON schema, not the code, to extract different fields
- **+** Includes a validation step before returning results
- **+** Unit tests in CI; opens in Studio
- **−** Default model string is dated (claude-3-5-sonnet-20240620)
- **−** Tavily is the only search tool
- **−** No batch runner; one topic per invocation
- **−** No UI beyond Studio

<sub>Jupyter Notebook, langgraph, anthropic, openai · Needs anthropic-or-openai-api-key, tavily-api-key, langgraph-cli · GitHub template · env example file · [Repo](https://github.com/langchain-ai/data-enrichment) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/data-enrichment/)</sub>

<a name="react-agent-js"></a>
### #&#8288;59 [react-agent-js](https://github.com/langchain-ai/react-agent-js) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 121 · MIT · Nov 2026</sub>

**TypeScript createAgent starter with example tools and middleware hooks.**

Four TypeScript files: agent.ts builds a LangChain createAgent, tools.ts defines calculator, time, weather and knowledge-search tools, prompts.ts holds the system prompt and index.ts is a CLI runner. Middleware for summarization and human-in-the-loop is shown but not wired, the model is a string like anthropic:claude-sonnet-4-5-20250929, and it opens in LangSmith Studio. For TypeScript developers starting a LangChain v1 agent.

- **+** Tool definition pattern with Zod is the one you will reuse
- **+** Shows summarization and human-in-the-loop middleware in code
- **+** Model switch is a single string
- **−** Example tools are stubs; no real integrations
- **−** No tests, no UI, no persistence
- **−** Seed shows 117 stars; small community

<sub>TypeScript, langchain, langgraph, anthropic, openai · Needs anthropic-or-openai-api-key · GitHub template · env example file · [Repo](https://github.com/langchain-ai/react-agent-js) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-agent-js/)</sub>

<a name="output"></a>
### #&#8288;60 [output](https://github.com/growthxai/output) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 445 · Apache-2.0 · Nov 2026</sub>

**TypeScript framework for AI workflows with prompts, evals and tracing built in.**

Output is a TypeScript framework for building LLM workflows and agents on Temporal. Each workflow is a folder holding code, .prompt files (YAML frontmatter plus Liquid), evaluators and JSON traces, so a coding agent like Claude Code can read and edit it. The CLI scaffolds a project and starts Temporal, an API server and a hot-reload worker locally.

- **+** Temporal gives retries with backoff, workflow history, replay, child workflows and parallel execution
- **+** Every LLM call and HTTP request is traced to JSON under logs/runs/ with tokens and cost
- **+** One API across Anthropic, OpenAI, Azure, Vertex AI and Bedrock, with structured output and tool calling
- **+** Credentials encrypted with AES-256-GCM, scoped per environment and workflow, managed via CLI
- **−** Local dev needs Docker Desktop to run the Temporal server
- **−** Tied to Temporal's workflow and step model, which adds concepts for simple scripts
- **−** No tagged release listed, so versioning relies on the npm packages
- **−** Workflow code must keep I/O in steps; deterministic-only workflow functions constrain structure

<sub>JavaScript, Anthropic, OpenAI, Azure, Vertex AI · Needs Node.js 20+, Docker Desktop, Temporal, LLM provider API key · [Repo](https://github.com/growthxai/output) · [📖 Docs ↗](https://docs.output.ai/operations/testing) · [🌐 Site ↗](https://output.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/output/)</sub>

<a name="marketing-team-eve-template"></a>
### #&#8288;61 [marketing-team-eve-template](https://github.com/vercel-labs/marketing-team-eve-template) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 457 · MIT · Nov 2026</sub>

**Slack-driven team of marketing agents built on eve, with approval gates.**

A TypeScript template on the eve agent framework: a lead agent routes requests to five specialists (product marketer, content marketer, social media, SEO, email). Output goes to Notion pages, Typefully drafts and Resend campaigns. Irreversible actions such as sending emails or scheduling posts wait for approval in Slack or the terminal.

- **+** Approval prompts before email sends, scheduled publishes, deletes and Notion page edits
- **+** Email specialist limited to 47 of Resend's roughly 85 tools
- **+** Notion and Resend authorized per person, so the agent acts with their permissions
- **+** Offline mock-model evals run in seconds without model calls
- **−** Tied to Vercel services: Connect, Blob, AI Gateway, Sandbox and OIDC
- **−** Needs Notion, Resend, Typefully and Slack accounts to be useful
- **−** Cannot create or verify Resend domains or segments; set those up first
- **−** Slack surface only runs against a deployment, not locally

<sub>TypeScript, Vercel AI Gateway models · Needs Vercel Connect, Vercel Blob, Vercel AI Gateway, Vercel Sandbox, Slack, Notion, Resend, Typefully, Node 24.x · GitHub template · [Repo](https://github.com/vercel-labs/marketing-team-eve-template) · [📖 Docs ↗](https://vercel.com/docs/frameworks/agents/eve) · [🌐 Site ↗](https://eve.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/marketing-team-eve-template/)</sub>

<a name="mcp-for-next-js"></a>
### #&#8288;62 [mcp-for-next.js](https://github.com/vercel-labs/mcp-for-next.js) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 375 · MIT · Oct 2026</sub>

**Stateless MCP server route for a Next.js App Router app.**

Next.js App Router project where app/mcp/route.ts hosts a stateless MCP server through mcp-handler 2 and the MCP TypeScript SDK v2, serving the 2026-07-28 protocol natively with a compatibility layer for 2025-era Streamable HTTP clients. Includes a sample client script that lists tools and calls echo. For teams adding an MCP endpoint to an existing Next.js app on Vercel; no auth is wired.

- **+** Stateless Streamable HTTP; no Redis or session store required
- **+** Current 2026-07-28 protocol plus 2025 Streamable HTTP compatibility
- **+** Sample client script for smoke-testing the endpoint
- **−** No auth; remote MCP clients will need OAuth added
- **−** Deprecated HTTP+SSE transport is not supported
- **−** Only an echo tool; the README is a few lines
- **−** No tests or Docker

<sub>JavaScript, MCP TypeScript SDK v2, mcp-handler 2 · [Repo](https://github.com/vercel-labs/mcp-for-next.js) · [🌐 Site ↗](https://vercel.com/templates/next.js/model-context-protocol-mcp-with-next-js) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-for-next-js/)</sub>

<a name="opengap"></a>
### #&#8288;63 [opengap](https://github.com/open-gitagent/opengap) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: popular (56) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Jul 2026</sub>

**Git-repo file standard and CLI for defining portable AI agents.**

OpenGAP defines an agent as a git repo: agent.yaml and SOUL.md are required, with optional RULES.md, DUTIES.md, skills/, tools/, workflows/, memory/ and sub-agents. The opengap CLI (npm, Node >= 18) validates the definition against a spec and exports it to targets such as Claude Code, OpenAI Agents SDK, CrewAI, Gemini CLI, Cursor and plain system prompts. It also covers financial compliance checks (FINRA, SR 11-7) and segregation-of-duties validation.

- **+** Exports one agent definition to about 15 targets, including Claude Code, OpenAI, CrewAI, Cursor and Gemini
- **+** Only two required files, so a minimal agent is agent.yaml plus SOUL.md
- **+** validate --compliance checks segregation-of-duties conflicts before deployment
- **+** Agent history, diffs, branches and tags come from plain git
- **−** Spec is v0.1.0, so the format may still change
- **−** Ports only identity layer; orchestration, tool execution and memory I/O stay in the framework
- **−** Compliance features are aimed at US financial regulation, with little else covered
- **−** Package was renamed twice (gitagent, gapman, opengap), which complicates searching docs and installs

<sub>TypeScript, Claude, OpenAI, Gemini, GitHub Models · Needs Node.js >= 18, git · [Repo](https://github.com/open-gitagent/opengap) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opengap/)</sub>

<a name="new-langgraphjs-project"></a>
### #&#8288;64 [new-langgraphjs-project](https://github.com/langchain-ai/new-langgraphjs-project) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 78 · MIT · Nov 2026</sub>

**Empty TypeScript LangGraph.js scaffold with message history and tests.**

The TypeScript counterpart of the blank LangGraph template: src/agent/graph.ts keeps a message history and returns a placeholder reply, with langgraph.json, .env.example and unit plus integration test workflows. It runs with npx @langchain/langgraph-cli dev and needs no API keys until you add a model. For TypeScript developers who want the LangGraph Platform layout without an opinionated agent.

- **+** Runs with zero secrets; add a model when ready
- **+** Unit and integration test workflows included
- **+** Studio-ready langgraph.json
- **−** Returns a placeholder until you add an LLM call
- **−** No UI, no tools
- **−** Seed shows 75 stars; the Python twin sees more activity

<sub>TypeScript, langgraph · Needs langgraph-cli · GitHub template · env example file · [Repo](https://github.com/langchain-ai/new-langgraphjs-project) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/new-langgraphjs-project/)</sub>

<a name="code-mode"></a>
### #&#8288;65 [code-mode](https://github.com/universal-tool-calling-protocol/code-mode) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: known (40) · Freshness: active (85) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MPL-2.0 · Aug 2026</sub>

**TypeScript library that lets an LLM call many tools through one code-execution tool.**

Exposes registered MCP, HTTP, file and CLI tools as TypeScript namespaces inside a Node.js VM, so a model writes one code block that chains calls and returns only a summary. Ships as the @utcp/code-mode npm package, a `utcp` CLI for shell-capable agents, and an MCP server for clients like Claude Desktop. Includes tool search, generated TypeScript interfaces, log capture and a 30-second default timeout.

- **+** Chains many tool calls in one execution and filters data in-sandbox before returning it
- **+** Mixes MCP, HTTP, file and CLI tool sources in a single code block
- **+** Three entry points: npm library, shell CLI, and MCP server for MCP-only clients
- **+** Configurable timeout and captured console logs returned with each result
- **−** Sandbox is Node.js VM contexts, not a separate container or process
- **−** Each protocol needs its own plugin package, such as @utcp/mcp
- **−** Cost-savings figures come from a third-party Python benchmark with two small models
- **−** Last tagged release is 2025-11-23; no hosted demo or dedicated docs site listed

<sub>TypeScript, unknown · Needs Node.js, @utcp/mcp, @utcp/http, UTCP client · [Repo](https://github.com/universal-tool-calling-protocol/code-mode) · [🌐 Site ↗](https://utcp.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/code-mode/)</sub>

<a name="ralph-loop-agent"></a>
### #&#8288;66 [ralph-loop-agent](https://github.com/vercel-labs/ralph-loop-agent) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 848 · Apache-2.0 · Sep 2026</sub>

**TypeScript library that reruns an AI SDK agent until a completion check passes.**

ralph-loop-agent wraps the Vercel AI SDK's generateText in an outer loop that calls a user-supplied verifyCompletion function after each pass. If verification fails, its reason string is injected into the next iteration. Stop conditions cap iterations, tokens or estimated cost. The repo includes a CLI example using Vercel Sandbox, Playwright, PostgreSQL and GitHub PRs, and the README marks the package as experimental.

- **+** Combinable stop conditions: iterationCountIs, tokenCountIs and costIs, stopping when any one triggers
- **+** Failed verification reasons are fed back into the next iteration as feedback
- **+** Works with AI SDK tools and AI Gateway model strings
- **+** Built-in context summarization and streaming of the final iteration
- **−** Marked experimental; the README warns APIs may change between versions
- **−** You must write verifyCompletion yourself; no default check is provided
- **−** Streaming runs earlier iterations non-streaming, so output only appears on the final pass
- **−** No tagged release is listed on the repository

<sub>TypeScript, Any AI SDK LanguageModel via AI Gateway strings (e.g. anthropic/claude-opus-4.5) · Needs ai (Vercel AI SDK), zod, AI Gateway or a model provider · [Repo](https://github.com/vercel-labs/ralph-loop-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph-loop-agent/)</sub>

<a name="new-langgraph-project"></a>
### #&#8288;67 [new-langgraph-project](https://github.com/langchain-ai/new-langgraph-project) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: patchy (35) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 301 · MIT · Nov 2026</sub>

**Blank Python LangGraph scaffold with config, tests and Studio support.**

The blank-slate LangGraph template: src/agent/graph.py holds a one-node graph that returns a fixed string and its runtime context, with langgraph.json, a .env.example and unit plus integration test workflows already in place. Start it with langgraph dev and open it in Studio; there is no model, no tools and no UI. For Python developers who want the LangGraph Platform layout without an opinionated agent.

- **+** Correct langgraph.json, package layout and CI from the first commit
- **+** No model dependency; add the provider you want
- **+** Unit and integration test workflows included
- **−** Does nothing until you add a model call and nodes
- **−** No chat UI; Studio or the API is the interface
- **−** Assumes LangGraph Server and Platform as the runtime

<sub>Python, langgraph · Needs langgraph-cli · env example file · [Repo](https://github.com/langchain-ai/new-langgraph-project) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/new-langgraph-project/)</sub>

<a name="template-mcp-server"></a>
### #&#8288;68 [template-mcp-server](https://github.com/redhat-data-and-ai/template-mcp-server) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 71 · Apache-2.0 · Oct 2026</sub>

**Python FastMCP server template with example tools and OAuth.**

A Python template for building MCP servers on FastMCP and FastAPI, with three example tools: a multiply calculator, a code review prompt generator and a Red Hat logo tool. It supports HTTP, SSE and streamable-HTTP transports, optional SSL, structlog JSON logging and Pydantic configuration from environment variables. It also ships a Containerfile, compose file, OpenShift manifests and GitHub Actions workflows.

- **+** Transport selectable with one env var: http, sse or streamable-http
- **+** Includes UBI-based Containerfile, compose file, OpenShift manifests and CI workflows
- **+** Optional OAuth with PostgreSQL token storage already wired in
- **+** Rename checklist and a five-minute first-tool tutorial
- **−** ENABLE_AUTH is False in .env.example but True in code; skipping .env enables auth
- **−** Example tools are trivial, so all real tool logic is yours to write
- **−** Renaming package, Makefile, manifests and workflows is a manual checklist
- **−** Defaults assume Red Hat conventions such as UBI images and OpenShift

<sub>Python · Needs Python 3.12+, PostgreSQL (OAuth token storage) · GitHub template · Docker · env example file · [Repo](https://github.com/redhat-data-and-ai/template-mcp-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/template-mcp-server/)</sub>

<a name="deer-workflow"></a>
### #&#8288;69 [deer-workflow](https://github.com/deerwork-ai/deer-workflow) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (13) · Freshness: active (97) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 561 · MIT · Aug 2026</sub>

**TypeScript runtime that runs coding agents as nodes in workflow graphs.**

deer-workflow is a Bun-based CLI and library where TypeScript modules define the execution paths and coding agents (Codex CLI by default, Claude Code and Pi built in) do the work inside each node. `deer-workflow create` generates a workflow module from a prompt using a bundled skill, and `deer-workflow run` executes it with a phase-aware TUI or a JSONL event stream via `--print`. It is described as a pilot for DeerFlow 3.0.

- **+** Control flow and failure handling live in reviewable TypeScript, not an agent conversation
- **+** Built-in Codex, Claude Code and Pi harnesses behind a vendor-neutral Agent interface
- **+** `--print` streams one JSON event per line for CI and pipelines
- **+** Generates runnable workflow modules from a prompt; includes deep-research and blog-writer examples
- **−** Requires Bun and an installed, signed-in coding agent such as Codex CLI
- **−** Described as a pilot project; API stability is unknown
- **−** Examples only run from a cloned repository, not the npm install
- **−** No Docker image or web UI; terminal TUI and JSONL only

<sub>TypeScript, Codex CLI, Claude Code, Pi · Needs Bun, Codex CLI, Claude Code (optional), Pi (optional) · [Repo](https://github.com/deerwork-ai/deer-workflow) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deer-workflow/)</sub>

<a name="cloudflare-agents-starter"></a>
### #&#8288;70 [agents-starter](https://github.com/cloudflare/agents-starter) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: known (34) · Freshness: active (89) · Maintenance: weak (8) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Jul 2026</sub>

**Cloudflare Agents SDK chat starter with Durable Object state and scheduling.**

A chat agent on Cloudflare Workers using the Agents SDK AIChatAgent class: streaming via Workers AI by default, three tool patterns (server auto-execute, client-side, human approval), one-off and cron scheduling, image input and a Kumo React UI. Messages persist in Durable Object SQLite, streams resume on reconnect, and swapping to OpenAI or Anthropic is an AI SDK provider import. For teams deploying agents on Cloudflare.

- **+** No model API key needed; Workers AI is the default
- **+** Approval, client-side and server tools shown side by side in server.ts
- **+** Built-in scheduling, MCP client and state sync from the Agents SDK
- **+** npm run deploy ships to workers.dev
- **−** Local dev still needs a Cloudflare login; Workers AI has no local simulator
- **−** Demo tools return fake data (getWeather is random)
- **−** No auth, no tests
- **−** State model is Durable Objects; not portable off Cloudflare

<sub>TypeScript, workers-ai, ai-sdk, openai, anthropic · Needs cloudflare-account, wrangler · [Repo](https://github.com/cloudflare/agents-starter) · [📖 Docs ↗](https://developers.cloudflare.com/agents/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloudflare-agents-starter/)</sub>

<a name="danghuangshang"></a>
### #&#8288;71 [danghuangshang](https://github.com/wanikua/danghuangshang) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: popular (53) · Freshness: recent (70) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · May 2026</sub>

**Multi-agent team on OpenClaw, modeled on Ming ministries, run from Discord.**

Installer and config templates that set up 14 to 18 role-based agents (dispatcher, prompt refiner, six ministries, code reviewer) on the OpenClaw framework. You @mention an agent in Discord or Feishu and tasks route through the hierarchy. Three org presets (Ming, Tang, modern CEO) can be switched by script. A React dashboard on port 18795 and a Hermes Agent runtime option are included.

- **+** Three org presets switchable with scripts/switch-regime.sh, each agent with its own memory
- **+** Supports Anthropic, OpenAI, Gemini and DeepSeek; models can differ per agent
- **+** Memory backup script uses sqlite3 .backup with daily, weekly and monthly retention
- **+** Multi-arch Docker image (amd64, arm64) plus local, remote and lite install scripts
- **−** Depends on the OpenClaw framework; not usable standalone
- **−** Discord multi-bot setup needs allowBots set to mentions or bots loop
- **−** Main README is Chinese; English and Japanese versions are separate files
- **−** Install relies on curl-piped shell scripts; README advises a cloud server

<sub>TypeScript, Anthropic, OpenAI, Gemini, DeepSeek · Needs OpenClaw, Discord bot token or Feishu app, LLM API key, Docker (optional), Notion (optional) · Docker · [Repo](https://github.com/wanikua/danghuangshang) · [📖 Docs ↗](https://github.com/wanikua/danghuangshang/blob/main/docs/README.md) · [🌐 Site ↗](https://danghuangshang.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/danghuangshang/)</sub>

<a name="assistant-ui-stockbroker"></a>
### #&#8288;72 [assistant-ui-stockbroker](https://github.com/assistant-ui/assistant-ui-stockbroker) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 284 · MIT · Nov 2026</sub>

**assistant-ui frontend and LangGraph.js stockbroker agent with approval steps.**

A Turborepo with a Next.js 16 frontend on assistant-ui and a LangGraph.js backend defining a stockbroker graph that calls GPT-4o, Financial Datasets and Tavily, with human-in-the-loop approval before trades. The frontend proxies to the LangGraph dev server (port 2024) with an optional LangSmith key, three API keys are needed, and there is no auth beyond LangGraph threads. For teams pairing assistant-ui with LangGraph.js.

- **+** Shows assistant-ui wired to a LangGraph.js graph with interrupts
- **+** Frontend and backend start together with pnpm dev
- **+** Biome lint and format configured
- **−** Three keyed services: OpenAI, Financial Datasets, Tavily
- **−** No tests, no auth
- **−** Demo domain; trading tools are not real brokers
- **−** Seed shows 281 stars

<sub>TypeScript, openai, langgraph, assistant-ui · Needs openai-api-key, financial-datasets-api-key, tavily-api-key · [Repo](https://github.com/assistant-ui/assistant-ui-stockbroker) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/assistant-ui-stockbroker/)</sub>

<a name="mcp-agent"></a>
### #&#8288;73 [mcp-agent](https://github.com/lastmile-ai/mcp-agent) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: popular (80) · Freshness: quiet (17) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · Apache-2.0 · Jan 2026</sub>

**Python framework for building MCP-connected agents with composable workflow patterns.**

mcp-agent is a Python library that connects LLMs to MCP servers and manages server connection lifecycles. It implements the patterns from Anthropic's Building Effective Agents (parallel, orchestrator, router, evaluator-optimizer) as composable workflows. Execution runs on asyncio by default, or on Temporal for durable, resumable runs without API changes.

- **+** Implements MCP tools, resources, prompts, OAuth, sampling, elicitation and roots
- **+** Same decorators run on asyncio or Temporal for durable execution
- **+** Agents can be exposed as MCP servers with a FastMCP-compatible API
- **+** CLI scaffolds projects via uvx mcp-agent init
- **−** Last release was 2025-05-09, well behind recent commits
- **−** Durable mode requires running a Temporal backend
- **−** Managed cloud deploy (mcp-c) is labeled beta
- **−** No Docker or compose files detected in the repo

<sub>Python, OpenAI, Anthropic, Google, Azure · Needs Temporal (optional, durable execution), MCP servers (e.g. uvx, npx), LLM provider API key · [Repo](https://github.com/lastmile-ai/mcp-agent) · [📖 Docs ↗](https://docs.mcp-agent.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-agent/)</sub>

<a name="openai-apps-sdk-examples"></a>
### #&#8288;74 [openai-apps-sdk-examples](https://github.com/openai/openai-apps-sdk-examples) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (51) · Freshness: recent (53) · Maintenance: weak (1) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Apr 2026</sub>

**Example MCP servers and widgets for ChatGPT apps on the Apps SDK.**

pnpm workspace with React widget sources, a Vite build that emits hashed HTML/JS/CSS bundles served on port 4444, and paired MCP servers in Node and Python (Pizzaz, kitchen-sink-lite, solar system, shopping cart, an OAuth-gated example). Widgets use the window.openai host API and _meta.ui.resourceUri to render inside ChatGPT. For developers building ChatGPT apps; test via developer mode and an ngrok tunnel.

- **+** Node and Python MCP servers for the same widgets
- **+** kitchen-sink-lite covers the full window.openai host API surface
- **+** Shopping-cart example shows widgetSessionId state across tool calls
- **+** Authenticated server demonstrates OAuth-gated tools
- **−** Examples only; no persistence or deploy config beyond BASE_URL
- **−** Requires ChatGPT developer mode and a public tunnel to test
- **−** Chrome 142+ needs a flag change to render widgets locally
- **−** Maintainers may not review all PRs

<sub>TypeScript, OpenAI Apps SDK, MCP TypeScript SDK, MCP Python SDK · Needs ChatGPT developer mode, ngrok or a public host for testing · [Repo](https://github.com/openai/openai-apps-sdk-examples) · [📖 Docs ↗](https://developers.openai.com/apps-sdk) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-apps-sdk-examples/)</sub>

<a name="agno-agent-ui"></a>
### #&#8288;75 [agent-ui](https://github.com/agno-agi/agent-ui) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: known (43) · Freshness: recent (61) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · May 2026</sub>

**Next.js chat frontend for Agno AgentOS with tool calls and reasoning.**

A Next.js and shadcn/ui chat interface that connects to a running Agno AgentOS instance (default localhost:7777) and renders streamed replies, tool calls with results, reasoning steps, references and image, video or audio content. Auth is a bearer token set via NEXT_PUBLIC_OS_SECURITY_KEY or the sidebar; the main branch targets Agno v2 and a v1 branch remains. For Agno users who need a frontend without writing one.

- **+** Scaffolds with npx create-agent-ui; endpoint and token editable in the UI
- **+** Renders reasoning steps, references and multimodal outputs, not only text
- **+** Separate branch kept for Agno v1
- **−** Only speaks to AgentOS; no use outside the Agno stack
- **−** Token is exposed as NEXT_PUBLIC and stored client-side
- **−** No tests, no persistence of its own
- **−** Last commit 2026-05

<sub>TypeScript, agno · Needs agno-agentos · GitHub template · [Repo](https://github.com/agno-agi/agent-ui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agno-agent-ui/)</sub>

<a name="mcp-framework"></a>
### #&#8288;76 [mcp-framework](https://github.com/quantgeekdev/mcp-framework) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (23) · Freshness: recent (64) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 931 · MIT · Apr 2026</sub>

**TypeScript framework for building MCP servers with directory-based tool discovery.**

MCP Framework is a TypeScript library and CLI for writing Model Context Protocol servers on top of the official MCP SDK. Tools, resources and prompts are classes auto-discovered from directories, with Zod schemas providing input types and validation. It supports stdio, SSE and HTTP Stream transports, with JWT, API key and OAuth 2.1 auth providers.

- **+** CLI scaffolds projects and adds tools, prompts and resources (mcp create, mcp add tool)
- **+** Three transports: stdio, SSE and HTTP Stream with sessions and optional resumability
- **+** Built-in JWT, API key and OAuth 2.1 auth, with JWKS validation or token introspection
- **+** Zod schemas give inferred input types; build and startup reject fields without descriptions
- **−** README labels the HTTP transport experimental and its CLI flag sets CORS origin to *
- **−** Auth providers are documented for SSE and HTTP Stream endpoints only, not stdio
- **−** TypeScript and Node only; no other language support
- **−** No Docker or compose files provided for deployment

<sub>TypeScript · Needs Node.js, npm, zod, @modelcontextprotocol/sdk · [Repo](https://github.com/quantgeekdev/mcp-framework) · [📖 Docs ↗](https://mcp-framework.com) · [🌐 Site ↗](https://mcp-framework.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-framework/)</sub>

<a name="kimi-agent-sdk"></a>
### #&#8288;77 [kimi-agent-sdk](https://github.com/moonshotai/kimi-agent-sdk) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (13) · Freshness: recent (69) · Maintenance: weak (8) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 583 · Apache-2.0 · May 2026</sub>

**Go, Node.js and Python clients that drive the Kimi CLI agent runtime.**

Kimi Agent SDK provides thin Go, Node.js and Python libraries that wrap the Kimi Code CLI as the execution engine. They reuse the CLI's configuration, tools, skills and MCP servers, stream responses, surface tool calls and approval requests, and let you register custom tools. Examples include a Go loop agent and Python custom tools and KAOS sandbox backends (BoxLite, E2B, Sprites).

- **+** Packages for Go, Node.js and Python with matching scope
- **+** Reuses existing Kimi CLI config, skills and MCP servers
- **+** Custom tools and programmatic approval handling supported
- **+** Python examples run agent tools in BoxLite, E2B or Sprites
- **−** Requires the Kimi CLI as the execution engine
- **−** No tagged release on the repository
- **−** Top-level README is brief; API details live in per-language guides
- **−** Tied to the Kimi CLI; other providers not mentioned

<sub>TypeScript, Kimi · Needs Kimi CLI (Kimi Code) · [Repo](https://github.com/moonshotai/kimi-agent-sdk) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kimi-agent-sdk/)</sub>

<a name="openai-cs-agents-demo"></a>
### #&#8288;78 [openai-cs-agents-demo](https://github.com/openai/openai-cs-agents-demo) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: popular (76) · Freshness: quiet (8) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Dec 2025</sub>

**Airline support multi-agent demo with visible handoffs and guardrails.**

A Python backend on the OpenAI Agents SDK that routes airline support requests between six agents (triage, flight info, booking, seats, FAQ, refunds) with relevance and jailbreak guardrails, plus a Next.js UI on ChatKit that shows each handoff and guardrail trip as it happens. Data is mock itineraries, tools are in-process functions, and there is no auth or persistence. For teams evaluating the Agents SDK handoff pattern.

- **+** Orchestration view makes handoffs and guardrail trips visible per message
- **+** Six agents and two guardrails in one readable backend
- **+** npm run dev starts both UI (3000) and backend (8000)
- **−** Demo data only; mock flights and bookings
- **−** No auth, persistence, tests or Docker
- **−** OpenAI Agents SDK and ChatKit only
- **−** Last commit 2025-12

<sub>Python, openai, openai-agents-sdk, chatkit · Needs openai-api-key · [Repo](https://github.com/openai/openai-cs-agents-demo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-cs-agents-demo/)</sub>

<a name="claude-managed-agents"></a>
### #&#8288;79 [claude-managed-agents](https://github.com/cloudflare/claude-managed-agents) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (6) · Freshness: recent (67) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 336 · MIT · May 2026</sub>

**Self-hosted control plane running Claude Managed Agents on Cloudflare Workers.**

A Cloudflare Workers control plane that receives Claude Managed Agents webhooks and starts a sandbox per session, either a Cloudflare Container or an Isolate sandbox. It adds egress policies with credential injection, Workers VPC access to private services, and built-in tools for email, browser automation and image generation. A dashboard and API are deployed to your own account. The README labels it alpha software meant as a starting point to fork.

- **+** Two sandbox backends: full containers or lightweight isolates, chosen per agent
- **+** Egress policies inject credentials so the agent never sees secrets
- **+** Custom tools declared in one file with direct access to Worker bindings
- **+** Private services reachable through Workers VPC without public exposure
- **−** README calls it alpha software: not stable, may contain bugs
- **−** Requires a paid Cloudflare Workers plan or Enterprise account
- **−** Dashboard is unsecured by default until Cloudflare Access is configured
- **−** Tied to Claude Managed Agents and Anthropic keys; no other model providers

<sub>TypeScript, Claude (Anthropic) · Needs Cloudflare Workers Paid plan, Cloudflare D1, Cloudflare KV, Cloudflare R2, Durable Objects, Anthropic API, Docker (terminal deploy) · Docker · [Repo](https://github.com/cloudflare/claude-managed-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-managed-agents/)</sub>

<a name="nanoagent"></a>
### #&#8288;80 [nanoagent](https://github.com/sanbuphy/nanoagent) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: niche (17) · Freshness: slowing (41) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 785 · MIT · Mar 2026</sub>

**Single-file Python agent loop with bash, read and write tools.**

nanoAgent is a roughly 100-line Python script that runs an OpenAI function-calling loop with three tools: execute_bash, read_file and write_file. It takes a task as a command-line argument and iterates until the model stops calling tools. Malformed JSON arguments and unknown tool names are returned to the model as tool errors instead of crashing the loop.

- **+** Whole agent is about 100 lines, easy to read and modify
- **+** Base URL and model set by env vars, so OpenAI-compatible endpoints work
- **+** Tool-call errors are fed back to the model rather than crashing
- **+** MIT license and a single pip requirements file
- **−** Runs arbitrary bash commands with no sandbox or confirmation step
- **−** Only three tools; no MCP support in this repo
- **−** CLI one-shot only: no UI, memory or conversation persistence documented
- **−** Uses the OpenAI chat completions API; other provider formats are not documented

<sub>Python, OpenAI function-calling models (default example gpt-4o-mini) · Needs OpenAI-compatible API key · [Repo](https://github.com/sanbuphy/nanoagent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nanoagent/)</sub>

<a name="mcp-forge"></a>
### #&#8288;81 [mcp-forge](https://github.com/achetronic/mcp-forge) <sub>score [16](../README.md#-how-we-rank "Score 16/100. Adoption: niche (2) · Freshness: quiet (20) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 99 · Apache-2.0 · Jan 2026</sub>

**Go MCP server template with OAuth discovery and JWT validation.**

Go 1.24+ template on mcp-go that runs as an HTTP or stdio MCP server from a YAML config, with RFC 8414 and 9728 OAuth discovery endpoints and JWT validation either delegated to a proxy like Istio or done locally via JWKS and CEL claim rules. Ships a Dockerfile, Helm chart, GitHub Actions and example configs for Claude Web, OpenAI and local clients through mcp-remote. You add tools under internal/tools.

- **+** OAuth discovery endpoints and JWT middleware for remote clients like Claude Web
- **+** Helm chart, Dockerfile and CI workflows included
- **+** Same binary serves HTTP or stdio by swapping the YAML config
- **+** Access logs can redact or drop fields
- **−** Needs an external OIDC provider with dynamic client registration (Keycloak suggested)
- **−** Author recommends a proxy for JWT validation and a hashring router for sessions
- **−** Last commit 2026-01; no tests mentioned in the README

<sub>Go, mcp-go · Needs OIDC provider (e.g. Keycloak), Kubernetes for the Helm chart (optional) · GitHub template · Docker · [Repo](https://github.com/achetronic/mcp-forge) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcp-forge/)</sub>

<a name="stockbot-on-groq"></a>
### #&#8288;82 [stockbot-on-groq](https://github.com/bklieger-groq/stockbot-on-groq) <sub>score [14](../README.md#-how-we-rank "Score 14/100. Adoption: known (36) · Freshness: quiet (10) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Dec 2025</sub>

**Groq chatbot answering with TradingView widgets via AI SDK generative UI.**

A Next.js chatbot forked from the Vercel AI Chatbot template where Llama 3 70B on Groq picks a tool and the UI renders a TradingView widget: price charts, financials, news, market overview, screeners, heatmaps and trending lists. Two sequential model calls produce the tool choice and the reply, one secret (GROQ_API_KEY) runs it, and there is no auth or persistence. For developers who want a worked example of tool-driven generative UI.

- **+** Nine widget types show the tool-to-component mapping end to end
- **+** Hosted demo at groq-stockbot.vercel.app
- **+** Single env var to run
- **−** Groq-only; model pinned to Llama 3 70B in prompts
- **−** Widgets are TradingView embeds, not your own data
- **−** No auth, history or tests
- **−** Last commit 2025-12

<sub>TypeScript, groq, ai-sdk · Needs groq-api-key · env example file · [Repo](https://github.com/bklieger-groq/stockbot-on-groq) · [▶️ Demo ↗](https://groq-stockbot.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/stockbot-on-groq/)</sub>

<a name="openai-structured-outputs-samples"></a>
### #&#8288;83 [openai-structured-outputs-samples](https://github.com/openai/openai-structured-outputs-samples) <sub>score [7](../README.md#-how-we-rank "Score 7/100. Adoption: niche (15) · Freshness: quiet (9) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 689 · MIT · Dec 2025</sub>

**Three Next.js samples driving UI from schema-constrained OpenAI outputs.**

Three small Next.js apps, each with its own README: resume extraction renders structured fields from a model response, generative UI builds components from a JSON-schema output, and conversational assistant combines multi-turn chat, tool calling and generative UI in one flow. All rely on OpenAI Structured Outputs so responses always match the schema. For developers deciding how to bind model JSON to React components.

- **+** Conversational assistant sample is a reasonable base for a schema-driven assistant
- **+** Each sample is independent; copy one folder
- **+** Shows the schema-to-component pattern without a framework
- **−** Root README has no setup; per-folder READMEs only
- **−** OpenAI-only
- **−** No auth, persistence or tests
- **−** Last commit 2025-12

<sub>TypeScript, openai · Needs openai-api-key · [Repo](https://github.com/openai/openai-structured-outputs-samples) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-structured-outputs-samples/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
