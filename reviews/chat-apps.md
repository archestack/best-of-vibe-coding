# 💬 Chat apps reviews · Best of Vibe Coding

Chat interfaces and single-feature text apps you fork as the base of a conversational product. Back to the [leaderboard](../README.md#-chat-apps).

<sub>🌐 Also on the web: [Chat apps on archestack.com](https://archestack.com/best-of-vibe-coding/chat-apps/), each project on its own page.</sub>

<a name="claude-quickstarts"></a>
### 🥇 [claude-quickstarts](https://github.com/anthropics/claude-quickstarts) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Nov 2026</sub>

**Claude API sample apps for agents, computer use and browser automation.**

Monorepo of reference projects for building on the Claude API. It includes a customer support agent, a financial data analyst chat, computer and browser use demos, an autonomous coding agent on the Claude Agent SDK, and Managed Agents examples (Slack, Linear, Sentry, an MCP server, scheduled briefs). Each quickstart has its own README and setup.

- **+** Maintained by Anthropic; covers current features like Managed Agents and computer_toolset_20260801
- **+** Wide range of patterns: webhook bridges, cron agents, MCP server, computer and browser use
- **+** The macOS computer-use sample shows prompt caching, image pruning, compaction and trajectory recording
- **+** MIT licensed; each quickstart is self-contained with its own README
- **−** Samples for learning, not one deployable product; some are explicitly not production code
- **−** Requires a Claude API key; examples are tied to Claude and Anthropic services
- **−** Languages and dependencies differ per quickstart, so there is no single install path
- **−** No tagged releases, so pinning a version means pinning a commit

<sub>Python, Claude · Needs Claude API key · [Repo](https://github.com/anthropics/claude-quickstarts) · [📖 Docs ↗](https://docs.claude.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-quickstarts/)</sub>

<a name="chat-js"></a>
### 🥈 [chat-js](https://github.com/franciscomoretti/chat-js) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

**Next.js AI chat app scaffold with auth, branching and sharing.**

ChatJS is a Next.js chat application generated with `npx chat-js@alpha create`, which asks for gateway, feature and auth choices and writes a `chat.config.ts`. It uses the AI SDK with Vercel AI Gateway for 120+ models, Better Auth, Drizzle on PostgreSQL, and the EVE runtime for durable conversations and approvals. Chat features include attachments, branching, public sharing, web search, image generation, code execution and MCP.

- **+** Scaffold CLI generates chat.config.ts and lists env vars for the chosen options
- **+** Covers branching, public sharing, attachments, MCP and sandboxed code execution
- **+** EVE runtime provides durable transcripts, approvals and stream recovery
- **+** Optional Electron packaging for macOS, Windows and Linux desktop apps
- **−** CLI is alpha and its APIs are still changing; no stable 1.0 yet
- **−** README says the EVE-only runtime is not yet established as production-ready
- **−** Historical ChatJS conversations are not imported into the EVE runtime
- **−** Built around Vercel AI Gateway and Blob; needs PostgreSQL and Node 24+

<sub>TypeScript, Claude, GPT, Gemini, Grok · Needs PostgreSQL, Vercel AI Gateway, Vercel Blob, EVE runtime, Node 24+, Bun · [Repo](https://github.com/franciscomoretti/chat-js) · [▶️ Demo ↗](https://demo.chatjs.dev) · [📖 Docs ↗](https://chatjs.dev/docs) · [🌐 Site ↗](https://chatjs.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chat-js/)</sub>

<a name="ant-design-x-vue"></a>
### 🥉 [ant-design-x-vue](https://github.com/wzc520pyfm/ant-design-x-vue) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Vue component library for building AI chat interfaces, port of Ant Design X.**

Vue 3 implementation of Ant Design X, a set of UI components for AI conversation pages such as Bubble, with an XProvider for configuration. It connects to OpenAI-compatible inference services and includes data stream management helpers. It is written in TypeScript and installed from npm alongside ant-design-vue.

- **+** Typed TypeScript components with fine-grained style customization
- **+** Targets OpenAI-standard inference services with built-in data stream management
- **+** Follows the upstream React Ant Design X API, easing porting between the two
- **+** MIT license with recent release and commits
- **−** Requires ant-design-vue and Vue 3.3 or newer
- **−** README is mainly in Chinese, and the English version is a separate file
- **−** Frontend components only; no backend or model serving included
- **−** Component list and templates are not detailed in the README

<sub>TypeScript, OpenAI-compatible APIs · Needs vue >=3.3, ant-design-vue · [Repo](https://github.com/wzc520pyfm/ant-design-x-vue) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ant-design-x-vue/)</sub>

<a name="chatgpt-telegram-workers"></a>
### #&#8288;4 [chatgpt-telegram-workers](https://github.com/tbxark/chatgpt-telegram-workers) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Nov 2026</sub>

**Telegram bot that proxies chat to multiple LLM providers on Cloudflare Workers.**

A TypeScript Telegram bot that forwards messages to LLM providers such as OpenAI, Anthropic, Cohere, Mistral, DeepSeek, Groq and Cloudflare AI. It runs serverless on Cloudflare Workers, with Vercel and Docker as alternatives, and stores configuration in KV. It adds streaming replies, custom commands for switching models or presets, text-to-image, plugins and a Telegram Mini App admin panel.

- **+** Supports many providers: OpenAI, Anthropic, Cohere, Mistral, DeepSeek, Groq, Cloudflare AI
- **+** Runs serverless on Cloudflare Workers; Vercel and Docker also supported
- **+** Custom commands switch models or system-prompt presets from within Telegram
- **+** Telegram Mini App admin panel and plugin system for configuration and extension
- **−** Tied to Telegram as the only chat front end
- **−** Cloudflare deployment depends on a KV namespace for configuration
- **−** Provider setup and plugin details are in separate docs, not the README
- **−** Migrating from v1 to v2 requires following a separate migration guide

<sub>TypeScript, OpenAI, Cloudflare AI, Cohere, Anthropic · Needs Telegram bot token, Cloudflare Workers KV · Docker · [Repo](https://github.com/tbxark/chatgpt-telegram-workers) · [📖 Docs ↗](https://github.com/TBXark/ChatGPT-Telegram-Workers/blob/master/doc/en/DEPLOY.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chatgpt-telegram-workers/)</sub>

<a name="vercel-chatbot"></a>
### #&#8288;5 [chatbot](https://github.com/vercel/chatbot) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: weak (29) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

**Next.js chat template with Auth.js, Postgres history and AI Gateway models.**

Clone it and you get a Next.js App Router chat app on the AI SDK with Auth.js login, chat history in Neon Postgres through Drizzle migrations, file uploads to Vercel Blob and a streaming UI on shadcn/ui. Models route through Vercel AI Gateway; Mistral, Moonshot, DeepSeek, OpenAI and xAI are preconfigured in lib/ai/models.ts. For teams starting a chat product on Vercel who want auth and persistence wired on day one.

- **+** Auth.js, Postgres chat history and Drizzle migrations wired out of the box
- **+** Live demo plus a separate docs site
- **+** Per-model provider routing in lib/ai/models.ts; swapping vendors is a small edit
- **+** Tests included
- **−** Defaults to Vercel services: AI Gateway, Neon Postgres, Vercel Blob
- **−** Off Vercel you must set AI_GATEWAY_API_KEY and replace Blob storage
- **−** No Docker or compose files

<sub>TypeScript, ai-gateway, ai-sdk, openai, mistral · Needs postgres, vercel-blob, ai-gateway-api-key · GitHub template · env example file · sign-in: Auth.js · [Repo](https://github.com/vercel/chatbot) · [▶️ Demo ↗](https://chatbot.ai-sdk.dev/demo) · [📖 Docs ↗](https://chatbot.ai-sdk.dev/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vercel-chatbot/)</sub>

<a name="boardui"></a>
### #&#8288;6 [boardui](https://github.com/boardui/boardui) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**React component library for agent UIs, installed as source via CLI.**

BoardUI is a set of 69 free React components, built on React Aria Components and Tailwind CSS v4, that `npx boardui add` copies into a Next.js project as source. It covers agent pieces (chat, thinking indicator, agent log, composer) and dashboard pieces (data table, data grid, charts, sidebar, auth cards). The repo also runs as a chat app at `/` that streams replies from a provider chosen by the API key's prefix.

- **+** Components are copied as source, so you can edit every file
- **+** One AI_API_KEY selects among 7 providers by key prefix, plus OpenAI-compatible servers
- **+** Ships an MCP server, AGENTS.md rules and llms.txt for coding agents
- **+** No database needed; chat history stays in the browser
- **−** Repo is generated from upstream source and accepts no pull requests
- **−** Free tier only; the README implies paid items exist beyond the 69 here
- **−** Chat endpoint is open to anyone with the URL, so cost depends on key limits
- **−** Install targets Next.js projects only

<sub>TypeScript, Anthropic, OpenAI, Google Gemini, OpenRouter · Needs Node.js, Next.js, LLM provider API key · env example file · [Repo](https://github.com/boardui/boardui) · [📖 Docs ↗](https://www.boardui.com/mcp) · [🌐 Site ↗](https://www.boardui.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/boardui/)</sub>

<a name="langchain-nextjs-template"></a>
### #&#8288;7 [langchain-nextjs-template](https://github.com/langchain-ai/langchain-nextjs-template) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

**Next.js routes for LangChain.js chat, agents, structured output and RAG.**

Five Next.js API routes that each show one LangChain.js pattern: plain chat, Zod structured output, a prebuilt LangGraph.js agent with Tavily search, and RAG as a chain and as an agent over a Supabase pgvector table. Tokens stream to the client through the AI SDK, routes run on Edge functions, and there is no auth or persistence beyond the vector table. For developers learning LangChain.js who want runnable routes to copy.

- **+** Each pattern is one route file you can lift into your own app
- **+** Hosted demo on Vercel
- **+** Mock-backed integration tests run without API keys or a live database
- **+** Supabase adapter reuses the documents table and match_documents function; no migration
- **−** No auth and no chat history persistence
- **−** OpenAI only out of the box; other providers need code changes
- **−** Re-ingesting the same text duplicates vectors; no dedupe
- **−** Agent and search examples need a Tavily key

<sub>TypeScript, openai, langchain, langgraph, ai-sdk · Needs openai-api-key, supabase, tavily-api-key · GitHub template · env example file · [Repo](https://github.com/langchain-ai/langchain-nextjs-template) · [▶️ Demo ↗](https://langchain-nextjs-template.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/langchain-nextjs-template/)</sub>

<a name="twitterbio"></a>
### #&#8288;8 [twitterbio](https://github.com/nutlope/twitterbio) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: known (45) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Single-form Next.js text generator streaming from Together AI.**

A one-page Next.js app: a form builds a prompt, sends it to Together AI and streams the reply back, with two open models wired (Qwen 3.5 9B with thinking off, GPT OSS 20B with a reasoning indicator). Nothing else is included: no auth, no database, no tests. For developers who want the smallest prompt-to-text starter to grow from.

- **+** One env var (TOGETHER_API_KEY) and it runs
- **+** Shows streaming for both a direct model and a reasoning model
- **+** Deployed live example at twitterbio.io
- **−** No auth, database, rate limiting or tests
- **−** Tied to Together AI; no provider layer
- **−** Single feature; most of a product is still to build

<sub>TypeScript, together · Needs together-api-key · env example file · [Repo](https://github.com/nutlope/twitterbio) · [▶️ Demo ↗](https://www.twitterbio.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/twitterbio/)</sub>

<a name="gemini-chatbot"></a>
### #&#8288;9 [gemini-chatbot](https://github.com/vercel-labs/gemini-chatbot) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (36) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Oct 2026</sub>

**Next.js chatbot template defaulting to Gemini with NextAuth and Postgres.**

An earlier cut of the Vercel chatbot template pinned to Google Gemini: Next.js App Router, AI SDK streaming with tool calls, NextAuth.js login, chat history in Vercel Postgres through Drizzle, and file storage on Vercel Blob. The default model is gemini-1.5-pro; the AI SDK lets you switch to OpenAI, Anthropic or Cohere. For teams on Google models who want the Vercel chat stack.

- **+** Auth, Postgres history and Blob uploads already wired
- **+** Two env vars to deploy: AUTH_SECRET and GOOGLE_GENERATIVE_AI_API_KEY
- **+** Deployed demo at gemini.vercel.ai
- **−** Default model gemini-1.5-pro is dated; update before shipping
- **−** Tied to Vercel Postgres and Blob; self-hosting means swapping both
- **−** No tests, no Docker
- **−** vercel/chatbot is the maintained successor for most uses

<sub>TypeScript, google, ai-sdk · Needs postgres, vercel-blob, google-api-key · GitHub template · env example file · sign-in: Auth.js · [Repo](https://github.com/vercel-labs/gemini-chatbot) · [▶️ Demo ↗](https://gemini.vercel.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-chatbot/)</sub>

<a name="nuxt-ui-chat"></a>
### #&#8288;10 [chat](https://github.com/nuxt-ui-templates/chat) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 380 · MIT · Nov 2026</sub>

**Nuxt chat app template with GitHub auth, SQLite history and AI SDK streaming.**

Nuxt application built on Nuxt UI components that streams chat responses through the Vercel AI SDK and routes models via Vercel AI Gateway. It stores chat history in SQLite through Drizzle ORM (Turso in production), signs users in with GitHub OAuth, and supports file uploads, web search, dictation, and chart and weather tool calls.

- **+** Chat history persisted via Drizzle ORM on SQLite, with Turso for production
- **+** Model access through one AI Gateway key rather than per-provider keys
- **+** Includes web search, reasoning toggle, dictation, file uploads and tool-call UI
- **+** Local blob storage by default; Vercel Blob, R2 or S3 drivers available
- **−** Auth is GitHub OAuth only; other providers need custom work with nuxt-auth-utils
- **−** File uploads only work for authenticated users
- **−** Model list and gateway setup are tied to Vercel AI Gateway
- **−** No Docker or compose files; deployment guidance centers on Vercel

<sub>Vue, Claude Haiku 5.5, Gemini 3 Flash, GPT-5.6 Luna · Needs Vercel AI Gateway, SQLite / Turso, GitHub OAuth app, NuxtHub Blob · GitHub template · env example file · [Repo](https://github.com/nuxt-ui-templates/chat) · [▶️ Demo ↗](https://chat-template.nuxt.dev/) · [📖 Docs ↗](https://ui.nuxt.com/docs/getting-started/installation/nuxt) · [🌐 Site ↗](https://ui.nuxt.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nuxt-ui-chat/)</sub>

<a name="bot-on-anything"></a>
### #&#8288;11 [bot-on-anything](https://github.com/zhayujie/bot-on-anything) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: popular (71) · Freshness: recent (57) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Jul 2026</sub>

**Python framework connecting LLMs to chat channels like Telegram, Slack, Discord.**

Bot on Anything connects a chosen model (OpenAI-compatible API, LinkAI, ERNIE Bot, New Bing, Bard) to one or more chat channels through a single config.json. Models and channels are decoupled, so any model runs on any of 12 channels, including terminal, web, Telegram, Slack, Gmail, DingTalk, Feishu, Discord and WeChat variants. Several channels can run together as separate processes.

- **+** Switch model or channel by editing the type field in config.json
- **+** 12 channels, including Slack Socket Mode that needs no public IP
- **+** Pure Python with MIT license; no database mentioned
- **+** Compatible with chatgpt-on-wechat plugins
- **−** Pinned to legacy openai SDK below 1.0.0
- **−** Last release is 2023-04-11 despite recent commits
- **−** Bing, Bard and ERNIE models rely on manually copied browser cookies
- **−** QQ channel needs a separate go-cqhttp process

<sub>Python, OpenAI-compatible API, LinkAI, ERNIE Bot, New Bing · Needs Python 3.7.1-3.10, openai<1.0.0, flask, flask_socketio, slack_bolt, pyTelegramBotAPI, werobot, go-cqhttp (QQ channel) · Docker · [Repo](https://github.com/zhayujie/bot-on-anything) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bot-on-anything/)</sub>

<a name="openai-chatkit-advanced-samples"></a>
### #&#8288;12 [openai-chatkit-advanced-samples](https://github.com/openai/openai-chatkit-advanced-samples) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: niche (13) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 672 · MIT · Aug 2026</sub>

**ChatKit feature demos with FastAPI backends and React frontends.**

Four ChatKit scenarios, each a FastAPI backend on the ChatKit Python SDK plus a React frontend: a virtual-cat caretaker, an airline support concierge, a newsroom assistant and a metro-map planner. Together they exercise server and client tools, widgets with actions, attachments, dictation, annotations, @-mentions and composer commands. For teams writing a custom ChatKit server who need a reference per feature.

- **+** Feature index maps every ChatKit capability to the file that implements it
- **+** Each demo starts with one command on its own port (5170 to 5173)
- **+** Attachment upload and dictation are implemented end to end
- **−** Samples, not a product base: no auth, persistence or tests
- **−** Python backend plus Node frontend; needs uv and npm
- **−** OpenAI-only

<sub>openai, chatkit · Needs openai-api-key, uv · [Repo](https://github.com/openai/openai-chatkit-advanced-samples) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chatkit-advanced-samples/)</sub>

<a name="ai-chat"></a>
### #&#8288;13 [ai-chat](https://github.com/pushpak1300/ai-chat) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (7) · Freshness: recent (76) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 383 · MIT · Jun 2026</sub>

**Laravel 12 chat starter streaming replies through Prism to eight providers.**

A Laravel 12 application with Inertia and Vue 3 that streams model replies over server-sent events through the Prism PHP SDK. Sanctum auth, user management, chat sharing and SQLite persistence are in place (MySQL or Postgres is a config change), and models are listed in an enum per provider: OpenAI, Anthropic, Gemini, Ollama, Groq, Mistral, DeepSeek, xAI. For Laravel teams who want a chat base in their own stack.

- **+** Installs with laravel new --using=pushpak1300/ai-chat
- **+** Auth, chat sharing and SSE streaming already wired
- **+** Adding a provider or model is one enum case
- **+** Tests included
- **−** No tool calling, multimodal input or image generation yet; all on the roadmap
- **−** README model list is dated (gpt-4o, claude-3-5); update the enum
- **−** No Docker files
- **−** PHP 8.3+ and Composer required

<sub>PHP, prism, openai, anthropic, google · Needs php-8.3, composer, sqlite-or-mysql-or-postgres, provider-api-keys · GitHub template · env example file · [Repo](https://github.com/pushpak1300/ai-chat) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-chat/)</sub>

<a name="chatgpt-android"></a>
### #&#8288;14 [chatgpt-android](https://github.com/skydoves/chatgpt-android) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: popular (67) · Freshness: quiet (10) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Jan 2026</sub>

**Android ChatGPT client sample built with Jetpack Compose and Stream Chat SDK.**

A Kotlin Android app that sends messages to the OpenAI Chat API and shows the conversation using Stream Chat SDK for Compose UI components. It follows Google's app architecture guidance (UI and data layers, Hilt, Room, WorkManager, Coroutines/Flow) and is split into modules. The README states that features other than chat are not completed.

- **+** Reference for Compose, Hilt, Room and WorkManager in a modularized Android app
- **+** Minimum SDK 21, so it covers a wide range of Android devices
- **+** Chat UI uses Stream's Compose components instead of hand-built screens
- **+** Apache-2.0 licensed
- **−** Requires a Stream account and API key, plus manual dashboard setup
- **−** Needs an OpenAI API key; README says rate limits unlock after $5 minimum spend
- **−** Only the chat feature is finished, per the README
- **−** Last release was July 2024

<sub>Kotlin, OpenAI Chat API · Needs OpenAI API key, Stream Chat account and API key, Android SDK (min API 21) · [Repo](https://github.com/skydoves/chatgpt-android) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chatgpt-android/)</sub>

<a name="openai-chatkit-starter-app"></a>
### #&#8288;15 [openai-chatkit-starter-app](https://github.com/openai/openai-chatkit-starter-app) <sub>score [20](../README.md#-how-we-rank "Score 20/100. Adoption: niche (22) · Freshness: slowing (44) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 898 · MIT · Mar 2026</sub>

**Minimal self-hosted and managed OpenAI ChatKit reference apps.**

Two reference apps for embedding OpenAI ChatKit: one self-hosted integration where you run the ChatKit backend yourself, and one managed integration that connects the widget to a hosted Agent Builder workflow. The root README is a two-line index, setup lives in each subfolder, and seed data lists Next.js plus Python. For teams committed to ChatKit who want the smallest working wiring.

- **+** Smallest ChatKit wiring published by OpenAI itself
- **+** Shows self-hosted and managed hosting modes side by side
- **−** Root README has no setup, env or port details
- **−** No auth, database, tests or Docker
- **−** Locked to OpenAI ChatKit and Agent Builder

<sub>Python, openai, chatkit · Needs openai-api-key · [Repo](https://github.com/openai/openai-chatkit-starter-app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chatkit-starter-app/)</sub>

<a name="zola"></a>
### #&#8288;16 [zola](https://github.com/ibelick/zola) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: known (41) · Freshness: quiet (6) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Dec 2025</sub>

**Multi-provider chat UI on Next.js with Ollama detection and BYOK.**

A Next.js chat interface on the AI SDK that talks to OpenAI, Mistral, Anthropic, Gemini and local Ollama models, with bring-your-own-key through OpenRouter. Supabase handles auth and file storage once you follow INSTALL.md, a docker-compose file pairs it with Ollama, and Zola is a running product (zola.chat) you fork rather than a scaffold. For builders who want a finished multi-model chat UI to brand.

- **+** Runs with one key or with local Ollama only; no database required for that path
- **+** docker-compose.ollama.yml included; auto-detects local Ollama models
- **+** Hosted instance at zola.chat shows the exact UI you get
- **−** Auth and uploads are optional extras behind Supabase setup in INSTALL.md
- **−** README marks it beta; MCP support is work in progress
- **−** No tests listed
- **−** Last commit 2025-12; check activity before forking

<sub>TypeScript, ai-sdk, openai, anthropic, google · Needs supabase, ollama, provider-api-keys · Docker · env example file · sign-in: Supabase Auth · [Repo](https://github.com/ibelick/zola) · [▶️ Demo ↗](https://zola.chat) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zola/)</sub>

<a name="langgraph-fullstack-python"></a>
### #&#8288;17 [langgraph-fullstack-python](https://github.com/langchain-ai/langgraph-fullstack-python) <sub>score [14](../README.md#-how-we-rank "Score 14/100. Adoption: niche (0) · Freshness: slowing (46) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 158 · MIT · Mar 2026</sub>

**LangGraph ReAct agent and FastHTML chat UI in one deployment.**

A Python project where langgraph.json mounts both a ReAct agent graph and a FastHTML chat page, so one langgraph dev process on port 2024 serves the UI and the agent. The model defaults to Claude 3.5 Sonnet with OpenAI as the alternative, Tavily search is the only tool, and there is no auth and no chat history persistence. For Python developers targeting LangGraph Platform who want a UI without a JavaScript build.

- **+** One process serves agent and UI; deploys as a single LangGraph app
- **+** Unit and integration test workflows run in CI
- **+** Opens directly in LangGraph Studio
- **−** No persistent chat history; the README lists it as a next step
- **−** No auth
- **−** Default model string claude-3-5-sonnet-20240620 is dated
- **−** Server-rendered FastHTML UI; limited for rich client-side features

<sub>Python, langgraph, anthropic, openai · Needs anthropic-or-openai-api-key, tavily-api-key, uv · env example file · [Repo](https://github.com/langchain-ai/langgraph-fullstack-python) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/langgraph-fullstack-python/)</sub>

<a name="openai-responses-starter-app"></a>
### #&#8288;18 [openai-responses-starter-app](https://github.com/openai/openai-responses-starter-app) <sub>score [8](../README.md#-how-we-rank "Score 8/100. Adoption: niche (18) · Freshness: quiet (7) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 884 · MIT · Dec 2025</sub>

**Next.js chat on the OpenAI Responses API with hosted tools.**

A Next.js chat UI wired to the OpenAI Responses API with streaming, multi-turn state, function calling and the hosted tools: web search, file search over a vector store you create from the UI, and code interpreter. It also configures public MCP servers and shows a Google Calendar and Gmail connector behind a browser OAuth flow; there is no auth or database. For developers building an assistant on OpenAI hosted tooling.

- **+** Web search, file search and code interpreter configurable from the UI
- **+** Working OAuth example for OpenAI first-party connectors (Calendar, Gmail)
- **+** Custom functions live in config/functions.ts; clear extension point
- **−** OpenAI-only; the Responses API is the architecture
- **−** No auth, persistence or tests
- **−** MCP servers that need auth are left to you
- **−** Last commit 2025-12

<sub>TypeScript, openai · Needs openai-api-key, google-oauth-client · GitHub template · env example file · [Repo](https://github.com/openai/openai-responses-starter-app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-responses-starter-app/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
