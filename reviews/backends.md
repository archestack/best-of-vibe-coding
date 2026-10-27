# 🗄️ Backends, databases and hosting reviews · Best of Vibe Coding

Open-source backends you ship apps on (auth, database, storage, APIs) and self-hosted platforms that deploy them from Git or Docker. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-databases-and-hosting).

<sub>🌐 Also on the web: [Backends, databases and hosting on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="appwrite"></a>
### 🥇 [appwrite](https://github.com/appwrite/appwrite) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · BSD-3-Clause · Oct 2026</sub>

**Backend with auth, databases, storage, functions and an MCP server for agents.**

Appwrite is a backend platform that bundles Auth, Databases, Storage, Functions, Sites, Messaging, Realtime and a Firewall behind REST, GraphQL and WebSocket APIs. It has client and server SDKs for 16 platforms and a hosted MCP server so coding agents can operate on a live project. It runs as a managed cloud or is self-hosted through a Docker-based installer.

- **+** Covers auth, databases, storage, functions, messaging and realtime in one backend
- **+** SDKs for Web, Flutter, Apple, Android, Node.js, Python, Go, Rust and more
- **+** Exposes REST, GraphQL and WebSocket APIs
- **+** Hosted MCP server uses OAuth, so no API keys are needed on Cloud
- **−** Self-hosting needs Docker and mounts the Docker socket for the installer
- **−** Hosted MCP is for Cloud; self-hosted instances need a separate local MCP server
- **−** Minimum RAM and CPU requirements are not stated in the README
- **−** Hybrid monolith with queue, workers and cache means several services to operate

<sub>no GPU · Docker + Compose · Needs Docker · port 80 · [Repo](https://github.com/appwrite/appwrite) · [▶️ Demo ↗](https://cloud.appwrite.io) · [📖 Docs ↗](https://appwrite.io/docs) · [🌐 Site ↗](https://appwrite.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/appwrite/)</sub>

<a name="supabase"></a>
### 🥈 [supabase](https://github.com/supabase/supabase) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 114k · Apache-2.0 · Oct 2026</sub>

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

<a name="dokploy"></a>
### 🥉 [dokploy](https://github.com/dokploy/dokploy) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · custom license · Oct 2026</sub>

**Self-hosted PaaS for deploying apps and databases across Docker Swarm nodes.**

Dokploy is a self-hostable platform-as-a-service that deploys applications, Docker Compose stacks and databases (MySQL, PostgreSQL, MongoDB, MariaDB, libsql, Redis) to your own servers. It uses Traefik for routing, Docker Swarm for multi-node scaling, and offers one-click open-source templates, database backups to external storage, and a CLI and API. It has no AI-specific features, so it fits as deployment infrastructure for apps built elsewhere.

- **+** Installs on a VPS with a single curl script
- **+** Native Docker Compose and Docker Swarm multi-node support
- **+** Built-in database backups, monitoring and deploy notifications
- **+** Exports logs and metrics to Grafana, Datadog, Splunk, CloudWatch and others
- **−** License is reported as NOASSERTION; terms need checking before commercial use
- **−** README gives no minimum RAM or CPU requirements
- **−** No AI features; general-purpose deployment tool only
- **−** Hosted Dokploy Cloud is offered alongside; feature split with self-hosted not stated

<sub>no GPU · Docker · Needs Docker, Docker Swarm, Traefik · [Repo](https://github.com/dokploy/dokploy) · [▶️ Demo ↗](https://app.dokploy.com) · [📖 Docs ↗](https://docs.dokploy.com) · [🌐 Site ↗](https://dokploy.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokploy/)</sub>

<a name="spacetimedb"></a>
### #&#8288;4 [spacetimedb](https://github.com/clockworklabs/spacetimedb) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Oct 2026</sub>

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

<a name="nocobase"></a>
### #&#8288;5 [nocobase](https://github.com/nocobase/nocobase) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Oct 2026</sub>

**No-code platform for building business systems, with a CLI for coding agents.**

NocoBase is a plugin-based platform for building business applications through a WYSIWYG interface, with data models, permissions, workflows and audit logs built in. It also ships a CLI (`nb`) and skills so coding agents such as Claude Code, Codex and Cursor can create data models, pages and workflows. It includes AI employees with role-based permissions, and exposes MCP and HTTP APIs for external agents.

- **+** Data stays in standard relational databases, separate from the UI
- **+** Permissions, workflows and audit logs are built-in modules, not generated code
- **+** Agents and people edit the same data models, pages and workflows
- **+** Microkernel design: features are added as official or custom plugins
- **−** License is reported as NOASSERTION; terms need checking before commercial use
- **−** README gives no RAM, database or port requirements
- **−** README does not list which LLM providers the AI employees support
- **−** Extending beyond the no-code UI requires learning its plugin architecture

<sub>Docker + Compose · Compose runs MySQL, PostgreSQL · [Repo](https://github.com/nocobase/nocobase) · [▶️ Demo ↗](https://demo.nocobase.com/new) · [📖 Docs ↗](https://docs.nocobase.com/) · [🌐 Site ↗](https://www.nocobase.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nocobase/)</sub>

<a name="payload"></a>
### #&#8288;6 [payload](https://github.com/payloadcms/payload) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Oct 2026</sub>

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

<a name="dokku"></a>
### #&#8288;7 [dokku](https://github.com/dokku/dokku) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Oct 2026</sub>

**Self-hosted mini-Heroku PaaS that deploys apps with git push.**

Dokku is a small Platform-as-a-Service that runs on a single Ubuntu or Debian VM and builds and runs applications in Docker containers. Applications are deployed over SSH, and the server is managed through the `dokku` command line, including domains and SSH keys. The README describes it as a Docker-powered mini-Heroku and does not mention any AI features.

- **+** Installs on a single VM with one bootstrap script
- **+** Supports Ubuntu 22.04/24.04/26.04 and Debian 11+ on amd64 and arm64
- **+** MIT license, with an active release history and Ubuntu and Arch packages
- **+** Written in Go, with documentation and a Slack support channel
- **−** Not an AI project; the README has no AI or model features
- **−** Targets one server; the README describes no multi-node setup
- **−** Only Ubuntu and Debian are listed as supported operating systems
- **−** Deployment and management are CLI and SSH based; the README mentions no web UI

<sub>Docker · Needs Docker, SSH keypair · [Repo](https://github.com/dokku/dokku) · [📖 Docs ↗](https://dokku.com/docs/getting-started/installation/) · [🌐 Site ↗](https://dokku.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokku/)</sub>

<a name="graphql-engine"></a>
### #&#8288;8 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Oct 2026</sub>

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

<a name="falkordb"></a>
### #&#8288;9 [falkordb](https://github.com/falkordb/falkordb) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · custom license · Oct 2026</sub>

**Property graph database on Redis with OpenCypher and sparse-matrix queries.**

FalkorDB is a property graph database built as a Redis module in Rust. It stores adjacency as GraphBLAS sparse matrices and runs OpenCypher queries (with proprietary extensions) through linear algebra. Queries go through GRAPH.QUERY from any Redis client or the official Python, Java, Node.js, Rust, Go and C# clients. It targets knowledge-graph and agent-memory backends for LLM apps.

- **+** Speaks OpenCypher, so existing Cypher queries and property-graph modeling carry over
- **+** Works with any Redis client via GRAPH.QUERY; official clients for six languages
- **+** Quick start is one docker run, with a browser UI on port 3000
- **+** Sparse-matrix storage and linear-algebra execution; benchmarks published on a separate site
- **−** SSPLv1 license is not OSI-approved and restricts offering it as a service
- **−** Building from source needs GraphBLAS, LAGraph, RediSearch and clang-23 with OpenMP
- **−** Runs as a Redis module, not a standalone server
- **−** Multi-tenant claim in the headline is not detailed in the README

<sub>no GPU · Needs Redis, GraphBLAS, LAGraph, RediSearch · port 3000 · [Repo](https://github.com/falkordb/falkordb) · [📖 Docs ↗](https://docs.falkordb.com/) · [🌐 Site ↗](https://www.falkordb.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/falkordb/)</sub>

<a name="apijson"></a>
### #&#8288;10 [apijson](https://github.com/apijson/apijson) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Oct 2026</sub>

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

<a name="parse-server"></a>
### #&#8288;11 [parse-server](https://github.com/parse-community/parse-server) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

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

<a name="insforge"></a>
### #&#8288;12 [insforge](https://github.com/insforge/insforge) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

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

<a name="nhost"></a>
### #&#8288;13 [nhost](https://github.com/nhost/nhost) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · MIT · Oct 2026</sub>

**Open-source Firebase alternative on Postgres, Hasura GraphQL, auth and storage.**

Nhost bundles PostgreSQL, a Hasura-generated GraphQL API, an auth service, file storage and Node.js serverless functions into one backend. It runs on the hosted Nhost platform, locally through the Nhost CLI, or self-hosted from an example docker-compose file. The CLI also ships an MCP server that lets coding assistants read the GraphQL schema, run allowed queries and manage metadata and migrations.

- **+** Full backend in one stack: Postgres, Hasura GraphQL, auth, storage and functions
- **+** CLI runs a local environment that tracks database migrations and Hasura metadata
- **+** Built-in MCP server in the CLI for Claude Code, Cursor, Codex and Gemini CLI
- **+** MIT licensed, with a JavaScript/TypeScript client and a Dart/Flutter client
- **−** GraphQL-first through Hasura; no REST-first or other database options are documented
- **−** Self-hosting guidance in the README is only an example docker-compose file
- **−** Serverless functions are Node.js only (JavaScript and TypeScript)
- **−** Resource requirements for self-hosting are not stated in the README

<sub>no GPU · Needs PostgreSQL, Hasura · README: alternative to Firebase · [Repo](https://github.com/nhost/nhost) · [📖 Docs ↗](https://docs.nhost.io) · [🌐 Site ↗](https://nhost.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nhost/)</sub>

<a name="convex-backend"></a>
### #&#8288;14 [convex-backend](https://github.com/convex/convex-backend) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · custom license · Oct 2026</sub>

**Reactive database with TypeScript server functions and live-updating clients.**

Convex is a reactive database where queries and mutations are written as TypeScript server functions with strong consistency. It provides client libraries for live-updating apps, and the backend is written in Rust. It runs on the Convex cloud or self-hosted via Docker or a prebuilt binary, with the dashboard and CLI included.

- **+** Database, server functions and client libraries come as one integrated backend
- **+** Self-hosting includes dashboard and CLI; works with Postgres, SQLite, Neon, RDS and others
- **+** Business logic is plain TypeScript with strong consistency
- **+** Release on 2026-10-10; repo synced with internal work within days
- **−** License is reported as NOASSERTION; terms need manual checking
- **−** Randomized and other internal test suites are not in the open source repo
- **−** Self-hosted builds send an anonymous beacon unless --disable-beacon is set
- **−** Less tested on Windows than on Linux and Mac

<sub>no GPU · Needs Docker or prebuilt binary (self-hosting) · [Repo](https://github.com/convex/convex-backend) · [📖 Docs ↗](https://docs.convex.dev/) · [🌐 Site ↗](https://convex.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/convex-backend/)</sub>

<a name="encore"></a>
### #&#8288;15 [encore](https://github.com/encoredev/encore) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MPL-2.0 · Oct 2026</sub>

**Go and TypeScript SDK that declares backend infrastructure in code.**

Encore is an infrastructure SDK for Go and TypeScript where databases, Pub/Sub topics, buckets, caches, cron jobs and secrets are declared in application code. `encore run` starts the app locally with Postgres, NSQ, Redis, tracing and a dashboard at localhost:9400. An optional commercial platform provisions the matching resources in your AWS or GCP account, or you can build a Docker image and supply your own infrastructure.

- **+** Same code runs locally with real Postgres, Pub/Sub and Redis, and deploys to AWS or GCP
- **+** SDK and CLI work without the paid platform; `encore build docker` supports self-hosting
- **+** Generates rules files for Cursor and Claude Code and runs a local MCP server
- **+** Local dashboard shows traces, APIs, databases and Pub/Sub messages
- **−** Only Go and TypeScript are supported; Python and Rust are early-access only
- **−** Automated provisioning covers AWS and GCP only; Azure is on the roadmap
- **−** Preview environments, approvals and managed provisioning need the commercial platform
- **−** Application code depends on the Encore SDK and its resource declarations

<sub>no GPU · Needs Postgres, NSQ, Redis, AWS or Google Cloud (for deployment) · port 9400 · [Repo](https://github.com/encoredev/encore) · [📖 Docs ↗](https://encore.dev/docs) · [🌐 Site ↗](https://encore.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/encore/)</sub>

<a name="pixeltable"></a>
### #&#8288;16 [pixeltable](https://github.com/pixeltable/pixeltable) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Oct 2026</sub>

**Python multimodal database with computed columns and HTTP routes in one file.**

Pixeltable stores images, video, audio and documents in tables, and treats transforms and indexes as declared columns that run on insert. Table models and FastAPI-style insert, update and compute routes are defined in one Python file and applied with the `pxt` CLI. It runs locally or on Pixeltable Cloud, which is in limited beta.

- **+** Tables, computed columns, indexes and HTTP routes declared in one Python file
- **+** Routes can be mounted on an existing FastAPI app via include_router
- **+** Native Image, Video, Audio and Document column types
- **+** Ships an agent skill, developer MCP server and Cursor/Claude/ChatGPT plugins
- **−** Pixeltable Cloud is limited beta and requires emailing for access
- **−** Uses its own TableModel schema; existing schemas must be rewritten
- **−** README gives no RAM, GPU or storage requirements
- **−** Schema and service updates are separate CLI steps

<sub>Needs Python, ANTHROPIC_API_KEY (starter chat /ask route only) · Models: Anthropic (starter kit) · [Repo](https://github.com/pixeltable/pixeltable) · [📖 Docs ↗](https://docs.pixeltable.com/) · [🌐 Site ↗](https://www.pixeltable.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pixeltable/)</sub>

<a name="zenstack"></a>
### #&#8288;17 [zenstack](https://github.com/zenstackhq/zenstack) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**Prisma-compatible TypeScript ORM with access control, built on Kysely.**

ZenStack V3 is a schema-first TypeScript ORM that keeps Prisma's schema style and query API but runs on its own engine built on Kysely, with no Rust or WASM components. It adds access control, data validation, polymorphic models, generated CRUD web APIs with framework adapters, TanStack Query hooks and Zod schemas. It is a data-layer library with no AI features.

- **+** Pure TypeScript implementation, no Rust or WASM engine
- **+** Prisma-compatible schema and query API, usable as a drop-in replacement
- **+** Typed Kysely query builder available as an escape hatch instead of raw SQL
- **+** Generates CRUD APIs, TanStack Query hooks and Zod schemas from the schema
- **−** Library only; no hosting, auth service or file storage included
- **−** Targets Node.js and Bun; other runtimes are not mentioned in the README
- **−** V3 is an engine rewrite, so Prisma feature parity needs checking
- **−** No AI features; fit with an AI project list is indirect

<sub>no GPU · Needs Node.js or Bun, Kysely · [Repo](https://github.com/zenstackhq/zenstack) · [▶️ Demo ↗](https://stackblitz.com/~/github.com/zenstackhq/v3-doc-quick-start?file=zenstack%2fschema.zmodel&file=main.ts&view=editor&showSidebar=0&hideNavigation=1&hideExplorer=1) · [📖 Docs ↗](https://zenstack.dev/docs/) · [🌐 Site ↗](https://zenstack.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zenstack/)</sub>

<a name="prest"></a>
### #&#8288;18 [prest](https://github.com/prest/prest) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Oct 2026</sub>

**REST and read-only MCP API generated from a PostgreSQL or MySQL database.**

pREST is a Go service that exposes tables in an existing PostgreSQL (9.5+) or MySQL (8.0.19+) database as REST endpoints at /{database}/{schema}/{table}, with auth, ACL and custom SQL routes. It also serves a read-only MCP endpoint so AI clients can query the same data. It can serve several databases from a registry or an allow-list.

- **+** Generates CRUD REST routes straight from an existing Postgres or MySQL schema
- **+** Custom SQL query scripts support bound parameters via sqlVal, sqlList and ident helpers
- **+** Serves multiple databases via a [[databases]] registry or pg.allowed_databases
- **+** Built-in read-only MCP endpoint, plus auth and ACL configuration
- **−** Only PostgreSQL and MySQL; MariaDB, TiDB and Aurora MySQL are roadmap items
- **−** Interpolated query-script values are screened and rejected if they contain quotes or SQL keywords
- **−** MySQL support is newer (v2.5.0) and with prepare = false interpolates placeholders
- **−** MCP endpoint is read-only, so AI clients cannot write through it

<sub>no GPU · Docker + Compose · Needs PostgreSQL 9.5+ or MySQL 8.0.19+ · [Repo](https://github.com/prest/prest) · [📖 Docs ↗](https://docs.prestd.com/) · [🌐 Site ↗](https://docs.prestd.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/prest/)</sub>

<a name="omnigraph"></a>
### #&#8288;19 [omnigraph](https://github.com/modernrelay/omnigraph) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Graph database on object storage with branching, typed schemas and hybrid retrieval.**

Omnigraph is a Rust graph database that stores data in the Lance format on local disk or S3-compatible storage. It enforces typed `.pg` schemas on write and combines graph traversal, vector search and full-text search in one query. Branching and three-way merge let agents write in isolation, and clusters are declared in `cluster.yaml` and applied with plan/apply commands.

- **+** Git-style branches, three-way merge and time travel across the whole graph
- **+** Graph traversal, vector ANN, full-text and Reciprocal Rank Fusion in one runtime
- **+** Cedar policy enforced server-side on every write path, including CLI and SDK
- **+** Open Lance storage on local disk, S3, R2, GCS or MinIO; built-in MCP endpoint
- **−** Azure storage is preview and needs an admission wrapper for writers
- **−** Managed Omnigraph Cloud is private preview, waitlist only
- **−** Custom schema and query formats (.pg, .gq) must be learned
- **−** Clients must match the server HTTP contract version, such as 0.14

<sub>Docker · Needs S3-compatible object storage (optional), protobuf-compiler (build/CI only) · Models: Embedding providers declared in cluster.yaml · [Repo](https://github.com/modernrelay/omnigraph) · [📖 Docs ↗](https://www.omnigraph.dev/llms.txt) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/omnigraph/)</sub>

<a name="nitric"></a>
### #&#8288;20 [nitric](https://github.com/nitrictech/nitric) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

**Multi-language backend framework that infers cloud infrastructure from app code.**

Nitric is a Go-based CLI and framework where you declare APIs, buckets, queues, key-value stores and SQL databases inline in application code. `nitric up` generates Pulumi or Terraform deployments for AWS, GCP or Azure, with IAM permissions derived from the access you declare. It also runs the app locally with a dashboard. It has no AI-specific features.

- **+** Infrastructure and least-privilege IAM inferred from a few lines of app code
- **+** SDKs for JavaScript, TypeScript, Python, Go and Dart
- **+** Deploys to AWS, GCP or Azure via Pulumi or Terraform providers
- **+** Custom providers supported; local run with dashboard included
- **−** Not an AI project; README mentions no model or agent features
- **−** Limited to the resource types Nitric abstracts; custom needs use escape hatches
- **−** Needs the Nitric CLI and a provider toolchain to deploy
- **−** Not a hosted backend; you still deploy to and pay for your own cloud

<sub>no GPU · Needs Pulumi or Terraform (deployment), AWS, GCP or Azure account (deployment) · [Repo](https://github.com/nitrictech/nitric) · [📖 Docs ↗](https://nitric.io/docs) · [🌐 Site ↗](https://nitric.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nitric/)</sub>

<a name="serverpod"></a>
### #&#8288;21 [serverpod](https://github.com/serverpod/serverpod) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · BSD-3-Clause · Oct 2026</sub>

**Dart backend for Flutter apps with generated client code and ORM.**

Serverpod is an app and web server written in Dart for Flutter projects. It generates client code and models by analyzing the server's endpoints, and includes an ORM, database migrations, caching, authentication, file uploads, streaming and scheduled future calls. Terraform scripts cover deployment to Google Cloud Platform and AWS.

- **+** Generates typed client code and models from server endpoints, so remote calls look like local methods
- **+** Built-in ORM with Dart types and null-safety, plus a database migration system
- **+** Distributed cache (local or Redis), authenticated socket streaming and persistent future calls
- **+** Terraform scripts for Google Cloud Platform and AWS
- **−** Main serverpod package is SSPL, not BSD-3; other packages are BSD-3
- **−** Server code must be written in Dart, which limits it mostly to Flutter teams
- **−** Built-in web server is described as experimental
- **−** Listed auth providers are Google, Apple, Firebase and email; others need custom work

<sub>no GPU · Docker · Needs Database, Redis (optional, for shared cache) · [Repo](https://github.com/serverpod/serverpod) · [📖 Docs ↗](https://docs.serverpod.dev) · [🌐 Site ↗](https://serverpod.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverpod/)</sub>

<a name="fusio"></a>
### #&#8288;22 [fusio](https://github.com/apioo/fusio) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Oct 2026</sub>

**PHP API gateway and management platform with developer portal and MCP support.**

Fusio is a self-hosted PHP backend that exposes databases and custom actions (PHP, JavaScript or Python workers) as REST APIs. It adds a developer portal, generated client SDKs, subscription billing and usage analytics. Version 7.0 added an AI agent that generates worker actions via Ollama, ChatGPT or Gemini, and MCP support for exposing APIs as agent tools.

- **+** Runs on MySQL, PostgreSQL or SQLite; Docker image and manual PHP install both documented
- **+** Actions written in PHP, or as worker code in JavaScript or Python
- **+** Includes developer portal, monetization plans, quotas and usage analytics
- **+** Official SDKs for C#, Go, Java, JavaScript, PHP and Python
- **−** Production use needs an Nginx/Apache setup; the built-in PHP server is dev only
- **−** SDK generation, marketplace and monitoring rely on separate external services needing credentials
- **−** README gives no RAM or hardware requirements
- **−** AI action generation needs an external or self-run LLM provider

<sub>no GPU · Needs MySQL, PostgreSQL or SQLite, Nginx or Apache (production), Ollama, OpenAI or Gemini (optional, AI agent) · Models: Ollama, ChatGPT, Gemini · port 8080 · [Repo](https://github.com/apioo/fusio) · [▶️ Demo ↗](https://demo.fusio-project.org) · [📖 Docs ↗](https://docs.fusio-project.org/) · [🌐 Site ↗](https://www.fusio-project.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fusio/)</sub>

<a name="butterbase"></a>
### #&#8288;23 [butterbase](https://github.com/butterbase-ai/butterbase) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

**Backend-as-a-service with per-app Postgres, functions, RAG and an MCP server.**

Butterbase is a backend-as-a-service that gives each app its own Postgres database with row-level security and auto-generated REST. It adds auth, S3/R2 file storage, Deno serverless functions, realtime, a KV store, an AI gateway, RAG and graph-spec agents, all exposed as MCP tools at /mcp. The runtime data plane is self-hostable through Docker Compose; the managed cloud adds billing, multi-region orchestration and upstream AI router adapters.

- **+** Real Postgres per app with RLS, migrations and auto-generated REST, no proprietary datastore
- **+** Every capability is exposed as MCP tools over HTTP at /mcp or stdio via npx @butterbase/mcp
- **+** Apache-2.0 data plane with no feature-gated community edition, per the README
- **+** Includes functions, realtime, KV, RAG, Durable Objects and agents in one stack
- **−** Self-host AI gateway has no upstream router adapters; you must implement RouterAdapter yourself
- **−** Multi-region orchestration, billing and dashboards are private to the managed offering
- **−** `butterbase clone` for templates requires an account at butterbase.ai
- **−** Setup needs submodules, manual migrations and a dev-user seed; README calls the OSS distribution young

<sub>no GPU · Compose · Needs Docker, Node 22+, PostgreSQL, Redis, S3/R2 (LocalStack locally), Deno, Cloudflare Workers (build-runner, dispatch-worker) · port 4000 · [Repo](https://github.com/butterbase-ai/butterbase) · [🌐 Site ↗](https://butterbase.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/butterbase/)</sub>

<a name="matecloud"></a>
### #&#8288;24 [matecloud](https://github.com/mateaix/matecloud) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: weak (27) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

**Java DDD microservice scaffold on Spring Boot 4 with Spring AI and MCP tools.**

MateCloud is a Spring Boot 4, Spring Cloud and Dubbo 3 microservice scaffold. It has gateway, auth, system and notice services and a Vue 3 admin UI. It ships 27 Starters (persistence, cache, MQ, tenancy, security, AI) and runs as a monolith or as microservices. The AI starter wraps Spring AI 2.0.1 with @Tool discovery, and mate-cli can expose those tools as an MCP server.

- **+** Switches between monolith (mate-monolith) and microservice deployment from one codebase
- **+** 27 Starters cover locking, rate limiting, multi-tenancy, sharding, Seata and audit logging
- **+** mate-cli generates DDD four-layer modules and code, and runs an MCP server for agents
- **+** Flyway migrations create the schema and seed an admin account on first start
- **−** Heavy stack: MySQL, Redis, RabbitMQ, Nacos and MinIO needed for the full setup
- **−** README and linked docs are in Chinese
- **−** Open edition has only four core services; other capabilities are Starters you wire in
- **−** AI features are an add-on starter, not a standalone chat or agent app

<sub>no GPU · Docker + Compose · Needs JDK 21, Maven 3.9, Docker Compose, MySQL, Redis, RabbitMQ, Nacos, MinIO, Node.js 20 · Models: Anthropic, OpenAI, DeepSeek, Ollama, Zhipu (compatible endpoint) · port 9010 · [Repo](https://github.com/mateaix/matecloud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/matecloud/)</sub>

<a name="steedos-platform"></a>
### #&#8288;25 [steedos-platform](https://github.com/steedos/steedos-platform) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (10) · Freshness: active (93) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · AGPL-3.0 · Oct 2026</sub>

**Metadata-driven low-code platform that generates enterprise apps, APIs and UI from YAML.**

Steedos Platform is a Salesforce-style metadata-driven enterprise app platform in TypeScript. Objects, pages and flows are defined in YAML (*.object.yml, *.page.yml), and the runtime exposes GraphQL and REST APIs and renders a React and Tailwind UI. The README says development is moving to the ObjectStack stack (ObjectQL, ObjectOS, Object UI), while v2.x remains supported.

- **+** Auto-generated GraphQL and REST APIs for every object defined in metadata
- **+** Field-level RBAC and workflow automation built into the runtime
- **+** Same metadata deploys to MongoDB, PostgreSQL or JSON files
- **+** Quick start via a Docker image or npx create-steedos-app scaffold
- **−** Active development is shifting to ObjectStack; this repo is in transition
- **−** README license badge says MIT, but detected license is AGPL-3.0
- **−** Text-to-app AI features are described but no models or providers are named
- **−** No RAM, GPU or sizing requirements documented

<sub>Docker + Compose · Needs MongoDB, PostgreSQL · port 5100 · [Repo](https://github.com/steedos/steedos-platform) · [📖 Docs ↗](https://docs.steedos.com/) · [🌐 Site ↗](https://objectstack.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/steedos-platform/)</sub>

<a name="classic-jazz"></a>
### #&#8288;26 [classic-jazz](https://github.com/garden-co/classic-jazz) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (30) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Oct 2026</sub>

**Local-first synced database with auth and permissions, now legacy.**

Classic Jazz is the first-generation Jazz database. It syncs data, files and LLM streams across frontend, containers, serverless functions and Jazz Cloud, exposed as reactive local JSON-like state. It includes auth, orgs, permissions, edit history, encryption and offline support. The README recommends Jazz v2 for new projects, so this repo is the legacy line.

- **+** Auth, orgs, permissions, edit history and encryption built into the data layer
- **+** Offline support and multiplayer sync with reactive local state
- **+** Self-host or use hosted Jazz Cloud
- **+** MIT licensed, TypeScript codebase
- **−** README recommends Jazz v2 for new projects; this is the legacy version
- **−** README gives no install steps, ports or hardware requirements
- **−** Self-hosting setup and Jazz Cloud pricing are not described in the README
- **−** Requires adopting Jazz's own data model rather than SQL

<sub>no GPU · [Repo](https://github.com/garden-co/classic-jazz) · [📖 Docs ↗](https://classic.jazz.tools/docs) · [🌐 Site ↗](https://classic.jazz.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/classic-jazz/)</sub>

<a name="1backend"></a>
### #&#8288;27 [1backend](https://github.com/1backend/1backend) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: niche (27) · Freshness: recent (67) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · May 2026</sub>

**Microservices platform with auth, routing and registry, plus an LLM runtime.**

1Backend is a Go server that acts as proxy and runtime for microservices and microfrontends. Services register their own accounts and instance URLs, then become reachable under their slug on port 11337. It also provides user accounts, email, an ORM that works without a database, and multitenancy, and can run LLMs in containers.

- **+** Language-agnostic HTTP API for service registration, with Go SDK and examples
- **+** Routes microfrontends by domain, with automatic SSL in edge proxy mode
- **+** Multitenant: several apps or sites on one install
- **+** Ships an oo CLI for login, environments and route management
- **−** AGPL-3.0 license constrains closed-source network use
- **−** Version 0.9.2, pre-1.0; last release 2025-10-12
- **−** Desktop version discontinued; CLI install requires Go
- **−** README gives no RAM, GPU or supported LLM format details

<sub>Compose · Needs Docker · port 11337 · [Repo](https://github.com/1backend/1backend) · [📖 Docs ↗](https://1backend.com/docs/category/running-the-server) · [🌐 Site ↗](https://1backend.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/1backend/)</sub>

<a name="go-backend-clean-architecture"></a>
### #&#8288;28 [go-backend-clean-architecture](https://github.com/amitshekhariitbhu/go-backend-clean-architecture) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: popular (52) · Freshness: slowing (37) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Feb 2026</sub>

**Go REST API template with Gin, MongoDB and JWT auth in layers.**

A Go backend template organized into router, controller, usecase, repository and domain layers. It ships signup, login, refresh-token, profile and task endpoints on Gin, with MongoDB storage, JWT access and refresh tokens, bcrypt hashing and Viper .env configuration. Unit tests use Testify with Mockery-generated mocks. It has no AI features.

- **+** Clear layer separation behind interfaces, so usecases and repositories are mockable in tests
- **+** JWT middleware with access and refresh token flow already implemented
- **+** Runs with go run or docker-compose; API served on port 8080
- **+** Postman API docs and curl examples for every endpoint
- **−** Only MongoDB is supported; other databases need a rewritten repository layer
- **−** Small example domain: users and tasks only, no billing or roles
- **−** Test coverage is thin; README lists more test cases as a TODO
- **−** No tagged releases

<sub>no GPU · Docker + Compose · Needs MongoDB, Go, Docker (optional) · port 8080 · [Repo](https://github.com/amitshekhariitbhu/go-backend-clean-architecture) · [📖 Docs ↗](https://documenter.getpostman.com/view/391588/2s8Z75S9xy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-backend-clean-architecture/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
