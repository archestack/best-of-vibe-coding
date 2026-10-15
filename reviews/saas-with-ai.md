# 💳 SaaS boilerplates reviews · Best of Vibe Coding

Product boilerplates with auth, billing and a database wired in, with AI features built in or ready to add. Back to the [leaderboard](../README.md#-saas-boilerplates).

<sub>🌐 Also on the web: [SaaS boilerplates on archestack.com](https://archestack.com/best-of-vibe-coding/saas-with-ai/), each project on its own page.</sub>

<a name="ant-design-pro"></a>
### 🥇 [ant-design-pro](https://github.com/ant-design/ant-design-pro) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (58) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Oct 2026</sub>

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
### 🥈 [next-js-boilerplate](https://github.com/ixartz/next-js-boilerplate) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<a name="react-starter-kit"></a>
### 🥉 [react-starter-kit](https://github.com/kriasoft/react-starter-kit) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (64) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Oct 2026</sub>

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

<a name="velobase-harness"></a>
### #&#8288;4 [velobase-harness](https://github.com/velobase/velobase-harness) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: fair (69) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 613 · MIT · Oct 2026</sub>

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

<a name="hackathon-starter"></a>
### #&#8288;5 [hackathon-starter](https://github.com/sahat/hackathon-starter) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: widely used (82) · Freshness: active (94) · Maintenance: fair (50) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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
### #&#8288;6 [gin-vue-admin](https://github.com/flipped-aurora/gin-vue-admin) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (73) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Oct 2026</sub>

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

<a name="open-saas"></a>
### #&#8288;7 [open-saas](https://github.com/wasp-lang/open-saas) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (60) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

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

<a name="ai-fullstack-saas-boilerplate"></a>
### #&#8288;8 [AI-Fullstack-SaaS-Boilerplate](https://github.com/alan345/ai-fullstack-saas-boilerplate) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (27) · Freshness: recent (70) · Maintenance: fair (60) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

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

<a name="next-ai-starter"></a>
### #&#8288;9 [next-ai-starter](https://github.com/kleneway/next-ai-starter) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (13) · Freshness: quiet (0) · Maintenance: weak (0) · Easy to run: easy (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 511 · MIT · Oct 2025</sub>

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

<a name="lastsaas"></a>
### #&#8288;10 [lastsaas](https://github.com/jonradoff/lastsaas) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: niche (3) · Freshness: recent (62) · Maintenance: weak (0) · Easy to run: hard (17) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 175 · MIT · Mar 2026</sub>

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

<a name="saas-starter"></a>
### #&#8288;11 [saas-starter](https://github.com/nextjs/saas-starter) <sub>score [17](../README.md#-how-we-rank "Score 17/100. Adoption: popular (54) · Freshness: quiet (21) · Maintenance: weak (6) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Dec 2025</sub>

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
