# 🖥️ Agent UI and generative UI reviews · Best of Vibe Coding

Frontends that render agent steps, tool calls, approvals or model-generated components. Back to the [leaderboard](../README.md#%EF%B8%8F-agent-ui-and-generative-ui).

<sub>🌐 Also on the web: [Agent UI and generative UI on archestack.com](https://archestack.com/best-of-vibe-coding/agent-ui/), each project on its own page.</sub>

<a name="opengenerativeui"></a>
### 🥇 [OpenGenerativeUI](https://github.com/copilotkit/openintelligentui) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: patchy (32) · Easy to run: hard (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

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

<a name="agent-chat-ui"></a>
### 🥈 [agent-chat-ui](https://github.com/langchain-ai/agent-chat-ui) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: patchy (30) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Next.js chat frontend for any LangGraph server with interrupts and artifacts.**

A Next.js frontend that connects to any LangGraph server exposing a messages key: enter the deployment URL and assistant ID (or set them as env vars) and you get streaming chat, tool-call rendering, human-in-the-loop interrupts and an artifacts side panel. A built-in API passthrough route injects your LangSmith key server-side for production. For teams that have a LangGraph backend and need a UI today.

- **+** Works against local and deployed LangGraph servers with no backend changes
- **+** Hosted version at agentchat.vercel.app and an npx scaffold
- **+** Message hiding and artifact rendering conventions are documented
- **+** Tests included; committed within the last two days
- **−** The passthrough proxy does not authenticate callers; README warns it exposes your deployment
- **−** Production auth requires custom LangGraph authentication and code edits
- **−** LangGraph SDK only; no AG-UI or AI SDK stream support
- **−** No persistence of its own; threads live in the LangGraph server

<sub>TypeScript, langgraph · Needs langgraph-server, langsmith-api-key-for-deployed-servers · env example file · [Repo](https://github.com/langchain-ai/agent-chat-ui) · [▶️ Demo ↗](https://agentchat.vercel.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-chat-ui/)</sub>

<a name="agno-agent-ui"></a>
### 🥉 [agent-ui](https://github.com/agno-agi/agent-ui) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: known (44) · Freshness: recent (75) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · May 2026</sub>

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

<a name="stockbot-on-groq"></a>
### #&#8288;4 [stockbot-on-groq](https://github.com/bklieger-groq/stockbot-on-groq) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: known (33) · Freshness: quiet (19) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Dec 2025</sub>

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

<a name="assistant-ui-stockbroker"></a>
### #&#8288;5 [assistant-ui-stockbroker](https://github.com/assistant-ui/assistant-ui-stockbroker) <sub>score [11](../README.md#-how-we-rank "Score 11/100. Adoption: niche (5) · Freshness: slowing (46) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 282 · MIT · Feb 2026</sub>

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

<a name="openai-structured-outputs-samples"></a>
### #&#8288;6 [openai-structured-outputs-samples](https://github.com/openai/openai-structured-outputs-samples) <sub>score [9](../README.md#-how-we-rank "Score 9/100. Adoption: niche (19) · Freshness: quiet (22) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 685 · MIT · Dec 2025</sub>

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
