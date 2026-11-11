# 🗄️ Backends, databases and hosting reviews · Best of Vibe Coding

Open-source backends you ship apps on (auth, database, storage, APIs) and self-hosted platforms that deploy them from Git or Docker. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-databases-and-hosting).

<sub>🌐 Also on the web: [Backends, databases and hosting on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="bun"></a>
### 🥇 [bun](https://github.com/oven-sh/bun) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 97k · custom license · Nov 2026</sub>

**JavaScript and TypeScript runtime with bundler, test runner and package manager.**

Bun ships as a single `bun` executable that runs JS and TS (including JSX) on JavaScriptCore, as a drop-in Node.js replacement. The same binary provides a Node-compatible package manager, a bundler, a test runner and a single-file executable compiler. It also has built-in APIs for an HTTP server, WebSockets, SQLite, PostgreSQL, Redis and S3.

- **+** One executable covers runtime, package manager, bundler and test runner
- **+** Runs TypeScript and JSX directly without a separate build step
- **+** Built-in clients for SQLite, PostgreSQL, Redis and S3 and a WebSocket-capable HTTP server
- **+** Canary build published on every commit to main; `bun upgrade` self-updates
- **−** Node.js compatibility is a goal, so some Node APIs or native modules may differ
- **−** x64 builds can fail with illegal instruction errors on CPUs lacking required features
- **−** Linux kernel 5.6+ strongly recommended; minimum is 5.1
- **−** Not a backend service: it is a runtime, so auth and storage are up to you

<sub>no GPU · [Repo](https://github.com/oven-sh/bun) · [📖 Docs ↗](https://bun.com/docs) · [🌐 Site ↗](https://bun.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bun/)</sub>

<a name="strapi"></a>
### 🥈 [strapi](https://github.com/strapi/strapi) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 73k · custom license · Nov 2026</sub>

**Headless CMS that generates REST and GraphQL APIs from content models.**

Strapi is a self-hosted headless CMS written in TypeScript. You define content types in a visual builder, and it generates REST and GraphQL APIs plus an admin UI for editors. It includes roles and permissions, a media library, i18n, draft and publish, and a plugin system, and stores data in SQLite, PostgreSQL, MySQL or MariaDB.

- **+** Auto-generated REST and GraphQL endpoints for every content type
- **+** Built-in roles and permissions, media library, i18n, and draft and publish
- **+** Supports SQLite, PostgreSQL, MySQL and MariaDB
- **+** Hosted live demo and a Next.js LaunchPad template to start from
- **−** No official Docker images; the README points to a community dockerize tool
- **−** License is not auto-detected (NOASSERTION); check the LICENSE file before commercial use
- **−** AI features are described as Strapi AI, with details only on the vendor site
- **−** Managed hosting is pushed through Strapi Cloud, a separate paid product

<sub>no GPU · Compose · Needs Node.js, SQLite, PostgreSQL, MySQL or MariaDB · [Repo](https://github.com/strapi/strapi) · [▶️ Demo ↗](https://strapi.io/demo) · [📖 Docs ↗](https://docs.strapi.io) · [🌐 Site ↗](https://strapi.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/strapi/)</sub>

<a name="traefik"></a>
### 🥉 [traefik](https://github.com/traefik/traefik) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · MIT · Nov 2026</sub>

**HTTP reverse proxy and load balancer that auto-discovers routes from orchestrators.**

Traefik is a reverse proxy and load balancer written in Go. It watches providers such as Docker, Swarm, Kubernetes, ECS, Consul, etcd or a file, and generates routes without restarts. It handles Let's Encrypt certificates, WebSocket, HTTP/2 and gRPC, and ships a web dashboard. It is not an AI project, so it fits this list only as infrastructure for hosting apps.

- **+** Updates routes live from Docker, Kubernetes, ECS or file providers, no restarts
- **+** Built-in Let's Encrypt HTTPS, including wildcard certificates
- **+** Single Go binary plus official Docker image
- **+** Exports metrics to Prometheus, Datadog, StatsD and InfluxDB 2.x
- **−** Not AI-specific; no model, agent or LLM features
- **−** Major version upgrades have breaking changes, so the v2-to-v3 migration guide applies
- **−** Web UI is described as simple; the README shows only a dashboard
- **−** Commercial support is through Traefik.io; community support is a forum

<sub>no GPU · Docker · Needs Docker, Kubernetes, Let's Encrypt · port 8080 · [Repo](https://github.com/traefik/traefik) · [📖 Docs ↗](https://doc.traefik.io/traefik/) · [🌐 Site ↗](https://traefik.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/traefik/)</sub>

<a name="appwrite"></a>
### #&#8288;4 [appwrite](https://github.com/appwrite/appwrite) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · BSD-3-Clause · Nov 2026</sub>

**Backend with auth, databases, storage, functions and an MCP server for agents.**

Appwrite is a backend platform that bundles Auth, Databases, Storage, Functions, Sites, Messaging, Realtime and a Firewall behind REST, GraphQL and WebSocket APIs. It has client and server SDKs for 16 platforms and a hosted MCP server so coding agents can operate on a live project. It runs as a managed cloud or is self-hosted through a Docker-based installer.

- **+** Covers auth, databases, storage, functions, messaging and realtime in one backend
- **+** SDKs for Web, Flutter, Apple, Android, Node.js, Python, Go, Rust and more
- **+** Exposes REST, GraphQL and WebSocket APIs
- **+** Hosted MCP server uses OAuth, so no API keys are needed on Cloud
- **−** Self-hosting needs Docker and mounts the Docker socket for the installer
- **−** Hosted MCP is for Cloud; self-hosted instances need a separate local MCP server
- **−** Hybrid monolith with queue, workers and cache means several services to operate

<sub>no GPU · Docker + Compose · Needs Docker · port 80 · [Repo](https://github.com/appwrite/appwrite) · [▶️ Demo ↗](https://cloud.appwrite.io) · [📖 Docs ↗](https://appwrite.io/docs) · [🌐 Site ↗](https://appwrite.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/appwrite/)</sub>

<a name="medusa"></a>
### #&#8288;5 [medusa](https://github.com/medusajs/medusa) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · custom license · Nov 2026</sub>

**Node.js commerce platform with modular products, carts, orders and payments.**

Medusa is a TypeScript commerce framework providing Store and Admin APIs, an admin dashboard and commerce modules for products, carts, orders, pricing and payments. It is used to build DTC or B2B stores, marketplaces and PoS systems. Provider modules cover Stripe, S3, SendGrid, Redis and several auth methods. It is not an AI project; the AI link is only that it is a base to build on.

- **+** Commerce modules (product, cart, order, pricing, payment) are published separately on npm
- **+** Ships Store and Admin API routes plus an admin dashboard in one monorepo
- **+** Provider modules for Stripe, S3, SendGrid, Redis and OIDC, GitHub and Google auth
- **+** Core is MIT licensed; scaffolds with one npx create-medusa-app command
- **−** RBAC Enterprise Edition materials require a commercial agreement with MedusaJS, Inc.
- **−** Needs Node.js v22.22.0 or later and a running PostgreSQL database
- **−** No built-in AI features described in the README
- **−** Open-core licensing; detected license is reported as NOASSERTION

<sub>no GPU · Needs Node.js 22.22.0+, PostgreSQL · [Repo](https://github.com/medusajs/medusa) · [📖 Docs ↗](https://docs.medusajs.com) · [🌐 Site ↗](https://www.medusajs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/medusa/)</sub>

<a name="tidb"></a>
### #&#8288;6 [tidb](https://github.com/pingcap/tidb) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · Apache-2.0 · Nov 2026</sub>

**Distributed MySQL-compatible SQL database with row and columnar storage.**

TiDB is a distributed SQL database written in Go that speaks the MySQL 8.0 protocol and runs ACID transactions across nodes using two-phase commit and Raft replication. It separates compute from storage, with TiKV for rows and TiFlash for columns, so one cluster handles transactional and analytical queries. It deploys locally, on Kubernetes via TiDB Operator, or as the managed TiDB Cloud.

- **+** MySQL 8.0 compatible, so existing drivers, ORMs and tools work with few changes
- **+** Raft replication with automated failover and configurable geographic replica placement
- **+** HTAP: TiKV row store plus TiFlash columnar replica in the same cluster
- **+** Compute and storage scale independently without downtime
- **−** Full cluster has several components (TiDB, TiKV, PD, TiFlash), heavier than a single-node database
- **−** Not a full MySQL drop-in; the README points to a separate compatibility page
- **−** Vector search is linked only via TiDB Cloud docs, so self-hosted support is unclear
- **−** General database infrastructure, not an AI app starter

<sub>no GPU · Docker · Needs TiKV, PD, TiFlash (optional) · [Repo](https://github.com/pingcap/tidb) · [▶️ Demo ↗](https://play.tidbcloud.com/?utm_source=github&utm_medium=tidb_readme) · [📖 Docs ↗](https://docs.pingcap.com/tidb/stable?utm_source=github&utm_medium=tidb) · [🌐 Site ↗](https://www.pingcap.com/?utm_source=github&utm_medium=tidb) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tidb/)</sub>

<a name="compose"></a>
### #&#8288;7 [compose](https://github.com/docker/compose) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · Apache-2.0 · Nov 2026</sub>

**CLI plugin that runs multi-container apps from a compose.yaml file.**

Docker Compose is a Go-based Docker CLI plugin that reads a compose.yaml, following the Compose specification, and starts the defined services with `docker compose up`. It is not AI-specific; it is the general tool many self-hosted AI projects use to run their stacks. It ships bundled with Docker Desktop on Windows and macOS, and as release binaries for Linux.

- **+** One command, `docker compose up`, builds and starts all services in a file
- **+** Implements the open Compose specification, so files are portable between tools
- **+** Included in Docker Desktop; Linux install is a single binary in cli-plugins
- **+** Written in Go, with CI, Codecov and OpenSSF Scorecard badges in the README
- **−** Not an AI project; no model, GPU or LLM features described in the README
- **−** Requires a Docker engine to run containers
- **−** Some Compose features are unavailable to Docker Swarm users, per the README
- **−** README gives little detail beyond install and a short example; features are in external docs

<sub>no GPU · Docker · Needs Docker Engine or Docker Desktop · [Repo](https://github.com/docker/compose) · [📖 Docs ↗](https://compose-spec.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/compose/)</sub>

<a name="nacos"></a>
### #&#8288;8 [nacos](https://github.com/alibaba/nacos) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Nov 2026</sub>

**Service discovery, health checking and dynamic config server for microservices.**

Nacos is a Java server that lets services register and discover each other over DNS or HTTP, with health checks, and pushes configuration changes to running applications without redeploys. It also offers weighted DNS routing and a web console for service metadata, config and metrics. Integrations cover Dubbo, gRPC, Spring Cloud and Kubernetes services. It is not an AI project, so it fits this list only loosely.

- **+** Covers service registry, health checks and dynamic config in one server
- **+** Documented integrations for Dubbo, Spring Cloud and Kubernetes
- **+** Standalone mode starts with a single startup script from the release zip
- **+** Web console in Chinese and English, plus Russian in the new UI
- **−** Not an AI or LLM project; fit with this list is marginal
- **−** README gives no Docker or compose instructions
- **−** Enterprise support is tied to Alibaba Cloud MSE

<sub>no GPU · [Repo](https://github.com/alibaba/nacos) · [📖 Docs ↗](https://nacos.io/docs/latest/overview/) · [🌐 Site ↗](https://nacos.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nacos/)</sub>

<a name="dragonfly"></a>
### #&#8288;9 [dragonfly](https://github.com/dragonflydb/dragonfly) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · custom license · Nov 2026</sub>

**Multi-threaded in-memory data store compatible with Redis and Memcached APIs.**

Dragonfly is an in-memory data store written in C++ that speaks the Redis and Memcached protocols, so existing clients work without code changes. It uses a shared-nothing, multi-threaded design with VLL-based transactions and a Dash-derived hashtable, plus fork-less snapshotting. About 185 Redis commands (roughly the Redis 5.0 API) and 13 Memcached commands are implemented.

- **+** Scales across CPU cores; README reports 3.8M QPS on c6gn.16xlarge versus a single Redis process
- **+** Fork-less snapshotting; README shows no visible memory growth during bgsave
- **+** Works with Redis clients; optional Memcached API via --memcached_port
- **+** HTTP console and Prometheus metrics served on the main port (6379)
- **−** Command coverage is about 185 commands, roughly the Redis 5.0 API
- **−** Key expiry capped at 2^28-1 seconds; expiration behavior differs from Redis in places
- **−** HTTP console is on by default; disable it if the port is exposed
- **−** Benchmarks are vendor-run on AWS; README gives no independent results

<sub>no GPU · port 6379 · [Repo](https://github.com/dragonflydb/dragonfly) · [📖 Docs ↗](https://dragonflydb.io/docs) · [🌐 Site ↗](https://www.dragonflydb.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dragonfly/)</sub>

<a name="kestra"></a>
### #&#8288;10 [kestra](https://github.com/kestra-io/kestra) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · Apache-2.0 · Nov 2026</sub>

**Event-driven workflow orchestrator with YAML flows, a UI editor and AI tasks.**

Kestra is a Java workflow orchestrator where flows are declared in YAML and edited through a code editor, a no-code editor or an AI Copilot, all kept in sync. It runs scheduled and event-triggered flows using hundreds of plugins (databases, cloud, message buses, scripts in Python, Node.js, R, Go, Shell). Version 2.0 adds AI agent and RAG task types, an MCP server exposing flows as tools, and gRPC worker communication.

- **+** Flows are plain YAML with Git sync, Terraform provider and API, so logic stays in code
- **+** Hundreds of plugins plus scripts in any language, run via Docker, Kubernetes or cloud VM task runners
- **+** Workers connect to the control plane over gRPC, so they can sit in another region or restricted network
- **+** Built-in MCP server and AI agent/RAG tasks call OpenAI, Anthropic, Gemini, Bedrock and Ollama
- **−** RBAC, Policies, Cases, Promote and external log store are Enterprise Edition only
- **−** 2.0 has breaking changes, e.g. ForEach and ForEachItem replaced by Loop, and the image suffix renamed
- **−** Quick start mounts the Docker socket and runs as root
- **−** Slim image fetches plugins from Maven Central at first use, so needs outbound access

<sub>no GPU · Docker + Compose · Needs Docker, PostgreSQL (production deployments, per cloud templates), Maven Central (slim image plugin auto-install) · Models: OpenAI, Anthropic, Google Gemini, Amazon Bedrock, Ollama · port 8080 · [Repo](https://github.com/kestra-io/kestra) · [📖 Docs ↗](https://kestra.io/docs) · [🌐 Site ↗](https://kestra.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kestra/)</sub>

<a name="nest"></a>
### #&#8288;11 [nest](https://github.com/nestjs/nest) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 77k · MIT · Nov 2026</sub>

**TypeScript framework for structured Node.js backends with dependency injection.**

Nest is a TypeScript backend framework for Node.js that provides modules, dependency injection, and fixed places for validation, authentication and error handling. It runs on Express, Fastify or node:http, and ships first-party packages for databases, queues, GraphQL, WebSockets, microservices, OpenAPI, AI and MCP servers. It is a framework to build on rather than a starter template, and an app can be a single file.

- **+** Runs on Express, Fastify or node:http; migration guides for Express and Fastify
- **+** First-party packages for TypeORM, Drizzle, Mongoose, Sequelize, BullMQ, GraphQL and OpenAPI
- **+** Scales from a single-file app to modular code with dependency injection
- **+** Docs published as markdown with llms.txt; new projects include AGENTS.md
- **−** Decorator and module conventions add a learning curve over plain Express
- **−** Framework only: no UI, hosting or bundled database; you assemble the packages
- **−** Newer packages such as @nestjs/ai and @nestjs/workflows have little track record
- **−** Observability product (NestJS Observe) is hosted, free only up to 300,000 events a month

<sub>no GPU · Needs Node.js · port 3000 · [Repo](https://github.com/nestjs/nest) · [📖 Docs ↗](https://docs.nestjs.com) · [🌐 Site ↗](https://nestjs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nest/)</sub>

<a name="turborepo"></a>
### #&#8288;12 [turborepo](https://github.com/vercel/turborepo) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

**Rust build system and task runner for JavaScript and TypeScript monorepos.**

Turborepo is a build system distributed as the `turbo` npm package and implemented in Rust. The README describes it as a build system for coding agents and defers all usage details to turborepo.dev. It is general build tooling rather than an AI app starter, so it fits this list only loosely.

- **+** MIT licensed and maintained by Vercel, with a release on 2026-10-20
- **+** Distributed as the `turbo` npm package
- **+** Implemented in Rust
- **+** Docs, showcase and community channels linked from the README
- **−** README has no usage, configuration or feature details; content is on the website
- **−** Not an AI app or starter, so a loose match for this list
- **−** README does not explain how it works with coding agents

<sub>no GPU · [Repo](https://github.com/vercel/turborepo) · [🌐 Site ↗](https://turborepo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/turborepo/)</sub>

<a name="better-auth"></a>
### #&#8288;13 [better-auth](https://github.com/better-auth/better-auth) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

**Framework-agnostic authentication and authorization library for TypeScript with plugins.**

Better Auth is a TypeScript authentication and authorization library that works across frameworks. It ships core auth features and a plugin system for additions such as 2FA and multi-tenant support. It is a library you add to an existing app, not a hosted service.

- **+** Framework-agnostic TypeScript library, not tied to one web stack
- **+** Plugin system for 2FA, multi-tenant and other advanced features
- **+** MIT licensed, with a release published on the latest commit date
- **+** Self-hosted in your own app, no third-party auth service required
- **−** README lists no supported frameworks, databases or auth providers
- **−** Library only: no standalone auth server or admin UI described
- **−** README has no install steps, code examples or docs link
- **−** TypeScript only, so non-JS backends cannot use it directly

<sub>no GPU · Compose · Compose runs MongoDB, Redis, PostgreSQL, MySQL · [Repo](https://github.com/better-auth/better-auth) · [🌐 Site ↗](https://better-auth.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/better-auth/)</sub>

<a name="nocobase"></a>
### #&#8288;14 [nocobase](https://github.com/nocobase/nocobase) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Nov 2026</sub>

**No-code platform for building business systems, with a CLI for coding agents.**

NocoBase is a plugin-based platform for building business applications through a WYSIWYG interface, with data models, permissions, workflows and audit logs built in. It also ships a CLI (`nb`) and skills so coding agents such as Claude Code, Codex and Cursor can create data models, pages and workflows. It includes AI employees with role-based permissions, and exposes MCP and HTTP APIs for external agents.

- **+** Data stays in standard relational databases, separate from the UI
- **+** Permissions, workflows and audit logs are built-in modules, not generated code
- **+** Agents and people edit the same data models, pages and workflows
- **+** Microkernel design: features are added as official or custom plugins
- **−** License is reported as NOASSERTION; terms need checking before commercial use
- **−** README gives no RAM, database or port requirements
- **−** Extending beyond the no-code UI requires learning its plugin architecture

<sub>[Repo](https://github.com/nocobase/nocobase) · [▶️ Demo ↗](https://demo.nocobase.com/new) · [📖 Docs ↗](https://docs.nocobase.com/) · [🌐 Site ↗](https://www.nocobase.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nocobase/)</sub>

<a name="rxdb"></a>
### #&#8288;15 [rxdb](https://github.com/pubkey/rxdb) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · Apache-2.0 · Nov 2026</sub>

**Local-first reactive NoSQL database for JavaScript apps with sync.**

RxDB is a NoSQL database that runs inside JavaScript clients: browsers, Node.js, React Native, Electron, Capacitor and Flutter. Queries and single fields are observable through RxJS, so UIs update when data changes. It replicates over a sync protocol of three HTTP endpoints, with plugins for GraphQL, CouchDB, WebSocket, WebRTC, Supabase, Firestore and NATS. It has no AI features and fits this list only as a data layer.

- **+** Swappable storage: LocalStorage, IndexedDB, OPFS, SQLite, memory, FoundationDB, DenoKV
- **+** Replication plugins for GraphQL, CouchDB, WebSocket, WebRTC, Supabase, Firestore and NATS
- **+** Observable queries and fields drive realtime UI updates without manual refetching
- **+** Schema validation, encryption, migration, CRDT and attachments available as plugins
- **−** Some plugins are sold separately as a premium tier
- **−** No AI, vector search or LLM features in the README
- **−** Requires rxjs alongside rxdb as an install dependency
- **−** Sync needs your own backend implementing the HTTP endpoints or a supported service

<sub>no GPU · Needs rxjs · [Repo](https://github.com/pubkey/rxdb) · [📖 Docs ↗](https://rxdb.info/quickstart.html) · [🌐 Site ↗](https://rxdb.info/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rxdb/)</sub>

<a name="scalar"></a>
### #&#8288;16 [scalar](https://github.com/scalar/scalar) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

**OpenAPI API reference renderer and offline-first API client.**

Scalar renders OpenAPI/Swagger documents as an interactive API reference with a built-in request tester and generated code examples. It also ships a desktop and browser API client for Windows, macOS and Linux, plus OpenAPI tooling such as a parser, upgrader, mock server and CLI. Integrations cover about 30 frameworks including FastAPI, Hono, Express, NestJS, Next.js, Laravel and ASP.NET Core.

- **+** Drop-in HTML/ESM setup from a CDN, no build step required
- **+** Dedicated integrations for about 30 frameworks across JS, Python, Java, Go, Rust, PHP and .NET
- **+** Default OpenAPI docs UI in Elysia, Nitro, Litestar, oRPC and others
- **+** Same repo includes API client, parser, mock server and OpenAPI upgrader
- **−** Not an AI project; fits the list's categories only loosely
- **−** Managed hosting, GitHub Sync and custom domains are in the hosted product, not this repo
- **−** Needs an existing OpenAPI document or a generator for your framework
- **−** Browser use may need a CORS proxy such as proxy.scalar.com

<sub>no GPU · [Repo](https://github.com/scalar/scalar) · [▶️ Demo ↗](https://docs.scalar.com/swagger-editor) · [📖 Docs ↗](https://scalar.com/products/api-references/getting-started) · [🌐 Site ↗](https://scalar.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scalar/)</sub>

<a name="rails"></a>
### #&#8288;17 [rails](https://github.com/rails/rails) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Nov 2026</sub>

**Ruby MVC web framework with ORM, mailers, jobs, WebSockets and file storage.**

Rails is a Ruby web framework for database-backed applications built on the Model-View-Controller pattern. It bundles Active Record (ORM), Action Pack (routing and controllers), Action View (ERB templates), plus Action Mailer, Action Mailbox, Active Job, Action Cable, Active Storage and Action Text. It has no AI-specific features; it is a general application framework.

- **+** Single framework covers ORM, routing, views, email, background jobs, WebSockets and file uploads
- **+** Active Record, Active Model, Action Pack, Action View and Active Support usable standalone
- **+** `rails new myapp` and `bin/rails server` give a running app on port 3000
- **+** MIT license, with active commits and recent releases
- **−** No built-in AI, LLM or agent features; you add those through gems
- **−** Ruby only, so teams on other languages cannot reuse it directly
- **−** Not a hosted backend: you run and deploy the app yourself
- **−** Opinionated MVC structure; API-only or non-MVC designs fit less naturally

<sub>no GPU · Needs Ruby · port 3000 · [Repo](https://github.com/rails/rails) · [📖 Docs ↗](https://guides.rubyonrails.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rails/)</sub>

<a name="directus"></a>
### #&#8288;18 [directus](https://github.com/directus/directus) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · custom license · Nov 2026</sub>

**Wraps any SQL database with REST and GraphQL APIs, an admin Studio and MCP.**

Directus connects to an existing SQL database (Postgres, MySQL, MariaDB, MS SQL, SQLite, OracleDB, CockroachDB) and generates REST and GraphQL APIs from the schema. It adds a visual Studio for non-technical users, field-level policy-based access control, and a native MCP server so AI agents work on live data under the same permissions. It is source-available under MSCL 1.0, not an OSI open-source license.

- **+** Generates REST and GraphQL APIs from an existing schema with no configuration
- **+** Supports Postgres, MySQL, MariaDB, MS SQL, SQLite, OracleDB and CockroachDB
- **+** Field-level permissions apply equally to human users and MCP-connected agents
- **+** Extensible with custom endpoints, hooks, interfaces and modules
- **−** MSCL 1.0 is source-available, not OSI open source
- **−** Free use limited to under $5M revenue and 50 employees
- **−** Advanced or enterprise features need a commercial license above those limits
- **−** Embedded AI Assistant details and model support are only linked, not described

<sub>no GPU · Docker + Compose · Needs SQL database, Redis (optional, in Railway template), S3-compatible storage (optional, in Railway template) · [Repo](https://github.com/directus/directus) · [📖 Docs ↗](https://directus.com/docs) · [🌐 Site ↗](https://directus.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/directus/)</sub>

<a name="dokploy"></a>
### #&#8288;19 [dokploy](https://github.com/dokploy/dokploy) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · custom license · Nov 2026</sub>

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
### #&#8288;20 [spacetimedb](https://github.com/clockworklabs/spacetimedb) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · custom license · Nov 2026</sub>

**Relational database that runs your server logic as modules and syncs clients live.**

SpacetimeDB is a relational database that hosts application logic written as modules in Rust, C#, TypeScript or C++. Clients connect directly, call reducers as ACID transactions, and subscribe to tables to receive committed changes without polling or a separate API server. It runs the BitCraft Online backend, and the quick start publishes a chat-react-ts template to Maincloud.

- **+** Modules in Rust, C#, TypeScript or C++ replace a separate web or game server
- **+** Table subscriptions push committed changes to clients; no polling or pub/sub layer
- **+** Commit log with group fsync; confirmed reads on by default since 2.0
- **+** Client SDKs for TypeScript, Rust, C# (Unity) and C++ (Unreal)
- **−** BSL 1.1 license; converts to AGPL v3.0 with linking exception only after years
- **−** Aimed at low-latency transactional work, not batch or analytical queries
- **−** Application logic lives inside the database, tying the app to its module model
- **−** Quick start publishes to Maincloud, which has pricing

<sub>no GPU · Docker + Compose · port 3000 · [Repo](https://github.com/clockworklabs/spacetimedb) · [📖 Docs ↗](https://spacetimedb.com/docs) · [🌐 Site ↗](https://spacetimedb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spacetimedb/)</sub>

<a name="novu"></a>
### #&#8288;21 [novu](https://github.com/novuhq/novu) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · custom license · Nov 2026</sub>

**Notification API and agent messaging layer for Inbox, email, SMS, push and chat.**

Novu exposes one API for sending notifications through Inbox, email, SMS, push and chat providers, with a workflow engine, digests and an embeddable React Inbox component. It also offers Agent Communication Infrastructure, which normalizes messages between Slack, Teams, Telegram, WhatsApp or email and an existing agent. The core is MIT; the enterprise folder is under a commercial license.

- **+** Wide provider coverage: 20 email, 37 SMS, 8 push and 13 chat providers
- **+** Workflow engine with branching, per-channel conditions and digests
- **+** Embeddable real-time Inbox and preferences components for React
- **+** Agent layer works with any agent stack, such as AI SDK or LangGraph
- **−** Open core: the enterprise folder requires a commercial license
- **−** README points to a hosted dashboard; self-hosting is only linked, not described
- **−** Inbox component is React only; React Native, Vue and Angular are marked coming soon
- **−** Agent features route messages only; Novu is not the agent itself

<sub>no GPU · Compose · [Repo](https://github.com/novuhq/novu) · [📖 Docs ↗](https://docs.novu.co) · [🌐 Site ↗](https://novu.co) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/novu/)</sub>

<a name="supabase"></a>
### #&#8288;22 [supabase](https://github.com/supabase/supabase) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 115k · Apache-2.0 · Nov 2026</sub>

**Postgres backend with auth, generated APIs, storage and realtime.**

Supabase is a Postgres-based backend platform that bundles JWT authentication (GoTrue), auto-generated REST (PostgREST) and GraphQL (pg_graphql) APIs, realtime subscriptions over websockets, S3-backed file storage, and database and edge functions. It also ships a vector/embeddings toolkit and a dashboard. It runs as a hosted service, or you can self-host or develop locally.

- **+** Auth, REST, GraphQL, realtime, storage and edge functions on one Postgres database
- **+** Official clients for JavaScript/TypeScript, Flutter, Swift and Python
- **+** Built on existing open-source components such as PostgREST and GoTrue
- **+** Vector/embeddings toolkit for AI features inside Postgres
- **−** Self-hosting means running several services: Postgres, Realtime, PostgREST, GoTrue, Storage, Envoy
- **−** Many client libraries are community-maintained and cover only some features
- **−** Realtime depends on Postgres replication, so it is tied to the database
- **−** Hosted platform is the primary path; the README gives no self-host sizing

<sub>no GPU · Compose · Needs PostgreSQL, S3-compatible storage · [Repo](https://github.com/supabase/supabase) · [📖 Docs ↗](https://supabase.com/docs) · [🌐 Site ↗](https://supabase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase/)</sub>

<a name="payload"></a>
### #&#8288;23 [payload](https://github.com/payloadcms/payload) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

**Next.js-native headless CMS and app framework with a React admin panel.**

Payload installs into an existing Next.js /app folder and provides a TypeScript headless CMS with auth, versions and drafts, localization, and a customizable React admin. Server components can query the database directly without REST or GraphQL. The README lists website and ecommerce templates plus one-click deploys to Vercel (Neon, Vercel Blob) and Cloudflare (Workers, R2, D1).

- **+** Installs inside an existing Next.js /app folder, so frontend and backend share one codebase
- **+** Auth, versions and drafts, localization, and field-level access control are built in
- **+** Generates TypeScript types for your data; hooks exist at document and field level
- **+** One-click deploy to Vercel (Neon, Blob) or Cloudflare (Workers, R2, D1)
- **−** README does not mention built-in AI features; it is a general CMS
- **−** Tied to Next.js and TypeScript for its native setup
- **−** v2 to v3 required a migration guide, so older projects need upgrade work

<sub>no GPU · Needs Next.js, Database (Neon Postgres or Cloudflare D1 in one-click deploys) · [Repo](https://github.com/payloadcms/payload) · [📖 Docs ↗](https://payloadcms.com/docs/getting-started/what-is-payload) · [🌐 Site ↗](https://payloadcms.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/payload/)</sub>

<a name="seaweedfs"></a>
### #&#8288;24 [seaweedfs](https://github.com/seaweedfs/seaweedfs) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Nov 2026</sub>

**Distributed object store and file system with S3 API and Iceberg catalog.**

SeaweedFS is a Go distributed storage system built from master, volume and filer servers. It stores billions of files as blobs in append-only volumes with one disk read per blob, and exposes them through an S3 gateway, FUSE mount, WebDAV, SFTP and HDFS. It also includes an Iceberg REST catalog, S3 Tables, and S3 Vectors backed by a separate vector engine.

- **+** Master is not in the read path; 16-byte in-memory index per blob, one seek per read
- **+** `weed mini` starts S3, filer, WebDAV, Iceberg catalog and Admin UI in one process
- **+** Filer metadata can live in PostgreSQL, MySQL, Redis, Cassandra, TiKV, etcd and others
- **+** Replication, erasure coding, cloud tiering and cross-cluster replication are built in
- **−** Multi-component architecture (master, volume, filer, S3) is more to operate than a single-node store
- **−** Vector search needs a separate Rust weed-vector binary; the default installer omits it
- **−** Rebalancing does not run automatically; it is triggered from weed shell or the maintenance worker
- **−** Storage infrastructure, not an AI app starter; AI relevance is limited to S3 Vectors

<sub>no GPU · Docker + Compose · Needs Optional filer metadata store (PostgreSQL, MySQL, Redis, etc.), weed-vector binary for S3 Vectors · port 8333 · [Repo](https://github.com/seaweedfs/seaweedfs) · [📖 Docs ↗](https://github.com/seaweedfs/seaweedfs/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/seaweedfs/)</sub>

<a name="graphql-engine"></a>
### #&#8288;25 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Nov 2026</sub>

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

<a name="saleor"></a>
### #&#8288;26 [saleor](https://github.com/saleor/saleor) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · BSD-3-Clause · Nov 2026</sub>

**Headless, GraphQL-only commerce backend for composable storefronts.**

Saleor is a Python e-commerce backend that exposes catalog, orders, payments and promotions only through a GraphQL API. It extends through webhooks, apps, metadata and dashboard iframes rather than in-process plugins. The dashboard and Next.js storefront live in separate repositories. It is not an AI project.

- **+** Per-channel control of pricing, currencies and stock for multichannel selling
- **+** Extensions run as separate apps via webhooks, so custom logic stays out of core
- **+** Covers multi-warehouse orders, returns, split payments, vouchers and gift cards
- **+** Single open-source version under BSD-3-Clause, with no feature split stated
- **−** API-only: dashboard and storefront are separate repos you must deploy and wire up
- **−** Service-oriented design is heavier than WordPress or Magento for small shops
- **−** main branch may be unstable; production use needs a tagged 3.x release
- **−** No AI features; it does not fit an AI-starter list on its own

<sub>no GPU · Docker · [Repo](https://github.com/saleor/saleor) · [▶️ Demo ↗](https://storefront.saleor.io/) · [📖 Docs ↗](https://docs.saleor.io/) · [🌐 Site ↗](https://saleor.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/saleor/)</sub>

<a name="coder"></a>
### #&#8288;27 [coder](https://github.com/coder/coder) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · AGPL-3.0 · Nov 2026</sub>

**Self-hosted cloud dev environments defined in Terraform, with AI coding agents.**

Coder provisions cloud development workspaces from Terraform templates (EC2 VMs, Kubernetes Pods, Docker containers), connects them over a WireGuard tunnel, and shuts them down when idle. Coder Agents runs an AI coding agent loop in the control plane, so workspaces hold no LLM API keys. It accepts Anthropic, OpenAI, Google, Bedrock or self-hosted models.

- **+** Workspaces defined in Terraform, so any infrastructure Terraform supports can host them
- **+** Agent loop runs in the control plane; no LLM credentials stored in workspaces
- **+** Idle workspaces shut down automatically to cut compute cost
- **+** Built-in database for evaluation; PostgreSQL 13+ for production
- **−** Premium tier gates features aimed at large teams, plus dedicated support
- **−** AGPL-3.0 license may be a problem for some organizations
- **−** Production use needs PostgreSQL and an external access URL
- **−** Templates require Terraform knowledge to write and maintain

<sub>no GPU · Compose · Needs PostgreSQL 13+ (production), Terraform · Models: Anthropic, OpenAI, Google, Bedrock, self-hosted · port 3000 · [Repo](https://github.com/coder/coder) · [📖 Docs ↗](https://coder.com/docs) · [🌐 Site ↗](https://coder.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coder/)</sub>

<a name="dokku"></a>
### #&#8288;28 [dokku](https://github.com/dokku/dokku) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Nov 2026</sub>

**Self-hosted Heroku-style PaaS that deploys apps with git push.**

Dokku is a small platform-as-a-service written in Go that runs on a single Ubuntu or Debian host and builds and runs apps in Docker containers. You set domains and SSH keys with the dokku CLI, then deploy by pushing to the server. It is a hosting layer, not an AI project, so it fits this list only as a place to run apps.

- **+** Installs with a bootstrap script on Ubuntu 22.04/24.04/26.04 or Debian 11+, amd64 and arm64
- **+** MIT licensed, with a release on 2026-10-30 and recent commits
- **+** Imports an existing SSH keypair automatically for git-based deploys
- **+** Ubuntu and Arch packages, plus documented upgrade and unattended install paths
- **−** README describes one VM; multi-host clustering is not mentioned
- **−** Host OS limited to Ubuntu and Debian
- **−** No AI-specific features; it only hosts apps built elsewhere
- **−** Managed through CLI and SSH; the README mentions no web UI

<sub>no GPU · Docker · Needs Docker, SSH keypair, Ubuntu or Debian VM · [Repo](https://github.com/dokku/dokku) · [📖 Docs ↗](https://dokku.com/docs/getting-started/installation/) · [🌐 Site ↗](https://dokku.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokku/)</sub>

<a name="pulumi"></a>
### #&#8288;29 [pulumi](https://github.com/pulumi/pulumi) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

**Infrastructure as code CLI and engine using general-purpose programming languages.**

Pulumi is a CLI, engine and set of language SDKs that provision cloud resources from programs written in TypeScript, Python, Go, .NET, Java or YAML. `pulumi up` computes a minimal diff against deployed state, and the Automation API lets you embed it in other software. It is not an AI project; the README mentions agents only in its title.

- **+** Seven languages marked Stable: JavaScript, TypeScript, Python, Go, .NET, Java and YAML
- **+** 300+ providers in the registry, including AWS, Azure, Google Cloud and Kubernetes
- **+** Automation API embeds deployments in your own programs
- **+** Loops, functions and package management replace YAML templating; `pulumi up` applies minimal diffs
- **−** Not an AI tool; no model, agent or LLM functionality described in the README
- **−** Needs a language runtime (Node.js, Python, Go, .NET or JDK 11+) per project
- **−** Provider libraries live in separate repos, not in this one
- **−** Secrets management (Pulumi ESC) is a separate product, not covered by this repo

<sub>Needs Cloud provider account (AWS, Azure, GCP, Kubernetes, etc.), Language runtime: Node.js, Python, Go, .NET or JDK 11+ · [Repo](https://github.com/pulumi/pulumi) · [📖 Docs ↗](https://www.pulumi.com/docs/) · [🌐 Site ↗](https://www.pulumi.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pulumi/)</sub>

<a name="redis"></a>
### #&#8288;30 [redis](https://github.com/redis/redis) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 77k · custom license · Nov 2026</sub>

**In-memory data structure server used as cache, database and message broker.**

Redis is a C server that keeps data primarily in memory and exposes strings, hashes, lists, sets, sorted sets, streams, JSON, time series and vector sets over a text-based protocol. It also covers pub/sub, transactions, Lua scripting, and Redis Search for full-text, geospatial and vector queries on hash and JSON documents. Common uses are caching, session storage, queues, and GenAI memory or semantic caching.

- **+** Wide set of native types: streams, JSON, time series, probabilistic structures, vector sets
- **+** Redis Search adds vector, full-text and geospatial queries over hash and JSON documents
- **+** Modules API lets you add new commands; official clients exist for most major languages
- **+** Install paths include Docker, Snap, Homebrew, RPM and Debian packages
- **−** Building all bundled modules needs LLVM 21, Rust 1.94 and CMake 3.25 to 3.31.6
- **−** CMake 4.x is unsupported and fails the build; bootstrap will not downgrade it
- **−** Vector set type is marked beta
- **−** Extra compliance and resiliency features are in paid Redis Software and Redis Cloud

<sub>no GPU · Docker · Needs LLVM 21 (module build), CMake 3.25-3.31.6 (module build), Rust 1.94 (module build), OpenSSL · port 6379 · [Repo](https://github.com/redis/redis) · [📖 Docs ↗](https://redis.io/docs/) · [🌐 Site ↗](https://redis.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/redis/)</sub>

<a name="nocodb"></a>
### #&#8288;31 [nocodb](https://github.com/nocodb/nocodb) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · custom license · Nov 2026</sub>

**Spreadsheet-style web UI and REST API on top of SQL databases.**

NocoDB provides an Airtable-like interface for creating and editing tables, with grid, gallery, form, kanban and calendar views. It exposes data through REST APIs and an SDK, and runs on SQLite by default or PostgreSQL via NC_DB. It is a general no-code database tool; the README mentions no AI features.

- **+** Five view types: grid, gallery, form, kanban, calendar
- **+** Role-based access control, plus public or password-protected shared views
- **+** Runs on SQLite by default or PostgreSQL through the NC_DB variable
- **+** Auto-upstall script sets up PostgreSQL, Redis, Traefik and SSL via Docker Compose
- **−** Sustainable Use License, not a standard OSI open-source license
- **−** README describes no AI or LLM features, so it is a loose fit for an AI list
- **−** Standalone binaries are documented only for quick local testing
- **−** Auto-upstall pipes a remote shell script into bash

<sub>no GPU · Compose · Needs SQLite or PostgreSQL, Redis (auto-upstall setup), Traefik (auto-upstall setup) · port 8080 · [Repo](https://github.com/nocodb/nocodb) · [📖 Docs ↗](https://docs.nocodb.com/) · [🌐 Site ↗](https://www.nocodb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nocodb/)</sub>

<a name="onedev"></a>
### #&#8288;32 [onedev](https://github.com/theonedev/onedev) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Nov 2026</sub>

**Self-hosted Git server with CI/CD, issues, packages and AI agents.**

OneDev is a Java-based self-hosted Git platform that combines code hosting, pull requests, kanban and issue workflows, a GUI-driven CI/CD system, package registries and a wiki. It also offers built-in AI users that review pull requests and fix CI failures, and browser workspaces where terminal agents such as Claude Code, Codex and OpenCode run in dev containers or sandbox VMs.

- **+** Git, CI/CD, issues, packages and wiki in one server, cross-referenced with each other
- **+** README says a 1 core, 2 GB box handles medium-sized projects
- **+** Jobs run in containers, on bare metal or sandbox VMs, scaled via Kubernetes or agents
- **+** Cluster mode replicates projects for availability or distributes them for scale
- **−** Supports only Linux and Windows (amd64/arm64) and Apple Silicon macOS; Intel Macs and FreeBSD dropped
- **−** Broad scope (AI users, workspaces, service desk) means more to configure than a plain Git host
- **−** README gives no Docker instructions; setup is in the external installation guide
- **−** Issues and pull requests go to the maintainers' own instance, not this repository

<sub>RAM ≥ 2 GB · no GPU · Models: OpenCode, Claude Code, Codex · [Repo](https://github.com/theonedev/onedev) · [▶️ Demo ↗](https://code.onedev.io) · [📖 Docs ↗](https://docs.onedev.io) · [🌐 Site ↗](https://onedev.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/onedev/)</sub>

<a name="casdoor"></a>
### #&#8288;33 [casdoor](https://github.com/casdoor/casdoor) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**Self-hosted SSO and identity provider with web console.**

Casdoor is a Go identity and access management server that stores users, issues tokens and provides a web console. It supports OAuth 2.0, OIDC, SAML 2.0, CAS, LDAP, SCIM 2.0, WebAuthn and TOTP/MFA, with social login via Google, GitHub and Entra ID. It also includes an MCP gateway and A2A support, and authorization uses Casbin models.

- **+** Many protocols on one user directory: OAuth, OIDC, SAML, CAS, LDAP, SCIM
- **+** Organizations, applications and providers editable in the UI without redeploy
- **+** Config as code via init data file and an official Terraform provider
- **+** SDKs for Go, Java, Python, Node.js, .NET, PHP and Rust, plus app Marketplace
- **−** All-in-one Docker image keeps SQLite data in the container; not for production
- **−** Compose file builds from source, so first start takes several minutes
- **−** Running more than one replica requires Redis
- **−** Old Ant Design console is no longer built; upgrading from v3 to v4 needs a guide

<sub>no GPU · Docker + Compose · Needs MySQL, PostgreSQL, SQLite or SQL Server, Redis (optional, needed for multiple replicas) · port 8000 · [Repo](https://github.com/casdoor/casdoor) · [▶️ Demo ↗](https://demo.casdoor.com) · [📖 Docs ↗](https://casdoor.ai/docs/overview) · [🌐 Site ↗](https://casdoor.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/casdoor/)</sub>

<a name="temporal"></a>
### #&#8288;34 [temporal](https://github.com/temporalio/temporal) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Nov 2026</sub>

**Durable execution server that runs workflows and retries failed steps.**

Temporal is the server side of a durable execution platform, written in Go. It runs application logic as Workflows that survive intermittent failures and retry failed operations automatically. It began as a fork of Uber's Cadence; workflows and workers are written with separate language SDKs, and a local dev server starts with `temporal server start-dev`.

- **+** MIT licensed, with a release published within the last two weeks
- **+** Local dev server starts with one CLI command and includes a Web UI on port 8233
- **+** Fork of Uber's Cadence, built by Cadence's creators
- **+** Ships a CLI for listing namespaces and workflows on a running server
- **−** Repo holds only the server; workflows need a separate SDK and worker code
- **−** README gives samples for Go and Java only
- **−** Production deployment, persistence and sizing are not covered in the README
- **−** No Docker or compose files detected in the repository

<sub>Docker · port 8233 · [Repo](https://github.com/temporalio/temporal) · [📖 Docs ↗](https://docs.temporal.io/) · [🌐 Site ↗](https://temporal.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/temporal/)</sub>

<a name="bytebase"></a>
### #&#8288;35 [bytebase](https://github.com/bytebase/bytebase) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Nov 2026</sub>

**Database change review, access control and audit platform for SQL and NoSQL.**

Bytebase sits between users, including AI agents, and databases such as PostgreSQL, MySQL, SQL Server, Oracle, MongoDB, Redis and Snowflake. It provides a web console for reviewing and deploying schema changes, with GitHub/GitLab GitOps, 200+ SQL lint rules, role-based access, just-in-time grants, data masking and audit logs. It also ships an MCP server and AI text-to-SQL in its SQL editor.

- **+** Covers many engines: PostgreSQL, MySQL, SQL Server, Oracle, MongoDB, Redis, Snowflake, ClickHouse and more
- **+** Combines change review, JIT access, column masking and audit logging in one console
- **+** Policies manageable as code through a Terraform provider and an API
- **+** Single docker run on port 8080 or a Helm chart for Kubernetes
- **−** Governance tool for existing databases, not a backend to build an app on
- **−** Which features need a paid plan is not clear from the README
- **−** Several moving parts (RBAC, policies, GitOps) add setup effort for small teams
- **−** AI features are secondary and need extra integration to be useful

<sub>no GPU · port 8080 · [Repo](https://github.com/bytebase/bytebase) · [📖 Docs ↗](https://docs.bytebase.com) · [🌐 Site ↗](https://www.bytebase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bytebase/)</sub>

<a name="go-admin"></a>
### #&#8288;36 [go-admin](https://github.com/go-admin-team/go-admin) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

**Go admin-panel backend with RBAC, code generation and Vue front ends.**

go-admin is a Gin + GORM backend for admin panels, paired with a separate Vue front end (Element UI, Arco Design or Ant Design). It provides Casbin RBAC, JWT auth, Swagger docs, user, role, menu and department management, operation logs, and a generator that produces CRUD code from table structures. It has no AI features.

- **+** Casbin RBAC with organization-based data-scope permissions, JWT auth and Swagger docs included
- **+** Code generator creates CRUD from table structure; form builder included
- **+** SQLite quick start; MySQL, PostgreSQL and SQL Server also supported
- **+** migrate and server subcommands, Dockerfile and cross-compile instructions
- **−** No AI or LLM functionality; a conventional admin boilerplate
- **−** Front end is a separate repo (go-admin-ui) that must be cloned alongside
- **−** SQLite build needs cgo and a C compiler, which fails on Windows without gcc
- **−** Unit tests are listed as TODO; much tutorial material is Chinese-language video

<sub>no GPU · Docker + Compose · Needs MySQL, PostgreSQL, SQL Server or SQLite, go-admin-ui front end, Node.js 22+ and pnpm 9+ for the UI · port 8000 · [Repo](https://github.com/go-admin-team/go-admin) · [▶️ Demo ↗](https://vue.go-admin.pro/#/login) · [📖 Docs ↗](https://www.go-admin.pro) · [🌐 Site ↗](https://www.go-admin.pro) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-admin/)</sub>

<a name="dapr"></a>
### #&#8288;37 [dapr](https://github.com/dapr/dapr) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

**Sidecar runtime for durable workflows, agents and distributed app APIs.**

Dapr runs as a sidecar next to your app and exposes building blocks over HTTP and gRPC: workflows with durable execution, service invocation with mTLS, state, pub/sub, actors, secrets, jobs and an LLM Conversation API. SDKs exist for .NET, Java, Python, Go, JavaScript/TypeScript and Rust. It is a CNCF graduated project written in Go, and it runs on Kubernetes, VMs or a laptop.

- **+** Workflows resume from the last completed step after crashes, restarts or rolling deploys
- **+** Sidecar model works from any language over HTTP and gRPC, with SDKs for six main languages
- **+** Built-in mTLS, workload identity and deny-by-default access policies
- **+** CNCF graduated; runs on Kubernetes, VMs, edge and air-gapped setups
- **−** Not an agent framework; agent logic still comes from your own code or another library
- **−** Adds a sidecar and component configuration to every deployment
- **−** Backing stores and brokers must be supplied and configured separately
- **−** README gives no starter app, so setup follows the separate docs and quickstarts

<sub>no GPU · Docker · Needs State store and message broker of your choice, Kubernetes (optional) · Models: LLMs via the Conversation API (providers unknown) · [Repo](https://github.com/dapr/dapr) · [📖 Docs ↗](https://docs.dapr.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dapr/)</sub>

<a name="openship"></a>
### #&#8288;38 [openship](https://github.com/oblien/openship) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**Self-hostable deployment platform that builds and routes apps from Git.**

Openship detects the stack of a GitHub repo, local folder or prebuilt artifact, builds it into a Docker image or bare release, runs it, and configures an OpenResty edge with Let's Encrypt certificates. It can be driven from a desktop app, web dashboard, CLI or JS/TS SDK, and exposes an MCP endpoint and REST API.

- **+** Auto-detects stack, build commands and port; openship.json is optional for overrides
- **+** Push-to-deploy via GitHub webhook, with rollbacks and monorepo-aware rebuilds
- **+** Manages databases, domains, TLS, backups and a built-in SMTP mail server
- **+** Desktop app, dashboard, CLI, SDK and MCP endpoint all work against one instance
- **−** Hosting apps on the same box needs Linux with Docker; macOS and Windows deploy over SSH
- **−** API container mounts the host Docker socket, so it should run only on a trusted host
- **−** Bundles a GPL-licensed iRedMail engine in several distributions despite the Apache-2.0 core
- **−** Multi-node clusters, load-balancing UI and private networking are still listed as upcoming

<sub>no GPU · Compose · Needs Docker (Compose mode), Postgres, Redis, OpenResty, Node 22+ (npm install) · [Repo](https://github.com/oblien/openship) · [📖 Docs ↗](https://openship.io/docs) · [🌐 Site ↗](https://openship.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openship/)</sub>

<a name="logto"></a>
### #&#8288;39 [logto](https://github.com/logto-io/logto) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MPL-2.0 · Nov 2026</sub>

**Self-hostable OIDC, OAuth 2.1 and SAML auth service with multi-tenancy and RBAC.**

Logto is an identity and auth server written in TypeScript that handles sign-in, social login, MFA, enterprise SSO, and organization-level RBAC. It ships pre-built sign-in flows and SDKs for 30+ frameworks, and the README says it also fits Model Context Protocol and agent-based setups. It can be self-hosted with Docker Compose or Node.js on PostgreSQL, or used as the managed Logto Cloud.

- **+** Supports OIDC, OAuth 2.1 and SAML, with enterprise SSO and multi-tenancy built in
- **+** SDKs for 30+ frameworks including React, Next.js, Angular, Vue, Flutter, Go, Python
- **+** Docker Compose one-liner for self-hosting; also installable via npm init @logto
- **+** Organization RBAC, member invites and just-in-time provisioning
- **−** Node.js install path requires a separately managed PostgreSQL database
- **−** MPL-2.0 has file-level copyleft, which may matter if you modify and ship it
- **−** Self-hosting means you operate and patch your own auth service

<sub>no GPU · Docker + Compose · Needs PostgreSQL, Docker (optional), Node.js (optional) · port 3002 · [Repo](https://github.com/logto-io/logto) · [📖 Docs ↗](https://docs.logto.io) · [🌐 Site ↗](https://logto.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/logto/)</sub>

<a name="kysely"></a>
### #&#8288;40 [kysely](https://github.com/kysely-org/kysely) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**Type-safe SQL query builder for TypeScript with autocompletion.**

Kysely is a TypeScript SQL query builder inspired by Knex.js. It checks table and column references at compile time and infers result row types, including aliases, subqueries and `with` statements. It targets Node.js and also runs on Deno, Bun, Cloudflare Workers and browsers. It is not an AI project, so it fits this list only loosely.

- **+** Result types contain only selected columns, with aliases inferred from the query
- **+** Dialects for PostgreSQL, MySQL, MSSQL, SQLite and PGlite
- **+** Runs on Node.js, Deno, Bun, Cloudflare Workers and browsers
- **+** `sql` template tag and DynamicModule cover queries that cannot be typed statically
- **−** Query builder only: no auth, storage or API layer, and no AI features
- **−** Table types must be declared or generated, for example with kysely-codegen
- **−** Not an ORM, so no relation mapping or model layer

<sub>no GPU · Compose · Needs PostgreSQL, MySQL, MSSQL, SQLite or PGlite database · [Repo](https://github.com/kysely-org/kysely) · [▶️ Demo ↗](https://kyse.link) · [📖 Docs ↗](https://kysely-org.github.io/kysely-apidoc/) · [🌐 Site ↗](https://kysely.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kysely/)</sub>

<a name="dagger"></a>
### #&#8288;41 [dagger](https://github.com/dagger/dagger) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

**Programmable engine for building, testing and shipping code in containers.**

Dagger runs build, test and deploy pipelines as typed functions that execute in containers, using the same definitions locally, in CI or in the cloud. Pipelines are written with SDKs for Go, Python, TypeScript, PHP, Java, .NET, Elixir and Rust, with content-addressed caching and OpenTelemetry traces for every operation. The README does not mention AI features, so its fit for this list is as delivery infrastructure.

- **+** SDKs for 8 languages generated from one API schema
- **+** Content-addressed incremental caching shared across local and CI runs
- **+** Every operation emits OpenTelemetry spans; exports to Jaeger or Honeycomb
- **+** Same pipeline behavior on laptop, CI server and cloud
- **−** Requires a Linux container runtime such as Docker, including Docker Desktop on macOS and Windows
- **−** README describes no AI or LLM features, so it is off-topic for most entries here
- **−** Pipelines must be rewritten as Dagger code; no import of existing CI YAML is described
- **−** Not a hosting platform; it does not deploy or run your apps

<sub>Needs Linux container runtime (e.g. Docker) · [Repo](https://github.com/dagger/dagger) · [📖 Docs ↗](https://docs.dagger.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dagger/)</sub>

<a name="falkordb"></a>
### #&#8288;42 [falkordb](https://github.com/falkordb/falkordb) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Nov 2026</sub>

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

<a name="webiny-js"></a>
### #&#8288;43 [webiny-js](https://github.com/webiny/webiny-js) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.1k · custom license · Nov 2026</sub>

**TypeScript headless CMS and website builder deployed to your AWS account.**

Webiny is a self-hosted headless CMS with a GraphQL API, a drag-and-drop Website Builder with a Next.js SDK, and a File Manager. It deploys to Lambda, DynamoDB, S3 and CloudFront through Pulumi with `yarn webiny deploy`. Customization is TypeScript code in an `extensions/` folder, and it ships an MCP server and skills for AI coding agents.

- **+** Serverless on Lambda, DynamoDB, S3 and CloudFront; no servers to patch or size
- **+** Typed extension points for API, admin UI, infrastructure and CLI
- **+** Multi-tenancy with hierarchical tenants, managed through the GraphQL API
- **+** Ships an MCP server and AI skills for Claude Code, Cursor and Kiro
- **−** Runs only on AWS; no GCP, Azure or on-prem option
- **−** RBAC, multi-tenancy and publishing workflows need a paid Business license
- **−** SSO and audit logs are Enterprise only
- **−** Extending it requires TypeScript and React; oversized for simple sites

<sub>no GPU · Needs AWS account, AWS Lambda, DynamoDB, S3, CloudFront, Pulumi, Node.js 22+, Yarn, OpenSearch (optional) · port 3001 · [Repo](https://github.com/webiny/webiny-js) · [📖 Docs ↗](https://www.webiny.com/docs) · [🌐 Site ↗](https://www.webiny.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/webiny-js/)</sub>

<a name="registry"></a>
### #&#8288;44 [registry](https://github.com/modelcontextprotocol/registry) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · custom license · Nov 2026</sub>

**Official registry server and publisher CLI for listing MCP servers.**

Go implementation of the MCP Registry, an HTTP API that gives MCP clients a catalog of published MCP servers. It stores data in PostgreSQL and ships an mcp-publisher CLI that publishes server.json entries, verifying namespace ownership via GitHub OAuth, GitHub OIDC, or DNS/HTTP challenges. The v0.1 API is under a freeze, and the project is still a preview release.

- **+** Namespace ownership checks via GitHub OAuth, GitHub OIDC, DNS or HTTP verification
- **+** Includes mcp-publisher CLI for publishing server.json entries
- **+** One command (make dev-compose) starts a dev stack seeded from the production API
- **+** Pre-built images published to GitHub Container Registry
- **−** Preview release; README warns of breaking changes or data resets before GA
- **−** Image does not bundle PostgreSQL; you must run and configure your own
- **−** Dev compose database is ephemeral and resets on every restart
- **−** Servers cannot be published through pull requests to this repo

<sub>no GPU · Compose · Needs PostgreSQL, Docker, ko · port 8080 · [Repo](https://github.com/modelcontextprotocol/registry) · [📖 Docs ↗](https://registry.modelcontextprotocol.io/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/registry/)</sub>

<a name="erupt"></a>
### #&#8288;45 [erupt](https://github.com/erupts/erupt) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Nov 2026</sub>

**Annotation-driven Java admin framework where one JPA entity becomes one admin page.**

Erupt generates admin UIs, REST endpoints and permission checks from annotations on JPA entities, on Java 17 and Spring Boot 3.x. It includes RBAC, Excel import/export and 30+ form components, plus an optional erupt-ai module with 50+ LLM providers, MCP tools and A2A. Workflow, multi-tenant and BI modules are commercial.

- **+** One annotated JPA entity yields paged, searchable, exportable, role-gated admin page without front-end code
- **+** Ships RBAC, row and column permissions, OAuth2/LDAP/SSO, Excel and OpenAPI in core modules
- **+** erupt-ai adds 50+ LLM providers, MCP over SSE and STDIO, and per-role tool whitelisting
- **+** Core modules are Apache 2.0; sample runs with in-memory H2 and no config
- **−** Java and Spring Boot only; JPA databases are MySQL, PostgreSQL, Oracle, SQL Server, DM
- **−** Workflow, multi-tenant SaaS and BI modules are paid, source-code delivery
- **−** Sends anonymous telemetry by default; opt-out via config or environment variable
- **−** UI customization is bounded by what the annotations expose

<sub>no GPU · Needs Java 17+, Spring Boot 3.x, Maven, JPA database (H2 default; MySQL, PostgreSQL, Oracle, SQL Server, DM), MongoDB (optional), Redis (optional) · Models: OpenAI, Claude, Gemini, DeepSeek, Qwen · port 8080 · [Repo](https://github.com/erupts/erupt) · [▶️ Demo ↗](https://demo.erupt.xyz) · [📖 Docs ↗](https://docs.erupt.xyz) · [🌐 Site ↗](https://www.erupt.xyz) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/erupt/)</sub>

<a name="parse-server"></a>
### #&#8288;46 [parse-server](https://github.com/parse-community/parse-server) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

**Node.js backend with REST, GraphQL, Live Query and Cloud Code.**

Parse Server is a Node.js backend that stores objects in MongoDB or PostgreSQL (with PostGIS) and exposes them through a REST API, GraphQL and Live Query. It runs standalone via the parse-server CLI or mounts on an existing Express app. Cloud Code, push notifications, file adapters and Parse SDKs cover server logic and client access.

- **+** Runs standalone via CLI or mounts into an existing Express app
- **+** Supports MongoDB 7 and 8 and PostgreSQL 16 to 18 with PostGIS
- **+** Access scopes via master, read-only master and session keys, plus CLP and ACL
- **+** Compatibility tables for Node.js, MongoDB and Postgres, plus an LTS branch
- **−** You must run and manage your own database
- **−** LTS branch only covers the previous major version, with limited security fixes
- **−** README has you build the Docker image locally; no compose file is provided
- **−** Dashboard is a separate project, not included in this repo

<sub>no GPU · Docker · Needs Node.js, MongoDB or PostgreSQL with PostGIS · port 1337 · [Repo](https://github.com/parse-community/parse-server) · [📖 Docs ↗](http://docs.parseplatform.org/parse-server/guide/) · [🌐 Site ↗](http://parseplatform.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/parse-server/)</sub>

<a name="flexprice"></a>
### #&#8288;47 [flexprice](https://github.com/flexprice/flexprice) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · AGPL-3.0 · Nov 2026</sub>

**Usage-based billing and metering API with credits, plans and invoicing.**

Flexprice is a Go billing backend that ingests usage events through an API or SDKs (Go, Python, JavaScript) and meters them in real time. It prices them against plans, applies prepaid or promotional credits, enforces feature entitlements and generates invoices. It can sync to payment, CRM and accounting tools, and runs on PostgreSQL, Kafka, ClickHouse and Temporal.

- **+** Covers usage, seat, tiered, prepaid-credit and hybrid pricing with per-customer plan overrides
- **+** Includes wallets, credit grants, auto top-ups and feature entitlements alongside invoicing
- **+** SDKs for Go, Python and JavaScript; make dev-setup starts the full stack via Compose
- **+** Can layer on existing providers such as Stripe or Chargebee instead of replacing them
- **−** Heavy infrastructure: PostgreSQL, Kafka, ClickHouse, Temporal and Redis all required
- **−** Open core: ee and internal/ee directories need a commercial license
- **−** AGPL-3.0 core may conflict with some company policies on network-served code
- **−** README gives no production deployment, sizing or throughput figures

<sub>no GPU · Docker + Compose · Needs PostgreSQL, Kafka, ClickHouse, Temporal, Redis, Docker Compose · port 8080 · [Repo](https://github.com/flexprice/flexprice) · [▶️ Demo ↗](https://www.loom.com/share/60d8308781254fe0bc5be341501f9fd5) · [📖 Docs ↗](https://docs.flexprice.io) · [🌐 Site ↗](https://flexprice.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flexprice/)</sub>

<a name="keystone"></a>
### #&#8288;48 [keystone](https://github.com/keystonejs/keystone) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · MIT · Nov 2026</sub>

**Schema-first headless CMS that generates a GraphQL API and admin UI.**

Keystone 6 is a Node.js CMS and app framework published on npm as @keystone-6/*. You describe a schema in TypeScript and it generates a GraphQL API and a management UI for the content and data. The README mentions no AI features, so it fits here only as a general backend base.

- **+** Schema definition produces both a GraphQL API and an admin UI
- **+** Written in TypeScript and distributed as npm packages
- **+** Follows semver and tracks Node Maintenance and Active LTS in CI
- **+** Includes runnable examples and an API reference
- **−** README describes no AI or LLM features
- **−** Guides and examples are still incomplete, per the README
- **−** No Docker or compose files in the repo for deployment
- **−** Keystone 5 is in maintenance mode, so migrating needs a separate codebase

<sub>no GPU · Needs Node.js (Maintenance or Active LTS) · [Repo](https://github.com/keystonejs/keystone) · [📖 Docs ↗](https://keystonejs.com/docs) · [🌐 Site ↗](https://keystonejs.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/keystone/)</sub>

<a name="vendure"></a>
### #&#8288;49 [vendure](https://github.com/vendurehq/vendure) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · custom license · Nov 2026</sub>

**TypeScript headless commerce backend with GraphQL APIs and a plugin system.**

Vendure is a Node.js, NestJS and GraphQL commerce backend covering catalog, orders, stock, promotions, payments, tax, shipping and multi-channel sales. It ships a React admin dashboard, a worker process and a CLI, and is extended through plugins and service overrides rather than forks. It is not an AI project; the README only notes that the introspectable schema can feed LLM tool-calling or MCP servers.

- **+** Typed Shop and Admin GraphQL APIs that can be extended with custom schema
- **+** Plugin contracts and service overrides change core behavior without forking
- **+** Built-in multi-channel, multi-currency, multi-language and multi-location stock
- **+** One npx command scaffolds server, worker and admin dashboard
- **−** GPLv3 core; a commercial license comes only with paid plans
- **−** B2B features (company accounts, quotes, SSO, audit logs) are in paid plans only
- **−** Needs an external SQL database: PostgreSQL, MySQL, MariaDB or SQLite
- **−** No AI features built in; MCP or agent integration is left to you

<sub>no GPU · Compose · Needs Node.js 22.12+, PostgreSQL, MySQL, MariaDB or SQLite · [Repo](https://github.com/vendurehq/vendure) · [📖 Docs ↗](https://docs.vendure.io) · [🌐 Site ↗](https://vendure.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vendure/)</sub>

<a name="teable"></a>
### #&#8288;50 [teable](https://github.com/teableio/teable) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

**Airtable-style collaborative database on PostgreSQL with AI chat and app builder.**

Teable is a spreadsheet-style database UI over PostgreSQL, with grid, form, kanban, gallery and calendar views, formulas, an API, and automations triggered by record changes, schedules or webhooks. The full self-hosted setup adds AI chat and an App Builder that runs agents in per-session sandbox containers and deploys apps as containers. The standalone install covers tables and automation only.

- **+** Data lives in real PostgreSQL, with an HTTP API and SQL query support
- **+** Five view types plus formulas, record history, undo/redo and real-time collaboration
- **+** Automations run on record changes, schedules and webhooks, with optional AI steps
- **+** Standalone install is available when AI features are not needed
- **−** Standalone self-host has no AI chat or App Builder
- **−** AI features need a paid plan activated with a license key
- **−** Full-featured self-host needs a separate deployment repo with multiple runtime components
- **−** Community edition is AGPL-3.0, which constrains closed-source network use

<sub>Needs PostgreSQL · [Repo](https://github.com/teableio/teable) · [▶️ Demo ↗](https://teable.ai) · [📖 Docs ↗](https://help.teable.ai) · [🌐 Site ↗](https://teable.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/teable/)</sub>

<a name="dgraph"></a>
### #&#8288;51 [dgraph](https://github.com/dgraph-io/dgraph) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Oct 2026</sub>

**Distributed graph database with a GraphQL-inspired query language.**

Dgraph is a sharded, distributed graph database written in Go. It provides distributed ACID transactions, consistent replication and linearizable reads, and is queried with a GraphQL-inspired language over gRPC or HTTP, returning JSON or Protocol Buffers. It is a general-purpose database backend rather than an AI-specific starter.

- **+** Distributed ACID transactions with consistent replication and linearizable reads
- **+** Automatic shard rebalancing across a cluster
- **+** Native full-text, regex and geo search without an external index
- **+** Official Docker image plus a standalone image for a quick single-node start
- **−** Official support only for Linux amd64 and arm64; Mac and Windows dropped in 2021
- **−** Query language is GraphQL-inspired, so Cypher or Gremlin queries need porting
- **−** Building from source needs Go 1.27+ and a C build toolchain
- **−** README describes no AI or vector search features

<sub>no GPU · Docker · port 8080 · [Repo](https://github.com/dgraph-io/dgraph) · [📖 Docs ↗](https://docs.dgraph.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dgraph/)</sub>

<a name="databend"></a>
### #&#8288;52 [databend](https://github.com/databendlabs/databend) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (51) · Freshness: active (98) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · Apache-2.0 · Nov 2026</sub>

**Rust data warehouse with SQL analytics, vector and full-text search on object storage.**

Databend is a data warehouse written in Rust that stores tables on object storage (S3, Azure, GCS). It runs SQL analytics, vector search via VECTOR INDEX, and full-text search via INVERTED INDEX on the same tables. It also supports Python UDFs run in sandbox workers and Git-like data branching, so agent workloads can run from SQL.

- **+** Vector, full-text and analytic queries run on the same table without a second system
- **+** Compute is separate from storage on S3, Azure Blob or GCS
- **+** Python UDFs run in sandbox workers and are called from plain SQL
- **+** Published TPC-H and search benchmarks, each with SQL to reproduce
- **−** Published benchmarks were run on Databend Cloud, not on self-hosted clusters
- **−** Some enterprise features are under Elastic 2.0, not Apache 2.0
- **−** Sandbox UDF needs separate sandbox workers; self-hosted setup is not covered in the README
- **−** Branching is mentioned but has no usage example in the README

<sub>Docker + Compose · Needs Object storage (S3, Azure Blob, GCS), BendSQL client · port 8000 · [Repo](https://github.com/databendlabs/databend) · [📖 Docs ↗](https://docs.databend.com/) · [🌐 Site ↗](https://databend.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/databend/)</sub>

<a name="nhost"></a>
### #&#8288;53 [nhost](https://github.com/nhost/nhost) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · MIT · Nov 2026</sub>

**Open-source Firebase alternative on Postgres, Hasura GraphQL, auth and storage.**

Nhost bundles PostgreSQL, a Hasura-generated GraphQL API, an auth service, file storage and Node.js serverless functions into one backend. It runs on the hosted Nhost platform, locally through the Nhost CLI, or self-hosted from an example docker-compose file. The CLI also ships an MCP server that lets coding assistants read the GraphQL schema, run allowed queries and manage metadata and migrations.

- **+** Full backend in one stack: Postgres, Hasura GraphQL, auth, storage and functions
- **+** CLI runs a local environment that tracks database migrations and Hasura metadata
- **+** Built-in MCP server in the CLI for Claude Code, Cursor, Codex and Gemini CLI
- **+** MIT licensed, with a JavaScript/TypeScript client and a Dart/Flutter client
- **−** GraphQL-first through Hasura; no REST-first or other database options are documented
- **−** Self-hosting guidance in the README is only an example docker-compose file
- **−** Serverless functions are Node.js only (JavaScript and TypeScript)

<sub>no GPU · Needs PostgreSQL, Hasura · README: alternative to Firebase · [Repo](https://github.com/nhost/nhost) · [📖 Docs ↗](https://docs.nhost.io) · [🌐 Site ↗](https://nhost.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nhost/)</sub>

<a name="devpush"></a>
### #&#8288;54 [devpush](https://github.com/hunvreus/devpush) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Nov 2026</sub>

**Self-hosted deploy platform for Docker Compose apps, triggered by GitHub pushes.**

devpush deploys Docker Compose apps from a connected GitHub repository to your own Linux servers. A small agent on each server handles HTTPS, deployment logs, monitoring and backups, while the dashboard runs on Cloudflare Workers or Node. It includes teams, environments, encrypted variables, a REST API and MCP.

- **+** Dashboard runs on Cloudflare Workers or Node, with a small Linux agent per server
- **+** Built-in HTTPS, deployment logs, monitoring and backups
- **+** Teams, environments, encrypted variables, REST API and MCP included
- **+** Installs with one command: npx devpush@latest init
- **−** Docker Compose is required; Dockerfiles only work inside a Compose file
- **−** In-place updates do not guarantee zero downtime
- **−** Only trusted code should be deployed; Docker workloads can access the host
- **−** Only GitHub is mentioned as a repository source

<sub>no GPU · Docker + Compose · Needs Docker Compose, GitHub, Cloudflare Workers or Node.js · port 7429 · [Repo](https://github.com/hunvreus/devpush) · [▶️ Demo ↗](https://devpu.sh/videos/devpush-demo.mp4) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devpush/)</sub>

<a name="angularfire"></a>
### #&#8288;55 [angularfire](https://github.com/angular/angularfire) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

**Angular library wrapping the Firebase JS SDK with DI and RxJS observables.**

AngularFire is an Angular library that wraps the Firebase JS SDK so Firebase services are provided through dependency injection and real-time data is exposed as RxJS observables. It covers Firestore, Realtime Database, Auth, Storage, Functions, Messaging, Analytics, App Check, AI Logic, Data Connect, Performance Monitoring and Remote Config. It installs with `ng add @angular/fire`.

- **+** Covers twelve Firebase products, each under its own @angular/fire/* import path
- **+** Zone.js wrappers aimed at SSR, pre-rendering and service worker compatibility
- **+** Firestore reads return typed observables via collectionData and data converters
- **+** Route guards for Firebase Authentication and Angular Router-aware Google Analytics
- **−** Only useful with Angular and a Firebase project; it is a client library, not a backend
- **−** Depends on the Firebase JS SDK, so SDK issues must be reported upstream
- **−** Issues and mailing list questions are answered on an as-available basis
- **−** Major version upgrades need migration guides (v7, v21, v22)

<sub>no GPU · Needs Angular, Firebase JS SDK, RxJS, Firebase project · [Repo](https://github.com/angular/angularfire) · [▶️ Demo ↗](https://stackblitz.com/edit/angular-fire-start) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/angularfire/)</sub>

<a name="graphjin"></a>
### #&#8288;56 [graphjin](https://github.com/dosco/graphjin) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Nov 2026</sub>

**GraphQL-to-SQL compiler that exposes databases to AI agents over MCP.**

GraphJin compiles GraphQL queries into single SQL statements and serves them as a Go library or standalone service with REST, WebSocket/SSE subscriptions and an MCP endpoint. It connects to Postgres, MySQL, MongoDB, SQLite, Snowflake, BigQuery and others, plus S3/GCS files and indexed source code. A built-in agent endpoint answers instructions using the caller's permissions.

- **+** Supports many sources: Postgres, MySQL, MongoDB, SQLite, Oracle, MSSQL, Snowflake, BigQuery, S3/GCS
- **+** Subscriptions batch many subscribers into one database query
- **+** Built-in demo runs with `graphjin serve --demo` on SQLite, no Docker
- **+** Installs via npm, Homebrew, Scoop, deb/rpm or Docker
- **−** Broad scope (agent, workflows, CodeSQL, watches) makes the config surface large
- **−** Built-in agent needs an OpenAI, Anthropic or Google API key
- **−** Subscriptions unsupported on dialects without batched polling
- **−** Analytics directives error on MongoDB and older database versions

<sub>no GPU · Docker · Needs PostgreSQL, MySQL, MongoDB, SQLite or other supported database, Model API key for built-in agent (optional) · Models: OpenAI, Anthropic, Google · port 8080 · [Repo](https://github.com/dosco/graphjin) · [📖 Docs ↗](https://graphjin.com/agentic/server-agent/) · [🌐 Site ↗](https://graphjin.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphjin/)</sub>

<a name="kong"></a>
### #&#8288;57 [kong](https://github.com/kong/kong) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Oct 2026</sub>

**API gateway with LLM and MCP traffic routing, extended through plugins.**

Kong Gateway is a Lua-based API gateway that proxies, routes, load balances and authenticates HTTP and L4 traffic, with behavior extended by plugins. Its AI features add a universal LLM API across providers such as OpenAI, Anthropic, Gemini, Bedrock and Azure AI, plus MCP traffic governance and MCP generation from REST APIs. It runs with Postgres, in DB-less mode, or in a hybrid control plane/data plane setup.

- **+** Plugins for auth, rate limiting, transformations and logging; writable in Lua, Go or JavaScript
- **+** One LLM API fronting OpenAI, Anthropic, Gemini, Bedrock, Azure AI, Mistral and others
- **+** DB-less declarative config, Postgres-backed, or hybrid control/data plane deployment
- **+** Official Kubernetes Ingress Controller; Admin API on 8001, Kong Manager UI on 8002
- **−** General API gateway, not an AI app starter; AI is one feature set among many
- **−** Analytics, service catalog and developer portals are in the paid Konnect offering
- **−** Needs gateway concepts (services, routes, plugins) and often Postgres to operate
- **−** README quick start uses the separate docker-kong repo, not this repository

<sub>no GPU · Needs PostgreSQL (optional, not needed in DB-less mode) · Models: OpenAI, Anthropic, GCP Gemini, AWS Bedrock, Azure AI · port 8002 · [Repo](https://github.com/kong/kong) · [📖 Docs ↗](https://docs.konghq.com) · [🌐 Site ↗](https://konghq.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kong/)</sub>

<a name="apijson"></a>
### #&#8288;58 [apijson](https://github.com/apijson/apijson) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Nov 2026</sub>

**Java ORM serving JSON-defined CRUD APIs over many databases without endpoint code.**

APIJSON is a Java library and JSON-based protocol where clients describe the data shape they want in the request body and the server turns it into queries, so backend developers do not write per-endpoint CRUD code. It supports reads and writes, fuzzy search, remote function calls and multi-table queries in one request, and generates API docs. The README lists many database targets (MySQL, PostgreSQL, Oracle, ClickHouse, Redis, Kafka and others) and community ports in Go, C#, PHP, Node.js, Python and Rust.

- **+** Clients shape responses and join related tables in a single request
- **+** Wide database coverage: MySQL, PostgreSQL, Oracle, SQL Server, ClickHouse, Redis, Kafka and more
- **+** Generated API docs and the APIAuto test UI cut backend documentation work
- **+** Published via JitPack for Maven and Gradle, with Spring Boot demos
- **−** License is detected as NOASSERTION, so terms need manual checking
- **−** Core is Java; Go, C#, PHP and Rust ports are separate third-party repos
- **−** Documentation and community material lean Chinese-first
- **−** Library rather than a deployable service; no Docker or compose files in the repo

<sub>no GPU · Needs Java 1.8+, A supported database such as MySQL or PostgreSQL · [Repo](https://github.com/apijson/apijson) · [▶️ Demo ↗](http://apijson.cn/api) · [📖 Docs ↗](https://github.com/APIJSON/APIJSON/blob/master/Document.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apijson/)</sub>

<a name="insforge"></a>
### #&#8288;59 [insforge](https://github.com/insforge/insforge) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

**Postgres-based backend platform that coding agents operate through an MCP server.**

InsForge bundles Postgres, auth, S3-compatible storage, edge functions, an OpenAI-compatible model gateway and site deployment behind an MCP server. Coding agents read docs, schemas and logs, and run migrations, deploy functions and create buckets as tools. Self-hosting uses Docker Compose with generated secrets; a hosted cloud edition also exists.

- **+** Covers auth, Postgres, storage, edge functions and model gateway in one stack
- **+** MCP server exposes schemas, logs and config so agents can verify their own work
- **+** Setup script generates JWT, encryption and database secrets into a mode 600 .env
- **+** Storage can use local disk, bundled MinIO or RustFS, or any S3-compatible store
- **−** CLI + Skills interface is cloud only; self-hosted gets the MCP server only
- **−** Compute (long-running containers) is in private preview
- **−** Running several instances needs manual per-project names and port overrides

<sub>no GPU · Docker + Compose · Needs Docker with Compose v2, Postgres, S3-compatible store (optional) · Models: OpenAI-compatible gateway across multiple LLM providers · port 7130 · [Repo](https://github.com/insforge/insforge) · [📖 Docs ↗](https://docs.insforge.dev/introduction) · [🌐 Site ↗](https://insforge.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/insforge/)</sub>

<a name="cloudnative-pg"></a>
### #&#8288;60 [cloudnative-pg](https://github.com/cloudnative-pg/cloudnative-pg) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · Apache-2.0 · Nov 2026</sub>

**Kubernetes operator that runs and manages PostgreSQL primary/standby clusters.**

CloudNativePG is a Go Kubernetes operator that manages the lifecycle of vanilla PostgreSQL clusters: deployment, failover, replica scaling, rolling updates and backups. It talks to the Kubernetes API directly instead of using Patroni, repmgr or Stolon, and exposes cluster status on the Cluster resource. It is a CNCF Sandbox project, originally built and sponsored by EDB.

- **+** Uses the Kubernetes API for failover, with no Patroni, repmgr or Stolon
- **+** Rolling updates upgrade replicas first, then switch over the primary
- **+** Custom resources for Backup, ScheduledBackup, Pooler, Database, Publication and Subscription
- **+** Extensible through the CNPG-I plugin interface
- **−** Kubernetes only; no support for other orchestrators
- **−** PostgreSQL only; no other databases such as MariaDB
- **−** PostgreSQL forks are supported only as extensions or pluggable frameworks
- **−** Targets vanilla upstream Kubernetes; other distributions are not described

<sub>no GPU · Docker · Needs Kubernetes, PostgreSQL · [Repo](https://github.com/cloudnative-pg/cloudnative-pg) · [📖 Docs ↗](https://cloudnative-pg.io/docs) · [🌐 Site ↗](https://cloudnative-pg.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloudnative-pg/)</sub>

<a name="cakephp"></a>
### #&#8288;61 [cakephp](https://github.com/cakephp/cakephp) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.8k · MIT · Nov 2026</sub>

**MVC web application framework for PHP with data mapping and front controller.**

CakePHP is a PHP web framework built on MVC, Front Controller and associative data mapping patterns. It installs through Composer, either into an existing project or via the separate app skeleton for new ones. It has no AI features and fits this list only as a general backend framework.

- **+** Installs with a single `composer require cakephp/cakephp`
- **+** Test suite runs on SQLite by default; other databases optional via phpunit.xml
- **+** Static analysis at PHPStan level 8 with tracked code coverage
- **+** Separate app skeleton repo for starting new projects
- **−** No built-in AI, model or agent integration
- **−** PHP only; no other language bindings
- **−** Framework library, not a ready-to-run backend with auth or storage service

<sub>no GPU · Docker · Needs PHP, Composer · [Repo](https://github.com/cakephp/cakephp) · [📖 Docs ↗](https://book.cakephp.org) · [🌐 Site ↗](https://cakephp.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cakephp/)</sub>

<a name="graphql-yoga"></a>
### #&#8288;62 [graphql-yoga](https://github.com/graphql-hive/graphql-yoga) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · MIT · Nov 2026</sub>

**GraphQL server library for Node, Deno, Bun and edge runtimes.**

GraphQL Yoga is a TypeScript GraphQL server built on the WHATWG Fetch API, so the same handler runs on Node, Deno, Bun, Cloudflare Workers and AWS Lambda. It includes GraphiQL, subscriptions over Server-Sent Events, file uploads, persisted queries and parsing/validation caching. Envelop plugins extend it. It is a general GraphQL library with no AI features.

- **+** Fetch-API core runs on Node, Deno, Bun, Workers and Lambda
- **+** Compliant with the GraphQL over HTTP spec; works with Apollo, Relay and urql
- **+** Subscriptions use Server-Sent Events, no WebSocket server required
- **+** Supports Envelop plugins; ships GraphiQL, file uploads and automatic persisted queries
- **−** Library only: no auth, database or storage layer included
- **−** No AI, model or agent functionality; not an AI project
- **−** Contributing guide pins pnpm 8, which suggests an older toolchain

<sub>no GPU · Needs graphql · port 4000 · [Repo](https://github.com/graphql-hive/graphql-yoga) · [📖 Docs ↗](https://www.the-guild.dev/graphql/yoga-server/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphql-yoga/)</sub>

<a name="encore"></a>
### #&#8288;63 [encore](https://github.com/encoredev/encore) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MPL-2.0 · Nov 2026</sub>

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

<a name="trailbase"></a>
### #&#8288;64 [trailbase](https://github.com/trailbaseio/trailbase) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (37) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · OSL-3.0 · Nov 2026</sub>

**Single-executable Firebase alternative on Rust and SQLite with REST and realtime APIs.**

TrailBase is a backend server written in Rust that bundles type-safe REST and realtime APIs, auth, an admin UI, a WebAssembly runtime and geospatial support on SQLite. Postgres is available experimentally from v0.28. It ships as one executable for Linux, macOS and Windows, with client libraries for eight languages. The project is marked alpha.

- **+** Single executable with no runtime dependencies; also published as a Docker image
- **+** Client libraries for JS/TS, Dart, Rust, C#, Swift, Kotlin, Go and Python
- **+** Extensible with WASM components, e.g. an optional auth UI added via one command
- **+** Client libraries are Apache-2.0, and the README says app code is not covered by OSL copyleft
- **−** Marked alpha status in the README
- **−** Postgres support is experimental; SQLite is the primary database
- **−** OSL-3.0 server license is less common, and the README admits compatibility is unclear
- **−** Contributions beyond bug fixes require signing a CLA

<sub>no GPU · Docker + Compose · Needs SQLite (bundled), Postgres (optional, experimental) · port 4000 · README: alternative to Firebase · [Repo](https://github.com/trailbaseio/trailbase) · [▶️ Demo ↗](https://demo.trailbase.io/_/admin?loginMessage=E-mail:%20admin@localhost%20%E2%80%A2%20Password:%20secret) · [🌐 Site ↗](https://trailbase.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trailbase/)</sub>

<a name="realm-swift"></a>
### #&#8288;65 [realm-swift](https://github.com/realm/realm-swift) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Sep 2026</sub>

**On-device object database for iOS, macOS, tvOS and watchOS apps.**

Realm Swift and Realm Objective-C are an embedded mobile database that stores objects on disk without an ORM. Models are Swift classes with @Persisted properties, and live objects, notifications and SwiftUI property wrappers such as @ObservedResults keep views in sync. Realms can be encrypted with a 64-byte key and installed through Swift Package Manager, CocoaPods, Carthage or XCFramework.

- **+** Object model with @Persisted classes needs no ORM or schema files
- **+** Live objects and observe() notifications update data across the app
- **+** SwiftUI wrappers like @ObservedResults bind queries directly to views
- **+** At-rest encryption via a 64-byte key in Realm.Configuration
- **−** Apple platforms only: iOS, macOS, tvOS and watchOS
- **−** Building from source requires Xcode 15.3 or newer
- **−** Local embedded store; README describes no server-side or hosted component
- **−** Not a fit for server backends or non-Apple clients

<sub>no GPU · Needs Xcode 15.3+ (building from source) · [Repo](https://github.com/realm/realm-swift) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/realm-swift/)</sub>

<a name="convex-backend"></a>
### #&#8288;66 [convex-backend](https://github.com/convex/convex-backend) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · custom license · Nov 2026</sub>

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

<a name="kubevela"></a>
### #&#8288;67 [kubevela](https://github.com/kubevela/kubevela) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · Apache-2.0 · Nov 2026</sub>

**Kubernetes app delivery control plane with CUE workflows and multi-cluster rollout.**

KubeVela is a Go application delivery platform built on the Open Application Model. It renders application definitions and runs deployment workflows, extensible with CUE, across multiple clusters and clouds, including canary and blue-green rollouts. It has no AI features; it fits this list only as general infrastructure for shipping apps.

- **+** Deployment workflows are programmable in CUE, with extensible steps
- **+** Multi-cluster placement, canary and blue-green rollout are built in
- **+** Control plane stated to run as one pod at 0.5 CPU and 1 GB
- **+** LDAP integrations, RBAC, multi-tenancy and community addons included
- **−** Requires a Kubernetes cluster; no standalone mode described
- **−** No AI or LLM features, so off-topic for an AI-focused list
- **−** Custom definitions need familiarity with OAM and CUE
- **−** README has no install steps; they live on the docs site

<sub>RAM ≥ 1 GB · no GPU · Docker · Needs Kubernetes · [Repo](https://github.com/kubevela/kubevela) · [📖 Docs ↗](https://kubevela.io/docs) · [🌐 Site ↗](https://kubevela.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubevela/)</sub>

<a name="pixeltable"></a>
### #&#8288;68 [pixeltable](https://github.com/pixeltable/pixeltable) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="openstatus"></a>
### #&#8288;69 [openstatus](https://github.com/openstatushq/openstatus) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (50) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · AGPL-3.0 · Nov 2026</sub>

**Status pages, uptime monitoring and incident response, configured as code.**

openstatus combines public status pages, uptime checks from 28 regions and incident management in one platform. Monitors, pages and notification channels are declared in YAML or Terraform and applied from a CLI or CI, and an MCP server and Slack agent can operate incidents. The stack is a Next.js dashboard, a Hono API, a Go checker, Turso for data and Tinybird for analytics, self-hosted via Docker Compose, Coolify or Railway.

- **+** Monitors and status pages declared in YAML or Terraform, applied from CLI or CI
- **+** MCP server, --json CLI and typed API with read-only or read-write key scopes
- **+** Checks run from 28 regions across 3 cloud providers
- **+** Prebuilt images and Compose, Coolify and Railway deployment paths
- **−** Needs several services: dashboard, API, workflows, checker, libSQL and Tinybird
- **−** AGPL-3.0 license restricts closed-source network use
- **−** Enterprise features are offered by contact; the README does not list which
- **−** No tagged release; self-hosters track the main branch or latest images

<sub>no GPU · Compose · Needs Docker, Turso/libSQL, Tinybird, Node.js, pnpm · port 3002 · [Repo](https://github.com/openstatushq/openstatus) · [▶️ Demo ↗](https://status.openstatus.dev) · [📖 Docs ↗](https://www.openstatus.dev/docs) · [🌐 Site ↗](https://www.openstatus.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openstatus/)</sub>

<a name="fission"></a>
### #&#8288;70 [fission](https://github.com/fission/fission) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · Apache-2.0 · Nov 2026</sub>

**Kubernetes-native serverless functions with a warm container pool.**

Fission runs functions on a Kubernetes cluster from source code alone, using language-specific environments (NodeJS, Python, Ruby, Go, PHP, Bash, any Linux executable). Functions are triggered by HTTP requests, message queues or schedules and scale automatically. A pool of warm containers with a dynamic loader gives cold starts of about 100 ms. It is a general serverless framework with no AI-specific features.

- **+** Warm container pool gives cold starts of about 100 ms, per the README
- **+** Triggers include HTTP, message queues and scheduled tasks
- **+** Environments cover NodeJS, Python, Ruby, Go, PHP, Bash and Linux executables
- **+** Reuses existing Kubernetes monitoring and log aggregation tooling
- **−** Requires an existing Kubernetes cluster; no standalone mode described
- **−** Not AI-specific: no model serving, agent or LLM features
- **−** Languages beyond the stock set need a custom environment image
- **−** No Docker or Compose quick start in the repository

<sub>no GPU · Needs Kubernetes · [Repo](https://github.com/fission/fission) · [📖 Docs ↗](https://fission.io/docs) · [🌐 Site ↗](https://fission.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fission/)</sub>

<a name="zenstack"></a>
### #&#8288;71 [zenstack](https://github.com/zenstackhq/zenstack) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

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

<a name="oceanbase"></a>
### #&#8288;72 [oceanbase](https://github.com/oceanbase/oceanbase) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · Apache-2.0 · Oct 2026</sub>

**Distributed MySQL-compatible relational database with Paxos replication and HTAP.**

OceanBase Database is a distributed relational database written in C++ and developed by Ant Group. It replicates data across a server cluster with Paxos for high availability, and it is MySQL compatible so existing MySQL applications can migrate. It supports mixed transactional and analytical workloads, and the README lists RPO 0 and RTO under 8 seconds.

- **+** Paxos-based replication with stated RPO = 0 and RTO under 8 seconds
- **+** MySQL compatible, so MySQL applications can migrate
- **+** Stated scale of 1,500 nodes in one cluster
- **+** Deploys via all-in-one installer, Docker image or ob-operator on Kubernetes
- **−** Not an AI app starter: the README mentions no AI or vector features
- **−** All-in-one installer is Linux only and runs a curl script from an OSS bucket
- **−** Docker quick start is a mini standalone instance, not a cluster
- **−** Real multi-node clusters mean operating a large C++ distributed system

<sub>[Repo](https://github.com/oceanbase/oceanbase) · [📖 Docs ↗](https://en.oceanbase.com/docs/oceanbase-database) · [🌐 Site ↗](https://en.oceanbase.com/product/opensource) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oceanbase/)</sub>

<a name="omnigraph"></a>
### #&#8288;73 [omnigraph](https://github.com/modernrelay/omnigraph) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

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

<a name="spring-cloud-alibaba"></a>
### #&#8288;74 [spring-cloud-alibaba](https://github.com/alibaba/spring-cloud-alibaba) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: widely used (80) · Freshness: active (92) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Sep 2026</sub>

**Spring Cloud integrations for Nacos, Sentinel, RocketMQ and Seata.**

Java library set that connects Spring Cloud applications to Alibaba middleware through starters and annotations. It covers service discovery and config (Nacos), flow control and degradation (Sentinel), messaging (RocketMQ), distributed transactions (Seata), and Alibaba Cloud OSS, SMS and SchedulerX. Versioned in step with Spring Boot; the 2025.1.x branch targets Spring Boot 4.0.x and JDK 17+.

- **+** Starters for Nacos, Sentinel, RocketMQ and Seata, imported through one BOM
- **+** Branches map to Spring Boot lines from 1.x to 4.0.x
- **+** Maven and Gradle dependency setup both documented
- **+** Examples module with readmes for Sentinel, Nacos and RocketMQ
- **−** Not an AI project; no model, agent or LLM features in the README
- **−** Needs separately run Nacos, Sentinel, RocketMQ or Seata servers
- **−** Several features depend on paid Alibaba Cloud services (OSS, SMS, SchedulerX)
- **−** Grayscale release and lossless online/offline are only in the enterprise MSE edition

<sub>no GPU · Needs Nacos, Sentinel, RocketMQ, Seata, Alibaba Cloud OSS, Alibaba Cloud SMS, Alibaba Cloud SchedulerX · [Repo](https://github.com/alibaba/spring-cloud-alibaba) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spring-cloud-alibaba/)</sub>

<a name="matrixone"></a>
### #&#8288;75 [matrixone](https://github.com/matrixorigin/matrixone) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

**MySQL-compatible HTAP database with Git-style snapshots and vector search.**

MatrixOne is a Go database that speaks the MySQL protocol and runs transactional, analytical, full-text and vector workloads in one engine. It adds zero-copy snapshots, time travel, branching and rollback for data, plus IVF and HNSW vector indexes for RAG use. A Python SDK covers vector and full-text queries, and storage is separated from compute.

- **+** MySQL protocol compatibility, so existing clients and ORMs connect on port 6001
- **+** Built-in IVF and HNSW vector indexes plus full-text search, no separate vector store
- **+** Snapshots, time travel and rollback for data without full backups
- **+** Python SDK with ORM support for vector and boolean full-text queries
- **−** Building from source needs Go 1.27.1 or later, GCC/Clang and Make
- **−** Full cluster setup has multiple node types, heavier than an embedded database
- **−** Infrastructure component, not an app starter you fork and run

<sub>no GPU · [Repo](https://github.com/matrixorigin/matrixone) · [📖 Docs ↗](https://docs.matrixorigin.cn/en/latest/) · [🌐 Site ↗](https://www.matrixorigin.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/matrixone/)</sub>

<a name="apitable"></a>
### #&#8288;76 [apitable](https://github.com/apitable/apitable) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · AGPL-3.0 · Sep 2026</sub>

**Self-hosted collaborative database-spreadsheet with REST API, forms and automations.**

APITable is a visual database with a spreadsheet-style UI, built on TypeScript (Next.js, NestJS) and Java (Spring Boot). It offers realtime multi-user editing via Operational Transformation, cross-table links, several view types (grid, kanban, gantt, calendar, gallery, mindmap), auto-generated forms, and a REST API. Installs with a docker compose script; SSO, SAML and audit are limited to hosted and enterprise editions.

- **+** Realtime collaboration using Operational Transformation, stated to handle 100k+ rows
- **+** REST API, widget SDK and scripting widget documented in a developer center
- **+** Row and column permissions via mirrors and folder-level access control
- **+** One-line docker compose install plus an all-in-one demo image
- **−** SAML, SSO, audit, backup and watermark are not in the open-source edition
- **−** Recommends 4 CPUs and 8GB RAM; arm64 images are not native and perform badly
- **−** All-in-one image is for demo only, amd64 only, and slow to start
- **−** AGPL-3.0 license; the Datasheet Query Language is listed as a future feature

<sub>RAM ≥ 8 GB · no GPU · Compose · Needs Docker, Docker Compose v2 · port 80 · [Repo](https://github.com/apitable/apitable) · [▶️ Demo ↗](https://gitpod.io/#https://github.com/apitable/apitable) · [📖 Docs ↗](https://developers.aitable.ai/) · [🌐 Site ↗](https://aitable.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apitable/)</sub>

<a name="prest"></a>
### #&#8288;77 [prest](https://github.com/prest/prest) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

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

<a name="kratos"></a>
### #&#8288;78 [kratos](https://github.com/go-kratos/kratos) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: weak (29) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

**Go microservice framework with HTTP/gRPC transport and Protobuf code generation.**

Kratos is a Go framework for building microservices. It provides a unified HTTP and gRPC transport layer, composable middleware (recovery, logging, validation, tracing, metrics, auth), and pluggable registry, config and encoding components. A kratos CLI scaffolds services and generates code from Protobuf definitions. It is a general backend framework, not an AI-specific project.

- **+** One transport abstraction for HTTP and gRPC, with code generated from Protobuf
- **+** CLI scaffolds a runnable service with kratos new and kratos run
- **+** Optional integrations (registries, config stores, observability) live in contrib packages
- **+** Logging uses standard-library log/slog; v3 reduces core dependencies
- **−** No AI, model or agent features; it is a general microservice framework
- **−** Requires Go 1.25+, protoc and protoc-gen-go installed locally
- **−** v3 makes implicit behavior explicit; v2 services need migration first
- **−** No Dockerfile or compose setup in the README

<sub>no GPU · Needs Go 1.25+, protoc, protoc-gen-go · port 8000 · [Repo](https://github.com/go-kratos/kratos) · [📖 Docs ↗](https://go-kratos.dev/docs/getting-started/start) · [🌐 Site ↗](https://go-kratos.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kratos/)</sub>

<a name="vercel"></a>
### #&#8288;79 [vercel](https://github.com/vercel/vercel) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: weak (25) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Oct 2026</sub>

**Source for the Vercel CLI and builders that deploy apps on git push.**

This is the source repository for the Vercel CLI (`vercel` and `vc`) and the builder packages that deploy projects to the hosted Vercel platform. It is a pnpm and Turborepo monorepo written in TypeScript, with an optional native CLI binary published as `@vercel/vc-native`. It is a deployment tool, not an AI app starter, so it fits this list only loosely.

- **+** Deploys from `git push`, the CLI, or the project import flow
- **+** Install with `npm i -g vercel`; optional native binary via `@vercel/vc-native`
- **+** Unit tests run on Vitest; local CLI changes run with `pnpm vercel`
- **+** Apache-2.0 licensed, with a release in July 2026
- **−** Deploys to the proprietary hosted Vercel platform; README describes no self-hosting
- **−** Integration tests need a Vercel account, access token and team ID
- **−** README describes no AI features or starter code
- **−** Contributors are asked to discuss changes on Vercel Community before opening a PR

<sub>no GPU · Needs Vercel account, Node.js, pnpm · [Repo](https://github.com/vercel/vercel) · [📖 Docs ↗](https://vercel.com/docs) · [🌐 Site ↗](https://vercel.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vercel/)</sub>

<a name="memgraph"></a>
### #&#8288;80 [memgraph](https://github.com/memgraph/memgraph) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (34) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · custom license · Nov 2026</sub>

**In-memory graph database with vector search for GraphRAG and analytics.**

Memgraph is an in-memory graph database written in C/C++ that speaks Neo4j-compatible Cypher and is ACID-compliant. Built-in vector, text and geospatial indexes let GraphRAG retrieval run as one Cypher query, and the MAGE library adds 40+ graph algorithms. Data loads from Kafka, Pulsar, RedPanda, CSV, JSON, Parquet and JSONL.

- **+** Vector, text and geospatial indexes combine with graph traversal in a single Cypher query
- **+** Cypher-compatible with Neo4j; drivers for Python, C/C++ and others, plus WebSocket
- **+** MAGE library has 40+ algorithms in C++, Python and CUDA, including PageRank
- **+** Streams from Kafka, Pulsar and RedPanda; loads Parquet and JSONL from disk, S3 or HTTP
- **−** Community edition is under BSL, not an OSI open-source license
- **−** HA, multi-tenancy, SSO and fine-grained access control are Enterprise (MEL) features
- **−** Data is held in memory, so dataset size is bounded by RAM
- **−** A database engine, not a RAG starter; retrieval pipelines must be built on top

<sub>GPU optional · [Repo](https://github.com/memgraph/memgraph) · [▶️ Demo ↗](https://playground.memgraph.com/) · [📖 Docs ↗](https://memgraph.com/docs) · [🌐 Site ↗](https://memgraph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/memgraph/)</sub>

<a name="airbyte"></a>
### #&#8288;81 [airbyte](https://github.com/airbytehq/airbyte) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (73) · Freshness: active (82) · Maintenance: patchy (44) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

**ELT platform with 700+ connectors for moving data into warehouses, lakes and AI agents.**

Airbyte syncs data from APIs, databases and files into warehouses, lakes and AI applications using a catalog of 700+ connectors. Connectors can be built with a no-code Connector Builder or a low-code CDK, and syncs can be orchestrated from Airflow, Dagster, Kestra or the Airbyte API. An Airbyte MCP server lets agents such as Claude and Cursor build pipelines, read logs and run syncs.

- **+** 700+ connectors across APIs, databases, warehouses, lakes and AI applications
- **+** No-code Connector Builder and low-code CDK for custom connectors
- **+** Orchestration integrations for Airflow, Dagster and Kestra, plus a public API
- **+** MCP server for agents to manage pipelines, syncs and logs
- **−** Direct API reads and search (context layer) are Airbyte Cloud only
- **−** Licensing is mixed (MIT and ELv2 badges); license detection reports NOASSERTION
- **−** Additional security features sit in the paid Enterprise edition
- **−** Last tagged release is 2025-10-15, older than recent commits

<sub>no GPU · [Repo](https://github.com/airbytehq/airbyte) · [▶️ Demo ↗](https://demo.airbyte.io/) · [📖 Docs ↗](https://docs.airbyte.com/) · [🌐 Site ↗](https://airbyte.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/airbyte/)</sub>

<a name="gitpod"></a>
### #&#8288;82 [gitpod](https://github.com/gitpod-io/gitpod) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (59) · Freshness: recent (70) · Maintenance: fair (63) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · AGPL-3.0 · Nov 2026</sub>

**Cloud development environments configured per repo with .gitpod.yml.**

Gitpod Classic starts ephemeral, Docker-based Linux workspaces in the cloud from a .gitpod.yml file in the repository. It integrates with GitHub, GitLab, Bitbucket and Azure DevOps, supports prebuilds, and runs VS Code in the browser or editor. The project has been renamed Ona, and the README no longer recommends this version.

- **+** Environments defined per repo in .gitpod.yml, giving reproducible workspaces
- **+** Supports GitHub, GitLab, Bitbucket and Azure DevOps
- **+** Prebuilt environments reduce setup time at workspace start
- **+** Related OpenVSCode Server and workspace images are published separately
- **−** README says this version is no longer recommended; Ona replaces it
- **−** Classic pay-as-you-go was sunset on October 15, 2025
- **−** Last release is June 2023
- **−** Not an AI starter; no model or agent features described

<sub>Needs GitHub, GitLab, Bitbucket or Azure DevOps · [Repo](https://github.com/gitpod-io/gitpod) · [📖 Docs ↗](https://www.gitpod.io/docs) · [🌐 Site ↗](https://www.gitpod.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gitpod/)</sub>

<a name="ubicloud"></a>
### #&#8288;83 [ubicloud](https://github.com/ubicloud/ubicloud) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · AGPL-3.0 · Nov 2026</sub>

**Open-source IaaS control plane for VMs, Postgres and Kubernetes on bare metal.**

Ubicloud is a Ruby control plane (Roda, Sequel, Postgres) that turns leased bare metal servers into a cloud. It provisions Cloud Hypervisor VMs, private subnets, firewalls, managed PostgreSQL, Kubernetes, GitHub Actions runners and AI inference endpoints over SSH. It can be self-hosted via a demo compose setup or used as a managed service.

- **+** Covers VMs, managed Postgres with HA and PITR, Kubernetes, and CI runners in one control plane
- **+** Managed through console, REST API with OpenAPI spec, ubi CLI, or Terraform provider
- **+** All state, including in-flight state machines, lives in a single Postgres database
- **+** Postgres also runs on AWS and GCP, not only bare metal
- **−** Self-host cloudify script currently supports only Hetzner bare metal servers
- **−** Self-hosting needs leased bare metal plus Hetzner credentials, SSH keys and Ubuntu 24.04
- **−** AGPL-3.0 license may restrict use in some commercial setups
- **−** Service catalog is small compared with public clouds; README states 10% of services as the goal

<sub>Docker · Needs PostgreSQL, Docker, Bare metal servers (Hetzner, Leaseweb, AWS Bare Metal), Ubuntu 24.04 on data plane hosts · port 3000 · [Repo](https://github.com/ubicloud/ubicloud) · [📖 Docs ↗](https://www.ubicloud.com/docs/architecture/attribute-based-access-control-abac) · [🌐 Site ↗](https://console.ubicloud.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ubicloud/)</sub>

<a name="ihp"></a>
### #&#8288;84 [ihp](https://github.com/digitallyinduced/ihp) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Nov 2026</sub>

**Haskell web framework with type-safe routing, queries and HTML templates.**

IHP is a full-stack Haskell web framework built on Nix, with type-safe routing, database queries and JSX-like HSX templates. It includes a visual schema designer, code generators, live reload, auth, and real-time views over PostgreSQL. It ships a CLAUDE.md so AI coding tools follow framework conventions, with the compiler checking generated code.

- **+** Compile-time checks on routes, queries and HTML catch errors in AI-generated code
- **+** Built-in schema designer, code generators, auth, forms and migrations
- **+** Declarative NixOS deploy via deploy-to-nixos, with socket-activated restarts
- **+** Ships CLAUDE.md describing framework conventions for AI tools
- **−** Requires Haskell and Nix, a narrow skill set for most teams
- **−** Deployment tooling centers on NixOS servers; Docker is secondary
- **−** AI support is limited to a CLAUDE.md and an OpenAI package
- **−** No billing or SaaS scaffolding mentioned in the README

<sub>no GPU · Needs Nix, devenv, PostgreSQL, GHC · Models: OpenAI (via ihp-openai) · [Repo](https://github.com/digitallyinduced/ihp) · [📖 Docs ↗](https://ihp.digitallyinduced.com/Guide/) · [🌐 Site ↗](https://ihp.digitallyinduced.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ihp/)</sub>

<a name="couchdb"></a>
### #&#8288;85 [couchdb](https://github.com/apache/couchdb) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · Apache-2.0 · Nov 2026</sub>

**Document database with an HTTP API, Fauxton admin UI and clustering.**

Apache CouchDB is a database written in Erlang, accessed over HTTP, and it ships with the Fauxton admin UI. The README covers installation on Unix-like systems and Windows, a dev cluster started with ./dev/run (three nodes, port 5984, optional haproxy) and a devcontainer for contributors. It describes no AI features.

- **+** ./dev/run starts a local three-node cluster listening on port 5984
- **+** Built-in Fauxton web UI and an install check at /_utils/#verifyinstall
- **+** Apache-2.0 licensed, with hosted docs, a changelog and mailing-list support
- **+** Devcontainer runs configure and make on first creation
- **−** README has no feature overview, API examples or data model description
- **−** No AI, vector search or LLM integration is described
- **−** No Docker or compose files detected in the repo
- **−** No tagged release listed; install is from source or per-OS guides

<sub>no GPU · Needs Erlang, haproxy (optional, dev cluster) · port 5984 · [Repo](https://github.com/apache/couchdb) · [📖 Docs ↗](https://docs.couchdb.org/) · [🌐 Site ↗](https://couchdb.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/couchdb/)</sub>

<a name="nitric"></a>
### #&#8288;86 [nitric](https://github.com/nitrictech/nitric) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="apollo-server"></a>
### #&#8288;87 [apollo-server](https://github.com/apollographql/apollo-server) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (60) · Freshness: active (99) · Maintenance: weak (27) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**TypeScript GraphQL server library for Node.js, standalone or federated.**

@apollo/server is a spec-compliant GraphQL server for Node.js, installed from npm alongside graphql. It ships a standalone HTTP server that handles CORS and body parsing, and can also run as a subgraph or gateway in an Apollo Federation supergraph. Express and other framework integrations are separate packages, community-maintained.

- **+** Standalone server works with two npm packages and about 20 lines of code
- **+** Runs as a plain server, a federated subgraph, or a federation gateway
- **+** Works with any GraphQL client and any data source
- **+** Serves Apollo Sandbox in the browser for trying queries
- **−** Library only: no database, auth or storage included
- **−** Framework integrations such as Express are community-maintained, not in the core package
- **−** Standalone server offers no fine-grained control over HTTP behavior
- **−** Most features are documented only on the external docs site

<sub>no GPU · Needs Node.js, graphql · port 4000 · [Repo](https://github.com/apollographql/apollo-server) · [📖 Docs ↗](https://www.apollographql.com/docs/apollo-server/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apollo-server/)</sub>

<a name="fusio"></a>
### #&#8288;88 [fusio](https://github.com/apioo/fusio) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Oct 2026</sub>

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

<a name="serverpod"></a>
### #&#8288;89 [serverpod](https://github.com/serverpod/serverpod) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · BSD-3-Clause · Nov 2026</sub>

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

<a name="agensgraph"></a>
### #&#8288;90 [agensgraph](https://github.com/skaiworldwide-oss/agensgraph) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Oct 2026</sub>

**PostgreSQL fork with a built-in property graph queried via SQL, openCypher and GQL.**

AgensGraph is a fork of PostgreSQL, not an extension, that stores graphs and relational tables in one database and commits them in one transaction. A graph is a schema, a label is a table, and vertices and edges are rows. Queries can mix SQL, openCypher and ISO GQL in a single statement, and an AI section lists MCP servers and LangChain, LlamaIndex, LightRAG and cognee integrations.

- **+** Graph and relational data share one transaction, so joins between Cypher results and tables work in SQL
- **+** Keeps PostgreSQL tooling: pg_dump, pg_upgrade, row-level security, streaming and logical replication
- **+** Works with pgvector for vector, full-text or hybrid search followed by graph traversal
- **+** Variable-length paths plus shortestpath(), allshortestpaths() and dijkstra() built in
- **−** Fork of PostgreSQL, so it cannot be added to an existing stock PostgreSQL server as an extension
- **−** Only a Python driver adds graph types; other languages use plain PostgreSQL drivers
- **−** Upgrading from 2.17 requires following a dedicated upgrade procedure to 2.18
- **−** AI integrations ship as separate Python packages, with no non-Python equivalents listed

<sub>no GPU · Models: pgvector embeddings, MCP clients, LangChain, LlamaIndex, LightRAG · [Repo](https://github.com/skaiworldwide-oss/agensgraph) · [📖 Docs ↗](https://tech.skaiworldwide.com/docs/en/agensgraph/18/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agensgraph/)</sub>

<a name="boilerplates"></a>
### #&#8288;91 [boilerplates](https://github.com/christianlempa/boilerplates) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (45) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · MIT · Aug 2026</sub>

**CLI that renders Docker Compose, Terraform and Ansible templates from git libraries.**

Boilerplates is a Python CLI that renders reusable infrastructure templates (Compose, Kubernetes, Terraform, Ansible, static files, Python, Bash) into concrete files. Templates use Jinja2-like `<< >>` delimiters and a `template.json` manifest, with variables set through an interactive wizard, CLI overrides or saved defaults. Template libraries are git repositories, and a separate library offers 100+ homelab presets. It contains no AI features.

- **+** Interactive prompts and non-interactive `--var` overrides cover both manual and scripted generation
- **+** Git-backed libraries can be added, updated and removed with `boilerplates repo` commands
- **+** Per-kind subcommands (compose, static) list, show and generate templates with one syntax
- **+** Installs via pipx script or Nix flake
- **−** Not an AI project; it is a general infrastructure templating tool
- **−** 0.2.0 dropped `template.yaml` and `.j2` formats, so older templates need migration
- **−** Python and Bash kinds only validate syntax, variables and rendering, not compilation or tests
- **−** Ships no Docker image or compose file for the tool itself

<sub>Needs pipx, git · [Repo](https://github.com/christianlempa/boilerplates) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/boilerplates/)</sub>

<a name="butterbase"></a>
### #&#8288;92 [butterbase](https://github.com/butterbase-ai/butterbase) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="nixopus"></a>
### #&#8288;93 [nixopus](https://github.com/nixopus/nixopus) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Sep 2026</sub>

**Self-hosted deployment platform with an AI agent that builds and ships repos.**

Nixopus deploys apps from a connected GitHub repo onto your own servers. An LLM agent, reachable from a web dashboard or a VS Code/Cursor extension, analyzes the codebase, generates build config, deploys, and manages domains, logs and rollbacks. Caddy handles TLS, and a single curl installer sets up Docker if it is missing.

- **+** Agent generates build config and deploys from chat, in the dashboard or the editor extension
- **+** Six LLM providers supported: OpenRouter, OpenAI, Anthropic, Google, DeepSeek and Groq
- **+** Caddy gives automatic Let's Encrypt TLS, custom domains, and rollbacks from retained images
- **+** Runs on a 1 GB VPS, amd64 or arm64, with a one-line installer
- **−** Automatic failure diagnosis and fix PRs are marked as in development
- **−** Multi-machine deployments, load balancing and autoscaling are only on the roadmap
- **−** Needs a fresh dedicated VPS; installer must run as root
- **−** AGPL-3.0 with a separate commercial license for enterprises

<sub>RAM ≥ 1 GB · no GPU · Compose · Needs Docker Engine, Docker Compose V2, Caddy, LLM provider API key, GitHub · Models: OpenRouter, OpenAI, Anthropic, Google, DeepSeek · port 80 · [Repo](https://github.com/nixopus/nixopus) · [▶️ Demo ↗](https://dashboard.nixopus.com) · [📖 Docs ↗](https://docs.nixopus.com) · [🌐 Site ↗](https://nixopus.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nixopus/)</sub>

<a name="classic-jazz"></a>
### #&#8288;94 [classic-jazz](https://github.com/garden-co/classic-jazz) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

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

<a name="matecloud"></a>
### #&#8288;95 [matecloud](https://github.com/mateaix/matecloud) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;96 [steedos-platform](https://github.com/steedos/steedos-platform) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (8) · Freshness: active (92) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · AGPL-3.0 · Nov 2026</sub>

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

<a name="amplication"></a>
### #&#8288;97 [amplication](https://github.com/amplication/amplication) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: popular (65) · Freshness: recent (63) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · custom license · Apr 2026</sub>

**Generates NestJS and Node.js backend services from data models, with team templates.**

Amplication generates backend microservices (APIs, data models, DTOs) from a modeled domain, and pushes the code to your Git repository. Organizations can define their own live templates and plugins so generated services follow shared standards, and the tool handles package updates and versioning. It can be used hosted at app.amplication.com or run locally as an Nx monorepo for development.

- **+** Generates editable service code (APIs, data models, DTOs) that you own and commit to Git
- **+** Plugin system and custom live templates enforce shared standards across services
- **+** Handles package updates, patches and versioning of generated services
- **+** Hosted version available, so no local setup is needed to try it
- **−** Components under the ee directory use a separate Enterprise Edition license
- **−** Self-hosting is documented only as a development setup, not a production deployment guide
- **−** Local setup needs Node.js, Docker and several services run via npm scripts

<sub>no GPU · Compose · Needs Node.js, Docker, Git · [Repo](https://github.com/amplication/amplication) · [▶️ Demo ↗](https://app.amplication.com) · [📖 Docs ↗](https://docs.amplication.com) · [🌐 Site ↗](https://amplication.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/amplication/)</sub>

<a name="openwhisk"></a>
### #&#8288;98 [openwhisk](https://github.com/apache/openwhisk) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: known (40) · Freshness: recent (70) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · Apache-2.0 · Nov 2026</sub>

**Serverless functions platform with triggers, rules and action composition.**

Apache OpenWhisk runs functions as serverless actions, exposes them as APIs, and wires events to them through triggers and rules. Each function runs in its own Docker container. It runs as a single Java process (Standalone mode) for local use, or on Kubernetes through the separate openwhisk-deploy-kube repo. It has no AI-specific features.

- **+** Standalone mode starts the full stack with one Gradle command and opens a browser Playground
- **+** Deploys on managed Kubernetes (AKS, EKS, IKS, GKE), Minikube or Docker for Mac
- **+** Supports triggers, rules, packages and feeds for event-driven wiring, plus function composition
- **+** Documented process for adding a runtime for a new language
- **−** Master moved to Apache Pekko in Oct 2025; upgrading requires new clusters and traffic cutover
- **−** Latest tagged release is April 2024; a 3.x branch for the Pekko change is still pending
- **−** Needs Docker, Java and Node.js locally; Kubernetes deploy lives in a separate repo
- **−** Generic serverless platform with no LLM, agent or model-serving tooling

<sub>Needs Docker, Java, Node.js, Kubernetes (optional) · port 3232 · [Repo](https://github.com/apache/openwhisk) · [🌐 Site ↗](http://openwhisk.apache.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openwhisk/)</sub>

<a name="vearch"></a>
### #&#8288;99 [vearch](https://github.com/vearch/vearch) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (18) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · Apache-2.0 · Jul 2026</sub>

**Distributed vector database with hybrid vector and scalar-filter search.**

Vearch is a distributed vector database for similarity search over embeddings. A Router exposes a REST API (upsert, delete, search, query), a Master manages schema and cluster metadata, and PartitionServers run the Gamma engine, built on faiss, with raft replication. It ships SDKs for Python, Go, Java and Rust, plus integrations for LangChain and LlamaIndex.

- **+** Combines vector search with scalar filtering in one query
- **+** Raft-based replication and scale-out across Master, Router and PartitionServer roles
- **+** SDKs for Python, Go, Java and Rust, plus LangChain and LlamaIndex integrations
- **+** Helm chart and Docker Compose profiles for standalone and cluster modes
- **−** Cluster mode needs several components, which is heavier than an embedded vector store
- **−** README gives no benchmarks beyond a 'millions of objects in milliseconds' claim
- **−** Visual search demo needs a separate image retrieval plugin

<sub>[Repo](https://github.com/vearch/vearch) · [📖 Docs ↗](https://vearch.readthedocs.io/en/latest) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vearch/)</sub>

<a name="graphql"></a>
### #&#8288;100 [graphql](https://github.com/redwoodjs/graphql) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: popular (69) · Freshness: quiet (21) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Dec 2025</sub>

**Full-stack React framework with GraphQL API and Prisma, now succeeded by RedwoodSDK.**

RedwoodJS is an opinionated TypeScript web framework: a React frontend (Vite) talks to a GraphQL API (GraphQL Yoga, Envelop) that uses Prisma for the database. Jest, Storybook and Pino logging are included, and auth and CSS frameworks are added by CLI command. The README redirects new work to RedwoodSDK, a Cloudflare-focused framework, and lists the Bighorn epoch (React Server Components) as unreleased.

- **+** Integrated stack: React, Vite, GraphQL Yoga, Prisma, Jest, Storybook and Pino
- **+** Deploys to serverless hosts (Netlify, Vercel) or servers and containers (AWS, Render)
- **+** Auth providers such as Auth0 and Tailwind CSS are each added with one command
- **+** TypeScript throughout, with JavaScript also supported
- **−** No AI features; it is a general web framework, not an AI starter
- **−** README points new development to RedwoodSDK, so this repo is the older line
- **−** Bighorn epoch with React Server Components has no production release
- **−** Opinionated stack with GraphQL and Prisma; swapping parts is not described

<sub>no GPU · Needs Node.js, Prisma-supported database · [Repo](https://github.com/redwoodjs/graphql) · [📖 Docs ↗](https://redwoodjs.com/docs/introduction) · [🌐 Site ↗](https://redwoodjs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphql/)</sub>

<a name="1backend"></a>
### #&#8288;101 [1backend](https://github.com/1backend/1backend) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (19) · Freshness: recent (62) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · May 2026</sub>

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
### #&#8288;102 [go-backend-clean-architecture](https://github.com/amitshekhariitbhu/go-backend-clean-architecture) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: known (38) · Freshness: slowing (31) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Feb 2026</sub>

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
