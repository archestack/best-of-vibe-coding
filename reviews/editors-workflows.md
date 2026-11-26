# ✏️ AI editors and workflow canvases reviews · Best of Vibe Coding

Rich-text editors with AI commands and node-based canvases for chaining model calls. Back to the [leaderboard](../README.md#%EF%B8%8F-ai-editors-and-workflow-canvases).

<sub>🌐 Also on the web: [AI editors and workflow canvases on archestack.com](https://archestack.com/best-of-vibe-coding/editors-workflows/), each project on its own page.</sub>

<a name="windmill"></a>
### 🥇 [windmill](https://github.com/windmill-labs/windmill) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · custom license · Nov 2026</sub>

**Workflow engine and app builder where scripts become UIs, APIs and cron jobs.**

Windmill turns plain scripts in Python, TypeScript, Go, Bash, SQL and other languages into generated forms, HTTP endpoints and scheduled jobs. Scripts compose into flows, data pipelines, AI agents and React or Svelte apps. The Rust backend runs stateless API servers and workers that pull jobs from a Postgres queue, with nsjail sandboxing and Git sync.

- **+** Stateless Rust API servers and workers; Postgres is the only required datastore
- **+** Typed script arguments generate forms, endpoints and CLI commands automatically
- **+** Triggers include schedules, webhooks, HTTP routes, Kafka, WebSockets and email
- **+** Git sync, CLI and VS Code extension, plus review gates and dev-to-prod promotion
- **−** Community Edition license restricts reselling, wrapping or re-exposing it in your product
- **−** Some features (agent workers, indexer, license key) are Enterprise Edition only
- **−** Deno and PHP runtimes ship only in the windmill-full images
- **−** Maintainers are not seeking outside contributions; only small, trivial PRs accepted

<sub>Rust · Needs PostgreSQL, Caddy (in the compose setup) · Docker · ⚠️ .env file committed · README: alternative to Lovable · [Repo](https://github.com/windmill-labs/windmill) · [▶️ Demo ↗](https://app.windmill.dev) · [📖 Docs ↗](https://www.windmill.dev/docs/intro/) · [🌐 Site ↗](https://www.windmill.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/windmill/)</sub>

<a name="penpot"></a>
### 🥈 [penpot](https://github.com/penpot/penpot) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 63k · MPL-2.0 · Nov 2026</sub>

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

<a name="plate"></a>
### 🥉 [plate](https://github.com/udecode/plate) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · custom license · Nov 2026</sub>

**Rich-text editor framework for React built on Slate, with plugins and AI.**

Plate is a plugin-based rich-text editor framework for React, built on slate-react and published on npm as platejs. The README points to three starting templates: a Notion-like one with plugins, AI and a backend, a playground with plugins and AI, and a minimal one with Plate only. Documentation is at platejs.org.

- **+** Three templates, from minimal editor to Notion-like app with AI and backend
- **+** Plugin system layered on slate-react, installable from npm as platejs
- **+** Chinese-language docs and contributing guide are included
- **−** Notion-like template is documented on pro.platejs.org, suggesting a separate paid tier
- **−** Detected license is NOASSERTION while the README badge says MIT
- **−** Tied to React and Slate; no other framework is mentioned
- **−** README has no feature list, so AI command coverage must be checked in the docs

<sub>TypeScript · Needs React, slate-react · [Repo](https://github.com/udecode/plate) · [📖 Docs ↗](https://platejs.org/docs) · [🌐 Site ↗](https://platejs.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/plate/)</sub>

<a name="next-ai-draw-io"></a>
### #&#8288;4 [next-ai-draw-io](https://github.com/dayuanjiang/next-ai-draw-io) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · Apache-2.0 · Nov 2026</sub>

**Chat with an AI to create and edit draw.io diagrams.**

Next.js app that has an LLM generate draw.io XML on a real draw.io canvas, so diagrams stay editable by hand and export as .drawio, .png, .svg or .drawio.svg. Each AI change is saved as a version you can compare, restore or undo. It also ships as a desktop app and as an MCP server (@next-ai-drawio/mcp-server) for agents such as Claude Code, Cursor and VS Code.

- **+** Output is a normal draw.io file, editable by hand and exportable to four formats
- **+** Per-change version history with compare, restore and Ctrl+Z undo
- **+** 25 providers including Ollama and an OpenAI-compatible preset; browser-entered keys stay local
- **+** Also runs as an MCP server and desktop app; admin panel for models and quotas
- **−** Small models tend to produce broken diagrams; README recommends a capable model
- **−** Default provider is AWS Bedrock, so provider setup is needed before first run
- **−** Hosted demo has a usage limit unless you supply your own API key

<sub>TypeScript, AWS Bedrock, OpenAI, Anthropic, Google AI · Needs LLM provider API key (or Ollama for local models), Node.js and npm · Docker · env example file · [Repo](https://github.com/dayuanjiang/next-ai-draw-io) · [▶️ Demo ↗](https://next-ai-drawio.jiang.jp/) · [📖 Docs ↗](https://next-ai-drawio.jiang.jp/en/docs) · [🌐 Site ↗](https://next-ai-drawio.jiang.jp/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-ai-draw-io/)</sub>

<a name="fresh"></a>
### #&#8288;5 [fresh](https://github.com/sinelaw/fresh) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · GPL-3.0 · Nov 2026</sub>

**Terminal text editor with VS Code-style keybindings, mouse support and LSP.**

Fresh is a Rust terminal text editor that uses standard keybindings, menus and a command palette instead of modal editing. It includes LSP support, multi-cursor editing, split panes, an integrated terminal and TypeScript plugins in a sandboxed QuickJS runtime. An Orchestrator feature runs one workspace per git worktree and can launch coding agents such as claude, codex, opencode and aider.

- **+** Opens multi-gigabyte files with low memory use, per the README
- **+** Single static musl binary for x86_64 and aarch64 with self-update
- **+** Orchestrator gives each git worktree its own workspace, terminals and agent sessions
- **+** Packaged for brew, winget, AUR, deb, rpm, Nix, npm, cargo and Flatpak
- **−** Agent support is a side feature; the core is a general text editor
- **−** Sends anonymous telemetry and daily update checks unless disabled
- **−** GPL-3.0-or-later license may block embedding in proprietary software
- **−** Fresh Desktop builds are unsigned, so macOS and Windows warn on first launch

<sub>Rust, claude, codex, opencode, aider · [Repo](https://github.com/sinelaw/fresh) · [📖 Docs ↗](https://getfresh.dev/docs) · [🌐 Site ↗](https://sinelaw.github.io/fresh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fresh/)</sub>

<a name="yn"></a>
### #&#8288;6 [yn](https://github.com/purocean/yn) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · AGPL-3.0 · Oct 2026</sub>

**Electron Markdown editor with AI completion and a plugin API.**

Yank Note is a desktop Markdown editor built on the Monaco kernel, with local Markdown files as storage. It adds an AI Copilot for text completion, generation and image generation through OpenAI, Ollama, Gemini, Kimi, Tongyi Qianwen or Flux.1, plus OpenCode agent support. Documents can embed runnable code, PlantUML, Drawio, ECharts, Mermaid and applets.

- **+** Notes stay as plain local Markdown files, with optional per-file encryption
- **+** AI backends include OpenAI, Ollama, Gemini, Kimi and Tongyi Qianwen
- **+** Runs JavaScript, PHP, Node.js, Python and bash code blocks inside documents
- **+** JavaScript plugins load from the home directory's plugins folder
- **−** README warns it allows command execution and arbitrary file access; untrusted files are risky
- **−** Encrypted files are decrypted in the front end; a lost password cannot be recovered
- **−** AGPL-3.0 license limits use in closed-source products
- **−** Mac App Store build is marked not recommended by the author

<sub>TypeScript, OpenAI, Ollama, Gemini, Kimi · Needs pandoc (export) · [Repo](https://github.com/purocean/yn) · [▶️ Demo ↗](https://demo.yank-note.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yn/)</sub>

<a name="shaders"></a>
### #&#8288;7 [shaders](https://github.com/shader-effects-inc/shaders) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Nov 2026</sub>

**WebGPU shader effects as components for React, Vue, Svelte, Solid and JS.**

An npm package of 200+ WebGPU effects (gradients, noise, glass, distortions, blurs, cursor effects) exposed as nested layer components. The same props work across React, Vue, Svelte, Solid and a plain JavaScript entry. A hosted design editor exports component code, and a CLI, agent skill and MCP server connect it to coding agents. It is not an AI model project.

- **+** Same component props across React, Vue, Svelte, Solid and vanilla JS entries
- **+** Layers blend on the GPU; custom effects can be written in WGSL via defineShader
- **+** Ships an agent skill, MCP server and llms.txt for coding agents
- **+** Engine and components are MIT licensed; TypeScript with SSR-safe usage
- **−** Not an AI model or LLM tool; fits the list's categories only loosely
- **−** Visual editor, presets and sections are separate from the MIT package, under their own terms
- **−** 1,000+ presets, sections and watermark-free rendering require the paid Pro plan
- **−** Requires WebGPU support in the browser; the std primitives API is marked experimental

<sub>TypeScript · Needs WebGPU-capable browser, shaders.com account for design editor and CLI sync · [Repo](https://github.com/shader-effects-inc/shaders) · [📖 Docs ↗](https://shaders.com/docs/components) · [🌐 Site ↗](https://shaders.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shaders/)</sub>

<a name="builder"></a>
### #&#8288;8 [builder](https://github.com/builderio/builder) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · MIT · Nov 2026</sub>

**Visual editor and SDKs for drag-and-drop editing with your own components.**

Builder.io is a visual development platform that connects to an existing site or app, so pages can be edited by drag and drop or generated from Figma designs using your own components. Changes are exported as code or published through SDKs. This repository holds the SDKs, usage examples, starter projects and plugins; the editor itself is used through a Builder account.

- **+** Renders pages from your existing components via SDKs
- **+** Imports Figma designs and exports them as code
- **+** Repo bundles SDKs, examples, starters and plugins in one place
- **+** MIT licensed, TypeScript codebase
- **−** Editor is used through a Builder.io account sign-up
- **−** README gives no self-hosting instructions
- **−** Monorepo of SDKs and examples, not a standalone app

<sub>TypeScript · Needs Builder.io account · [Repo](https://github.com/builderio/builder) · [📖 Docs ↗](https://www.builder.io/c/docs/developers) · [🌐 Site ↗](https://builder.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/builder/)</sub>

<a name="ui-components"></a>
### #&#8288;9 [ui-components](https://github.com/starc007/ui-components) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

**Animated React and Next.js components installed via the shadcn registry.**

beUI is a library of Framer Motion components for React and Next.js, built with TypeScript and Tailwind CSS. It covers primitives, blocks, AI agent chat UIs, charts and casino games, and installs one component at a time with `npx shadcn@latest add @beui/<name>`. A public MCP server at https://mcp.beui.dev/mcp and a beui skill let coding agents find and retrieve component source.

- **+** Per-component install through the shadcn registry; source is copied into your app
- **+** Public MCP server and llms.txt let coding agents fetch component source without a key
- **+** Includes agent UI pieces: chat layouts, prompt inputs, approvals, tool results
- **+** Accessibility test suite; reduced-motion support where applicable
- **−** Requires a project already set up for shadcn/ui, Tailwind and Framer Motion
- **−** Complete pages and full Next.js templates are in the paid beUI Pro
- **−** Only an accessibility test suite is maintained; no other tests are stated
- **−** Not a starter app: it supplies UI pieces, with no backend, auth or model wiring

<sub>TypeScript · Needs React, Next.js, Tailwind CSS, Framer Motion, shadcn/ui CLI, Bun (to run the repo locally) · env example file · [Repo](https://github.com/starc007/ui-components) · [📖 Docs ↗](https://beui.dev/docs/ai-agents) · [🌐 Site ↗](https://beui.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui-components/)</sub>

<a name="andesine"></a>
### #&#8288;10 [andesine](https://github.com/vriteio/andesine) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · custom license · Nov 2026</sub>

**Collaborative content workspace with structured collections, publishing and an MCP server.**

Andesine is a team content workspace with a real-time Markdown editor, structured collections with schemas and versions, and publishing to hosted documentation sites, an API and SDK, or two-way GitHub sync. It also provides AI search and answers with sources, and an MCP server for Claude, ChatGPT and Cursor. Self-hosting runs through Docker Compose; a managed cloud is also offered.

- **+** Two-way GitHub sync and a TypeScript SDK alongside the hosted docs sites
- **+** Ships an MCP server and CLI for connecting content to AI apps
- **+** Schemas, collections and versions give content a defined structure
- **+** Roles, groups and restricted collections cover team access control
- **−** Mixed licensing: AGPL-3.0 core, MIT packages, Elastic License 2.0 billing code
- **−** Self-hosting details live only on the external docs site

<sub>TypeScript · env example file · [Repo](https://github.com/vriteio/andesine) · [📖 Docs ↗](https://andesine.app/docs) · [🌐 Site ↗](https://andesine.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/andesine/)</sub>

<a name="plate-playground-template"></a>
### #&#8288;11 [plate-playground-template](https://github.com/udecode/plate-playground-template) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 243 · MIT · Nov 2026</sub>

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

<a name="workflow-builder-template"></a>
### #&#8288;12 [workflow-builder-template](https://github.com/vercel-labs/workflow-builder-template) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="nuxt-ui-editor"></a>
### #&#8288;13 [editor](https://github.com/nuxt-ui-templates/editor) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (0) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 171 · MIT · Nov 2026</sub>

**Nuxt template for a Notion-like TipTap editor with AI completions.**

A Nuxt and Nuxt UI starter that wraps TipTap in a Notion-style WYSIWYG editor with slash commands, tables, mentions, drag handles and markdown content. AI completions and text transformations (fix, extend, summarize, translate) stream through the Vercel AI SDK and AI Gateway. Image uploads use NuxtHub Blob, and Y.js collaboration via PartyKit is optional.

- **+** Inline completions with Tab accept, plus selection actions like summarize and translate
- **+** Image upload supports local disk, Vercel Blob, Cloudflare R2 or S3 through NuxtHub
- **+** Collaboration is optional and the Y.js provider can be swapped for Liveblocks or Tiptap
- **+** Content type is markdown, which keeps serialization simple
- **−** AI features need a Vercel AI Gateway key for local development
- **−** Collaboration requires deploying a separate PartyKit server
- **−** Tied to Vue, Nuxt and Nuxt UI; not usable from React
- **−** No Docker setup and no tagged releases

<sub>TypeScript, Any model via Vercel AI Gateway · Needs Vercel AI Gateway (optional), NuxtHub Blob (optional), PartyKit (optional) · GitHub template · env example file · [Repo](https://github.com/nuxt-ui-templates/editor) · [▶️ Demo ↗](https://editor-template.nuxt.dev/) · [📖 Docs ↗](https://ui.nuxt.com/docs/getting-started/installation/nuxt) · [🌐 Site ↗](https://ui.nuxt.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nuxt-ui-editor/)</sub>

<a name="tersa"></a>
### #&#8288;14 [tersa](https://github.com/vercel-labs/tersa) <sub>score [18](../README.md#-how-we-rank "Score 18/100. Adoption: niche (18) · Freshness: slowing (44) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · MIT · Feb 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
