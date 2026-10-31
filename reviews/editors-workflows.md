# ✏️ AI editors and workflow canvases reviews · Best of Vibe Coding

Rich-text editors with AI commands and node-based canvases for chaining model calls. Back to the [leaderboard](../README.md#%EF%B8%8F-ai-editors-and-workflow-canvases).

<sub>🌐 Also on the web: [AI editors and workflow canvases on archestack.com](https://archestack.com/best-of-vibe-coding/editors-workflows/), each project on its own page.</sub>

<a name="penpot"></a>
### 🥇 [penpot](https://github.com/penpot/penpot) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 62k · MPL-2.0 · Oct 2026</sub>

**Open-source design and prototyping tool with real-time collaboration and design tokens.**

Penpot is a browser-based design and prototyping platform that stores designs in open formats (SVG, CSS, HTML, JSON). It offers native design tokens, components and variants, CSS Grid and Flex layout, an inspect tab that shows code, and a plugin system with an API and webhooks. An MCP server lets AI tools read and act on designs. It can be self-hosted or used on the hosted SaaS.

- **+** Designs use open standards (SVG, CSS, HTML, JSON), with an inspect tab for code
- **+** Native design tokens, components and variants for design systems
- **+** MCP server, plugin system and access-token API allow automation and AI workflows
- **+** Self-hostable (Docker, Kubernetes, Elestio) or usable on the hosted SaaS
- **−** Admin Console and SSO are only in the paid Enterprise plan
- **−** Not an AI app starter; the AI features are limited to the MCP server
- **−** README gives no hardware requirements for self-hosting
- **−** Clojure codebase may be unfamiliar to many contributors

<sub>Clojure · Docker · env example file · [Repo](https://github.com/penpot/penpot) · [▶️ Demo ↗](https://design.penpot.app) · [📖 Docs ↗](https://help.penpot.app/technical-guide/) · [🌐 Site ↗](https://penpot.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/penpot/)</sub>

<a name="next-ai-draw-io"></a>
### 🥈 [next-ai-draw-io](https://github.com/dayuanjiang/next-ai-draw-io) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · Apache-2.0 · Oct 2026</sub>

**Chat with an AI to create and edit draw.io diagrams.**

Next.js app that has an LLM generate draw.io XML on a real draw.io canvas, so diagrams stay editable by hand and export as .drawio, .png, .svg or .drawio.svg. Each AI change is saved as a version you can compare, restore or undo. It also ships as a desktop app and as an MCP server (@next-ai-drawio/mcp-server) for agents such as Claude Code, Cursor and VS Code.

- **+** Output is a normal draw.io file, editable by hand and exportable to four formats
- **+** Per-change version history with compare, restore and Ctrl+Z undo
- **+** 25 providers including Ollama and an OpenAI-compatible preset; browser-entered keys stay local
- **+** Also runs as an MCP server and desktop app; admin panel for models and quotas
- **−** Small models tend to produce broken diagrams; README recommends a capable model
- **−** Default provider is AWS Bedrock, so provider setup is needed before first run
- **−** Hosted demo has a usage limit unless you supply your own API key
- **−** RAM requirements are not documented

<sub>TypeScript, AWS Bedrock, OpenAI, Anthropic, Google AI · Needs LLM provider API key (or Ollama for local models), Node.js and npm · Docker · env example file · [Repo](https://github.com/dayuanjiang/next-ai-draw-io) · [▶️ Demo ↗](https://next-ai-drawio.jiang.jp/) · [📖 Docs ↗](https://next-ai-drawio.jiang.jp/en/docs) · [🌐 Site ↗](https://next-ai-drawio.jiang.jp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-ai-draw-io/)</sub>

<a name="plate-playground-template"></a>
### 🥉 [plate-playground-template](https://github.com/udecode/plate-playground-template) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 242 · MIT · Oct 2026</sub>

**Next.js rich-text editor template on Plate with AI commands.**

Next.js 16 template with the Plate editor, shadcn/ui and the Plate AI kit (installable via npx shadcn add @plate/editor-ai), plus an MCP component config. Uploads go through UploadThing with a development-only check in src/lib/uploadthing.ts; AI calls use an AI Gateway key the user enters in editor settings, routed through example API routes. For teams wanting a Notion-style editor with AI inside a React app.

- **+** Plate AI editor installable with one shadcn command
- **+** UploadThing file uploads already wired
- **+** AI routes use the caller's key, so no shared server credential by default
- **−** Upload auth is a development stub; replace before production
- **−** Per-user AI usage limits are left to you
- **−** README is short; features are documented on platejs.org
- **−** No tests; requires bun

<sub>TypeScript, Vercel AI Gateway via AI SDK · Needs UploadThing token, Vercel AI Gateway key (user-supplied) · GitHub template · env example file · [Repo](https://github.com/udecode/plate-playground-template) · [📖 Docs ↗](https://platejs.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/plate-playground-template/)</sub>

<a name="nuxt-ui-editor"></a>
### #&#8288;4 [editor](https://github.com/nuxt-ui-templates/editor) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 171 · MIT · Oct 2026</sub>

**Notion-style Nuxt editor with AI completions and optional collaboration.**

Nuxt template on the Nuxt UI Editor component and TipTap: headings, tables, slash commands, drag handle, mentions, emoji, markdown output and image upload via NuxtHub Blob. AI features (inline completions, continue, fix grammar, extend, simplify, summarize, translate) stream through AI SDK useCompletion and Vercel AI Gateway; collaboration uses Y.js with PartyKit. Scaffold with npm create nuxt -t ui/editor.

- **+** AI, blob storage and collaboration are each optional and env-gated
- **+** One AI Gateway key instead of per-provider keys
- **+** Collaboration via Y.js, swappable from PartyKit to Liveblocks or Tiptap
- **+** Live demo at editor-template.nuxt.dev
- **−** No auth or document persistence; content is not saved server-side
- **−** Collaboration requires deploying a separate PartyKit server
- **−** Translate supports English, French, Spanish and German only
- **−** No tests

<sub>TypeScript, Vercel AI Gateway via AI SDK useCompletion · Needs Vercel AI Gateway key (optional), Blob storage: Vercel Blob, R2 or S3 (optional), PartyKit (optional) · GitHub template · env example file · [Repo](https://github.com/nuxt-ui-templates/editor) · [▶️ Demo ↗](https://editor-template.nuxt.dev/) · [📖 Docs ↗](https://ui.nuxt.com/docs/getting-started/installation/nuxt) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nuxt-ui-editor/)</sub>

<a name="tersa"></a>
### #&#8288;5 [tersa](https://github.com/vercel-labs/tersa) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: niche (23) · Freshness: recent (52) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Feb 2026</sub>

**Node canvas for chaining text, image and video models via AI Gateway.**

Next.js 15 app with a ReactFlow canvas where you connect text, image and video nodes and run them through the Vercel AI SDK Gateway (25+ providers), with streaming output, reasoning display, cost indicators and TipTap for rich text. Canvas state persists in browser local storage; media goes to Vercel Blob. For developers who want a visual model playground to fork; no auth, database or server-side workflow storage.

- **+** One AI Gateway key reaches text, image and video models from 25+ providers
- **+** Relative cost indicators and reasoning output per model
- **+** ReactFlow, TipTap, shadcn/ui and Kibo UI already composed
- **−** Workflows live only in browser local storage
- **−** No auth or multi-user support
- **−** Vercel Blob required for media; Vercel-centric
- **−** Last commit 2026-02; no tests

<sub>TypeScript, Vercel AI SDK Gateway · Needs Vercel AI Gateway credentials, Vercel Blob · [Repo](https://github.com/vercel-labs/tersa) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tersa/)</sub>

<a name="workflow-builder-template"></a>
### #&#8288;6 [workflow-builder-template](https://github.com/vercel-labs/workflow-builder-template) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: known (34) · Freshness: quiet (27) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Jan 2026</sub>

**Visual AI workflow builder on Workflow DevKit with real integrations.**

Next.js 16 app with a React Flow canvas, Monaco editor, Better Auth, Drizzle on Postgres and Workflow DevKit execution. Trigger nodes (webhook, schedule, manual, database event) feed plugins for AI Gateway, Resend, Linear, Slack, GitHub, Stripe, Firecrawl, Perplexity, fal.ai, Clerk, Blob, v0, Webflow and Superagent; workflows can be generated from a prompt and exported as TypeScript with the use workflow directive.

- **+** Fourteen integration plugins with executable step code, not mocks
- **+** Workflows export to TypeScript with the use workflow directive
- **+** Execution history and per-node logs stored in Postgres
- **+** Better Auth and Drizzle already wired
- **−** Each integration needs its own API key
- **−** AI generation goes through Vercel AI Gateway only
- **−** Last commit 2026-01
- **−** Built on Workflow DevKit; swapping the engine is a rewrite

<sub>TypeScript, Vercel AI Gateway (OpenAI GPT-5) · Needs PostgreSQL, Vercel AI Gateway API key, integration API keys (Resend, Linear, Slack, Stripe and others) · GitHub template · sign-in: Better Auth · [Repo](https://github.com/vercel-labs/workflow-builder-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/workflow-builder-template/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
