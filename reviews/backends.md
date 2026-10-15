# 🗄️ Backends and databases reviews · Best of Vibe Coding

Open-source backends you ship apps on: auth, database, storage and APIs in one, self-hosted or managed. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-and-databases).

<sub>🌐 Also on the web: [Backends and databases on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="appwrite"></a>
### 🥇 [appwrite](https://github.com/appwrite/appwrite) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: very easy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · BSD-3-Clause · Oct 2026</sub>

**Self-hostable backend with auth, databases, storage, functions, messaging and hosting.**

Appwrite is a backend platform that bundles Auth, Databases, Storage, Functions, Sites, Messaging, Realtime and a Firewall behind REST, GraphQL and WebSocket APIs. It runs as a managed cloud or self-hosted via a Docker installer, and offers a hosted MCP server so coding agents can operate on a live project. Client and server SDKs cover Web, Flutter, Apple, Android, React Native, Unity, Node.js, Python, PHP, Go, Rust and others.

- **+** One Docker-based installer sets up the full stack, with Compose and env files also published
- **+** SDKs for 6 client and 10 server platforms, plus REST, GraphQL and Realtime APIs
- **+** Hosted MCP server uses OAuth, so no API keys are needed on Cloud
- **+** Same product runs on managed Cloud or on your own infrastructure
- **−** Installer needs access to the Docker socket on the host
- **−** Self-hosted instances must use a separate local MCP server, not the hosted one
- **−** Hybrid monolith-plus-workers architecture means many services to operate
- **−** RAM and CPU requirements are not stated in the README

<sub>no GPU · Docker + Compose · Needs Docker · port 20080 · [Repo](https://github.com/appwrite/appwrite) · [▶️ Demo ↗](https://cloud.appwrite.io) · [📖 Docs ↗](https://appwrite.io/docs) · [🌐 Site ↗](https://appwrite.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/appwrite/)</sub>

<a name="supabase"></a>
### 🥈 [supabase](https://github.com/supabase/supabase) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (72) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 112k · Apache-2.0 · Oct 2026</sub>

**Postgres backend with auth, storage, realtime and edge functions.**

Supabase bundles a Postgres database with generated REST and GraphQL APIs, JWT-based auth, S3-backed file storage, realtime change feeds over websockets, and edge functions. It also includes a vector and embeddings toolkit for AI workloads. It runs as a hosted platform, can be self-hosted, or run locally, and has official clients for JavaScript, Flutter, Swift and Python.

- **+** Built on Postgres, PostgREST, GoTrue and Realtime, so the data layer is plain SQL
- **+** Official clients for JavaScript/TypeScript, Flutter, Swift and Python
- **+** Hosted, self-hosted and local development options
- **+** Apache-2.0 license; vector and embeddings toolkit included
- **−** Many separate services to run when self-hosting; README gives no resource requirements
- **−** Go, Java, Rust, Ruby and C# clients are community-maintained, some partial
- **−** Repo has no Docker or compose files; self-hosting is documented elsewhere

<sub>no GPU · Compose · Needs PostgreSQL, S3-compatible storage, Envoy · [Repo](https://github.com/supabase/supabase) · [📖 Docs ↗](https://supabase.com/docs) · [🌐 Site ↗](https://supabase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase/)</sub>

<a name="parse-server"></a>
### 🥉 [parse-server](https://github.com/parse-community/parse-server) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (78) · Easy to run: easy (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

**Node.js backend with REST and GraphQL APIs on MongoDB or PostgreSQL.**

Parse Server is a self-hosted backend that runs on Node.js, either standalone via the parse-server CLI or mounted on an Express app. It exposes REST and GraphQL APIs backed by MongoDB or PostgreSQL (with PostGIS), and adds Cloud Code, Live Query, push notifications, file adapters and per-key access scopes. Official Parse SDKs cover the major client platforms.

- **+** Runs standalone or embedded in an existing Express app
- **+** Supports both MongoDB (7, 8) and PostgreSQL (16-18) with PostGIS
- **+** Includes Cloud Code, Live Query, GraphQL, push and pluggable file storage adapters
- **+** Fine-grained access scopes: master, read-only master, session and maintenance keys
- **−** No built-in admin UI in this repo; a separate dashboard project is needed
- **−** Requires you to provision and operate your own MongoDB or PostgreSQL
- **−** Docker image must be built from the repo; README shows no prebuilt image or compose file
- **−** Node.js version support is tied to specific majors and shifts with each release

<sub>no GPU · Docker · Needs Node.js 20, 22 or 24, MongoDB 7/8 or PostgreSQL 16-18 with PostGIS · port 1337 · [Repo](https://github.com/parse-community/parse-server) · [📖 Docs ↗](http://docs.parseplatform.org/parse-server/guide/) · [🌐 Site ↗](http://parseplatform.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/parse-server/)</sub>

<a name="graphql-engine"></a>
### #&#8288;4 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (82) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Oct 2026</sub>

**GraphQL API layer over Postgres, MongoDB, ClickHouse and SQL Server.**

Hasura GraphQL Engine exposes data from PostgreSQL and its flavors, MongoDB, ClickHouse and MS SQL Server through a single GraphQL endpoint. Custom business logic can be added with TypeScript, Python and Go connector SDKs. The repo is a mono-repo holding the V3 engine (which powers Hasura DDN) and the stable V2 engine, with all data connectors open source.

- **+** Supports PostgreSQL, MongoDB, ClickHouse and MS SQL Server as data sources
- **+** Connector SDKs in TypeScript, Python and Go for custom logic
- **+** Core engines and data connectors are Apache-2.0 licensed
- **+** V2 remains available as the current stable version
- **−** Large mono-repo with long history; README recommends shallow or sparse clones
- **−** V2 and V3 are separate codebases with separate docs
- **−** V3 is documented around the hosted Hasura DDN workflow
- **−** README lists no RAM, port or AI model details

<sub>no GPU · Compose · Needs PostgreSQL, MongoDB, ClickHouse, MS SQL Server · [Repo](https://github.com/hasura/graphql-engine) · [📖 Docs ↗](https://hasura.io/docs/3.0/) · [🌐 Site ↗](https://hasura.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphql-engine/)</sub>

<a name="spacetimedb"></a>
### #&#8288;5 [spacetimedb](https://github.com/clockworklabs/spacetimedb) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (83) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Oct 2026</sub>

**Relational database that runs your app logic as modules and syncs clients live.**

SpacetimeDB is a relational database that doubles as the application server. You write tables and reducers as a module in Rust, C#, TypeScript or C++, upload it, and clients connect directly, subscribe to tables and receive committed changes automatically. State is held in memory with an on-disk commit log for durability, and reducers run as ACID transactions.

- **+** Replaces the API server and pub/sub layer: clients subscribe to tables and get pushed updates
- **+** Module languages: Rust, C#, TypeScript, C++; client SDKs include React hooks, Unity and Unreal
- **+** Reducers are ACID transactions; confirmed reads wait for commit log durability by default
- **+** Used for the full backend of the MMORPG BitCraft Online
- **−** BSL 1.1 license, converting to AGPL v3.0 with linking exception after a few years
- **−** Aimed at low-latency transactional workloads, not batch or analytical queries
- **−** Application logic lives inside the database, tying the app to its module model
- **−** RAM requirements are unknown, though all application state is held in memory

<sub>no GPU · Docker + Compose · port 3000 · [Repo](https://github.com/clockworklabs/spacetimedb) · [📖 Docs ↗](https://spacetimedb.com/docs) · [🌐 Site ↗](https://spacetimedb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spacetimedb/)</sub>

<a name="insforge"></a>
### #&#8288;6 [insforge](https://github.com/insforge/insforge) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (82) · Easy to run: easy (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

**Postgres-based backend platform that coding agents operate through an MCP server.**

InsForge bundles Postgres, auth, S3-compatible storage, edge functions, an OpenAI-compatible model gateway and site deployment behind an MCP server. Coding agents read docs, schemas and logs, and run migrations, deploy functions and create buckets as tools. Self-hosting uses Docker Compose with generated secrets; a hosted cloud edition also exists.

- **+** Covers auth, Postgres, storage, edge functions and model gateway in one stack
- **+** MCP server exposes schemas, logs and config so agents can verify their own work
- **+** Setup script generates JWT, encryption and database secrets into a mode 600 .env
- **+** Storage can use local disk, bundled MinIO or RustFS, or any S3-compatible store
- **−** CLI + Skills interface is cloud only; self-hosted gets the MCP server only
- **−** Compute (long-running containers) is in private preview
- **−** Resource requirements such as RAM are not documented in the README
- **−** Running several instances needs manual per-project names and port overrides

<sub>no GPU · Docker + Compose · Needs Docker with Compose v2, Postgres, S3-compatible store (optional) · Models: OpenAI-compatible gateway across multiple LLM providers · port 7130 · [Repo](https://github.com/insforge/insforge) · [📖 Docs ↗](https://docs.insforge.dev/introduction) · [🌐 Site ↗](https://insforge.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/insforge/)</sub>

<a name="payload"></a>
### #&#8288;7 [payload](https://github.com/payloadcms/payload) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (75) · Easy to run: hard (0) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 45k · MIT · Oct 2026</sub>

**Next.js-native headless CMS and app framework with a React admin panel.**

Payload installs into an existing Next.js /app folder and provides a TypeScript headless CMS with auth, versions and drafts, localization, and a customizable React admin. Server components can query the database directly without REST or GraphQL. The README lists website and ecommerce templates plus one-click deploys to Vercel (Neon, Vercel Blob) and Cloudflare (Workers, R2, D1).

- **+** Installs inside an existing Next.js /app folder, so frontend and backend share one codebase
- **+** Auth, versions and drafts, localization, and field-level access control are built in
- **+** Generates TypeScript types for your data; hooks exist at document and field level
- **+** One-click deploy to Vercel (Neon, Blob) or Cloudflare (Workers, R2, D1)
- **−** README does not mention built-in AI features; it is a general CMS
- **−** Tied to Next.js and TypeScript for its native setup
- **−** Supported databases and minimum resources are not stated in the README
- **−** v2 to v3 required a migration guide, so older projects need upgrade work

<sub>no GPU · Needs Next.js, Database (Neon Postgres or Cloudflare D1 in one-click deploys) · [Repo](https://github.com/payloadcms/payload) · [📖 Docs ↗](https://payloadcms.com/docs/getting-started/what-is-payload) · [🌐 Site ↗](https://payloadcms.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/payload/)</sub>

<a name="convex-backend"></a>
### #&#8288;8 [convex-backend](https://github.com/get-convex/convex-backend) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: fair (71) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · custom license · Oct 2026</sub>

**Reactive database with TypeScript server functions and client libraries.**

Convex is a reactive database where queries and mutations are written as TypeScript server functions, with client libraries that keep app data live-updating. The backend is a Rust codebase with a JS runtime for user-defined functions. It can be used on Convex's cloud platform or self-hosted with Docker or a prebuilt binary, and the self-hosted version includes the dashboard and CLI.

- **+** Server logic and queries written in plain TypeScript with strong consistency
- **+** Self-hosted build includes the dashboard and CLI, with Docker or prebuilt binary options
- **+** Works with external databases such as Postgres, SQLite and RDS when self-hosting
- **+** Repository is synced with internal development within a handful of days
- **−** Test frameworks, including randomized tests, are not included in the open source repo
- **−** Self-hosted builds send an anonymous beacon unless started with --disable-beacon
- **−** Less tested on Windows than on Linux and Mac
- **−** License is not identified as a standard SPDX license (NOASSERTION)

<sub>no GPU · Needs Postgres, MySQL or SQLite (optional, self-hosted) · [Repo](https://github.com/get-convex/convex-backend) · [📖 Docs ↗](https://docs.convex.dev/) · [🌐 Site ↗](https://convex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/convex-backend/)</sub>

<a name="apijson"></a>
### #&#8288;9 [apijson](https://github.com/apijson/apijson) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Oct 2026</sub>

**Java ORM that exposes CRUD APIs over JSON requests without per-endpoint code.**

APIJSON is a Java library and JSON-based protocol. Clients send a JSON describing the tables and fields they want, and the server maps it to SQL and returns JSON in the same shape, so backend developers write no per-endpoint CRUD code. It covers reads, writes, fuzzy search and remote function calls, and ships with API docs and test tooling (APIAuto).

- **+** One JSON request can query several related tables, replacing multiple endpoint calls
- **+** Many data sources listed: MySQL, PostgreSQL, Oracle, SQL Server, ClickHouse, Redis, Kafka, Elasticsearch
- **+** Added via Maven or Gradle through JitPack; works with Spring, SpringBoot, JFinal, Nutz
- **+** Community ports listed for Go, C#, PHP, Node.js, Python and Rust
- **−** Java-centric; non-Java ports are separate third-party repositories with unknown maturity
- **−** License is reported as NOASSERTION, so terms need checking before use
- **−** README gives no setup steps for a standalone server; points to a separate demo repo
- **−** Not AI-specific; it is a general ORM and API protocol

<sub>no GPU · Needs Java 1.8+, A supported database (e.g. MySQL 5.7+, PostgreSQL 9.5+) · [Repo](https://github.com/apijson/apijson) · [▶️ Demo ↗](http://apijson.cn/api) · [📖 Docs ↗](https://github.com/APIJSON/APIJSON/blob/master/Document.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apijson/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
