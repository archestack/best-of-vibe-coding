# 💳 SaaS and app starters reviews · Best of Vibe Coding

Product boilerplates with auth, billing and a database wired in and AI built in, plus mobile and browser-extension starters. Back to the [leaderboard](../README.md#-saas-and-app-starters).

<sub>🌐 Also on the web: [SaaS and app starters on archestack.com](https://archestack.com/best-of-vibe-coding/saas-with-ai/), each project on its own page.</sub>

<a name="start-ui-web"></a>
### 🥇 [start-ui-web](https://github.com/bearstudio/start-ui-web) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (19) · Freshness: active (100) · Easy to run: very easy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**TanStack Start web app starter with oRPC, Prisma, Better Auth and shadcn/ui.**

Full-stack web starter from BearStudio, scaffolded with `pnpm create start-ui -t web`. It combines TanStack Start, React, Tailwind, shadcn/ui, oRPC, Prisma on PostgreSQL and Better Auth, with Storybook, Vitest and Playwright set up. It has no AI features of its own; it is a general web app boilerplate.

- **+** Auth, Prisma/PostgreSQL, S3-compatible storage and email run locally through a Docker Compose stack
- **+** Includes Storybook, Vitest and Playwright E2E, plus react-email templates with a preview server
- **+** Generates OpenAPI docs for the backend at /api/openapi/app
- **+** Production Dockerfile runs as non-root user on port 3000 with a HEALTHCHECK
- **−** No AI or model integration in the README; it is a generic web starter
- **−** Billing is not mentioned in the README
- **−** Needs Node.js 22 or newer, pnpm, and Docker or a PostgreSQL database
- **−** Uses the TypeScript 7 native compiler, so editors need a separate extension to match CI

<sub>TypeScript · Needs Node.js >= 22, pnpm, PostgreSQL, Docker, S3-compatible storage, SMTP server · GitHub template · Docker · [Repo](https://github.com/bearstudio/start-ui-web) · [📖 Docs ↗](https://docs.web.start-ui.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/start-ui-web/)</sub>

<a name="next-js-boilerplate"></a>
### 🥈 [next-js-boilerplate](https://github.com/ixartz/next-js-boilerplate) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<a name="dotnet-starter-kit"></a>
### 🥉 [dotnet-starter-kit](https://github.com/fullstackhero/dotnet-starter-kit) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (56) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · MIT · Oct 2026</sub>

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

<a name="twenty"></a>
### #&#8288;4 [twenty](https://github.com/twentyhq/twenty) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: hard (0) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · custom license · Oct 2026</sub>

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

<a name="ant-design-pro"></a>
### #&#8288;5 [ant-design-pro](https://github.com/ant-design/ant-design-pro) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (53) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Oct 2026</sub>

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

<a name="react-starter-kit"></a>
### #&#8288;6 [react-starter-kit](https://github.com/kriasoft/react-starter-kit) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (85) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<a name="next-shadcn-dashboard-starter"></a>
### #&#8288;7 [next-shadcn-dashboard-starter](https://github.com/kiranism/next-shadcn-dashboard-starter) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (50) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.2k · MIT · Oct 2026</sub>

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

<a name="basic"></a>
### #&#8288;8 [basic](https://github.com/fantastic-admin/basic) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (61) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="create-better-t-stack"></a>
### #&#8288;9 [create-better-t-stack](https://github.com/amanvarshney01/create-better-t-stack) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (96) · Easy to run: hard (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · MIT · Oct 2026</sub>

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

<a name="saas-boilerplate"></a>
### #&#8288;10 [saas-boilerplate](https://github.com/ixartz/saas-boilerplate) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (47) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Aug 2026</sub>

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

<a name="hackathon-starter"></a>
### #&#8288;11 [hackathon-starter](https://github.com/sahat/hackathon-starter) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (92) · Freshness: active (94) · Maintenance: fair (50) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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

<a name="open-saas"></a>
### #&#8288;12 [open-saas](https://github.com/wasp-lang/open-saas) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: fair (74) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

**Wasp SaaS template with auth, three payment providers, OpenAI demo app.**

A Wasp (React, Node, Prisma) SaaS template: email-verified and social auth, Stripe, Polar or Lemon Squeezy payments, cron jobs, S3 uploads, SendGrid, Mailgun or SMTP email, an admin dashboard, an Astro Starlight docs and blog site, Playwright end-to-end tests and an example OpenAI function-calling app. Scaffold with wasp new -t saas and deploy to Railway or Fly with one command. For teams that accept Wasp for a complete SaaS base.

- **+** Three payment providers and three email providers are switchable
- **+** Playwright e2e tests, admin dashboard and docs site included
- **+** One-command deploy to Railway or Fly
- **+** Live demo at opensaas.sh and a dedicated docs site
- **−** Wasp is the framework; its config DSL and release cadence become your dependency
- **−** AI part is one OpenAI example app; no usage metering or credits
- **−** Pulling template updates after forking is a documented manual process
- **−** No Docker files

<sub>MDX, openai · Needs wasp-cli, postgres, stripe-or-polar-or-lemonsqueezy, openai-api-key, aws-s3, email-provider · [Repo](https://github.com/wasp-lang/open-saas) · [▶️ Demo ↗](https://opensaas.sh) · [📖 Docs ↗](https://docs.opensaas.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-saas/)</sub>

<a name="velobase-harness"></a>
### #&#8288;13 [velobase-harness](https://github.com/velobase/velobase-harness) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: fair (75) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 614 · MIT · Oct 2026</sub>

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

<a name="gin-vue-admin"></a>
### #&#8288;14 [gin-vue-admin](https://github.com/flipped-aurora/gin-vue-admin) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: fair (57) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Oct 2026</sub>

**Go and Vue 3 admin platform with RBAC and a CRUD code generator.**

Full-stack admin framework with a Gin and GORM backend and a Vue 3 and Element Plus frontend. It ships JWT and Casbin permissions, dynamic menus and routes, a form builder and a code generator that produces basic CRUD for backend and frontend. The README also advertises an MCP integration for AI editors that drives code generation.

- **+** JWT plus Casbin role, menu and API permissions built in
- **+** Code generator produces backend and frontend CRUD from a template
- **+** Swagger docs via swag; Redis-backed multi-login limit
- **+** File upload to Qiniu, Aliyun and Tencent Cloud included
- **−** AI is limited to an MCP hook for code generation; no AI app features
- **−** No billing or tenancy described; some features need a paid license
- **−** No free technical support; paid support only
- **−** README is mainly in Chinese; no Docker setup detected

<sub>Go · Needs MySQL or MariaDB 5.7+, Redis, Go >= 1.22, Node > 18.16.0 · Docker · [Repo](https://github.com/flipped-aurora/gin-vue-admin) · [▶️ Demo ↗](http://demo.gin-vue-admin.com) · [📖 Docs ↗](https://www.gin-vue-admin.com) · [🌐 Site ↗](https://www.gin-vue-admin.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gin-vue-admin/)</sub>

<a name="next-saas-stripe-starter"></a>
### #&#8288;15 [next-saas-stripe-starter](https://github.com/mickasmt/next-saas-stripe-starter) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (83) · Easy to run: hard (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Sep 2026</sub>

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

<a name="pagoda"></a>
### #&#8288;16 [pagoda](https://github.com/mikestefanello/pagoda) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (42) · Freshness: active (100) · Maintenance: patchy (47) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Aug 2026</sub>

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

<a name="tauri-ui"></a>
### #&#8288;17 [tauri-ui](https://github.com/agmmnn/tauri-ui) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (76) · Easy to run: hard (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Aug 2026</sub>

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

<a name="startup-nextjs"></a>
### #&#8288;18 [startup-nextjs](https://github.com/nextjstemplates/startup-nextjs) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (15) · Freshness: quiet (19) · Easy to run: very easy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Dec 2025</sub>

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

<a name="apptension-saas-boilerplate"></a>
### #&#8288;19 [saas-boilerplate](https://github.com/apptension/saas-boilerplate) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (45) · Freshness: active (96) · Maintenance: weak (30) · Easy to run: hard (17) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

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

<a name="next-forge"></a>
### #&#8288;20 [next-forge](https://github.com/vercel/next-forge) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (70) · Freshness: active (82) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · May 2026</sub>

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

<a name="bullet-train"></a>
### #&#8288;21 [bullet_train](https://github.com/bullet-train-co/bullet_train) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: patchy (30) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

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

<a name="free-nextjs-admin-dashboard"></a>
### #&#8288;22 [free-nextjs-admin-dashboard](https://github.com/tailadmin/free-nextjs-admin-dashboard) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (44) · Easy to run: hard (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Sep 2026</sub>

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

<a name="scaffold-eth-2"></a>
### #&#8288;23 [scaffold-eth-2](https://github.com/scaffold-eth/scaffold-eth-2) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (27) · Freshness: recent (70) · Maintenance: weak (24) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

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

<a name="open-mercato"></a>
### #&#8288;24 [open-mercato](https://github.com/open-mercato/open-mercato) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (21) · Freshness: active (100) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

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

<a name="shipfree"></a>
### #&#8288;25 [shipfree](https://github.com/revokslab/shipfree) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (17) · Freshness: active (90) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Jun 2026</sub>

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

<sub>TypeScript · Needs Postgres, Bun, Stripe, Resend · [Repo](https://github.com/revokslab/shipfree) · [📖 Docs ↗](https://shipfree.revoks.dev/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shipfree/)</sub>

<a name="extro"></a>
### #&#8288;26 [extro](https://github.com/turbostarter/extro) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (10) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 413 · MIT · Aug 2026</sub>

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

<a name="wave"></a>
### #&#8288;27 [wave](https://github.com/thedevdojo/wave) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: popular (63) · Freshness: recent (77) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · May 2026</sub>

**Laravel SaaS framework with auth, billing, roles, blog and themes.**

Wave is a Laravel-based SaaS framework that ships the common product pieces: authentication, user profiles, impersonation, billing with subscription plans, roles and permissions, notifications, an API and an admin panel. It also includes a blog, changelog, pages, themes and plugins. The README does not mention built-in AI features, so any AI functionality would be added by the developer.

- **+** Auth, billing, subscription plans and roles/permissions are included out of the box
- **+** Ships admin panel, API, blog, changelog and user impersonation
- **+** Theme and plugin system, with a live demo that previews themes
- **+** MIT licensed, with documentation and an automated installer
- **−** No AI features described in the README; they must be added yourself
- **−** Requires a PHP and Laravel stack
- **−** Video course and premium content sit behind a paid DevDojo Pro subscription
- **−** Payment providers and database requirements are not listed in the README

<sub>CSS · Needs PHP, Laravel · env example file · [Repo](https://github.com/thedevdojo/wave) · [▶️ Demo ↗](https://devdojo.com/wave/demo) · [📖 Docs ↗](https://devdojo.com/wave/docs) · [🌐 Site ↗](https://devdojo.com/wave) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wave/)</sub>

<a name="saas-starter-kit"></a>
### #&#8288;28 [saas-starter-kit](https://github.com/boxyhq/saas-starter-kit) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: popular (56) · Freshness: recent (50) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · Apache-2.0 · May 2026</sub>

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

<a name="react-native-ai"></a>
### #&#8288;29 [react-native-ai](https://github.com/dabit3/react-native-ai) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (10) · Freshness: active (96) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Jul 2026</sub>

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

<a name="vuesion"></a>
### #&#8288;30 [vuesion](https://github.com/vuesion/vuesion) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: known (39) · Freshness: recent (73) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Aug 2026</sub>

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

<sub>Vue · Needs Nuxt, Storybook, Cypress, Vitest · Docker · [Repo](https://github.com/vuesion/vuesion) · [📖 Docs ↗](https://www.vuesion.dev/docs) · [🌐 Site ↗](https://www.vuesion.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vuesion/)</sub>

<a name="fulling"></a>
### #&#8288;31 [fulling](https://github.com/fullagent/fulling) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: known (33) · Freshness: active (99) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Jul 2026</sub>

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

<a name="ai-fullstack-saas-boilerplate"></a>
### #&#8288;32 [AI-Fullstack-SaaS-Boilerplate](https://github.com/alan345/ai-fullstack-saas-boilerplate) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (12) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

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

<a name="lastsaas"></a>
### #&#8288;33 [lastsaas](https://github.com/jonradoff/lastsaas) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (1) · Freshness: active (95) · Maintenance: weak (10) · Easy to run: hard (17) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 176 · MIT · Oct 2026</sub>

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

<sub>Go · Needs MongoDB, Stripe, Resend · Docker · env example file · [Repo](https://github.com/jonradoff/lastsaas) · [🌐 Site ↗](https://metavert.io/lastsaas) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lastsaas/)</sub>

<a name="cmsaasstarter"></a>
### #&#8288;34 [cmsaasstarter](https://github.com/scosman/cmsaasstarter) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (31) · Freshness: recent (55) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Mar 2026</sub>

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

<a name="saas-starter"></a>
### #&#8288;35 [saas-starter](https://github.com/nextjs/saas-starter) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: widely used (82) · Freshness: quiet (18) · Maintenance: weak (6) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Dec 2025</sub>

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

<a name="next-ai-starter"></a>
### #&#8288;36 [next-ai-starter](https://github.com/kleneway/next-ai-starter) <sub>score [22](../README.md#-how-we-rank "Score 22/100. Adoption: niche (6) · Freshness: quiet (0) · Maintenance: weak (0) · Easy to run: easy (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 511 · MIT · Oct 2025</sub>

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
