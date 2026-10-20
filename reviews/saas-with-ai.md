# 💳 SaaS and app starters reviews · Best of Vibe Coding

Product boilerplates with auth, billing and a database wired in and AI built in, plus mobile and browser-extension starters. Back to the [leaderboard](../README.md#-saas-and-app-starters).

<sub>🌐 Also on the web: [SaaS and app starters on archestack.com](https://archestack.com/best-of-vibe-coding/saas-with-ai/), each project on its own page.</sub>

<a name="ant-design-pro"></a>
### 🥇 [ant-design-pro](https://github.com/ant-design/ant-design-pro) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: fair (57) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Oct 2026</sub>

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

<a name="next-js-boilerplate"></a>
### 🥈 [next-js-boilerplate](https://github.com/ixartz/next-js-boilerplate) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (86) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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
### 🥉 [dotnet-starter-kit](https://github.com/fullstackhero/dotnet-starter-kit) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (56) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · MIT · Oct 2026</sub>

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

<a name="react-starter-kit"></a>
### #&#8288;4 [react-starter-kit](https://github.com/kriasoft/react-starter-kit) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (78) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<a name="hackathon-starter"></a>
### #&#8288;5 [hackathon-starter](https://github.com/sahat/hackathon-starter) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (89) · Freshness: active (94) · Maintenance: fair (50) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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

<a name="velobase-harness"></a>
### #&#8288;6 [velobase-harness](https://github.com/velobase/velobase-harness) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: fair (75) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 613 · MIT · Oct 2026</sub>

**Next.js AI SaaS base with credits, usage billing, workers and anti-abuse.**

A Next.js 15 and tRPC application with Prisma on Postgres and BullMQ on Redis that already has accounts, subscriptions, a credit ledger, Stripe and NowPayments, entitlement checks, affiliate accounting, server-side attribution, anti-abuse controls (rate limits, Turnstile, disposable-email checks), lifecycle email, an admin area and a multi-provider AI chat module. One command starts Postgres and Redis in Docker. For builders turning an AI prototype into a paid product.

- **+** Credit ledger, usage metering and entitlements are built in, not left to you
- **+** Anti-abuse for free credits: rate limits, Turnstile, disposable-email checks, clawbacks
- **+** Runs as one process or split web, worker and API by SERVICE_MODE
- **+** Docker compose, English and Chinese docs, AGENTS.md and CLAUDE.md
- **−** No unit-test script; only service-mode smoke tests
- **−** Large surface area; the framework guide asks for domain design before coding
- **−** Payments are Stripe and NowPayments; others need adapters
- **−** Seed shows 607 stars; young project

<sub>TypeScript, ai-sdk, openai, anthropic, google · Needs postgres, redis, docker, stripe, model-api-keys · GitHub template · Docker · env example file · sign-in: Auth.js · [Repo](https://github.com/velobase/velobase-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/velobase-harness/)</sub>

<a name="open-saas"></a>
### #&#8288;7 [open-saas](https://github.com/wasp-lang/open-saas) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

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

<a name="gin-vue-admin"></a>
### #&#8288;8 [gin-vue-admin](https://github.com/flipped-aurora/gin-vue-admin) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (57) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Oct 2026</sub>

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

<a name="saas-boilerplate"></a>
### #&#8288;9 [saas-boilerplate](https://github.com/ixartz/saas-boilerplate) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (49) · Freshness: active (100) · Maintenance: patchy (47) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Aug 2026</sub>

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

<a name="next-forge"></a>
### #&#8288;10 [next-forge](https://github.com/vercel/next-forge) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (53) · Freshness: active (83) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · May 2026</sub>

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

<a name="extro"></a>
### #&#8288;11 [extro](https://github.com/turbostarter/extro) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: weak (10) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 413 · MIT · Aug 2026</sub>

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
### #&#8288;12 [react-native-ai](https://github.com/dabit3/react-native-ai) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (19) · Freshness: active (97) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Jul 2026</sub>

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

<a name="ai-fullstack-saas-boilerplate"></a>
### #&#8288;13 [AI-Fullstack-SaaS-Boilerplate](https://github.com/alan345/ai-fullstack-saas-boilerplate) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (22) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

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
### #&#8288;14 [lastsaas](https://github.com/jonradoff/lastsaas) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: niche (2) · Freshness: active (95) · Maintenance: weak (10) · Easy to run: hard (17) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 176 · MIT · Oct 2026</sub>

**Go multi-tenant SaaS kit with Stripe billing and an MCP admin server.**

A Go backend with a React frontend served from the same binary: multi-tenant accounts with owner, admin and user roles, JWT with refresh rotation, OAuth, magic links and TOTP, Stripe subscriptions, per-seat pricing, trials and credit bundles, white-label branding, scoped API keys, 19 signed outgoing webhooks, analytics and health monitoring on MongoDB. The AI part is a stdio MCP server exposing 32 read-only admin tools. For founders who want a Go SaaS base an agent can query.

- **+** Credit buckets, entitlement middleware and billing enforcement are implemented
- **+** Outgoing webhooks with HMAC signing and delivery tracking; scoped API keys
- **+** MCP server gives Claude read-only access to ARR, logs, health and users
- **+** CI with coverage reporting; 14 MB Alpine image; Fly.io deploy
- **−** No model calls in the product itself; AI access is the MCP admin server
- **−** MongoDB, not Postgres; migrations and queries are Mongo-specific
- **−** One author; seed shows 173 stars
- **−** Last commit 2026-03

<sub>Go, mcp · Needs mongodb, stripe, resend · Docker · env example file · [Repo](https://github.com/jonradoff/lastsaas) · [🌐 Site ↗](https://metavert.io/lastsaas) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lastsaas/)</sub>

<a name="wave"></a>
### #&#8288;15 [wave](https://github.com/thedevdojo/wave) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (41) · Freshness: recent (78) · Maintenance: weak (0) · Easy to run: hard (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · May 2026</sub>

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
### #&#8288;16 [saas-starter-kit](https://github.com/boxyhq/saas-starter-kit) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (33) · Freshness: recent (51) · Maintenance: weak (0) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · Apache-2.0 · May 2026</sub>

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

<a name="next-ai-starter"></a>
### #&#8288;17 [next-ai-starter](https://github.com/kleneway/next-ai-starter) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (11) · Freshness: quiet (0) · Maintenance: weak (0) · Easy to run: easy (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 511 · MIT · Oct 2025</sub>

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

<a name="saas-starter"></a>
### #&#8288;18 [saas-starter](https://github.com/nextjs/saas-starter) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: popular (71) · Freshness: quiet (19) · Maintenance: weak (6) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Dec 2025</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
