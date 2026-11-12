# 🏗️ App builder starters reviews · Best of Vibe Coding

Prompt-to-app builders and platforms that run coding agents in sandboxes. Back to the [leaderboard](../README.md#%EF%B8%8F-app-builder-starters).

<sub>🌐 Also on the web: [App builder starters on archestack.com](https://archestack.com/best-of-vibe-coding/app-builders/), each project on its own page.</sub>

<a name="jeecgboot"></a>
### 🥇 [jeecgboot](https://github.com/jeecgboot/jeecgboot) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · Apache-2.0 · Nov 2026</sub>

**Java and Vue3 low-code platform with built-in AI apps and knowledge base.**

JeecgBoot is a Spring Boot 4 and Vue3 base for enterprise business systems, with RBAC, multi-tenancy, Flowable workflows, report and dashboard designers, and a CRUD code generator. It also includes an AI app platform with model management, a RAG knowledge base, flow orchestration, MCP and chat, built on langchain4j. Claude Code skills can generate modules, forms and BPMN flows from a prompt.

- **+** Code generator emits Java, Vue3, table SQL and menu permissions for single, tree and one-to-many models
- **+** Button, row and field-level permissions plus multi-tenancy are built in
- **+** Supports MySQL, Oracle, PostgreSQL, SQL Server, MariaDB, Dameng and Kingbase; monolith or Spring Cloud
- **+** Official live demo and a separate Claude Code skills repository
- **−** Java-only backend; README says it suits non-Java teams and small tools poorly
- **−** Needs MySQL, Redis, Maven and pnpm; microservice mode adds Nacos and more
- **−** Only MySQL scripts ship by default; other databases need manual conversion
- **−** Docs and community support channels are mostly Chinese, including QQ groups

<sub>Java, ChatGPT, DeepSeek, Qwen, Zhipu · Needs MySQL 5.7+, Redis, JDK 17, Maven, Node 20+, pnpm 10+, Docker Compose, Nacos (microservice mode) · [Repo](https://github.com/jeecgboot/jeecgboot) · [▶️ Demo ↗](https://boot3.jeecg.com) · [📖 Docs ↗](https://help.jeecg.com) · [🌐 Site ↗](http://www.jeecg.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jeecgboot/)</sub>

<a name="dyad"></a>
### 🥈 [dyad](https://github.com/dyad-sh/dyad) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

**Desktop app that builds apps from prompts on your own machine.**

Dyad is a local, open-source prompt-to-app builder, positioned as an alternative to Lovable, v0 and Bolt that runs on your own computer. It ships as a downloadable app for Mac and Windows and uses your own AI API keys, with no sign-up. Code outside src/pro is Apache 2.0; src/pro is under the Functional Source License 1.1.

- **+** Runs locally as a desktop app, with no sign-up needed to download
- **+** Bring your own API keys, so no hosted-platform lock-in
- **+** Mac and Windows builds available
- **+** Code outside src/pro is Apache 2.0 licensed
- **−** src/pro is fair-source (FSL 1.1), not fully open-source
- **−** No Linux build mentioned in the README
- **−** Desktop only; no Docker or self-hosted web deployment mentioned

<sub>TypeScript · Needs Your own AI provider API keys · env example file · [Repo](https://github.com/dyad-sh/dyad) · [🌐 Site ↗](https://dyad.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dyad/)</sub>

<a name="ai-website-cloner-template"></a>
### 🥉 [ai-website-cloner-template](https://github.com/jcodesmore/ai-website-cloner-template) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Nov 2026</sub>

**Agent skill that rebuilds a website from a URL as a Next.js app.**

A Next.js 16 template that ships a portable `/clone-website` agent skill. Given a URL, the agent maps routes, inspects desktop and mobile pages, extracts assets and fonts, builds React components with shadcn/ui and Tailwind v4, then compares screenshots against the source. It works with Claude Code, Codex CLI, Cursor and OpenCode.

- **+** One skill in .agents/skills is read directly by Codex, Cursor and OpenCode
- **+** Four-step flow ends with source-vs-local comparison and a list of remaining gaps
- **+** Output is editable Next.js 16, React 19, TypeScript strict, Tailwind v4 code
- **+** Includes docker compose services for production and dev-mode runs
- **−** Needs a separate coding agent with browser access; it does not run standalone
- **−** Recommended Claude Code with Opus 5.5 implies paid model usage; cost is not stated
- **−** Output quality is not quantified; gaps are reported per run by the agent
- **−** Requires Node.js 24+, which is newer than many default installs

<sub>TypeScript, Claude Code (Opus 5.5 recommended), Codex CLI, Cursor, OpenCode · Needs Node.js 24+, AI coding agent with browser access · GitHub template · Docker · [Repo](https://github.com/jcodesmore/ai-website-cloner-template) · [▶️ Demo ↗](https://youtu.be/O669pVZ_qr0) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-website-cloner-template/)</sub>

<a name="wasmer"></a>
### #&#8288;4 [wasmer](https://github.com/wasmerio/wasmer) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Nov 2026</sub>

**WebAssembly runtime and CLI for running code in sandboxes.**

Wasmer is a Rust WebAssembly runtime with a CLI that downloads packages from a registry (Python, Bash, PHP, SQLite, FFmpeg, PostgreSQL via pglite) and runs them in sandboxes. File, network and environment access are opt-in, for example via --volume and --net. Alpha SDKs for JavaScript, Python, Rust and Swift, kept in a separate repo, embed sandboxes in apps and agents.

- **+** File, network and environment access is denied unless granted with flags such as --volume and --net
- **+** Runs Python, Bash, PHP, SQLite and FFmpeg from a registry without installing them on the host
- **+** Same sandbox API across JavaScript, Python, Rust and Swift, including iOS and browser
- **+** MIT licensed, with a Rust API and C API for lower-level WebAssembly embedding
- **−** The sandbox SDK is alpha and lives in a separate repository
- **−** Rust SDK is a source dependency; crates.io publishing is currently disabled
- **−** Browser execution needs cross-origin isolation headers on the page
- **−** Not an agent framework or app builder; it provides only the sandbox layer

<sub>Rust · [Repo](https://github.com/wasmerio/wasmer) · [▶️ Demo ↗](https://wasmer.sh) · [📖 Docs ↗](https://docs.wasmer.io) · [🌐 Site ↗](https://wasmer.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wasmer/)</sub>

<a name="e2b"></a>
### #&#8288;5 [e2b](https://github.com/e2b-dev/e2b) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**SDKs for running AI-generated code in isolated cloud sandboxes.**

E2B provides JavaScript and Python SDKs that start isolated cloud sandboxes and run shell commands inside them. Companion packages add a Code Interpreter (runCode/run_code) and a Desktop SDK for mouse, keyboard and screenshot control. The runtime can be self-hosted with Terraform on AWS, GCP, Azure or a generic Linux machine; the hosted service needs an API key.

- **+** Official JavaScript/TypeScript and Python SDKs with a matching sandbox API
- **+** Separate Code Interpreter and Desktop SDKs cover code execution and computer use
- **+** Self-hosting supported on AWS, GCP, Azure and generic Linux via Terraform
- **+** Apache-2.0 license; cookbook repo has examples for several LLMs and frameworks
- **−** Hosted use requires an E2B account and API key
- **−** Self-hosted runtime lives in a separate repo, e2b-dev/runtime
- **−** README gives no resource requirements, pricing or sandbox limits
- **−** Provides sandboxes only; agent logic and LLM integration are left to you

<sub>Python · Needs E2B API key (hosted), Terraform (self-hosting) · Docker · [Repo](https://github.com/e2b-dev/e2b) · [📖 Docs ↗](https://e2b.dev/docs) · [🌐 Site ↗](https://e2b.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/e2b/)</sub>

<a name="appsmith"></a>
### #&#8288;6 [appsmith](https://github.com/appsmithorg/appsmith) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · Apache-2.0 · Nov 2026</sub>

**Low-code builder for internal dashboards and admin panels on your own data.**

Appsmith is a low-code platform for building internal tools such as dashboards, admin panels and customer 360 views, then deploying and maintaining them. It can be self-hosted or used through Appsmith Cloud. The README also promotes a separate product, Appsmith Agents, which adds AI models over private data; its availability and licensing in this repo are not stated.

- **+** Self-host via Docker, Kubernetes or AWS AMI, with a hosted Cloud option
- **+** Apache-2.0 licensed, TypeScript codebase with frequent releases (latest 2026-10-21)
- **+** Documentation, tutorials and templates are linked from the README
- **+** Targets internal tools like admin panels and dashboards rather than generic apps
- **−** Not a prompt-to-app builder; AI features sit in the separate Agents product
- **−** Appsmith Agents is only described as a product pitch; open-source status unclear
- **−** No docker-compose file detected in the repo

<sub>TypeScript · Docker · env example file · [Repo](https://github.com/appsmithorg/appsmith) · [📖 Docs ↗](https://docs.appsmith.com) · [🌐 Site ↗](https://www.appsmith.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/appsmith/)</sub>

<a name="lowdefy"></a>
### #&#8288;7 [lowdefy](https://github.com/lowdefy/lowdefy) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

**YAML-config framework for building internal web apps and admin tools.**

Lowdefy builds web apps from YAML config instead of hand-written React. Pages are composed from 70+ UI blocks and 50+ logic operators, with connectors for MongoDB, PostgreSQL, MySQL, REST, Google Sheets, S3, Elasticsearch and Stripe. The runtime is built on Hono, Vite and Auth.js and extends through npm plugins. The README pitches the config as a reviewable target for AI-generated apps.

- **+** Schema-validated config is interpreted, not executed, so there are no arbitrary code paths
- **+** Ships 70+ UI blocks and 10+ data connectors including MongoDB, PostgreSQL and Stripe
- **+** Auth.js integration with 75+ auth providers, role-based access control and private pages
- **+** Plugin system for blocks, connections, operators, actions and auth providers via npm
- **−** No built-in LLM features; the AI role is only generating config for you
- **−** Logic lives in YAML operators, which gets awkward for complex behavior
- **−** Custom UI beyond the provided blocks requires writing npm plugins
- **−** README promotes the maintainer's paid app-building service alongside the project

<sub>JavaScript · Needs Node.js · [Repo](https://github.com/lowdefy/lowdefy) · [📖 Docs ↗](https://docs.lowdefy.com) · [🌐 Site ↗](https://lowdefy.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lowdefy/)</sub>

<a name="vibesdk"></a>
### #&#8288;8 [vibesdk](https://github.com/cloudflare/vibesdk) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (47) · Freshness: active (92) · Maintenance: fair (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Oct 2026</sub>

**Self-hosted prompt-to-app platform on Cloudflare Workers and Durable Objects.**

Bun and Vite project that runs a coding agent (Cloudflare Think) in a Durable Object per project, keeps files in a SpaceDO workspace, stores git history in Cloudflare Artifacts, loads previews as Dynamic Workers and gives each generated app SQLite via Durable Object Facets. Models route through AI Gateway; D1 holds platform data. Needs a Workers Paid plan, Workers for Platforms and a custom domain with wildcard DNS.

- **+** Previews load as Dynamic Workers; no long-running dev server
- **+** Restore points and rollback via Cloudflare Artifacts
- **+** bun run setup provisions resources, AI Gateway, auth and migrations
- **+** Bash is disabled in the agent; tool boundaries are explicit
- **−** Requires Workers Paid plan, Workers for Platforms and wildcard DNS for previews
- **−** Entirely Cloudflare-specific; nothing is portable to other hosts
- **−** Feature toggles live in the dashboard, not in wrangler.jsonc
- **−** Long setup guide with several API token permissions to get right

<sub>TypeScript, Cloudflare AI Gateway (configured providers) · Needs Cloudflare account with Workers Paid plan, Cloudflare AI Gateway, D1, model provider API key, custom domain with wildcard DNS · [Repo](https://github.com/cloudflare/vibesdk) · [▶️ Demo ↗](https://build.cloudflare.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibesdk/)</sub>

<a name="magic"></a>
### #&#8288;9 [magic](https://github.com/polterguy/magic) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Self-hosted backend generator that builds secured APIs and apps from plain English.**

Magic Cloudlet is a .NET 10 backend with a React dashboard. It generates database CRUD endpoints, auth, role-based access and frontend files from natural-language prompts, in a language called Hyperlambda. Every endpoint in the modules folder can be exposed as an MCP tool through the mcp plugin, and it also includes OpenAPI import, a chatbot wizard and a sandbox endpoint for caller-supplied code.

- **+** Generates secured CRUD APIs over MySQL, PostgreSQL, SQL Server or MariaDB schemas
- **+** Built-in MCP server turns each endpoint into a tool for Claude, Cursor or Codex
- **+** Saved code runs immediately, with no build or deploy step
- **+** MIT license; Docker Compose setup with ports 4444 (API) and 5555 (dashboard)
- **−** Apps are written in Hyperlambda, a niche language, so skills and code do not carry over
- **−** Code generator is the author's proprietary LLM, not an open model
- **−** Defaults to OpenAI; semantic retrieval still needs OpenAI embeddings even with Ollama
- **−** Default login is root/root; the benchmark is single-machine and not independently replicated

<sub>C#, OpenAI, Ollama, HuggingFace · Needs OpenAI API key (default), Docker Compose, SQLite · README: alternative to Cursor, Lovable, Replit · [Repo](https://github.com/polterguy/magic) · [📖 Docs ↗](https://docs.ainiro.io/getting-started/) · [🌐 Site ↗](https://hyperlambda.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/magic/)</sub>

<a name="runtime"></a>
### #&#8288;10 [runtime](https://github.com/e2b-dev/runtime) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · Apache-2.0 · Nov 2026</sub>

**Firecracker microVM sandbox backend for running untrusted AI agent code.**

Go backend behind E2B Cloud: a REST API, a per-node orchestrator that drives Firecracker, an in-VM agent (envd), an edge proxy and a template builder. Each sandbox is a microVM restored from a snapshot with lazy memory paging, and it can be paused, resumed or forked. A single-host Embed package runs the stack on a Linux machine with KVM.

- **+** Hardware isolation per sandbox: own microVM, cgroup, network namespace and nftables egress rules
- **+** Pause, resume and fork of live sandboxes, with up to 100 forks per request
- **+** Templates built from Docker images with hashed, cached layers
- **+** Single-host Embed package, plus Terraform for GCP, AWS and Azure and a Kubernetes manifest
- **−** Requires a Linux host with KVM; no macOS or Windows host support
- **−** Needs PostgreSQL, Redis, ClickHouse and object storage, so it is heavy to operate
- **−** Embed is limited to one machine; multi-node production is a paid enterprise deployment
- **−** Architecture is complex; the README tells readers to study the architecture doc first

<sub>Go · Needs Linux with KVM, Firecracker, PostgreSQL, Redis, ClickHouse, Object storage, Docker Compose (Embed) · [Repo](https://github.com/e2b-dev/runtime) · [📖 Docs ↗](https://docs.e2b.dev/) · [🌐 Site ↗](https://e2b.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/runtime/)</sub>

<a name="llamacoder"></a>
### #&#8288;11 [llamacoder](https://github.com/nutlope/llamacoder) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.2k · MIT · Oct 2026</sub>

**Next.js app that turns one prompt into a small React app.**

Llama Coder sends a text prompt to Llama 3.1 405B through Together AI and renders the generated app in a sandboxed iframe using esbuild-wasm and esm.sh. It is a Next.js app router project with Tailwind, Prisma on PostgreSQL, and optional screenshot uploads to S3.

- **+** In-browser preview via esbuild-wasm and esm.sh in a sandboxed iframe
- **+** MIT license, plain Next.js and Tailwind codebase that is easy to fork
- **+** Optional Braintrust observability and screenshot uploads
- **−** Requires a Together AI API key; no other LLM providers documented
- **−** Needs a PostgreSQL database (Neon suggested) even for local runs
- **−** Screenshot uploads need S3 credentials and a bucket lifecycle rule
- **−** No Docker setup or release; run from source with npm

<sub>TypeScript, Llama 3.1 405B · Needs Together AI API, PostgreSQL (Neon), Prisma, S3 bucket (screenshot uploads), Braintrust (optional), esm.sh · [Repo](https://github.com/nutlope/llamacoder) · [▶️ Demo ↗](https://www.llamacoder.io) · [🌐 Site ↗](https://www.llamacoder.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llamacoder/)</sub>

<a name="open-lovable"></a>
### #&#8288;12 [open-lovable](https://github.com/firecrawl/open-lovable) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: weak (15) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

**Chat-driven React app builder that clones sites via Firecrawl and runs code in sandboxes.**

Next.js app where you describe a React app in chat and an LLM generates and edits the code inside a remote sandbox (Vercel Sandbox by default, or E2B). It uses the Firecrawl API to scrape existing sites as reference material. The LLM can be Gemini, Anthropic, OpenAI or Groq, with optional Morph for faster edit application.

- **+** Supports four LLM providers: Gemini, Anthropic, OpenAI and Groq, chosen via env keys
- **+** Sandbox backend is switchable between Vercel Sandbox and E2B with one variable
- **+** Setup is clone, install, set .env.local, run pnpm dev on port 3000
- **+** MIT licensed
- **−** Requires a Firecrawl API key; it is listed as required
- **−** Needs a Vercel or E2B account for sandboxes; no local sandbox option documented
- **−** Described as an example app; no docs on deployment, auth or persistence
- **−** No Dockerfile or compose file, and no tagged releases

<sub>TypeScript, Gemini, Anthropic, OpenAI, Groq · Needs Firecrawl API, Vercel Sandbox or E2B, Morph (optional) · env example file · [Repo](https://github.com/firecrawl/open-lovable) · [🌐 Site ↗](https://firecrawl.dev/?ref=open-lovable-github) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-lovable/)</sub>

<a name="fragments"></a>
### #&#8288;13 [fragments](https://github.com/e2b-dev/fragments) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Oct 2026</sub>

**Open-source Claude Artifacts alternative that runs AI-generated apps in sandboxes.**

Next.js 14 app that takes a chat prompt, has an LLM generate code, and runs it in an E2B cloud sandbox with a live preview. Built-in stacks are Python interpreter, Next.js, Vue.js, Streamlit and Gradio, and more can be added as E2B sandbox templates. It supports OpenAI, Anthropic, Google AI, Mistral, Groq, Fireworks, Together AI and Ollama.

- **+** Adds stacks via an E2B Dockerfile plus an entry in lib/templates.json
- **+** Eight LLM providers including Ollama; custom models and providers are config edits
- **+** Generated code runs in E2B sandboxes, with npm and pip packages installable
- **+** Optional Morph Apply model for faster code edits
- **−** Requires an E2B API key; sandbox execution is not self-hosted in this setup
- **−** No Dockerfile or compose file; README documents only npm run dev and build
- **−** No tagged releases
- **−** README lists Next.js 14, which may lag current Next.js

<sub>TypeScript, OpenAI, Anthropic, Google AI, Google Vertex · Needs E2B API key, LLM provider API key, Supabase (optional, auth), Vercel/Upstash KV (optional), PostHog (optional), Morph API key (optional) · env example file · [Repo](https://github.com/e2b-dev/fragments) · [▶️ Demo ↗](https://fragments.e2b.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fragments/)</sub>

<a name="monkeycode"></a>
### #&#8288;14 [monkeycode](https://github.com/chaitin/monkeycode) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (44) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · AGPL-3.0 · Nov 2026</sub>

**AI development platform that runs coding tasks in server-side environments.**

MonkeyCode is a web platform where AI agents carry out development tasks inside server-side environments, with build, test and preview done remotely. It adds model management, task management, requirement/SPEC management and automated PR/MR review for engineering teams. It can be used online or installed inside a private network with an install script.

- **+** Runs tasks in server-side dev environments, no local setup needed
- **+** Integrates GLM, Kimi, MiniMax, Qwen and DeepSeek, switchable per task
- **+** Includes requirement/SPEC management, team collaboration and PR/MR review
- **+** Private deployment possible; source is auditable under AGPL-3.0
- **−** No local IDE, local CLI or code completion, per its own comparison table
- **−** Self-hosting needs a dev environment host of at least 8C/16 GB/100 GB
- **−** Install is a curl-piped script; no Docker or Compose files detected
- **−** AGPL-3.0 adds source-disclosure obligations for network use

<sub>TypeScript, GLM, Kimi, MiniMax, Qwen · [Repo](https://github.com/chaitin/monkeycode) · [▶️ Demo ↗](https://monkeycode-ai.net/) · [📖 Docs ↗](https://monkeycode.docs.baizhi.cloud/) · [🌐 Site ↗](https://monkeycode-ai.net/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/monkeycode/)</sub>

<a name="codesandbox-client"></a>
### #&#8288;15 [codesandbox-client](https://github.com/codesandbox/codesandbox-client) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (70) · Freshness: recent (70) · Maintenance: weak (15) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · custom license · Sep 2026</sub>

**Browser-based online IDE client for web development and prototyping.**

The web client of CodeSandbox, an online IDE for creating, running and sharing web projects from a browser. The repository holds only the client; the Phoenix API server and Nginx config live elsewhere, and the README describes no AI features. Last release was 2024-08-26 and the license is reported as NOASSERTION.

- **+** Full IDE for web projects that runs in a browser on any device
- **+** Documentation is published on the CodeSandbox website
- **+** Git Extractor and CLI are open source in a separate repository
- **−** Client only; the Phoenix API server is not in this repository
- **−** License is not identified (NOASSERTION)
- **−** README mentions no AI or prompt-to-app features
- **−** Last tagged release dates from 2024-08-26

<sub>JavaScript · Needs Phoenix API server, Nginx · Docker · ⚠️ .env file committed · [Repo](https://github.com/codesandbox/codesandbox-client) · [📖 Docs ↗](https://codesandbox.io/docs/learn/introduction/overview) · [🌐 Site ↗](https://codesandbox.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codesandbox-client/)</sub>

<a name="tkinter-designer"></a>
### #&#8288;16 [tkinter-designer](https://github.com/parthjadhav/tkinter-designer) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: popular (64) · Freshness: recent (70) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · BSD-3-Clause · Oct 2026</sub>

**Generates Tkinter GUI code from Figma designs via the Figma API.**

Tkinter Designer is a Python CLI, installed with `pip install tkdesigner`, that reads a Figma file through the Figma API and writes a Tkinter `gui.py` plus the image assets it needs. It takes a Figma URL and API token, and supports a class-based template, a multi-frame pages template with Back/Next navigation, and ttk themes. It is deterministic design-to-code conversion, not an LLM tool.

- **+** Installs with pip; CLI takes a Figma URL and token
- **+** Multi-frame apps with Back/Next navigation via --template pages
- **+** Generated gui.py imports without starting mainloop, so you can regenerate the UI later
- **+** Offers class-based output and ttk themes
- **−** Requires a Figma account, API token and network access to the Figma API
- **−** Generates UI layout only; event logic must be written separately
- **−** Last release was January 2023, so the PyPI package may lag the repo
- **−** Output depends on how the Figma design is structured

<sub>Python · Needs Python 3.9+, Figma API token, Figma · Docker · [Repo](https://github.com/parthjadhav/tkinter-designer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tkinter-designer/)</sub>

<a name="open-agents"></a>
### #&#8288;17 [open-agents](https://github.com/vercel-labs/open-agents) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: popular (50) · Freshness: recent (74) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Jun 2026</sub>

**Reference app for background coding agents on Vercel sandboxes.**

pnpm monorepo (web app, agent, sandbox and shared packages) where a Next.js app with Better Auth (Vercel and GitHub OAuth) starts durable Workflow SDK runs that drive an agent with file, shell, search and web tools against isolated Vercel sandboxes with snapshot resume. Needs Postgres and a GitHub App for clone, push and PRs; Redis and ElevenLabs voice are optional. For teams forking a hosted coding agent on Vercel.

- **+** Agent runs as a durable workflow outside the sandbox, resumable by reconnecting
- **+** GitHub App integration for repo access, auto-commit, push and PR
- **+** Better Auth with Vercel and GitHub providers wired
- **+** pnpm run ci covers lint, typecheck, tests and migration check
- **−** Tied to Vercel Sandbox and Workflow SDK; not portable off Vercel
- **−** Setup needs a Vercel OAuth app, a GitHub App and six GitHub env vars
- **−** Model provider configuration is not described in the README

<sub>TypeScript · Needs PostgreSQL (Neon), Vercel Sandbox, Vercel OAuth app, GitHub App, Redis (optional), ElevenLabs (optional) · [Repo](https://github.com/vercel-labs/open-agents) · [▶️ Demo ↗](https://open-agents.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-agents/)</sub>

<a name="lealone"></a>
### #&#8288;18 [lealone](https://github.com/lealone/lealone) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (24) · Freshness: recent (70) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · custom license · Oct 2026</sub>

**Java database and service runtime with a built-in LLM agent for prompt-to-app.**

Lealone is a Java project that runs from a single jar and exposes an agent mode. In that mode, a prompt such as "implement a todo app" returns a URL for the generated app. It also lets you declare services, tables and workflows in SQL-like statements (create service, create workflow) and serves them over HTTP on port 8080. LLM providers are Doubao and DeepSeek.

- **+** Run with one jar via java -jar; no Docker or external database step in the README
- **+** Services, tables and workflows declared in SQL-like syntax and callable as HTTP URLs
- **+** Agent mode generates a runnable app from one prompt in about 20 seconds
- **−** Only Doubao and DeepSeek are supported as LLM providers
- **−** README is Chinese only and gives no architecture or API reference
- **−** Only an 8.0.0-SNAPSHOT jar is offered; last tagged release is from 2024
- **−** License is not a recognized SPDX type (NOASSERTION); terms must be read in LICENSE.md

<sub>Java, doubao, deepseek · Needs JDK 21+, Maven (to build), Doubao or DeepSeek API key · [Repo](https://github.com/lealone/lealone) · [🌐 Site ↗](https://lealone-plugins.github.io/lealone.github.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lealone/)</sub>

<a name="chef"></a>
### #&#8288;19 [chef](https://github.com/convex/chef) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: known (39) · Freshness: slowing (40) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Mar 2026</sub>

**Prompt-to-app builder that generates full-stack web apps on a Convex backend.**

Chef is a fork of the bolt.diy stable branch that generates web apps backed by Convex, giving them a database, auth, file uploads, real-time queries and background workflows. The agent loop in `chef-agent/` injects a system prompt, defines tools and calls Anthropic, Google, OpenAI or xAI models. It can run locally, but sign-in depends on Convex's hosted control plane and an OAuth app.

- **+** Generated apps get database, auth, file storage and workflows from Convex without extra config
- **+** System prompt is published with each release, so the agent behavior can be inspected
- **+** Supports Anthropic, Google, OpenAI and xAI keys, set in .env.local or the settings page
- **+** Includes a test harness (test-kitchen) for the agent loop and a CLI (chefshot)
- **−** Auth is tied to Convex's internal control plane; forks for production must replace it
- **−** Local setup needs a Convex account, an OAuth app and several environment variables
- **−** Locked to Convex as the backend; no other database or backend option
- **−** Must be opened at 127.0.0.1; localhost does not work; no Docker setup provided

<sub>TypeScript, Anthropic, Google, OpenAI, xAI · Needs Convex (hosted control plane), Convex OAuth application, WorkOS client ID, Node.js via nvm, pnpm · sign-in: WorkOS · [Repo](https://github.com/convex/chef) · [▶️ Demo ↗](https://chef.convex.dev) · [📖 Docs ↗](https://docs.convex.dev/chef) · [🌐 Site ↗](https://chef.convex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chef/)</sub>

<a name="claudable"></a>
### #&#8288;20 [claudable](https://github.com/anymorph-ai/claudable) <sub>score [22](../README.md#-how-we-rank "Score 22/100. Adoption: known (35) · Freshness: slowing (37) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Mar 2026</sub>

**Local Next.js app builder that drives Claude Code, Codex or Cursor CLI.**

Claudable is a Next.js web app that wraps locally installed coding-agent CLIs (Claude Code, Codex CLI, Cursor CLI, Qwen Code, Z.AI GLM-4.6) behind a prompt-to-app interface with live preview. It generates Next.js code with Tailwind and shadcn/ui, and connects to GitHub, Vercel and Supabase using tokens you enter in settings. State is stored in a local SQLite file, and an Electron desktop build is available.

- **+** Supports five agent CLIs, so you reuse an existing Claude, ChatGPT or Cursor login
- **+** Local SQLite database at data/cc.db, no separate database server needed
- **+** Built-in GitHub, Vercel and Supabase integrations for deploy and Postgres
- **+** Electron packaging scripts for macOS, Windows and Linux
- **−** Requires a separately installed and logged-in agent CLI, which may carry its own subscription cost
- **−** No Docker or compose files; setup is clone, npm install and npm run dev
- **−** Native MCP, checkpoints and subagents are listed as upcoming, not shipped
- **−** Last tagged release is 2025-08-30; README references the opactorai/Claudable repo

<sub>TypeScript, Claude Code (Claude Opus 4.6), Codex CLI (GPT-5), Cursor CLI, Qwen Code (Qwen3-Coder) · Needs Node.js 18+, Git, Claude Code, Codex CLI, Cursor CLI, Qwen Code or Z.AI GLM agent, SQLite, GitHub, Vercel, Supabase · [Repo](https://github.com/anymorph-ai/claudable) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claudable/)</sub>

<a name="coding-agent-template"></a>
### #&#8288;21 [coding-agent-template](https://github.com/vercel-labs/coding-agent-template) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: niche (14) · Freshness: slowing (33) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · Apache-2.0 · Feb 2026</sub>

**Run Claude Code, Codex and other coding CLIs in Vercel Sandbox.**

Next.js 15 app with Drizzle on Postgres that lets signed-in users (GitHub or Vercel OAuth) submit a repo URL and a task, runs Claude Code, Codex CLI, Copilot CLI, Cursor CLI, Gemini CLI or opencode in a Vercel Sandbox, and commits to an AI-named branch. Per-user API keys and tokens are encrypted at rest; MCP servers can be attached for Claude Code. Needs Vercel sandbox credentials, JWE_SECRET and ENCRYPTION_KEY.

- **+** Six coding agents selectable per task
- **+** Per-user OAuth, GitHub tokens and API keys encrypted at rest
- **+** Sandbox timeout (5 min to 5 h) and keep-alive for follow-ups
- **+** One-click Vercel deploy provisions Neon Postgres
- **−** Vercel Sandbox only; needs a Vercel token, team and project id
- **−** Default MAX_MESSAGES_PER_DAY is 5 per user
- **−** v2.0.0 broke v1 deployments; migration guide required
- **−** No tests mentioned; last commit 2026-02

<sub>TypeScript, Claude Code, OpenAI Codex CLI, GitHub Copilot CLI, Cursor CLI · Needs PostgreSQL (Neon), Vercel Sandbox credentials, GitHub or Vercel OAuth app, agent API keys (Anthropic, OpenAI, Cursor, Gemini, AI Gateway) · GitHub template · [Repo](https://github.com/vercel-labs/coding-agent-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coding-agent-template/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
