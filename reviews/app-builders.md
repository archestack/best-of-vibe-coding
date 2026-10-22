# 🏗️ App builder starters reviews · Best of Vibe Coding

Prompt-to-app builders and platforms that run coding agents in sandboxes. Back to the [leaderboard](../README.md#%EF%B8%8F-app-builder-starters).

<sub>🌐 Also on the web: [App builder starters on archestack.com](https://archestack.com/best-of-vibe-coding/app-builders/), each project on its own page.</sub>

<a name="ai-website-cloner-template"></a>
### 🥇 [ai-website-cloner-template](https://github.com/jcodesmore/ai-website-cloner-template) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (100) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · MIT · Oct 2026</sub>

**Next.js template with an agent skill that rebuilds a website from its URL.**

A Next.js 16 template (React 19, Tailwind CSS v4, shadcn/ui) that bundles a portable `clone-website` agent skill. Given a URL, the agent maps routes, inspects desktop and mobile pages, extracts assets and fonts, builds editable components, then compares source and local pages and runs `npm run check`. It works with Claude Code, Codex CLI, Cursor and OpenCode.

- **+** Same skill is read by Claude Code, Codex CLI, Cursor and OpenCode
- **+** Output is a typed Next.js codebase with extracted assets, not a screenshot
- **+** Writes route mappings, comparison screenshots and a list of remaining gaps
- **+** MIT license; Docker Compose files for app and dev mode (port 3001)
- **−** Needs a separate AI coding agent with browser access; no standalone mode
- **−** README recommends Claude Code with Opus 5.5; other agents are only listed as supported
- **−** Requires Node.js 24+
- **−** Output is Next.js only; no other target framework is mentioned

<sub>TypeScript, Claude Code (Opus 5.5 recommended), Codex CLI, Cursor, OpenCode · Needs Node.js 24+, AI coding agent with browser access · GitHub template · Docker · [Repo](https://github.com/jcodesmore/ai-website-cloner-template) · [▶️ Demo ↗](https://youtu.be/O669pVZ_qr0) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-website-cloner-template/)</sub>

<a name="jeecgboot"></a>
### 🥈 [jeecgboot](https://github.com/jeecgboot/jeecgboot) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: hard (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · Apache-2.0 · Oct 2026</sub>

**Java low-code platform with code generator and built-in AI app builder.**

JeecgBoot is a Spring Boot 4 and Vue3 platform for building enterprise systems such as OA, ERP and CRM. It pairs an online form builder and code generator with an AI module (model management, knowledge base with RAG, flow orchestration, MCP plugins, chat assistant) built on langchain4j. It runs as a monolith or as Spring Cloud Alibaba microservices.

- **+** Code generator emits front end, back end, table SQL and menu permissions
- **+** Switches between monolith and Spring Cloud Alibaba microservices (Nacos, Gateway, Sentinel)
- **+** Row, column and form-field level data permissions plus multi-tenant SaaS support
- **+** Supports MySQL, PostgreSQL, Oracle, SQL Server, MariaDB, Dameng, Kingbase and TiDB
- **−** Only MySQL scripts ship by default; other databases need manual conversion
- **−** README and docs are primarily in Chinese, with English and Japanese variants linked
- **−** Large stack: needs Redis and a database, and microservice mode adds Nacos and more
- **−** AI features are one module in a broad platform, not a standalone AI app server

<sub>Java, ChatGPT, DeepSeek, Qwen, Zhipu · Needs MySQL 5.7+, Redis, Nacos (microservice mode), MinIO or Aliyun OSS (optional) · [Repo](https://github.com/jeecgboot/jeecgboot) · [▶️ Demo ↗](https://boot3.jeecg.com) · [📖 Docs ↗](https://help.jeecg.com) · [🌐 Site ↗](http://www.jeecg.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jeecgboot/)</sub>

<a name="dyad"></a>
### 🥉 [dyad](https://github.com/dyad-sh/dyad) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (88) · Easy to run: hard (17) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Oct 2026</sub>

**Desktop app that builds apps from prompts on your own machine.**

Dyad is a local, open-source prompt-to-app builder, positioned as an alternative to Lovable, v0 and Bolt that runs on your own computer. It ships as a downloadable app for Mac and Windows and uses your own AI API keys, with no sign-up. Code outside src/pro is Apache 2.0; src/pro is under the Functional Source License 1.1.

- **+** Runs locally as a desktop app, with no sign-up needed to download
- **+** Bring your own API keys, so no hosted-platform lock-in
- **+** Mac and Windows builds available
- **+** Code outside src/pro is Apache 2.0 licensed
- **−** src/pro is fair-source (FSL 1.1), not fully open-source
- **−** README does not list supported models or providers
- **−** No Linux build mentioned in the README
- **−** Desktop only; no Docker or self-hosted web deployment mentioned

<sub>TypeScript · Needs Your own AI provider API keys · env example file · [Repo](https://github.com/dyad-sh/dyad) · [🌐 Site ↗](https://dyad.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dyad/)</sub>

<a name="e2b"></a>
### #&#8288;4 [e2b](https://github.com/e2b-dev/e2b) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (82) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Oct 2026</sub>

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

<a name="llamacoder"></a>
### #&#8288;5 [llamacoder](https://github.com/nutlope/llamacoder) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: patchy (33) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Oct 2026</sub>

**Open-source Claude Artifacts clone generating React apps with Llama.**

Next.js App Router app with Tailwind that sends a prompt to Llama 3.1 405B on Together AI and renders the generated React app in a sandboxed iframe using esbuild-wasm and esm.sh. Needs TOGETHER_API_KEY, a Postgres DATABASE_URL via Prisma (Neon suggested) and S3 credentials for screenshot uploads; Braintrust tracing is optional. For developers building a prompt-to-app demo on open models.

- **+** In-browser preview via esbuild-wasm and esm.sh; no server sandbox cost
- **+** Prisma and Postgres persistence for generated apps
- **+** Braintrust observability wired as an optional env var
- **+** Live deployment at llamacoder.io shows the finished product
- **−** Together AI only; no provider abstraction
- **−** Screenshot upload requires five S3-related env vars
- **−** No auth or rate limiting described
- **−** No .env.example

<sub>TypeScript, Together AI (Llama 3.1 405B) · Needs Together AI API key, PostgreSQL (Neon), S3 bucket for screenshots, Braintrust (optional) · [Repo](https://github.com/nutlope/llamacoder) · [▶️ Demo ↗](https://www.llamacoder.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/llamacoder/)</sub>

<a name="vibesdk"></a>
### #&#8288;6 [vibesdk](https://github.com/cloudflare/vibesdk) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: known (44) · Freshness: active (94) · Maintenance: fair (56) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="monkeycode"></a>
### #&#8288;7 [monkeycode](https://github.com/chaitin/monkeycode) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (51) · Easy to run: hard (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · AGPL-3.0 · Oct 2026</sub>

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

<a name="open-lovable"></a>
### #&#8288;8 [open-lovable](https://github.com/firecrawl/open-lovable) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: weak (16) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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
### #&#8288;9 [fragments](https://github.com/e2b-dev/fragments) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: patchy (40) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Oct 2026</sub>

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

<a name="open-agents"></a>
### #&#8288;10 [open-agents](https://github.com/vercel-labs/open-agents) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: known (49) · Freshness: active (82) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Jun 2026</sub>

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

<a name="coding-agent-template"></a>
### #&#8288;11 [coding-agent-template](https://github.com/vercel-labs/coding-agent-template) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (8) · Freshness: slowing (41) · Maintenance: weak (0) · Easy to run: easy (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · Apache-2.0 · Feb 2026</sub>

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

<a name="chef"></a>
### #&#8288;12 [chef](https://github.com/convex/chef) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: known (34) · Freshness: slowing (47) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Mar 2026</sub>

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
### #&#8288;13 [claudable](https://github.com/anymorph-ai/claudable) <sub>score [15](../README.md#-how-we-rank "Score 15/100. Adoption: niche (28) · Freshness: slowing (44) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Mar 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
