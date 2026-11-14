# 💳 SaaS and app starters reviews · Best of Vibe Coding

Product boilerplates with auth, billing and a database wired in and AI built in, plus mobile and browser-extension starters. Back to the [leaderboard](../README.md#-saas-and-app-starters).

<sub>🌐 Also on the web: [SaaS and app starters on archestack.com](https://archestack.com/best-of-vibe-coding/saas-with-ai/), each project on its own page.</sub>

<a name="twenty"></a>
### 🥇 [twenty](https://github.com/twentyhq/twenty) <sub>score [97](../README.md#-how-we-rank "Score 97/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 61k · custom license · Nov 2026</sub>

**Open-source CRM extensible with objects, views and agents defined as code.**

Twenty is a CRM built on NestJS, React, PostgreSQL and Redis, with BullMQ for jobs. Teams define custom objects, fields and views in TypeScript with twenty-sdk, scaffold apps with `npx create-twenty-app`, and publish them to a workspace from the CLI. It also includes workflows, AI agents and chat, and runs as a cloud service or self-hosted via Docker Compose.

- **+** Objects, fields and views defined in TypeScript and published with `npx twenty app:publish`
- **+** Cloud and self-hosted options; Docker Compose guide in the docs
- **+** Official agent skills for Claude Code, Codex and Cursor to build Twenty apps
- **+** Standard stack: NestJS, PostgreSQL, Redis, React, Nx monorepo
- **−** License is reported as NOASSERTION; terms need manual checking
- **−** README gives no RAM, CPU or port requirements for self-hosting
- **−** Self-hosting needs PostgreSQL and Redis alongside the app
- **−** README does not name supported AI providers or models

<sub>TypeScript · Needs PostgreSQL, Redis · [Repo](https://github.com/twentyhq/twenty) · [📖 Docs ↗](https://docs.twenty.com) · [🌐 Site ↗](https://twenty.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/twenty/)</sub>

<a name="wails"></a>
### 🥈 [wails](https://github.com/wailsapp/wails) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · MIT · Nov 2026</sub>

**Framework for building desktop apps with a Go backend and web frontend.**

Wails packages Go code and an HTML/JS/CSS frontend into a single desktop binary, using the operating system's native webview instead of an embedded browser. A CLI handles project creation, compilation and bundling, and Go methods can be called from JavaScript with generated TypeScript definitions. It has no AI features; it is a general desktop app framework and fits this list only loosely.

- **+** Uses native rendering engines, so no bundled browser as in Electron
- **+** Auto-generated TypeScript definitions for Go structs and methods
- **+** Works with any frontend stack, with pre-built project templates
- **+** Native dialogs, menus, dark/light mode and window translucency effects
- **−** No AI, model or agent functionality; off-topic for this list
- **−** Backend must be written in Go
- **−** Two active versions (v2 and v3) with separate install paths and docs

<sub>Go · Needs Go toolchain · [Repo](https://github.com/wailsapp/wails) · [📖 Docs ↗](https://v2.wails.io/) · [🌐 Site ↗](https://wails.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wails/)</sub>

<a name="quasar"></a>
### 🥉 [quasar](https://github.com/quasarframework/quasar) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Nov 2026</sub>

**Vue.js framework for web, mobile, desktop and extension apps from one codebase.**

Quasar is a Vue.js framework with a component library and a Vite-based CLI. One codebase can target SPAs, SSR, SSG, PWAs, browser extensions, hybrid mobile apps and Electron apps. The README says its docs and API can be read offline by AI coding agents and lists an @quasar/mcp package. It is a general UI framework, not an AI starter with auth or billing.

- **+** One codebase targets SPA, SSR, SSG, PWA, browser extension, mobile and Electron
- **+** Official create-quasar scaffolder and Vite integration via @quasar/app-vite
- **+** Docs and API readable offline by coding agents, plus an @quasar/mcp package
- **+** MIT license, with separate CI test workflows per package
- **−** No built-in auth, billing, database or model integration
- **−** Tied to Vue.js; not usable with React or other frameworks
- **−** AI support is limited to docs and an MCP package, with no LLM features
- **−** Fits the SaaS and app starters category only loosely; it is a UI framework

<sub>JavaScript · Needs Node.js, Vue.js, Vite · [Repo](https://github.com/quasarframework/quasar) · [📖 Docs ↗](https://quasar.dev) · [🌐 Site ↗](https://quasar.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/quasar/)</sub>

<a name="next-js"></a>
### #&#8288;4 [next.js](https://github.com/vercel/next.js) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 144k · MIT · Nov 2026</sub>

**React framework for full-stack web apps with Rust-based build tooling.**

Next.js is a React framework for building full-stack web applications, extending current React features and using Rust-based JavaScript tooling for builds. This repository is the framework itself, not an AI starter. It is the base that many AI web app templates build on.

- **+** Full documentation, a Learn course and a showcase of production sites
- **+** Rust-based tooling is used for builds
- **+** MIT license, with a recent release and recent commits
- **+** GitHub Discussions, Discord and a bug bounty program
- **−** Framework only: no built-in AI features, auth, billing or database
- **−** README gives no install steps, version requirements or feature list
- **−** Not an AI project; relevant here only as a dependency of starters
- **−** README does not describe hosting or deployment options

<sub>JavaScript · Needs React · [Repo](https://github.com/vercel/next.js) · [📖 Docs ↗](https://nextjs.org/docs) · [🌐 Site ↗](https://nextjs.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-js/)</sub>

<a name="heroui"></a>
### #&#8288;5 [heroui](https://github.com/heroui-inc/heroui) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · Apache-2.0 · Nov 2026</sub>

**React component library on React Aria and Tailwind CSS v4.**

HeroUI (formerly NextUI) is a React component library that pairs React Aria accessibility primitives with Tailwind CSS v4 styling. It uses a compound component API such as Card.Header and Card.Content, needs no Provider wrapper, and targets React 19 and Next.js. It also publishes an MCP server (@heroui/react-mcp), llms.txt and agent skills for AI coding tools.

- **+** Built on React Aria for keyboard, focus and screen-reader behavior
- **+** Tailwind CSS v4 styling with no CSS-in-JS runtime
- **+** No Provider wrapper; per-component subpath imports available
- **+** Ships MCP server, llms.txt, AGENTS.md download and agent skills
- **−** UI library only; no auth, billing, database or AI features included
- **−** React and Tailwind v4 only; no support for other frameworks
- **−** v3 API differs from v2, so older NextUI code needs migration
- **−** Not copy-paste source like shadcn/ui; customization goes through the library

<sub>TypeScript · Needs React 19, Tailwind CSS v4 · [Repo](https://github.com/heroui-inc/heroui) · [📖 Docs ↗](https://heroui.com/docs/react/getting-started/quick-start) · [🌐 Site ↗](https://heroui.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/heroui/)</sub>

<a name="reflex"></a>
### #&#8288;6 [reflex](https://github.com/reflex-dev/reflex) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Nov 2026</sub>

**Python framework for building full-stack web apps without writing JavaScript.**

Reflex lets you write both the frontend UI and backend logic of a web app in Python. State lives in classes with event handlers, and the dev server runs at localhost:3000 with fast refresh. The README's example calls an OpenAI image model from an async event handler.

- **+** UI, state and event handlers all written in Python, no JavaScript required
- **+** Fast refresh in the dev server shows code changes on save
- **+** Installs from PyPI and starts with uv: init, then run
- **+** Optional Agent Toolkit connects MCP and Skills to coding assistants
- **−** General web framework, not an AI starter; no built-in auth, billing or database described
- **−** Ships no Docker or compose files in the detected repo facts
- **−** AI Builder and app hosting are separate hosted offerings
- **−** Architecture details are on an external page, not in the README

<sub>Python, OpenAI image generation (example only) · Needs uv · [Repo](https://github.com/reflex-dev/reflex) · [📖 Docs ↗](https://reflex.dev/docs/getting-started/introduction) · [🌐 Site ↗](https://reflex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reflex/)</sub>

<a name="astryx"></a>
### #&#8288;7 [astryx](https://github.com/meta/astryx) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Nov 2026</sub>

**React 19 design system with 150+ components, themes and a CLI for agents.**

Astryx is a React component library from Meta with 150+ typed, accessible components, seven ready-made themes, dark mode and page templates. Styles are authored in StyleX but shipped as pre-built CSS, so consumers need no build plugin and can override with className (Tailwind, CSS modules, plain CSS). A CLI exposes component docs, scaffolding, themes and codemods so coding assistants and people use the same reference. Currently in beta.

- **+** Ships pre-built CSS; no build plugin, PostCSS or Babel config required
- **+** Themes are CSS custom property overrides, so no forking or wrapping components
- **+** Swizzle ejects a component's full source into your project
- **+** CLI provides component docs and scaffolding for both developers and AI assistants
- **−** Beta status; APIs may change before a stable release
- **−** Requires React 19 or later
- **−** Chart packages are published only under the @canary npm tag
- **−** Not an app starter: no auth, billing or database included

<sub>TypeScript · Needs React 19+, @stylexjs/stylex, Node 22+ and pnpm 11 (contributors) · [Repo](https://github.com/meta/astryx) · [▶️ Demo ↗](https://astryx.atmeta.com/sandbox/) · [📖 Docs ↗](https://astryx.atmeta.com) · [🌐 Site ↗](https://astryx.atmeta.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/astryx/)</sub>

<a name="adminlte"></a>
### #&#8288;8 [adminlte](https://github.com/colorlibhq/adminlte) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Oct 2026</sub>

**Bootstrap 5.3 admin dashboard template in vanilla JavaScript, no jQuery.**

AdminLTE 4 is an HTML/CSS/TypeScript admin dashboard template built on Bootstrap 5.3.8 with no jQuery. It ships dark mode, RTL support and demo pages such as Calendar, Kanban, Chat, Mailbox and Tabulator data tables. Separate repositories provide React/Next.js, Vue/Nuxt, Angular, Laravel, Django, Symfony, ASP.NET and Drupal editions. It has no AI features, so it fits this list only as a UI starter.

- **+** Installs via CDN, npm or Composer; the CDN path needs no build step
- **+** Dark mode uses Bootstrap's native data-bs-theme attribute; RTL is included
- **+** Official editions for React, Vue, Angular, Laravel, Django, Symfony, ASP.NET and Drupal
- **+** Demo pages cover Calendar, Kanban, Chat, File Manager, Mailbox, Wizard and invoices
- **−** UI template only: no auth, billing, database or backend, and no AI features
- **−** v4 breaks v3: renamed classes and data attributes, bundled plugins/ folder removed
- **−** Demo pages must be excluded from production deploys to avoid exposing examples
- **−** Premium templates are promoted in the README; some pages and editions are paid elsewhere

<sub>Astro · Needs Bootstrap 5.3, Node.js 22.22.3+ / 24.16.0+ / 26.3.0+ and npm 10+ (to develop AdminLTE itself) · [Repo](https://github.com/colorlibhq/adminlte) · [▶️ Demo ↗](https://adminlte.io/themes/v4/) · [📖 Docs ↗](https://adminlte.io/themes/v4/docs/introduction.html) · [🌐 Site ↗](https://adminlte.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/adminlte/)</sub>

<a name="tabler"></a>
### #&#8288;9 [tabler](https://github.com/tabler/tabler) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Nov 2026</sub>

**Bootstrap 5 admin dashboard UI kit with layouts, components and demo pages.**

Tabler is an HTML/CSS/JS UI kit on Bootstrap 5 for admin panels and dashboards, shipped as the @tabler/core npm package or via CDN. It includes over 120 demo pages, dark mode, RTL stylesheets, Sass and TypeScript sources, and more than 20 bundled plugins. It has no AI features, though the README mentions an installable skill for coding agents.

- **+** Plain HTML and CSS, with setup guides for React, Vue, Angular, Laravel, Django and others
- **+** Over 120 demo pages: dashboards, forms, tables, auth screens, error pages
- **+** Dark mode on every component and RTL version of every stylesheet
- **+** Sass sources and TypeScript types included for theme customization
- **−** UI only: no backend, auth logic, billing or database, and no built-in AI features
- **−** Needs recent browsers: Chrome 123, Firefox 128, Safari 17.5 minimum
- **−** Bundled ApexCharts is dual-licensed; revenue above $2M needs a paid license
- **−** Not a fit for the AI-starter list's usual scope; the agent skill is a side feature

<sub>Astro · Needs Bootstrap 5 (bundled), Node.js and pnpm (for local development) · Docker · [Repo](https://github.com/tabler/tabler) · [▶️ Demo ↗](https://preview.tabler.io) · [📖 Docs ↗](https://docs.tabler.io) · [🌐 Site ↗](https://tabler.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tabler/)</sub>

<a name="react-admin"></a>
### #&#8288;10 [react-admin](https://github.com/marmelab/react-admin) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Nov 2026</sub>

**React framework for CRUD admin apps on top of REST or GraphQL APIs.**

react-admin is a TypeScript library of React components and hooks for building browser-based admin and back-office apps. It uses Material UI, react-hook-form, react-router and react-query, and talks to any API through swappable Data Providers (more than 45 adapters listed). It has no AI features, so it fits this list only as a general app starter.

- **+** Data Provider adapters: 45+ listed, and a custom one is described as a matter of hours
- **+** Ships list, edit and create views, forms, auth hooks, i18n, roles and rich text editor
- **+** Any component can be replaced, including swapping Material UI for Bootstrap
- **+** Demo apps with source: e-commerce, CRM, helpdesk, blog, plus a tutorial
- **−** No AI features, so it does not match the theme of this list
- **−** Default UI is tied to Material UI
- **−** Library only: no backend, auth server or database is included
- **−** Commercial support is sold through a paid Enterprise Edition

<sub>TypeScript · Needs React, Material UI, react-hook-form, react-router, react-query, a REST or GraphQL API · env example file · [Repo](https://github.com/marmelab/react-admin) · [▶️ Demo ↗](https://marmelab.com/react-admin-demo/) · [📖 Docs ↗](https://marmelab.com/react-admin/documentation.html) · [🌐 Site ↗](https://marmelab.com/react-admin/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-admin/)</sub>

<a name="wasp"></a>
### #&#8288;11 [wasp](https://github.com/wasp-lang/wasp) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

**Full-stack framework that generates React, Node.js and Prisma apps from a spec.**

Wasp is a Rails-like framework for React, Node.js (Express) and Prisma. You describe routes, pages, auth, queries and actions in a main.wasp.ts spec, and the compiler generates the front end, back end and deployment code. It includes auth, client-server RPC, jobs and email sending, and offers official plugins for AI coding agents.

- **+** Declarative spec covers routes, auth, queries and actions in one file
- **+** Built-in auth, RPC, jobs and email sending
- **+** Generated code is viewable in .wasp/ and deployable to any provider
- **+** Official agent plugins for Cursor, Claude Code and similar tools
- **−** Supports only React, Express and Prisma; other stacks are future plans
- **−** Declared beta; changes between versions are expected
- **−** Adds a spec layer on top of the stack that you must learn
- **−** Not an AI starter itself; no LLM integration described in the README

<sub>TypeScript · Needs Node.js, Prisma · [Repo](https://github.com/wasp-lang/wasp) · [📖 Docs ↗](https://wasp.sh/docs) · [🌐 Site ↗](https://wasp.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wasp/)</sub>

<a name="polar"></a>
### #&#8288;12 [polar](https://github.com/polarsource/polar) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · Apache-2.0 · Nov 2026</sub>

**Billing and merchant-of-record platform with usage metering and subscriptions.**

Polar is a billing backend for software products, supporting usage-based billing, subscriptions, seats, credits, trials and discounts. It acts as merchant of record, handling receipts, customer accounts, dunning, sales tax and VAT. The stack is a Python FastAPI API with a Next.js dashboard, exposed through a public API, webhooks and JS and Python SDKs.

- **+** Meters events such as tokens, API calls, agent runs and GPU seconds
- **+** Merchant of record handles sales tax, VAT, receipts and dunning
- **+** Public API, webhooks and official JavaScript and Python SDKs
- **+** Apache-2.0 licensed; built on FastAPI, SQLAlchemy, Dramatiq and Next.js
- **−** Hosted service charges 3.4% to 5% plus a fixed fee per transaction
- **−** README has no self-hosting steps; DEVELOPMENT.md covers dev setup only
- **−** No Docker or compose files detected in the repository
- **−** Full platform codebase, not a small starter to fork and customize

<sub>Python · Needs IPinfo, Sentry · [Repo](https://github.com/polarsource/polar) · [📖 Docs ↗](https://polar.sh/docs) · [🌐 Site ↗](https://polar.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/polar/)</sub>

<a name="gentelella"></a>
### #&#8288;13 [gentelella](https://github.com/colorlibhq/gentelella) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Sep 2026</sub>

**Vanilla JS and SCSS admin dashboard template with 58 static pages.**

Gentelella v4 is an admin dashboard template built with vanilla ES2022, SCSS and Vite 8, with no Bootstrap, jQuery or SPA framework. It ships 58 HTML pages covering dashboards, auth screens, forms, DataTables, 20 ECharts variants, inbox, kanban, calendar and e-commerce views, plus dark mode, RTL and PWA support. It has no AI features of its own beyond helper files for Claude Code, Cursor and Copilot.

- **+** No Bootstrap, jQuery or framework runtime; 3 production dependencies
- **+** 58 prebuilt pages including inbox, kanban, file manager and 4 dashboard variants
- **+** Builds to static files deployable to any static host, with subpath support
- **+** Ships CLAUDE.md, Cursor rules, Copilot instructions and AGENTS.md for AI tools
- **−** Front-end only: no real auth, billing or database; data is seeded or via ?api=1 adapter
- **−** No AI functionality in the template; category fit is loose
- **−** Not tied to React, Vue or Svelte; other stacks need separate paid templates
- **−** Only a Laravel edition is listed as a framework port

<sub>HTML · Needs Node.js, npm, Google Fonts (Inter) · [Repo](https://github.com/colorlibhq/gentelella) · [▶️ Demo ↗](https://preview.colorlib.com/theme/gentelella/) · [📖 Docs ↗](https://gentelella.colorlib.com/docs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gentelella/)</sub>

<a name="yudao-cloud"></a>
### #&#8288;14 [yudao-cloud](https://github.com/yunaiv/yudao-cloud) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Nov 2026</sub>

**Spring Cloud Alibaba admin platform with multi-tenancy, workflow and code generator.**

Yudao-cloud is a Java microservice backend for admin and business systems on Spring Cloud Alibaba (Nacos, Gateway, Sentinel, Seata, XXL-Job). It ships RBAC, SaaS multi-tenancy, Flowable workflows, payments, a code generator for Java/Vue/SQL, and optional ERP, CRM, mall and AI modules. Vue3 admin frontends are separate repositories.

- **+** MIT license; README states no commercial edition and all code is open
- **+** Code generator emits Java, Vue, SQL and tests for single, tree and master-detail tables
- **+** Supports MySQL, PostgreSQL, Oracle, SQL Server and several Chinese domestic databases
- **+** Built-in multi-tenancy, SSO/OAuth2, and Flowable workflow with BPMN and DingTalk-style designers
- **−** AI is one optional module in the full edition; the core is a generic admin platform
- **−** Needs Nacos, Redis and a database; full microservice stack is heavy to run
- **−** Default master branch is JDK 8 + Spring Boot 2.7; newer JDKs sit on other branches
- **−** README and docs are mainly in Chinese; frontends and the mini edition live in separate repos

<sub>Java · Needs Nacos, Redis, MySQL, XXL-Job, Sentinel, Seata · [Repo](https://github.com/yunaiv/yudao-cloud) · [▶️ Demo ↗](http://dashboard-vue3.yudao.iocoder.cn) · [📖 Docs ↗](https://cloud.iocoder.cn/quick-start/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yudao-cloud/)</sub>

<a name="next-js-boilerplate"></a>
### #&#8288;15 [next-js-boilerplate](https://github.com/ixartz/next-js-boilerplate) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

**Next.js 16 starter with Clerk auth, Drizzle ORM, Tailwind 4 and tooling.**

A clone-and-edit Next.js App Router starter in TypeScript with Tailwind CSS 4, Clerk authentication, and Drizzle ORM on PostgreSQL (PGlite locally, Neon suggested for production). It also wires in next-intl i18n, Vitest, Playwright, Storybook, Sentry, LogTape and Arcjet. It includes no AI features beyond agent instruction files and CodeRabbit review.

- **+** Runs locally with embedded PGlite database, no Docker or extra setup
- **+** Broad dev tooling preconfigured: Vitest, Playwright, Storybook, Commitlint, Knip, i18n-check
- **+** Drizzle ORM supports PostgreSQL, SQLite and MySQL, with migration scripts
- **+** Includes instruction files for Claude Code, Codex, Cursor, OpenCode and Copilot
- **−** Auth depends on a hosted Clerk account and API keys
- **−** No billing; Stripe, teams, RBAC and shadcn UI are in the paid Pro kit
- **−** No built-in AI features such as chat or model calls
- **−** Many sponsor-linked services (Sentry, Arcjet, Crowdin, Better Stack) to configure or strip out

<sub>TypeScript · Needs Node.js 24+, npm, Clerk, PostgreSQL (PGlite locally, Neon optional), Sentry, Crowdin, Arcjet · GitHub template · ⚠️ .env file committed · sign-in: Clerk · [Repo](https://github.com/ixartz/next-js-boilerplate) · [▶️ Demo ↗](https://demo.nextjs-boilerplate.com) · [🌐 Site ↗](https://nextjs-boilerplate.com/pro-saas-starter-kit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-js-boilerplate/)</sub>

<a name="ant-design-pro"></a>
### #&#8288;16 [ant-design-pro](https://github.com/ant-design/ant-design-pro) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Oct 2026</sub>

**React admin dashboard template built on Ant Design 6 and Umi Max.**

Ant Design Pro is a React 19 and TypeScript boilerplate for enterprise back-office apps, built on Umi Max 4 and antd 6. It ships ready-made pages for dashboards, forms, lists, profiles, account settings, login and error screens, plus i18n, mock data and unit and e2e tests. A built-in AI chatbot page uses Ant Design X, and an `npm run simple` script strips the template down to a minimal version.

- **+** Includes dashboard, form, list, profile, account and result page templates
- **+** Built-in i18n, mock development setup, and unit and e2e tests
- **+** Ships Claude Code skills for upgrading the template and querying antd APIs
- **+** TypeScript with Tailwind CSS v4 and antd-style theming
- **−** AI support is a single chatbot page; no model backend is described
- **−** `npm run simple` permanently deletes files and cannot be undone
- **−** Tied to the Umi Max and antd stack; no other frameworks
- **−** No Docker or compose setup mentioned in the README

<sub>TypeScript · GitHub template · [Repo](https://github.com/ant-design/ant-design-pro) · [▶️ Demo ↗](https://preview.pro.ant.design) · [📖 Docs ↗](https://github.com/ant-design/ant-design-pro/blob/master/docs/cheatsheet.en-US.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ant-design-pro/)</sub>

<a name="abp"></a>
### #&#8288;17 [abp](https://github.com/abpframework/abp) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · LGPL-3.0 · Nov 2026</sub>

**Opinionated .NET framework for enterprise apps with DDD, modules and multi-tenancy.**

ABP is an application framework on top of ASP.NET Core that supplies infrastructure for domain-driven design, modular monoliths, microservices and multi-tenancy. It ships startup templates, pre-built modules (Identity, OpenIddict, CMS Kit, SaaS, Account), and tooling: ABP CLI, ABP Studio and ABP Suite for page generation. It is not an AI project; it is a general .NET business-application framework.

- **+** Built-in event bus, background jobs, audit logging, BLOB storing and data seeding
- **+** First-class multi-tenancy, modularity and DDD support
- **+** Pre-built modules for identity, OpenIddict, CMS and tenant management
- **+** Active: release on 2026-11-03, commit on 2026-11-09
- **−** No AI features described; poor fit for an AI-focused starter list
- **−** Several modules and tools (Suite, Account, SaaS) link to Pro editions
- **−** Opinionated architecture locks you into ABP conventions and .NET
- **−** LGPL-3.0 license has linking and distribution obligations

<sub>C# · Needs .NET, ASP.NET Core · [Repo](https://github.com/abpframework/abp) · [📖 Docs ↗](https://abp.io/docs/latest) · [🌐 Site ↗](https://abp.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/abp/)</sub>

<a name="wave"></a>
### #&#8288;18 [wave](https://github.com/thedevdojo/wave) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Nov 2026</sub>

**Laravel SaaS framework with auth, billing, roles, blog and themes.**

Wave is a Laravel-based SaaS framework that ships the common product pieces: authentication, user profiles, impersonation, billing with subscription plans, roles and permissions, notifications, an API and an admin panel. It also includes a blog, changelog, pages, themes and plugins. The README does not mention built-in AI features, so any AI functionality would be added by the developer.

- **+** Auth, billing, subscription plans and roles/permissions are included out of the box
- **+** Ships admin panel, API, blog, changelog and user impersonation
- **+** Theme and plugin system, with a live demo that previews themes
- **+** MIT licensed, with documentation and an automated installer
- **−** No AI features described in the README; they must be added yourself
- **−** Requires a PHP and Laravel stack
- **−** Video course and premium content sit behind a paid DevDojo Pro subscription

<sub>PHP · Needs PHP, Laravel · env example file · [Repo](https://github.com/thedevdojo/wave) · [▶️ Demo ↗](https://devdojo.com/wave/demo) · [📖 Docs ↗](https://devdojo.com/wave/docs) · [🌐 Site ↗](https://devdojo.com/wave) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wave/)</sub>

<a name="react-bits"></a>
### #&#8288;19 [react-bits](https://github.com/davidhdev/react-bits) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 52k · custom license · Nov 2026</sub>

**Animated React component library installed through the shadcn CLI.**

React Bits is a collection of 215+ animated React components: text effects, cursor and hover animations, cards and galleries, micro-interactions, and 63 shader and particle backgrounds. Each comes in JS or TS, with CSS or Tailwind, and installs through the shadcn CLI or jsrepo, or by copying files. A shadcn registry entry lets coding agents such as Claude Code or Cursor add components through MCP.

- **+** Four variants per component: JS or TS, CSS or Tailwind
- **+** Installs per component with one shadcn or jsrepo command, no package dependency
- **+** Live demos with controls, plus browser tools for exporting backgrounds as code, image or video
- **+** Works with the shadcn MCP server so agents can find and add components
- **−** License is MIT + Commons Clause, which restricts selling the software; not OSI open source
- **−** Not an AI project: a UI library with only an agent-install path
- **−** Pages, templates and agent skills are in the paid Pro tier
- **−** Heavy shader and particle backgrounds can cost performance; README gives no benchmarks

<sub>JavaScript · Needs React, shadcn CLI or jsrepo · [Repo](https://github.com/davidhdev/react-bits) · [▶️ Demo ↗](https://reactbits.dev) · [📖 Docs ↗](https://reactbits.dev/get-started/introduction) · [🌐 Site ↗](https://reactbits.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-bits/)</sub>

<a name="create-better-t-stack"></a>
### #&#8288;20 [create-better-t-stack](https://github.com/amanvarshney01/create-better-t-stack) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

**CLI that scaffolds type-safe TypeScript monorepos from a chosen stack.**

create-better-t-stack is an interactive CLI that generates a TypeScript project from selected parts: frontend (React, Next.js, Nuxt, Svelte, Solid, Astro, React Native), backend (Hono, Express, Fastify, Elysia, Convex), tRPC or oRPC, a database with Drizzle, Prisma or Mongoose, and Better Auth or Clerk. It also ships a Claude Code plugin with an MCP server so an assistant can plan and generate a stack.

- **+** Wide choice of frontends, backends, ORMs and databases; only selected parts are generated
- **+** Addons include Turborepo, Nx, Biome, Tauri, PWA and WXT
- **+** Bundled Claude Code plugin and MCP server can scaffold stacks from a description
- **+** Web Stack Builder generates the CLI command for a chosen stack
- **−** Scaffolds a project once; README describes no update or migration path
- **−** AI is only an optional example template, not a core feature
- **−** Web deploy targets only Cloudflare Workers
- **−** Billing is not among the listed generated options

<sub>TypeScript · Needs Bun, pnpm or npm, Turso, Neon, Supabase, MongoDB Atlas or Cloudflare D1 (optional DB setup) · [Repo](https://github.com/amanvarshney01/create-better-t-stack) · [📖 Docs ↗](https://better-t-stack.dev/docs/cli/agent-workflows) · [🌐 Site ↗](https://better-t-stack.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/create-better-t-stack/)</sub>

<a name="formkit"></a>
### #&#8288;21 [formkit](https://github.com/formkit/formkit) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Nov 2026</sub>

**Form framework for React and Vue with inline validation and schema-generated forms.**

FormKit provides a single `<FormKit>` component for every input type, with 30+ built-in validation rules declared inline and data structured by nested group and list types. Forms can also be generated from serializable JSON schemas. It has a framework-agnostic core with Vue 3 and React 18/19 bindings, and `npx formkit skill` configures coding agents with its docs.

- **+** One component for all inputs, with automatic ARIA labels and descriptions
- **+** JSON schema can generate whole forms, including conditionals and loops
- **+** Shared core across Vue 3 and React 18/19 bindings
- **+** Ships 30+ languages for i18n, switchable at runtime
- **−** Only Vue and React bindings; no other frameworks listed
- **−** Advanced inputs (datepicker, autocomplete, repeater) are in the paid Pro tier
- **−** Not an AI project itself; the agent angle is a skill installer and docs
- **−** Tailwind-oriented Regenesis theme; other styling needs custom work

<sub>TypeScript · [Repo](https://github.com/formkit/formkit) · [📖 Docs ↗](https://formkit.com/getting-started/installation) · [🌐 Site ↗](https://formkit.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/formkit/)</sub>

<a name="shadcn-svelte"></a>
### #&#8288;22 [shadcn-svelte](https://github.com/huntabyte/shadcn-svelte) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · MIT · Nov 2026</sub>

**Copy-paste accessible UI components for Svelte, ported from shadcn/ui.**

shadcn-svelte is a community port of shadcn/ui for Svelte. It provides accessible, customizable components that you copy into your own project and edit, rather than installing as a locked dependency. It is meant as a base for building your own component library, and it contains no AI functionality itself.

- **+** Components are copied into your codebase, so you own and can edit the source
- **+** MIT licensed, with documentation hosted at shadcn-svelte.com
- **+** Follows the shadcn/ui design approach, familiar to React users moving to Svelte
- **+** Active: commit and release both dated 2026-11-03
- **−** Unofficial port, not affiliated with the shadcn/ui authors
- **−** Svelte only; no React, Vue or other framework output
- **−** No AI features, auth, billing or database; UI components only
- **−** Copied components must be updated by hand when upstream changes

<sub>TypeScript · Needs Svelte · [Repo](https://github.com/huntabyte/shadcn-svelte) · [📖 Docs ↗](https://shadcn-svelte.com/docs) · [🌐 Site ↗](https://www.shadcn-svelte.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shadcn-svelte/)</sub>

<a name="astrowind"></a>
### #&#8288;23 [astrowind](https://github.com/arthelokyo/astrowind) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Sep 2026</sub>

**Astro and Tailwind CSS template for marketing sites and blogs.**

Static website template built on Astro and Tailwind CSS v4, with 30+ typed page-section widgets, a Markdown/MDX blog with RSS, categories and tags, sitemap, Open Graph tags and optional Google Analytics. It is not an AI app: the AI angle is an AGENTS.md and task skills in .agents/skills/ for coding assistants such as Claude Code, Codex and Cursor. Site settings live in src/config.yaml.

- **+** 30+ typed section widgets plus six ready-made landing pages in src/pages/landing
- **+** Static output with image optimization, sitemap, RSS and Open Graph tags configured
- **+** Ships AGENTS.md and step-by-step skills so coding assistants can apply common changes
- **+** Dark mode, RTL and shadcn/ui-compatible design tokens included
- **−** No auth, billing or database; it is a content site, not a SaaS boilerplate
- **−** No AI features at runtime; AI support is limited to agent instruction files
- **−** Blog only works with prerender = true, which constrains server-rendered setups
- **−** README says v1 is in maintenance mode, with new work going to v2

<sub>Astro · Needs Node.js >= 22.22.3 · GitHub template · Docker · [Repo](https://github.com/arthelokyo/astrowind) · [▶️ Demo ↗](https://astrowind.vercel.app/) · [🌐 Site ↗](https://arthelokyo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/astrowind/)</sub>

<a name="vue-vben-admin"></a>
### #&#8288;24 [vue-vben-admin](https://github.com/vbenjs/vue-vben-admin) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Nov 2026</sub>

**Vue 3 and Vite admin dashboard template with permissions and i18n.**

Vue Vben Admin is a front-end template for middle and back-office admin apps, built on Vue 3, Vite and TypeScript. It ships theme options, built-in internationalization and dynamic route-based permission generation. Version 5.0 is not compatible with earlier versions, which remain on the v2 branch.

- **+** MIT license, with a live preview and a test account
- **+** Built-in i18n, multiple theme colors and dynamic route-based permissions
- **+** Documentation site, plus README in English, Chinese and Japanese
- **+** Plain pnpm workflow: install, dev, build
- **−** Front end only: no AI features, backend, database or billing in the README
- **−** Version 5.0 is incompatible with v2 projects, so upgrading means a rewrite
- **−** Full-version preview site is in Chinese
- **−** Modern browsers only: Safari 16.4+, Chrome 111+, Firefox 128+

<sub>TypeScript · Needs Node.js, pnpm, corepack · [Repo](https://github.com/vbenjs/vue-vben-admin) · [▶️ Demo ↗](https://vben.pro/) · [📖 Docs ↗](https://doc.vben.pro/) · [🌐 Site ↗](https://vben.pro/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vue-vben-admin/)</sub>

<a name="next-shadcn-dashboard-starter"></a>
### #&#8288;25 [next-shadcn-dashboard-starter](https://github.com/kiranism/next-shadcn-dashboard-starter) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Nov 2026</sub>

**Next.js 16 admin dashboard template with Clerk auth, organizations and billing.**

Admin dashboard starter built on Next.js 16 (App Router), React 19, Tailwind CSS v4 and shadcn/ui on Base UI primitives. Tables, forms, auth, organizations and billing are wired end to end, using TanStack Query with server prefetch and nuqs URL state. A cleanup script removes demo features you do not need, including Clerk.

- **+** Working data tables with server prefetch, URL-synced search, filter, sort and pagination
- **+** Clerk organizations, billing and plan-gated pages included
- **+** Cleanup script removes optional features, including Clerk, with a dry-run mode
- **+** Ships AGENTS.md, CLAUDE.md and a Claude Code skill for coding agents
- **−** Auth, orgs and billing depend on Clerk; replacing it means wiring your own auth
- **−** Product and user data are mock data in constants, with no database layer
- **−** AI chat page is a scripted demo with no model or API route
- **−** Pulling upstream changes after forking can cause merge conflicts

<sub>TypeScript · Needs Clerk, Sentry, Bun or npm · GitHub template · Docker · sign-in: Clerk · [Repo](https://github.com/kiranism/next-shadcn-dashboard-starter) · [▶️ Demo ↗](https://dub.sh/shadcn-dashboard) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-shadcn-dashboard-starter/)</sub>

<a name="hackathon-starter"></a>
### #&#8288;26 [hackathon-starter](https://github.com/sahat/hackathon-starter) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (91) · Freshness: active (92) · Maintenance: patchy (42) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Nov 2026</sub>

**Node.js and Express boilerplate with auth, API examples and AI samples.**

Hackathon Starter is an Express and MongoDB web app template with local, passkey and OAuth 2.0 sign-in, account management, 2FA, a contact form and file upload. It ships examples for third-party APIs such as Stripe, Twilio and Google Maps, plus AI samples: a ReAct agent with tool calling and MongoDB session persistence, and RAG with embedding caching. Views are server-rendered Pug with Bootstrap 5.3 and Sass.

- **+** Local, passkey and eight OAuth 2.0 providers already wired up
- **+** Account flows included: email verification, password reset, 2FA, account deletion
- **+** Many API integration examples: Stripe, Twilio, Google Drive, Maps, Steam
- **+** Live demo and a production checklist (PROD_CHECKLIST.md)
- **−** Requires MongoDB; no other database option is documented
- **−** No Dockerfile or compose file detected
- **−** AI examples are a small part of a general web boilerplate
- **−** Most integrations need separate API keys and OAuth app setup

<sub>JavaScript, LangChain, Groq, Hugging Face, GPT-OSS · Needs MongoDB, Node.js LTS 24, SMTP provider · env example file · sign-in: Passport · [Repo](https://github.com/sahat/hackathon-starter) · [▶️ Demo ↗](https://hackathon-starter-1.ydftech.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hackathon-starter/)</sub>

<a name="gin-vue-admin"></a>
### #&#8288;27 [gin-vue-admin](https://github.com/flipped-aurora/gin-vue-admin) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Nov 2026</sub>

**Go and Vue 3 admin panel with Casbin permissions and a CRUD code generator.**

Gin-vue-admin is a separated frontend/backend admin platform built on Gin, GORM and Vue 3 with Element Plus. It ships JWT login, Casbin role, API and menu permissions, dynamic menus, a form builder and a code generator that produces CRUD code for both sides. The README also mentions an MCP integration that lets AI editors drive the generator.

- **+** Code generator produces backend and frontend CRUD code, with MCP support for AI editors
- **+** Casbin-based role, API and menu permissions with dynamic routes included
- **+** Swagger API docs generated with swag, served at /swagger/index.html
- **+** Public demo site, online docs and a plugin marketplace
- **−** AI is a side feature; the core is a conventional admin framework
- **−** Requires working knowledge of Go and Vue, per the README
- **−** Some features and official support need a paid commercial license
- **−** README says no free technical support; docs are mainly Chinese

<sub>Go · Needs MySQL or MariaDB 5.7+, Redis, Go >= 1.26.10, Node > 18.16.0 · Docker · [Repo](https://github.com/flipped-aurora/gin-vue-admin) · [▶️ Demo ↗](http://demo.gin-vue-admin.com) · [📖 Docs ↗](https://www.gin-vue-admin.com/guide/start-quickly/initialization.html) · [🌐 Site ↗](https://www.gin-vue-admin.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gin-vue-admin/)</sub>

<a name="open-saas"></a>
### #&#8288;28 [open-saas](https://github.com/wasp-lang/open-saas) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

**Wasp-based SaaS starter with auth, payments, jobs, and an OpenAI example.**

Open SaaS is a full-stack SaaS template built on the Wasp framework (React, Node.js, Prisma). It ships with email and social auth, Stripe, Polar.sh or Lemon Squeezy payments, S3 file uploads, background jobs, an admin dashboard, an OpenAI function-calling example, and an Astro Starlight docs and blog site. It also includes plugins, skills and rules for AI coding tools such as Claude Code and Cursor.

- **+** Auth, payments, email, S3 uploads, and admin dashboard are wired in
- **+** Offers three payment providers: Stripe, Polar.sh, Lemon Squeezy
- **+** Includes Playwright end-to-end tests and ESLint/Prettier CI checks
- **+** MIT license; scaffolded with one command: wasp new -t saas
- **−** Tied to the Wasp framework, so apps inherit its conventions and config
- **−** AI features are limited to one OpenAI function-calling example
- **−** Needs several third-party accounts (payments, email, S3, analytics) for full use
- **−** README states some SaaS features are still missing

<sub>MDX, OpenAI API · Needs Wasp CLI, Node.js, Prisma database, Stripe, Polar.sh or Lemon Squeezy, OpenAI API, AWS S3, SendGrid, Mailgun or SMTP · [Repo](https://github.com/wasp-lang/open-saas) · [▶️ Demo ↗](https://opensaas.sh) · [📖 Docs ↗](https://docs.opensaas.sh) · [🌐 Site ↗](https://opensaas.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-saas/)</sub>

<a name="dotnet-starter-kit"></a>
### #&#8288;29 [dotnet-starter-kit](https://github.com/fullstackhero/dotnet-starter-kit) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · MIT · Nov 2026</sub>

**.NET 10 multi-tenant SaaS starter with two React 19 front-ends.**

A modular .NET 10 monolith using vertical slices, Mediator CQRS, EF Core on PostgreSQL and Finbuckle multitenancy. It ships Identity, Billing, Files, Webhooks, Auditing, Chat and other modules, plus admin and tenant React 19 apps. The fsh CLI or dotnet new scaffolds the full source, and .NET Aspire starts the stack locally.

- **+** Full source scaffolded with project references, no hidden runtime NuGet packages
- **+** Multitenancy, JWT/Identity auth, billing, auditing and webhooks already wired in
- **+** 1,600+ backend tests and 200+ Playwright E2E tests, with NetArchTest boundary checks
- **+** Docker Compose and AWS Terraform deployment included
- **−** No AI or LLM features described in the README
- **−** PostgreSQL only; other databases are not mentioned
- **−** Local stack needs .NET 10 SDK, Docker and Node 20+
- **−** Many modules to learn and trim before it fits a smaller product

<sub>C# · Needs PostgreSQL, Valkey, RustFS (S3-compatible storage), .NET 10 SDK, Docker, Node 20+ · GitHub template · [Repo](https://github.com/fullstackhero/dotnet-starter-kit) · [📖 Docs ↗](https://fullstackhero.net/docs/getting-started/introduction/) · [🌐 Site ↗](https://fullstackhero.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dotnet-starter-kit/)</sub>

<a name="laravel-starter"></a>
### #&#8288;30 [laravel-starter](https://github.com/nasirkhan/laravel-starter) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · GPL-3.0 · Nov 2026</sub>

**Modular Laravel 13 starter with auth, roles, admin backend and posts module.**

Laravel Starter is a Laravel 13.x project template with authentication, social login (Google, Facebook, GitHub), user and role-permission management, and a separate admin backend and public frontend. Features are split into modules, with an Article module (posts, categories, tags, comments) included and a `module:build` command to scaffold new ones. It also includes backup, a log viewer and Tailwind CSS v4 themes. It has no built-in AI features.

- **+** Ships auth, social login, roles/permissions, settings, backup and log viewer out of the box
- **+** Modules are reusable across starter-based projects; `module:build` scaffolds new ones
- **+** Interactive `starter:install` wizard handles .env, database, migrations, seeding and npm build
- **+** Live demo available, plus Laravel Sail setup for Docker
- **−** No AI or model integration, despite this list's focus
- **−** No billing or payments wired in
- **−** GPL-3.0 license constrains closed-source derivatives

<sub>PHP · Needs PHP, Composer, Node.js/npm, SQL database · GitHub template · env example file · [Repo](https://github.com/nasirkhan/laravel-starter) · [▶️ Demo ↗](https://laravel.nasirkhn.com) · [📖 Docs ↗](https://github.com/nasirkhan/laravel-starter/wiki/Installation) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/laravel-starter/)</sub>

<a name="react-starter-kit"></a>
### #&#8288;31 [react-starter-kit](https://github.com/kriasoft/react-starter-kit) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (82) · Freshness: recent (70) · Maintenance: fair (55) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

**Full-stack SaaS monorepo template on React 19, tRPC and Cloudflare Workers.**

A GitHub template for SaaS apps split into three Cloudflare Workers (Astro marketing site, React 19 SPA, Hono and tRPC API) joined by service bindings. Better Auth handles email OTP, passkeys, Google OAuth and organizations, with optional Stripe subscriptions. Drizzle ORM talks to Neon PostgreSQL through Hyperdrive, provisioned with Terraform.

- **+** Auth, organizations and Stripe billing are already wired in
- **+** One TypeScript type contract from Drizzle schema through tRPC to the React UI
- **+** Separate migrate and deploy scripts for staging and production, same script in CI
- **+** A merge-seed skill pulls upstream template changes into your project
- **−** Tied to Cloudflare Workers, Neon PostgreSQL and Hyperdrive; no alternative runtime documented
- **−** Requires Bun 1.4+ instead of Node.js and npm
- **−** README describes no built-in AI features; they must be added yourself
- **−** Email OTP sign-in needs a verified Resend domain for users other than you

<sub>TypeScript · Needs Cloudflare Workers, Neon PostgreSQL, Bun, Resend, Stripe (optional), Terraform · GitHub template · ⚠️ .env file committed · [Repo](https://github.com/kriasoft/react-starter-kit) · [📖 Docs ↗](https://reactstarter.com/getting-started/) · [🌐 Site ↗](https://reactstarter.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-starter-kit/)</sub>

<a name="cosscom-ui"></a>
### #&#8288;32 [ui](https://github.com/cosscom/ui) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**React component library on Base UI and Tailwind, copied into your project.**

coss ui is the Cal.com design system: accessible React components built on Base UI primitives and styled with Tailwind CSS, distributed in the copy-and-own style of shadcn/ui. The repo is a Turborepo monorepo with the marketing site, the component docs (Fumadocs), and a legacy Radix-based Origin UI snapshot. It contains no AI features, so it fits this list only as a UI base for app starters.

- **+** Built on Base UI primitives, with Tailwind styling and TypeScript throughout
- **+** Copy-and-own model: components live in your codebase, not behind a package API
- **+** Used as the design system for cal.com, so it has a production consumer
- **+** MIT license covers the whole repository, including the legacy Origin UI components
- **−** No AI, model or chat functionality; it is a UI kit only
- **−** Origin UI components are a legacy snapshot with limited maintenance
- **−** No tagged release; the repo has no versioned package releases
- **−** Monorepo setup needs three .env.local files to make cross-app links work

<sub>TypeScript · Needs Base UI, Tailwind CSS, Next.js, Bun, Turborepo · [Repo](https://github.com/cosscom/ui) · [🌐 Site ↗](https://coss.com/ui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cosscom-ui/)</sub>

<a name="uni-app"></a>
### #&#8288;33 [uni-app](https://github.com/dcloudio/uni-app) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · Apache-2.0 · Nov 2026</sub>

**Vue framework that builds app, web and mini-program clients from one codebase.**

uni-app is a Vue.js framework that compiles one codebase to iOS, Android, HarmonyOS, responsive web, mini-programs (WeChat, Alipay, Baidu, Douyin and others) and quick apps. This branch is uni-app x, which renders natively on app platforms and supports js, ts and uts. uts is a TypeScript-like language compiled to Kotlin, Swift, ArkTS or js, used mainly for native plugins.

- **+** One Vue codebase targets app, web and over ten mini-program platforms
- **+** uni-app x renders natively on Android, iOS and HarmonyOS
- **+** uts compiles to Kotlin, Swift, ArkTS or js for native plugin work
- **+** Repo includes examples, tests and per-platform benchmark reports
- **−** Not an AI product; AI support is a separate uni-agent tool and training CLI
- **−** README and docs are primarily in Chinese
- **−** Performance claims (2-4x native) come from the vendor's own benchmarks
- **−** Main branch is uni-app x; Vue 2 and Vue 3 versions are on other branches

<sub>JavaScript · [Repo](https://github.com/dcloudio/uni-app) · [📖 Docs ↗](https://doc.dcloud.net.cn/uni-app-x/ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/uni-app/)</sub>

<a name="exact"></a>
### #&#8288;34 [exact](https://github.com/expo/exact) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Nov 2026</sub>

**Cross-platform app runtime with a declarative UI language and agent test driver.**

Exact compiles UI written in Contract, a small declarative language, into a plan that runs as DOM on the web and as AppKit, UIKit or GPU-painted views on macOS, iOS and Linux, with no webview. Data logic is TypeScript on Hermes or Rust. A ten-operation driver, scripts/agent.mjs, lets a coding agent build, screenshot, tap and test an app on every host. Pre-1.0 with no API stability.

- **+** One app.contract renders natively on web, macOS, iOS and Linux without a webview
- **+** Same ten driver operations and app.test.contract files run unchanged on every host
- **+** Agent-controlled clock and machine-readable diagnostics make tests deterministic
- **+** Reports 99 ms dev rebuilds and a ~20 KB web runtime, measured by the authors
- **−** Pre-1.0 and changes daily; no API stability or migration guide by design
- **−** Native hosts need macOS with Xcode 27.1+; first native build takes 10-15 minutes
- **−** UI must be written in Contract, a new language with little outside tooling
- **−** TypeScript on native hosts requires installing a pinned Hermes bundle separately

<sub>Rust · Needs Rust (rustup), Bun 1.4.2, Google Chrome, Xcode 27.1+, Hermes bundle · [Repo](https://github.com/expo/exact) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/exact/)</sub>

<a name="next-saas-stripe-starter"></a>
### #&#8288;35 [next-saas-stripe-starter](https://github.com/mickasmt/next-saas-stripe-starter) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Sep 2026</sub>

**Next.js SaaS starter with Better Auth, Drizzle, Neon and Stripe billing.**

Next.js 16 SaaS boilerplate with Google sign-in via Better Auth, Neon Postgres through Drizzle, and Stripe Checkout, customer portal and webhooks. Auth, billing, admin, docs, blog and changelog are modules toggled in config/features.ts, and `pnpm modules:prune` deletes the ones you don't want. Teams, seat billing, onboarding and emails are only in a paid Pro version.

- **+** Each module is a feature flag; disabled routes 404 and endpoints are refused
- **+** `pnpm modules:prune` lists and deletes a module's routes, components and packages
- **+** Stripe Checkout, customer portal and webhooks included, with plan prices read from Stripe
- **+** MDX docs, blog and changelog via Fumadocs, plus admin panel in the free version
- **−** Teams, seat billing, onboarding and Resend emails are Pro only ($99-$149)
- **−** Google is the only sign-in provider listed
- **−** Requires Neon Postgres and Stripe accounts for auth and billing modules
- **−** No AI features described in the README despite the list context

<sub>TypeScript · Needs Neon Postgres, Stripe, Google OAuth · env example file · sign-in: Better Auth · [Repo](https://github.com/mickasmt/next-saas-stripe-starter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-saas-stripe-starter/)</sub>

<a name="open-mercato"></a>
### #&#8288;36 [open-mercato](https://github.com/open-mercato/open-mercato) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2026</sub>

**Next.js and PostgreSQL framework with prebuilt CRM, sales and warehouse modules.**

Open Mercato is a TypeScript framework on Next.js and PostgreSQL that scaffolds a business back office with modules for customers, catalog, sales, warehouse, portal and workflows. Each generated app ships an AGENTS.md, skills and specs in .ai/specs/ so Claude Code, Codex or Cursor know where new modules belong. Cezar, a separate MIT orchestrator, can run those agent tasks unattended.

- **+** Scaffolds via npx create-mercato-app with classic, crm, wms and empty presets
- **+** Ships AGENTS.md and om-* skills that route agents to the right code location
- **+** Specs in .ai/specs/ drive a plan, approve, implement flow with tests
- **+** Core is MIT with no per-seat licence; REST API docs served under /backend/docs
- **−** Enterprise modules are licensed separately from the MIT core
- **−** Setup needs Node.js 24, Yarn 4 and Docker; Windows requires WSL2
- **−** Dev server serves scripts to localhost only, not 127.0.0.1 or other hosts
- **−** Fresh 0.8.0 apps report typecheck errors in agent_examples until next release

<sub>TypeScript, Claude Code, Codex, Cursor, GitHub Copilot (experimental) · Needs Node.js 24, Yarn 4, Docker, PostgreSQL 17 with pgvector, Redis 7, Meilisearch · Docker · [Repo](https://github.com/open-mercato/open-mercato) · [📖 Docs ↗](https://docs.openmercato.com/) · [🌐 Site ↗](https://openmercatocloud.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-mercato/)</sub>

<a name="dub-link"></a>
### #&#8288;37 [dub.link](https://github.com/dubinc/dub.link) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Oct 2026</sub>

**Link shortener with click analytics and conversion tracking, built on Next.js.**

Dub Links is a link attribution platform for short links and conversion tracking. It is a Turborepo monorepo in TypeScript using Next.js, Prisma, NextAuth.js, Stripe and Tinybird analytics. Most of the code is AGPLv3, and a small /ee directory needs a commercial license. A self-hosting guide is on the docs site.

- **+** Full product stack with auth, SAML/SSO via BoxyHQ, Stripe payments and email wired in
- **+** README reports 250M+ clicks and 12M+ links per month on the hosted service
- **+** Core is AGPLv3, with a self-hosting guide and a local development guide
- **+** Dev seed script with an optional confirmed truncate for local testing
- **−** Needs several external services: Upstash, Tinybird, PlanetScale, Stripe and Resend
- **−** The /ee directory is under a commercial license, so enterprise features are not open source
- **−** No AI features described, so it fits this list only as an app starter
- **−** No Docker or compose files detected, and the stack targets Vercel deployment

<sub>TypeScript · Needs Upstash Redis, Tinybird, PlanetScale, Stripe, Resend, BoxyHQ SAML/SSO, Node v23.11.0, pnpm 9.15.9 · [Repo](https://github.com/dubinc/dub.link) · [📖 Docs ↗](https://dub.co/docs/self-hosting/guide) · [🌐 Site ↗](https://dub.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dub-link/)</sub>

<a name="vue-admin-better"></a>
### #&#8288;38 [vue-admin-better](https://github.com/zxwk1998/vue-admin-better) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

**Vue 2 and Element UI admin dashboard template with RBAC and JWT.**

Front-end admin template built on Vue 2 and Element UI, with 40+ example pages, RBAC with JWT permission control, and routes that can be rendered from a backend. Builds run on Rspack (`npm run serve:rspack`). It has no AI features; the Vue 3 Element Plus and Arco Design variants live in separate repos.

- **+** Route permissions can be controlled from the front end or from the backend
- **+** Includes mock auto-generation, RSA-encrypted login, error log capture and theme/layout switching
- **+** MIT license, and the README states free commercial use
- **+** Responsive across PC, tablet and phone, with live demos
- **−** No AI or LLM functionality; it is a generic admin UI template
- **−** Targets Vue 2 and Element UI; Vue 3 versions are in separate repos
- **−** Front end only: no backend, database or billing included
- **−** README is in Chinese, and some variants are paid commercial editions

<sub>Vue · Needs Node.js, pnpm · [Repo](https://github.com/zxwk1998/vue-admin-better) · [▶️ Demo ↗](https://zxwk1998.github.io/vue-admin-better/) · [🌐 Site ↗](https://vuejs-core.cn/vue-admin-better) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vue-admin-better/)</sub>

<a name="ng-alain"></a>
### #&#8288;39 [ng-alain](https://github.com/ng-alain/ng-alain) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

**Angular admin UI scaffold built on ng-zorro-antd and the @delon component packages.**

NG-ALAIN is an Angular starter for enterprise admin applications, built on ng-zorro-antd (Ant Design) and the companion @delon business component packages. It provides a responsive layout, i18n, RTL, theming with Less and lazy-loaded assets. It has no AI features; it fits this list only as a generic app starter.

- **+** Built on ng-zorro-antd with @delon admin business components included
- **+** Ships i18n, RTL, responsive layout and customizable Less themes
- **+** MIT licensed with a release and commit on 2026-10-29
- **−** No AI functionality, so it is not an AI starter
- **−** Frontend only; no backend, auth service, billing or database included
- **−** Angular and Less stack only; no other framework support
- **−** Business theme is sold separately

<sub>TypeScript · Needs ng-zorro-antd, @delon · [Repo](https://github.com/ng-alain/ng-alain) · [▶️ Demo ↗](https://ng-alain.surge.sh) · [📖 Docs ↗](https://ng-alain.com/docs/getting-started) · [🌐 Site ↗](https://ng-alain.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ng-alain/)</sub>

<a name="basic"></a>
### #&#8288;40 [basic](https://github.com/fantastic-admin/basic) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Vue 3 admin dashboard framework with themes, menu modes and permission control.**

Fantastic-admin is the basic edition of a Vue 3 admin-panel framework built on Vite, Pinia, UnoCSS, VueUse and TypeScript. It ships 18 themes, 7 navigation menu modes, page keep-alive control, permission checks, i18n with RTL support and 19 extension slots, and includes Skills for AI coding agents. Some listed features belong to the paid professional edition.

- **+** Includes bundled Skills so coding agents can work on the codebase
- **+** Lets you choose your own third-party UI library
- **+** 18 themes, 7 menu modes, i18n and RTL support
- **+** 19 reserved slots for extending layout content
- **−** Some listed features are professional-edition only; README does not say which
- **−** README is mainly in Chinese
- **−** No AI model integration, backend, auth server or billing included
- **−** Main branch may contain unreleased changes; releases are recommended

<sub>Vue · Needs Node.js · GitHub template · [Repo](https://github.com/fantastic-admin/basic) · [🌐 Site ↗](https://fantastic-admin.hurui.me) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/basic/)</sub>

<a name="yournextstore"></a>
### #&#8288;41 [yournextstore](https://github.com/yournextstore/yournextstore) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (52) · Freshness: active (91) · Maintenance: fair (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Nov 2026</sub>

**Next.js 16 storefront template backed by the Your Next Store API and Stripe.**

A Next.js 16 e-commerce storefront using App Router, Tailwind v4 and Shadcn UI, with products, carts and checkout served through the Commerce Kit SDK against a YNS API key. It ships an AGENTS.md with SDK examples and Biome rules so coding agents like Claude Code, Cursor and Codex can edit it. 149 visual themes live on separate git branches.

- **+** AGENTS.md documents SDK methods, patterns and a validation checklist for coding agents
- **+** 149 theme branches change visuals only; products, cart and checkout stay the same
- **+** Typed Commerce Kit SDK (productBrowse, cartUpsert) covers products, carts and checkout
- **+** Live demo and one-click Vercel deploy are provided
- **−** Requires a YNS_API_KEY from the yns.store platform; not standalone
- **−** Template updates need the platform's Upgrade button or script, not git merge
- **−** Needs Node.js 24+ and Bun; no Docker or compose files
- **−** AI is only a development aid; no AI features in the storefront itself

<sub>TypeScript · Needs YNS API (yns.store), Stripe, Node.js 24+, Bun 1.0+ · GitHub template · env example file · [Repo](https://github.com/yournextstore/yournextstore) · [▶️ Demo ↗](https://demo.yournextstore.com) · [🌐 Site ↗](https://yournextstore.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yournextstore/)</sub>

<a name="cleanarchitecture"></a>
### #&#8288;42 [cleanarchitecture](https://github.com/jasontaylordev/cleanarchitecture) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (79) · Freshness: active (95) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Nov 2026</sub>

**ASP.NET Core solution template using Clean Architecture with Angular or React.**

A .NET template, installed with `dotnet new install`, that scaffolds a Clean Architecture solution on ASP.NET Core 10, EF Core 10 and Aspire. You pick an Angular 21 or React 19 client, or a Web API only, and SQLite, PostgreSQL or SQL Server. It has no AI features; it is a general enterprise app starter.

- **+** Angular, React or API-only, and three database providers, chosen by CLI flags
- **+** SQLite default needs no container runtime to run locally
- **+** Includes MediatR, FluentValidation, NUnit and Respawn test setup, plus ADRs
- **+** Older .NET versions kept on branches back to .NET Core 3.1
- **−** No AI functionality; it is a generic .NET starter
- **−** Relies on MediatR and AutoMapper, which add dependencies and indirection
- **−** Requires .NET 10 SDK; Node.js needed for the frontends
- **−** Auth and billing support are not described in the README

<sub>C# · Needs .NET 10 SDK, Node.js (Angular/React only), Docker or Podman (PostgreSQL/SQL Server only), Aspire · [Repo](https://github.com/jasontaylordev/cleanarchitecture) · [📖 Docs ↗](https://cleanarchitecture.jasontaylor.dev/docs/getting-started/) · [🌐 Site ↗](https://cleanarchitecture.jasontaylor.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cleanarchitecture/)</sub>

<a name="next-shadcn-admin-dashboard"></a>
### #&#8288;43 [next-shadcn-admin-dashboard](https://github.com/arhamkhnz/next-shadcn-admin-dashboard) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Nov 2026</sub>

**Next.js 16 admin dashboard template with shadcn/ui and theme presets.**

Admin dashboard template built on Next.js 16 (App Router), TypeScript, Tailwind CSS v4 and shadcn/ui. It includes prebuilt dashboards (CRM, Finance, Analytics, E-commerce, Logistics and others), four authentication screens, and pages such as Kanban, Calendar, Chat and Users. Theme presets and layout options like a collapsible sidebar are included.

- **+** Many prebuilt dashboards and pages: CRM, Finance, Kanban, Calendar, Invoice, Users, Roles
- **+** Light/dark modes with color presets such as Tangerine, Neo Brutalism and Soft Pop
- **+** Colocated per-route file structure; Biome and Husky preconfigured
- **+** Live demo available; archive branches for Next.js 15 and Next.js 14
- **−** RBAC with multi-tenant support is marked as planned, not implemented
- **−** Only authentication screens; no database or billing wiring mentioned
- **−** Frequent updates may include breaking changes for forks
- **−** No AI features; it is a UI template only

<sub>TypeScript · Needs Node.js, npm · [Repo](https://github.com/arhamkhnz/next-shadcn-admin-dashboard) · [▶️ Demo ↗](https://studio-admin.arhamkhnz.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-shadcn-admin-dashboard/)</sub>

<a name="refine"></a>
### #&#8288;44 [refine](https://github.com/refinedev/refine) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (91) · Freshness: active (96) · Maintenance: weak (24) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Sep 2026</sub>

**Headless React framework for admin panels, dashboards and internal tools.**

Refine Core is a React meta-framework that supplies hooks and components for the CRUD parts of an app: authentication, access control, routing, data fetching, state via React Query, and i18n. It is headless, so UI is your own or one of the built-in integrations (Ant Design, Material UI, Mantine, Chakra UI). Data providers cover 15+ backends, including REST, GraphQL, Supabase, Strapi and Firebase.

- **+** Headless design works with Tailwind or any custom UI, plus Ant Design, MUI, Mantine, Chakra
- **+** Data provider connectors for 15+ backends including REST, GraphQL, Supabase, Hasura, Firebase
- **+** Works with Next.js, Remix, React Native and Electron through a router interface
- **+** Built-in auth, access control, live updates, audit logs and i18n hooks
- **−** Not an AI project: AI features are only in a separate hosted Refine agent
- **−** React and TypeScript only; no support for other frontend frameworks
- **−** Not a backend or boilerplate; you supply the API and database
- **−** Last tagged release is 2026-04-02, months behind recent commits

<sub>TypeScript · Needs Node.js, React, a backend API (REST, GraphQL, Supabase, etc.) · [Repo](https://github.com/refinedev/refine) · [▶️ Demo ↗](https://refine.dev/core/?playground=true) · [📖 Docs ↗](https://refine.dev/core/docs/) · [🌐 Site ↗](https://refine.dev/core/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/refine/)</sub>

<a name="semi-design"></a>
### #&#8288;45 [semi-design](https://github.com/douyinfe/semi-design) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (66) · Freshness: active (85) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · custom license · Nov 2026</sub>

**React UI component library with Figma design-to-code and theming tokens.**

Semi UI (@douyinfe/semi-ui) is a React component library from ByteDance's Douyin front-end team with 80+ components, written in TypeScript. It ships a Figma plugin that exports JSX with SCSS, Emotion or Tailwind, and a design system manager (DSM) exposing 3000+ design tokens for theming. It is not an AI project; it fits this list only loosely as a UI starter dependency.

- **+** 80+ components with TypeScript types, SSR compatibility and dark mode
- **+** Figma plugin converts designs to JSX with SCSS, Emotion or Tailwind
- **+** 3000+ design tokens and DSM for theming and keeping Figma and code in sync
- **+** Tested with unit, Cypress E2E and Chromatic visual tests; a11y and RTL support
- **−** React only; no AI, chat or model features included
- **−** Not a starter app: no auth, billing or database wiring
- **−** Last release 2025-11-18, nearly a year before the latest commit
- **−** Some blog and community links are Chinese-language or Feishu-only

<sub>TypeScript · Needs React · [Repo](https://github.com/douyinfe/semi-design) · [📖 Docs ↗](https://semi.design/en-US/start/getting-started) · [🌐 Site ↗](https://semi.design/en-US/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/semi-design/)</sub>

<a name="angular-realworld-example-app"></a>
### #&#8288;46 [angular-realworld-example-app](https://github.com/realworld-apps/angular-realworld-example-app) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.7k · custom license · Nov 2026</sub>

**Angular front end for the RealWorld "Conduit" blogging app.**

A Medium-style blogging front end ("Conduit") written in Angular and TypeScript that follows the RealWorld spec. It covers JWT login and signup, article CRUD, comments, favorites, follows, tags and paginated feeds against a separate backend API. It has no AI features; it is a reference app for structuring an Angular client.

- **+** Covers auth, CRUD, routing and pagination in one small Angular codebase
- **+** Follows the Angular style guide and the shared RealWorld API spec
- **+** Live demo available at demo.realworld.show
- **+** Works with RealWorld-compatible backends, so the API server can be swapped
- **−** No AI or model integration despite the list's theme
- **−** Front end only; needs a separate RealWorld backend to run
- **−** README says it may be too simple for complex Angular patterns
- **−** Setup needs Bun and a git submodule for the spec

<sub>TypeScript · Needs Bun, RealWorld-compatible backend API · [Repo](https://github.com/realworld-apps/angular-realworld-example-app) · [▶️ Demo ↗](https://demo.realworld.show) · [📖 Docs ↗](https://docs.realworld.show/introduction/) · [🌐 Site ↗](https://realworld.show) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/angular-realworld-example-app/)</sub>

<a name="adminator-admin-dashboard"></a>
### #&#8288;47 [adminator-admin-dashboard](https://github.com/puikinsh/adminator-admin-dashboard) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (46) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

**Vanilla-JS admin dashboard template with CSS-variable theming and dark mode.**

Adminator 4 is a static admin dashboard template with 18 pages (dashboard, email, calendar, chat, data table, auth, error pages). It uses no jQuery or Bootstrap: one SCSS token system drives light and dark themes, and a single Shell.js renders the sidebar, topbar and footer. It contains no AI features and no backend, auth logic or billing.

- **+** No jQuery or Bootstrap; v4.2.0 ships 130 KB JS+CSS on every page
- **+** Dark mode via one data-theme attribute; Chart.js, FullCalendar, jsvectormap re-render
- **+** Nav items live in one NAV array in Shell.js, so adding a page is four steps
- **+** MIT license; also published on npm with prebuilt dist/ and served via jsDelivr
- **−** Front-end only: no backend, database, real auth or billing, only demo pages
- **−** No AI functionality, so it fits this list only loosely
- **−** v4 is a rewrite; v3 users must migrate or stay on the legacy-v3 branch
- **−** README promotes paid DashboardPack templates for advanced features and support

<sub>HTML · Needs Node.js 22.22.2+, npm 10+ · [Repo](https://github.com/puikinsh/adminator-admin-dashboard) · [▶️ Demo ↗](https://preview.colorlib.com/theme/adminator/index.html) · [📖 Docs ↗](https://adminator.colorlib.com/docs/) · [🌐 Site ↗](https://adminator.colorlib.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/adminator-admin-dashboard/)</sub>

<a name="saas-boilerplate"></a>
### #&#8288;48 [saas-boilerplate](https://github.com/ixartz/saas-boilerplate) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Aug 2026</sub>

**Next.js SaaS starter with Clerk auth, teams, roles and Drizzle ORM.**

Next.js 16 and React 19 template with Tailwind CSS 4 and Shadcn UI. It includes a landing page, user dashboard, Clerk authentication with multi-tenancy, team invites and role-based access, and Drizzle ORM on PostgreSQL (PGlite locally, Neon suggested for production). Also ships next-intl i18n, Sentry, Vitest and Playwright tests. The README lists no built-in AI features.

- **+** Multi-tenancy, team invites and RBAC included in the free MIT version
- **+** Local dev runs on PGlite, so no external database is needed to start
- **+** Testing setup covers Vitest, Playwright, Storybook and visual regression, with GitHub Actions CI
- **+** Includes a saas-builder skill for Codex and Claude Code to scaffold from the repo
- **−** Authentication depends on Clerk, a hosted third-party service with its own keys
- **−** Stripe billing, dark mode and oRPC are only in paid Plus/Pro/Max versions
- **−** No AI features built in; the README documents none
- **−** Requires Node.js 24+, which may be newer than some environments

<sub>TypeScript · Needs Clerk, PostgreSQL (Neon suggested; PGlite for local dev), Sentry, Crowdin · GitHub template · ⚠️ .env file committed · sign-in: Clerk · [Repo](https://github.com/ixartz/saas-boilerplate) · [▶️ Demo ↗](https://react-saas.com) · [🌐 Site ↗](https://react-saas.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/saas-boilerplate/)</sub>

<a name="velobase-harness"></a>
### #&#8288;49 [velobase-harness](https://github.com/velobase/velobase-harness) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 623 · MIT · Oct 2026</sub>

**Next.js AI SaaS boilerplate with credits, payments, workers and anti-abuse.**

Next.js 15 and TypeScript starter that adds the monetization layer an AI app needs: credit ledger, subscriptions, Stripe and NowPayments, BullMQ workers, and an admin area. It also includes multi-LLM chat, affiliate and referral tracking, server-side ad attribution, and free-credit abuse controls such as Turnstile and rate limits. Runs on PostgreSQL and Redis, with an optional Hono API service.

- **+** Credit ledger, orders, subscriptions and promo codes included, not just auth and a checkout page
- **+** Anti-abuse controls: Turnstile, disposable-email checks, guest quotas, credit clawbacks
- **+** Web, BullMQ worker and optional Hono API run as one process or split services
- **+** Local start needs no external accounts; seeded admin sign-in via pnpm dev:local
- **−** Requires PostgreSQL and Redis even for local development
- **−** Payment docs cover only Stripe and NowPayments
- **−** No general unit-test script; only service-mode smoke tests
- **−** Real model calls, payments and email need your own provider connections

<sub>TypeScript, multi-LLM chat (providers unknown) · Needs PostgreSQL 16, Redis 7, Docker, Node.js, pnpm, Stripe, NowPayments · GitHub template · Docker · env example file · sign-in: Auth.js · [Repo](https://github.com/velobase/velobase-harness) · [📖 Docs ↗](https://github.com/velobase/velobase-harness/blob/main/docs/en/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/velobase-harness/)</sub>

<a name="html5-boilerplate"></a>
### #&#8288;50 [html5-boilerplate](https://github.com/h5bp/html5-boilerplate) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: widely used (97) · Freshness: recent (70) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · MIT · Nov 2026</sub>

**Plain HTML, CSS and JS starter template for websites and web apps.**

Front-end starter template with Open Graph placeholders, CSS helper classes, media query placeholders and print styles. It also includes an example package.json with WebPack commands. It imposes no framework, and the published artifact is the dist/ folder, available via npx, npm, a template repo or a zip. It has no AI functionality.

- **+** No framework imposed; delete-key friendly, so unused parts are easy to strip out
- **+** Several install paths: npx create script, GitHub template repo, npm package, zip
- **+** Documentation is bundled with the project for offline reading
- **+** MIT license, with more than 10 years of iterative development
- **−** No AI features, auth, billing or database; static front-end files only
- **−** Last tagged release is v9.0.0 from April 2024
- **−** Cloning this repo is not the intended use; only dist/ is the product
- **−** Build setup relies on WebPack commands and has no component model

<sub>JavaScript · Needs Node.js, npm · [Repo](https://github.com/h5bp/html5-boilerplate) · [🌐 Site ↗](https://html5boilerplate.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/html5-boilerplate/)</sub>

<a name="pagoda"></a>
### #&#8288;51 [pagoda](https://github.com/mikestefanello/pagoda) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**Go full-stack web starter with Echo, Ent, HTMX and SQLite.**

Pagoda is a starter kit, not a framework, for server-rendered web apps in Go. It wires together Echo, Ent ORM, Gomponents, HTMX, Alpine.js and DaisyUI, and includes sessions, authentication, an admin panel generated from Ent schemas, background task queues, cron, a cache, file uploads and email. Data and task queues live in SQLite by default. It has no AI features.

- **+** SQLite handles storage and persistent task queues, so no Postgres or Redis is needed
- **+** Auth, sessions, admin panel, tasks, cron, cache and email are included in one codebase
- **+** You own the code; Echo, Ent and the frontend libraries can each be swapped out
- **+** Admin panel is generated from Ent schemas, so new entity types appear in the UI
- **−** No AI or LLM features; it is a generic web starter
- **−** Removing Ent also removes the generated admin panel
- **−** Default cache is in-memory; the Postgres and Redis branch is no longer maintained
- **−** Session encryption key default must be changed manually for live environments

<sub>Go · Needs Go, SQLite, Tailwind CLI (optional), Air (optional) · GitHub template · [Repo](https://github.com/mikestefanello/pagoda) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pagoda/)</sub>

<a name="coreui-free-react-admin-template"></a>
### #&#8288;52 [coreui-free-react-admin-template](https://github.com/coreui/coreui-free-react-admin-template) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Sep 2026</sub>

**React 19 admin dashboard template built on CoreUI components and Vite.**

A free React admin dashboard starter using @coreui/react components, Vite, SCSS and a sidebar/header/footer layout with route and nav config files. It ships context files for AI assistants (.cursorrules, ARCHITECTURE.md, DEVELOPMENT.md) and JSDoc and PropTypes on components. The dev server runs on port 3000; several components and the data grid and scheduler add-ons are paid.

- **+** MIT licensed, with Vite dev server and hot reload on localhost:3000
- **+** Includes .cursorrules, ARCHITECTURE.md and DEVELOPMENT.md to give AI assistants project context
- **+** Layout, routing (routes.js) and sidebar nav (_nav.jsx) are already configured
- **+** Components documented with JSDoc and PropTypes
- **−** No AI features, auth, billing or database; it is a front-end UI shell only
- **−** Many components (Smart Table, date pickers, stepper) require paid CoreUI PRO
- **−** Data Grid and Scheduler are separate paid add-ons
- **−** JavaScript with PropTypes rather than TypeScript

<sub>JavaScript · Needs Node.js, npm or yarn, @coreui/react · [Repo](https://github.com/coreui/coreui-free-react-admin-template) · [📖 Docs ↗](https://coreui.io/react/docs/templates/installation/) · [🌐 Site ↗](https://coreui.io/product/free-react-admin-template/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coreui-free-react-admin-template/)</sub>

<a name="free-nextjs-admin-dashboard"></a>
### #&#8288;53 [free-nextjs-admin-dashboard](https://github.com/tailadmin/free-nextjs-admin-dashboard) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

**Next.js and Tailwind admin dashboard template with charts, tables and auth pages.**

TailAdmin is a free admin dashboard template built on Next.js 16, React 19, TypeScript and Tailwind CSS v4. The free edition ships one dashboard, 30+ dashboard components and 50+ UI elements, including sidebar, tables, ApexCharts charts, auth forms and dark mode. It is a UI starter with no AI or backend logic described beyond an AI settings page and AI dashboard in the changelog.

- **+** Current stack: Next.js 16, React 19, Tailwind CSS v4, TypeScript
- **+** MIT license; free edition has 30+ components and 50+ UI elements
- **+** Dark mode, RTL and multi-language support as of v2.4.0
- **+** Includes AGENTS.md for working with AI coding agents
- **−** Free edition has only 1 dashboard; others are in the paid Pro version
- **−** No database, billing or backend wiring described in the README
- **−** Figma files in free edition are basic; complete set is Pro only
- **−** Community support only on free; email support is Pro

<sub>TypeScript · Needs Node.js 20+ · [Repo](https://github.com/tailadmin/free-nextjs-admin-dashboard) · [▶️ Demo ↗](https://nextjs-free-demo.tailadmin.com) · [📖 Docs ↗](https://tailadmin.com/docs) · [🌐 Site ↗](https://tailadmin.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/free-nextjs-admin-dashboard/)</sub>

<a name="tauri-ui"></a>
### #&#8288;54 [tauri-ui](https://github.com/agmmnn/tauri-ui) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Oct 2026</sub>

**CLI that scaffolds Tauri v2 desktop apps with shadcn/ui and desktop defaults.**

create-tauri-ui runs the official shadcn/ui and create-tauri-app setups, then combines the frontend with the native shell. It applies desktop defaults such as no startup flash, external links opening in the system browser, and no overscroll. Frontend choices are Vite, Next.js, React Router, Astro, or TanStack Start. It has no AI features of its own.

- **+** Wraps upstream shadcn and create-tauri-app CLIs instead of forking templates
- **+** Five frontend adapters: Vite, Next.js, React Router, Astro, TanStack Start
- **+** Add, update or remove batteries later with list/add/update/remove commands
- **+** Dev-only debug panel (Cmd/Ctrl+D) shows routes, invokes, window state and logs
- **−** No AI features, auth, billing or database; only a desktop shell starter
- **−** README examples assume Bun (bunx, bun run)
- **−** Patches upstream CLI output, so it depends on upstream changes
- **−** Showcase list names only one example app

<sub>TypeScript · Needs Bun, Tauri v2 · [Repo](https://github.com/agmmnn/tauri-ui) · [🌐 Site ↗](https://tauriui.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tauri-ui/)</sub>

<a name="shadcn-dashboard-landing-template"></a>
### #&#8288;55 [shadcn-dashboard-landing-template](https://github.com/shadcnstore/shadcn-dashboard-landing-template) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Admin dashboard and landing page template in Vite and Next.js with shadcn/ui.**

Two parallel codebases, one on Vite and one on Next.js 16 App Router, each with two dashboard variants, 30+ pages and a marketing landing page. It uses shadcn/ui on Base UI (base-nova style) with Tailwind CSS v4, and includes mail, tasks, chat, calendar and user-management demo apps plus a live tweakcn-based theme customizer. The apps are UI demos only, with no AI features or backend described.

- **+** Same UI shipped for both Vite and Next.js 16, so you pick your framework
- **+** Includes auth page variants, settings, billing, error pages and a full landing page
- **+** Built-in theme customizer with presets and CSS variable export; removal steps documented
- **+** MIT licensed, with TanStack Table, Recharts, Zustand, React Hook Form and Zod already wired in
- **−** No backend, database or real auth; pages are front-end demos
- **−** No AI features described, so it fits this list only as a UI shell
- **−** 2.0 moved from Radix UI to Base UI; customized 1.x copies need migration
- **−** Two duplicated codebases to keep in sync if you adopt both

<sub>TypeScript · Needs Node.js 20.19+, pnpm or npm · [Repo](https://github.com/shadcnstore/shadcn-dashboard-landing-template) · [▶️ Demo ↗](https://shadcnstore.com/templates/dashboard/shadcn-dashboard-landing-template/dashboard) · [🌐 Site ↗](https://shadcnstore.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shadcn-dashboard-landing-template/)</sub>

<a name="antd-admin"></a>
### #&#8288;56 [antd-admin](https://github.com/zuiidea/antd-admin) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (64) · Freshness: active (95) · Maintenance: weak (20) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · MIT · Oct 2026</sub>

**React admin dashboard templates with JWT login, mock API and Ant Design.**

Antd Admin is a set of admin-panel templates built on React 19, Ant Design 6, TanStack Router/Query, Zustand and Zod, scaffolded with the init-antd-admin CLI. It ships a basic variant and one with Lingui i18n (en and zh). It runs against a mock API with no backend, and includes JWT access/refresh login, backend-driven menus and Playwright E2E tests.

- **+** Runs locally against mocks, so no backend is needed to start
- **+** URL-synced table state for pagination, sorting and search
- **+** Each template has an AGENTS.md for Cursor, Claude Code and Codex
- **+** Playwright E2E tests included
- **−** No AI features; it is a general-purpose admin UI
- **−** No billing or real database layer; backend must be supplied
- **−** Only two templates; i18n covers just English and Chinese
- **−** No live demo link in the README

<sub>TypeScript · [Repo](https://github.com/zuiidea/antd-admin) · [📖 Docs ↗](https://antd-admin-doc.zuiidea.top) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/antd-admin/)</sub>

<a name="aimeos"></a>
### #&#8288;57 [aimeos](https://github.com/aimeos/aimeos) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT · Nov 2026</sub>

**Laravel e-commerce shop with admin backend, JSON API and MCP server.**

Aimeos is a PHP e-commerce application built on Laravel, installed with `composer create-project`. It provides a storefront, an admin backend at `/admin`, a JSON:API REST interface, a GraphQL admin API, and multi-vendor, multi-language and subscription support. AI features are limited to text translation and an MCP server that lets agents like Claude manage products, orders and customers.

- **+** Ships storefront, admin backend, JSON:API and GraphQL admin API in one install
- **+** Built-in MCP endpoint with Sanctum tokens or Passport OAuth for remote clients
- **+** Multi-vendor, multi-language and subscriptions are toggled through `.env` settings
- **+** Runs on MySQL, MariaDB, PostgreSQL or SQL Server; MIT and LGPLv3 licensed
- **−** AI is secondary: MCP server and translation only, not the core of the product
- **−** Multi-routing adds database queries per request and affects performance
- **−** SPA or PWA builds need the separate aimeos-headless distribution
- **−** Install is via composer on a PHP 8.2+ host; no Docker image is mentioned

<sub>JavaScript · Needs PHP >= 8.2, Composer 2.2+, MySQL >= 5.7.8 / MariaDB >= 10.2.2 / PostgreSQL 9.6+ / SQL Server 2019+, Apache or Nginx, Laravel Sanctum (MCP auth), Laravel Passport (optional, OAuth) · env example file · [Repo](https://github.com/aimeos/aimeos) · [▶️ Demo ↗](https://laravel.demo.aimeos.org) · [📖 Docs ↗](https://aimeos.org/docs/latest/laravel) · [🌐 Site ↗](https://aimeos.org/Laravel) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aimeos/)</sub>

<a name="start-ui-web"></a>
### #&#8288;58 [start-ui-web](https://github.com/bearstudio/start-ui-web) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**TanStack Start web app starter with oRPC, Prisma, Better Auth and shadcn/ui.**

Full-stack web starter from BearStudio, scaffolded with `pnpm create start-ui -t web`. It combines TanStack Start, React, Tailwind, shadcn/ui, oRPC, Prisma on PostgreSQL and Better Auth, with Storybook, Vitest and Playwright set up. It has no AI features of its own; it is a general web app boilerplate.

- **+** Auth, Prisma/PostgreSQL, S3-compatible storage and email run locally through a Docker Compose stack
- **+** Includes Storybook, Vitest and Playwright E2E, plus react-email templates with a preview server
- **+** Generates OpenAPI docs for the backend at /api/openapi/app
- **+** Production Dockerfile runs as non-root user on port 3000 with a HEALTHCHECK
- **−** No AI or model integration in the README; it is a generic web starter
- **−** Needs Node.js 22 or newer, pnpm, and Docker or a PostgreSQL database
- **−** Uses the TypeScript 7 native compiler, so editors need a separate extension to match CI

<sub>TypeScript · Needs Node.js >= 22, pnpm, PostgreSQL, Docker, S3-compatible storage, SMTP server · GitHub template · Docker · env example file · sign-in: Better Auth · [Repo](https://github.com/bearstudio/start-ui-web) · [📖 Docs ↗](https://docs.web.start-ui.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/start-ui-web/)</sub>

<a name="cove"></a>
### #&#8288;59 [cove](https://github.com/mugnavo/cove) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Unlicense · Nov 2026</sub>

**TanStack Start starter with Drizzle, Postgres and Better Auth.**

Cove Stack is a TypeScript starter for TanStack Start (React, Router, Query) with Tailwind, shadcn/ui on Base UI, Drizzle ORM on PostgreSQL, and Better Auth. It is scaffolded with `pnpm create cove` or the GitHub template button and builds with Vite Plus and Nitro. The README describes no built-in AI features, so it is a general web app base.

- **+** Auth, Drizzle/Postgres and shadcn/ui pre-wired, with sample auth middleware for server functions
- **+** Nitro presets allow deploying to Netlify, Vercel, Node.js and others
- **+** Typed env validation via Varlock and structured per-request logs via evlog
- **+** Vitest and Playwright test setup included; public domain Unlicense
- **−** No AI or model integration in the README
- **−** No billing or payments setup mentioned
- **−** Relies on pre-release parts: Nitro v3 beta, Drizzle v1 RC, TanStack Devtools alpha
- **−** Needs Node 24+, pnpm 12+, Vite Plus and your own PostgreSQL

<sub>TypeScript · Needs PostgreSQL, Node.js >= 24, pnpm >= 12, Vite Plus · GitHub template · sign-in: Better Auth · [Repo](https://github.com/mugnavo/cove) · [▶️ Demo ↗](https://cove.mugnavo.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cove/)</sub>

<a name="lithium"></a>
### #&#8288;60 [lithium](https://github.com/wsvincent/lithium) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · custom license · Nov 2026</sub>

**Django starter project with allauth login, Bootstrap 5 styling and SQLite.**

Lithium is a Django 6.1 starter for Python 3.12+ that ships sign up, login and password reset through django-allauth. It also wires in Whitenoise for static files, Bootstrap 5, django-debug-toolbar, django-crispy-forms and custom 403, 404 and 500 pages. It uses SQLite locally and installs with uv or pip. It has no AI features.

- **+** Login, signup and password reset preconfigured via django-allauth
- **+** SQLite for local development, so no database server is needed
- **+** Installs with either uv or pip from requirements.txt
- **+** Includes debug toolbar, crispy forms and custom error pages
- **−** No billing or payments included
- **−** No AI or LLM integration
- **−** Environment variables, gunicorn and mail provider are left for you to add
- **−** No Docker or compose files provided

<sub>Python · Needs Python 3.12+, uv or pip, SQLite · GitHub template · [Repo](https://github.com/wsvincent/lithium) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lithium/)</sub>

<a name="papermark"></a>
### #&#8288;61 [papermark](https://github.com/papermark/papermark) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (63) · Freshness: active (86) · Maintenance: weak (29) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · custom license · Aug 2026</sub>

**Document sharing with tracked links, custom domains and analytics, like DocSend.**

Papermark is a Next.js and TypeScript app for sharing documents through custom links, with a custom domain, branding and view analytics. It stores data in PostgreSQL through Prisma, uses NextAuth for login, and sends analytics events to Tinybird. The README describes no AI features, so it fits this list only as a SaaS-style app base.

- **+** Custom domains and branding on shared document links
- **+** Standard stack: Next.js, Prisma, PostgreSQL, NextAuth, shadcn/ui
- **+** Self-hostable with a short setup: npm install, .env, Prisma init, npm run dev
- **+** Includes Stripe billing and Resend email integrations in the stack
- **−** No AI features described in the README
- **−** Requires external services: Tinybird, Resend and S3 or Vercel Blob
- **−** No Dockerfile or compose file detected; setup is a manual Node install
- **−** Page-by-page analytics is listed as upcoming, not shipped

<sub>TypeScript · Needs Node.js >= 18.17.0, PostgreSQL, AWS S3 or Vercel Blob, Resend, Tinybird, Stripe · env example file · sign-in: Auth.js · [Repo](https://github.com/papermark/papermark) · [🌐 Site ↗](https://www.papermark.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/papermark/)</sub>

<a name="shipswift"></a>
### #&#8288;62 [shipswift](https://github.com/signerlabs/shipswift) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (38) · Freshness: active (100) · Maintenance: weak (30) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Nov 2026</sub>

**SwiftUI component library with skills and an MCP server for AI coding tools.**

ShipSwift is a MIT-licensed set of SwiftUI source files for iOS 18+: 44 animation components (some Metal shaders), charts, UI components, and modules for auth, camera, chat, paywall and settings. Components are copied into an Xcode project, or fetched by an AI assistant through installable skills or a hosted MCP server. Backend guides and compliance templates are in a paid Pro tier.

- **+** Components are self-contained files you can copy directly into Xcode
- **+** Local skills mode reads source from the repo, works offline without MCP
- **+** Covers Metal-shader animations, nine chart types, and auth, camera and chat modules
- **+** Showcase app and website provide live previews of components
- **−** Backend routes, compliance templates and pitfall guides are Pro-only
- **−** Requires iOS 18.0+ and Swift; no Android or cross-platform support
- **−** Auth depends on Amplify/Cognito; voice input uses VolcEngine ASR
- **−** No tagged releases; consumed by copying files, not as a package

<sub>Swift · Needs Xcode, iOS 18+, Amplify SDK (Cognito), StoreKit 2, VolcEngine ASR · [Repo](https://github.com/signerlabs/shipswift) · [▶️ Demo ↗](https://apps.apple.com/us/app/shipswift-mcp-codebase/id6759209764) · [🌐 Site ↗](https://www.shipswift.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shipswift/)</sub>

<a name="jetstream"></a>
### #&#8288;63 [jetstream](https://github.com/laravel/jetstream) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Nov 2026</sub>

**Laravel starter kit for Laravel 11.x and earlier.**

Jetstream is a PHP application starter kit for Laravel 11.x and prior versions. The README is a single notice and lists no features, so its scope is not described there. It directs new projects to the newer Laravel starter kits at laravel.com/starter-kits.

- **+** MIT licensed PHP codebase from the Laravel project
- **+** Recent commit activity, last commit 2026-10-17
- **+** Targets Laravel 11.x and earlier, matching existing apps on those versions
- **−** Not for the latest Laravel; README points to newer starter kits
- **−** README lists no features, setup steps or AI integration
- **−** Last release 2026-05-19 is older than the latest commits

<sub>PHP · [Repo](https://github.com/laravel/jetstream) · [🌐 Site ↗](https://laravel.com/starter-kits) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jetstream/)</sub>

<a name="apptension-saas-boilerplate"></a>
### #&#8288;64 [saas-boilerplate](https://github.com/apptension/saas-boilerplate) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: known (37) · Freshness: active (94) · Maintenance: weak (30) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**React, Django and GraphQL SaaS starter with Stripe billing and multi-tenancy.**

Full-stack SaaS boilerplate with a React 19 and Vite frontend, a Django 5.2 and Graphene GraphQL backend, Celery workers, and AWS CDK infrastructure. It ships auth (OAuth, passkeys, 2FA, SAML/OIDC SSO), Stripe subscriptions, multi-tenancy with RBAC, Contentful CMS, and an OpenAI example. An MCP-based AI agent and Plop CRUD generators are included.

- **+** Auth covers OAuth, passkeys, 2FA, SAML/OIDC SSO and SCIM sync
- **+** Stripe subscriptions, trials and multi-tenant roles (Owner, Admin, Member) included
- **+** Plop generators scaffold tenant-scoped CRUD with forms, tables and GraphQL operations
- **+** AWS CDK infrastructure supports multiple deployment environments
- **−** Opinionated stack: Django, GraphQL and AWS CDK are hard to swap out
- **−** Depends on Stripe, Contentful, Sentry and OpenAI services
- **−** Local setup needs Docker, Node 20+ and pnpm 9+ (WSL 2 on Windows)
- **−** AI features are an OpenAI example and an MCP agent, not a general AI framework

<sub>TypeScript, OpenAI · Needs Docker, Node.js 20+, pnpm 9+, Postgres 14+, Redis 7+, Stripe, Contentful, Sentry, OpenAI, AWS · [Repo](https://github.com/apptension/saas-boilerplate) · [▶️ Demo ↗](https://app.demo.saas.apptoku.com/) · [📖 Docs ↗](https://docs.demo.saas.apptoku.com/) · [🌐 Site ↗](https://www.apptension.com/saas-boilerplate?utm_source=readme-file&utm_medium=referral&utm_campaign=SaaS%20Boilerplate&utm_term=SaaS%20Boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apptension-saas-boilerplate/)</sub>

<a name="oinone-pamirs"></a>
### #&#8288;65 [oinone-pamirs](https://github.com/oinone/oinone-pamirs) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · AGPL-3.0 · Sep 2026</sub>

**Java back-end framework for metadata-driven low-code enterprise apps.**

Oinone Pamirs is the Java back end of a low-code framework in which models, views and logic are described as metadata, aimed at enterprise systems such as ERP, MES and OMS. The README also describes Aino, an agent layer built on the same metadata, and Spec practices for AI-assisted coding. The repo is split into modules such as pamirs-framework, pamirs-core, pamirs-boot and pamirs-middleware.

- **+** Metadata-driven design: one model definition feeds the back end and the visual designer
- **+** Modular packages (framework, core, boot, SPI, middleware) split by responsibility
- **+** Quickstart uses a compose file and serves the UI on port 88
- **+** Framework source is open, so AI coding tools can read it
- **−** AGPL-3.0 license imposes obligations on networked derivative works
- **−** A separate Enterprise Edition exists; the README does not list what it adds
- **−** The 7.x live demo is listed as not yet released
- **−** Front end is a separate repo (oinone-kunlun); the repo has no tagged release

<sub>Java · Needs Docker Compose (quickstart), Java · [Repo](https://github.com/oinone/oinone-pamirs) · [📖 Docs ↗](https://guide.oinone.ai/en/InstallOrUpgrade/CommunityEdition.html) · [🌐 Site ↗](https://www.oinone.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oinone-pamirs/)</sub>

<a name="free-react-tailwind-admin-dashboard"></a>
### #&#8288;66 [free-react-tailwind-admin-dashboard](https://github.com/tailadmin/free-react-tailwind-admin-dashboard) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**React 19 and Tailwind v4 admin dashboard template in TypeScript.**

TailAdmin is a front-end admin dashboard template built on React 19, TypeScript and Tailwind CSS v4. The free edition ships one dashboard, 35+ dashboard components and 50+ UI elements, including tables, charts, calendar, auth forms and dark mode. It has no backend, and the AI Dashboard and AI Settings pages are UI pages.

- **+** Current stack: React 19, TypeScript, Tailwind CSS v4, Node.js 20 or later
- **+** Includes charts, tables, calendar, auth forms, dark mode, and RTL and multi-language support
- **+** MIT licensed, with versions for Next.js, Vue, Angular, Laravel and plain HTML
- **+** Includes an AGENTS.md for working with AI coding agents
- **−** Free edition has 1 dashboard; the other 6 dashboards are in the paid Pro version
- **−** No backend, database or billing; auth is forms only
- **−** AI pages cover token usage and model settings UI only, with no model integration documented
- **−** Free edition has community support only, and the Figma files are basic

<sub>JavaScript · Needs Node.js 20+ · [Repo](https://github.com/tailadmin/free-react-tailwind-admin-dashboard) · [▶️ Demo ↗](https://free-react-demo.tailadmin.com/) · [📖 Docs ↗](https://tailadmin.com/docs) · [🌐 Site ↗](https://tailadmin.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/free-react-tailwind-admin-dashboard/)</sub>

<a name="coreui-free-bootstrap-admin-template"></a>
### #&#8288;67 [coreui-free-bootstrap-admin-template](https://github.com/coreui/coreui-free-bootstrap-admin-template) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (69) · Freshness: active (99) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Aug 2026</sub>

**Bootstrap 5 admin dashboard template built with Pug, Sass and plain JavaScript.**

Static admin dashboard template on CoreUI's Bootstrap 5 component library, with Pug sources compiled to HTML, plus SCSS and JS modules. It includes authentication, forms, icon and error page views. For AI-assisted work it ships a .cursorrules file, ARCHITECTURE.md, DEVELOPMENT.md and JSDoc comments. It is a UI shell and has no AI features itself.

- **+** MIT licensed, with Pug, SCSS and JS sources and a minified build via npm run build
- **+** Includes .cursorrules, ARCHITECTURE.md and DEVELOPMENT.md so coding assistants get project conventions
- **+** Prebuilt views for authentication pages, forms, icons, components and error pages
- **+** Hot-reload dev server via npm start; no backend or database required
- **−** No backend, auth logic, billing or database; the login pages are only markup
- **−** Several components (date pickers, multi select, stepper, rating) are PRO-only
- **−** Data Grid and Scheduler are separate paid add-ons, not part of this template
- **−** Contains no AI functionality; the AI-friendly part is only context files

<sub>HTML · Needs Node.js, npm · [Repo](https://github.com/coreui/coreui-free-bootstrap-admin-template) · [📖 Docs ↗](https://coreui.io/bootstrap/docs/templates/installation/) · [🌐 Site ↗](https://coreui.io/product/free-bootstrap-admin-template/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coreui-free-bootstrap-admin-template/)</sub>

<a name="eladmin"></a>
### #&#8288;68 [eladmin](https://github.com/elunez/eladmin) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: widely used (81) · Freshness: recent (70) · Maintenance: weak (9) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

**Spring Boot and Vue admin panel with RBAC and code generator.**

ELADMIN is a front/back-separated admin system built on Spring Boot 2.7.18, Spring Data JPA, Spring Security, JWT, Redis and a Vue frontend (separate eladmin-web repo). It covers user, role, menu, department, dictionary and log management, Quartz jobs, and a generator that emits CRUD code for backend and frontend. It has no AI features; it is a conventional admin boilerplate.

- **+** Code generator produces front and back CRUD code
- **+** Interface-level and data-level permissions via annotations, plus Redis rate limiting
- **+** Bundled Quartz jobs, Druid SQL monitor, S3-compatible storage, Alipay and email
- **+** Live demo and docs site available
- **−** No AI functionality; fits this list only as a generic app boilerplate
- **−** README and docs are in Chinese only
- **−** Last release is 2023-07-05; Spring Boot 2.7 is end-of-life
- **−** Frontend is in a separate repo; no Docker or compose files

<sub>Java · Needs Redis, Java, Vue frontend (eladmin-web), JWT_BASE64_SECRET env var for prod · [Repo](https://github.com/elunez/eladmin) · [▶️ Demo ↗](https://eladmin.vip/demo) · [📖 Docs ↗](https://eladmin.vip) · [🌐 Site ↗](https://eladmin.vip) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eladmin/)</sub>

<a name="shadcn-admin"></a>
### #&#8288;69 [shadcn-admin](https://github.com/satnaing/shadcn-admin) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: popular (76) · Freshness: recent (67) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Jun 2026</sub>

**Vite and shadcn/ui admin dashboard with 10+ pages and RTL support.**

A React admin dashboard UI built on shadcn/ui (Tailwind and Radix), Vite and TanStack Router, written in TypeScript. It ships a sidebar, global search command, light/dark mode and more than 10 pages, with some shadcn components modified for right-to-left layouts. Clerk handles auth only partially, and the README says this is a UI collection rather than a starter template. It has no AI features.

- **+** Built-in sidebar, global search command and light/dark mode
- **+** RTL support, with modified components listed in the README
- **+** Standard stack: Vite, TanStack Router, TypeScript, ESLint, Prettier
- **+** MIT license; runs locally with pnpm install and pnpm run dev
- **−** No AI features; fits this list only loosely
- **−** Auth via Clerk is partial; no billing or database included
- **−** Author states it is not a starter template
- **−** Customized components need manual merging when updating via the shadcn CLI

<sub>TypeScript · Needs Clerk (partial auth) · GitHub template · env example file · sign-in: Clerk · [Repo](https://github.com/satnaing/shadcn-admin) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shadcn-admin/)</sub>

<a name="coreui-free-vue-admin-template"></a>
### #&#8288;70 [coreui-free-vue-admin-template](https://github.com/coreui/coreui-free-vue-admin-template) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (40) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Sep 2026</sub>

**Vue 3 admin dashboard template with CoreUI components and AI assistant rules.**

A Vue 3 single-page admin dashboard template built on Vite, Vue Router, Pinia and the CoreUI Vue component library. It ships layouts, sidebar and header components, and example views. It also includes .cursorrules, ARCHITECTURE.md and DEVELOPMENT.md so Cursor, Copilot or Claude Code follow its conventions.

- **+** MIT licensed; npm or yarn install, dev server on port 3000
- **+** Includes .cursorrules, ARCHITECTURE.md and DEVELOPMENT.md for AI coding assistants
- **+** Vue 3 Composition API with script setup, Pinia, Vue Router and Vite
- **+** Semantic versioning with changelogs on GitHub releases
- **−** Smart Table, date pickers, multi-select and others require paid CoreUI PRO
- **−** No backend, auth, billing or database; frontend UI only
- **−** Data Grid and Scheduler are separate paid add-ons
- **−** AI support is config and docs only; no model integration

<sub>Vue · Needs Node.js, npm or yarn · [Repo](https://github.com/coreui/coreui-free-vue-admin-template) · [📖 Docs ↗](https://coreui.io/vue/docs/templates/installation.html) · [🌐 Site ↗](https://coreui.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coreui-free-vue-admin-template/)</sub>

<a name="bullet-train"></a>
### #&#8288;71 [bullet_train](https://github.com/bullet-train-co/bullet_train) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (24) · Freshness: active (99) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2026</sub>

**Ruby on Rails template for building multi-tenant SaaS apps.**

Bullet Train is a Ruby on Rails application template for SaaS products. You clone it (not fork), run bin/configure and bin/setup, and it serves locally on port 3000 using PostgreSQL and Redis for Action Cable and job queues. The README describes no AI features, so it fits this list only as a general SaaS starter.

- **+** MIT-licensed Rails template with bin/configure, bin/setup and bin/dev scripts
- **+** Deploy buttons for Render (about $30/month) and Heroku (about $140/month)
- **+** Standard Rails stack: PostgreSQL, Redis, Action Cable, background jobs
- **+** Developer docs and a community Discord server
- **−** README mentions no built-in AI or LLM integration
- **−** Ruby on Rails only; Node and Yarn also required
- **−** Homebrew setup steps cover macOS only
- **−** Setup needs manual rbenv, nvm and shell configuration

<sub>Ruby · Needs PostgreSQL, Redis, Ruby (rbenv), Node.js (nvm), Yarn · Docker · [Repo](https://github.com/bullet-train-co/bullet_train) · [📖 Docs ↗](https://bullettrain.co/docs) · [🌐 Site ↗](https://bullettrain.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bullet-train/)</sub>

<a name="flutter-responsive-admin-panel-or-dashboard"></a>
### #&#8288;72 [flutter-responsive-admin-panel-or-dashboard](https://github.com/abuanwar072/flutter-responsive-admin-panel-or-dashboard) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: popular (58) · Freshness: active (93) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Jul 2026</sub>

**Flutter admin dashboard UI with charts, tables and info cards.**

A responsive admin panel template written in Dart with Flutter. It lays out charts, tables and info cards, and targets web, macOS, tablets, Android and iOS from one codebase. It depends on flutter_svg, google_fonts and provider, uses the Poppins font, and has a YouTube build tutorial.

- **+** One Flutter codebase for web, macOS, tablet, Android and iOS
- **+** Small dependency set: flutter_svg, google_fonts, provider
- **+** Live web preview and a step-by-step video tutorial
- **+** MIT license
- **−** UI only: no auth, billing, database or backend included
- **−** No AI features despite the list it appears on
- **−** No tagged releases
- **−** README has no setup, customization or API documentation

<sub>Dart · Needs flutter_svg, google_fonts, provider · [Repo](https://github.com/abuanwar072/flutter-responsive-admin-panel-or-dashboard) · [▶️ Demo ↗](https://abuanwar072.github.io/Flutter-Responsive-Admin-Panel-or-Dashboard/#/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flutter-responsive-admin-panel-or-dashboard/)</sub>

<a name="ai-fullstack-saas-boilerplate"></a>
### #&#8288;73 [AI-Fullstack-SaaS-Boilerplate](https://github.com/alan345/ai-fullstack-saas-boilerplate) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (18) · Freshness: recent (70) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

**Fastify, tRPC and React SaaS base with Better Auth and SSE chat.**

A pnpm monorepo: a Fastify server with tRPC routers on port 2022, Drizzle over Postgres, Better Auth with user impersonation, and a Vite React 19 client with React Router that ships as static files. The AI feature is an OpenAI chat streamed over server-sent events, an external-API example and a debounced search hook round it out, and Playwright tests run against the live app. For teams who want type-safe APIs without Next.js.

- **+** End-to-end types through tRPC; the client is static files you can host on S3
- **+** Better Auth with admin impersonation already wired
- **+** Playwright e2e tests and a seed script included
- **+** Hosted demo on Render
- **−** No billing, no usage metering; AI is a single SSE chat
- **−** OpenAI only
- **−** Static SPA; README notes it is not SEO-friendly
- **−** Demo on a free Render tier spins down; expect 50 second cold starts

<sub>TypeScript, openai · Needs postgres, openai-api-key · env example file · [Repo](https://github.com/alan345/ai-fullstack-saas-boilerplate) · [▶️ Demo ↗](https://fsb-client.onrender.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-fullstack-saas-boilerplate/)</sub>

<a name="scaffold-eth-2"></a>
### #&#8288;74 [scaffold-eth-2](https://github.com/scaffold-eth/scaffold-eth-2) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (27) · Freshness: recent (70) · Maintenance: weak (19) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Ethereum dapp starter with Next.js, Wagmi, Viem and Foundry or Hardhat.**

Scaffold-ETH 2 generates a monorepo for building Ethereum dapps, with a Next.js frontend using RainbowKit, Wagmi and Viem and smart contracts in Foundry or Hardhat. The frontend reloads when contracts change, and a Debug Contracts page lets you call deployed functions locally. The repo includes agent config folders (.agents, .claude, .opencode, .cursor), but AI is a side feature.

- **+** Contract hot reload keeps the frontend in sync with contract edits
- **+** Typed React hooks wrap Wagmi for contract reads and writes
- **+** Burner wallet and local faucet allow testing without external wallets
- **+** Choice of Foundry or Hardhat; extensions add starter kits via create-eth
- **−** Ethereum-only; no model or AI functionality beyond agent config files
- **−** Needs Node >= 22.13.0 and Yarn; no Docker setup provided
- **−** Local dev needs three terminals: chain, deploy and frontend
- **−** Last tagged release is from 2024-04-16, though commits continue

<sub>TypeScript · Needs Node >= 22.13.0, Yarn, Git, Foundry or Hardhat · GitHub template · [Repo](https://github.com/scaffold-eth/scaffold-eth-2) · [📖 Docs ↗](https://docs.scaffoldeth.io) · [🌐 Site ↗](https://scaffoldeth.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scaffold-eth-2/)</sub>

<a name="nextarter-chakra"></a>
### #&#8288;75 [nextarter-chakra](https://github.com/agustinusnathaniel/nextarter-chakra) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (21) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 838 · MIT · Nov 2026</sub>

**Next.js 16 starter with Chakra UI v3, TypeScript, Biome and Playwright.**

A Next.js App Router template with Chakra UI v3, Emotion, next-themes and TypeScript 5 preconfigured. It separates routing (src/app) from page and layout logic (src/lib) and UI components (src/components), and adds Biome for lint and format, Playwright for E2E tests and Turborepo for builds. It has no AI features, auth or database; it is a plain frontend scaffold.

- **+** Current stack: Next.js 16 App Router, Chakra UI v3, TypeScript 5
- **+** Biome and Playwright E2E preconfigured, with pnpm scripts for both
- **+** Routing is split from page logic in src/lib, keeping src/app thin
- **+** Deploy buttons for Vercel, Netlify, Railway and StackBlitz
- **−** No auth, billing or database wired in
- **−** No AI or LLM integration; only loosely fits this list
- **−** No tagged releases; you fork the main branch
- **−** Uses pnpm; no Docker setup provided

<sub>TypeScript · GitHub template · [Repo](https://github.com/agustinusnathaniel/nextarter-chakra) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nextarter-chakra/)</sub>

<a name="react"></a>
### #&#8288;76 [react](https://github.com/duxianwei520/react) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (50) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Jul 2026</sub>

**React 18 admin dashboard starter with login, role permissions and mock API.**

A Vite-based React 18 admin front-end template using Redux Toolkit, React Router 6, Ant Design 6 and Less. It ships login with permission control, user, role and module management pages, ECharts and DraftJS demos, and a Mock.js backend started with `npm start`. It has no AI features, and the README is mostly in Chinese.

- **+** Includes user, role and module permission management pages out of the box
- **+** Mock.js server runs with the dev server, so no backend is needed to try it
- **+** Current stack: React 18.3, Vite 6, Redux Toolkit 2, Ant Design 6
- **+** Companion Express and Node repos provide real login, register and user-info APIs
- **−** No AI or model integration despite the list's focus
- **−** No database, billing or server-side auth in this repo; data is mocked
- **−** README is in Chinese, with a QQ group for support
- **−** No Docker setup or tagged releases

<sub>JavaScript · Needs Node.js, npm · [Repo](https://github.com/duxianwei520/react) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react/)</sub>

<a name="typescript-nextjs-starter"></a>
### #&#8288;77 [typescript-nextjs-starter](https://github.com/jpedroschmitz/typescript-nextjs-starter) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (17) · Freshness: active (91) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Nov 2026</sub>

**Next.js 16 and TypeScript starter with linting, commit hooks and typed env vars.**

A project template for Next.js 16 (App Router) with React 19 and TypeScript, installed through create-next-app. It preconfigures Oxlint, Oxfmt, Husky, Commitlint, lint-staged, Renovate, a PR type-check workflow, T3 Env, a minimal CSP and typed redirects. It contains no AI features, auth, billing or database.

- **+** Tooling is preconfigured: Oxlint, Oxfmt, Commitlint, Renovate and a CI workflow for type check and lint
- **+** Type-safe environment variables via T3 Env, with client and server schemas
- **+** Minimal default CSP and typed redirects array are set up in config
- **+** Does not impose a UI library, auth or database choice
- **−** No AI, model or LLM integration, so it does not fit an AI-focused list on its own
- **−** No auth, billing or database included; all of that must be added
- **−** Requires Node.js 24 or newer and pnpm 10 by default
- **−** Husky pre-commit hook is disabled by default and needs a manual opt-in

<sub>TypeScript · Needs Node.js >= 24, pnpm 10 · GitHub template · [Repo](https://github.com/jpedroschmitz/typescript-nextjs-starter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typescript-nextjs-starter/)</sub>

<a name="lightswind-ui-library"></a>
### #&#8288;78 [lightswind-ui-library](https://github.com/codewithmuhilan/lightswind-ui-library) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: weak (27) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**React component library installed as source via CLI, with an MCP server.**

Lightswind UI is a shadcn-style library of 160+ React components (Tailwind, Framer Motion, GSAP) copied into your project as .tsx files with `npx lightswind add`. It covers UI primitives, animated backgrounds, text and cursor effects, and 3D/WebGL pieces. A bundled MCP server lets Cursor, Claude Desktop or Cline search, read and install components.

- **+** Components are copied as local source, so no runtime dependency on the package
- **+** CLI resolves component prerequisites and detects Next.js, Vite or CRA setups
- **+** MCP server exposes search, source fetch and install tools to coding agents
- **+** Includes 3D, shader and animated background components beyond standard UI primitives
- **−** Some components and page blocks require a paid Pro license key
- **−** Needs Tailwind CSS v3 or v4 and React 18/19; no other frameworks listed
- **−** Not an AI app starter: no auth, billing, database or model integration
- **−** Animation and WebGL components pull in extra dependencies per component

<sub>TypeScript · Needs Node.js 18+, React 18 or 19, Tailwind CSS v3 or v4 · [Repo](https://github.com/codewithmuhilan/lightswind-ui-library) · [📖 Docs ↗](https://lightswind.com/components/introduction) · [🌐 Site ↗](https://lightswind.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lightswind-ui-library/)</sub>

<a name="ui"></a>
### #&#8288;79 [ui](https://github.com/creativetimofficial/ui) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (69) · Freshness: slowing (31) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Mar 2026</sub>

**shadcn/ui-based React components and page blocks installed through a CLI.**

Creative Tim UI is a component registry built on shadcn/ui. Its CLI (`npx @creative-tim/ui@latest add <name>`) copies components and page blocks into a Next.js project. Blocks cover modals, account, billing, testimonials, contact, footers, FAQs, blog, ecommerce and Web 3.0 sections.

- **+** Installs via the native shadcn CLI or its own npx command
- **+** Blocks include account and billing screens plus marketing and ecommerce sections
- **+** MIT licensed, and components are copied into your repo so you can edit them
- **+** Block counts are listed per category, such as 17 testimonials and 16 footers
- **−** No AI features described; it is a general UI kit, so it fits this list loosely
- **−** Requires Next.js, Tailwind CSS and an initialized shadcn/ui project
- **−** Front-end blocks only; no auth, billing or database backend is wired in
- **−** Last tagged release is from 2023-05-04, though commits continued into 2026

<sub>TypeScript · Needs Node.js 18+, Next.js, shadcn/ui, Tailwind CSS · [Repo](https://github.com/creativetimofficial/ui) · [📖 Docs ↗](https://creative-tim.com/ui/docs/components) · [🌐 Site ↗](https://creative-tim.com/ui) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui/)</sub>

<a name="next-forge"></a>
### #&#8288;80 [next-forge](https://github.com/vercel/next-forge) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (60) · Freshness: recent (75) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · May 2026</sub>

**Turborepo monorepo template for SaaS apps built on Next.js.**

next-forge is a Turborepo monorepo scaffolded with `npx next-forge@latest init`. It includes a marketing site, main app, API, docs, email templates and Storybook, with shared packages for Clerk auth, a typed database ORM, Stripe payments, Resend email, analytics, Sentry and Arcjet security. An AI utilities package is included, but it is one package among many.

- **+** Auth, payments, email, analytics, observability and security packages are pre-wired in one monorepo
- **+** Each app is independently deployable; packages are shared across apps
- **+** Live demos for web, app, Storybook and API health check
- **+** Docs include migration guides for swapping providers
- **−** Default stack needs many third-party accounts: Clerk, Stripe, Resend, Sentry, Arcjet, PostHog
- **−** AI package is described only as 'AI integration utilities'; specifics not in README
- **−** Opinionated stack; replacing providers means following migration guides
- **−** Requires Node.js 20+ and Stripe CLI for local webhook testing

<sub>TypeScript · Needs Node.js 20+, Bun, Stripe CLI, Clerk, Stripe, Resend, Sentry, BetterStack, Arcjet, PostHog, Google Analytics · GitHub template · [Repo](https://github.com/vercel/next-forge) · [▶️ Demo ↗](https://demo.next-forge.com) · [📖 Docs ↗](https://www.next-forge.com/docs) · [🌐 Site ↗](https://www.next-forge.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-forge/)</sub>

<a name="fulling"></a>
### #&#8288;81 [fulling](https://github.com/fullagent/fulling) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (31) · Freshness: active (93) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Jul 2026</sub>

**Next.js app with GitHub sign-in and per-user Kubernetes credential validation.**

Fulling is a Next.js and TypeScript app that is being rebuilt around persistent AI workspaces. The current v3 foundation provides GitHub-only sign-in via Better Auth, PostgreSQL-backed users and sessions, and storage of one kubeconfig per user, validated through Kubernetes SelfSubjectReview. The workspace features themselves (skills, files, memory, runtime) are the target model, not yet shipped.

- **+** Kubeconfig validation rejects exec plugins, local file credentials, proxies, non-HTTPS servers and redirects
- **+** Public app builds and runs without env vars, PostgreSQL or an OAuth provider
- **+** Deploys on Vercel's native Next.js flow with no vercel.json
- **+** Includes Vitest and Playwright tests plus Prisma schema validation commands
- **−** Kubeconfigs are stored as plaintext in PostgreSQL; database read access exposes them
- **−** Workspace runtime, skills and memory are a target model, not implemented yet
- **−** Any HTTPS API server address is allowed, an accepted SSRF boundary
- **−** v3 uses a new baseline schema and does not migrate v2 data

<sub>TypeScript · Needs Node.js 24, PostgreSQL, GitHub OAuth App, Kubernetes cluster · Docker · env example file · sign-in: Better Auth · [Repo](https://github.com/fullagent/fulling) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fulling/)</sub>

<a name="shipfree"></a>
### #&#8288;82 [shipfree](https://github.com/revokslab/shipfree) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (22) · Freshness: active (82) · Maintenance: weak (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Jun 2026</sub>

**Next.js SaaS starter with Better-Auth, multi-provider billing and Postgres.**

ShipFree is a free ShipFast-style SaaS boilerplate built on Next.js, Bun, Drizzle ORM and Postgres. It wires in Better-Auth for login, six payment providers (Stripe, Polar, Autumn, Dodo Payments, Commet, Creem) and email via Resend, Postmark, Plunk or Nodemailer. It also includes next-intl routing for English, French and Spanish. The README does not describe any AI features.

- **+** Six billing providers supported, including Stripe, Polar and Creem
- **+** Four email options: Resend, Postmark, Plunk and Nodemailer
- **+** next-intl i18n with en, fr and es and as-needed locale prefixes
- **+** Drizzle ORM with Postgres and Better-Auth for authentication
- **−** README documents no AI features despite the list's AI focus
- **−** Requires Bun as runtime and package manager
- **−** Includes a premium-purchase module that must be removed manually
- **−** No Docker or compose files provided

<sub>TypeScript · Needs Postgres, Bun, Stripe, Resend · Docker · env example file · sign-in: Better Auth · README: alternative to ShipFast · [Repo](https://github.com/revokslab/shipfree) · [📖 Docs ↗](https://shipfree.revoks.dev/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shipfree/)</sub>

<a name="remix-saas"></a>
### #&#8288;83 [remix-saas](https://github.com/dev-xo/remix-saas) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

**Remix SaaS starter with auth, billing and SQLite.**

Remix SaaS is a TypeScript Remix template for subscription apps, installed with `npx create-remix-saas@latest`. Setup generates a .env with random secrets, a local SQLite database, roles and demo plans, and login works via email code or magic link. A MOCK_SERVICES mode keeps email and billing local in development. The README describes no built-in AI features.

- **+** Local setup needs no external credentials; npm run setup creates SQLite, roles and demo plans
- **+** Mock mode keeps email and billing local and is rejected in production
- **+** Live demo and a docs folder are available
- **+** Ships npm run check and smoke tests to verify the app
- **−** README describes no AI features; any model integration must be added by you
- **−** No Google login; GitHub login only appears when credentials are configured
- **−** No tagged releases; README notes known upstream security findings
- **−** Demo runs on a free tier and can be slow to load

<sub>TypeScript · Needs Node 24 LTS, npm, SQLite · Docker · env example file · [Repo](https://github.com/dev-xo/remix-saas) · [▶️ Demo ↗](https://remix-saas.fly.dev) · [📖 Docs ↗](https://github.com/dev-xo/remix-saas/tree/main/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/remix-saas/)</sub>

<a name="vuesion"></a>
### #&#8288;84 [vuesion](https://github.com/vuesion/vuesion) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: known (34) · Freshness: recent (71) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**Archived Vue and Nuxt boilerplate with design system, auth and test setup.**

Vuesion 5 is a Vue and Nuxt boilerplate with a 35+ component design system, Nuxt auth module, i18n, PWA support and code generators for components, pages, REST APIs and Pinia stores. It ships with Vitest, Cypress and Testing Library setups (250+ example tests) and Storybook. The repository is no longer maintained; development continues in a commercial product at vuesion.dev.

- **+** Includes 250+ example tests using Vitest, Cypress and Testing Library
- **+** Design system with 35+ components, theming and a Figma UI kit
- **+** Code generators for components, pages, REST APIs and Pinia stores
- **+** Supports SSR, SPA or static generation through Nuxt
- **−** No new features or maintenance; last release was 2025-06-09
- **−** Current Vuesion version is commercial and closed source
- **−** No AI features or billing in this version; auth only
- **−** Uses vee-validate v3, an older major version

<sub>Vue · Needs Nuxt, Storybook, Cypress, Vitest · Docker · sign-in: Auth.js · [Repo](https://github.com/vuesion/vuesion) · [📖 Docs ↗](https://www.vuesion.dev/docs) · [🌐 Site ↗](https://www.vuesion.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vuesion/)</sub>

<a name="create-t3-app"></a>
### #&#8288;85 [create-t3-app](https://github.com/t3-oss/create-t3-app) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: widely used (87) · Freshness: quiet (21) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Dec 2025</sub>

**CLI that scaffolds a typesafe Next.js app with tRPC and Prisma or Drizzle.**

create-t3-app is an npm CLI that generates a Next.js project from the T3 Stack: TypeScript, Tailwind CSS, tRPC, NextAuth.js, and Prisma or Drizzle. Each piece is optional and chosen through prompts, so the output matches the selected options. It ships no model or agent code; it is a general full-stack web scaffold.

- **+** Modular: tRPC, Prisma, Drizzle, NextAuth.js and Tailwind are each opt-in
- **+** Runs through npm, yarn, pnpm or bun with one create command
- **+** Typesafety from database schema to client via tRPC and TypeScript
- **+** MIT licensed, with a docs site and an active Discord
- **−** No AI features, model integrations or LLM examples included
- **−** No billing, state management or deployment setup; you bring your own
- **−** Opinionated stack: Next.js and TypeScript only, no other frameworks
- **−** No Docker or compose files provided

<sub>TypeScript · Needs Node.js, Next.js, tRPC, Tailwind CSS, Prisma, Drizzle, NextAuth.js · [Repo](https://github.com/t3-oss/create-t3-app) · [📖 Docs ↗](https://create.t3.gg/en/installation) · [🌐 Site ↗](https://create.t3.gg) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/create-t3-app/)</sub>

<a name="mall-swarm"></a>
### #&#8288;86 [mall-swarm](https://github.com/macrozheng/mall-swarm) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: popular (71) · Freshness: slowing (48) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · May 2026</sub>

**Spring Cloud microservice e-commerce system with Vue admin console.**

mall-swarm is a Java e-commerce backend split into microservices: auth, gateway, admin, portal, search and monitor. It is built on Spring Cloud 2025, Spring Boot 3.5, Sa-Token, MyBatis and Elasticsearch. It pairs with separate Vue admin and uni-app storefront repos, and includes a registry, config center, monitoring and Kubernetes deployment notes.

- **+** Full microservice split: gateway, auth, admin, portal, search, monitor, with Seata for transactions
- **+** Live demos for both the admin console and the mobile storefront
- **+** Extensive tutorials and video course; dev-v2 branch keeps Spring Boot 2.7
- **+** Deployment coverage includes Docker, Jenkins and Kubernetes
- **−** Heavy dependency stack: MySQL, Redis, Elasticsearch, MongoDB, RabbitMQ, Logstash, Nginx
- **−** Admin and mobile frontends live in separate repositories
- **−** Documentation and tutorials are mainly in Chinese
- **−** No Docker or Compose files detected; last release was 2024-03

<sub>Java · Needs JDK 17, MySQL 5.7, Redis 7.0, Elasticsearch 7.17.3, MongoDB 5.0, RabbitMQ 3.10.5, Nginx 1.22, Nacos, Logstash 7.17.3, Kibana 7.17.3 · [Repo](https://github.com/macrozheng/mall-swarm) · [▶️ Demo ↗](https://www.macrozheng.com/admin/index.html) · [📖 Docs ↗](https://cloud.macrozheng.com) · [🌐 Site ↗](https://cloud.macrozheng.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mall-swarm/)</sub>

<a name="quickapp"></a>
### #&#8288;87 [quickapp](https://github.com/emonney/quickapp) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (14) · Freshness: active (88) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Sep 2026</sub>

**Angular 21 and ASP.NET Core 10 starter with auth and user management.**

QuickApp is a full-stack starter pairing an Angular 21 frontend with an ASP.NET Core 10 backend. It ships OpenIddict/OAuth2 JWT auth, user and role management with permission-based policies, EF Core migrations and an admin UI. An ai-rules/AI_RULES.md file and shared base classes let AI tools add features by following existing patterns.

- **+** OpenIddict/OAuth2 auth, roles, permission policies and user admin UI already built
- **+** Includes ai-rules/AI_RULES.md and base classes (BaseEntity, BaseApiController, EndpointBase)
- **+** EF Core Code First migrations, Swagger/OpenAPI, i18n and Bootstrap 5 theming included
- **+** MIT license, with a live demo of the Standard edition
- **−** No billing or payments wired in
- **−** README lists SQL Server only; other databases are in the successor NetForge
- **−** Author says new work happens in NetForge, not QuickApp
- **−** No Docker or compose files

<sub>TypeScript · Needs SQL Server, .NET 10 SDK, Node.js and npm · [Repo](https://github.com/emonney/quickapp) · [▶️ Demo ↗](https://quickapp-standard.ebenmonney.com) · [🌐 Site ↗](https://netforge.ebenmonney.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/quickapp/)</sub>

<a name="lastsaas"></a>
### #&#8288;88 [lastsaas](https://github.com/metavert-io/lastsaas) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (1) · Freshness: active (93) · Maintenance: weak (10) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 180 · MIT · Oct 2026</sub>

**Go and React multi-tenant SaaS boilerplate with Stripe billing and admin UI.**

LastSaaS is a SaaS starter with a Go backend and React + TypeScript frontend, backed by MongoDB. It includes multi-tenant accounts with owner/admin/user roles, JWT and OAuth login, MFA, Stripe subscriptions and credit bundles, white-label branding, API keys, outgoing webhooks, and an admin dashboard. It also ships a read-only MCP server (stdio) for querying admin data from Claude.

- **+** Broad built-in scope: tenants, RBAC, Stripe billing, credits, webhooks, API keys, admin UI
- **+** Go backend ships as a small container; README cites a 14MB Alpine image
- **+** Read-only MCP server exposes admin data (ARR, logs, health) to Claude over stdio
- **+** MIT license; includes health monitoring and product analytics dashboards out of the box
- **−** Requires MongoDB; no option for a relational database
- **−** Depends on Stripe for billing and Resend for email
- **−** Deployment docs target Fly.io; other hosts are not covered in the visible README
- **−** AI features are limited to the admin MCP server, not an in-app model layer

<sub>Go · Needs MongoDB, Stripe, Resend · Docker · env example file · [Repo](https://github.com/metavert-io/lastsaas) · [🌐 Site ↗](https://metavert.io/lastsaas) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lastsaas/)</sub>

<a name="extro"></a>
### #&#8288;89 [extro](https://github.com/turbostarter/extro) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 414 · MIT · Aug 2026</sub>

**WXT and React browser extension starter with Supabase auth and AI.**

Bun-based WXT project for Chrome (MV3) and Firefox (MV2) with every entrypoint (popup, side panel, devtools, new tab, options, content) preconfigured, Supabase OAuth shared across pages, storage, messaging, i18n, OpenPanel analytics, shadcn/ui, Biome, unit tests and a publish workflow. Native AI integration is marked experimental. For teams shipping a React extension with accounts; billing is marked coming soon.

- **+** All extension entrypoints wired, including side panel and devtools
- **+** Auth session and storage shared between popup, content and options pages
- **+** CI publishing to Chrome Web Store and Firefox Add-ons
- **+** Plasmo variant maintained on a separate branch
- **−** AI integration is marked experimental and thinly documented in the README
- **−** Billing is listed as coming soon
- **−** Firefox builds target MV2 and load only in temporary mode
- **−** Requires Bun

<sub>TypeScript, Vercel AI SDK, browser built-in AI (experimental) · Needs Supabase project, OpenPanel (analytics, optional) · GitHub template · env example file · [Repo](https://github.com/turbostarter/extro) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/extro/)</sub>

<a name="react-native-ai"></a>
### #&#8288;90 [react-native-ai](https://github.com/dabit3/react-native-ai) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (12) · Freshness: active (88) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Jul 2026</sub>

**Expo chat and image app with an Express proxy for multiple LLMs.**

Scaffolded with npx rn-ai: an Expo React Native app with streaming chat and image screens plus an Express server that proxies to OpenAI, Anthropic, Gemini, Z.ai GLM 5.2 and Moonshot Kimi K2.7, with Gemini image generation. Keys stay in server/.env; five themes ship and models are added by editing constants.ts and a server route. For teams starting a mobile AI assistant with keys off the device.

- **+** Server proxy keeps API keys off the device and leaves room for auth
- **+** Streaming responses from all five LLM providers
- **+** Gemini image generation wired on the server
- **+** Five themes with a documented pattern for adding more
- **−** Adding a model touches the app screen, constants, utils and a server route
- **−** No auth implemented; the proxy is where you add it
- **−** No persistence of chats described
- **−** Last commit 2026-07

<sub>TypeScript, OpenAI, Anthropic, Google Gemini, Z.ai · Needs OpenAI, Anthropic, Gemini, Z.ai or Moonshot API keys, GEMINI_API_KEY for images · GitHub template · [Repo](https://github.com/dabit3/react-native-ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-native-ai/)</sub>

<a name="ant-design-pro-blazor"></a>
### #&#8288;91 [ant-design-pro-blazor](https://github.com/ant-design-blazor/ant-design-pro-blazor) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (6) · Freshness: recent (58) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 835 · Apache-2.0 · Jun 2026</sub>

**Ant Design Pro admin UI as a Blazor dotnet project template.**

A `dotnet new` template that scaffolds a Blazor enterprise admin app based on Ant Design Pro, with prebuilt pages for dashboards, forms, lists, profiles, account, result, exception and login/register. It can target webapp, wasm or server hosting and use plain CSS or Less for themes. It has no AI features, so it fits this list only as a generic app starter.

- **+** Installs via `dotnet new install AntDesign.Templates`; no manual cloning needed
- **+** Supports webapp, wasm and server hosting models via `--host`
- **+** Ships many prebuilt pages: dashboards, step forms, lists, profiles, login, error pages
- **+** Optional Less theme compilation via `--styles less`
- **−** No AI functionality; unrelated to model or LLM workflows
- **−** README mentions no auth backend, billing or database wiring
- **−** Last release is 2025-05-13, older than the latest commits
- **−** Full page set requires the `--full` flag; default output is smaller

<sub>HTML · Needs .NET SDK, NodeJS (only for Less styles) · GitHub template · [Repo](https://github.com/ant-design-blazor/ant-design-pro-blazor) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ant-design-pro-blazor/)</sub>

<a name="saas-starter-kit"></a>
### #&#8288;92 [saas-starter-kit](https://github.com/boxyhq/saas-starter-kit) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (49) · Freshness: slowing (45) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · Apache-2.0 · May 2026</sub>

**Next.js SaaS boilerplate with teams, SAML SSO, SCIM and audit logs.**

Next.js and TypeScript boilerplate for multi-tenant SaaS apps, using Prisma on Postgres and NextAuth.js for login. It includes team management, roles and permissions, SAML SSO and SCIM directory sync via BoxyHQ Jackson, Svix webhooks, Retraced audit logs and Stripe payments. It has no AI features built in; those are left to the user.

- **+** Enterprise features included: SAML SSO, SCIM directory sync, audit logs, roles and permissions
- **+** Login via email/password, magic link, Google and GitHub through NextAuth.js
- **+** Playwright E2E tests and a docker-compose file with Postgres for local setup
- **+** Deploy buttons for Vercel, Heroku and DigitalOcean
- **−** No AI features or model integrations; the AI part is entirely up to you
- **−** Billing and subscriptions are listed under Coming Soon; only Stripe payments exist
- **−** Webhooks and audit logs depend on external services (Svix, Retraced)
- **−** Unit and integration tests are not yet written; last release is 2024-12-24

<sub>TypeScript · Needs PostgreSQL, Node.js >=18, SMTP provider, Svix, Retraced, Stripe, BoxyHQ SAML Jackson · env example file · sign-in: Auth.js · [Repo](https://github.com/boxyhq/saas-starter-kit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/saas-starter-kit/)</sub>

<a name="django-react-boilerplate"></a>
### #&#8288;93 [django-react-boilerplate](https://github.com/vintasoftware/django-react-boilerplate) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (28) · Freshness: recent (62) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · May 2026</sub>

**Django REST and React TypeScript project template with Celery and Render deploy config.**

A Django project template, installed with `django-admin startproject --template`, that pairs a DRF backend with a React, TypeScript, Tailwind and Webpack frontend. It generates a TypeScript API client from the drf-spectacular OpenAPI schema and includes Celery, Sentry, Postgres, a GitHub Actions CI file and a Render blueprint. The README describes no AI features.

- **+** Typed frontend client generated from the DRF OpenAPI schema via openapi-ts
- **+** Docker Compose setup with make targets, plus a non-Docker path using SQLite or Postgres
- **+** Ships Celery, Sentry, django-csp, django-defender and WhiteNoise preconfigured
- **+** Includes render.yaml, a build script and a CI workflow file for deployment
- **−** No AI or LLM integration; it is a general Django and React starter
- **−** Media storage on S3 or similar is not supported
- **−** Celery worker is commented out in render.yaml because Render workers cost money
- **−** Schema and client must be regenerated manually after any view change unless pre-commit is enabled

<sub>Python · Needs PostgreSQL, Redis, Celery, Mailhog, Sentry, SendGrid, Render.com · [Repo](https://github.com/vintasoftware/django-react-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/django-react-boilerplate/)</sub>

<a name="nextacular"></a>
### #&#8288;94 [nextacular](https://github.com/nextacular/nextacular) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (15) · Freshness: recent (50) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · May 2026</sub>

**Next.js starter for multi-tenant SaaS with workspaces, teams and billing.**

Nextacular is a Next.js, Tailwind and Prisma starter for multi-tenant SaaS apps. It includes authentication, workspaces and teams, custom domains, email through Nodemailer, and Stripe subscription billing. The README describes no AI features; it is a general SaaS boilerplate.

- **+** Multi-tenancy, workspaces, teams and custom domains included out of the box
- **+** Auth, Stripe billing, email and Prisma database already wired in
- **+** Live demo and hosted documentation available
- **+** One-click Vercel deploy button with the required env vars listed
- **−** README lists no AI features or model integrations
- **−** Pinned to Next.js 13.1.0, Prisma 4.4.0 and Stripe 10.13.0; dependencies are dated
- **−** Last release was 2022-12-28
- **−** Needs an external SQL/PostgreSQL database and an SMTP email service

<sub>TypeScript · Needs PostgreSQL, Stripe, SMTP email service, Vercel · GitHub template · env example file · sign-in: Auth.js · [Repo](https://github.com/nextacular/nextacular) · [▶️ Demo ↗](https://demo.nextacular.co) · [📖 Docs ↗](https://docs.nextacular.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nextacular/)</sub>

<a name="saas-starter"></a>
### #&#8288;95 [saas-starter](https://github.com/nextjs/saas-starter) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: popular (74) · Freshness: quiet (10) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Dec 2025</sub>

**Next.js SaaS template with Stripe billing, email/password auth and team dashboard.**

A minimal Next.js starter with a landing page, a pricing page wired to Stripe Checkout, and a dashboard with user and team CRUD. Auth is email/password with JWTs in cookies, roles are Owner and Member, and data lives in Postgres through Drizzle. The README describes it as a learning resource and points to paid templates for fuller feature sets.

- **+** Stripe Checkout, Customer Portal and webhook handling already wired up
- **+** Small stack: Next.js, Postgres, Drizzle, shadcn/ui, with migration and seed scripts
- **+** Activity logging and Zod-validated Server Action middleware included
- **+** MIT licensed, with a live demo on Vercel
- **−** No AI features included despite the list's AI focus
- **−** Only email/password auth; no OAuth or social login mentioned
- **−** Only two roles (Owner, Member); RBAC is basic
- **−** Requires Stripe CLI and a Stripe account even for local setup

<sub>TypeScript · Needs Postgres, Stripe, Stripe CLI, pnpm · env example file · [Repo](https://github.com/nextjs/saas-starter) · [▶️ Demo ↗](https://next-saas-start.vercel.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/saas-starter/)</sub>

<a name="nextjs-billing"></a>
### #&#8288;96 [nextjs-billing](https://github.com/lmsqueezy/nextjs-billing) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (5) · Freshness: recent (78) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 743 · MIT · Jun 2026</sub>

**Next.js subscription billing starter with Lemon Squeezy and GitHub auth.**

A Next.js 14 App Router demo for subscription SaaS apps, with Lemon Squeezy billing, GitHub OAuth through Auth.js v5, and Postgres on Neon via Drizzle ORM. A webhook endpoint at /api/webhook processes subscription_created and subscription_updated events. The README notes that Lemon Squeezy's own Customer Portal covers the same features.

- **+** Auth, billing and database already wired together in one TypeScript codebase
- **+** Includes a Setup webhook action that registers the webhook via the Lemon Squeezy SDK
- **+** Drizzle with Neon serverless Postgres works with Vercel Edge Functions
- **+** MIT license
- **−** Tied to Lemon Squeezy, Neon and GitHub OAuth; swapping any means rewriting code
- **−** Only handles subscription_created and subscription_updated webhook events
- **−** Local webhook testing needs a tunnel such as ngrok or LocalCan
- **−** Pinned to Next.js 14; no release is published

<sub>TypeScript · Needs Lemon Squeezy account, Neon Postgres, GitHub OAuth app, ngrok or similar tunnel for local webhooks · env example file · sign-in: Auth.js · [Repo](https://github.com/lmsqueezy/nextjs-billing) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nextjs-billing/)</sub>

<a name="cmsaasstarter"></a>
### #&#8288;97 [cmsaasstarter](https://github.com/scosman/cmsaasstarter) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: known (30) · Freshness: slowing (46) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Mar 2026</sub>

**SvelteKit SaaS template with Supabase auth and Stripe subscriptions.**

A SvelteKit boilerplate for SaaS products covering a marketing site, blog, pricing page, user dashboard, Supabase auth and Stripe Checkout billing with a self-serve portal. Styling uses Tailwind and DaisyUI, data lives in Supabase Postgres, and the documented deployment target is Cloudflare Pages. It has no built-in AI features; it is a general SaaS base.

- **+** Auth, Stripe billing, pricing page, onboarding and settings are already wired together
- **+** Marketing, pricing and blog pages are pre-rendered; README reports 100/100 PageSpeed
- **+** Step-by-step setup docs from clone to Cloudflare deployment, plus a live demo
- **+** CI workflows for build, formatting, linting and spell checking are included
- **−** No AI functionality included; LLM features must be added yourself
- **−** Tied to Supabase for auth and database, and Stripe for payments
- **−** Manual setup of Supabase schema, auth callbacks and Stripe portal required
- **−** No Docker or compose files; self-hosting the backend means using Supabase

<sub>Svelte · Needs Supabase (Auth, Postgres), Stripe, Cloudflare Pages (suggested), Node.js / npm · GitHub template · env example file · sign-in: Supabase Auth · [Repo](https://github.com/scosman/cmsaasstarter) · [▶️ Demo ↗](https://saasstarter.work) · [📖 Docs ↗](https://github.com/CriticalMoments/CMSaasStarter#quick-start) · [🌐 Site ↗](https://saasstarter.work) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cmsaasstarter/)</sub>

<a name="startup-nextjs"></a>
### #&#8288;98 [startup-nextjs](https://github.com/nextjstemplates/startup-nextjs) <sub>score [9](../README.md#-how-we-rank "Score 9/100. Adoption: niche (21) · Freshness: quiet (10) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Dec 2025</sub>

**Next.js and Tailwind landing page template for startup and SaaS sites.**

A free Next.js 16 and Tailwind CSS v4 website template in TypeScript, with standard landing page sections, dark and light themes, and a blog layout. It is a marketing site starter with no AI features. Auth, database, payments and the Sanity-backed blog are only in the paid Pro version.

- **+** MIT licensed and allowed in commercial projects
- **+** Current stack: Next.js 16, Tailwind v4, TypeScript
- **+** Dark and light themes included
- **+** Live demos for both Free and Pro versions
- **−** No AI features in the free template
- **−** Auth, database, payments and functional blog are Pro only
- **−** One homepage variation in the free version
- **−** No email support in the free version

<sub>TypeScript · GitHub template · [Repo](https://github.com/nextjstemplates/startup-nextjs) · [▶️ Demo ↗](https://startup.nextjstemplates.com/) · [📖 Docs ↗](https://nextjstemplates.com/docs) · [🌐 Site ↗](https://nextjstemplates.com/templates/startup) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/startup-nextjs/)</sub>

<a name="chadnext"></a>
### #&#8288;99 [chadnext](https://github.com/moinulmoin/chadnext) <sub>score [7](../README.md#-how-we-rank "Score 7/100. Adoption: niche (13) · Freshness: quiet (9) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Dec 2025</sub>

**Next.js starter template with auth, Prisma database and UI components.**

ChadNext is a Next.js starter template with simple authentication, a Prisma-backed database and a prebuilt UI library. Setup is clone, pnpm install, fill in .env, run `pnpm prisma db push`, then `pnpm dev`. A Vercel deploy button is included. The README does not mention any AI features.

- **+** Vercel deploy button with the required env vars listed
- **+** Env vars indicate GitHub auth, Resend email and UploadThing uploads are wired in
- **+** MIT licensed TypeScript codebase
- **+** Short setup: five steps from clone to dev server
- **−** README describes no AI features or model integrations
- **−** Last release is 2024-11-23
- **−** Needs several external accounts and keys before it runs
- **−** README gives no docs, demo or database engine details

<sub>TypeScript · Needs Prisma, GitHub OAuth, Resend, UploadThing, Vercel, pnpm · GitHub template · env example file · [Repo](https://github.com/moinulmoin/chadnext) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chadnext/)</sub>

<a name="shadboard"></a>
### #&#8288;100 [shadboard](https://github.com/qualiora/shadboard) <sub>score [4](../README.md#-how-we-rank "Score 4/100. Adoption: niche (4) · Freshness: quiet (9) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 741 · MIT · Dec 2025</sub>

**Next.js 15 and shadcn/ui admin dashboard template with auth and prebuilt apps.**

Shadboard is an admin dashboard template built on Next.js 15, React 19, Tailwind CSS 4 and shadcn/ui. It ships NextAuth.js authentication, i18n, a theme customizer, and prebuilt pages such as email, chat, calendar, kanban, pricing and account settings. The README describes no AI features; it is a general UI starter.

- **+** Current stack: Next.js 15, React 19, Tailwind CSS 4, shadcn/ui
- **+** Includes sign-in, register, forgot-password and verify-email pages with NextAuth.js
- **+** Prebuilt email, chat, calendar and kanban apps plus billing and settings pages
- **+** Built-in i18n and a theme customizer for colors, radii and modes
- **−** No AI or model integration; the chat page is a UI app, not an LLM client
- **−** No Docker or compose files in the repo
- **−** Last release is June 2025, so versions may lag current Next.js
- **−** Billing and payment are UI pages; no payment provider integration is described

<sub>TypeScript · [Repo](https://github.com/qualiora/shadboard) · [▶️ Demo ↗](https://shadboard.vercel.app/) · [📖 Docs ↗](https://shadboard.vercel.app/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shadboard/)</sub>

<a name="next-ai-starter"></a>
### #&#8288;101 [next-ai-starter](https://github.com/kleneway/next-ai-starter) <sub>score [4](../README.md#-how-we-rank "Score 4/100. Adoption: niche (3) · Freshness: quiet (0) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 510 · MIT · Oct 2025</sub>

**Next.js 14, tRPC and Prisma starter with LLM SDKs and agent checklists.**

A Next.js 14 App Router template with tRPC, Prisma on Supabase Postgres, NextAuth, Resend email, S3 uploads and Inngest background jobs, plus SDK wiring for OpenAI, Anthropic, Perplexity and Groq. Its distinctive part is agent-helpers/ (a task checklist, scratchpad and logs) and Cursor slash commands that drive AI coding tools through the backlog; there is no billing. For solo builders working through an AI coding assistant.

- **+** Auth, database, email, uploads and background jobs wired
- **+** agent-helpers workflow and Cursor commands are ready for AI-assisted development
- **+** Database is swappable through DATABASE_URL; no Supabase client lock-in
- **−** Next.js 14 and dated model names (Sonnet 3.5, GPT-4); upgrade before use
- **−** No billing or usage metering
- **−** Author accepts no feature PRs; last commit 2025-10
- **−** No tests or Docker

<sub>TypeScript, openai, anthropic, perplexity, groq · Needs postgres, resend, aws-s3, inngest, model-api-keys · GitHub template · env example file · sign-in: Auth.js · [Repo](https://github.com/kleneway/next-ai-starter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/next-ai-starter/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
