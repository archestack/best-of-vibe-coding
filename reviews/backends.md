# 🗄️ Backends, databases and hosting reviews · Best of Vibe Coding

Open-source backends you ship apps on (auth, database, storage, APIs) and self-hosted platforms that deploy them from Git or Docker. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-databases-and-hosting).

<sub>🌐 Also on the web: [Backends, databases and hosting on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="bun"></a>
### 🥇 [oven-sh/bun](https://github.com/oven-sh/bun) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 97k · custom license · Nov 2026</sub>

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

<a name="filament"></a>
### 🥈 [filament](https://github.com/filamentphp/filament) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**Laravel framework for admin panels, CRMs and internal business apps.**

Filament is a PHP framework built on Laravel and Livewire for building admin panels, customer portals and internal tools. It provides tables, forms, infolists, notifications, dashboard widgets and actions that share conventions, so CRUD screens need little custom code. It contains no AI features; it fits the list only as a base for app front ends.

- **+** Tables with search, filters, and bulk actions, plus reactive forms, in one component set
- **+** MIT license, with a live demo and public docs
- **+** Actively maintained: last release 2026-11-15, last commit 2026-11-19
- **+** Builds on Laravel and Livewire, so no separate JavaScript front end is needed
- **−** Tied to Laravel 11+, Livewire, and PHP 8.2+; unusable outside that stack
- **−** No built-in AI, LLM, or agent features
- **−** No Docker or compose files in the repo
- **−** Not a standalone backend; it is a UI layer over your Laravel app

<sub>no GPU · Needs PHP 8.2+, Laravel 11+, Livewire 3 · [Repo](https://github.com/filamentphp/filament) · [▶️ Demo ↗](https://demo.filamentphp.com) · [📖 Docs ↗](https://filamentphp.com/docs) · [🌐 Site ↗](https://filamentphp.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/filament/)</sub>

<a name="coolify"></a>
### 🥉 [coolify](https://github.com/coollabsio/coolify) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · Apache-2.0 · Nov 2026</sub>

**Self-hosted Heroku and Vercel alternative that deploys apps and databases over SSH.**

Coolify manages servers reached over SSH and deploys applications from GitHub, GitLab, Bitbucket or Gitea using Nixpacks, Railpack, Dockerfile, Docker Compose or prebuilt images. It also runs databases and more than 360 one-click services, with automatic HTTPS, backups, pull-request previews and rollbacks. Control is through a dashboard, API, CLI or MCP.

- **+** Needs only SSH access to a target server; VPS, bare metal or Raspberry Pi work
- **+** Builds from Nixpacks, Railpack, Dockerfile, Compose or prebuilt images
- **+** More than 360 one-click services plus managed databases with backups
- **+** Running resources keep working if Coolify is removed
- **−** Recommended setup uses a separate server for Coolify itself
- **−** Install is a curl-to-bash script, so review it before running
- **−** High availability and email notifications are tied to the paid Cloud service
- **−** General deployment platform with no AI-specific features

<sub>no GPU · Docker + Compose · Needs SSH-accessible server · README: alternative to Vercel, Heroku · [Repo](https://github.com/coollabsio/coolify) · [📖 Docs ↗](https://coolify.io/docs) · [🌐 Site ↗](https://coolify.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/coolify/)</sub>

<a name="traefik"></a>
### #&#8288;4 [traefik](https://github.com/traefik/traefik) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · MIT · Nov 2026</sub>

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
### #&#8288;5 [appwrite](https://github.com/appwrite/appwrite) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · BSD-3-Clause · Nov 2026</sub>

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
### #&#8288;6 [medusa](https://github.com/medusajs/medusa) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · custom license · Nov 2026</sub>

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

<a name="strapi"></a>
### #&#8288;7 [strapi](https://github.com/strapi/strapi) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 74k · custom license · Nov 2026</sub>

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

<a name="tidb"></a>
### #&#8288;8 [tidb](https://github.com/pingcap/tidb) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · Apache-2.0 · Nov 2026</sub>

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
### #&#8288;9 [compose](https://github.com/docker/compose) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · Apache-2.0 · Nov 2026</sub>

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

<a name="remix"></a>
### #&#8288;10 [remix](https://github.com/remix-run/remix) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**Web framework built from composable Fetch API packages for any JS runtime.**

Remix 3 is a monorepo of single-purpose TypeScript packages (fetch-router, component runtime, data-table, sessions, auth, middleware, test runner) distributed together as one `remix` package. Packages build on Web APIs and run on Node.js, Bun, Deno and Cloudflare Workers without a bundler. New apps are scaffolded with `npx remix new`, and the repo ships an agent skill for building apps. It is under active development.

- **+** Packages are usable standalone and target Web APIs, so they run on Node, Bun, Deno and Workers
- **+** Runtime-first design: tests run without bundling, TypeScript/JSX via --import loaders
- **+** Covers router, middleware, sessions, auth, data-table (MySQL, Postgres, SQLite) and S3 file storage
- **+** MIT licensed, with a commit and a release in the past two weeks
- **−** README says it is under active development, so APIs may change
- **−** General web framework; AI use is a stated principle, with no listed model package
- **−** Not a ready-made app: you assemble routes, data and UI yourself
- **−** Preview builds are tarball URLs that expire, which complicates pinning

<sub>no GPU · Needs Node.js, Bun, Deno or Cloudflare Workers, Optional: MySQL, PostgreSQL, SQLite, S3, Redis, Memcache · [Repo](https://github.com/remix-run/remix) · [🌐 Site ↗](https://remix.run) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/remix/)</sub>

<a name="dragonfly"></a>
### #&#8288;11 [dragonfly](https://github.com/dragonflydb/dragonfly) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · custom license · Nov 2026</sub>

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
### #&#8288;12 [kestra](https://github.com/kestra-io/kestra) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · Apache-2.0 · Nov 2026</sub>

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

<a name="scalar"></a>
### #&#8288;13 [scalar](https://github.com/scalar/scalar) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

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

<a name="meteor"></a>
### #&#8288;14 [meteor](https://github.com/meteor/meteor) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 45k · custom license · Nov 2026</sub>

**Full-stack JavaScript framework for web, mobile and desktop apps.**

Meteor is a JavaScript application platform with a CLI (`meteor create`, `meteor`) for building web apps. The same code can target iOS, Android and desktop. It has tutorials for React, Blaze, Vue, Svelte and Solid, and requires Node 22 or newer. It is a general web framework, not an AI project; the README only mentions Meteor Agent Skills for AI coding assistants.

- **+** Tutorials for five front ends: React, Blaze, Vue, Svelte and Solid
- **+** One codebase can target web, iOS, Android and desktop
- **+** Active project: commit and release within the last week
- **+** Atmosphere package registry and official Agent Skills docs for AI assistants
- **−** No built-in AI features, models or LLM integrations described
- **−** License is reported as NOASSERTION, so terms need checking in the repo
- **−** Deployment path promoted in the README is Galaxy, a commercial service
- **−** Full framework with its own CLI and build, not a small starter to fork

<sub>no GPU · Needs Node.js >=22 · [Repo](https://github.com/meteor/meteor) · [📖 Docs ↗](https://docs.meteor.com/#/full/) · [🌐 Site ↗](https://www.meteor.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/meteor/)</sub>

<a name="duckdb"></a>
### #&#8288;15 [duckdb](https://github.com/duckdb/duckdb) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 43k · MIT · Nov 2026</sub>

**In-process analytical SQL database that queries CSV, Parquet and JSON files directly.**

DuckDB is an embedded analytical database written in C++ that runs inside the host application, with no separate server. It reads and writes CSV, Parquet, JSON and Excel from local disk or S3, HTTP, Azure and GCS, and can attach PostgreSQL, MySQL and SQLite databases. It ships as a CLI and as clients for Python, R, Java, Rust, Go and Wasm. It is not an AI project; it fits this list only as a data backend.

- **+** Runs in-process with no server and no external dependencies
- **+** Queries files by name in FROM, e.g. SELECT * FROM 'myfile.parquet'
- **+** Attaches PostgreSQL, MySQL and SQLite and queries them in place
- **+** Extension system for formats, connectors and functions; clients for many languages
- **−** No AI, LLM or vector features described in the README
- **−** Built for analytics (OLAP), not as a general multi-user application backend
- **−** No auth, storage API or hosting layer; embedding or the quack protocol is the access path
- **−** Building from source needs CMake, Python 3 and a C++17 compiler

<sub>[Repo](https://github.com/duckdb/duckdb) · [📖 Docs ↗](https://duckdb.org/docs/current/) · [🌐 Site ↗](https://duckdb.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/duckdb/)</sub>

<a name="nacos"></a>
### #&#8288;16 [nacos](https://github.com/alibaba/nacos) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Nov 2026</sub>

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

<a name="nocobase"></a>
### #&#8288;17 [nocobase](https://github.com/nocobase/nocobase) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Nov 2026</sub>

**Open-source application foundation for business systems built by coding agents.**

NocoBase is a TypeScript framework that supplies the shared building blocks of business apps, such as permissions, workflows and files, so coding agents only write business-specific logic. It installs through an agent Skill or `pnpm create @nocobase/app`, and the quick start runs on SQLite. The wider ecosystem also lists NocoBase Studio, which coordinates Claude Code, Codex and OpenCode, and prebuilt Solutions.

- **+** Permissions, workflows and files ship ready, so agents do not rebuild them per project
- **+** Quick start uses SQLite, so no separate database server is needed
- **+** Install through an agent Skill (nocobase-create-app) or a pnpm create command
- **−** Quick start installs the beta tag (@beta), not a stable release
- **−** Requires Node.js 24+ and pnpm 11; Windows users must use WSL
- **−** No Docker or compose files detected in the repository

<sub>no GPU · Needs Node.js 24+, pnpm 11 · Models: Claude Code, Codex, OpenCode · [Repo](https://github.com/nocobase/nocobase) · [📖 Docs ↗](https://docs.nocobase.com/) · [🌐 Site ↗](https://www.nocobase.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nocobase/)</sub>

<a name="nuxt"></a>
### #&#8288;18 [nuxt](https://github.com/nuxt/nuxt) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 61k · MIT · Nov 2026</sub>

**Vue framework for full-stack web apps with SSR, static and hybrid rendering.**

Nuxt is a TypeScript framework on top of Vue.js for building full-stack web applications and sites. It handles file-based routing, auto-imports, data fetching, and server-side, static, hybrid or edge rendering, with a server/ directory for backend routes. It has no built-in AI features, so it fits this list only as a general web app foundation.

- **+** Supports SSR, static generation, hybrid and edge rendering in one framework
- **+** server/ directory adds backend routes without a separate service
- **+** 300+ modules listed for extending projects
- **+** TypeScript works with zero configuration; components and composables auto-import
- **−** No AI, LLM or chat functionality included; you wire in providers yourself
- **−** No bundled auth, billing or database; these come from modules or your own code
- **−** Vue only; teams on React need a different framework
- **−** Not a ready-made starter app, only a scaffold via npm create nuxt

<sub>Needs npm · [Repo](https://github.com/nuxt/nuxt) · [📖 Docs ↗](https://nuxt.com/docs) · [🌐 Site ↗](https://nuxt.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nuxt/)</sub>

<a name="better-auth"></a>
### #&#8288;19 [better-auth](https://github.com/better-auth/better-auth) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

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

<a name="spacetimedb"></a>
### #&#8288;20 [spacetimedb](https://github.com/clockworklabs/spacetimedb) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · custom license · Nov 2026</sub>

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

<a name="coder"></a>
### #&#8288;21 [coder](https://github.com/coder/coder) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · AGPL-3.0 · Nov 2026</sub>

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

<a name="ktor"></a>
### #&#8288;22 [ktor](https://github.com/ktorio/ktor) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**Kotlin coroutine-based framework for web servers and microservices.**

Ktor is a JetBrains framework for building microservices and web applications in Kotlin, using coroutines for asynchronous I/O. Features are installed through a unified interception pipeline and configured with a Kotlin DSL. Applications run on Netty, Jetty, or in Servlet 3.0+ containers such as Tomcat. It is a general web framework with no AI-specific functionality.

- **+** Coroutine-based async I/O across all host engines
- **+** Runs on Netty, Jetty, or Servlet 3.0+ containers
- **+** Test environment emulates a server without real networking
- **+** Unopinionated: logging, persistence, serialization, DI are your choice
- **−** No built-in AI, LLM, or agent features
- **−** Kotlin/JVM only, so a Gradle or Maven project is required
- **−** Unopinionated design means you assemble persistence and logging yourself
- **−** Framework library, not a starter template with ready-made app structure

<sub>no GPU · Needs Kotlin, Gradle or Maven, Netty, Jetty, or a servlet container · port 8080 · [Repo](https://github.com/ktorio/ktor) · [📖 Docs ↗](https://ktor.io/docs/gradle.html) · [🌐 Site ↗](https://ktor.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ktor/)</sub>

<a name="nest"></a>
### #&#8288;23 [nest](https://github.com/nestjs/nest) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 77k · MIT · Nov 2026</sub>

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

<a name="directus"></a>
### #&#8288;24 [directus](https://github.com/directus/directus) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · custom license · Nov 2026</sub>

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

<a name="turborepo"></a>
### #&#8288;25 [turborepo](https://github.com/vercel/turborepo) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

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

<a name="turso"></a>
### #&#8288;26 [turso](https://github.com/tursodatabase/turso) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Nov 2026</sub>

**In-process SQLite-compatible database in Rust with experimental Postgres frontend.**

Turso Database is a Rust rewrite of SQLite that runs in-process and compiles SQL to VDBE bytecode. It reads existing SQLite files, tracks SQLite 3.50.4, and adds BEGIN CONCURRENT (MVCC), change data capture, vector search and io_uring async I/O on Linux. Bindings cover Rust, JavaScript, Python, Go, Java, .NET and WebAssembly, and the CLI can run as an MCP server.

- **+** Opens existing SQLite files and keeps the SQLite C API and SQL dialect
- **+** Official bindings for Rust, JS, Python, Go, Java, .NET and WebAssembly
- **+** BEGIN CONCURRENT with MVCC for higher write throughput than single-writer SQLite
- **+** Built-in MCP server mode with nine tools via tursodb --mcp
- **−** Not yet 1.0; README advises keeping independent backups
- **−** Not fully SQLite compatible yet; gaps are tracked in COMPAT.md
- **−** Postgres frontend, encryption, full-text search and DBSP views are experimental
- **−** Approximate vector indexing is only on the roadmap; vector search is exact

<sub>no GPU · Docker · [Repo](https://github.com/tursodatabase/turso) · [🌐 Site ↗](https://turso.tech) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/turso/)</sub>

<a name="spring-boot"></a>
### #&#8288;27 [spring-boot](https://github.com/spring-projects/spring-boot) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 82k · Apache-2.0 · Nov 2026</sub>

**Java framework for building stand-alone Spring applications with embedded servers.**

Spring Boot is an opinionated layer over the Spring platform for building Java services that start with `java -jar` or deploy as WARs. It supplies embedded servers, security, metrics, health checks and externalized configuration, with no code generation and no XML configuration required. The README does not mention AI features, so it fits this list only as a general backend framework.

- **+** Runs as a stand-alone JAR with embedded server, or as a traditional WAR
- **+** Ships production features: metrics, health checks, security, externalized configuration
- **+** No code generation and no XML configuration required
- **+** Reference docs, how-to guides and a first-application tutorial are published
- **−** No AI, model or agent features described in the README
- **−** Not a hosted backend: no bundled database, auth service or storage
- **−** Building from source requires JDK 25 and the Gradle wrapper
- **−** Java-centric; the README documents no other language support

<sub>Needs JDK 25 (building from source), Gradle wrapper (building from source) · [Repo](https://github.com/spring-projects/spring-boot) · [📖 Docs ↗](https://docs.spring.io/spring-boot) · [🌐 Site ↗](https://spring.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spring-boot/)</sub>

<a name="orm"></a>
### #&#8288;28 [orm](https://github.com/prisma/orm) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · Apache-2.0 · Nov 2026</sub>

**TypeScript ORM for PostgreSQL and MongoDB with a plugin SPI and agent skills.**

Prisma 8 is a TypeScript rewrite of Prisma ORM that targets PostgreSQL and MongoDB. It uses a minimal core with a public extension SPI, and ships pgvector, PostGIS and other extensions built on it. The installers scaffold a contract and db.ts, and add SKILL.md files for Claude Code, Cursor, Copilot and Devin. It is currently a release candidate.

- **+** Scaffolds Next.js, Hono, Nuxt, Astro, NestJS, SvelteKit, TanStack Start or Elysia apps via npm create prisma
- **+** Public extension SPI; pgvector, PostGIS, ParadeDB and Supabase extensions already published
- **+** Installs per-workflow agent skills for Claude Code, Cursor, Copilot and Devin
- **+** Adds to an existing project with npx prisma orm init without touching framework setup
- **−** Prisma 8 is a release candidate; breaking changes possible until 8.0.0 final
- **−** SQLite is only a proof of concept; MySQL is not supported yet
- **−** Requires Node.js 24 or newer
- **−** Some features are missing, listed in the scorecard, so Prisma 7 migration may hit gaps

<sub>no GPU · Compose · Needs Node.js 24+, PostgreSQL or MongoDB · [Repo](https://github.com/prisma/orm) · [📖 Docs ↗](https://www.prisma.io/docs/orm) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orm/)</sub>

<a name="novu"></a>
### #&#8288;29 [novu](https://github.com/novuhq/novu) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · custom license · Nov 2026</sub>

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

<a name="dokploy"></a>
### #&#8288;30 [dokploy](https://github.com/dokploy/dokploy) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · custom license · Nov 2026</sub>

**Self-hosted PaaS for deploying apps and databases to your own servers.**

Dokploy is a self-hostable platform-as-a-service that deploys applications, Docker Compose stacks and databases (MySQL, PostgreSQL, MongoDB, MariaDB, libsql, Redis) to your own VPS. It routes traffic through Traefik, can scale across nodes with Docker Swarm, and manages remote servers. It also offers 600+ one-click templates, database backups to external storage, and a CLI and API.

- **+** Supports apps, Docker Compose and six database types in one panel
- **+** Multi-node scaling via Docker Swarm and deployment to remote servers
- **+** 600+ one-click templates and automated database backups to external storage
- **+** Ships logs and metrics to Grafana, Datadog, Splunk, CloudWatch and others
- **−** License is reported as NOASSERTION; terms need checking before commercial use
- **−** Tied to Docker, Swarm and Traefik; no Kubernetes support mentioned
- **−** Installed by piping a remote script to bash on the server

<sub>no GPU · Docker · Needs Docker, Docker Swarm, Traefik · [Repo](https://github.com/dokploy/dokploy) · [▶️ Demo ↗](https://app.dokploy.com) · [📖 Docs ↗](https://docs.dokploy.com) · [🌐 Site ↗](https://dokploy.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokploy/)</sub>

<a name="surrealdb"></a>
### #&#8288;31 [surrealdb](https://github.com/surrealdb/surrealdb) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · custom license · Nov 2026</sub>

**Multi-model database in one Rust binary with built-in auth and live queries.**

SurrealDB is a database written in Rust that stores document, graph, relational, time-series, geospatial and key-value data and queries it with SurrealQL. It adds full-text, vector and hybrid search, live queries, row-level permissions and end-user auth, so it can also serve as an app backend. It runs embedded, in the browser via WebAssembly, as a single server node, or as a distributed cluster.

- **+** One engine covers document, graph, relational, geospatial and vector data, with multi-table ACID transactions
- **+** Runs embedded, in-browser via WASM, single node or distributed from the same binary
- **+** Row-level permissions and end-user auth let clients query the database directly
- **+** SDKs for Rust, JavaScript, Python, Go, .NET, PHP and Java; includes an MCP server
- **−** BSL 1.1 license, not an OSI-approved open-source license
- **−** SurrealQL is a new query language to learn, though other dialects are offered over wire protocols
- **−** Hosted SurrealDB Cloud is promoted alongside self-hosting in the README
- **−** No compose file detected in the repo; Docker is documented only as a single docker run

<sub>no GPU · Docker · port 8000 · [Repo](https://github.com/surrealdb/surrealdb) · [📖 Docs ↗](https://surrealdb.com/docs) · [🌐 Site ↗](https://surrealdb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/surrealdb/)</sub>

<a name="rails"></a>
### #&#8288;32 [rails](https://github.com/rails/rails) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Nov 2026</sub>

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

<a name="seaweedfs"></a>
### #&#8288;33 [seaweedfs](https://github.com/seaweedfs/seaweedfs) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Nov 2026</sub>

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

<a name="saleor"></a>
### #&#8288;34 [saleor](https://github.com/saleor/saleor) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · BSD-3-Clause · Nov 2026</sub>

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

<a name="node-mongodb-native"></a>
### #&#8288;35 [node-mongodb-native](https://github.com/mongodb/node-mongodb-native) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · Apache-2.0 · Nov 2026</sub>

**Official MongoDB driver for Node.js with TypeScript types.**

The official MongoDB client library for Node.js, installed with `npm install mongodb`. It provides MongoClient, CRUD operations, indexing and a typed error hierarchy, and supports MongoDB servers 4.4+. Optional add-on packages cover zstd and snappy compression, field-level and queryable encryption, and Kerberos and AWS authentication.

- **+** Maintained by MongoDB; releases are GPG-signed and carry npm provenance attestations
- **+** Ships TypeScript types, checked against typescript 5.6.0 and later
- **+** Semantic versioning with a documented error class tree safe for instanceof checks
- **+** Optional packages for field-level encryption, Kerberos and zstd compression
- **−** Works only with MongoDB; not a general database abstraction or ODM
- **−** Native add-ons (kerberos, encryption, zstd) can hit C++ compilation problems
- **−** Non-Node runtimes are still in progress; SCRAM-SHA-1 needs Node.js
- **−** Experimental features are excluded from semver and may break in any release

<sub>no GPU · Needs MongoDB server 4.4+, Node.js · [Repo](https://github.com/mongodb/node-mongodb-native) · [📖 Docs ↗](https://mongodb.github.io/node-mongodb-native) · [🌐 Site ↗](https://www.mongodb.com/docs/drivers/node) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/node-mongodb-native/)</sub>

<a name="mongo-go-driver"></a>
### #&#8288;36 [mongo-go-driver](https://github.com/mongodb/mongo-go-driver) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Nov 2026</sub>

**Official MongoDB driver for Go, with a BSON package.**

Go client library for MongoDB, installed as a Go module (go.mongodb.org/mongo-driver/v2). It provides a mongo.Client with Database and Collection handles, cursors, a bson package, and network compression via snappy, zlib or zstd. Version 2.0 is current, and a migration guide covers upgrading from 1.x.

- **+** Maintained by MongoDB; follows semantic versioning with a v2.0 migration guide
- **+** Supports snappy, zlib and zstd network compression, negotiated with the server
- **+** Connect does not block on server discovery; Ping checks reachability explicitly
- **+** Includes its own bson package, so no extra serialization dependency
- **−** Requires Go 1.25 or higher; only the last two Go minor versions are supported
- **−** Needs MongoDB 4.4 or newer; older servers are unsupported
- **−** Running the driver test suite requires Go 1.26 or higher
- **−** Upgrading from 1.x to 2.0 involves breaking changes and a migration step

<sub>no GPU · Docker · Needs MongoDB 4.4+ · [Repo](https://github.com/mongodb/mongo-go-driver) · [📖 Docs ↗](https://www.mongodb.com/docs/drivers/go/current/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongo-go-driver/)</sub>

<a name="clickhouse"></a>
### #&#8288;37 [clickhouse](https://github.com/clickhouse/clickhouse) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 51k · Apache-2.0 · Nov 2026</sub>

**Column-oriented database for real-time analytical reports.**

ClickHouse is an open-source column-oriented database management system written in C++, built to generate analytical reports in real time. It installs on Linux, macOS and FreeBSD with a curl one-liner, and the maintainers also run a hosted ClickHouse Cloud service. It is a general analytics database rather than an AI starter, so it fits this list only as a backend component.

- **+** Apache-2.0 licensed, with a monthly release cadence and recorded release calls
- **+** Single curl install script for Linux, macOS and FreeBSD
- **+** Official docs, tutorial for a small cluster, and a managed cloud option from the maintainers
- **−** Not an AI or vibe-coding starter; no auth, billing or app scaffolding included
- **−** Install is a curl-to-shell script; no Docker or Compose files detected in the repo
- **−** README is mostly links and event listings, with no usage examples or benchmarks
- **−** Analytical column store, so not a general-purpose transactional database

<sub>Docker · [Repo](https://github.com/clickhouse/clickhouse) · [📖 Docs ↗](https://clickhouse.com/docs/) · [🌐 Site ↗](https://clickhouse.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/clickhouse/)</sub>

<a name="graphql-engine"></a>
### #&#8288;38 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Nov 2026</sub>

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

<a name="pulumi"></a>
### #&#8288;39 [pulumi](https://github.com/pulumi/pulumi) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

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

<a name="temporal"></a>
### #&#8288;40 [temporal](https://github.com/temporalio/temporal) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Nov 2026</sub>

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

<a name="rxdb"></a>
### #&#8288;41 [rxdb](https://github.com/pubkey/rxdb) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · Apache-2.0 · Nov 2026</sub>

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

<a name="rqlite"></a>
### #&#8288;42 [rqlite](https://github.com/rqlite/rqlite) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Nov 2026</sub>

**Distributed, fault-tolerant relational database built on SQLite.**

rqlite replicates a SQLite database across a cluster of nodes and exposes it through an HTTP JSON API, with a built-in console and CLI. It ships as a single Go binary with no external dependencies and can load SQLite extensions such as sqlite-vec. Clusters can form automatically via Kubernetes, Docker Compose, Consul, etcd or DNS.

- **+** Single binary with no external dependencies; one docker run command starts a node
- **+** Full SQLite SQL, including FTS5, JSON and loadable extensions like sqlite-vec
- **+** Tunable read consistency and durability per request
- **+** Hot backups, with automatic backups to AWS S3, MinIO and Google Cloud
- **−** Access is through an HTTP API rather than a native SQLite driver
- **−** Not an AI project; vector search needs a separately loaded extension
- **−** Change Data Capture streams to an external system you must provide

<sub>no GPU · Docker · port 4001 · [Repo](https://github.com/rqlite/rqlite) · [📖 Docs ↗](https://rqlite.io/docs/quick-start/) · [🌐 Site ↗](https://rqlite.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rqlite/)</sub>

<a name="onedev"></a>
### #&#8288;43 [onedev](https://github.com/theonedev/onedev) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Nov 2026</sub>

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

<a name="caprover"></a>
### #&#8288;44 [caprover](https://github.com/caprover/caprover) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Nov 2026</sub>

**Self-hosted app and database deployment manager with CLI and web GUI.**

CapRover is a self-hosted deployment platform that runs apps and databases on your own server using Docker Swarm, nginx and Let's Encrypt. It has a web GUI and a CLI for deploying NodeJS, Python, PHP, ASP.NET, Ruby and Go apps, and installs MariaDB, MySQL, MongoDB, Postgres or WordPress from a dropdown. It is pitched as a cheaper alternative to Heroku-style hosting.

- **+** Docker Swarm underneath, so clustering across servers is supported
- **+** Automatic free HTTPS via Let's Encrypt
- **+** Customizable nginx template for load balancing
- **+** No lock-in: apps keep running if CapRover is removed
- **−** License detected as NOASSERTION, so terms need manual checking
- **−** No AI features; it is a general deployment tool
- **−** Depends on Docker Swarm, nginx and NetData stack
- **−** Pitch focuses on single-server cost savings; no benchmarks given

<sub>no GPU · Needs Docker, Docker Swarm, nginx, Let's Encrypt, NetData · [Repo](https://github.com/caprover/caprover) · [📖 Docs ↗](https://caprover.com/) · [🌐 Site ↗](https://caprover.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/caprover/)</sub>

<a name="casdoor"></a>
### #&#8288;45 [casdoor](https://github.com/casdoor/casdoor) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

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

<a name="supabase"></a>
### #&#8288;46 [supabase](https://github.com/supabase/supabase) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 115k · Apache-2.0 · Nov 2026</sub>

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

<a name="nocodb"></a>
### #&#8288;47 [nocodb](https://github.com/nocodb/nocodb) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 66k · custom license · Nov 2026</sub>

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

<a name="payload"></a>
### #&#8288;48 [payload](https://github.com/payloadcms/payload) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

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

<a name="rocksdb"></a>
### #&#8288;49 [rocksdb](https://github.com/meta/rocksdb) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · GPL-2.0 · Nov 2026</sub>

**Embedded LSM-tree key-value store library for flash and RAM.**

RocksDB is a C++ library that stores persistent key-value data using a log-structured merge (LSM) design. It lets you tune the tradeoff between write, read and space amplification, and uses multi-threaded compactions to handle multiple terabytes in one database. It is a building block for a key-value server, not an AI tool; it is dual-licensed under GPLv2 and Apache 2.0.

- **+** Tunable write, read and space amplification tradeoffs through LSM design
- **+** Multi-threaded compactions suit multi-terabyte single databases
- **+** Built on LevelDB; maintained by Facebook Database Engineering
- **+** Dual-licensed GPLv2 or Apache 2.0, at the user's choice
- **−** Embedded library only: no server, auth or network API included
- **−** Only headers in include/ are public; internal APIs may change without warning
- **−** Not AI-related, so it fits this list only loosely
- **−** Tuning compaction and amplification requires reading the wiki in depth

<sub>no GPU · [Repo](https://github.com/meta/rocksdb) · [📖 Docs ↗](https://github.com/meta/rocksdb/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rocksdb/)</sub>

<a name="dokku"></a>
### #&#8288;50 [dokku](https://github.com/dokku/dokku) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Nov 2026</sub>

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

<a name="tdengine"></a>
### #&#8288;51 [tdengine](https://github.com/taosdata/tdengine) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · AGPL-3.0 · Nov 2026</sub>

**Distributed time-series database for IoT and industrial data, written in C.**

TDengine is a time-series database with built-in caching, stream processing and data subscription, aimed at IoT, connected-car and industrial workloads. It uses super tables, time-based partitioning and Raft-based clustering, and includes the TDgpt component for forecasting and anomaly detection. This README mainly covers building from source, producing taosd, the taos CLI, taosBenchmark and taosdump.

- **+** Built-in caching, stream processing and data subscription in one server
- **+** Native clustering with sharding, Raft and compute/storage separation
- **+** TDgpt adds forecasting, anomaly detection, imputation and classification
- **+** Ships CLI, taosBenchmark and taosdump tools alongside the taosd server
- **−** AGPL-3.0 license restricts use in closed-source network services
- **−** S3 support is switched off in community builds
- **−** taoskeeper, taos-explorer, taosx and connectors live in other repositories
- **−** Windows support in the open-source tree is limited

<sub>RAM ≥ 4 GB · no GPU · Needs CMake 3.21+, Python 3 (tests), Go 1.23+ (taosAdapter, taosKeeper) · [Repo](https://github.com/taosdata/tdengine) · [▶️ Demo ↗](https://cloud.tdengine.com) · [📖 Docs ↗](https://docs.tdengine.com) · [🌐 Site ↗](https://tdengine.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tdengine/)</sub>

<a name="bytebase"></a>
### #&#8288;52 [bytebase](https://github.com/bytebase/bytebase) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Nov 2026</sub>

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

<a name="emdash-cms-emdash"></a>
### #&#8288;53 [emdash-cms/emdash](https://github.com/emdash-cms/emdash) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Nov 2026</sub>

**TypeScript CMS on Astro with sandboxed plugins and a built-in MCP server.**

EmDash is an Astro integration that adds an admin panel, REST API, passkey-first auth, media library and plugin system to an Astro site. Content types are defined in the database through the admin UI, with each collection backed by a real SQL table and rich text stored as Portable Text. It runs on Cloudflare (D1, R2, Workers) or on Node.js with SQLite, and includes a WordPress import wizard.

- **+** Plugins run in sandboxed Worker isolates with declared capability manifests
- **+** Portable storage layers: SQLite, D1, Turso, PostgreSQL; R2, S3 or local files
- **+** Imports WordPress content from WXR exports, REST API or WordPress.com
- **+** Ships a CLI, agent skills and a built-in MCP server for AI tools
- **−** Tied to Astro; the CMS is an integration, not a standalone service
- **−** First-party plugins and plugin tooling are still on 0.x and may change
- **−** Plugin sandboxing needs Worker Loaders on Cloudflare or a workerd child process on Node
- **−** Three starter templates only: blog, marketing and portfolio

<sub>no GPU · Docker + Compose · Needs Astro, Cloudflare D1/R2/Workers or Node.js with SQLite, Optional: PostgreSQL, Turso/libSQL, S3, Redis · port 4321 · [Repo](https://github.com/emdash-cms/emdash) · [📖 Docs ↗](https://docs.emdashcms.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/emdash-cms-emdash/)</sub>

<a name="starrocks"></a>
### #&#8288;54 [starrocks](https://github.com/starrocks/starrocks) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Nov 2026</sub>

**Distributed vectorized SQL engine for real-time and data lake analytics.**

StarRocks is an MySQL-protocol-compatible analytical database with a cost-based optimizer and a vectorized execution engine, written in Java (frontend) and C++ (backend). It supports primary-key upserts and deletes, materialized views, and direct queries over Hive, Iceberg, Delta Lake and Hudi tables without importing. Since 3.0 it also offers a shared-data architecture. It is a general OLAP database, not an AI-specific project.

- **+** MySQL protocol and ANSI SQL, so existing clients and BI tools connect directly
- **+** Queries Hive, Iceberg, Delta Lake and Hudi tables in place, without importing
- **+** Primary-key upsert/delete plus auto-refreshed materialized views chosen at query time
- **+** Shared-data architecture available since 3.0; per-tenant resource isolation
- **−** Cluster of separate Frontend and Backend node types, heavier than a single-binary database
- **−** Speed claims (3x, 5-10x) come from vendor benchmarks, not reproduced in the README
- **−** No AI, LLM or vector features described; it is an analytics database

<sub>Compose · [Repo](https://github.com/starrocks/starrocks) · [▶️ Demo ↗](https://github.com/StarRocks/demo) · [📖 Docs ↗](https://docs.starrocks.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/starrocks/)</sub>

<a name="frappe"></a>
### #&#8288;55 [frappe](https://github.com/frappe/frappe) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Nov 2026</sub>

**Full-stack Python and JavaScript framework with metadata-driven admin UI and REST API.**

Frappe Framework is a full-stack web framework using Python and MariaDB on the server and an integrated JavaScript client library. Applications are defined through metadata, which generates forms, list views, a REST API, role-based permissions and a report builder. It began as the base for ERPNext and now includes an MCP server that lets agents read and change documents as a site user.

- **+** Metadata-defined models generate admin UI, forms, list views and REST API automatically
- **+** Role-based permission system and no-code report builder included
- **+** Built-in MCP server exposes schemas, documents and methods to agents
- **+** Proven on ERPNext, which has more than 700 object types
- **−** Server side is built on MariaDB; no other database is mentioned
- **−** README says it is not a good first framework for beginners
- **−** Needs the bench CLI and Frappe conventions rather than standard Python web stacks
- **−** AI support is limited to the MCP server; no model or provider integrations

<sub>no GPU · Needs MariaDB, bench, Docker (optional) · port 8000 · [Repo](https://github.com/frappe/frappe) · [📖 Docs ↗](https://docs.frappe.io/framework) · [🌐 Site ↗](https://frappe.io/framework) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frappe/)</sub>

<a name="flexprice"></a>
### #&#8288;56 [flexprice](https://github.com/flexprice/flexprice) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · AGPL-3.0 · Nov 2026</sub>

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

<a name="valkey"></a>
### #&#8288;57 [valkey](https://github.com/valkey-io/valkey) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · BSD-3-Clause · Nov 2026</sub>

**Key/value data structure server forked from Redis, with modules and clustering.**

Valkey is a C data structure server for key/value workloads, forked from Redis before its move to source-available licenses. It builds with make, or an experimental CMake setup, on Linux, macOS and the BSDs. It supports TLS, experimental RDMA, a module system, replication, Cluster and Sentinel. It is general infrastructure, not an AI project, so it fits this list only as a backing store.

- **+** BSD-3-Clause license, run as an open community project under LF Projects
- **+** Builds on Linux, macOS and BSDs, 32 or 64 bit, with jemalloc default on Linux
- **+** TLS as built-in or module; optional Zstandard compression for RDB and replication
- **+** make install adds Redis-named symlinks (redis-server, redis-cli) for compatibility
- **−** Not an AI project; README describes no model, agent or retrieval features
- **−** RDMA support is experimental and may change or be removed in any version
- **−** CMake build is experimental; Makefile is the main build path
- **−** No Docker or compose files detected; README covers building from source only

<sub>no GPU · Needs C compiler and make, OpenSSL (optional, for TLS), Zstandard 1.4.7+ (optional) · [Repo](https://github.com/valkey-io/valkey) · [🌐 Site ↗](https://valkey.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/valkey/)</sub>

<a name="mongoose"></a>
### #&#8288;58 [mongoose](https://github.com/automattic/mongoose) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Nov 2026</sub>

**MongoDB object modeling library for Node.js with schemas, validation and middleware.**

Mongoose is an ODM for MongoDB built on the official Node.js driver. Schemas define document structure, validators, defaults, getters, setters, indexes, middleware and populate (pseudo-JOINs). It runs on Node.js, with alpha Deno support, and installs through npm, pnpm, Yarn or Bun.

- **+** Schema-level validators, defaults, indexes and pre/post middleware for documents and embedded documents
- **+** Buffers commands until connected, so models and queries can be defined before connect completes
- **+** Built on the official MongoDB Node.js driver; raw collection stays reachable via Model.collection
- **+** Plugin system with hundreds of community modules listed on plugins.mongoosejs.io
- **−** MongoDB only; no support for other databases
- **−** Deno support is labelled alpha
- **−** Using Model.collection directly bypasses hooks and validation
- **−** Version 9.0.0 includes backwards-breaking changes requiring a migration guide

<sub>no GPU · Needs MongoDB, Node.js · [Repo](https://github.com/automattic/mongoose) · [📖 Docs ↗](https://mongoosejs.com/docs/api/mongoose.html) · [🌐 Site ↗](https://mongoosejs.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongoose/)</sub>

<a name="mybatis-plus"></a>
### #&#8288;59 [mybatis-plus](https://github.com/baomidou/mybatis-plus) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

**MyBatis extension adding CRUD mappers, query wrappers and pagination for Java.**

MyBatis-Plus is a Java library layered on MyBatis. Extending BaseMapper gives a mapper ready-made CRUD methods, and QueryWrapper or lambda-style wrappers build WHERE conditions without hand-written XML. It also covers pagination, primary key strategies, active record and SQL injection defense, with starters for Spring Boot 2, 3 and 4. It is not an AI project.

- **+** Fully compatible with MyBatis; existing mappers and XML keep working
- **+** BaseMapper supplies CRUD methods; lambda wrappers avoid column-name strings
- **+** Separate starters for Spring Boot 2, 3 and 4, plus @MybatisPlusTest test starters
- **+** SQL-parsing plugins can use JSqlParser 4.9 to 5.4, matched to your JDK
- **−** Not an AI tool; it is a Java database access library, so category fit is loose
- **−** Since 3.5.9, pagination and similar plugins need a separate JSqlParser module
- **−** Advanced features are in the separate enterprise edition, Mybatis-Mate
- **−** README is partly Chinese, and the community group is joined via WeChat

<sub>no GPU · Needs MyBatis, Spring Boot (optional starters), JSqlParser (optional), Relational database · [Repo](https://github.com/baomidou/mybatis-plus) · [📖 Docs ↗](https://baomidou.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mybatis-plus/)</sub>

<a name="spree"></a>
### #&#8288;60 [spree](https://github.com/spree/spree) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · BSD-3-Clause · Nov 2026</sub>

**Headless Ruby commerce backend with REST APIs, React admin, marketplace and B2B.**

Spree is a Ruby headless ecommerce backend exposing REST APIs with TypeScript SDKs, a Vite and React admin dashboard, and an optional Next.js storefront. The core covers multi-vendor marketplaces with commissions and Stripe Connect payouts, B2B price lists and companies, and multi-region markets. It also includes a built-in MCP server and agent skills for coding tools, and is scaffolded with `npx create-spree-app`.

- **+** Marketplace, B2B and cross-border features are in the BSD-3-Clause core, not paid-only
- **+** Ships Stripe, Adyen and PayPal payments, plus Avalara and Stripe Tax calculation
- **+** Built-in MCP server and agent skills for managing and customizing a store with AI tools
- **+** Provider contracts for ERP, PIM, WMS, DAM, SSO and payouts fit existing stacks
- **−** Multi-tenant SaaS, B2B approval workflows and audit logging need the paid Enterprise Edition
- **−** Local setup needs Node.js 24+ and Docker; the backend is Ruby
- **−** Storefront lives in a separate repo from the backend and admin, adding parts to maintain
- **−** Typo-tolerant search relies on a separate MeiliSearch service or a custom provider

<sub>no GPU · Needs Docker, Node.js 24+, Git, MeiliSearch (optional), Stripe (optional) · [Repo](https://github.com/spree/spree) · [▶️ Demo ↗](https://demo.spreecommerce.org/) · [📖 Docs ↗](https://spreecommerce.org/docs/) · [🌐 Site ↗](https://spreecommerce.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spree/)</sub>

<a name="logto"></a>
### #&#8288;61 [logto](https://github.com/logto-io/logto) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MPL-2.0 · Nov 2026</sub>

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
### #&#8288;62 [kysely](https://github.com/kysely-org/kysely) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

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

<a name="redis"></a>
### #&#8288;63 [redis](https://github.com/redis/redis) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 78k · custom license · Nov 2026</sub>

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

<a name="etcd"></a>
### #&#8288;64 [etcd](https://github.com/etcd-io/etcd) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 53k · Apache-2.0 · Nov 2026</sub>

**Distributed key-value store using Raft, with a gRPC API.**

etcd is a replicated key-value store written in Go that uses the Raft consensus algorithm for a highly available log. Clients talk to it over gRPC, with TLS and optional client certificate authentication. It is not an AI project; it is infrastructure commonly paired with Kubernetes, and it ships with the etcdctl CLI and a Go client library.

- **+** Raft-replicated log gives consistent, highly available storage across cluster members
- **+** Documented benchmark of 10,000 writes/sec
- **+** Automatic TLS with optional client cert authentication
- **+** Robustness test suite in the repo; used in production with Kubernetes
- **−** No AI features; unrelated to LLM or vibe-coding starters
- **−** Key-value only, no SQL or rich query model
- **−** Main branch may be unstable; use tagged releases
- **−** Multi-member clusters need separate setup and tuning

<sub>no GPU · Docker · Needs goreman (optional, for local example cluster) · port 2379 · [Repo](https://github.com/etcd-io/etcd) · [▶️ Demo ↗](https://etcd.io/docs/latest/demo) · [📖 Docs ↗](https://etcd.io/docs/latest) · [🌐 Site ↗](https://etcd.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/etcd/)</sub>

<a name="foundationdb"></a>
### #&#8288;65 [foundationdb](https://github.com/apple/foundationdb) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

**Distributed ordered key-value store with ACID transactions.**

FoundationDB is a distributed database that stores structured data as an ordered key-value store and applies ACID transactions to all operations. It runs on clusters of commodity servers and is accessed through language bindings. The repo is C++ built with CMake and Ninja, with binary packages on the releases page.

- **+** ACID transactions on every operation over an ordered key-value model
- **+** Releases validated via simulation and real cluster tests, per the README
- **+** Supported 8.0 and 7.4 branches with documented upgrade paths
- **+** Language bindings, plus prebuilt binary packages for download
- **−** Source build has many dependencies; the Docker build image is the recommended route
- **−** Source build needs at least 8GB of memory, more when parallel
- **−** Key-value API only; no SQL or document layer in this repo
- **−** Windows builds support only Visual Studio with ClangCl

<sub>RAM ≥ 8 GB · no GPU · Needs CMake 3.24.2+, Ninja, Mono, Boost 1.89 · [Repo](https://github.com/apple/foundationdb) · [📖 Docs ↗](https://apple.github.io/foundationdb/) · [🌐 Site ↗](https://www.foundationdb.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/foundationdb/)</sub>

<a name="electric-pglite"></a>
### #&#8288;66 [electric-pglite](https://github.com/neondatabase/electric-pglite) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · Apache-2.0 · Nov 2026</sub>

**Postgres compiled to WASM, run in browser, Node, Bun and Deno.**

PGlite packages Postgres built to WebAssembly as a TypeScript library, so it runs in the browser, Node.js, Bun and Deno with no other install. It works as an in-memory database or persists to the file system or IndexedDB, and supports extensions such as pgvector and PostGIS. It runs Postgres in single-user mode with an I/O layer, not in a Linux VM.

- **+** About 3 MB gzipped, with no dependencies to install
- **+** Runs real Postgres in WASM, not a Linux VM
- **+** Supports extensions including pgvector and PostGIS
- **+** Persists to the file system or IndexedDB, or runs in memory
- **−** Single user and single connection only
- **−** README labels the project alpha status
- **−** Building the WASM module from source requires Docker
- **−** Single-process design, not a drop-in server replacement

<sub>no GPU · [Repo](https://github.com/neondatabase/electric-pglite) · [📖 Docs ↗](https://pglite.dev) · [🌐 Site ↗](https://pglite.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/electric-pglite/)</sub>

<a name="openship"></a>
### #&#8288;67 [openship](https://github.com/oblien/openship) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

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

<a name="go-admin"></a>
### #&#8288;68 [go-admin](https://github.com/go-admin-team/go-admin) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<a name="react-native-firebase"></a>
### #&#8288;69 [react-native-firebase](https://github.com/invertase/react-native-firebase) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Nov 2026</sub>

**Official React Native modules wrapping the native Firebase iOS and Android SDKs.**

A Lerna monorepo of npm packages, each a thin JavaScript layer over the native Firebase SDKs on iOS and Android. It covers Auth, Cloud Firestore, Realtime Database, Cloud Storage, Cloud Functions, Cloud Messaging, Analytics, Crashlytics, Remote Config, App Check and an AI package. The API mirrors the Firebase Web SDK, so code can be shared with web apps.

- **+** Uses the native iOS and Android Firebase SDKs rather than a JS reimplementation
- **+** Separate npm package per Firebase service, so apps install only what they use
- **+** API mirrors the Firebase Web SDK, which helps reuse code on web
- **+** TypeScript types included; README claims over 95% test coverage per module
- **−** Client SDK only; it needs a Firebase project and does not self-host a backend
- **−** Requires native iOS and Android configuration, so it does not run in Expo Go
- **−** License is not identified by the detector (NOASSERTION), so check the LICENSE file
- **−** Tied to Google's proprietary Firebase services, which makes migrating away costly

<sub>no GPU · Needs Firebase project, Native Firebase iOS SDK, Native Firebase Android SDK · [Repo](https://github.com/invertase/react-native-firebase) · [🌐 Site ↗](https://rnfirebase.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-native-firebase/)</sub>

<a name="webiny-js"></a>
### #&#8288;70 [webiny-js](https://github.com/webiny/webiny-js) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.1k · custom license · Nov 2026</sub>

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
### #&#8288;71 [registry](https://github.com/modelcontextprotocol/registry) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · custom license · Nov 2026</sub>

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

<a name="harlequin"></a>
### #&#8288;72 [harlequin](https://github.com/tconbeer/harlequin) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Nov 2026</sub>

**Terminal SQL IDE with adapters for DuckDB, SQLite, Postgres and other databases.**

Harlequin is a Python terminal application for writing and running SQL, browsing a data catalog and exporting results. It ships with DuckDB and SQLite adapters, and other databases such as Postgres, MySQL/MariaDB and ODBC connect through separately installed adapter packages. A companion CLI, hsql, runs queries headlessly for scripts and agents, with read-only and timeout options.

- **+** DuckDB and SQLite adapters ship in the box; opens in-memory or file databases directly
- **+** Adapter plug-ins cover other databases, installable as extras like harlequin[postgres]
- **+** hsql companion CLI offers --read-only, --timeout and catalog search for agent use
- **+** Profiles in config files can reference environment variables, keeping credentials out of shared configs
- **−** Terminal UI only; no web or desktop interface
- **−** Adapters install as separate Python packages into the same environment
- **−** Not an MCP server; agent access goes through the hsql CLI
- **−** Homebrew formula is community-maintained and less tested than the Python installs

<sub>no GPU · Needs Python 3.9+, uv (recommended installer) · [Repo](https://github.com/tconbeer/harlequin) · [📖 Docs ↗](https://harlequin.sh/docs/getting-started/index) · [🌐 Site ↗](https://harlequin.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/harlequin/)</sub>

<a name="postgrest"></a>
### #&#8288;73 [postgrest](https://github.com/postgrest/postgrest) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Nov 2026</sub>

**REST API server generated directly from an existing PostgreSQL schema.**

PostgREST is a Haskell server, built on Warp and Hasql, that exposes tables and views of an existing PostgreSQL database as a RESTful API. Authentication uses JSON Web Tokens, and authorization is delegated to PostgreSQL roles, with JSON serialization and validation done in SQL. It is stateless and can be scaled horizontally.

- **+** Authorization lives in database roles, giving one source of truth for security
- **+** Stateless server with a connection pool, so it scales horizontally
- **+** Generates OpenAPI documentation that Swagger-UI can render
- **+** API versioning through database schemas and views over underlying tables
- **−** Works only with PostgreSQL, no other databases
- **−** Business logic must be written as SQL constraints, views and functions
- **−** Verifies JWTs but has no built-in user management or login
- **−** No built-in file storage, realtime or admin UI, unlike full backend platforms

<sub>no GPU · Needs PostgreSQL · [Repo](https://github.com/postgrest/postgrest) · [📖 Docs ↗](https://docs.postgrest.org/en/stable/explanations/install.html) · [🌐 Site ↗](http://postgrest.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/postgrest/)</sub>

<a name="dapr"></a>
### #&#8288;74 [dapr](https://github.com/dapr/dapr) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

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

<a name="actix-web"></a>
### #&#8288;75 [actix-web](https://github.com/actix/actix-web) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Nov 2026</sub>

**Rust web framework for HTTP/1.x and HTTP/2 servers on Tokio.**

Actix Web is a general-purpose Rust web framework with routing macros, middleware, WebSockets, multipart streams and static file serving. It runs on Tokio and supports TLS through OpenSSL or Rustls. It has no AI-specific features; it fits this list as a base for a backend service that exposes models or agents over an API.

- **+** Supports HTTP/1.x, HTTP/2, WebSockets and streaming in one framework
- **+** Built-in compression (br, gzip, deflate, zstd) and TLS via OpenSSL or Rustls
- **+** Examples repo covers Postgres, SQLite, MongoDB, Diesel and templating
- **+** Compatible with Tokio and runs on stable Rust 1.89+
- **−** No AI, LLM or agent features; model serving must be built by the user
- **−** Rust-only, so Python AI libraries need a separate service or bindings
- **−** Experimental features are prefixed and may break in any release
- **−** Library, not a template; auth, database and layout are left to you

<sub>no GPU · Needs Rust 1.89+, Tokio · [Repo](https://github.com/actix/actix-web) · [📖 Docs ↗](https://docs.rs/actix-web) · [🌐 Site ↗](https://actix.rs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/actix-web/)</sub>

<a name="questdb"></a>
### #&#8288;76 [questdb](https://github.com/questdb/questdb) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Nov 2026</sub>

**Time-series SQL database for high-rate ingestion and queries over live and historical data.**

QuestDB is a time-series database written in zero-GC Java with C++ and Rust on the hot paths. It stores data in time-partitioned columns, with Parquet conversion for older partitions. SQL extends the standard with SAMPLE BY, LATEST ON and ASOF JOIN, and clients write and read over its binary QWP protocol, PostgreSQL wire (8812), ILP or REST (9000).

- **+** Reports 8.59M rows/sec TSBS ingestion on one 32 vCPU instance, ahead of ClickHouse and TimescaleDB
- **+** Speaks QWP, PostgreSQL wire, InfluxDB Line Protocol and REST, so existing drivers and collectors work
- **+** Time-series SQL built in: SAMPLE BY, ASOF JOIN, materialized views, deduplication and out-of-order handling
- **+** Web Console with SQL editor, charts and CSV import on port 9000, plus a public live demo
- **−** Replication, high availability, RBAC, TLS, SSO and automatic object-storage tiering are Enterprise only
- **−** Open source needs manual ALTER TABLE to convert partitions to Parquet
- **−** Native libraries bundled for Apple Silicon only; Intel Macs must use Docker
- **−** Live views are in beta, and the Node.js client lacks QWP support for now

<sub>no GPU · port 9000 · [Repo](https://github.com/questdb/questdb) · [▶️ Demo ↗](https://demo.questdb.io/) · [📖 Docs ↗](https://questdb.com/docs/) · [🌐 Site ↗](https://questdb.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/questdb/)</sub>

<a name="doris"></a>
### #&#8288;77 [doris](https://github.com/apache/doris) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · Apache-2.0 · Nov 2026</sub>

**MPP analytics database for real-time SQL, lakehouse queries and hybrid search.**

Apache Doris is an MPP analytics database that serves sub-second SQL queries under high concurrency, with streaming ingestion. It also queries Iceberg, Delta Lake and Hudi tables and supports full-text, JSON and vector search in SQL. It runs in compute-storage coupled mode or in a decoupled mode with stateless compute groups over shared object storage.

- **+** Queries Iceberg, Delta Lake and Hudi tables directly, without a separate engine
- **+** Decoupled mode scales stateless compute groups over shared object storage
- **+** Official Flink, Spark, Kafka connectors, Stream Loader and Kubernetes operator
- **+** Apache top-level project since June 2022, with regular releases
- **−** Analytics database, not an app backend with auth, storage or APIs
- **−** Some third-party dependencies conflict with Apache 2.0; features must be disabled to comply
- **−** Cluster deployment is more involved than a single-node database
- **−** README gives no hardware sizing; no Docker or compose files detected

<sub>Docker · Needs Object storage (decoupled mode) · [Repo](https://github.com/apache/doris) · [📖 Docs ↗](https://doris.apache.org/docs/dev/getting-started/what-is-apache-doris) · [🌐 Site ↗](https://doris.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/doris/)</sub>

<a name="citus"></a>
### #&#8288;78 [citus](https://github.com/citusdata/citus) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · AGPL-3.0 · Nov 2026</sub>

**PostgreSQL extension that shards tables across nodes for distributed queries.**

Citus is a C-based PostgreSQL extension that adds distributed tables, replicated reference tables, a distributed query engine and columnar storage. It runs on a single node or a coordinator plus worker cluster, with shard rebalancing when nodes are added. Aimed at multi-tenant, real-time analytics and time-series workloads that outgrow one Postgres server.

- **+** Runs inside regular PostgreSQL, so existing SQL, extensions and tools keep working
- **+** Co-located distributed tables allow distributed joins and foreign keys on the distribution column
- **+** create_distributed_table_concurrently converts live tables without blocking reads or writes
- **+** Schema-based sharding for multi-tenant and microservice apps without query changes
- **−** Columnar tables do not support update, delete or foreign keys
- **−** Licensed AGPL-3.0, which may constrain some commercial use
- **−** Multi-node setup needs manual coordinator and worker configuration and shard rebalancing
- **−** Requires choosing a distribution column up front for good query routing

<sub>no GPU · Needs PostgreSQL 18 · [Repo](https://github.com/citusdata/citus) · [📖 Docs ↗](https://docs.citusdata.com/) · [🌐 Site ↗](https://www.citusdata.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/citus/)</sub>

<a name="peewee"></a>
### #&#8288;79 [peewee](https://github.com/coleifer/peewee) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Nov 2026</sub>

**Small Python ORM and query builder for SQLite, MySQL, MariaDB and PostgreSQL.**

Peewee is a single-module Python ORM with no required dependencies. It defines models and fields, builds composable SQL queries, and supports SQLite, MySQL, MariaDB and PostgreSQL, with asyncio support on aiosqlite, asyncpg and aiomysql. It also ships a diff-based migration runner (pwmigrate) and Flask, FastAPI and Pydantic integrations. It is not an AI project; it fits this list only as a data-layer library.

- **+** Single module with no required dependencies; SQLite works through the standard library
- **+** Covers SQLite, MySQL, MariaDB and PostgreSQL, with sync and asyncio APIs
- **+** Includes a diff-based migration runner (pwmigrate) and playhouse extensions
- **+** Documented Flask and FastAPI integration, plus Pydantic utilities
- **−** Library only: no auth, API server, storage or hosting included
- **−** No AI or LLM features; unrelated to models, agents or RAG
- **−** Async API uses separate a-prefixed methods (acreate, asave) alongside the sync ones
- **−** Database drivers are optional extras that must be installed separately

<sub>no GPU · Needs pymysql (mysql extra), psycopg2 or psycopg3 (postgres extras), aiosqlite, aiomysql or asyncpg (async extras) · [Repo](https://github.com/coleifer/peewee) · [📖 Docs ↗](https://docs.peewee-orm.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/peewee/)</sub>

<a name="falkordb"></a>
### #&#8288;80 [falkordb](https://github.com/falkordb/falkordb) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Nov 2026</sub>

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

<a name="pinot"></a>
### #&#8288;81 [pinot](https://github.com/apache/pinot) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Nov 2026</sub>

**Distributed real-time OLAP datastore with SQL queries over streaming and batch data.**

Apache Pinot is a column-oriented distributed datastore for low-latency analytical SQL on fresh data. It ingests from Kafka, Pulsar and Kinesis as well as batch sources such as HDFS, S3, ADLS and GCS, and can combine both in one table. It also offers vector similarity search, with a built-in query console and REST API.

- **+** Pluggable indexes: timestamp, inverted, StarTree, Bloom, range, text, JSON, geospatial
- **+** Real-time ingest from Kafka, Pulsar and Kinesis, with upserts and batch/stream hybrid tables
- **+** Joins, built-in multitenancy and a Helm chart for Kubernetes clusters
- **+** Vector index supports semantic search and RAG on the same SQL engine
- **−** Multi-component cluster to operate; not a single-process database
- **−** Building from source requires JDK 25+ and a long Maven build
- **−** Suited to immutable, time-series style analytics rather than transactional workloads
- **−** Lucene upgrades or downgrades can trigger index rebuilds, adding CPU and load time

<sub>RAM ≥ 6 GB · no GPU · Needs Apache Kafka (optional, for streaming ingest), Kubernetes/Helm (optional, for cluster deployment), JDK 25+ (to build) · port 9000 · [Repo](https://github.com/apache/pinot) · [📖 Docs ↗](https://docs.pinot.apache.org) · [🌐 Site ↗](https://pinot.apache.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pinot/)</sub>

<a name="typeorm"></a>
### #&#8288;82 [typeorm](https://github.com/typeorm/typeorm) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · MIT · Nov 2026</sub>

**TypeScript and JavaScript ORM with decorators, migrations and many database drivers.**

TypeORM maps TypeScript and JavaScript classes to database tables using decorators, and supports both Active Record and Data Mapper patterns. It works with Postgres, MySQL/MariaDB, SQL Server, Oracle, SAP HANA, Google Spanner, SQLite and MongoDB. It runs in Node.js, browsers, React Native, Electron and other platforms, and includes a QueryBuilder, generated migrations and a CLI.

- **+** Supports Postgres, MySQL/MariaDB, SQL Server, Oracle, SAP HANA, Spanner, SQLite and MongoDB
- **+** Offers both Active Record and Data Mapper patterns
- **+** Migrations can be generated automatically; CLI included
- **+** Runs in Node.js, React Native, Electron, Cordova, Expo and browsers
- **−** A library, not a backend service: no auth, storage or hosting included
- **−** Decorator-based entity model ties schemas to class definitions
- **−** Not an AI project; fits this list only as general backend infrastructure
- **−** Fixtures, ER diagrams and seeding come from third-party extensions

<sub>no GPU · Compose · Needs A supported database (Postgres, MySQL/MariaDB, SQL Server, Oracle, SAP HANA, Spanner, SQLite or MongoDB) · [Repo](https://github.com/typeorm/typeorm) · [🌐 Site ↗](http://typeorm.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typeorm/)</sub>

<a name="dolt"></a>
### #&#8288;83 [dolt](https://github.com/dolthub/dolt) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Nov 2026</sub>

**MySQL-compatible SQL database with Git-style branch, merge, push and pull.**

Dolt is a SQL database that versions tables the way Git versions files. It runs as a single Go binary with a MySQL-compatible server (`dolt sql-server`, port 3306) and a `dolt` CLI that mirrors Git commands. Version control is also exposed in SQL through `dolt_*` system tables, functions and stored procedures. The README says it backs Beads and Gas Town as an agent memory store.

- **+** Git-style commit, branch, merge, diff and blame on tables, from CLI or SQL
- **+** Works with standard MySQL clients; server listens on port 3306 by default
- **+** Single ~103 MB binary; installs via Homebrew, Chocolatey, pacman, MacPorts or script
- **+** Supports foreign keys, triggers, secondary indexes, check constraints and stored procedures
- **−** MySQL 9.0 clients cannot connect by default; MySQL 8.4 recommended unless auth is reconfigured
- **−** Dolt commits differ from SQL transaction commits, which adds a concept to learn
- **−** Joins are documented as supported up to twelve tables
- **−** Building from source needs Go plus a working cgo C toolchain

<sub>no GPU · Docker · port 3306 · [Repo](https://github.com/dolthub/dolt) · [📖 Docs ↗](https://dolthub.com/docs/introduction/installation/windows) · [🌐 Site ↗](https://www.dolthub.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dolt/)</sub>

<a name="timescaledb"></a>
### #&#8288;84 [timescaledb](https://github.com/timescale/timescaledb) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · custom license · Nov 2026</sub>

**PostgreSQL extension for time-series and event data with columnar storage.**

TimescaleDB adds hypertables to PostgreSQL, which partition data into time-based chunks, plus a columnstore that accepts direct inserts for analytical queries. It also provides incrementally refreshed continuous aggregates, time_bucket(), and SkipScan for DISTINCT ON queries. It is used through standard SQL and any PostgreSQL client.

- **+** Runs inside PostgreSQL, so existing SQL, clients and extensions keep working
- **+** Continuous aggregates refresh incrementally, unlike plain materialized views
- **+** Columnstore compression, README cites 90%+ typical, with direct insert into columnar format
- **+** Quickstart includes a local start script and worked examples with sample datasets
- **−** Not an AI project; it is a general time-series database extension
- **−** License is detected as NOASSERTION; check the license terms before commercial use
- **−** Some features, such as tiering to S3, are described under hosted Tiger Cloud
- **−** One-line install script is for local development only, not production

<sub>RAM ≥ 8 GB · no GPU · Needs PostgreSQL, Docker (quickstart), psql · [Repo](https://github.com/timescale/timescaledb) · [📖 Docs ↗](https://docs.tigerdata.com/) · [🌐 Site ↗](https://www.tigerdata.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/timescaledb/)</sub>

<a name="phoenix"></a>
### #&#8288;85 [phoenixframework/phoenix](https://github.com/phoenixframework/phoenix) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

**Elixir web framework for HTTP, WebSocket channels and server-rendered apps.**

Phoenix is a web framework written in Elixir. It includes a `phx.new` Mix task that generates new projects and a JavaScript client (Phoenix.js) for channels. The README describes no AI features. It is a general web and backend framework that you would build an AI app on top of.

- **+** MIT licensed, with the `phx.new` generator for new projects
- **+** Ships the Phoenix.js client library with its own documentation
- **+** Maintained: release 2026-10-20, last commit 2026-11-17
- **+** API docs hosted on HexDocs
- **−** No built-in AI, LLM or agent features described
- **−** Requires Elixir and Mix; no Docker or compose files provided
- **−** A framework, not a ready-to-fork starter with auth or billing

<sub>no GPU · Needs Elixir, Mix · [Repo](https://github.com/phoenixframework/phoenix) · [📖 Docs ↗](https://phoenix.hexdocs.pm) · [🌐 Site ↗](https://www.phoenixframework.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/phoenix/)</sub>

<a name="dagger"></a>
### #&#8288;86 [dagger](https://github.com/dagger/dagger) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

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

<a name="sea-orm"></a>
### #&#8288;87 [sea-orm](https://github.com/seaql/sea-orm) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · Apache-2.0 · Nov 2026</sub>

**Rust ORM with entity relations, migrations and async or sync APIs.**

SeaORM is a Rust ORM built on SQLx and SeaQuery. It maps tables to entities with 1-1, 1-N and M-N relations, loads nested relations without N+1 queries, and persists nested object graphs through ActiveModel. It also includes migrations, an entity-first schema sync mode, a raw SQL macro, and a separate sync crate.

- **+** Entity Loader uses joins for 1-1 and batched loading for 1-N, avoiding N+1
- **+** sea-orm-cli generates entity files from an existing database
- **+** Raw SQL macro supports parameter interpolation without string formatting of SQL
- **+** sea-orm-sync crate offers the same API without an async runtime
- **−** Default features enable no TLS; you must add an SQLx TLS feature yourself
- **−** README describes 2.0 as a release candidate with breaking changes
- **−** SQL Server support is a separate product with commercial access
- **−** Nested ActiveModel requires the 2.0 dense entity format

<sub>no GPU · Needs SQLx, SeaQuery, Tokio (runtime feature), Postgres, MySQL or SQLite · [Repo](https://github.com/seaql/sea-orm) · [📖 Docs ↗](https://www.sea-ql.org/SeaORM) · [🌐 Site ↗](https://www.sea-ql.org/SeaORM) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sea-orm/)</sub>

<a name="baserow"></a>
### #&#8288;88 [baserow](https://github.com/baserow/baserow) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · custom license · Nov 2026</sub>

**No-code database and app builder, positioned as an Airtable alternative.**

Baserow is a spreadsheet-style database built on Django, Vue.js and PostgreSQL. It adds an application builder that publishes on custom domains, automations, dashboards, and an AI assistant (Kuma) that creates databases and workflows from natural language. It runs as a single Docker image (ports 80 and 443) or on Helm, Heroku, Render and AWS, and exposes a REST API with OpenAPI docs.

- **+** Self-hostable via Docker, Compose, Helm, Heroku, Render, AWS, Cloudron and Railway
- **+** API-first, with a public REST API and OpenAPI schema
- **+** Non-premium features under MIT; stack is Django, Vue.js and PostgreSQL
- **+** Database views, app builder, automations and dashboards in one product
- **−** Open-core: premium and enterprise features sit outside the MIT license
- **−** Detected license is NOASSERTION, so mixed licensing needs checking before commercial use
- **−** Merged and closed PRs from the GitLab history were not imported

<sub>no GPU · Docker + Compose · Needs PostgreSQL · port 80 · [Repo](https://github.com/baserow/baserow) · [📖 Docs ↗](https://baserow.io/docs/index) · [🌐 Site ↗](https://baserow.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/baserow/)</sub>

<a name="vike"></a>
### #&#8288;89 [vike](https://github.com/vikejs/vike) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · MIT · Nov 2026</sub>

**Web framework for React, Vue or Solid apps, positioned as a Next.js/Nuxt replacement.**

Vike is a TypeScript web framework presented as a replacement for Next.js and Nuxt. This monorepo holds the core `vike` package, the `create-vike-core` scaffolding package and the vike.dev documentation site. UI integrations (vike-react, vike-vue, vike-solid) live in separate repositories.

- **+** Separate integration packages for React, Vue and Solid
- **+** Public CHANGELOG tracks version history and breaking changes
- **+** Docs site provides an llms.txt index for AI agents
- **+** MIT licensed with commits and a release in November 2026
- **−** General web framework; no built-in AI features, auth or billing
- **−** UI integrations live in separate repos, not this one
- **−** Not an AI project, so it fits this list only loosely
- **−** README has no install steps or feature list; see vike.dev

<sub>no GPU · [Repo](https://github.com/vikejs/vike) · [📖 Docs ↗](https://vike.dev) · [🌐 Site ↗](https://vike.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vike/)</sub>

<a name="mongo-python-driver"></a>
### #&#8288;90 [mongo-python-driver](https://github.com/mongodb/mongo-python-driver) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · Apache-2.0 · Nov 2026</sub>

**Official Python driver for MongoDB with sync and async APIs.**

PyMongo is the native Python driver for MongoDB. It ships three packages: `pymongo` with synchronous and asynchronous clients, `bson` for BSON encoding, and `gridfs` for GridFS storage. It supports MongoDB 4.4 through 9.0 on CPython 3.11+. It is a database client library, not an AI starter.

- **+** Maintained by MongoDB, with releases following semantic versioning
- **+** Sync and async APIs in one package
- **+** Optional extras for GSSAPI, AWS auth, OCSP, snappy/zstd compression and field-level encryption
- **+** Bundles its own bson and gridfs packages
- **−** Needs a separate MongoDB server; it is not a backend by itself
- **−** No AI, vector search or LLM helpers described in the README
- **−** CPython 3.11+ only
- **−** mongodb+srv:// URIs need dnspython installed separately

<sub>no GPU · Needs MongoDB server 4.4-9.0, dnspython (for mongodb+srv URIs) · [Repo](https://github.com/mongodb/mongo-python-driver) · [📖 Docs ↗](https://www.mongodb.com/docs/languages/python/pymongo-driver/current/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongo-python-driver/)</sub>

<a name="parse-server"></a>
### #&#8288;91 [parse-server](https://github.com/parse-community/parse-server) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

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

<a name="apijson"></a>
### #&#8288;92 [apijson](https://github.com/apijson/apijson) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Nov 2026</sub>

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

<a name="router"></a>
### #&#8288;93 [tanstack/router](https://github.com/tanstack/router) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Nov 2026</sub>

**Type-safe client router for React, with a full-stack SSR framework built on it.**

TanStack Router is a TypeScript routing library with typed routes, params and loaders, and schema-validated search params. It includes caching, prefetching, invalidation, nested layouts and error boundaries. TanStack Start builds on it and adds full-document SSR, streaming and server functions. The README describes no AI features, so this is a general web framework, not an AI project.

- **+** End-to-end type safety across routes, params and loaders
- **+** Search params are schema-driven and validated
- **+** Built-in caching, prefetching and invalidation for route data
- **+** Start adds SSR, streaming and server functions on the same router
- **−** No AI, LLM or agent functionality; a poor fit for this list's themes
- **−** Not a backend or database; Start only covers server rendering and functions
- **−** README gives no install steps or code examples; it defers to the docs site

<sub>no GPU · [Repo](https://github.com/tanstack/router) · [📖 Docs ↗](https://tanstack.com/router) · [🌐 Site ↗](https://tanstack.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/router/)</sub>

<a name="dexie-js"></a>
### #&#8288;94 [dexie.js](https://github.com/dexie/dexie.js) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · Apache-2.0 · Nov 2026</sub>

**Typed IndexedDB wrapper with chainable queries, bulk ops and React hooks.**

Dexie.js wraps the browser's IndexedDB with a declarative schema, chainable where/collection queries and promise-based CRUD and bulk methods. It runs in browsers, Electron, Capacitor and PWAs, and dexie-react-hooks adds a useLiveQuery hook. Sync, auth and access control come from the separate Dexie Cloud addon, hosted or self-hosted.

- **+** Bulk methods skip per-item onsuccess handling, which speeds up large writes
- **+** Works around IndexedDB bugs across browser engines, per the README
- **+** Chainable queries like where('age').below(30) with TypeScript entity typing
- **+** Runs in browsers, Electron and Capacitor; installs from npm or a script tag
- **−** Client-side storage only; sync needs the separate Dexie Cloud addon and service
- **−** Legacy sync packages dexie-observable and dexie-syncable are deprecated and unmaintained
- **−** Not an AI project; no model or LLM features in the library
- **−** Queries rely on declared indexes and IndexedDB semantics, not SQL

<sub>no GPU · Needs IndexedDB (browser) · [Repo](https://github.com/dexie/dexie.js) · [▶️ Demo ↗](https://dexie.github.io/Dexie.js/dexie-cloud-todo-app/) · [📖 Docs ↗](https://dexie.org/docs/) · [🌐 Site ↗](https://dexie.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dexie-js/)</sub>

<a name="yugabyte-db"></a>
### #&#8288;95 [yugabyte-db](https://github.com/yugabyte/yugabyte-db) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Nov 2026</sub>

**PostgreSQL-compatible distributed SQL database with Raft replication.**

YugabyteDB is a distributed SQL database that reuses the PostgreSQL query layer (YSQL) and also offers a Cassandra-style API (YCQL). Writes are replicated with Raft and use distributed ACID transactions based on the Spanner design, with snapshot, serializable and read committed isolation. Clusters scale by adding nodes and can span zones, regions and clouds, with xCluster asynchronous replication between regions.

- **+** Reuses the PostgreSQL query layer; PostgreSQL 15 fork in the v2025.1 stable release
- **+** Raft replication with distributed ACID transactions; README cites RPO 0 and RTO of 3 seconds
- **+** Core includes backups, TLS, encryption at rest, CDC and read replicas under Apache 2.0
- **+** pgvector with HNSW indexing supports vector similarity search
- **−** Repo mixes licenses: core is Apache 2.0, managed/ (YugabyteDB Anywhere) is Polyform Free Trial
- **−** Not a drop-in PostgreSQL: several features, such as parallel query and CBO, are still on the roadmap
- **−** Multi-node distributed deployment adds operational complexity compared with a single PostgreSQL instance
- **−** Existing universes keep old defaults after upgrade, so new features may need manual enabling

<sub>[Repo](https://github.com/yugabyte/yugabyte-db) · [📖 Docs ↗](https://docs.yugabyte.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yugabyte-db/)</sub>

<a name="mikro-orm"></a>
### #&#8288;96 [mikro-orm](https://github.com/mikro-orm/mikro-orm) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · MIT · Nov 2026</sub>

**TypeScript ORM for Node.js with Unit of Work and Identity Map.**

MikroORM is a Data Mapper ORM for TypeScript and Node.js that tracks entity changes through an Identity Map and Unit of Work, then writes them in one transaction on em.flush(). It has drivers for PostgreSQL, MySQL, MariaDB, SQLite, libSQL, MongoDB, MSSQL and Oracle. It is a general database library with no AI features, so it fits this list only as a data-layer dependency.

- **+** Drivers for ten databases, including PGlite, libSQL, MongoDB, MSSQL and Oracle
- **+** Unit of Work batches all tracked changes into one transaction on flush()
- **+** Includes migrations, schema generator, entity generator and seeding
- **+** Entities can be defined with defineEntity, decorators or EntitySchema
- **−** Not an AI project; no model, agent or LLM functionality
- **−** Needs RequestContext per request in web apps to isolate the identity map
- **−** Library only; no hosted backend, auth or storage layer
- **−** Separate driver package per database; extra packages need @mikro-orm/core installed explicitly

<sub>no GPU · Compose · Needs Node.js, PostgreSQL, MySQL, MariaDB, SQLite, libSQL, MongoDB, MSSQL or Oracle · [Repo](https://github.com/mikro-orm/mikro-orm) · [📖 Docs ↗](https://mikro-orm.io/docs/quick-start) · [🌐 Site ↗](https://mikro-orm.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mikro-orm/)</sub>

<a name="server"></a>
### #&#8288;97 [server](https://github.com/mariadb/server) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · GPL-2.0 · Nov 2026</sub>

**MySQL-compatible relational database server with built-in vector search.**

MariaDB Server is a relational database forked from MySQL that keeps wire-protocol and syntax compatibility. It offers pluggable storage engines (InnoDB, Aria, MyRocks, ColumnStore, Spider, S3), Galera multi-primary clustering, and a native VECTOR type with HNSW indexing since 11.8. It is a general-purpose database, not an AI-specific tool.

- **+** Native VECTOR type with HNSW index since 11.8, no extension needed
- **+** MySQL wire and syntax compatibility eases migration
- **+** Multiple storage engines, including ColumnStore for analytics and Spider for sharding
- **+** Yearly LTS releases maintained for three years
- **−** GPLv2 only, without the 'any later version' clause
- **−** Full database server, heavier to operate than embedded databases
- **−** Vector search requires version 11.8 or later
- **−** No embedding or model tooling included; vectors must be generated elsewhere

<sub>no GPU · [Repo](https://github.com/mariadb/server) · [📖 Docs ↗](https://mariadb.com/docs/) · [🌐 Site ↗](https://mariadb.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/server/)</sub>

<a name="vendure"></a>
### #&#8288;98 [vendure](https://github.com/vendurehq/vendure) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · custom license · Nov 2026</sub>

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

<a name="hatchet"></a>
### #&#8288;99 [hatchet](https://github.com/hatchet-dev/hatchet) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · MIT · Nov 2026</sub>

**Task queue and durable workflow engine for background jobs and AI agents.**

Hatchet runs background tasks, DAGs and durable workflows from Python, TypeScript, Go and Ruby SDKs. It stores task state and observability data in Postgres, and adds retries, cron, rate limits, priorities and a web UI with alerting. It can be self-hosted or used through Hatchet Cloud.

- **+** Postgres is the durability layer for both tasks and observability, so self-hosting needs no broker
- **+** Durable tasks, DAGs, cron, event triggers and webhooks in one engine
- **+** Concurrency keys, dynamic rate limits, priorities and worker slots for fair scheduling
- **+** OpenTelemetry, Prometheus metrics, multi-tenancy, users and roles included
- **−** README says it was load-tested to 10k tasks/second, below Redis or RabbitMQ queues
- **−** Uses more resources than Redis- or RabbitMQ-based queues because of durable history
- **−** SSO, autoscaling and multi-region are listed as Hatchet Cloud features
- **−** Local setup via the CLI requires Docker

<sub>no GPU · Compose · Needs Postgres, Docker (for local CLI setup) · [Repo](https://github.com/hatchet-dev/hatchet) · [📖 Docs ↗](https://docs.hatchet.run) · [🌐 Site ↗](https://hatchet.run) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hatchet/)</sub>

<a name="laravel-mongodb"></a>
### #&#8288;100 [laravel-mongodb](https://github.com/mongodb/laravel-mongodb) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · MIT · Nov 2026</sub>

**Eloquent model and query builder extensions for MongoDB in Laravel.**

Official MongoDB package that extends Laravel's Eloquent models and query builder so they run against MongoDB using the standard Laravel API. It extends the original Laravel classes, so existing method names apply. This is a general PHP database integration, and the README describes no AI features.

- **+** Extends Laravel's own Eloquent and query builder classes, so the same methods apply
- **+** Maintained by MongoDB, Inc., with documentation on mongodb.com
- **+** Release tags are GPG-signed with the PHP team's key
- **+** MIT license with recent releases (latest 2026-11-13)
- **−** No AI, LLM or vector search features described in the README
- **−** README states compatibility with Laravel 10.x; older versions need old branches
- **−** Issues are tracked in MongoDB's JIRA rather than GitHub issues
- **−** Needs a MongoDB server; it is a driver layer, not a backend or host

<sub>no GPU · Docker + Compose · Needs MongoDB, Laravel, PHP · [Repo](https://github.com/mongodb/laravel-mongodb) · [📖 Docs ↗](https://www.mongodb.com/docs/drivers/php/laravel-mongodb/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/laravel-mongodb/)</sub>

<a name="erupt"></a>
### #&#8288;101 [erupt](https://github.com/erupts/erupt) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Nov 2026</sub>

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

<a name="kong"></a>
### #&#8288;102 [kong](https://github.com/kong/kong) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Nov 2026</sub>

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

<a name="drizzle-orm"></a>
### #&#8288;103 [drizzle-orm](https://github.com/drizzle-team/drizzle-orm) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · Apache-2.0 · Nov 2026</sub>

**TypeScript ORM with SQL-like and relational queries for Postgres, MySQL and SQLite.**

Drizzle is a TypeScript ORM where you declare SQL schemas in code and query through either a SQL-like builder or a relational query API. It has zero dependencies, is about 7.4kb minified and gzipped, and runs on Node.js, Bun, Deno, Cloudflare Workers and in browsers. Drizzle Kit generates or applies migrations, and Drizzle Studio browses data. It contains no AI features.

- **+** Zero dependencies, about 7.4kb gzipped, tree shakeable
- **+** Covers PostgreSQL, MySQL and SQLite, including Neon, Turso, PlanetScale and Cloudflare D1
- **+** Runs on Node.js, Bun, Deno, edge runtimes and browsers without a Rust binary
- **+** Drizzle Kit handles migrations and Drizzle Studio gives a data browser
- **−** Not an AI project; it is a database layer only
- **−** No auth, storage or hosting, so it is not a full backend
- **−** Only PostgreSQL, MySQL and SQLite families are supported
- **−** Migrations and Studio need the separate Drizzle Kit tooling

<sub>no GPU · Needs PostgreSQL, MySQL or SQLite database · [Repo](https://github.com/drizzle-team/drizzle-orm) · [📖 Docs ↗](https://orm.drizzle.team/docs/overview) · [🌐 Site ↗](https://orm.drizzle.team) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/drizzle-orm/)</sub>

<a name="efcore"></a>
### #&#8288;104 [efcore](https://github.com/dotnet/efcore) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Nov 2026</sub>

**Object-database mapper for .NET with LINQ queries, change tracking and migrations.**

Entity Framework Core is Microsoft's ORM for .NET. It maps C# classes to tables, translates LINQ to SQL, tracks changes and manages schema migrations. Database support comes from provider packages (SQL Server, SQLite, Cosmos DB, and others). The repo also ships Microsoft.Data.Sqlite, an ADO.NET provider. It is not an AI project and fits this list only loosely.

- **+** LINQ queries, change tracking and schema migrations in one library
- **+** Provider plugin API covers SQL Server, SQLite, Cosmos DB, MySQL, PostgreSQL and more
- **+** Installed as NuGet packages; no server component to run
- **+** Includes Microsoft.Data.Sqlite, usable standalone as an ADO.NET provider
- **−** No AI, LLM or agent functionality; off-topic for this list
- **−** Library only: no auth, storage or API layer, so not a full backend
- **−** Tied to the .NET ecosystem and C#
- **−** README says official releases lag well behind daily builds

<sub>no GPU · Needs a .NET SDK, a database provider package such as SQL Server, SQLite or Cosmos DB · [Repo](https://github.com/dotnet/efcore) · [📖 Docs ↗](https://docs.microsoft.com/ef/core/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/efcore/)</sub>

<a name="nakama"></a>
### #&#8288;105 [nakama](https://github.com/heroiclabs/nakama) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Nov 2026</sub>

**Game and app backend with accounts, chat, leaderboards, matchmaking and multiplayer.**

Nakama is a Go server that provides user accounts, storage, friends and groups, chat, leaderboards, tournaments, parties, matchmaking and realtime or turn-based multiplayer. Logic is extended with Lua, TypeScript/JavaScript or Go modules. It exposes gRPC, REST and WebSocket APIs, ships an embedded web console, and needs CockroachDB or another Postgres wire-compatible database.

- **+** Single server binary with embedded admin console on port 7351
- **+** Runtime extensible in Lua, TypeScript/JavaScript or native Go
- **+** Official clients for Unity, Unreal, Godot, Defold, .NET, JavaScript, Java and Swift
- **+** Covers social, leaderboards, tournaments, matchmaker and purchase validation out of the box
- **−** Requires a separate CockroachDB or Postgres-compatible database
- **−** Aimed at games and social apps; no built-in AI features
- **−** Managed hosting is the vendor's Heroic Cloud service
- **−** Production sizing is vague: recommends n1-standard-1 on Google Cloud, no RAM figure

<sub>no GPU · Compose · Needs CockroachDB or Postgres wire-compatible database · port 7351 · [Repo](https://github.com/heroiclabs/nakama) · [📖 Docs ↗](https://heroiclabs.com/docs) · [🌐 Site ↗](https://heroiclabs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nakama/)</sub>

<a name="nhost"></a>
### #&#8288;106 [nhost](https://github.com/nhost/nhost) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · MIT · Nov 2026</sub>

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

<a name="exposed"></a>
### #&#8288;107 [exposed](https://github.com/jetbrains/exposed) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · Apache-2.0 · Nov 2026</sub>

**Kotlin ORM with a typesafe SQL DSL and DAO API over JDBC or R2DBC.**

Exposed is a JetBrains SQL library for Kotlin that offers a typesafe DSL wrapping SQL and a lightweight DAO API. It runs on JDBC or R2DBC (since 1.0.0) and supports H2, MariaDB, MySQL, Oracle, PostgreSQL, Redshift (JDBC only), SQL Server and SQLite. Extension modules cover date-time types, JSON, encryption, migrations, and Spring Boot 3 and 4 starters. It contains no AI features.

- **+** Supports both JDBC and R2DBC drivers, with separate migration modules for each
- **+** Eight database engines supported, so switching engines needs few or no code changes
- **+** Modular artifacts on Maven Central, including Spring Boot 3 and 4 starters
- **+** Both a SQL-like DSL and an entity-based DAO API are available
- **−** Kotlin-only library, requires Kotlin 2.2+ and a JVM
- **−** DAO over R2DBC (exposed-dao-r2dbc) is an experimental preview and its API may change
- **−** Redshift is supported over JDBC only, not R2DBC
- **−** Not an AI project and not a deployable backend service; it is a library only

<sub>no GPU · Needs Kotlin 2.2+, JDK 8+ (JDK 11+ for R2DBC, JDK 17+ for Spring modules), JDBC or R2DBC database driver · [Repo](https://github.com/jetbrains/exposed) · [📖 Docs ↗](https://www.jetbrains.com/help/exposed/home.html) · [🌐 Site ↗](https://www.jetbrains.com/exposed/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/exposed/)</sub>

<a name="che"></a>
### #&#8288;108 [che](https://github.com/eclipse-che/che) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.2k · EPL-2.0 · Nov 2026</sub>

**Kubernetes-hosted cloud development workspaces with a web IDE, defined by devfiles.**

Eclipse Che runs developer workspaces as pods on a Kubernetes cluster, bundling dependencies, containerized runtimes, a web IDE and project code. A workspace starts from a Git URL or a devfile.yaml, either through the browser factory URL or the chectl CLI. The instance is configured through the CheCluster custom resource. It has no AI features described in the README.

- **+** Opens any Git repository as a workspace via a factory URL
- **+** Devfile (schemaVersion 2.3.0) defines tools, images, memory limits and commands per project
- **+** Runs on any Kubernetes cluster; configured through the CheCluster custom resource
- **+** Embedded Open VSX extension registry and swappable editor definitions
- **−** Requires a Kubernetes cluster; no single-host or Docker Compose install in the README
- **−** No AI or coding-agent features, so it is a loose fit for this list
- **−** Operator-based administration adds overhead for small teams

<sub>Needs Kubernetes · [Repo](https://github.com/eclipse-che/che) · [📖 Docs ↗](https://eclipse.dev/che/docs) · [🌐 Site ↗](https://eclipse.dev/che/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/che/)</sub>

<a name="hexclave"></a>
### #&#8288;109 [hexclave](https://github.com/hexclave/hexclave) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · custom license · Nov 2026</sub>

**Auth, teams, payments, emails and analytics service for app users.**

Hexclave is a hosted or self-hosted service that handles user-related features for an app: authentication (passkeys, OAuth, CLI auth), teams with RBAC, API keys, payments, emails, analytics, webhooks and a data vault. It integrates through SDKs for Next.js, React and JS, and setup is done by pasting a prompt into a coding agent that reads skill.hexclave.com.

- **+** Auth, teams, RBAC, payments and emails share one user model
- **+** Auth methods and roles toggle from a dashboard without code changes
- **+** Available as hosted cloud or self-hosted
- **+** Agent-driven setup via a single prompt pointing at skill.hexclave.com
- **−** SDKs listed only for Next.js, React and JS
- **−** README badge says MIT / AGPLv3, but detected license is NOASSERTION
- **−** No self-hosting steps or Docker files in the README
- **−** Setup instructions are fetched from an external URL rather than the repo

<sub>no GPU · Docker · [Repo](https://github.com/hexclave/hexclave) · [📖 Docs ↗](https://docs.hexclave.com) · [🌐 Site ↗](https://hexclave.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hexclave/)</sub>

<a name="inngest"></a>
### #&#8288;110 [inngest](https://github.com/inngest/inngest) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · custom license · Nov 2026</sub>

**Durable step functions and event-driven job queue with a local dev server.**

Inngest runs background jobs and multi-step workflows by invoking your functions over HTTPS when events, cron schedules or webhooks fire. Each step is retried and its output persisted, so runs can last months. The Go server includes an event API, queue, executor and dashboard, and can be self-hosted or used through the hosted platform.

- **+** Per-step retries with persisted state, plus waitForEvent and cancelOn for long-running workflows
- **+** Flow control built in: concurrency keys, throttling, debouncing, rate limiting, prioritization, batching
- **+** SDKs for TypeScript, Python, Go and Kotlin/Java; SDKs are Apache 2.0
- **+** Local dev server starts with one npx command and serves a dashboard
- **−** Server and CLI use SSPL, converting to Apache 2.0 only after a delay
- **−** Not AI-specific; no model or agent tooling in the README
- **−** Self-hosting storage and queue requirements are not detailed in the README
- **−** Cloud sandboxes are experimental and need a paid hosted plan

<sub>no GPU · Docker · port 8288 · [Repo](https://github.com/inngest/inngest) · [📖 Docs ↗](https://www.inngest.com/docs) · [🌐 Site ↗](https://www.inngest.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/inngest/)</sub>

<a name="orpc"></a>
### #&#8288;111 [orpc](https://github.com/middleapi/orpc) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · MIT · Nov 2026</sub>

**TypeScript framework for typesafe APIs with OpenAPI output and MCP tools.**

oRPC lets you define API procedures as plain TypeScript functions with Zod, Valibot or ArkType input schemas. It gives you a typed client without code generation, an OpenAPI-compatible REST handler, and a package that exposes procedures as MCP tools. It runs on Node.js, Bun, Deno and Cloudflare Workers, with add-ons for Next.js, NestJS, TanStack Query, tRPC and OpenTelemetry.

- **+** Typed client inferred from the router, no code generation step
- **+** Same procedures serve RPC, OpenAPI REST and MCP tools
- **+** Runs on Node.js, Bun, Deno and Cloudflare Workers
- **+** Optional Redis and Upstash adapters for pub/sub, rate limiting and locking
- **−** TypeScript only; non-TS clients must go through the OpenAPI output
- **−** A library, not a starter app: no auth, billing or database included
- **−** Locking package is published as experimental (@orpc/experimental-lock)
- **−** Many separate npm packages to learn and keep in sync

<sub>no GPU · Needs Redis (optional), Upstash (optional) · Models: Zod, Valibot, ArkType · [Repo](https://github.com/middleapi/orpc) · [📖 Docs ↗](https://orpc.dev/docs/getting-started) · [🌐 Site ↗](https://orpc.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/orpc/)</sub>

<a name="cal-diy"></a>
### #&#8288;112 [cal.diy](https://github.com/calcom/cal.diy) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (95) · Freshness: active (93) · Maintenance: patchy (40) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · MIT · Nov 2026</sub>

**Self-hosted scheduling app, MIT fork of Cal.com without enterprise features.**

Cal.diy is a booking and scheduling web app built on Next.js, tRPC, Prisma and PostgreSQL. It is a fork of Cal.com with the enterprise code removed (Teams, Organizations, Insights, Workflows, SSO/SAML), so no license key is needed. It runs through Docker Compose or from source with yarn, and the README recommends it only for personal, non-production use.

- **+** Whole codebase is MIT, with no enterprise edition or license key
- **+** Docker Compose stack bundles the web app, Postgres and Prisma Studio
- **+** `yarn dx` starts a local Postgres and seeds test users for development
- **+** Calendar integrations can be added after setup from Settings > Integrations
- **−** README advises personal, non-production use only
- **−** Teams, Organizations, Workflows and SSO/SAML are removed
- **−** No hosted version; you run and secure the server yourself
- **−** Docker source build needs a live database and DOCKER_BUILDKIT=0

<sub>no GPU · Docker + Compose · Needs PostgreSQL >=13, Node.js >=18, Docker Compose, Daily.co (video) · port 3000 · [Repo](https://github.com/calcom/cal.diy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cal-diy/)</sub>

<a name="keystone"></a>
### #&#8288;113 [keystone](https://github.com/keystonejs/keystone) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · MIT · Nov 2026</sub>

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

<a name="databend"></a>
### #&#8288;114 [databend](https://github.com/databendlabs/databend) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (64) · Freshness: active (97) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · Apache-2.0 · Nov 2026</sub>

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

<a name="angularfire"></a>
### #&#8288;115 [angularfire](https://github.com/angular/angularfire) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

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

<a name="rainbond"></a>
### #&#8288;116 [rainbond](https://github.com/goodrain/rainbond) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · custom license · Nov 2026</sub>

**Self-hosted platform that deploys apps to Kubernetes through a web console.**

Rainbond is a Go container platform that builds and deploys applications on Kubernetes from source code, container images, Docker Compose, Helm or application templates, using a graphical console. It tracks application topology, upgrades and rollbacks, and offers a marketplace with one-click install and offline package export/import. It also targets private deployment of AI apps such as Dify or RAGFlow.

- **+** Deploys from source, images, Docker Compose, Helm or templates in one console
- **+** Marketplace with one-click install, upgrade and offline export/import
- **+** Manages topology, upgrades and rollbacks across multiple environments and clusters
- **+** Installs with one shell script; console served on port 7070
- **−** License is Rainbond Open Source License (Apache 2.0 plus extra conditions), not plain Apache
- **−** Exposes less Kubernetes detail, so cluster-level control is narrower than Rancher-style tools
- **−** Console, UI, operator and builder live in separate repositories
- **−** Recommended 8GB RAM and 50GB disk is heavy for a small single host

<sub>RAM ≥ 8 GB · no GPU · Docker · Needs Kubernetes · port 7070 · [Repo](https://github.com/goodrain/rainbond) · [▶️ Demo ↗](https://run.rainbond.com) · [📖 Docs ↗](https://www.rainbond.com/docs/) · [🌐 Site ↗](https://www.rainbond.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rainbond/)</sub>

<a name="openfga"></a>
### #&#8288;117 [openfga](https://github.com/openfga/openfga) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Nov 2026</sub>

**Fine-grained authorization server modeled on Google Zanzibar.**

OpenFGA is a Go authorization service that stores relationship tuples and evaluates permission checks against a user-defined authorization model. It exposes HTTP and gRPC APIs, and can also be embedded as a Go library. Storage is in-memory, PostgreSQL 14+, MySQL 8 or SQLite (beta).

- **+** HTTP and gRPC APIs with SDKs for Java, Node.js, Go, Python and .NET
- **+** Runs as one binary with in-memory storage, or on Postgres or MySQL
- **+** Local playground to model and test authorization; CLI for model tests
- **+** Used in production by Auth0 FGA since December 2021
- **−** Not an AI project; it only covers authorization, not auth or user management
- **−** In-memory storage loses data on stop and is for development only
- **−** MySQL backend has stricter length limits on tuple properties
- **−** Playground only connects to a server on localhost

<sub>no GPU · Docker + Compose · Needs PostgreSQL 14+ or MySQL 8 (optional, for persistent storage) · port 8080 · [Repo](https://github.com/openfga/openfga) · [📖 Docs ↗](https://openfga.dev/docs) · [🌐 Site ↗](https://openfga.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openfga/)</sub>

<a name="ministack"></a>
### #&#8288;118 [ministack](https://github.com/ministackorg/ministack) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Nov 2026</sub>

**Local AWS emulator exposing 60+ services on one port for dev and CI.**

MiniStack emulates more than 60 AWS services (S3, SQS, DynamoDB, Lambda, Step Functions, EC2 and others) behind a single endpoint on port 4566, working with boto3, the AWS CLI, Terraform, CDK and Pulumi. RDS, ElastiCache and ECS start real Docker containers, and Athena runs on DuckDB in the full image. Bedrock Converse and InvokeModel can be proxied to Ollama, llama.cpp or vLLM.

- **+** Idle footprint stated as ~30MB RAM, startup under 2 seconds
- **+** Account from 12-digit access key and per-region state isolation on one endpoint
- **+** Reset, health and message-inspection endpoints suit test suites and CI
- **+** Installs via pip, Docker image or compose; no account or API key
- **−** S3 and Aurora DSQL state is not isolated per region
- **−** RDS, ECS and Lambda containers need the Docker socket mounted
- **−** Athena and native Postgres/MySQL drivers require the larger full image
- **−** Not a backend to ship apps on; it only emulates AWS for testing

<sub>RAM ≥ 0.03 GB · no GPU · Docker + Compose · Needs Docker (optional, for RDS, ElastiCache, ECS, Lambda containers), Ollama, llama.cpp or vLLM (optional, for Bedrock proxy) · Models: Amazon Bedrock Converse/InvokeModel API, Ollama, llama.cpp, vLLM · port 4566 · [Repo](https://github.com/ministackorg/ministack) · [🌐 Site ↗](https://ministack.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ministack/)</sub>

<a name="easyadminbundle"></a>
### #&#8288;119 [easyadminbundle](https://github.com/easycorp/easyadminbundle) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Nov 2026</sub>

**Admin panel generator for Symfony apps built on Doctrine entities.**

EasyAdmin is a Symfony bundle that generates CRUD backends from Doctrine ORM entities using make:admin:dashboard and make:admin:crud commands. It provides search, filters, pagination, 30+ field types, and access control at dashboard, menu, action, field and entity level. It is not an AI project; the only AI feature is an installer command that adds an agent skill describing its API to coding agents.

- **+** Two console commands generate a working dashboard and CRUD from existing entities
- **+** Permissions can be set per dashboard, menu, action, field and entity
- **+** Supports Symfony 6.4, 7.x and 8.x; 5.x branch is stable, 4.x gets bug fixes
- **+** MIT-licensed core; installs an agent skill for Claude Code, Codex, Cursor and Copilot
- **−** Symfony and Doctrine ORM only; unusable with other PHP frameworks or non-Doctrine data layers
- **−** Audit log, content lock, Messenger inspector and Markdown field are in paid EasyAdmin Pro
- **−** Not an AI tool; fits this list only through its optional agent skill
- **−** Versions 3.x and earlier are no longer maintained

<sub>no GPU · Compose · Needs PHP 8.2+, Symfony 6.4+, Doctrine ORM, Composer · [Repo](https://github.com/easycorp/easyadminbundle) · [📖 Docs ↗](https://symfony.com/bundles/EasyAdminBundle/current/index.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/easyadminbundle/)</sub>

<a name="mongoid"></a>
### #&#8288;120 [mongoid](https://github.com/mongodb/mongoid) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Nov 2026</sub>

**Ruby object-document mapper for MongoDB, built on the official Ruby driver.**

Mongoid is an ODM that maps Ruby objects to MongoDB documents. It is built on the official MongoDB Ruby driver and maintained by MongoDB Inc. The README lists tested support for MRI 2.7 to 4.0, JRuby 9.4 and 10.0, and MongoDB server 3.6 to 8.2. It has no AI features.

- **+** Maintained by MongoDB Inc.; latest release dated 2026-11-12
- **+** Tested against MRI 2.7-4.0 and JRuby 9.4 and 10.0
- **+** Supports a wide MongoDB server range, 3.6 through 8.2
- **+** MIT license, with user and API docs hosted on mongodb.com
- **−** Ruby only, and works only with MongoDB, not other databases
- **−** Issues are tracked in MongoDB JIRA, not on GitHub
- **−** Not an AI project; README shows no model or LLM features
- **−** Library only: provides no auth, storage or hosting

<sub>no GPU · Needs MongoDB server 3.6 - 8.2, Ruby (MRI 2.7 - 4.0 or JRuby 9.4/10.0), MongoDB Ruby driver · [Repo](https://github.com/mongodb/mongoid) · [📖 Docs ↗](https://www.mongodb.com/docs/mongoid/current/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongoid/)</sub>

<a name="mongo-csharp-driver"></a>
### #&#8288;121 [mongo-csharp-driver](https://github.com/mongodb/mongo-csharp-driver) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Nov 2026</sub>

**Official MongoDB driver for .NET and C#, with typed and BSON document APIs.**

The official MongoDB client library for .NET/C#, distributed on NuGet as MongoDB.Driver. It connects through MongoClient and exposes async insert and find operations on collections, using either untyped BsonDocument or typed classes with lambda filters. It follows semantic versioning since v3.0.0. It is a database driver rather than an AI project, so it fits this list only loosely.

- **+** Maintained by MongoDB, with a release four days before the last commit
- **+** Supports both untyped BsonDocument and typed class collections with lambda filters
- **+** Async API for insert and find operations
- **+** Semantic versioning since v3.0.0 makes upgrades predictable
- **−** Client library only; needs a separate MongoDB server to be useful
- **−** No AI, LLM or vector search features described in the README
- **−** Bug reports go to Jira rather than GitHub issues
- **−** Works only with MongoDB, not other databases

<sub>no GPU · Compose · Needs MongoDB server · [Repo](https://github.com/mongodb/mongo-csharp-driver) · [📖 Docs ↗](https://www.mongodb.com/docs/drivers/csharp/current/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongo-csharp-driver/)</sub>

<a name="teable"></a>
### #&#8288;122 [teable](https://github.com/teableio/teable) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

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
### #&#8288;123 [dgraph](https://github.com/dgraph-io/dgraph) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

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

<a name="adonisjs-core"></a>
### #&#8288;124 [adonisjs/core](https://github.com/adonisjs/core) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

**TypeScript MVC web framework for Node.js apps and APIs.**

AdonisJS core is the main package of a fullstack MVC web framework for Node.js, written in TypeScript. The README describes it as a framework for building web apps and micro services behind a stable API. It has no AI features of its own, so it works only as a backend base that you add model calls to.

- **+** Written in TypeScript, published on npm as @adonisjs/core
- **+** MIT license, with a release on 2026-10-05 and recent commits
- **+** Covers both server-rendered web apps and micro services
- **+** Separate guides site at docs.adonisjs.com
- **−** No built-in AI, LLM or agent features in this package
- **−** README has no install steps, feature list or version requirements
- **−** Not an AI starter, so model wiring and billing are yours to add
- **−** No Dockerfile or compose file in the repo

<sub>no GPU · Needs Node.js · [Repo](https://github.com/adonisjs/core) · [📖 Docs ↗](https://docs.adonisjs.com) · [🌐 Site ↗](https://adonisjs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/adonisjs-core/)</sub>

<a name="diesel"></a>
### #&#8288;125 [diesel](https://github.com/diesel-rs/diesel) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Nov 2026</sub>

**Type-checked ORM and query builder for Rust.**

Diesel is a Rust crate that builds SQL queries through the type system, so malformed queries and column type mismatches fail at compile time. It supports PostgreSQL, MySQL, SQLite and MariaDB, selected by a Cargo feature. Derive macros map structs to rows and insert or update payloads, and a raw SQL API covers queries the builder cannot express. It is not an AI project.

- **+** Query errors are caught at compile time through Rust's type system
- **+** Derive macros (Queryable, Insertable, Selectable) remove manual row mapping
- **+** Supports PostgreSQL, MySQL, SQLite and MariaDB behind Cargo features
- **+** Raw SQL escape hatch via sql_query with bound parameters
- **−** Library only: no auth, storage or hosting, so it is not a full backend
- **−** No AI or LLM features; it fits this list only loosely
- **−** Rust only; the README shows no async API
- **−** Heavy generic types can make compile errors hard to read

<sub>no GPU · Compose · Needs PostgreSQL, MySQL, MariaDB or SQLite · [Repo](https://github.com/diesel-rs/diesel) · [📖 Docs ↗](https://docs.diesel.rs/main/diesel/index.html) · [🌐 Site ↗](https://diesel.rs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diesel/)</sub>

<a name="cakephp"></a>
### #&#8288;126 [cakephp](https://github.com/cakephp/cakephp) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.8k · MIT · Nov 2026</sub>

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
### #&#8288;127 [graphql-yoga](https://github.com/graphql-hive/graphql-yoga) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · MIT · Nov 2026</sub>

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

<a name="aspire"></a>
### #&#8288;128 [aspire](https://github.com/microsoft/aspire) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Nov 2026</sub>

**Code-first toolchain to define, run and deploy distributed apps.**

Aspire lets you describe services, frontends, containers, databases and caches in an app definition written in C# (apphost.cs) or TypeScript (apphost.ts). The Aspire CLI runs the whole app locally with OpenTelemetry-based observability and reuses the same definition for deployment. The repo holds the CLI, AppHost SDK, dashboard, service discovery, project templates, integrations and a VS Code extension.

- **+** One app definition in C# or TypeScript covers local run and deployment
- **+** Includes a dashboard and OpenTelemetry-based observability
- **+** Ships CLI, project templates, integrations and a VS Code extension
- **+** MIT license with recent commits and releases
- **−** Not AI-specific; no model, agent or LLM tooling described
- **−** Container integrations are third-party; users must vet their security
- **−** Orchestrates apps; it is not a backend with its own auth or database
- **−** Only C# and TypeScript app definitions are shown

<sub>[Repo](https://github.com/microsoft/aspire) · [📖 Docs ↗](https://aspire.dev/docs/) · [🌐 Site ↗](https://aspire.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aspire/)</sub>

<a name="uncloud"></a>
### #&#8288;129 [uncloud](https://github.com/psviderski/uncloud) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · Apache-2.0 · Nov 2026</sub>

**Multi-machine container orchestrator over a WireGuard mesh, with no control plane.**

Uncloud connects Docker hosts (cloud VMs or bare metal) into a WireGuard mesh and deploys Compose-format services across them. Cluster state is shared peer-to-peer via Corrosion (CRDT-backed SQLite), so there is no central control plane or quorum. It includes DNS-based service discovery, a Caddy reverse proxy with Let's Encrypt HTTPS, and a Docker-like `uc` CLI that works over SSH.

- **+** No control plane or quorum; any machine holds full cluster state
- **+** Uses Compose files and a Docker-like CLI, no new DSL
- **+** Built-in Caddy ingress with automatic HTTPS and rolling updates
- **+** Pushes images directly to machines via Unregistry, sending only missing layers
- **−** Pre-1.0; README warns of occasional breaking changes between releases
- **−** Automatic rollback on failed deploys is not implemented yet
- **−** Imperative model, no state reconciliation like Kubernetes
- **−** Targets Docker hosts reached over SSH; non-root users need sudo

<sub>no GPU · Docker · Needs Docker, WireGuard, Caddy, Corrosion, SSH access to machines, Systemd · [Repo](https://github.com/psviderski/uncloud) · [▶️ Demo ↗](https://labs.iximiuz.com/playgrounds/uncloud-cluster-64523f7c) · [📖 Docs ↗](https://uncloud.run/docs) · [🌐 Site ↗](https://uncloud.run) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/uncloud/)</sub>

<a name="restate"></a>
### #&#8288;130 [restate](https://github.com/restatedev/restate) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · custom license · Nov 2026</sub>

**Durable execution engine for workflows, services and AI agents.**

Restate is a server written in Rust that persists the execution progress of your handlers, so failed code retries without re-running completed steps. It provides exactly-once messaging, durable promises and timers, and per-entity key-value state, with SDKs for TypeScript, Java/Kotlin, Python, Go and Rust. It is a backend runtime for workflows and agents rather than an AI-specific framework.

- **+** SDKs for TypeScript, Java/Kotlin, Python, Go and Rust
- **+** Retries resume from recorded steps instead of re-executing completed work
- **+** Built-in UI, CLI and OpenTelemetry traces for inspecting invocations
- **+** Installs via Homebrew, npx or Docker; automatic data migration between x.y releases
- **−** Adds a separate server your services must register with and be invoked through
- **−** License is reported as NOASSERTION, so terms need checking before use
- **−** AI agent support lives in a separate examples repo, not this one
- **−** Handlers must follow the SDK's durable execution model, which changes how code is written

<sub>no GPU · Docker · port 9070 · [Repo](https://github.com/restatedev/restate) · [📖 Docs ↗](https://docs.restate.dev) · [🌐 Site ↗](https://restate.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/restate/)</sub>

<a name="ravendb"></a>
### #&#8288;131 [ravendb](https://github.com/ravendb/ravendb) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · custom license · Nov 2026</sub>

**ACID-compliant NoSQL document database with a built-in web studio.**

RavenDB is a document-oriented NoSQL database written in C# with fully ACID transactions and a built-in web UI, the Management Studio. It runs on Linux, macOS, Windows, containers and Raspberry Pi, and is also sold as a hosted service, RavenDB Cloud. Official client SDKs exist for .NET, Node.js, Python, Java, PHP, Go, C++ and Ruby.

- **+** Fully ACID transactions, with security on by default
- **+** Official clients for eight languages, including .NET, Python, Java and Go
- **+** Management Studio web UI ships with the server
- **+** Installs from a download, .deb package or Docker image
- **−** README says AGPLv3, but detected license is NOASSERTION, so terms need checking
- **−** README links a developer license request, so some use may need a license
- **−** Database only: no auth, file storage or API layer for apps
- **−** Not an AI project: no model or vector features described in README

<sub>no GPU · Docker · port 8080 · [Repo](https://github.com/ravendb/ravendb) · [▶️ Demo ↗](http://live-test.ravendb.net/) · [📖 Docs ↗](https://ravendb.net/docs) · [🌐 Site ↗](https://ravendb.net/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ravendb/)</sub>

<a name="django"></a>
### #&#8288;132 [django](https://github.com/django/django) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 92k · BSD-3-Clause · Nov 2026</sub>

**High-level Python web framework for building web backends.**

Django is a general-purpose Python web framework. The README points to the docs: an install guide, ordered tutorials, topical guides, HOWTOs, a reference and a deployment guide. It has no AI features of its own, so it is a backend base to build on, not an AI starter.

- **+** Documentation covers install, ordered tutorials, topical guides, HOWTOs, reference and deployment
- **+** Written in Python, so it sits alongside Python AI libraries
- **+** BSD-3-Clause license; last commit 2026-11-11
- **+** Support via Discord, Forum and a public ticket tracker
- **−** No built-in AI, LLM or model-serving features; add them yourself
- **−** No tagged release listed in the repository metadata
- **−** Not a ready-made starter; the app is built by following the tutorials
- **−** No Docker or Compose files in the repository

<sub>[Repo](https://github.com/django/django) · [📖 Docs ↗](https://docs.djangoproject.com/en/stable/) · [🌐 Site ↗](https://www.djangoproject.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/django/)</sub>

<a name="scylladb"></a>
### #&#8288;133 [scylladb](https://github.com/scylladb/scylladb) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · custom license · Nov 2026</sub>

**Cassandra- and DynamoDB-compatible distributed database written in C++ on Seastar.**

ScyllaDB is a distributed NoSQL database that speaks CQL (the Apache Cassandra API) by default and offers an optional DynamoDB-compatible API called Alternator. It uses a shared-nothing, per-core design built on the Seastar framework. The repo is the database server itself, not an AI starter, so it fits this list only as backend infrastructure.

- **+** CQL compatibility with Apache Cassandra drivers and tooling
- **+** Optional DynamoDB API (Alternator), enabled through configuration
- **+** Shared-nothing, per-core architecture built on Seastar
- **+** Free hands-on courses available through Scylla University
- **−** Not an AI project; README mentions no model, vector or LLM features
- **−** Building needs a very recent C++23 toolchain; frozen Docker toolchain recommended
- **−** README gives build-from-source steps only, no packaged install or Docker run
- **−** License is reported as NOASSERTION; check the repo license files

<sub>no GPU · Needs Docker or Podman (frozen build toolchain), C++23 compiler, ninja · [Repo](https://github.com/scylladb/scylladb) · [📖 Docs ↗](https://docs.scylladb.com/) · [🌐 Site ↗](https://www.scylladb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scylladb/)</sub>

<a name="pressly-goose"></a>
### #&#8288;134 [pressly/goose](https://github.com/pressly/goose) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Nov 2026</sub>

**Database schema migration tool for Go, as CLI and library.**

Goose applies versioned schema changes written as SQL files or Go functions, tracking state in a migrations table (default goose_db_version). It runs as a CLI or is imported as a Go library, with commands such as up, down, redo, status, fix and validate. Drivers include Postgres, MySQL, SQLite, ClickHouse, MSSQL, Spanner, YDB and others.

- **+** Supports SQL and Go migrations, plus migrations embedded in the binary via go:embed
- **+** Many drivers: Postgres, MySQL, SQLite, Spanner, MSSQL, ClickHouse, YDB, Redshift, TiDB
- **+** Build tags (e.g. no_postgres) strip unused drivers for a smaller binary
- **+** Out-of-order migrations, env var substitution in SQL, and a fix command for sequential numbering
- **−** Go migrations require building your own goose binary; the stock CLI runs SQL only
- **−** Container image has no shell and supports .sql migrations only
- **−** ClickHouse is only fully supported in some deployment modes
- **−** MySQL needs parseTime and multiStatements enabled for status and multi-statement files

<sub>no GPU · Docker · Needs A supported database (Postgres, MySQL, SQLite, etc.) · [Repo](https://github.com/pressly/goose) · [📖 Docs ↗](https://pressly.github.io/goose/installation/) · [🌐 Site ↗](https://pressly.github.io/goose/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pressly-goose/)</sub>

<a name="cloudnative-pg"></a>
### #&#8288;135 [cloudnative-pg](https://github.com/cloudnative-pg/cloudnative-pg) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · Apache-2.0 · Nov 2026</sub>

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

<a name="servicestack"></a>
### #&#8288;136 [servicestack](https://github.com/servicestack/servicestack) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · custom license · Nov 2026</sub>

**.NET web services framework with message-based DTO APIs and typed clients.**

ServiceStack is a C# framework for building web services from typed request DTOs. It serves JSON, XML, CSV, ProtoBuf, MsgPack and SOAP, and adds Auto Query over OrmLite-supported databases, plus RabbitMQ, Redis and SQS message hosts. Typed clients for C#, TypeScript, Swift, Java, Kotlin and Dart come from the server DTOs. The README describes no AI features.

- **+** Auto Query builds queryable APIs from a single request DTO across major RDBMS
- **+** Typed clients for C#, TypeScript, Swift, Java, Kotlin and Dart from server DTOs
- **+** Many wire formats built in: JSON, XML, CSV, JSV, ProtoBuf, MsgPack, SOAP
- **+** Message queue hosts for RabbitMQ, Redis and Amazon SQS
- **−** Source is AGPL with FOSS exception; v4+ NuGet packages are commercial with free quotas
- **−** No AI, LLM or agent functionality described in the README
- **−** README is dated: references Silverlight, Xamarin Studio and Google+
- **−** Server side is C#/.NET only

<sub>no GPU · Docker + Compose · Needs NuGet, RDBMS via OrmLite (optional), RabbitMQ (optional), Redis (optional), Amazon SQS (optional) · [Repo](https://github.com/servicestack/servicestack) · [📖 Docs ↗](https://docs.servicestack.net) · [🌐 Site ↗](https://servicestack.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/servicestack/)</sub>

<a name="opennextjs-aws"></a>
### #&#8288;137 [opennextjs-aws](https://github.com/opennextjs/opennextjs-aws) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Nov 2026</sub>

**Adapter that packages Next.js build output for AWS Lambda or Node servers.**

OpenNext takes the Next.js build output and converts it into packages deployable on AWS Lambda or a classic Node.js server. It covers App and Pages Router, ISR, middleware, server actions and image optimization, and is configured through an optional open-next.config.ts. It also ships a warmer function to reduce Lambda cold starts.

- **+** Supports App and Pages Router, ISR, middleware, server actions and image optimization
- **+** Runs without a config file; defaults apply when open-next.config.ts is absent
- **+** Includes a warmer function to reduce Lambda cold starts
- **+** Prerelease packages published on every push to main via pkg.pr.new
- **−** Targets Next.js 15; some features are listed as work in progress
- **−** Native support limited to AWS Lambda and Node.js server
- **−** Warmer does not remove all cold starts, such as lazy-loaded routes
- **−** Debug mode can make output 2-3x larger

<sub>no GPU · Needs Next.js, AWS Lambda, Node.js · [Repo](https://github.com/opennextjs/opennextjs-aws) · [📖 Docs ↗](https://opennext.js.org/aws) · [🌐 Site ↗](https://opennext.js.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opennextjs-aws/)</sub>

<a name="cockroach"></a>
### #&#8288;138 [cockroach](https://github.com/cockroachdb/cockroach) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · custom license · Sep 2026</sub>

**Distributed SQL database with horizontal scaling and Postgres wire support.**

CockroachDB is a distributed SQL database written in Go, built on a transactional, strongly consistent key-value store. It scales horizontally, keeps serving through disk, machine, rack and datacenter failures, and speaks the PostgreSQL wire protocol so existing drivers and ORMs connect. It is a general-purpose database with no AI features, so it fits this list only as a backend to ship apps on.

- **+** Serializable ACID transactions across a horizontally scaled cluster
- **+** Survives disk, machine, rack and datacenter failures without manual intervention
- **+** PostgreSQL wire protocol, so standard Postgres drivers and ORMs work
- **+** Built-in SQL client, plus a managed CockroachCloud option
- **−** Releases since v24.3 use the CockroachDB Software License, not an OSI open-source license
- **−** Compatibility with Postgres is at the wire protocol and SQL level, not identical
- **−** Multi-node cluster deployment is more operational work than a single-node database
- **−** No AI or LLM features described in the README

<sub>no GPU · [Repo](https://github.com/cockroachdb/cockroach) · [📖 Docs ↗](https://cockroachlabs.com/docs/stable/) · [🌐 Site ↗](https://www.cockroachlabs.com/product/overview/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cockroach/)</sub>

<a name="influxdb"></a>
### #&#8288;139 [influxdb](https://github.com/influxdata/influxdb) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Oct 2026</sub>

**Time series database for real-time ingest and SQL queries over Parquet.**

InfluxDB 3 Core is a time series database written in Rust on Apache Arrow and DataFusion. It ingests line protocol, persists data as Parquet on object storage (S3, Azure, GCP) or local disk, and answers SQL, InfluxQL or Flight SQL queries over HTTP on port 8181. It also embeds a Python VM for plugins and triggers.

- **+** Runs on local disk with no dependencies, or on S3, Azure or GCP object storage
- **+** Accepts InfluxDB 1.x and 2.x write APIs and the 1.x InfluxQL query API
- **+** Embedded Python VM for plugins and triggers
- **+** Data persisted as open Parquet files, queryable via SQL, InfluxQL and Flight SQL
- **−** Flux is not supported on this branch; it exists only in the v2.x and v1.x branches
- **−** A separate InfluxDB 3 Enterprise edition exists; README does not list the feature differences
- **−** Not an AI project; fits this list only as a general-purpose backend
- **−** Other InfluxDB versions live on separate branches, so the main branch covers v3 only

<sub>no GPU · Docker · port 8181 · [Repo](https://github.com/influxdata/influxdb) · [📖 Docs ↗](https://docs.influxdata.com/influxdb3/core/) · [🌐 Site ↗](https://www.influxdata.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/influxdb/)</sub>

<a name="shardingsphere"></a>
### #&#8288;140 [shardingsphere](https://github.com/apache/shardingsphere) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (82) · Freshness: active (93) · Maintenance: patchy (49) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

**Sharding, read/write splitting and encryption layer over existing SQL databases.**

ShardingSphere adds data sharding, read/write splitting, distributed transactions, encryption, masking and SQL federation on top of existing databases such as MySQL, PostgreSQL, Oracle and SQL Server. It ships as ShardingSphere-JDBC, a Java driver delivered as a JAR, and ShardingSphere-Proxy, a standalone server speaking the MySQL and PostgreSQL protocols. It is database middleware with no AI functionality, so it fits this list only loosely.

- **+** JDBC mode needs no extra deployment; it is a JAR compatible with MyBatis, JPA and Hibernate
- **+** Proxy mode serves any MySQL or PostgreSQL protocol client, so non-Java stacks can use it
- **+** Pluggable micro-kernel; sharding, encryption and masking are separate features you combine as needed
- **+** Apache top-level project since 2020; registry integration with ZooKeeper and ETCD
- **−** No AI or LLM features; it is database middleware, a weak fit for this list
- **−** README warns the ANTLR SQL parse cache can grow and cause OOM in JDBC mode
- **−** JDBC adapter is Java only; other languages must run the separate Proxy
- **−** Adds a routing layer in front of databases, which adds operational complexity

<sub>no GPU · Needs Java, MySQL, PostgreSQL, Oracle, SQL Server or other supported database, ZooKeeper or ETCD (registry center, optional) · [Repo](https://github.com/apache/shardingsphere) · [📖 Docs ↗](https://shardingsphere.apache.org/document/current/en/overview/) · [🌐 Site ↗](https://shardingsphere.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shardingsphere/)</sub>

<a name="insforge"></a>
### #&#8288;141 [insforge](https://github.com/insforge/insforge) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

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

<a name="encore"></a>
### #&#8288;142 [encore](https://github.com/encoredev/encore) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MPL-2.0 · Nov 2026</sub>

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
### #&#8288;143 [trailbase](https://github.com/trailbaseio/trailbase) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · OSL-3.0 · Nov 2026</sub>

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

<a name="go-whatsapp-web-multidevice"></a>
### #&#8288;144 [go-whatsapp-web-multidevice](https://github.com/aldinokemal/go-whatsapp-web-multidevice) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Nov 2026</sub>

**Go server exposing WhatsApp multi-device over REST, webhooks and MCP.**

GoWA is a Go service built on whatsmeow that links one or more WhatsApp accounts as devices and exposes them through a REST API, per-device webhooks and an MCP endpoint at /mcp. It sends text, media, stickers, status updates and scheduled or recurring messages, and handles newsletter channels. Sessions can be stored in PostgreSQL, and the web dashboard lives in a separate repo (gowa-ui) that the server downloads at startup.

- **+** Multiple WhatsApp accounts in one instance, scoped by X-Device-Id header or device_id parameter
- **+** REST, MCP and webhooks served from one `./whatsapp rest` process
- **+** Webhooks are HMAC-SHA-256 signed, with event-type and JID filtering and per-device URLs
- **+** Scheduled and recurring sends persist across restarts; n8n node and Chatwoot guide included
- **−** Relies on the unofficial WhatsApp Web protocol via whatsmeow; changes can break it
- **−** Interactive messages are experimental; recipient compatibility varies
- **−** Dashboard is downloaded from a separate repo at startup, complicating air-gapped setups
- **−** Scheduled sends are not exactly-once; live newsletter subscriptions are lost on restart

<sub>no GPU · Docker + Compose · Needs WhatsApp account, PostgreSQL (optional, e.g. Neon) · port 3000 · [Repo](https://github.com/aldinokemal/go-whatsapp-web-multidevice) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-whatsapp-web-multidevice/)</sub>

<a name="devpush"></a>
### #&#8288;145 [devpush](https://github.com/hunvreus/devpush) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Nov 2026</sub>

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

<a name="pg-boss"></a>
### #&#8288;146 [pg-boss](https://github.com/timgit/pg-boss) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Nov 2026</sub>

**Postgres-backed job queue for Node.js using SKIP LOCKED.**

pg-boss is a Node.js library that stores background jobs in PostgreSQL and uses SKIP LOCKED so concurrent workers claim jobs without blocking each other. It supports retries with backoff, priority and dead letter queues, cron and RRULE scheduling, job dependencies, and enqueueing inside an existing database transaction. It is a general job queue with no AI-specific features, so it fits as infrastructure under an AI app.

- **+** No separate broker: jobs live in the Postgres you already run
- **+** Can enqueue jobs in an existing transaction; adapters for Drizzle, Knex, Kysely, Prisma
- **+** Retries with exponential backoff, dead letter queues with redrive, cron and RRULE scheduling
- **+** Optional CLI for migrations, web dashboard, HTTP proxy and OpenTelemetry traces and metrics
- **−** Requires PostgreSQL 13+ and Node 22.12+ or Bun
- **−** Maintained by a single person, per the README
- **−** Throughput is bounded by Postgres; no numbers given
- **−** Not an AI tool; no model, agent or LLM integration

<sub>no GPU · Compose · Needs PostgreSQL 13+, Node.js 22.12+ or Bun · [Repo](https://github.com/timgit/pg-boss) · [📖 Docs ↗](https://pgboss.io/) · [🌐 Site ↗](https://pgboss.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pg-boss/)</sub>

<a name="graphjin"></a>
### #&#8288;147 [graphjin](https://github.com/dosco/graphjin) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="convex-backend"></a>
### #&#8288;148 [convex-backend](https://github.com/convex/convex-backend) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · custom license · Nov 2026</sub>

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

<a name="cassandra"></a>
### #&#8288;149 [cassandra](https://github.com/apache/cassandra) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · Apache-2.0 · Nov 2026</sub>

**Distributed partitioned row-store database queried with CQL.**

Apache Cassandra is a partitioned row-store database written in Java. Tables require a primary key, data is distributed across machines automatically, and the cluster repartitions as nodes are added or removed. It is queried with CQL, which the README describes as SQL minus joins and subqueries, plus collections.

- **+** Automatic partitioning across machines, repartitions when nodes are added or removed
- **+** CQL syntax is close to SQL, with a bundled cqlsh client
- **+** Runs as a single node from a tarball for local testing
- **+** Apache-2.0 licensed with Jira, mailing lists and Slack for support
- **−** CQL has no joins or subqueries, so data modeling differs from relational databases
- **−** Not an AI project; the README describes no model or vector features
- **−** Needs a Java runtime and Python for cqlsh; supported versions only in build.xml
- **−** No tagged release listed; README banner shows a 7.0-SNAPSHOT trunk build

<sub>no GPU · Needs Java, Python (for cqlsh) · [Repo](https://github.com/apache/cassandra) · [📖 Docs ↗](https://cassandra.apache.org/doc/latest/cassandra/getting-started/index.html) · [🌐 Site ↗](https://cassandra.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cassandra/)</sub>

<a name="kubevela"></a>
### #&#8288;150 [kubevela](https://github.com/kubevela/kubevela) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · Apache-2.0 · Nov 2026</sub>

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

<a name="pig"></a>
### #&#8288;151 [pig-mesh/pig](https://github.com/pig-mesh/pig) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · Apache-2.0 · Nov 2026</sub>

**Spring Cloud RBAC admin platform with OAuth2 auth, gateway and code generation.**

Pig is a Java 17 admin backend built on Spring Boot 4.1 and Spring Cloud, with a Vue 3 and Element Plus frontend in the separate pig-ui repo. It includes an OAuth2 authorization server, Spring Cloud Gateway, user and permission management, monitoring, a code generator and a Quartz job console. It runs as microservices or as a single pig-boot application. It has no AI features.

- **+** Same codebase builds as microservices (-Pcloud) or a single app (-Pboot)
- **+** Auth uses Spring Authorization Server: authorization code, password and refresh token flows
- **+** Docker Compose files start MySQL, Redis, Nacos and the services
- **+** Includes a graphical code generator and a Quartz job console
- **−** Multi-tenancy, data permissions, dynamic routing and workflow are only in the commercial edition
- **−** Microservice mode needs MySQL, Redis and Nacos running
- **−** README and docs are in Chinese
- **−** Frontend lives in a separate repo and needs Node.js 20.19+

<sub>no GPU · Compose · Needs MySQL, Redis, Nacos, JDK 17+, Maven 3.9+, Docker Compose · port 9999 · [Repo](https://github.com/pig-mesh/pig) · [📖 Docs ↗](https://docs.pig4cloud.com/open) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pig/)</sub>

<a name="terminusdb"></a>
### #&#8288;152 [terminusdb](https://github.com/terminusdb/terminusdb) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · Apache-2.0 · Nov 2026</sub>

**Knowledge graph database with git-style branch, diff and merge for JSON.**

TerminusDB stores linked JSON and JSON-LD documents as a knowledge graph and records a commit for every update. It supports branch, merge, diff, patch, push/pull/clone and time-travel queries, and exposes a document REST API, GraphQL and WOQL, a datalog query language. The 12.1 release candidate adds built-in vector search.

- **+** Commit per update, with diff and patch between commits and queries at any historical commit
- **+** Three query interfaces: REST document API, GraphQL and WOQL datalog with path queries
- **+** Schema constraints and arbitrary-precision xsd:decimal for data-quality-sensitive use
- **+** Official Python and JavaScript clients; docker-compose.yml included
- **−** Written in Prolog, which makes contributing harder for most teams
- **−** Full JSON-LD, Turtle and RDF/XML, clustering and faster writes are Enterprise-only
- **−** Built-in vector search is only in the 12.1 release candidate, not a final release
- **−** WOQL is a niche query language with its own learning curve

<sub>no GPU · Docker + Compose · Needs Docker · port 6363 · [Repo](https://github.com/terminusdb/terminusdb) · [📖 Docs ↗](https://terminusdb.com/docs) · [🌐 Site ↗](https://terminusdb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terminusdb/)</sub>

<a name="apollo-server"></a>
### #&#8288;153 [apollo-server](https://github.com/apollographql/apollo-server) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

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

<a name="openstatus"></a>
### #&#8288;154 [openstatus](https://github.com/openstatushq/openstatus) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · AGPL-3.0 · Nov 2026</sub>

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

<a name="luban"></a>
### #&#8288;155 [luban](https://github.com/focus-creative-games/luban) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

**Game config pipeline that turns Excel, JSON and XML tables into typed code and data.**

Luban is a C# tool that reads game configuration tables (csv, xls/xlsx, json, xml, yaml, lua) and generates typed loader code and exported data. It targets many languages, including C#, Java, Go, C++, Lua, TypeScript and Rust, and exports binary, json, bson, xml, lua or yaml. Since 5.0.0 it also ships Agent skills, a Luban.Agent CLI and a Luban.Mcp server for IDE tool calls.

- **+** Supports type inheritance, so nested data like skills and behavior trees fits the schema
- **+** Built-in validation: ref checks, resource path checks and range checks
- **+** Generates code for 12+ languages with no reflection, compatible with obfuscators
- **+** Ships MCP server, Agent CLI, and JSON schema and error output for agents
- **−** Main README is in Chinese; English version is a separate file
- **−** Scoped to game configuration, not a general-purpose backend or database
- **−** Needs a custom schema and extended Excel header conventions to adopt
- **−** Test and build setup relies on the .NET toolchain

<sub>no GPU · [Repo](https://github.com/focus-creative-games/luban) · [📖 Docs ↗](https://www.datable.cn/docs/intro) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/luban/)</sub>

<a name="lakesoul"></a>
### #&#8288;156 [lakesoul](https://github.com/lakesoul-io/lakesoul) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Nov 2026</sub>

**Lakehouse on object storage with a PostgreSQL wire endpoint and vector search.**

LakeSoul is a Rust lakehouse engine that stores Parquet or Vortex files in S3, OSS or HDFS, with table metadata in PostgreSQL. It exposes a PostgreSQL wire endpoint supporting DDL, upsert, COPY and transactions, plus pgvector-style ANN queries, BM25 search, federated foreign tables, CDC subscriptions and incremental SQL. A Python SDK reads the same tables into Arrow, Daft, Ray or PyTorch.

- **+** Standard PostgreSQL clients (psql, JDBC, psycopg, DBeaver) connect without a custom driver
- **+** Vector (IVF + RaBitQ) and BM25 indexes are maintained on write, in the same plan as filters
- **+** Built-in PostgreSQL and MySQL CDC subscriptions and ADBC federation to BigQuery, Snowflake, Trino and others
- **+** Primary-key upsert with merge-on-read; Spark 3.5, Flink 1.20 and Presto 0.296 integrations listed
- **−** Requires a separate PostgreSQL metadata database plus object storage; not a single binary
- **−** Quick start builds from source with cargo; no Docker image or compose file for the engine
- **−** SQL surface is a subset of PostgreSQL, tracked in a separate compatibility matrix
- **−** Positioned as an analytics lakehouse, not a drop-in OLTP or app backend with auth and APIs

<sub>Docker + Compose · Needs PostgreSQL (metadata), Object storage (S3/OSS/HDFS) · [Repo](https://github.com/lakesoul-io/lakesoul) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lakesoul/)</sub>

<a name="omnigraph"></a>
### #&#8288;157 [omnigraph](https://github.com/modernrelay/omnigraph) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Nov 2026</sub>

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

<a name="supabase-py"></a>
### #&#8288;158 [supabase-py](https://github.com/supabase/supabase-py) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

**Python client libraries for Supabase auth, database, storage, functions and realtime.**

Monorepo of the official Python SDKs for Supabase services: supabase, supabase_auth, postgrest, storage3, supabase_functions, realtime and supabase_utils. It targets Python 3.12 and later, is pure Python, and is tested on Linux. The main branch holds v3, which is in early development; v2 on its own branch only gets critical and security fixes.

- **+** Covers auth, PostgREST, storage, edge functions and realtime as separate packages
- **+** Pure Python, expected to run on any CPython platform
- **+** Supported Python versions are defined and tested in CI
- **+** MIT licensed, with a release in November 2026
- **−** Main branch is v3, in early development; no external issues or contributions accepted
- **−** v2 branch receives only critical bug and security fixes
- **−** Compatibility guaranteed only with the latest release of each Supabase service
- **−** Requires Python 3.12 or newer; PyPy is untested

<sub>no GPU · Needs Supabase project or self-hosted Supabase services, Python 3.12+ · [Repo](https://github.com/supabase/supabase-py) · [📖 Docs ↗](https://supabase.com/docs/reference/python/introduction) · [🌐 Site ↗](https://supabase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase-py/)</sub>

<a name="soul"></a>
### #&#8288;159 [soul](https://github.com/thevahidal/soul) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Nov 2026</sub>

**SQLite database server exposing REST and WebSocket APIs.**

Soul is a Node.js command line tool that serves a SQLite file or :memory: database over a REST API and a WebSocket server on one port. It has optional JWT auth with users, roles and permissions tables, rate limiting, CORS control and an extension mechanism for custom APIs. It is a generic database backend with no AI features.

- **+** One CLI command turns a SQLite file into REST and WebSocket endpoints
- **+** Optional JWT auth with roles, permissions and an initial superuser
- **+** API docs served at /api/docs while the server runs
- **+** Extensions allow custom APIs and static content hosting
- **−** Requires Node.js 22, 24 or 26 because of better-sqlite3
- **−** Soul Studio GUI is described as early-stage and not useful yet
- **−** No prebuilt Docker image; README only gives a Dockerfile to build
- **−** Losing the token secret locks all users out after restart

<sub>no GPU · Needs Node.js 22/24/26, better-sqlite3 · port 8000 · [Repo](https://github.com/thevahidal/soul) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/soul/)</sub>

<a name="pixeltable"></a>
### #&#8288;160 [pixeltable](https://github.com/pixeltable/pixeltable) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="mongo"></a>
### #&#8288;161 [mongo](https://github.com/mongodb/mongo) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Nov 2026</sub>

**Source code for the MongoDB document database server and sharding router.**

This is the C++ source of MongoDB: `mongod`, the database server, and `mongos`, the sharding router. The README covers downloads (Homebrew, Docker image, release page), building from source, packaging into RPM and Debian packages, and running a single server. It is not an AI project or a starter template; it is the database itself, released under the SSPL v1.

- **+** Ships both a single-node server (mongod) and a sharding router (mongos)
- **+** Packaging script generates RPM and Debian packages from source
- **+** Client drivers exist for most programming languages
- **+** Official Homebrew tap and Docker image for installing without building
- **−** SSPL v1 license since October 2018 is not OSI-approved open source
- **−** Building from source requires a separate C++ toolchain setup per docs/building.md
- **−** No AI, vector search or RAG functionality described in the README
- **−** No tagged releases in the repository; binaries come from the download page

<sub>no GPU · [Repo](https://github.com/mongodb/mongo) · [📖 Docs ↗](https://docs.mongodb.com/manual/) · [🌐 Site ↗](https://www.mongodb.com/try/download/community) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongo/)</sub>

<a name="realm-swift"></a>
### #&#8288;162 [realm-swift](https://github.com/realm/realm-swift) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Sep 2026</sub>

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

<a name="tyk"></a>
### #&#8288;163 [tyk](https://github.com/tyktechnologies/tyk) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Nov 2026</sub>

**Go API gateway with auth, rate limiting and MCP traffic control.**

Tyk Gateway is an API gateway written in Go that proxies REST, GraphQL, gRPC, TCP and SOAP traffic, with JWT, bearer token, basic and client-certificate auth, rate limits, quotas and plugins. It can also sit in front of remote MCP servers, applying policy per tool, resource and prompt, and can generate an MCP proxy from a REST API. Redis is required to run it.

- **+** Parses MCP JSON-RPC and applies auth and rate limits per tool, resource and prompt
- **+** Plugins in Python, JavaScript, Go or any language reachable over gRPC
- **+** Hitless config reloads and OpenAPI import (OAS 2.x and 3.0.1) to scaffold APIs
- **+** Install options include Docker, Helm, Ansible, deb and rpm packages, or source build
- **−** Code in the ee folder is under a commercial license; the rest is MPL 2.0
- **−** Dashboard, Developer Portal and Kubernetes Operator need a paid licence
- **−** Analytics in the open source gateway are raw logs only
- **−** Officially supported only on Linux (amd64, i386, arm64)

<sub>no GPU · Docker + Compose · Needs Redis · port 8080 · [Repo](https://github.com/tyktechnologies/tyk) · [📖 Docs ↗](https://tyk.io/docs/) · [🌐 Site ↗](https://tyk.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tyk/)</sub>

<a name="aws-sam-cli"></a>
### #&#8288;164 [aws-sam-cli](https://github.com/aws/aws-sam-cli) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · Apache-2.0 · Nov 2026</sub>

**CLI to build, test locally, and deploy AWS Lambda serverless applications.**

AWS SAM CLI builds, packages and deploys serverless apps defined in SAM or CloudFormation templates, covering Lambda, API Gateway, Step Functions, EventBridge, SQS and SNS. It runs Lambda functions and API Gateway locally in Docker containers via `sam local`, works with CDK apps, and syncs changes to the cloud with `sam sync`. It is written in Python and uses Click for the command line.

- **+** Local Lambda and API Gateway emulation in Docker through `sam local`
- **+** `sam sync` pushes code changes to a cloud dev environment without a full deploy
- **+** `sam init` scaffolds apps from AWS templates for all supported runtimes
- **+** `sam pipeline init` generates CI/CD pipelines; `sam logs` and `sam traces` tail CloudWatch and X-Ray
- **−** Targets AWS only; deployments go through CloudFormation
- **−** Local emulation requires Docker to be installed and running
- **−** Not an AI project; no model or LLM features in the README

<sub>no GPU · Docker · Needs Docker, AWS account, AWS CloudFormation · [Repo](https://github.com/aws/aws-sam-cli) · [📖 Docs ↗](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/what-is-sam.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aws-sam-cli/)</sub>

<a name="objectbox-java"></a>
### #&#8288;165 [objectbox-java](https://github.com/objectbox/objectbox-java) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (44) · Freshness: active (98) · Maintenance: fair (71) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Nov 2026</sub>

**Embedded object database with vector search for Java, Kotlin and Android.**

ObjectBox Java is an on-device NoSQL object database for Android and JVM apps on Linux, macOS and Windows. You annotate plain classes with @Entity and read and write them through typed Box objects, with built-in relations and automatic schema migrations. It also stores vectors for on-device similarity search, which the README positions for RAG and generative AI features.

- **+** Runs in-process on Android 5.0+ and JVM 8+ (Linux x64/arm64/armv7, macOS, Windows x64)
- **+** Annotation-based entities with built-in relations and automatic schema migrations, no SQL
- **+** Vector search sits next to regular objects in the same store
- **+** Distributed through Maven Central with a Gradle plugin; Apache-2.0 SDK code
- **−** Maven setup is supported only for JVM projects, not Android
- **−** Gradle plugin requires JDK 11+, Gradle 7.0+ and AGP 8.1+
- **−** Sync and time-series features are separate products, not in this repository
- **−** Apache-2.0 covers this repository only; other ObjectBox components have separate licenses

<sub>[Repo](https://github.com/objectbox/objectbox-java) · [📖 Docs ↗](https://docs.objectbox.io) · [🌐 Site ↗](https://objectbox.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/objectbox-java/)</sub>

<a name="supabase-js"></a>
### #&#8288;166 [supabase-js](https://github.com/supabase/supabase-js) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

**Official JavaScript client SDK for Supabase services.**

Monorepo of the TypeScript client libraries for Supabase: a combined @supabase/supabase-js package plus separate auth, PostgREST, realtime, storage and edge functions clients. It runs in Node.js, Deno, Bun, browsers, React Native and Cloudflare Workers. It is a client for an existing Supabase backend, not a server or starter app.

- **+** Split into auth-js, postgrest-js, realtime-js, storage-js and functions-js packages, usable individually
- **+** Documented support for Node.js, Deno, Bun, browsers, React Native and Cloudflare Workers
- **+** MIT license, with npm provenance attestations verifiable via npm audit signatures
- **+** Written in TypeScript with a stated runtime version support policy
- **−** Needs a Supabase backend (hosted or self-hosted) to be useful
- **−** Compatibility guaranteed only with latest service releases; PostgREST minimum is v12
- **−** Drops end-of-life Node.js versions in minor releases, e.g. Node 20 in 2.110.0
- **−** Realtime requires native WebSocket support in the runtime

<sub>no GPU · Needs Supabase backend (Auth, PostgREST, Realtime, Storage, Edge Functions) · [Repo](https://github.com/supabase/supabase-js) · [📖 Docs ↗](https://supabase.com/docs/reference/javascript/introduction) · [🌐 Site ↗](https://supabase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase-js/)</sub>

<a name="terraform-hcloud-kube-hetzner"></a>
### #&#8288;167 [terraform-hcloud-kube-hetzner](https://github.com/mysticaltech/terraform-hcloud-kube-hetzner) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Sep 2026</sub>

**Terraform/OpenTofu module that builds k3s or RKE2 clusters on Hetzner Cloud.**

Kube-Hetzner is a Terraform/OpenTofu module that provisions a Kubernetes cluster on Hetzner Cloud, running k3s or RKE2 on openSUSE Leap Micro nodes. It wires in private networking, firewalls, CSI storage, ingress, cert management, and automatic OS and Kubernetes upgrades. A `createkh` script generates the project folder, `kube.tf`, and node images.

- **+** HA control plane, multi-location pools, and Cluster Autoscaler nodepools
- **+** Choice of k3s or RKE2, and Flannel, Calico, or Cilium networking
- **+** Plan-time validation rejects invalid topology and variable combinations before apply
- **+** State-aware destroy script reports possible Hetzner orphans; ships agent skills for migration and upgrades
- **−** Hetzner Cloud only; Robot dedicated servers need a separate integration
- **−** Requires Packer to build Leap Micro images alongside Terraform/OpenTofu and hcloud
- **−** v2 to v3 upgrade needs a manual migration; blind apply is discouraged
- **−** Cloudflare Mesh/WARP is not supported as node transport

<sub>no GPU · Needs Hetzner Cloud account and API token, OpenTofu or Terraform >= 1.10.1, Packer 1.16.0, kubectl, hcloud CLI · [Repo](https://github.com/mysticaltech/terraform-hcloud-kube-hetzner) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terraform-hcloud-kube-hetzner/)</sub>

<a name="openmeter"></a>
### #&#8288;168 [openmeter](https://github.com/openmeterio/openmeter) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

**Usage metering, entitlements and usage-based billing API for AI and API products.**

OpenMeter ingests CloudEvents, aggregates them into per-customer meters in real time, and exposes the results through a REST API with JavaScript, Python and Go SDKs. On top of metering it provides a product catalog (plans, features, add-ons, tiered and package pricing), entitlements for access and usage limits, and an invoice lifecycle with credits. Releases are described as beta and can include breaking changes.

- **+** Covers metering, plans, entitlements, credits and invoicing behind one API, and parts can be used alone
- **+** Ingests CloudEvents and queries usage by time window or dimension, backed by ClickHouse
- **+** Official JavaScript and Go SDKs plus a preview Python SDK; webhooks and external invoicing providers supported
- **+** Compose quickstart ships a ready api_requests_total meter for trying event ingestion
- **−** Runtime needs Kafka, ClickHouse and PostgreSQL, with Redis and Svix optional; heavy to self-host
- **−** Releases are beta and may include breaking changes between versions
- **−** Official Helm chart is for development only, and the Compose stack is not a production topology
- **−** No operator UI, payment processor or tax engine; Python SDK is preview

<sub>no GPU · Docker + Compose · Needs Kafka, ClickHouse, PostgreSQL, Redis (optional), Svix (optional, webhooks) · port 48888 · [Repo](https://github.com/openmeterio/openmeter) · [📖 Docs ↗](https://openmeter.io/docs) · [🌐 Site ↗](https://openmeter.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openmeter/)</sub>

<a name="oceanbase"></a>
### #&#8288;169 [oceanbase](https://github.com/oceanbase/oceanbase) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · Apache-2.0 · Nov 2026</sub>

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

<a name="micronaut-core"></a>
### #&#8288;170 [micronaut-core](https://github.com/micronaut-projects/micronaut-core) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Nov 2026</sub>

**JVM framework for microservices and HTTP servers with compile-time dependency injection.**

Micronaut Framework is a Java, Kotlin and Groovy framework for building HTTP servers, microservices, message-driven apps and command-line apps. It does dependency injection and AOP at compile time instead of through runtime reflection and bytecode generation, which the README says gives fast startup and lower memory use. It is a general application framework with no built-in AI features.

- **+** DI and AOP are computed at compile time, with minimal reflection and no runtime bytecode generation
- **+** Microservice pieces included: distributed config, service discovery, HTTP routing, client-side load balancing
- **+** Supports Java, Kotlin and Groovy
- **+** Uses Semantic Versioning 2.0.0, with @Experimental and @Internal APIs excluded
- **−** No AI, LLM or agent features in this repository
- **−** Not a hosted backend: you write and deploy the JVM application yourself
- **−** Building from source needs Gradle and publishes to the local Maven repository
- **−** Compile-time processing differs from Spring's runtime model, so Spring code needs porting

<sub>no GPU · Needs JVM, Gradle · [Repo](https://github.com/micronaut-projects/micronaut-core) · [🌐 Site ↗](https://micronaut.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/micronaut-core/)</sub>

<a name="permify"></a>
### #&#8288;171 [permify](https://github.com/permify/permify) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · AGPL-3.0 · Nov 2026</sub>

**Zanzibar-inspired authorization service for RBAC, ReBAC and ABAC access checks.**

Permify is a Go authorization service that answers access checks (for example, can user X view document Y) over REST and gRPC. Permissions are defined in a domain-specific modeling language covering RBAC, ReBAC and ABAC, with per-tenant isolation. It follows the design of Google Zanzibar and comes as a self-hosted Community Edition or a paid cloud service.

- **+** REST on port 3476 and gRPC on 3478 from a single serve command
- **+** One modeling language covers RBAC, ReBAC and ABAC, with tenant-level isolation
- **+** Published load test: 10,000 RPS target, 0% failed requests, p95 about 59ms
- **+** Online playground to model and test permissions with sample data
- **−** Community Edition omits observability dashboards and data synchronization, which are cloud-only
- **−** CE ships as a long-term release four times a year, so new features arrive late
- **−** AGPL-3.0 license may constrain embedding in proprietary products
- **−** Default quickstart stores data in memory; persistent storage setup is not described in the README

<sub>no GPU · Docker + Compose · port 3476 · [Repo](https://github.com/permify/permify) · [▶️ Demo ↗](https://play.permify.co/) · [📖 Docs ↗](https://docs.permify.co/) · [🌐 Site ↗](https://permify.co/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/permify/)</sub>

<a name="tsuru"></a>
### #&#8288;172 [tsuru](https://github.com/tsuru/tsuru) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (50) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · BSD-3-Clause · Nov 2026</sub>

**Extensible PaaS that deploys apps onto Kubernetes clusters via a CLI.**

tsuru is a Go-based Platform as a Service that deploys and manages applications on Kubernetes, driven by the `tsuru` command-line client. It supports language platforms for Python, Node.js, Go, Ruby, PHP, Perl, Lua and Java, and attaches add-on resources such as SQL and NoSQL databases, memcached and Redis. It is a general application platform, not an AI-specific project.

- **+** Targets work like kubectl contexts, so one CLI manages several environments
- **+** Eight language platforms: Python, Node.js, Go, Ruby, PHP, Perl, Lua, Java
- **+** Install guides for Minikube and GKE; local dev via make local.setup and local.run
- **+** Add-on resources include SQL and NoSQL databases, memcached and Redis
- **−** Requires a Kubernetes cluster; no standalone single-node install is described
- **−** Local development needs docker or podman, minikube, go and yq
- **−** No AI or model-serving features; it is a general-purpose PaaS
- **−** Quick start defers most setup detail to external docs

<sub>no GPU · Docker + Compose · Needs Kubernetes, Minikube (local dev), Docker or Podman (local dev), Go, yq · [Repo](https://github.com/tsuru/tsuru) · [📖 Docs ↗](https://docs.tsuru.io/) · [🌐 Site ↗](https://tsuru.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tsuru/)</sub>

<a name="armeria"></a>
### #&#8288;173 [armeria](https://github.com/line/armeria) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Nov 2026</sub>

**Java microservice framework for gRPC, Thrift and REST services.**

Armeria is a Java framework for building reactive microservices, created by the author of Netty and colleagues at LINE. It integrates with gRPC, Thrift, Kotlin, Retrofit, Reactive Streams, Spring Boot and Dropwizard. The README describes no AI-specific features, so it fits this list only as a general backend service base.

- **+** Supports gRPC, Thrift, Retrofit and Reactive Streams in one framework
- **+** Integrates with Spring Boot, Dropwizard and Kotlin
- **+** Runs on Java 8 or later for users
- **+** Active: release on 2026-11-06, Apache-2.0 license
- **−** No AI, LLM or agent features described in the README
- **−** JVM-only; not usable directly from Python or Node.js stacks
- **−** README has no quickstart, benchmarks or feature details

<sub>no GPU · Needs Java 8 or later · [Repo](https://github.com/line/armeria) · [🌐 Site ↗](https://armeria.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/armeria/)</sub>

<a name="prest"></a>
### #&#8288;174 [prest](https://github.com/prest/prest) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

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

<a name="good-job"></a>
### #&#8288;175 [good_job](https://github.com/bensheldon/good_job) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

**Multithreaded Postgres-backed Active Job queue for Ruby on Rails.**

GoodJob is a Rails gem that runs Active Job background jobs from a Postgres table, using advisory locks for run-once safety and LISTEN/NOTIFY to cut queue latency. Jobs run in a separate `good_job start` process or in threads inside the web server. It also covers cron-style jobs, batches, concurrency and throttling controls, and a web dashboard.

- **+** Needs only Postgres, no Redis; uses advisory locks and LISTEN/NOTIFY
- **+** Can run inside the web process (async mode) or as a separate CLI worker
- **+** Built-in cron, batches, concurrency controls and a web dashboard
- **+** Works with standard Active Job features: queues, priorities, delays, retries
- **−** Rails and Postgres only; no other databases or non-Rails frameworks
- **−** Requires Rails 6.1+, Ruby 3.0+ (or JRuby 9.4+) and Postgres 10+
- **−** Not an AI project; fits this list only as general app infrastructure
- **−** Needs extra setup for PgBouncer and database connection sizing

<sub>no GPU · Needs PostgreSQL 10+, Ruby on Rails 6.1+ · [Repo](https://github.com/bensheldon/good_job) · [▶️ Demo ↗](https://goodjob-demo.herokuapp.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/good-job/)</sub>

<a name="sqlc"></a>
### #&#8288;176 [sqlc](https://github.com/sqlc-dev/sqlc) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (80) · Freshness: active (97) · Maintenance: patchy (39) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**SQL compiler that generates type-safe application code from SQL queries.**

sqlc reads SQL queries and generates type-safe code with interfaces to those queries, so application code calls generated functions instead of hand-written database glue. Go, Kotlin, Python and TypeScript are supported through separate sqlc-gen plugins, and other languages can be added as community plugins. It is written in Go and has a browser playground.

- **+** Queries stay in plain SQL; generated code gives typed interfaces to them
- **+** Language backends are plugins: Go, Kotlin, Python and TypeScript, plus community ones
- **+** Browser playground at play.sqlc.dev for trying it without installing
- **+** MIT licensed, written in Go, with downloads and docs published
- **−** Not a database or backend; it only generates client code for SQL you write
- **−** Language support lives in separate plugin repositories, each with its own maturity
- **−** README does not describe how schemas or database engines are configured

<sub>no GPU · Docker + Compose · Compose runs MySQL, PostgreSQL, ClickHouse · [Repo](https://github.com/sqlc-dev/sqlc) · [▶️ Demo ↗](https://play.sqlc.dev/) · [📖 Docs ↗](https://docs.sqlc.dev) · [🌐 Site ↗](https://sqlc.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sqlc/)</sub>

<a name="hsweb-framework"></a>
### #&#8288;177 [hsweb-framework](https://github.com/hs-web/hsweb-framework) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · Apache-2.0 · Nov 2026</sub>

**Reactive Java admin-backend framework on Spring WebFlux and R2DBC.**

hsweb is a set of Maven modules for building admin backends on Spring Boot 2.x, WebFlux and R2DBC. It provides generic reactive CRUD through easy-orm, RBAC and data-level permissions, reactive caching, and built-in user, permission and dictionary management. It has no AI features. The README recommends depending on selected modules rather than cloning the repo.

- **+** End-to-end reactive stack: WebFlux, R2DBC and reactive transactions
- **+** Injectable ReactiveRepository gives CRUD without writing SQL; DSL queries are parameterized
- **+** RBAC plus data permissions, applied with annotations like @SaveAction
- **+** Modular: pull only the Maven modules you need
- **−** Non-reactive (MVC/JDBC) support is listed as not done
- **−** Two-factor auth and file instant-upload are unchecked in the feature list
- **−** Requires working knowledge of Reactor and Spring WebFlux
- **−** Docs are Chinese-language and spread across per-module READMEs

<sub>no GPU · Needs Java 8, Maven 3, Spring Boot 2.x, H2, MySQL, SQL Server or PostgreSQL · [Repo](https://github.com/hs-web/hsweb-framework) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hsweb-framework/)</sub>

<a name="readyset"></a>
### #&#8288;178 [readyset](https://github.com/readysettech/readyset) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · custom license · Nov 2026</sub>

**Wire-compatible caching proxy for Postgres and MySQL reads.**

Readyset sits between an application and a Postgres or MySQL database and serves cached results for chosen SQL reads. It keeps the cache current by consuming the database's replication stream, so there is no manual invalidation and no app rewrite. Written in Rust, it speaks the Postgres and MySQL wire protocols, so existing ORMs and clients connect to it unchanged.

- **+** Cache stays in sync through the database replication stream, with no manual invalidation
- **+** Wire-compatible with Postgres and MySQL, so existing ORMs and drivers work unchanged
- **+** Handles complex SQL reads, not just key lookups
- **+** Install options: Docker image, Linux binary, or a curl quickstart script
- **−** BSL 1.1 license, not OSI open source until it converts to Apache 2.0 after 4 years
- **−** Supports only Postgres and MySQL as upstream databases
- **−** Needs replication access to the primary database
- **−** Managed offering (Readyset Cloud) is a separate hosted service

<sub>no GPU · Compose · Needs Postgres or MySQL with replication enabled · [Repo](https://github.com/readysettech/readyset) · [▶️ Demo ↗](https://readyset.io/docs/) · [📖 Docs ↗](https://docs.readyset.io) · [🌐 Site ↗](https://readyset.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/readyset/)</sub>

<a name="dynamic-datasource"></a>
### #&#8288;179 [dynamic-datasource](https://github.com/baomidou/dynamic-datasource) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Oct 2026</sub>

**Spring Boot starter that routes calls to multiple datasources via @DS.**

Java library for Spring Boot 1.5 to 4.x that picks which DataSource a method call runs against, using an @DS annotation and YAML-declared datasources. It covers read/write splitting, one-master-many-slaves groups, runtime add/remove of datasources, and local multi-datasource transactions, with Seata and Atomikos XA for distributed commits. It is a general JDBC routing library with no AI features, so it fits this list only loosely.

- **+** Separate starters for Spring Boot 2, 3 and 4; CI-tested on JDK 17/21/25/27 and GraalVM Native
- **+** @DSTransactional gives local multi-datasource transactions with 7 propagation levels, no external coordinator
- **+** Datasources can be added, removed or lazily created at runtime, useful for per-tenant databases
- **+** Supports Druid, HikariCP, BeeCP, DBCP2, C3P0, Oracle UCP and ENC(...) encrypted credentials
- **−** Connection pools and JDBC drivers are not bundled; you must add and align them yourself
- **−** Full reference docs are in Chinese; the English wiki is still being migrated
- **−** Only chooses the datasource; no sharding, schema management or ORM of its own
- **−** Not an AI project; the repo only ships an agent skill for troubleshooting help

<sub>no GPU · Needs Spring Boot, JDK 8+ (JDK 17+ for Boot 3/4), JDBC driver, Connection pool (Druid, HikariCP, etc.) · [Repo](https://github.com/baomidou/dynamic-datasource) · [📖 Docs ↗](https://doc.xiuceyun.cn) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dynamic-datasource/)</sub>

<a name="microfeed"></a>
### #&#8288;180 [microfeed](https://github.com/microfeed/microfeed) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · AGPL-3.0 · Sep 2026</sub>

**Headless CMS that publishes web, RSS and JSON feeds from Cloudflare Workers.**

microfeed is a CMS that publishes audio, video, images, documents, posts and external links to a website, an RSS feed and a JSON Feed. It runs on Cloudflare Workers with D1 for metadata and R2 for media, and has a built-in email/password admin dashboard. Content can also be managed through an API, webhooks and the @microfeed/cli, which a local AI agent can use to deploy the site and edit content.

- **+** No server to run: Workers, D1 and R2, with free-tier quotas covering small sites
- **+** Versioned themes stored in D1, with draft preview, explicit activation and rollback
- **+** Snapshot command exports the database, R2 bucket and migration history to one archive
- **+** Podcast fields (Podcasting 2.0 tags, transcripts, chapters) plus OpenAPI docs and llms.txt
- **−** Cloudflare only; other serverless platforms are not supported yet
- **−** README describes the project as in open alpha
- **−** AGPL-3.0 license constrains modified hosted deployments
- **−** Snapshot archives are unencrypted and contain admin password hashes

<sub>no GPU · Needs Cloudflare Workers, Cloudflare D1, Cloudflare R2 · [Repo](https://github.com/microfeed/microfeed) · [▶️ Demo ↗](https://llamacorn.listennotes.com/) · [📖 Docs ↗](https://docs.microfeed.org) · [🌐 Site ↗](https://www.microfeed.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/microfeed/)</sub>

<a name="zenstack"></a>
### #&#8288;181 [zenstack](https://github.com/zenstackhq/zenstack) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

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

<a name="serenity"></a>
### #&#8288;182 [serenity](https://github.com/serenity-is/serenity) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

**ASP.NET Core and TypeScript framework for database-driven CRUD business apps.**

Serenity is an MIT-licensed application platform for data-centric business apps. The Sergen generator reads database tables and produces C# rows, services, and TypeScript grids, dialogs and types. Attributes on rows drive validation, permissions, lookups and Excel export. It supports SQL Server, PostgreSQL, MySQL, Oracle, Firebird and SQLite. It has no AI features.

- **+** Sergen generates rows, services, grids and dialogs from existing database tables
- **+** C# metadata generates TypeScript types, so the C#/TypeScript boundary is checked at build time
- **+** Row- and field-level permissions, audit logging and soft delete are built in
- **+** Supports six databases with FluentMigrator migrations; no separate SPA to deploy
- **−** Tied to the .NET and ASP.NET Core stack; no support for other backend languages
- **−** Dashboards, email client and other modules are in the paid StartSharp template
- **−** No AI or LLM features, so it fits this list only as a general app starter
- **−** Opinionated attribute-driven approach; the generated code must be learned before customizing

<sub>no GPU · Needs .NET 10 SDK, Node.js 24 LTS, SQL database (SQL Server, PostgreSQL, MySQL, Oracle, Firebird or SQLite) · port 5000 · [Repo](https://github.com/serenity-is/serenity) · [▶️ Demo ↗](https://demo.serenity.is) · [📖 Docs ↗](https://serenity.is/docs) · [🌐 Site ↗](https://serenity.is) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serenity/)</sub>

<a name="avo"></a>
### #&#8288;183 [avo](https://github.com/avo-hq/avo) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · custom license · Nov 2026</sub>

**Admin panel and internal tool framework for Ruby on Rails apps.**

Avo is a Ruby gem that adds an admin panel, CMS or internal tool to an existing or new Rails app. Resources are defined in Ruby and generate CRUD views over Active Record, with fields, associations, filters, actions, dashboards and Pundit-based authorization. The UI is built on Hotwire, and the README lists no AI features.

- **+** Drops into an existing Rails app without changing its code
- **+** Covers CRUD, search, filters, actions, dashboards and Active Storage uploads
- **+** Pundit authorization and i18n support are built in
- **+** Custom fields and custom tools for pages beyond CRUD
- **−** Rails and Active Record only; unusable outside Ruby apps
- **−** No AI or LLM features described, so a loose fit for this list
- **−** License is reported as NOASSERTION; check the repo before commercial use
- **−** Several features, such as theming and inline editing, are still roadmap items

<sub>no GPU · Docker + Compose · Needs Ruby on Rails, Active Record, Pundit (optional, for authorization) · [Repo](https://github.com/avo-hq/avo) · [▶️ Demo ↗](https://main.avodemo.com/) · [📖 Docs ↗](https://docs.avohq.io) · [🌐 Site ↗](https://avohq.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/avo/)</sub>

<a name="arcadedb"></a>
### #&#8288;184 [arcadedb](https://github.com/arcadedata/arcadedb) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Nov 2026</sub>

**Multi-model database covering graph, document, key/value, time series and vectors.**

ArcadeDB is an ACID database written in Java that stores graph, document, key/value, time series, vector and geospatial data in one engine. It accepts SQL, Cypher, Gremlin, GraphQL and MongoDB queries, and is reachable over HTTP/JSON, the Postgres wire protocol, and subsets of the Redis and MongoDB protocols. It also ships a built-in MCP server and a Claude Code plugin.

- **+** One engine covers graph, document, key/value, time series, vector and geospatial models
- **+** Many query languages and protocols: SQL, Cypher, Gremlin, GraphQL, Postgres wire, HTTP/JSON
- **+** Built-in MCP server plus a Claude Code plugin for AI assistant access
- **+** Runs embedded on the JVM, as a server, or as an experimental native image
- **−** Redis and MongoDB drivers implement only a subset of operations
- **−** Requires Java 21+; Java 17 is supported only on a separate branch
- **−** GraalVM native-image build is labeled experimental
- **−** Studio AI assistant is marked Beta

<sub>no GPU · Compose · Needs Java 21+ · port 2480 · [Repo](https://github.com/arcadedata/arcadedb) · [📖 Docs ↗](https://docs.arcadedb.com) · [🌐 Site ↗](https://arcadedb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/arcadedb/)</sub>

<a name="sqlx"></a>
### #&#8288;185 [sqlx](https://github.com/transact-rs/sqlx) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Nov 2026</sub>

**Async Rust SQL toolkit with compile-time checked queries and no DSL.**

SQLx is a Rust crate for talking to PostgreSQL, MySQL/MariaDB and SQLite using async/await on tokio or async-std. Queries are plain SQL; the query macros connect to a development database at build time to verify syntax and types. It includes connection pooling, row streaming, statement caching, migrations and an Any driver, but it is not an ORM.

- **+** Compile-time checked SQL via the query macros, verified by a development database
- **+** Postgres and MySQL drivers in pure Rust with forbid(unsafe_code)
- **+** Runs on tokio or async-std, with native-tls or rustls backends
- **+** Built-in pooling, nested transactions, LISTEN/NOTIFY, migrations and offline query cache
- **−** Not an ORM; no query builder or model layer
- **−** Query macros need DATABASE_URL at build time or a prepared offline cache
- **−** MSSQL support was removed in 0.7 pending a driver rewrite
- **−** Must pick runtime and TLS feature flags from many combinations

<sub>no GPU · Needs PostgreSQL, MySQL/MariaDB or SQLite, Rust toolchain, tokio or async-std · [Repo](https://github.com/transact-rs/sqlx) · [📖 Docs ↗](https://docs.rs/sqlx) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sqlx/)</sub>

<a name="camel"></a>
### #&#8288;186 [apache/camel](https://github.com/apache/camel) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Nov 2026</sub>

**Java integration framework with 350+ connectors, routes in Java, YAML or XML.**

Apache Camel connects databases, APIs, message brokers and cloud services through routes written in Java, YAML, or XML, with Enterprise Integration Patterns built in. It runs on Spring Boot, Quarkus, or standalone via the Camel CLI. For AI use, it ships an MCP server exposing the Camel catalog to coding assistants, plus LangChain4j and OpenAI components and A2A protocol support.

- **+** 350+ connectors including Kafka, JDBC, AWS, Azure, GCP and Salesforce
- **+** Same route can be written in Java, YAML, or XML
- **+** Runs on Spring Boot, Quarkus, Kubernetes (Camel K), or standalone CLI
- **+** In production since 2007; Apache-2.0 licensed
- **−** AI features are secondary; this is a general integration framework, not an AI app starter
- **−** JVM-based; needs Java tooling and Maven or the Camel CLI
- **−** No published release detected by tooling for this repository
- **−** Large component surface means a steep learning curve for newcomers

<sub>no GPU · Needs Java, Maven · Models: LangChain4j, OpenAI · [Repo](https://github.com/apache/camel) · [📖 Docs ↗](https://camel.apache.org/manual/getting-started.html) · [🌐 Site ↗](https://camel.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/camel/)</sub>

<a name="uptrace-bun"></a>
### #&#8288;187 [uptrace/bun](https://github.com/uptrace/bun) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · BSD-2-Clause · Nov 2026</sub>

**SQL-first Go ORM for PostgreSQL, MySQL, MSSQL, SQLite and Oracle.**

Bun is a Go library built on database/sql that maps structs to tables and lets you write queries in a builder that mirrors SQL, including CTEs. It covers relations via struct tags, bulk insert/update/delete, migrations, and query hooks for debug logging and OpenTelemetry. It is a data-access library, not an AI project or a hosted backend.

- **+** Query builder follows SQL closely, including CTEs and raw expressions
- **+** One API across PostgreSQL, MySQL/MariaDB, MSSQL, SQLite and Oracle
- **+** Scans into structs, maps, scalars or slices
- **+** Ships migrations, fixtures, soft deletes and an OpenTelemetry query hook
- **−** Go only; it is a library, not a standalone service
- **−** Queries use string expressions, so some SQL errors surface only at runtime
- **−** Not related to AI; it only fits as a database layer in a Go backend
- **−** Each database needs its own driver and dialect package

<sub>no GPU · Needs A SQL database (PostgreSQL, MySQL/MariaDB, MSSQL, SQLite or Oracle) · [Repo](https://github.com/uptrace/bun) · [📖 Docs ↗](https://bun.uptrace.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/uptrace-bun/)</sub>

<a name="remult"></a>
### #&#8288;188 [remult](https://github.com/remult/remult) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Nov 2026</sub>

**TypeScript entity library that generates CRUD, realtime API and typed client.**

Remult uses decorated TypeScript entity classes as a single definition for a REST API with live queries, a type-safe frontend client, and a backend ORM. It ships adapters for Express, Fastify, Next.js, Nuxt, SvelteKit, SolidStart, Nest, Koa, Hapi and Hono, and data providers for PostgreSQL, MySQL, SQLite, MongoDB, MSSQL and Oracle. Validation and authorization rules are declared once in code and enforced on both sides.

- **+** One entity definition drives API, typed client, ORM and validation, no code generation
- **+** Adapters for ten server frameworks and six database families
- **+** Built-in live queries, relations, Open API and GraphQL options, and an admin UI
- **+** Can be adopted incrementally in an existing project
- **−** Major version still 0.x; v1 API not finalized
- **−** Docs described by the README as a work in progress
- **−** Library only: you provide the server, database and hosting
- **−** Entity model relies on decorators unless you use the non-decorator syntax

<sub>no GPU · Needs Node.js, PostgreSQL, MySQL, SQLite, MongoDB, MSSQL or Oracle · [Repo](https://github.com/remult/remult) · [▶️ Demo ↗](https://learn.remult.dev/) · [📖 Docs ↗](https://remult.dev/docs) · [🌐 Site ↗](https://remult.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/remult/)</sub>

<a name="harness-harness"></a>
### #&#8288;189 [harness/harness](https://github.com/harness/harness) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: widely used (93) · Freshness: active (97) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · Apache-2.0 · Nov 2026</sub>

**Self-hosted Git hosting with CI pipelines, Gitspaces and artifact registries.**

Harness Open Source is a Go server that combines Git repository hosting, Docker-based CI pipelines, hosted development environments (Gitspaces) and artifact registries behind one web UI and REST API. It is the successor to Drone, though pipeline parity with Drone is not yet reached. It has no AI features; it fits this list only as a self-hosted platform for building and shipping apps.

- **+** Code hosting, pipelines, Gitspaces and registries in one server
- **+** Starts with a single docker run on port 3000
- **+** Swagger spec served at /swagger, plus a CLI for creating tokens
- **+** Builds and runs on any OS and architecture Go supports
- **−** Pipeline features not yet at parity with Drone, which lives on a separate branch
- **−** Pipelines need access to the host Docker socket
- **−** Default admin login is admin/changeit and must be changed
- **−** Contains no AI features; the README describes only DevOps tooling

<sub>no GPU · Docker · Needs Docker · port 3000 · [Repo](https://github.com/harness/harness) · [📖 Docs ↗](https://developer.harness.io/docs/open-source) · [🌐 Site ↗](https://developer.harness.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/harness-harness/)</sub>

<a name="spring-cloud-alibaba"></a>
### #&#8288;190 [spring-cloud-alibaba](https://github.com/alibaba/spring-cloud-alibaba) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: widely used (88) · Freshness: active (91) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Nov 2026</sub>

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

<a name="arangodb"></a>
### #&#8288;191 [arangodb](https://github.com/arangodb/arangodb) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · custom license · Nov 2026</sub>

**Multi-model database for graphs, JSON documents and full-text search via AQL.**

ArangoDB is a C++ database that stores key-value pairs, JSON documents and graphs, and queries them with a single language, AQL. It includes ArangoSearch for indexing and ranked text search, and it shards and replicates data across cluster nodes with automatic failover. It is a general data backend rather than an AI starter, suited to graph or search-heavy apps.

- **+** One query language (AQL) covers documents, graphs, joins and ranked full-text search
- **+** Horizontal sharding, replication and automatic failover in cluster mode
- **+** Schema-free by default, with optional schema validation and multi-collection transactions
- **+** Runs on-prem, in the cloud or as a managed service (Arango Managed Platform)
- **−** SmartGraphs, SmartJoins, Hot Backups and Encryption 360 are listed as Enterprise features
- **−** Community Edition has no stated dataset limit removal; Enterprise is needed for unlimited size
- **−** AQL is specific to ArangoDB, so SQL or Cypher queries need rewriting
- **−** No tagged GitHub release; packages come from the vendor download page

<sub>no GPU · port 8529 · [Repo](https://github.com/arangodb/arangodb) · [📖 Docs ↗](https://docs.arango.ai/) · [🌐 Site ↗](https://arango.ai/downloads/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/arangodb/)</sub>

<a name="tortoise-orm"></a>
### #&#8288;192 [tortoise-orm](https://github.com/tortoise/tortoise-orm) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · Apache-2.0 · Nov 2026</sub>

**Async Python ORM with a Django-like API and built-in migrations.**

Tortoise ORM is an asyncio object-relational mapper for Python 3.10+ with a Django-style model and query API. It supports SQLite, PostgreSQL, MySQL, Microsoft SQL Server and Oracle, and ships a migration CLI (init, makemigrations, migrate, sqlmigrate). It is a general database library, not an AI project, so it fits the backends category as a data layer for apps.

- **+** Async-native API with Django-like models, filters, prefetch_related and related-field lookups
- **+** Built-in migrations: autodetect changes, RunPython/RunSQL, reversible ops, SQL preview
- **+** Covers SQLite, PostgreSQL, MySQL, MS SQL and Oracle, with a choice of drivers for some
- **+** Publishes benchmarks against other Python ORMs on PostgreSQL 17
- **−** A library only: no server, auth, storage or hosting, so it is not a full backend
- **−** MS SQL and Oracle both go through the asyncodbc extra
- **−** generate_schemas is development-only; production needs the migration framework
- **−** No AI or LLM features; it is a general-purpose ORM

<sub>no GPU · Needs Python 3.10+, aiosqlite (SQLite default), asyncpg or psycopg (PostgreSQL), aiomysql or asyncmy (MySQL), asyncodbc (MS SQL, Oracle) · [Repo](https://github.com/tortoise/tortoise-orm) · [📖 Docs ↗](https://tortoise.github.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tortoise-orm/)</sub>

<a name="drift"></a>
### #&#8288;193 [drift](https://github.com/simolus3/drift) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Nov 2026</sub>

**Reactive SQLite persistence library for Flutter and Dart with generated type-safe queries.**

Drift is a Dart and Flutter library on top of SQLite. Tables and queries are written in Dart or SQL, and code generation produces type-safe APIs, with SQL checked at compile time. Queries can be exposed as auto-updating streams, and database work can run across isolates. It targets Android, iOS, macOS, Windows, Linux and the web. It is not an AI project.

- **+** Queries written in Dart or SQL, including WITH and WINDOW clauses, checked at compile time
- **+** Any query, including multi-table ones, can be turned into an auto-updating stream
- **+** Built-in transactions, schema migrations, DAOs and batched updates
- **+** Runs on Android, iOS, macOS, Windows, Linux and web; includes a sample Flutter todo app
- **−** Limited to Dart and Flutter; no support for other languages
- **−** Needs a code generator (drift_dev) in the build step
- **−** Local SQLite persistence only; no server, auth or sync, which need separate tools
- **−** Not an AI project; fits this list only loosely

<sub>no GPU · Docker · Needs SQLite · [Repo](https://github.com/simolus3/drift) · [📖 Docs ↗](https://drift.simonbinder.eu/docs/getting-started/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/drift/)</sub>

<a name="matrixone"></a>
### #&#8288;194 [matrixone](https://github.com/matrixorigin/matrixone) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

**MySQL-compatible HTAP database with Git-style snapshots and vector search.**

MatrixOne is a Go database that speaks the MySQL protocol and runs transactional, analytical, full-text and vector workloads in one engine. It adds zero-copy snapshots, time travel, branching and rollback for data, plus IVF and HNSW vector indexes for RAG use. A Python SDK covers vector and full-text queries, and storage is separated from compute.

- **+** MySQL protocol compatibility, so existing clients and ORMs connect on port 6001
- **+** Built-in IVF and HNSW vector indexes plus full-text search, no separate vector store
- **+** Snapshots, time travel and rollback for data without full backups
- **+** Python SDK with ORM support for vector and boolean full-text queries
- **−** Building from source needs Go 1.27.1 or later, GCC/Clang and Make
- **−** Full cluster setup has multiple node types, heavier than an embedded database
- **−** Infrastructure component, not an app starter you fork and run

<sub>no GPU · [Repo](https://github.com/matrixorigin/matrixone) · [🌐 Site ↗](https://www.matrixorigin.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/matrixone/)</sub>

<a name="gorm"></a>
### #&#8288;195 [gorm](https://github.com/go-gorm/gorm) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

**ORM library for Go with associations, hooks, migrations and plugins.**

GORM is a Go object-relational mapper that maps structs to SQL tables. It covers associations, hooks, eager loading with Preload and Joins, nested transactions with save points, batch operations and auto migrations. A plugin API adds features such as read/write splitting across databases and Prometheus metrics. It has no AI functionality, so it fits this list only loosely.

- **+** Supports Has One, Has Many, Belongs To, Many To Many and polymorphic associations
- **+** Transactions with nested transactions and save points, plus DryRun and prepared statement modes
- **+** Plugin API for database resolver (multiple databases, read/write splitting) and Prometheus
- **+** Companion Gen tool and documentation site at gorm.io
- **−** Not an AI project; no model, agent or LLM features
- **−** Library only: no server, auth, storage or hosting included
- **−** README lists no supported databases or driver setup; those are on the docs site
- **−** Auto migrations and hooks can hide SQL behavior from the developer

<sub>no GPU · [Repo](https://github.com/go-gorm/gorm) · [📖 Docs ↗](https://gorm.io) · [🌐 Site ↗](https://gorm.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gorm/)</sub>

<a name="sequelize"></a>
### #&#8288;196 [sequelize](https://github.com/sequelize/sequelize) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (88) · Freshness: active (93) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Nov 2026</sub>

**Promise-based Node.js ORM for Postgres, MySQL, SQLite, SQL Server and more.**

Sequelize is a TypeScript/Node.js ORM that maps models to tables across Postgres, MySQL, MariaDB, SQLite, DB2, Microsoft SQL Server, Snowflake, Oracle DB and Db2 for IBM i. It provides transactions, relations, eager and lazy loading, and read replication. Version 6 is the stable line and version 7 is in alpha.

- **+** Supports nine SQL databases, including Oracle, Snowflake, DB2 and SQL Server
- **+** Transactions, relations, eager/lazy loading and read replication built in
- **+** MIT license with published upgrade guides for v5 to v6 and v6 to v7
- **+** Extensions exist for CockroachDB, YugabyteDB and GraphQL
- **−** Not an AI project; it is a general database library
- **−** Next major version (v7) is still alpha
- **−** README says new maintainers are being sought to finish v7
- **−** Library only: no hosted backend, auth or storage

<sub>no GPU · Needs Node.js, A supported SQL database · [Repo](https://github.com/sequelize/sequelize) · [📖 Docs ↗](https://sequelize.org/docs/v6/getting-started) · [🌐 Site ↗](https://sequelize.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sequelize/)</sub>

<a name="apitable"></a>
### #&#8288;197 [apitable](https://github.com/apitable/apitable) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · AGPL-3.0 · Sep 2026</sub>

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

<a name="ubicloud"></a>
### #&#8288;198 [ubicloud](https://github.com/ubicloud/ubicloud) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · AGPL-3.0 · Nov 2026</sub>

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
### #&#8288;199 [ihp](https://github.com/digitallyinduced/ihp) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Nov 2026</sub>

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

<a name="spring-cloud-gateway"></a>
### #&#8288;200 [spring-cloud-gateway](https://github.com/spring-cloud/spring-cloud-gateway) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · Apache-2.0 · Nov 2026</sub>

**API gateway for Spring Boot 3 with route predicates and per-route filters.**

Spring Cloud Gateway is a Java API gateway built on Spring Framework 6 and Spring Boot 3 (Java 17). It matches requests by path, method, header or host, then applies filters scoped to the route that modify the downstream request and response, such as header changes, path rewrites and circuit breaker. Routes can be defined in configuration or through an API, and can come from a Spring Cloud DiscoveryClient.

- **+** Routes can be defined in configuration or through a Java API
- **+** Route matching is built into Spring Handler Mapping
- **+** Per-route filters cover headers, parameters, path rewrite and circuit breaker
- **+** Spring Cloud DiscoveryClient can supply routes
- **−** Requires a JVM (Java 17) and the Spring Boot 3 stack
- **−** README covers only building and contributing, no usage or config examples
- **−** No Docker image or compose file detected in the repository
- **−** Not a model or LLM gateway; no AI features described

<sub>no GPU · Needs JDK 17, Maven, Spring Boot 3, Docker (tests needing Redis) · [Repo](https://github.com/spring-cloud/spring-cloud-gateway) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spring-cloud-gateway/)</sub>

<a name="graphql-php"></a>
### #&#8288;201 [graphql-php](https://github.com/webonyx/graphql-php) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Nov 2026</sub>

**PHP implementation of the GraphQL specification, ported from graphql-js.**

graphql-php is a PHP library for building GraphQL servers, based on the JavaScript reference implementation graphql-js. It installs with Composer and is compliant with the October 2021 GraphQL specification, with September 2025 compliance in progress. It is a library rather than a starter app, so you wire it into your own HTTP framework.

- **+** Fully compliant with the October 2021 GraphQL specification
- **+** Semantic Versioning, with public API elements marked @api in PHPDoc
- **+** Examples directory with a README per example
- **+** Docs site includes a class reference; MIT license
- **−** Repository is planned to move to a new home
- **−** Only the latest version is actively developed; older ones mainly for sponsors
- **−** September 2025 specification compliance is still in progress
- **−** Library only: no HTTP server, UI or AI features included

<sub>no GPU · Needs PHP, Composer · [Repo](https://github.com/webonyx/graphql-php) · [📖 Docs ↗](https://webonyx.github.io/graphql-php) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphql-php/)</sub>

<a name="nornicdb"></a>
### #&#8288;202 [nornicdb](https://github.com/orneryd/nornicdb) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 935 · MIT · Nov 2026</sub>

**Neo4j-compatible graph database with vector search and historical reads.**

NornicDB is a graph database written in Go that accepts Cypher queries over Bolt and HTTP, so existing Neo4j drivers can connect. It combines graph traversal with vector and full-text retrieval, and keeps retained history through MVCC for historical reads. It runs as a server with CPU, CUDA, Metal or Vulkan builds, or embeds in a Go application.

- **+** Speaks Bolt and Cypher, so Neo4j drivers and a migration guide apply
- **+** Graph traversal, vector and full-text retrieval in a single database
- **+** MVCC with retained history allows reads of past state
- **+** Runs as a server or embeds as a Go library
- **−** Neo4j compatibility has its own guide; check Cypher coverage before migrating
- **−** README gives no inline benchmark numbers, only links to separate guides
- **−** Docker on macOS cannot use Metal; GPU needs a native install
- **−** Separate image per platform (arm64 Metal, amd64 CPU, CUDA, Vulkan) to choose from

<sub>GPU optional · Docker + Compose · Models: BGE embeddings (bundled in -bge images) · port 7474 · [Repo](https://github.com/orneryd/nornicdb) · [📖 Docs ↗](https://orneryd.github.io/NornicDB/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nornicdb/)</sub>

<a name="bex"></a>
### #&#8288;203 [bex](https://github.com/bex-co/bex) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 927 · Apache-2.0 · Nov 2026</sub>

**Open-source Render-style PaaS that deploys from Git, operable by agents via MCP.**

bex is a self-hostable platform-as-a-service written in Go that deploys Dockerfile or native-build projects (Go, Node.js, Python, Ruby, Rust, Elixir) from Git to HTTPS. It reads Render-style render.yaml Blueprints and exposes REST, GraphQL, MCP, a Render-compatible CLI and Kubernetes CRDs over one core. A Kubernetes operator runs workloads on Cluster API machines: Docker containers locally, Hetzner in production-shaped clusters. The README calls it an alpha, not ready for production.

- **+** Reads render.yaml Blueprints and reuses the upstream Render CLI commands
- **+** Dashboard, REST, GraphQL, MCP, CLI and CRDs all sit on one Go core
- **+** Covers managed Postgres with PITR, Valkey-compatible Key Value, cron jobs, workers and static sites
- **+** Render parity gaps are tracked in a documented evidence ledger
- **−** README warns it is not ready for production; APIs and config can change
- **−** Local quickstart needs kind, Cluster API, clusterctl and Go 1.25+; no Docker or compose install
- **−** Some capabilities need optional backing services and fail closed without them
- **−** Production-shaped clusters are described only for Hetzner machines via Cluster API

<sub>no GPU · Docker · Needs Docker or OrbStack, Go 1.25+, kubectl, kind, clusterctl, Cluster API, PostgreSQL, Zot registry · README: alternative to Heroku · [Repo](https://github.com/bex-co/bex) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bex/)</sub>

<a name="vercel"></a>
### #&#8288;204 [vercel](https://github.com/vercel/vercel) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: weak (24) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Nov 2026</sub>

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

<a name="fission"></a>
### #&#8288;205 [fission](https://github.com/fission/fission) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: weak (30) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · Apache-2.0 · Nov 2026</sub>

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

<a name="docker-node"></a>
### #&#8288;206 [docker-node](https://github.com/nodejs/docker-node) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · MIT · Nov 2026</sub>

**Source for the official Node.js Docker base images on Docker Hub.**

Dockerfiles and build automation for the official `node` images, which bundle Node.js and npm. Variants include the default buildpack-deps image, slim, alpine (musl), and Debian bookworm and trixie, plus a floating `lts` tag. It is a base image for Node.js apps, not an AI project or a starter, so the fit with this list is loose.

- **+** Maintained under the nodejs org, with new images built automatically when Node.js releases
- **+** Variants for different size and libc needs: default, slim, alpine (musl), bookworm, trixie
- **+** `lts` floating tag selects the Active LTS release, and combines with variants like `lts-slim`
- **+** Includes a usage guide with a multi-stage pattern for smaller images without npm or yarn
- **−** Not an AI project and not a starter app; it only provides a runtime base image
- **−** Alpine images use musl and omit git and bash, so glibc-built apps may need gcompat
- **−** Alpine musl builds for amd64 are Node.js tier Experimental; other architectures are untested before release
- **−** New tags can appear on Docker Hub with missing architectures for hours, causing 'no matching manifest'

<sub>no GPU · Needs Docker · [Repo](https://github.com/nodejs/docker-node) · [🌐 Site ↗](https://hub.docker.com/_/node) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/docker-node/)</sub>

<a name="medoo"></a>
### #&#8288;207 [medoo](https://github.com/catfan/medoo) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · MIT · Oct 2026</sub>

**Single-file PHP database library with a query builder over PDO.**

Medoo is a PHP library that wraps PDO with a array-based API for insert, select and other queries, using prepared statements. It supports MySQL, MariaDB, PostgreSQL, SQLite, MSSQL, Oracle and Sybase, and installs through Composer. It is not an AI project and has no AI features; it is a general data-access layer.

- **+** Single-file package with minimal dependencies; needs only PHP 7.3+ and PDO
- **+** Supports MySQL, MariaDB, PostgreSQL, SQLite, MSSQL, Oracle and Sybase
- **+** Documentation available in 16 languages at medoo.in
- **+** MIT license; works alongside Laravel, CodeIgniter, Yii and Slim
- **−** No AI, LLM or vector-search features; a general PHP query builder only
- **−** Library, not a backend: no auth, storage or API server included
- **−** Not an ORM per the README; no migrations or schema tooling mentioned
- **−** Ships no Docker image or compose file

<sub>no GPU · Needs PHP 7.3 or later, PDO extension, Composer · [Repo](https://github.com/catfan/medoo) · [📖 Docs ↗](https://medoo.in) · [🌐 Site ↗](https://medoo.in) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/medoo/)</sub>

<a name="ergo"></a>
### #&#8288;208 [ergo](https://github.com/ergo-services/ergo) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Nov 2026</sub>

**Actor model framework for Go with supervision trees and clustering.**

Ergo is a Go framework modeled on Erlang/OTP. Isolated processes exchange messages, are restarted by supervision trees, and are addressed the same way locally or across nodes. It ships an Observer web UI with an MCP endpoint, Prometheus metrics, tracing, and Erlang distribution protocol support. It is a general distributed-systems library, not an AI-specific project.

- **+** Zero external dependencies; pure Go, requires Go 1.21 or newer
- **+** Supervision trees with One For One, All For One, Rest For One strategies
- **+** Same messaging API locally and across nodes; README reports 25M+ msg/sec local on a 32-core Threadripper
- **+** Observer web UI plus MCP endpoint for inspecting a running cluster from AI clients
- **−** Requires learning actor and OTP concepts; not a drop-in replacement for goroutines
- **−** Go-only; mixed-language clusters work only with Erlang/Elixir via the Erlang protocol
- **−** Not an AI framework; agent patterns must be built on the actor primitives
- **−** Throughput numbers come from the project's own benchmark on specific hardware

<sub>no GPU · [Repo](https://github.com/ergo-services/ergo) · [📖 Docs ↗](https://docs.ergo.services) · [🌐 Site ↗](https://ergo.services) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ergo/)</sub>

<a name="memgraph"></a>
### #&#8288;209 [memgraph](https://github.com/memgraph/memgraph) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · custom license · Nov 2026</sub>

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

<sub>GPU optional · [Repo](https://github.com/memgraph/memgraph) · [📖 Docs ↗](https://memgraph.com/docs) · [🌐 Site ↗](https://memgraph.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/memgraph/)</sub>

<a name="octelium"></a>
### #&#8288;210 [octelium](https://github.com/octelium/octelium) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · AGPL-3.0 · Nov 2026</sub>

**Self-hosted zero trust access platform with VPN, tunnels, API and AI gateway.**

Octelium is a Kubernetes-based, identity-aware proxy platform that gives humans and workloads per-request, L7-aware access to private and public resources over WireGuard/QUIC tunnels or clientless. It covers use cases from remote-access VPN and ngrok-style tunnels to an API gateway, LLM/MCP gateway and a PaaS-like container deployment. Policies are written in CEL and OPA, and upstream credentials are injected so users never handle API keys.

- **+** Secretless access to HTTP APIs, SSH, Kubernetes and PostgreSQL/MySQL without distributing credentials
- **+** Per-request ABAC with CEL and OPA policy-as-code; no standing admin user
- **+** Single-node install script; declarative config through octeliumctl fits GitOps
- **+** Exports every request log to OpenTelemetry OTLP receivers
- **−** Requires a Kubernetes cluster; the installer targets a dedicated Linux VM
- **−** Web dashboard, SCIM and SIEM integrations are in the separate source-available enterprise edition
- **−** Pre-v1.0 and maintained by one developer
- **−** Pull requests are not accepted; the QUIC tunnel is experimental

<sub>RAM ≥ 2 GB · no GPU · Needs Kubernetes, Linux VM or server (Ubuntu 24.04+ or Debian 12+), Domain name · [Repo](https://github.com/octelium/octelium) · [▶️ Demo ↗](https://github.com/octelium/playground) · [📖 Docs ↗](https://octelium.com/docs/octelium/latest/overview/intro) · [🌐 Site ↗](https://octelium.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/octelium/)</sub>

<a name="kubeblocks"></a>
### #&#8288;211 [kubeblocks](https://github.com/apecloud/kubeblocks) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (34) · Freshness: active (91) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · AGPL-3.0 · Nov 2026</sub>

**Kubernetes operator managing many database engines through one set of CRDs.**

KubeBlocks is a Go-based Kubernetes operator that uses a unified Cluster CRD to run and manage database engines such as PostgreSQL, MySQL, Redis, MongoDB, Kafka, Milvus and ClickHouse. It handles day-2 operations like upgrades, scaling, backup, continuous backup and point-in-time recovery. New engines are added by writing addons, and a kbcli command line tool complements kubectl.

- **+** One Cluster API covers 35 engines, including Milvus, Qdrant and Weaviate vector databases
- **+** Full backups, continuous backups and point-in-time recovery
- **+** Prometheus integration with Grafana templates
- **+** New engines added through addons, without a dedicated operator
- **−** README maturity badge says alpha
- **−** AGPL-3.0 license may restrict some commercial use
- **−** Requires a Kubernetes cluster; not usable standalone
- **−** Engine addons live in a separate kubeblocks-addons repository

<sub>no GPU · Docker · Needs Kubernetes, Prometheus, Grafana · [Repo](https://github.com/apecloud/kubeblocks) · [📖 Docs ↗](https://kubeblocks.io/docs/preview/user_docs/overview/install-kubeblocks) · [🌐 Site ↗](https://kubeblocks.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubeblocks/)</sub>

<a name="rbatis"></a>
### #&#8288;212 [rbatis](https://github.com/rbatis/rbatis) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

**Rust ORM and dynamic SQL compiler using compile-time code generation.**

Rbatis is a Rust ORM that compiles dynamic SQL written in py_sql, MyBatis-style html_sql or raw SQL into native Rust through procedural macros at build time. It generates CRUD methods with a macro and runs on async Tokio drivers for MySQL, PostgreSQL, SQLite, MSSQL and others. It is not an AI project; the README links rbdc-mcp and rbatis-skill as separate AI add-ons.

- **+** Dynamic SQL is translated at compile time, so no runtime SQL interpretation
- **+** Drivers for MySQL, PostgreSQL, SQLite, MSSQL, DuckDB, Turso, plus community Oracle and TDengine
- **+** Three SQL styles: py_sql, MyBatis-like html_sql and raw SQL
- **+** Choice of connection pools: FastPool (default), Deadpool, MobcPool
- **−** Oracle and TDengine drivers live in separate third-party repositories
- **−** Rust only; py_sql and html_sql templates add macro syntax to learn
- **−** Not an AI tool; relevant here only through the separate rbdc-mcp add-on
- **−** Benchmarks are single-thread numbers from the author's own machines

<sub>no GPU · Needs Rust toolchain, Tokio, A database such as MySQL, PostgreSQL, SQLite or MSSQL · [Repo](https://github.com/rbatis/rbatis) · [📖 Docs ↗](https://docs.rs/rbatis/) · [🌐 Site ↗](https://rbatis.github.io/rbatis.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rbatis/)</sub>

<a name="doco-cd"></a>
### #&#8288;213 [doco-cd](https://github.com/kimdre/doco-cd) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · Apache-2.0 · Nov 2026</sub>

**GitOps deployment tool for Docker Compose projects and Swarm stacks.**

doco-cd watches Git repositories or OCI artifacts and deploys or updates Docker Compose projects and Swarm stacks, triggered by webhooks or polling. It supports multiple Docker hosts via Docker Contexts, external secret providers, SOPS encryption, sync windows and Prometheus metrics. The README positions it as a lightweight alternative to Portainer or ArgoCD for plain Docker hosts.

- **+** Webhook and cron-scheduled polling triggers, with timezone-aware sync windows
- **+** Deploys to multiple Docker hosts through Docker Contexts
- **+** Supports SOPS encryption and external secret providers
- **+** Exposes Prometheus metrics, a REST API and an MCP server
- **−** No web UI described in the README; configuration is declarative
- **−** Targets Docker Compose and Swarm only, not Kubernetes
- **−** Most details live in external docs rather than the README

<sub>no GPU · Docker + Compose · Needs Docker, Git provider · [Repo](https://github.com/kimdre/doco-cd) · [📖 Docs ↗](https://doco.cd/latest/) · [🌐 Site ↗](https://doco.cd/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/doco-cd/)</sub>

<a name="kratos"></a>
### #&#8288;214 [kratos](https://github.com/go-kratos/kratos) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: weak (29) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<a name="gitpod"></a>
### #&#8288;215 [gitpod](https://github.com/gitpod-io/gitpod) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (72) · Freshness: recent (70) · Maintenance: fair (62) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · AGPL-3.0 · Nov 2026</sub>

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

<a name="couchdb"></a>
### #&#8288;216 [couchdb](https://github.com/apache/couchdb) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="hanami"></a>
### #&#8288;217 [hanami](https://github.com/hanami/hanami) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Nov 2026</sub>

**Full-stack Ruby web framework built from small, separable libraries.**

Hanami is a Ruby web framework that combines a Rack-compatible router, actions, views, a database layer and asset management. This repository holds the glue that ties those libraries together, and each library can also be used on its own. It has no AI features; it fits this list only as a general backend framework to build an app on.

- **+** Router, action, view, db and assets libraries work independently or together
- **+** Database layer includes migrations, repositories, relations and structs
- **+** Rack-compatible router and actions fit the existing Rack ecosystem
- **+** Installs as a gem; `hanami new` scaffolds an app with a dev server
- **−** No AI, model or agent features; not an AI starter
- **−** Ruby only, so it suits teams already using Ruby
- **−** No auth, billing or admin is listed; those must be added separately

<sub>no GPU · Needs Ruby, Bundler · port 2300 · [Repo](https://github.com/hanami/hanami) · [📖 Docs ↗](https://guides.hanamirb.org/getting-started/) · [🌐 Site ↗](https://hanamirb.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hanami/)</sub>

<a name="csghub"></a>
### #&#8288;218 [csghub](https://github.com/opencsgs/csghub) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · Apache-2.0 · Nov 2026</sub>

**Self-hosted hub for models, datasets and Spaces, like a private Hugging Face.**

CSGHub stores, versions and distributes LLM assets such as models, datasets, Spaces and code. Assets are reachable through a web UI, the git command line, a chatbot or the CSGHub SDK, and OpenAPIs allow integration with existing systems. It can be installed on-premise with Docker Compose or a Helm chart for offline use.

- **+** Works as an on-premise, Hugging Face-style hub for models, datasets and Spaces
- **+** Assets accessible via web UI, git CLI, SDK and OpenAPIs
- **+** Documented install paths for Docker Compose and Helm on Kubernetes
- **+** Apache-2.0 licensed with a recent commit and release
- **−** README gives no RAM, GPU or disk requirements for a self-hosted install
- **−** Install steps live in external docs, not in the README
- **−** Several listed features (annotation, Copilot, HA) are named but not described
- **−** Repo is Vue-based; README does not say where backend services live

<sub>Docker · Needs Docker Compose or Helm/Kubernetes · Models: DeepSeek, Llama · [Repo](https://github.com/opencsgs/csghub) · [▶️ Demo ↗](https://opencsg.com) · [📖 Docs ↗](https://opencsg.com/docs/csghub/101/introduction) · [🌐 Site ↗](https://opencsg.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/csghub/)</sub>

<a name="nestjs"></a>
### #&#8288;219 [nestjs](https://github.com/golevelup/nestjs) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Nov 2026</sub>

**NestJS modules for RabbitMQ, Stripe, Hasura, Pub/Sub and webhooks.**

Monorepo of npm packages under the @golevelup scope that add integrations and utilities to NestJS apps. Packages cover RabbitMQ (RPC and pub/sub), Google Cloud Pub/Sub, Graphile Worker, Stripe client and webhooks, Hasura event handlers, a GraphQL client, provider discovery, and Jest testing helpers. It contains no AI features, so it fits this list only loosely as backend plumbing.

- **+** Separate npm packages per integration, so you install only what you use
- **+** Covers RabbitMQ RPC and pub/sub, Stripe webhooks, and Hasura events
- **+** Includes a discovery module and ts-jest helpers for testing NestJS apps
- **+** MIT licensed, with per-package changelogs and changesets-based releases
- **−** No AI, LLM, or agent functionality; unrelated to the rest of this list
- **−** Only usable inside NestJS applications, in TypeScript
- **−** Library collection, not a deployable backend or starter template
- **−** README gives only one-line descriptions; usage lives in per-package folders

<sub>no GPU · Compose · Needs NestJS, RabbitMQ, Stripe, Hasura, Google Cloud Pub/Sub, Graphile Worker · [Repo](https://github.com/golevelup/nestjs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nestjs/)</sub>

<a name="mall"></a>
### #&#8288;220 [mall](https://github.com/macrozheng/mall) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (99) · Freshness: recent (70) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 85k · Apache-2.0 · Sep 2026</sub>

**Spring Boot e-commerce backend with admin and storefront APIs.**

mall is a Java e-commerce system built on Spring Boot 3.5, JDK 17 and MyBatis. It splits into mall-admin (back-office API), mall-portal (storefront API) and mall-search (Elasticsearch product search), with Vue admin and uni-app frontends in separate repos. It contains no AI features, so it fits this list only as a general application backend.

- **+** Covers products, orders, members, promotions, content and permissions in one codebase
- **+** Live demos for both the admin console and the mobile storefront
- **+** Separate Spring Cloud Alibaba variant (mall-swarm) and a dev-v2 branch for Spring Boot 2.7/JDK 8
- **+** Apache-2.0 licensed, with extensive tutorials and video guides
- **−** No AI functionality; it is a conventional shop backend
- **−** Needs MySQL, Redis, MongoDB, RabbitMQ and Elasticsearch for the full stack
- **−** Docs and community channels are mostly in Chinese
- **−** No Dockerfile or compose file in the repo; deployment is in external tutorials

<sub>no GPU · Needs MySQL 5.7, Redis 7.0, MongoDB 5.0, RabbitMQ 3.10.5, Elasticsearch 7.17.3, Nginx 1.22, MinIO or Aliyun OSS, Logstash and Kibana (optional) · [Repo](https://github.com/macrozheng/mall) · [▶️ Demo ↗](https://www.macrozheng.com/admin/index.html) · [📖 Docs ↗](https://www.macrozheng.com) · [🌐 Site ↗](https://www.macrozheng.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mall/)</sub>

<a name="goravel"></a>
### #&#8288;221 [goravel](https://github.com/goravel/goravel) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (46) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · MIT · Nov 2026</sub>

**Laravel-style web application framework for Go.**

Goravel is a Go web framework that mirrors Laravel's structure and APIs, so PHP developers can reuse their conventions. It ships modules for HTTP routing, ORM, migrations, queues, task scheduling, JWT and session auth, cache, mail, gRPC and an Artisan-style CLI. It is a general backend scaffold with no AI-specific features.

- **+** Broad built-in module set: ORM, migrations, queues, scheduler, mail, validation, gRPC
- **+** Laravel-like API and Artisan console lower the learning curve for PHP developers
- **+** Auth with JWT and session drivers, plus gates and policies for authorization
- **+** MIT licensed, with a separate docs site and example repo
- **−** No AI or model integration; it is a generic web framework
- **−** Laravel-style facades and conventions may feel unidiomatic to Go developers
- **−** Extensions come from separate packages rather than the core

<sub>no GPU · Docker + Compose · Needs Go · [Repo](https://github.com/goravel/goravel) · [📖 Docs ↗](https://www.goravel.dev) · [🌐 Site ↗](https://www.goravel.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goravel/)</sub>

<a name="squidex"></a>
### #&#8288;222 [squidex](https://github.com/squidex/squidex) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

**Headless CMS with REST API, OData filtering and Swagger, built on ASP.NET Core.**

Squidex is a headless content management system written in C# on ASP.NET Core with a CQRS architecture. It exposes content through an API with OData filters and Swagger definitions, and leaves the front end to you. It stores data in MongoDB, PostgreSQL, MySQL or SQL Server and has no AI features described in the README.

- **+** API with OData filtering and Swagger definitions for client generation
- **+** Supports MongoDB, PostgreSQL, MySQL or SQL Server as the data store
- **+** Deployment guides for Azure, AWS, GCP, Kubernetes, Docker, Heroku, Render, Vultr and IIS
- **+** MIT license, with an optional hosted cloud version
- **−** No built-in front end; you build the UI on top of the API
- **−** Documentation is described as work in progress
- **−** Requires the .NET 8 SDK for development, plus Node.js
- **−** No AI features or AI-specific starters in the README

<sub>no GPU · Docker · Needs MongoDB, PostgreSQL, MySQL or SQL Server, .NET 8 SDK (development), Node.js (development only) · [Repo](https://github.com/squidex/squidex) · [📖 Docs ↗](https://docs.squidex.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/squidex/)</sub>

<a name="dante-cloud"></a>
### #&#8288;223 [dante-cloud](https://github.com/dromara/dante-cloud) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 972 · Apache-2.0 · Nov 2026</sub>

**Spring Cloud microservice base that also runs as a monolith from one codebase.**

Dante Cloud is a Java microservice foundation built on Spring Boot 4.1, Spring Cloud 2025.1.4 and Spring Authorization Server. The same code deploys either as microservices or as a single monolith. It includes a gateway, OAuth2 authentication, permission management, messaging, object storage and workflow modules. Spring AI 2.0.2 appears in the badges, but the README describes no AI features.

- **+** One codebase switches between microservice and monolith deployment
- **+** OAuth2 via Spring Authorization Server, with Passkey login and method-level permissions
- **+** Infrastructure adapters for Spring Cloud Alibaba, Tencent or native, with Nacos 3.2.4
- **+** Apache-2.0 license; release on 2026-10-26
- **−** Requires JDK 25+; older Spring Boot branches are no longer maintained
- **−** README and docs are in Chinese
- **−** Supplementary terms restrict removing author or copyright notices and re-open-sourcing
- **−** Core library and UIs live in separate repos; no Docker or compose files detected

<sub>no GPU · Needs JDK 25+, Nacos, Dante Engine, Spring Boot Admin, EMQX, Minio · [Repo](https://github.com/dromara/dante-cloud) · [📖 Docs ↗](https://www.herodotus.cn) · [🌐 Site ↗](https://www.herodotus.cn) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dante-cloud/)</sub>

<a name="cdk-blocks"></a>
### #&#8288;224 [cdk-blocks](https://github.com/aws/cdk-blocks) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 412 · Apache-2.0 · Nov 2026</sub>

**TypeScript backend blocks that run locally and deploy to AWS through CDK.**

AWS CDK Blocks is a TypeScript toolkit where each Block (KVStore, Database, Auth, FileBucket, AsyncJob, Agent, KnowledgeBase and others) bundles runtime code, a local implementation and CDK infrastructure. Node conditional exports select in-memory or filesystem storage in development, CDK constructs at synth time, and AWS SDK calls on Lambda. A scaffolder offers templates such as react, nextjs, sql, auth and amplify.

- **+** Full app runs locally with npm run dev, no AWS account or credentials needed
- **+** Same code deploys to AWS; Blocks synthesize CloudFormation through CDK
- **+** Web types flow end to end without code generation; native clients generated from a spec
- **+** Covers auth, data, jobs, email, realtime and observability, plus Agent and KnowledgeBase
- **−** Deploys only to AWS; Blocks map to AWS services such as DynamoDB and Lambda
- **−** Requires Node.js 22+ and npm 10+
- **−** Native Kotlin, Swift and Dart clients talk to the backend over JSON-RPC
- **−** Agent and KnowledgeBase blocks are listed without model or provider details

<sub>no GPU · Needs Node.js 22+, npm 10+, AWS account (deploy only) · port 3000 · [Repo](https://github.com/aws/cdk-blocks) · [📖 Docs ↗](https://docs.aws.amazon.com/blocks/latest/devguide/what-is-blocks.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cdk-blocks/)</sub>

<a name="faas"></a>
### #&#8288;225 [faas](https://github.com/openfaas/faas) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (86) · Freshness: recent (77) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · custom license · Oct 2026</sub>

**Serverless functions platform with auto-scaling and language templates.**

OpenFaaS packages code or an existing binary as an OCI image and runs it as an HTTP or event-triggered function with auto-scaling (including to zero) and metrics. Functions are scaffolded with faas-cli from templates (Node.js, Python 3, Go and others) and defined in YAML. This repository is the Community Edition, licensed for non-commercial use and a 60-day commercial PoC; production use requires a paid tier.

- **+** Templates for many languages, or any Dockerfile or existing binary as a function
- **+** Auto-scales on demand, including to zero, with built-in metrics
- **+** Runs on Kubernetes, OpenShift or faasd, which needs no Kubernetes
- **+** Triggers from HTTP, Apache Kafka and AWS SQS, plus async queueing
- **−** CE license bars commercial use beyond a 60-day PoC; production needs a paid tier
- **−** CE has basic features; the multi-tenant dashboard is only in paid editions
- **−** CE gets limited maintenance; product development happens in private repos
- **−** General serverless platform; no model serving or LLM features described

<sub>Needs Kubernetes, OpenShift or faasd, OCI/Docker images, faas-cli · [Repo](https://github.com/openfaas/faas) · [📖 Docs ↗](https://docs.openfaas.com) · [🌐 Site ↗](https://www.openfaas.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/faas/)</sub>

<a name="airbyte"></a>
### #&#8288;226 [airbyte](https://github.com/airbytehq/airbyte) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (83) · Freshness: active (81) · Maintenance: patchy (38) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

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

<a name="tenancy"></a>
### #&#8288;227 [tenancy](https://github.com/archtechx/tenancy) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Nov 2026</sub>

**Laravel package that adds multi-tenancy without changing application code.**

stancl/tenancy is a PHP package that makes an existing Laravel app multi-tenant. It identifies tenants by hostname, including second-level domains, and switches the database connection per tenant without model traits or replacing Laravel classes such as Cache and Storage. The README points to v4 documentation on a separate site.

- **+** No model traits needed to switch the database connection per tenant
- **+** Cache, Storage and similar Laravel classes are kept, not replaced
- **+** Built-in hostname tenant identification, including second-level domains
- **+** MIT license with CI workflow and a dedicated documentation site
- **−** Laravel only; not usable in other PHP frameworks
- **−** Not an AI project and has no AI features
- **−** README badge says Laravel 10.x while its alt text says 11.x
- **−** README has no install steps or tenancy models; those are in external docs

<sub>no GPU · Docker + Compose · Needs Laravel, PHP · [Repo](https://github.com/archtechx/tenancy) · [📖 Docs ↗](https://v4.tenancyforlaravel.com) · [🌐 Site ↗](https://tenancyforlaravel.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tenancy/)</sub>

<a name="data-client"></a>
### #&#8288;228 [data-client](https://github.com/reactive/data-client) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Nov 2026</sub>

**Normalized client-side data cache for React with REST, GraphQL and websocket support.**

TypeScript library that defines API resources with schemas (Entity, Collection, Query) and binds them to React components through hooks like useSuspense and useLive. It keeps a normalized cache with optimistic updates and Suspense, and runs in Next.js, React Native, Expo and Vue. It is a frontend data layer, not an AI project, though it ships setup skills and plugins for Claude Code, Cursor and Codex.

- **+** Normalized cache gives shared entities and referential equality across components without updater functions
- **+** Covers REST, GraphQL, websockets and SSE through one schema-driven resource definition
- **+** Built-in fixtures, MockResolver and Storybook mocking for testing data-dependent components
- **+** Ships agent setup skills and plugins for Claude Code, Cursor and Codex
- **−** Client-side library only; does not provide a backend, database or hosting
- **−** Not an AI project; fits this list only through its agent setup skills
- **−** Requires learning its own schema and Manager concepts instead of plain fetch hooks
- **−** README lists Vue support but all examples use React

<sub>no GPU · Needs React, npm · [Repo](https://github.com/reactive/data-client) · [▶️ Demo ↗](https://stackblitz.com/github/reactive/data-client/tree/master/examples/todo-app?file=src%2Fpages%2FHome%2FTodoList.tsx) · [📖 Docs ↗](https://dataclient.io/docs) · [🌐 Site ↗](https://dataclient.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/data-client/)</sub>

<a name="openchoreo"></a>
### #&#8288;229 [openchoreo](https://github.com/openchoreo/openchoreo) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Nov 2026</sub>

**Kubernetes developer platform with Backstage portal, CI, GitOps and observability.**

OpenChoreo is a CNCF Sandbox developer platform for Kubernetes, written in Go. A control plane maps high-level abstractions (components, endpoints, dependencies, environments) onto Kubernetes resources, alongside data, observability and optional CI planes. Platform teams define ComponentTypes, Traits and Workflows as CRDs, and developers use a Backstage-based portal, CLI, GitOps or AI agents.

- **+** Platform API is Kubernetes CRDs: ComponentTypes, Traits and Workflows, no custom controllers
- **+** Separate control, data, observability and optional CI planes operate independently
- **+** Default CI uses Buildpacks and Argo Workflows; deploys from source or prebuilt image
- **+** Ships Backstage portal, RBAC and observability, so less glue to assemble
- **−** Requires a Kubernetes cluster; heavier to run than a single-host PaaS
- **−** Opinionated component and platform model has to be learned and mapped to
- **−** Not a general backend or database host; scope is deploying and operating workloads
- **−** CNCF Sandbox stage; roadmap items are still being scheduled by quarter

<sub>no GPU · Docker · Needs Kubernetes, Backstage, Argo Workflows, Buildpacks · [Repo](https://github.com/openchoreo/openchoreo) · [📖 Docs ↗](https://openchoreo.dev/docs/getting-started/quick-start-guide/) · [🌐 Site ↗](https://openchoreo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openchoreo/)</sub>

<a name="conduit"></a>
### #&#8288;230 [conduit](https://github.com/conduitplatform/conduit) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 928 · MIT · Nov 2026</sub>

**Modular backend with auth, database, storage and generated REST/GraphQL APIs.**

Conduit is a self-hosted backend built from ready-made modules: authentication, authorization, database, storage, email, SMS, push notifications, chat, forms and a router that exposes REST, GraphQL and WebSockets. Schemas defined in the database module get auto-generated CRUD endpoints, backed by MongoDB or PostgreSQL. A CLI bootstraps a local deployment with an admin dashboard, and Kubernetes instructions are provided.

- **+** Auto-generated CRUD endpoints with Swagger and GraphQL docs from database schemas
- **+** Database module supports both MongoDB and PostgreSQL
- **+** CLI bootstrap includes an admin dashboard for local deployments
- **+** Docker and Kubernetes deployment instructions are included
- **−** Embeddings module is opt-in, disabled by default and not in standalone v1
- **−** Local deployment starts with default admin/admin credentials
- **−** Windows users must run the CLI through WSL
- **−** Bootstrap installs the CLI via a curl-piped shell script

<sub>no GPU · Docker + Compose · Needs Docker, Docker Compose, MongoDB or PostgreSQL · [Repo](https://github.com/conduitplatform/conduit) · [📖 Docs ↗](https://getconduit.dev/docs/overview/intro) · [🌐 Site ↗](https://getconduit.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/conduit/)</sub>

<a name="gun"></a>
### #&#8288;231 [gun](https://github.com/amark/gun) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: widely used (81) · Freshness: recent (70) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · custom license · Nov 2026</sub>

**Decentralized realtime graph database that syncs peer-to-peer in browsers and Node.**

GUN is a JavaScript graph synchronization engine that stores key/value, document, table and graph data locally and merges it across peers using CRDT conflict resolution. It runs in browsers and Node.js, with an optional SEA module for user auth and encryption, and relay peers deployable to Heroku, Docker or a Linux host. The README claims about 9KB gzipped and 20M+ API ops/sec.

- **+** Runs in browser and Node.js; about 9KB gzipped per the README
- **+** Offline-first with realtime peer-to-peer sync and CRDT conflict resolution
- **+** SEA module adds user auth and end-to-end encryption
- **+** Graph model covers key/value, documents and tables, including circular references
- **−** Last tagged release is 2019-04-15 despite recent commits
- **−** License is detected as NOASSERTION; check terms before use
- **−** Docker image is community contributed and may lack security updates
- **−** Node and React Native need a WebCrypto shim to use SEA

<sub>no GPU · Docker · Needs Node.js, npm, @peculiar/webcrypto (Node/React Native, for SEA) · [Repo](https://github.com/amark/gun) · [▶️ Demo ↗](http://try.axe.eco/) · [📖 Docs ↗](https://gun.eco/docs/API) · [🌐 Site ↗](https://gun.eco/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gun/)</sub>

<a name="neo4j"></a>
### #&#8288;232 [neo4j](https://github.com/neo4j/neo4j) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (79) · Freshness: recent (70) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · GPL-3.0 · Oct 2026</sub>

**Graph database with ACID transactions, storing nodes and relationships.**

Neo4j is a Java graph database that stores data as nodes and relationships and queries it with a graph query language, with ACID transactions. This repository holds the GPL-3.0 Community Edition, built with Maven and started with bin/neo4j-admin server start on localhost:7474. Enterprise features are closed source and not in this repository.

- **+** ACID transactions on a native graph model of nodes and relationships
- **+** Community Edition is GPL-3.0 and builds from source with Maven
- **+** Runs as standalone server, via Neo4j Desktop, or as managed Aura service
- **+** Graph query and visualization tools work with self-managed instances
- **−** Enterprise Edition components are closed source and need a commercial license
- **−** GPL-3.0 may constrain embedding in proprietary software
- **−** Building needs Maven 3.9.11+, a recent JDK and a raised open-file limit
- **−** No Docker or compose setup described in the README

<sub>no GPU · Needs Java 21 (JDK), Apache Maven 3.9.11+ (build only) · port 7474 · [Repo](https://github.com/neo4j/neo4j) · [🌐 Site ↗](https://neo4j.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neo4j/)</sub>

<a name="serverpod"></a>
### #&#8288;233 [serverpod](https://github.com/serverpod/serverpod) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · BSD-3-Clause · Nov 2026</sub>

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

<a name="fjall"></a>
### #&#8288;234 [fjall](https://github.com/fjall-rs/fjall) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

**Embeddable LSM-tree key-value storage engine for Rust applications.**

Fjall is a log-structured key-value store written in safe Rust, used as a library via `cargo add fjall`. It offers a thread-safe BTreeMap-like API with range and prefix iteration, multiple keyspaces with cross-keyspace atomicity, LZ4 compression, and optional serializable transactions. It is not a database server and has no query language. It has no AI features.

- **+** 100% safe, stable Rust; embeds in-process with no server to run
- **+** Optimistic or single-writer serializable transactions over an MVCC LSM-tree
- **+** Optional key-value separation for large blobs and custom compaction filters
- **+** Stable disk format; breaking changes come with a major version and migration path
- **−** Rust-only library; no server, network protocol or query language
- **−** A database cannot be opened by multiple processes at once
- **−** Default writes reach OS buffers only; disk durability needs an explicit persist call
- **−** Not an AI project; fits this list only loosely as a storage backend

<sub>no GPU · [Repo](https://github.com/fjall-rs/fjall) · [📖 Docs ↗](https://docs.rs/fjall) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fjall/)</sub>

<a name="wrangler-action"></a>
### #&#8288;235 [wrangler-action](https://github.com/cloudflare/wrangler-action) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Sep 2026</sub>

**GitHub Action that runs Wrangler to deploy Cloudflare Workers and Pages.**

A GitHub Action that installs and runs Wrangler (v4 by default, v3 selectable) in a workflow to deploy Workers or Pages projects. It authenticates with a Cloudflare API token, can set Worker secrets, run pre and post commands, and expose deployment URLs and command output to later steps. It also supports Workers Previews and GitHub Deployments.

- **+** Accepts any Wrangler command, including pages deploy, versions upload and preview
- **+** Outputs deployment-url, pages-deployment-alias-url and command-output for later workflow steps
- **+** Detects npm, yarn, pnpm or bun from lockfiles; wranglerVersion pins the CLI version
- **+** Pushes Worker secrets from GitHub secrets via the secrets and environment inputs
- **−** Deploys to Cloudflare only, so it does not help with other hosts
- **−** Global API key and email auth are not supported, only API tokens
- **−** Workers Previews need Wrangler 4.136.3 or newer
- **−** Version tags need the v prefix, so older 3.x.x syntax breaks

<sub>no GPU · Needs GitHub Actions, Cloudflare account and API token, Wrangler (npm) · [Repo](https://github.com/cloudflare/wrangler-action) · [📖 Docs ↗](https://developers.cloudflare.com/workers/wrangler/ci-cd/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wrangler-action/)</sub>

<a name="bob"></a>
### #&#8288;236 [bob](https://github.com/stephenafamo/bob) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Go SQL toolkit with query builder, generated models, factories and typed queries.**

Bob is a set of Go packages that starts as a dialect-specific query builder and can be adopted step by step up to generated ORM models, test factories and sqlc-style typed query code. All layers support Postgres, MySQL/MariaDB and SQLite. It is a general database library with no AI features, so it fits this list only as a backend building block.

- **+** Adoptable in layers, from raw query builder to generated ORM and factories
- **+** Hand-written builder per dialect for Postgres, MySQL/MariaDB and SQLite
- **+** Generates factories that create dependent rows for tests
- **+** Generates typed Go code from hand-written SQL, like sqlc
- **−** Go only; no support for other languages
- **−** Supports only three databases: Postgres, MySQL/MariaDB, SQLite
- **−** Query builder alone gives no type safety without generated mods
- **−** No AI features; it is a general SQL library

<sub>no GPU · Needs Postgres, MySQL/MariaDB or SQLite database · [Repo](https://github.com/stephenafamo/bob) · [📖 Docs ↗](https://bob.stephenafamo.com/docs) · [🌐 Site ↗](https://bob.stephenafamo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bob/)</sub>

<a name="nuxt-hub-core"></a>
### #&#8288;237 [nuxt-hub/core](https://github.com/nuxt-hub/core) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Nov 2026</sub>

**Nuxt module adding SQL database, blob storage, cache and KV to Nuxt apps.**

NuxtHub (@nuxthub/core) is a Nuxt module that adds optional server-side features to a Nuxt app: a SQL database with automatic migrations, file storage, a cache layer for pages, API routes and server functions, and a globally accessible key-value store. It is distributed on npm and documented at hub.nuxt.com. The README does not name the underlying providers.

- **+** Covers SQL, blob, cache and KV through one Nuxt module
- **+** SQL database has automatic migrations
- **+** MIT licensed, with a release on 2026-10-27
- **+** Templates and a separate CLI are provided
- **−** Tied to Nuxt; not usable with other frameworks
- **−** Legacy 0.9 version lives on a separate branch and docs site
- **−** No AI features; AI use cases need separate wiring

<sub>no GPU · [Repo](https://github.com/nuxt-hub/core) · [📖 Docs ↗](https://hub.nuxt.com/docs/getting-started/installation) · [🌐 Site ↗](https://hub.nuxt.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nuxt-hub-core/)</sub>

<a name="h5i"></a>
### #&#8288;238 [h5i](https://github.com/h5i-dev/h5i) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 933 · Apache-2.0 · Nov 2026</sub>

**Rust web framework with Lean 4 verifiable kernels and a red-teaming CLI.**

h5i is an Axum-based Rust web framework (h5i-app) that separates application logic into a kernel, translates it to Lean 4 with Aeneas, and lets you prove properties about it. The same kernel can run on servers, on bare-metal devices through a no_std HTTP/1.1 server, and on GPUs with CPU fallback. A separate CLI covers browser automation, HTTP replay, recon crawling, YAML security tests for CI, sandboxes for running agents, and a local dashboard.

- **+** Rust application logic can be extracted to Lean 4 and proved with h5i app prove
- **+** Same kernel targets servers, no_std embedded devices and GPUs with CPU fallback
- **+** Axum-compatible, so it deploys to Cloudflare Workers, Vercel and Fly.io
- **+** Red-team, test and sandbox tooling works without adopting h5i-app
- **−** Formal verification requires Lean 4 and Aeneas knowledge, a steep learning curve
- **−** Framework crate is at version 0.5.6, so the API may still change
- **−** Install is a curl-piped shell script rather than a plain cargo install
- **−** Scope spans framework, pentest tooling and sandboxes, which makes it broad to adopt

<sub>GPU optional · Docker · Needs Lean 4, Aeneas, Postgres (optional feature) · [Repo](https://github.com/h5i-dev/h5i) · [🌐 Site ↗](https://h5i.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/h5i/)</sub>

<a name="et"></a>
### #&#8288;239 [et](https://github.com/egametang/et) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 10.0k · custom license · Aug 2026</sub>

**C# Unity and .NET MMO game framework with AI coding skills and analyzers.**

ET10 is a C# framework for online games, with a Unity client and a distributed .NET server that share logic code. It uses Fibers with actor messaging, service discovery and hot reload. It adds AI harness packages: skills, Roslyn analyzers that constrain generated code, a multi-bot test framework and a Unity bridge with 68 editor commands.

- **+** Client and server share C# code, so one test can drive both ends with bot clients
- **+** Fiber actor runtime with location service, service discovery and server hot reload
- **+** Analyzers enforce async, entity lifecycle and package dependency rules on AI-written code
- **+** Unity bridge exposes 68 editor commands (scene, prefab, inspector, play mode, logs) to agents
- **−** ET License allows learning only; modification and commercial use need a 4999 license
- **−** Locked to Unity on the client and C# on the server
- **−** Documentation is mostly in Chinese; the README asks readers to machine-translate it
- **−** Several add-on packages (mongodb patching, webgl, yiui numeric) are paid, priced 100 to 999 yuan

<sub>no GPU · Needs Unity, NET SDK, MongoDB · [Repo](https://github.com/egametang/et) · [🌐 Site ↗](https://et-framework.cn) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/et/)</sub>

<a name="loopback-next"></a>
### #&#8288;240 [loopback-next](https://github.com/loopbackio/loopback-next) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · custom license · Nov 2026</sub>

**TypeScript framework for building REST APIs defined with OpenAPI.**

LoopBack 4 is a TypeScript framework for building API servers that integrate with other systems. A CLI (`npm create loopback` or `npx -p @loopback/cli lb app`) generates projects, and data and endpoints are defined with OpenAPI. It has no AI features, so it is a general backend framework rather than an AI starter.

- **+** Generates API projects from a single CLI command
- **+** Endpoints and data are defined with OpenAPI
- **+** Separate API reference, tutorials and examples on the docs site
- **+** Supports Node.js 22 and 24 LTS
- **−** No built-in AI, model or agent support
- **−** No LTS version of LoopBack 4 is offered yet
- **−** No Docker or compose files in the repository
- **−** Detected license is NOASSERTION, though the README says MIT

<sub>no GPU · Needs Node.js · [Repo](https://github.com/loopbackio/loopback-next) · [📖 Docs ↗](https://loopback.io/doc/en/lb4/) · [🌐 Site ↗](https://loopback.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loopback-next/)</sub>

<a name="nitric"></a>
### #&#8288;241 [nitric](https://github.com/nitrictech/nitric) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="feder-cr-git-ai"></a>
### #&#8288;242 [feder-cr/git-ai](https://github.com/feder-cr/git-ai) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · custom license · Nov 2026</sub>

**Git server for coding agents that lands concurrent changes by compare-and-swap.**

gitai is a fork of GitLab's Gitaly that implements the server-centric source control design Anthropic described for Scion. Agents fetch sparse trees over gRPC, and changes are rebased and landed with a compare-and-swap, batched per branch instead of queued. Conflicts can go to a resolver you choose (any LLM, a deterministic tool, or none), and the server itself never calls a model.

- **+** Batched landing: 200 of 250 changes landed vs 100-106 classic in the 50-agent benchmark
- **+** Vendor neutral: server makes no LLM calls; resolvers are pluggable or optional
- **+** Changeset log in SQLite or PostgreSQL, with packs in object storage and stateless nodes
- **+** Per-agent tokens, RPC allowlist and branch policies; policy reloads on SIGUSR1
- **−** Version 0.4.2; interfaces may change before 1.0
- **−** Multi-node tested only on one machine; S3, GCS and Azure buckets untested
- **−** Build needs Go 1.26, a C toolchain, Meson and Ninja; no Docker image mentioned
- **−** Benchmark was run on the 0.3.0 tree and not repeated for 0.4.0

<sub>no GPU · Needs Go 1.26, C toolchain, Meson, Ninja, SQLite or PostgreSQL, object storage (file, S3, GCS, Azure) · Models: any LLM provider for optional conflict resolution · [Repo](https://github.com/feder-cr/git-ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/feder-cr-git-ai/)</sub>

<a name="enroute"></a>
### #&#8288;243 [enroute](https://github.com/enroute-sh/enroute) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 444 · Apache-2.0 · Nov 2026</sub>

**Programmable Git server in Rust that stores repositories in object storage.**

Enroute is a Git server written in Rust that terminates smart HTTP Git connections and exposes a gRPC API. Repositories are stored as immutable layers in S3, GCS or Azure Blob, with a replicated log per repository on three ledger nodes. Opt-in hooks for authentication, visibility, pre-receive and post-receive let your application decide access and which pushes land.

- **+** One binary with no external database; a local directory works as the object store
- **+** Claims over 7,500 pushes per second to a single repository, acknowledged after majority ledger disk write
- **+** Same binary scales from one node to separate compute and three or more ledger nodes
- **+** Hooks and gRPC API let you build custom code hosting without forking the server
- **−** Early status: any 0.x release can change storage format, configuration and API
- **−** Storage format changes require moving repositories to a new deployment
- **−** Only smart HTTP today; SSH and git:// transports are on the roadmap
- **−** Pull requests are disabled; patches go by email under a CLA assigning rights

<sub>no GPU · Needs Object storage (S3, Google Cloud Storage, Azure Blob, or local directory), Persistent disk per ledger node · port 8080 · [Repo](https://github.com/enroute-sh/enroute) · [🌐 Site ↗](https://enroute.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/enroute/)</sub>

<a name="badger"></a>
### #&#8288;244 [badger](https://github.com/dgraph-io/badger) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · Apache-2.0 · Oct 2026</sub>

**Embeddable key-value database for Go with ACID transactions.**

BadgerDB is an embeddable, persistent key-value store written in pure Go, with no Cgo. It is an LSM tree that keeps values in a separate log, following the WiscKey paper, and is tuned for SSDs. It provides concurrent ACID transactions with serializable snapshot isolation, TTLs, snapshots and per-key versioning. It is the storage layer for Dgraph.

- **+** Pure Go with no Cgo, so it builds without a C toolchain
- **+** Concurrent ACID transactions with serializable snapshot isolation, tested by a nightly 8h bank test
- **+** Supports TTLs, snapshots and multiple versions per key via the Iterator API
- **+** Used in production by Dgraph, Jaeger and lakeFS, with data sets in the hundreds of TB
- **−** Embedded library only: no server, network API or built-in replication
- **−** Go-only API, so non-Go applications cannot use it directly
- **−** Directory locking and fsync are weaker on AIX, Windows, Plan9 and WASM
- **−** Pinned to Go 1.23, which limits use of newer language features

<sub>no GPU · Needs Go 1.23 or above · [Repo](https://github.com/dgraph-io/badger) · [📖 Docs ↗](https://badger.dgraph.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/badger/)</sub>

<a name="platform"></a>
### #&#8288;245 [platform](https://github.com/orchidsoftware/platform) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (46) · Freshness: active (94) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Nov 2026</sub>

**Laravel package for building admin panels and back-office apps in PHP.**

Orchid is a Laravel package for building admin panels, back-office apps and dashboards from PHP code, without writing HTML, CSS or JavaScript. It ships a form builder, role-based access permissions, Eloquent-based filtering and sorting, and Laravel Scout full-text search. Page transitions use Hotwire to avoid full reloads. It has no AI features.

- **+** Admin UI is defined in PHP; no frontend code needed
- **+** Built-in roles, permissions, form fields, notifications and table filtering/sorting
- **+** Hotwire gives SPA-like navigation without extra code
- **+** MIT licensed, free for commercial use
- **−** Tied to Laravel and PHP; unusable outside that stack
- **−** No AI or model features; fits this list only loosely
- **−** Last tagged release is March 2026, behind recent commits
- **−** Going beyond built-in components means learning Orchid's own abstractions

<sub>no GPU · Needs Laravel, PHP · [Repo](https://github.com/orchidsoftware/platform) · [📖 Docs ↗](https://orchid.software/en/docs) · [🌐 Site ↗](https://orchid.software/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/platform/)</sub>

<a name="absinthe"></a>
### #&#8288;246 [absinthe](https://github.com/absinthe-graphql/absinthe) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · custom license · Oct 2026</sub>

**GraphQL server library for Elixir with Phoenix, Plug and Relay support.**

Absinthe implements the GraphQL spec for Elixir. Schemas are defined with macros that are checked at compile time, and the query pipeline (parser, validations, resolution) can be swapped or extended. It is a Hex dependency, not an AI project, and has no model or LLM features.

- **+** Schema macros are verified at compile time, catching structure errors before runtime
- **+** Batched and async field resolution addresses N+1 query problems
- **+** Complexity analysis with configurable limits, plus precompiled documents to block custom queries
- **+** Pipeline is configurable per document: parser, validations and resolution can be replaced
- **−** Elixir only; requires Elixir 1.10 or higher
- **−** Library, not a standalone server: auth, storage and database must be built separately
- **−** No AI, LLM or MCP functionality, so it is outside this list's usual scope
- **−** README shows version ~> 1.7.0 and the license is not detected automatically

<sub>no GPU · Needs Elixir 1.10+, Hex · [Repo](https://github.com/absinthe-graphql/absinthe) · [📖 Docs ↗](https://hexdocs.pm/absinthe) · [🌐 Site ↗](https://absinthe-graphql.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/absinthe/)</sub>

<a name="apl-core"></a>
### #&#8288;247 [apl-core](https://github.com/linode/apl-core) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · Apache-2.0 · Nov 2026</sub>

**Kubernetes platform bundling Istio, Argo CD, Keycloak, Harbor and Tekton.**

App Platform (APL) installs a pre-integrated set of Kubernetes apps onto an LKE or other conformant cluster. Teams get self-service image builds, GitOps deployments, a private registry, and logs, metrics and traces. Administrators get multi-tenant team onboarding, user management, policy enforcement and configuration-as-code. It is a general Kubernetes platform with no AI features.

- **+** Pre-wired stack: Istio, Argo CD, Keycloak, Gitea, Tekton, cert-manager, ExternalDNS, Sealed Secrets
- **+** Runs on LKE or any conformant Kubernetes cluster
- **+** Optional one-click apps: Harbor, Kyverno, Trivy Operator, Prometheus, Grafana, Loki, Knative
- **+** Multi-tenant team onboarding with built-in security policies and zero-trust networking
- **−** Requires an existing Kubernetes cluster; no single-host install path
- **−** Not an AI project; no model serving, agents or LLM tooling
- **−** Many bundled components to operate and upgrade
- **−** Install guides center on Akamai Cloud (LKE)

<sub>no GPU · Docker + Compose · Needs Kubernetes cluster · [Repo](https://github.com/linode/apl-core) · [📖 Docs ↗](https://techdocs.akamai.com/app-platform/docs/getting-started) · [🌐 Site ↗](https://techdocs.akamai.com/app-platform/docs/welcome) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apl-core/)</sub>

<a name="fusio"></a>
### #&#8288;248 [fusio](https://github.com/apioo/fusio) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

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

<a name="sqlite-data"></a>
### #&#8288;249 [sqlite-data](https://github.com/pointfreeco/sqlite-data) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

**Swift SQLite persistence library replacing SwiftData, with CloudKit sync.**

SQLiteData is a Swift package built on GRDB and StructuredQueries that gives Apple-platform apps a SwiftData-like API (@Table, @FetchAll, @FetchOne) over a local SQLite database. A SyncEngine can replicate selected tables to CloudKit, including record sharing between iCloud users. It works from SwiftUI, UIKit and @Observable models. It is not an AI project and has no AI features.

- **+** CloudKit sync and sharing via a SyncEngine configured per table
- **+** Decoding benchmarks near raw SQLite C calls, ahead of GRDB Codable in the README
- **+** Type-safe query builder plus #sql macro; works in SwiftUI, UIKit and @Observable
- **+** Includes example apps: Reminders, SyncUps, CloudKitDemo and case studies
- **−** Swift and Apple platforms only; CloudKit sync ties data to iCloud
- **−** Expects working SQLite knowledge: schema design, joins, migrations and indices
- **−** Not an AI project; fits this list only as an app persistence layer
- **−** You create and migrate the database yourself; no automatic schema as in SwiftData

<sub>no GPU · Needs GRDB, StructuredQueries, CloudKit (optional sync) · [Repo](https://github.com/pointfreeco/sqlite-data) · [📖 Docs ↗](https://swiftpackageindex.com/pointfreeco/sqlite-data/main/documentation/sqlitedata) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sqlite-data/)</sub>

<a name="piccolo"></a>
### #&#8288;250 [piccolo](https://github.com/piccolo-orm/piccolo) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Async and sync Python ORM and query builder with migrations and admin.**

Piccolo is a Python ORM and query builder that supports both asyncio and sync use, with PostgreSQL and SQLite drivers. It includes a User model, authentication, migrations and a playground, and `piccolo asgi new` scaffolds an ASGI app on one of nine frameworks. Separate packages add an admin GUI and REST endpoints with auth middleware. It has no AI features.

- **+** Same table definitions work as a query builder or as an object-style ORM
- **+** Scaffolds ASGI apps for Starlette, FastAPI, Litestar, Sanic, Quart, Falcon and others
- **+** Ships migrations, a User model and auth; admin GUI and REST API are separate packages
- **+** Fully type annotated, with tab completion in iPython and VSCode
- **−** Only PostgreSQL and SQLite drivers are listed; no MySQL support mentioned
- **−** Admin GUI and REST/middleware utilities live in separate packages to install and learn
- **−** Not an AI project; no model, agent or LLM integration
- **−** No hosting or deployment layer; it is a library, not a backend service

<sub>no GPU · Needs PostgreSQL or SQLite · [Repo](https://github.com/piccolo-orm/piccolo) · [📖 Docs ↗](https://piccolo-orm.readthedocs.io/en/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/piccolo/)</sub>

<a name="data-api-builder"></a>
### #&#8288;251 [data-api-builder](https://github.com/azure/data-api-builder) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Nov 2026</sub>

**Generates REST, GraphQL and MCP endpoints from SQL and Cosmos DB schemas.**

Data API builder (DAB) reads a JSON config and exposes tables, views and stored procedures as REST, GraphQL and MCP endpoints, translating requests to SQL at runtime. It supports Azure SQL, SQL Server, SQLDW, Cosmos DB, PostgreSQL and MySQL, and installs as a .NET global tool (`dab`) that needs .NET 8 or later. In production it runs as a container.

- **+** No-code: endpoints come from dab-config.json, with CLI commands `dab init` and `dab add`
- **+** Covers Azure SQL, SQL Server, SQLDW, Cosmos DB, PostgreSQL and MySQL
- **+** Serves REST, GraphQL and MCP from one config, with per-role entity permissions
- **+** Development mode enables Swagger and Nitro UIs plus a /health endpoint
- **−** Exposes existing database objects only; no auth, storage or hosting beyond the data API
- **−** CLI needs .NET 8 or later installed
- **−** Default config uses the AppService auth provider, so other providers need extra setup
- **−** Branded for Azure databases, so some docs and samples assume Azure

<sub>no GPU · Docker · Needs NET 8 runtime or later, One of: Azure SQL, SQL Server, SQLDW, Cosmos DB, PostgreSQL, MySQL · port 5000 · [Repo](https://github.com/azure/data-api-builder) · [📖 Docs ↗](https://learn.microsoft.com/azure/data-api-builder/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/data-api-builder/)</sub>

<a name="busabase"></a>
### #&#8288;252 [busabase](https://github.com/busabase/busabase) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 930 · MIT · Nov 2026</sub>

**Shared database and workspace where multiple AI agents read and write reviewed records.**

Busabase is a workspace of typed records, docs, files, skills, whiteboards, workflows and small apps that Claude Code, Codex, Cursor or custom agents access through MCP, OpenAPI, a CLI, or SDKs. Agent writes arrive as Change Requests with a field-level diff and history, and permissions decide whether they merge immediately or wait for review. It runs locally with embedded PGlite via `npx busabase server`, or on external Postgres.

- **+** Every agent write is a Change Request with diff, author and history
- **+** Starts with one npx command on embedded PGlite; no account or config
- **+** Agent access via Skill, MCP, OpenAPI, CLI, plus TypeScript and Python SDKs
- **+** Can switch to external Postgres and S3-compatible storage by env vars
- **−** Open-source server is single-workspace; roles and multi-user need the paid Cloud
- **−** Only one process can hold the same PGlite database at a time
- **−** Not meant for public exposure; needs a reverse proxy and auth for remote use
- **−** No built-in model, so you must bring and configure your own agent

<sub>no GPU · Needs Postgres (optional), S3-compatible storage (optional) · port 15419 · [Repo](https://github.com/busabase/busabase) · [📖 Docs ↗](https://busabase.com/docs) · [🌐 Site ↗](https://busabase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/busabase/)</sub>

<a name="ent"></a>
### #&#8288;253 [ent](https://github.com/ent/ent) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (78) · Freshness: active (95) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · Apache-2.0 · Oct 2026</sub>

**Entity framework for Go that generates typed database code from schemas.**

ent models a database schema as Go code and generates a statically typed API for queries, aggregations and graph traversal. It supports MySQL, MariaDB, TiDB, PostgreSQL, CockroachDB, SQLite and Gremlin, and can be customized through Go templates. It is a general-purpose Go data-layer library with no AI features in the README.

- **+** Schema defined as Go code, with a generated, statically typed query API
- **+** Supports seven storage drivers, including PostgreSQL, MySQL, SQLite and CockroachDB
- **+** Graph-style traversal and aggregation across related entities
- **+** Code generation can be extended with custom Go templates
- **−** Not an AI project; it is a data-access library, so it fits this list loosely
- **−** Go only, and requires a code generation step after schema changes
- **−** v1 has not shipped; the README links to a v1 roadmap issue
- **−** Library, not a hosted backend: no auth, storage or API server included

<sub>no GPU · Needs MySQL, MariaDB, TiDB, PostgreSQL, CockroachDB, SQLite, Gremlin · [Repo](https://github.com/ent/ent) · [📖 Docs ↗](https://entgo.io) · [🌐 Site ↗](https://entgo.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ent/)</sub>

<a name="ignite"></a>
### #&#8288;254 [apache/ignite](https://github.com/apache/ignite) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · Apache-2.0 · Nov 2026</sub>

**Distributed in-memory database with SQL, ACID transactions and compute APIs.**

Apache Ignite is a distributed database written in Java that keeps data in memory with optional disk persistence. It provides ACID transactions across servers, an ANSI-99 SQL engine reachable over JDBC, ODBC and native APIs, and MapReduce-style compute tasks across nodes. The README describes no AI-specific features.

- **+** ACID transactions that span multiple servers, in memory and on disk
- **+** Optional native persistence for datasets larger than RAM and faster restarts
- **+** SQL via JDBC, ODBC and native APIs for Java, C#, C++ and Python
- **+** Compute APIs run arbitrary MapReduce-style tasks across cluster nodes
- **−** No AI or LLM features; a general-purpose database, not a starter
- **−** DDL support is only a subset of commands relevant to distributed systems
- **−** No Dockerfile or compose files detected in the repository
- **−** No tagged release listed for the repository

<sub>no GPU · [Repo](https://github.com/apache/ignite) · [📖 Docs ↗](https://ignite.apache.org/docs/latest/) · [🌐 Site ↗](https://ignite.apache.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ignite/)</sub>

<a name="mongoengine"></a>
### #&#8288;255 [mongoengine](https://github.com/mongoengine/mongoengine) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (42) · Freshness: active (94) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Sep 2026</sub>

**Python object-document mapper for MongoDB built on PyMongo.**

MongoEngine maps Python classes to MongoDB collections, with typed fields, validation, document inheritance and a queryset API such as BlogPost.objects(tags='x').count(). It sits on top of PyMongo and is tested against MongoDB 4.4 through 8.0. It is a general database library with no AI features, so it fits this list only as a backend component.

- **+** Declarative Document classes with field validation and inheritance, queried through a queryset API
- **+** Tested against MongoDB 4.4, 5.0, 6.0, 7.0 and 8.0
- **+** Only PyMongo >=4.0 required; Pillow, python-dateutil and blinker are optional
- **+** Docs include a tutorial, user guide and API reference on Read the Docs
- **−** Python and MongoDB only; no other databases supported
- **−** Requires Python 3.10 or newer
- **−** No AI or LLM features; unrelated to model serving or agents
- **−** Tests need a running MongoDB on the standard port

<sub>no GPU · Docker + Compose · Needs MongoDB, PyMongo >=4.0, Python >=3.10 · [Repo](https://github.com/mongoengine/mongoengine) · [📖 Docs ↗](https://mongoengine-odm.readthedocs.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mongoengine/)</sub>

<a name="zappa"></a>
### #&#8288;256 [zappa](https://github.com/zappa/zappa) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**CLI that deploys Python WSGI and ASGI apps to AWS Lambda and API Gateway.**

Zappa packages a Python web app with its virtualenv dependencies, uploads it to S3, and creates the Lambda function, IAM role and API Gateway routes. It works with Flask, Bottle, Django, and ASGI apps such as FastAPI, Starlette and Quart. The CLI also covers updates, rollback, scheduled events, log tailing, custom domains with SSL, and async tasks.

- **+** Deploys existing Flask, Django or FastAPI apps with zappa init and zappa deploy
- **+** Covers the deploy lifecycle: update, rollback, undeploy, tail logs, schedule, certify
- **+** Supports ZIP and ECR Docker image deploys, plus slim_handler for packages over 50MB
- **+** Includes async tasks, EventBridge schedules, keep-warm, and API Gateway auth options
- **−** AWS only: tied to Lambda, API Gateway, S3 and IAM
- **−** ASGI mode has no WebSocket, lifespan protocol or streaming responses
- **−** API Gateway caps requests at 30s; longer work needs an ALB
- **−** Default IAM policy is permissive and needs customizing for production

<sub>no GPU · Needs AWS account, AWS Lambda, API Gateway, S3, Python 3.9-3.14 · [Repo](https://github.com/zappa/zappa) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zappa/)</sub>

<a name="tile38"></a>
### #&#8288;257 [tile38](https://github.com/tidwall/tile38) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · MIT · Nov 2026</sub>

**In-memory geospatial database with spatial search and realtime geofencing.**

Tile38 is a Go server that stores lat/lon points, bounding boxes, Geohashes, and GeoJSON in memory, persists them to disk, and answers Nearby, Within, and Intersects queries. Any search can become a geofence with the FENCE keyword, delivering enter/exit/cross events over webhooks, pub/sub channels, or open connections. It speaks Redis RESP, HTTP, websockets, and telnet.

- **+** Any search becomes a geofence with FENCE; events via webhooks, pub/sub, or websockets
- **+** Speaks RESP, so most Redis client libraries work; HTTP with curl also supported
- **+** Ships server, CLI, and benchmark tool; native Prometheus metrics via --metrics-addr
- **+** Accepts points, bounds, Geohash, and GeoJSON; WHERE and MATCH filters on fields and ids
- **−** Dataset lives in memory, so capacity is bounded by available RAM
- **−** Fields are double-precision floats only; string values need GeoJSON properties
- **−** XYZ tile and QuadKey types can be used in searches but not stored
- **−** Replication is leader/follower only; no clustering described

<sub>no GPU · Docker · port 9851 · [Repo](https://github.com/tidwall/tile38) · [📖 Docs ↗](https://tile38.com/commands) · [🌐 Site ↗](https://tile38.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tile38/)</sub>

<a name="spring-boot-starter"></a>
### #&#8288;258 [spring-boot-starter](https://github.com/mybatis/spring-boot-starter) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (41) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · Apache-2.0 · Nov 2026</sub>

**Spring Boot auto-configuration and starters for the MyBatis SQL mapper.**

Java library that auto-configures MyBatis inside Spring Boot applications, with a starter dependency available through Spring Initializr. It also ships a test auto-configure module for MyBatis tests. Master targets MyBatis 3.5, MyBatis-Spring 4.1, Java 17+ and Spring Boot 4.1, with older branches for Boot 2.7 to 4.0.

- **+** Release branches cover Spring Boot 2.7, 3.2-3.5, 4.0 and 4.1
- **+** Separate test auto-configure module for MyBatis tests
- **+** Selectable in Spring Initializr and published on Maven Central
- **+** Has a quick-start wiki page for native image builds
- **−** Java and Spring Boot only; not usable from other stacks
- **−** Master requires Java 17+ and Spring Boot 4.1
- **−** Spring Boot 2.7 needs the older 2.3.x line
- **−** Not an AI project; fits this list only loosely

<sub>no GPU · Needs Java 17+, Spring Boot, MyBatis 3.5, MyBatis-Spring · [Repo](https://github.com/mybatis/spring-boot-starter) · [📖 Docs ↗](http://www.mybatis.org/spring-boot-starter/mybatis-spring-boot-autoconfigure) · [🌐 Site ↗](https://mybatis.org/spring-boot-starter/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spring-boot-starter/)</sub>

<a name="beanie"></a>
### #&#8288;259 [beanie](https://github.com/beanieodm/beanie) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · Apache-2.0 · Oct 2026</sub>

**Async Python ODM for MongoDB with Pydantic models.**

Beanie maps MongoDB collections to Pydantic-based Document classes and exposes async insert, find, update and delete using Python expression syntax. It uses the PyMongo async client under the hood and includes data and schema migrations. A synchronous sibling, Bunnet, exists for non-async code.

- **+** Queries written as Python expressions, e.g. Product.price < 10
- **+** Pydantic models double as document schemas; Indexed fields declare indexes
- **+** Data and schema migrations are built in
- **+** Linked examples cover FastAPI, JWT auth and Azure Cosmos DB
- **−** MongoDB only; no support for other databases
- **−** Maintainers warn reviews and issue replies are slower while v3 is built
- **−** Async only; sync use needs the separate Bunnet library
- **−** Library, not a service: no hosting, auth or API layer included

<sub>no GPU · Needs MongoDB, Pydantic, PyMongo · [Repo](https://github.com/beanieodm/beanie) · [📖 Docs ↗](https://beanie-odm.dev) · [🌐 Site ↗](https://beanie-odm.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beanie/)</sub>

<a name="agensgraph"></a>
### #&#8288;260 [agensgraph](https://github.com/skaiworldwide-oss/agensgraph) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Models: pgvector embeddings, MCP clients, LangChain, LlamaIndex, LightRAG · [Repo](https://github.com/skaiworldwide-oss/agensgraph) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agensgraph/)</sub>

<a name="webman"></a>
### #&#8288;261 [webman](https://github.com/walkor/webman) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (30) · Freshness: active (92) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**PHP web framework built on the workerman event-driven server.**

webman is a PHP web framework built on workerman, a resident-memory PHP server, rather than the usual PHP-FPM request cycle. The README is mostly links to the docs, install guide, Q&A forum and app marketplace, plus sponsor and donation notes. It describes no AI features, so it fits this list only as a generic backend framework.

- **+** Built on workerman, so the PHP process stays resident between requests
- **+** MIT licensed, with separate docs site and an app marketplace
- **+** Active repository: last commit 2026-10-23, last release 2026-02-24
- **−** No AI, model or agent functionality described; not an AI project
- **−** README has no install steps, benchmarks or requirements inline
- **−** Much of the README and community content is in Chinese
- **−** Framework only: no bundled auth, database or storage service described

<sub>no GPU · Docker + Compose · Needs PHP, workerman · [Repo](https://github.com/walkor/webman) · [📖 Docs ↗](https://webman.workerman.net) · [🌐 Site ↗](https://www.workerman.net/webman) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/webman/)</sub>

<a name="robustmq"></a>
### #&#8288;262 [robustmq](https://github.com/robustmq/robustmq) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Nov 2026</sub>

**Rust message broker for MQTT, Kafka, NATS and AMQP on shared storage.**

RobustMQ is a single-binary message broker written in Rust, with built-in Raft metadata consensus and a storage layer shared across protocols. MQTT 3.x/5.0 is the mature part. Kafka, NATS, AMQP and the mq9 agent mailbox are still in development. mq9 adds an agent registry with semantic discovery and per-agent persistent mailboxes, reachable through NATS clients or SDKs.

- **+** Single binary with built-in Raft, no external dependencies
- **+** Per-topic storage: memory, RocksDB or file, with cold tiering to S3
- **+** MQTT 3.x/5.0, auth/ACL, shared subscription and Prometheus metrics listed as available
- **+** mq9 SDKs for Python, Go, TypeScript, Java, Rust, C#, plus a LangChain toolkit
- **−** README says not production-ready; production targeted for 0.4.0
- **−** Kafka, NATS, AMQP and mq9 are in development or only demo-validated
- **−** Web console ships only in packages built with the frontend
- **−** Cross-protocol consume examples rely on protocols not yet marked available

<sub>no GPU · Docker + Compose · port 58080 · [Repo](https://github.com/robustmq/robustmq) · [▶️ Demo ↗](http://demo.robustmq.com:58080) · [📖 Docs ↗](https://robustmq.com/QuickGuide/Overview.html) · [🌐 Site ↗](https://robustmq.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/robustmq/)</sub>

<a name="wcdb"></a>
### #&#8288;263 [wcdb](https://github.com/tencent/wcdb) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (69) · Freshness: active (95) · Maintenance: weak (12) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · custom license · Oct 2026</sub>

**SQLite and SQLCipher-based embedded database with ORM for mobile and desktop apps.**

WCDB is the database framework used in WeChat. It wraps SQLite and SQLCipher with an ORM and a native query layer (WINQ) for C++, Java, Kotlin, Swift and Objective-C, all sharing one core. It adds encryption, corruption recovery, full-text search, data migration and Zstd field compression. It is not an AI project; it fits this list only loosely, as an embedded storage layer.

- **+** Same core across C++, Java, Kotlin, Swift and Objective-C, so mixed-language apps share one database
- **+** Built-in SQLCipher encryption, corruption repair kit and SQL injection protection
- **+** Concurrent read-read and read-write access through connection pooling
- **+** Per-field Zstd compression and database-to-database migration via configuration
- **−** Embedded client library only; no server, auth or hosted storage
- **−** Not AI-related; no vector search or model integration is described
- **−** License is reported as NOASSERTION, so terms need manual checking
- **−** Build and tutorial wiki links point to Chinese-language pages

<sub>no GPU · Needs SQLite, SQLCipher, Zstd · [Repo](https://github.com/tencent/wcdb) · [📖 Docs ↗](https://github.com/Tencent/wcdb/wiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wcdb/)</sub>

<a name="faasd"></a>
### #&#8288;264 [faasd](https://github.com/openfaas/faasd) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (35) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · custom license · Nov 2026</sub>

**Single-host serverless functions runtime on containerd, using OpenFaaS components.**

faasd runs OpenFaaS on one Linux host without Kubernetes. It is a single Go binary run as a systemd service, using containerd and CNI to run the OpenFaaS Gateway, Queue-Worker, event connectors and scale to zero. It also supports stateful containers with persistent volumes such as PostgreSQL, Grafana and Prometheus. It is a general function-hosting runtime, not an AI project.

- **+** Single Go binary run as a systemd service, no Kubernetes to maintain
- **+** Runs on 2 vCPU and 2GB RAM, x86_64 and Arm64
- **+** Reuses the OpenFaaS Gateway, Queue-Worker and scale-to-zero containers
- **+** Supports persistent volumes for stateful containers like PostgreSQL
- **−** faasd CE is restricted to non-commercial personal use under its EULA
- **−** Commercial use needs the paid OpenFaaS Edge license
- **−** Single host only, so no multi-node clustering
- **−** No AI or model features; a general serverless runtime

<sub>RAM ≥ 2 GB · no GPU · Compose · Needs containerd, CNI, systemd · [Repo](https://github.com/openfaas/faasd) · [📖 Docs ↗](https://docs.openfaas.com/deployment/edge/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/faasd/)</sub>

<a name="butterbase"></a>
### #&#8288;265 [butterbase](https://github.com/butterbase-ai/butterbase) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="lucky"></a>
### #&#8288;266 [lucky](https://github.com/luckyframework/lucky) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (31) · Freshness: active (97) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

**Type-safe Crystal web framework with compile-time checked routes and queries.**

Lucky is a full-stack web framework written in Crystal. It provides actions for routing, the Avram ORM for Postgres models and queries, and HTML pages written as Crystal classes. Missing route params, mistyped columns and nil output are caught at compile time. It has no AI features, so it fits this list only loosely as a general backend base.

- **+** Routes, column names and page params are checked at compile time
- **+** Covers JSON APIs, HTML rendering and a database ORM in one framework
- **+** MIT licensed, with guides and API docs published online
- **+** Lucky JumpStart repo offers a working app to copy
- **−** No AI, LLM or agent features; unrelated to vibe coding tooling
- **−** Requires Crystal, a smaller ecosystem than Rails or Node frameworks
- **−** README only shows Postgres; other databases are not described
- **−** Not a hosted backend; no auth or storage service is described

<sub>no GPU · Docker + Compose · Needs Crystal, PostgreSQL · [Repo](https://github.com/luckyframework/lucky) · [📖 Docs ↗](https://luckyframework.org/guides) · [🌐 Site ↗](https://luckyframework.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lucky/)</sub>

<a name="madong-admin"></a>
### #&#8288;267 [madong-admin](https://github.com/madong-code/madong-admin) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.0k · Apache-2.0 · Nov 2026</sub>

**PHP Webman admin backend with plugins, code generator and two admin UIs.**

Madong is a PHP 8.2–8.4 backend for admin panels, built on Webman 2.2 with MySQL and Redis. It provides JWT auth, permission management, file upload, i18n, a plugin system and a code generator for controllers, models and services. Frontends live in separate repos (two admin UIs, Single or Aura, plus a Nuxt site) and are fetched with a CLI command.

- **+** Code generator produces controllers, models and service-layer code
- **+** Plugin system merges dependencies, ref-counts them and rolls back failed installs
- **+** CLI install wizard writes database and Redis config automatically
- **+** Two selectable admin UIs (Single, Aura) and a public live demo
- **−** Frontends are separate repos that must be downloaded or cloned separately
- **−** No Docker or compose files; PHP, MySQL, Redis, Composer and Node installed by hand
- **−** README is in Chinese; the English version is a separate file
- **−** No release published; versioning relies on branches

<sub>no GPU · Needs PHP 8.2-8.4, MySQL 8.0+, Redis 7.0+, Composer 2.x, Node.js with pnpm, Nginx or Apache · port 8500 · [Repo](https://github.com/madong-code/madong-admin) · [▶️ Demo ↗](http://v5.madong.tech/admin) · [📖 Docs ↗](https://madong.tech) · [🌐 Site ↗](https://madong.tech) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/madong-admin/)</sub>

<a name="mica"></a>
### #&#8288;268 [mica](https://github.com/lets-mica/mica) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (26) · Freshness: active (91) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · LGPL-3.0 · Nov 2026</sub>

**Spring Boot and Spring Cloud base components and utilities for Java microservices.**

Mica is a Java library set (Maven BOM net.dreamlu:mica-bom) of base components and utility toolkits for Spring Boot and Spring Cloud microservices, supporting both Spring Web and WebFlux. Release lines track Spring Boot versions: 4.0.x, 3.5.x and 3.4.x are maintained. It contains no AI or model features, so it fits this list only loosely as a backend building block.

- **+** Version numbers follow Spring Boot, with maintained lines for 4.0, 3.5 and 3.4
- **+** Supports both Spring Web and WebFlux
- **+** Published to Maven Central, with auto-published SNAPSHOT builds after each push
- **+** Related modules exist for MQTT, WeChat and Spring Boot starter generation
- **−** No AI, LLM or agent functionality; it is a general Java service library
- **−** Primary docs and README are in Chinese; the English README is a separate file
- **−** LGPL-3.0 plus a stated 19999 fee for closed-source modification without consent
- **−** Known Lombok issue breaks Map/Bean conversion for properties like xX; no fix planned

<sub>no GPU · Needs JDK 17+, Spring Boot, Maven · [Repo](https://github.com/lets-mica/mica) · [🌐 Site ↗](http://wiki.dreamlu.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mica/)</sub>

<a name="ruoyi-cloud"></a>
### #&#8288;269 [ruoyi-cloud](https://github.com/yangzongzhuan/ruoyi-cloud) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (20) · Freshness: active (95) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Nov 2026</sub>

**Spring Cloud and Vue admin platform with code generation.**

RuoYi-Cloud is the microservice edition of the RuoYi admin framework. The backend uses Spring Boot 4.x and Spring Cloud & Alibaba, with a Vue front end. It includes gateway, auth, system, code-generation, job, file and monitor modules, using Nacos for registry and config, Redis for auth, Sentinel for flow control and Seata for distributed transactions. It is a general admin scaffold with no AI features.

- **+** Built-in user, role, menu, department, dictionary and log management modules
- **+** Code generator produces Java, XML, SQL and front-end CRUD code
- **+** Maintained branches for Spring Boot 2.x, 3.x and 4.x
- **+** Three front-end variants: Vue 2, Vue 3 and Vue 3 TypeScript
- **−** Needs Nacos, Redis and a database running beside several services
- **−** No AI or model features, so it is not an LLM starter
- **−** README and community links are mostly in Chinese
- **−** No Docker or Compose files in the repository

<sub>no GPU · Docker + Compose · Needs Nacos, Redis, Sentinel, Seata · port 80 · [Repo](https://github.com/yangzongzhuan/ruoyi-cloud) · [▶️ Demo ↗](http://ruoyi.vip) · [📖 Docs ↗](http://doc.ruoyi.vip) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruoyi-cloud/)</sub>

<a name="libsql"></a>
### #&#8288;270 [libsql](https://github.com/tursodatabase/libsql) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (78) · Freshness: recent (70) · Maintenance: weak (21) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Nov 2026</sub>

**SQLite fork with embedded replicas, a remote server and multi-language drivers.**

libSQL is an open-contribution fork of SQLite maintained by Turso. It keeps the SQLite file format and C API, and adds embedded replicas, a server for remote access, an extended ALTER TABLE, randomized ROWID, WebAssembly user-defined functions and a virtual WAL interface. Official drivers cover TypeScript/JS, Rust and Go; the README says new features are now developed in Turso, a Rust rewrite.

- **+** Keeps the SQLite file format and full SQLite C API compatibility
- **+** Embedded replicas plus libsql-server for remote access
- **+** Official drivers for TypeScript/JS, Rust and Go
- **+** MIT licensed and open to outside contributions
- **−** Inherits SQLite's single-writer model; no concurrent writes
- **−** README points new projects to Turso, where new features are built
- **−** Python and C drivers are marked experimental
- **−** Last tagged release is 2025-02-14

<sub>no GPU · Docker + Compose · [Repo](https://github.com/tursodatabase/libsql) · [📖 Docs ↗](https://docs.turso.tech) · [🌐 Site ↗](https://turso.tech/libsql) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/libsql/)</sub>

<a name="madong-admin-saas"></a>
### #&#8288;271 [madong-admin-saas](https://github.com/madong-code/madong-admin-saas) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · Apache-2.0 · Nov 2026</sub>

**Multi-tenant PHP admin backend on Webman with tenant isolation and plugins.**

Madong-Saas is the server side of a multi-tenant admin system built on the Webman resident-memory PHP framework. It exposes APIs for a separate frontend, with DAO/Service/Controller layers, a plugin system, and per-tenant isolation and resource configuration. A browser install wizard on port 8500 collects MySQL, Redis and admin settings, then writes .env and initializes tables.

- **+** Built-in multi-tenancy with tenant isolation and per-tenant resource configuration
- **+** Web install wizard generates .env and initializes database tables
- **+** Layered DAO/Service/Controller structure plus a plugin system
- **+** Swagger API docs package included as a Composer dependency
- **−** Backend only; frontend lives in separate repos and needs interface adjustments
- **−** Requires external MySQL and Redis; no Docker files in this repo
- **−** README and docs are primarily in Chinese
- **−** No tagged release; 4.x line is kept under a separate tag

<sub>no GPU · Needs PHP 8.2-8.4, Composer 2.x, MySQL 5.7/8.0, Redis 5.0+ · port 8500 · [Repo](https://github.com/madong-code/madong-admin-saas) · [📖 Docs ↗](https://madong.tech) · [🌐 Site ↗](https://madong.tech) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/madong-admin-saas/)</sub>

<a name="neon"></a>
### #&#8288;272 [neon](https://github.com/neondatabase/neon) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: widely used (84) · Freshness: recent (75) · Maintenance: weak (9) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · Apache-2.0 · Aug 2026</sub>

**Serverless Postgres with separated storage and compute, plus branching.**

Neon replaces the PostgreSQL storage layer with a distributed storage engine made of a pageserver and safekeepers, a redundant WAL service. Compute nodes are stateless Postgres instances on top of it, and timelines can be branched so a branch sees the parent's data while its writes stay isolated. Written in Rust, it can be built and run locally with `cargo neon`; the README points to the hosted free tier as the quick start.

- **+** Branches a timeline; the branch sees parent data and its writes stay isolated
- **+** Stateless Postgres compute on a pageserver plus redundant safekeeper storage
- **+** Local environment via `cargo neon` starts pageserver, safekeeper, broker and endpoints
- **+** Integration tests run across supported Postgres versions, including 17
- **−** Self-hosting means building from source with a patched Postgres; no package or compose file
- **−** README covers local development only, with no production deployment guide
- **−** Build needs Rust, protoc 3.15+ and many system packages
- **−** Last tagged release is 2025-07-29, well behind recent commits

<sub>no GPU · Docker + Compose · Needs Rust toolchain, protoc 3.15+, PostgreSQL client, Python 3.11+ and poetry (tests only) · [Repo](https://github.com/neondatabase/neon) · [📖 Docs ↗](https://neon.com/docs) · [🌐 Site ↗](https://neon.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/neon/)</sub>

<a name="boilerplates"></a>
### #&#8288;273 [boilerplates](https://github.com/christianlempa/boilerplates) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · MIT · Aug 2026</sub>

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

<a name="lamp-cloud"></a>
### #&#8288;274 [lamp-cloud](https://github.com/dromara/lamp-cloud) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · Apache-2.0 · Oct 2026</sub>

**Java multi-tenant Spring Cloud admin platform with RBAC and code generator.**

lamp-cloud is a Java 17 back-end framework for admin systems, built on Spring Cloud Alibaba and Spring Boot. It targets multi-tenant SaaS with nested tenants, database-per-tenant, column isolation or no tenancy, and includes RBAC, gateway authentication, data permissions and a code generator. The README describes no AI features; it is a general business back-end scaffold.

- **+** Supports nested tenants, per-tenant database, column isolation and non-tenant modes
- **+** Ships RBAC, gateway auth, data permissions and a visual code generator
- **+** Live demos for each tenant mode, with vben5 and vben2 front ends
- **+** Integrates Seata, Sentinel, RabbitMQ, MinIO/FastDFS and SkyWalking
- **−** No AI or model features, so fit with an AI-focused list is weak
- **−** README and docs are mainly in Chinese
- **−** Front end is a separate repo, and lamp-util must be built first
- **−** Some features are only in the paid sponsor edition

<sub>no GPU · Needs Nacos, Seata, Sentinel, RabbitMQ, MinIO or FastDFS, SkyWalking, lamp-util · [Repo](https://github.com/dromara/lamp-cloud) · [▶️ Demo ↗](https://max-datasource.tangyh.top) · [📖 Docs ↗](https://tangyh.top/doc/%E7%AE%80%E4%BB%8B.html) · [🌐 Site ↗](https://tangyh.top) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lamp-cloud/)</sub>

<a name="olric"></a>
### #&#8288;275 [olric](https://github.com/olric-data/olric) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · Apache-2.0 · Nov 2026</sub>

**Distributed in-memory key/value cache in Go, embeddable or standalone.**

Olric is a distributed in-memory key/value store and cache written in Go. It shards and replicates data across a cluster, speaks the Redis protocol (RESP) so redis-cli and existing Redis clients work, and also provides Redis-compatible publish/subscribe. It runs either embedded in a Go application or as the standalone olric-server. It is not an AI project and has no model or LLM features.

- **+** Redis protocol, so redis-cli and standard Redis clients connect without a custom SDK
- **+** Automatic partitioning, rebalancing and replication with no external coordination service
- **+** Runs embedded in a Go app or as a standalone olric-server
- **+** Eviction by LRU, TTL and max idle duration; atomic ops and lock primitive
- **−** In-memory only; no persistence, so data is lost when the cluster goes down
- **−** Eventually consistent (PA/EC); not suitable for data needing strict consistency
- **−** Authentication is a single password with no TLS; needs a proxy or VPN
- **−** Embedded client is not covered by authentication; locks are for non-critical use

<sub>no GPU · Docker + Compose · [Repo](https://github.com/olric-data/olric) · [📖 Docs ↗](https://pkg.go.dev/github.com/olric-data/olric/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/olric/)</sub>

<a name="nixopus"></a>
### #&#8288;276 [nixopus](https://github.com/nixopus/nixopus) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Sep 2026</sub>

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

<a name="pouchdb"></a>
### #&#8288;277 [pouchdb](https://github.com/apache/pouchdb) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: popular (79) · Freshness: recent (70) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Nov 2026</sub>

**JavaScript document database for browsers and Node.js that syncs with CouchDB.**

PouchDB is a JavaScript database inspired by Apache CouchDB, built to run inside the browser so web apps keep working offline. Data is stored locally and can be synced with CouchDB-style servers when a connection is available. It fits none of the AI-focused categories closely; the nearest match is the backends and databases category.

- **+** Runs in the browser, so apps can work offline and online
- **+** Modeled on CouchDB, with replication to CouchDB-style servers
- **+** Databases auto-migrate across versions, from 1.0.0 to 4.0.0+
- **+** Follows semantic versioning, with a changelog and breaking-changes wiki
- **−** No AI, LLM or vector search features described in the README
- **−** Embedded client library, not a server for auth, storage or APIs
- **−** Still listed as incubating at the Apache Software Foundation
- **−** Last release was 2024-06-21, over a year before the last commit

<sub>no GPU · [Repo](https://github.com/apache/pouchdb) · [📖 Docs ↗](https://pouchdb.com/api.html) · [🌐 Site ↗](https://pouchdb.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pouchdb/)</sub>

<a name="go-spring"></a>
### #&#8288;278 [go-spring](https://github.com/go-spring/go-spring) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · Apache-2.0 · Nov 2026</sub>

**Spring Boot-style dependency injection and starter framework for Go services.**

Go-Spring is a Go application framework with an IoC container, constructor-based dependency injection, layered configuration with hot reload, and a unified lifecycle built around Runners and Servers. It ships 90+ separate Go-module starters wrapping Gin, gRPC, Kitex, Dubbo-go, Redis, MySQL, Kafka and others, plus a CLI (`gs`), an HTTP IDL code generator and a mock library. The project is marked unreleased, and breaking API changes are allowed.

- **+** 90+ starters, each an independent Go module, so you pull in only what you need
- **+** One layered config engine (CLI, env, files, Nacos/etcd/Consul/Vault/K8s) with gs.Dync[T] hot reload
- **+** Wraps existing frameworks and plain net/http instead of imposing its own transport or layout
- **+** Observability spec across 54 components is checked by scripts/check-observability.sh in CI
- **−** Marked unreleased; README allows large breaking changes before a stable API
- **−** Large surface (core, cloud, 90+ starters) means a steep learning curve for small services
- **−** Needs the gs CLI and its conventions to get the intended project layout
- **−** Claude Code skill is the only AI-agent integration; no other assistant tooling is described

<sub>no GPU · [Repo](https://github.com/go-spring/go-spring) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-spring/)</sub>

<a name="sanic"></a>
### #&#8288;279 [sanic](https://github.com/sanic-org/sanic) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: widely used (81) · Freshness: recent (78) · Maintenance: weak (2) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · May 2026</sub>

**Async Python web server and framework with a built-in CLI runner.**

Sanic is a Python 3.10+ web server and framework built on async/await. It ships its own HTTP server, started with `sanic hello.app`, listening on 127.0.0.1:8000 by default, and is also ASGI compliant so it can run under another ASGI server. It has no AI features; it fits the list only as a generic backend for exposing models or agents over HTTP.

- **+** Built-in server and CLI; `pip install sanic` is enough to run an app
- **+** ASGI compliant, so it can run under alternative ASGI servers
- **+** Uses uvloop and ujson for speed, each can be disabled via env variable at install
- **+** MIT licensed, with recent commits and releases
- **−** No AI, LLM or model-serving integration; you write all of that yourself
- **−** Not a starter template: no auth, database or project scaffold included
- **−** Requires Python 3.10 or newer
- **−** Smaller ecosystem than FastAPI or Flask for AI backends

<sub>no GPU · Docker · Needs uvloop, ujson · port 8000 · [Repo](https://github.com/sanic-org/sanic) · [📖 Docs ↗](https://sanic.dev) · [🌐 Site ↗](https://sanic.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sanic/)</sub>

<a name="doracms"></a>
### #&#8288;280 [doracms](https://github.com/doramart/doracms) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: known (37) · Freshness: recent (70) · Maintenance: patchy (30) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Nov 2026</sub>

**Content management system on EggJS 3 and Vue 3 with a separate admin panel.**

EggCMS (DoraCMS) is a pnpm monorepo with an EggJS 3 server, a Vue 3 user front end and a Vue 3 + TypeScript admin panel built on SoybeanAdmin. The server runs on MongoDB via Mongoose or MariaDB via Sequelize, with optional Redis and OSS or Qiniu uploads. The README shows an AI content publishing screen but does not document how it works.

- **+** Supports both MongoDB and MariaDB, with a migration guide between them
- **+** Docker Compose profiles for MariaDB, Redis and Nginx
- **+** Public demo site with separate front end and admin panel
- **+** Server-side locale detection and shared i18n keys for API responses
- **−** Last tagged release is 2020-08-01, though commits continue
- **−** AI content publishing appears only as a screenshot, with no setup docs
- **−** Several npm packages (sdk, types, utils) are still marked as planned
- **−** README and most linked docs are in Chinese

<sub>no GPU · Docker + Compose · Needs MongoDB or MariaDB, Redis (optional), Nginx (optional), Aliyun OSS or Qiniu (optional) · port 8080 · [Repo](https://github.com/doramart/doracms) · [▶️ Demo ↗](https://demo.doracms.net) · [📖 Docs ↗](https://www.doracms.net/deployment/docker) · [🌐 Site ↗](https://www.doracms.net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/doracms/)</sub>

<a name="skytable"></a>
### #&#8288;281 [skytable](https://github.com/skytable/skytable) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (30) · Freshness: recent (70) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · AGPL-3.0 · Sep 2026</sub>

**In-memory NoSQL database with a column-oriented model and SQL-like BlueQL.**

Skytable is a primarily in-memory NoSQL database written in Rust. It uses multithreaded async I/O and a custom AOF-based storage engine with delayed-durability transactions. Data is organized into spaces and models and queried with BlueQL, a SQL-based language that requires parameterized queries. The README notes that version 0.9 (clustering, new data types) is developed privately, and this branch holds 0.8.

- **+** BlueQL enforces parameterized queries, which deters injection by design
- **+** Models support complex types such as lists, defined with SQL-like syntax
- **+** Ships as bundled binaries: skyd server and skysh REPL client
- **+** Official Rust client driver is Apache-2.0 licensed
- **−** AGPL-3.0 license can constrain use in proprietary network services
- **−** Clustering and HA are not in this branch; 0.9 development is private
- **−** Only an official Rust client driver is mentioned; other languages need community drivers
- **−** Last release is 2024-08-07, and the 0.9 code is not yet public

<sub>no GPU · Docker · [Repo](https://github.com/skytable/skytable) · [📖 Docs ↗](https://docs.skytable.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skytable/)</sub>

<a name="json-server"></a>
### #&#8288;282 [json-server](https://github.com/typicode/json-server) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: widely used (98) · Freshness: recent (55) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 76k · MIT · Mar 2026</sub>

**Fake REST API served from a single JSON or JSON5 file.**

json-server is an npm package that turns a db.json or db.json5 file into a REST API with no code. Array keys get full CRUD routes, object keys get GET/PUT/PATCH, and it supports filtering, sorting, pagination, embedding and serving static files. The README documents the current v1 beta, which has breaking changes from 0.17.4.

- **+** Starts with one command: npx json-server db.json, on port 3000 by default
- **+** Query operators include gt, lt, in, contains and startsWith, plus _sort, _embed and _where
- **+** Pagination returns first, prev, next, last, pages and items metadata
- **+** Serves ./public and extra static directories via the -s flag
- **−** v1 docs are labeled beta, with breaking changes expected
- **−** Data lives in a flat JSON file, so it is a mock rather than a production backend
- **−** v1 forces ids to strings and replaces _expand and _limit, which breaks 0.x clients
- **−** The --delay option was removed in v1

<sub>no GPU · Needs Node.js, npm · port 3000 · [Repo](https://github.com/typicode/json-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/json-server/)</sub>

<a name="nebula"></a>
### #&#8288;283 [vesoft-inc/nebula](https://github.com/vesoft-inc/nebula) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (70) · Freshness: recent (70) · Maintenance: weak (12) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Sep 2026</sub>

**Distributed graph database with OpenCypher-compatible queries.**

NebulaGraph is a graph database written in C++ that separates storage from compute and scales horizontally. It uses the Raft protocol for strong consistency, accepts an OpenCypher-compatible query language, and has role-based access control. The README points to its docs for install and quick start.

- **+** Storage and compute are separate, so each layer scales horizontally on its own
- **+** Raft consensus gives strong data consistency across replicas
- **+** OpenCypher-compatible query language
- **+** Apache-2.0 license allows use as a SaaS backend
- **−** Multi-component distributed deployment is heavier than single-binary databases
- **−** README lists build from source or AWS cloud; no Docker or compose files detected
- **−** Last release is 2024-05-17, though commits continue
- **−** Not an AI or LLM tool itself, so fit for AI starters is indirect

<sub>no GPU · Docker · [Repo](https://github.com/vesoft-inc/nebula) · [📖 Docs ↗](https://docs.nebula-graph.io/) · [🌐 Site ↗](https://nebula-graph.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nebula/)</sub>

<a name="sqlboiler"></a>
### #&#8288;284 [sqlboiler](https://github.com/aarondl/sqlboiler) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (58) · Freshness: recent (72) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · custom license · Nov 2026</sub>

**Database-first Go ORM generator that builds typed models from your schema.**

SQLBoiler is a command-line code generator that reads an existing database schema and emits a type-safe Go ORM package, including queries, relationships with eager loading, hooks, transactions and generated tests. Drivers cover PostgreSQL, MySQL, MSSQL 2012+ and SQLite3, with CockroachDB as a third-party driver. It is not an AI project, and the README says it is in maintenance mode and points to Bob and sqlc as maintained alternatives.

- **+** Generates typed models from the live schema, avoiding a reflection-heavy runtime layer
- **+** Relationships, recursive eager loading, hooks, auto timestamps and soft deletes are generated
- **+** Works with any boil.Executor, including *sql.DB, *sql.Tx and sqlx.DB
- **+** Drivers for PostgreSQL, MySQL, MSSQL and SQLite3, plus support for out-of-band drivers
- **−** Maintenance mode: no new features, and maintainers usually do not resolve reported issues
- **−** No multi-column foreign key support
- **−** Materialized views supported on PostgreSQL only
- **−** Schema must exist first; migrations need a separate tool such as sql-migrate

<sub>no GPU · Needs Go 1.13+, PostgreSQL, MySQL 5.6.30+, MSSQL 2012+ or SQLite3 for generation · [Repo](https://github.com/aarondl/sqlboiler) · [📖 Docs ↗](https://pkg.go.dev/mod/github.com/aarondl/sqlboiler/v4) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sqlboiler/)</sub>

<a name="qor"></a>
### #&#8288;285 [qor](https://github.com/qor/qor) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: known (50) · Freshness: recent (70) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Nov 2026</sub>

**Go libraries for building admin panels, CMS and e-commerce back offices.**

QOR is a set of Go libraries for business applications, CMSs and e-commerce systems. Modules include Admin (generates an admin UI and RESTful API from data models), Publish (staged content review), Transition (state machine), Media Library, Worker, Exchange (CSV/Excel), i18n, l10n and Roles. It is a toolkit, not a turnkey product, and the README does not mention AI features.

- **+** Admin module generates an admin interface and RESTful API from data models
- **+** Modular: publish staging, state machine, roles, i18n/l10n and CSV/Excel exchange as separate libraries
- **+** Media Library supports several cloud storage backends and CDN publishing
- **+** Live demo and example app source are available
- **−** No AI or LLM functionality; weak fit for an AI-focused list
- **−** Last release was 2022-11-14, so tagged versions are old
- **−** Not turnkey; requires Go coding skills to assemble a system
- **−** Frontend build needs Node.js and Gulp

<sub>no GPU · Needs Go, Node.js, Gulp · [Repo](https://github.com/qor/qor) · [📖 Docs ↗](https://doc.getqor.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qor/)</sub>

<a name="classic-jazz"></a>
### #&#8288;286 [classic-jazz](https://github.com/garden-co/classic-jazz) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

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
### #&#8288;287 [matecloud](https://github.com/mateaix/matecloud) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

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

<a name="exograph"></a>
### #&#8288;288 [exograph](https://github.com/exograph/exograph) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (1) · Freshness: active (98) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 352 · custom license · Nov 2026</sub>

**Declarative backend framework that generates GraphQL APIs from a domain model.**

Exograph is a backend framework written in Rust. You describe your domain model and business logic declaratively, and it provides GraphQL query and mutation APIs. The README links example projects that pair it with Next.js, Apollo, Urql, Auth0, Clerk and Tailwind.

- **+** Provides GraphQL queries and mutations from a declarative domain model
- **+** Examples repo covers Next.js, Apollo, Urql, Auth0, Clerk and Tailwind
- **+** Written in Rust, with local build steps in DEVELOPMENT.md
- **−** README describes GraphQL APIs only, with no REST option mentioned
- **−** License is reported as NOASSERTION, so terms need manual checking
- **−** No AI or model integration described; it is a general backend
- **−** No Dockerfile or compose file detected in the repository

<sub>Docker · [Repo](https://github.com/exograph/exograph) · [📖 Docs ↗](https://exograph.dev/docs) · [🌐 Site ↗](https://exograph.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/exograph/)</sub>

<a name="steedos-platform"></a>
### #&#8288;289 [steedos-platform](https://github.com/steedos/steedos-platform) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (17) · Freshness: active (91) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · AGPL-3.0 · Nov 2026</sub>

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

<a name="openwhisk"></a>
### #&#8288;290 [openwhisk](https://github.com/apache/openwhisk) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: popular (57) · Freshness: recent (70) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · Apache-2.0 · Nov 2026</sub>

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

<a name="motor"></a>
### #&#8288;291 [motor](https://github.com/mongodb/motor) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (29) · Freshness: recent (70) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Nov 2026</sub>

**Non-blocking MongoDB driver for Python asyncio and Tornado.**

Motor is a coroutine-based MongoDB driver for asyncio and Tornado applications, built on PyMongo (>=4.9,<5) and requiring Python 3.11+. It is deprecated as of May 14, 2025 in favor of the PyMongo Async API, with only critical bug fixes until final support ends May 14, 2027. It is a database client library, not an AI project.

- **+** Coroutine API for both asyncio and Tornado
- **+** Optional extras for gssapi, aws, srv, ocsp, snappy, zstd and client-side encryption
- **+** Supports the same optional dependencies as PyMongo
- **+** Installs with a single pip command; documented on ReadTheDocs
- **−** Deprecated; no new features, and the May 14, 2026 end-of-life date has passed
- **−** Only critical fixes until support ends May 14, 2027
- **−** Requires a separate MongoDB server and PyMongo
- **−** Not an AI tool; fits this list only loosely as a database client

<sub>no GPU · Needs MongoDB, PyMongo >=4.9,<5, Python 3.11+ · [Repo](https://github.com/mongodb/motor) · [📖 Docs ↗](https://motor.readthedocs.io/en/stable/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/motor/)</sub>

<a name="go-restful"></a>
### #&#8288;292 [go-restful](https://github.com/emicklei/go-restful) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: known (48) · Freshness: recent (76) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

**Go package for building REST web services with routing, filters and JSON/XML.**

go-restful is a Go library for defining REST APIs by mapping HTTP methods and path patterns to handler functions grouped into WebServices. It reads and writes JSON and XML, supports filters at service or route level, and handles gzip/deflate, CORS, OPTIONS and panic recovery. It is a general HTTP library with no AI-specific features.

- **+** Default router supports path params, regex and Google custom methods like /resource/name:customVerb
- **+** Filters at service or route level cover CORS, OPTIONS and content encoding
- **+** Swagger/OpenAPI declaration available via the separate go-restful-openapi package
- **+** Hooks for router, JSON decoder, compression, panic recovery and error handlers
- **−** No AI, model or agent functionality; it is a generic HTTP service library
- **−** Go modules supported only from v3; v2 and earlier do not support them
- **−** Only JSON and XML built in; other serializers need custom EntityReaderWriter
- **−** Last release (2025-08-15) is older than the latest commit (2026-10-08)

<sub>no GPU · [Repo](https://github.com/emicklei/go-restful) · [📖 Docs ↗](https://pkg.go.dev/github.com/emicklei/go-restful/v3) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-restful/)</sub>

<a name="kubero"></a>
### #&#8288;293 [kubero](https://github.com/kubero-dev/kubero) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: known (43) · Freshness: recent (79) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · GPL-3.0 · Oct 2026</sub>

**Self-hosted PaaS that deploys containers and Git apps on Kubernetes.**

Kubero is a self-hosted Heroku-style PaaS that runs on Kubernetes through two containers, a web UI and an operator. It deploys existing Docker images or builds from Git (GitHub, GitLab, Gitea, Bitbucket, Gogs) into pipelines with up to four staging environments and PR review apps. It ships 160+ app templates and add-ons such as PostgreSQL and Redis, and stores state in etcd rather than a separate database.

- **+** No extra database: all state is stored in the cluster's etcd
- **+** Pipelines with up to 4 staging stages and automatic PR review apps
- **+** 160+ app templates and built-in add-ons like PostgreSQL, Redis, MongoDB
- **+** UI, CLI and API; GitHub and OAuth2 SSO, scheduled vulnerability scans
- **−** Requires a Kubernetes cluster; it is not a single-host Docker tool
- **−** Built-in add-ons are not HA ready; HA needs separate operators
- **−** Bitnami-based add-ons are deprecated and slated for removal
- **−** GPL-3.0 license; last tagged release is 2025-09-17

<sub>no GPU · Docker + Compose · Needs Kubernetes, Kubero Operator, Kubero CLI · [Repo](https://github.com/kubero-dev/kubero) · [▶️ Demo ↗](https://demo.kubero.dev) · [📖 Docs ↗](https://www.kubero.dev/docs/) · [🌐 Site ↗](https://www.kubero.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubero/)</sub>

<a name="laf"></a>
### #&#8288;294 [laf](https://github.com/labring/laf) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (59) · Freshness: recent (63) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · Apache-2.0 · Jul 2026</sub>

**Cloud development platform with JS/TS cloud functions, database and storage.**

laf is a cloud development platform that provides cloud functions written in JS/TS, a cloud database, object storage, static website hosting and WebSocket support. Functions are edited and published from a web IDE, and a client SDK targets any JS runtime. Self-hosting requires a Kubernetes cluster with your own domain, certificates and gateway.

- **+** Functions, database, storage, hosting and WebSocket bundled in one platform
- **+** Web IDE edits and publishes functions, with logs viewable in the browser
- **+** JS/TS functions share a language with frontend code; client SDK runs in any JS runtime
- **+** Self-hostable, so apps avoid vendor lock-in and source can be delivered to clients
- **−** Self-hosting needs Kubernetes operations knowledge, plus domain, certificate and gateway setup
- **−** Last release is 2023-12-19, though commits continue
- **−** README and main docs are primarily in Chinese
- **−** Flutter, Android and iOS SDKs are listed only as future work

<sub>no GPU · Needs Kubernetes · [Repo](https://github.com/labring/laf) · [▶️ Demo ↗](https://bja.sealos.run) · [🌐 Site ↗](https://laf.run/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/laf/)</sub>

<a name="keto"></a>
### #&#8288;295 [keto](https://github.com/ory/keto) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (50) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · Apache-2.0 · Jul 2026</sub>

**Open-source Zanzibar-style authorization server for relationship-based permission checks.**

Ory Keto is a Go server implementing Google's Zanzibar model. You define namespaces in the Ory Permission Language, store relation tuples, and query them to check permissions (ReBAC). The README claims sub-10ms checks and horizontal scaling to billions of relationships, with PostgreSQL, MySQL or CockroachDB as storage.

- **+** Implements the Zanzibar relation-tuple model with a dedicated policy language (OPL)
- **+** Supports PostgreSQL, MySQL and CockroachDB as storage
- **+** Installs on Linux, macOS, Windows, Docker and Kubernetes, or builds from source
- **+** Works with any identity provider; not tied to other Ory components
- **−** Enterprise features, CVE-patch SLAs and multi-tenancy require the paid Ory Enterprise License
- **−** Quickstart uses the Ory Network hosted service, not a local self-hosted run
- **−** Authorization only; identity and login need separate tools such as Kratos
- **−** Latency and scale figures are README claims with no benchmark shown

<sub>no GPU · Docker + Compose · Needs PostgreSQL, MySQL, CockroachDB · [Repo](https://github.com/ory/keto) · [📖 Docs ↗](https://www.ory.com/docs/keto) · [🌐 Site ↗](https://www.ory.com/cloud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/keto/)</sub>

<a name="judge0"></a>
### #&#8288;296 [judge0](https://github.com/judge0/judge0) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (44) · Freshness: recent (70) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · GPL-3.0 · Oct 2026</sub>

**Sandboxed code execution API for 90+ languages, self-hosted or managed.**

Judge0 is an HTTP JSON API that compiles and runs untrusted source code in a sandbox and returns stdout, stderr and execution results. It supports 90+ languages, multi-file projects, custom compiler options, time and memory limits, and webhooks. It targets online judges, coding assessment sites, online IDEs and AI agents that run generated code, with a Python SDK available.

- **+** Simple HTTP JSON API; one curl call to /submissions?wait=true returns results
- **+** Per-submission compiler options, command-line arguments, time and memory limits
- **+** Supports multi-file programs and additional files alongside the user's program
- **+** Official Python SDK and published architecture paper
- **−** Last tagged release is 2024-04-18, though commits continue
- **−** GPL-3.0 license may constrain embedding in proprietary products
- **−** Self-hosting steps live in CHANGELOG.md rather than the README
- **−** Judge0 Extra CE with additional languages is on a separate `extra` branch

<sub>Docker + Compose · Compose runs PostgreSQL, Redis · [Repo](https://github.com/judge0/judge0) · [▶️ Demo ↗](https://ide.judge0.com) · [📖 Docs ↗](https://ce.judge0.com) · [🌐 Site ↗](https://judge0.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/judge0/)</sub>

<a name="amplication"></a>
### #&#8288;297 [amplication](https://github.com/amplication/amplication) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: popular (76) · Freshness: recent (59) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · custom license · Apr 2026</sub>

**Generates NestJS and Node.js backend services from data models, with team templates.**

Amplication generates backend microservices (APIs, data models, DTOs) from a modeled domain, and pushes the code to your Git repository. Organizations can define their own live templates and plugins so generated services follow shared standards, and the tool handles package updates and versioning. It can be used hosted at app.amplication.com or run locally as an Nx monorepo for development.

- **+** Generates editable service code (APIs, data models, DTOs) that you own and commit to Git
- **+** Plugin system and custom live templates enforce shared standards across services
- **+** Handles package updates, patches and versioning of generated services
- **+** Hosted version available, so no local setup is needed to try it
- **−** Components under the ee directory use a separate Enterprise Edition license
- **−** Self-hosting is documented only as a development setup, not a production deployment guide
- **−** Local setup needs Node.js, Docker and several services run via npm scripts

<sub>no GPU · Compose · Needs Node.js, Docker, Git · [Repo](https://github.com/amplication/amplication) · [🌐 Site ↗](https://amplication.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/amplication/)</sub>

<a name="pony"></a>
### #&#8288;298 [pony](https://github.com/ponyorm/pony) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (38) · Freshness: active (96) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Aug 2026</sub>

**Python ORM that translates generator expressions into SQL queries.**

Pony is a Python object-relational mapper that analyzes the abstract syntax tree of generator expressions and lambdas and translates them into SQL. It supports SQLite, MySQL, PostgreSQL and Oracle. It is a general database library, not an AI project, so it fits the list only loosely as a backend building block.

- **+** Queries written as Python generator expressions, e.g. select(p for p in Product if ...)
- **+** Supports SQLite, MySQL, PostgreSQL and Oracle dialects
- **+** Error messages point to the exact part of the query; generated SQL is printed indented
- **+** Apache-2.0 licensed with hosted documentation and an online ER diagram editor
- **−** No AI or LLM functionality; only a database access layer
- **−** Generator-expression query style differs from the more common SQLAlchemy and Django ORM APIs
- **−** README lists no async support, migrations tool or supported Python versions
- **−** Does not cover auth, storage or hosting; it is only an ORM

<sub>no GPU · Needs SQLite, MySQL, PostgreSQL or Oracle database · [Repo](https://github.com/ponyorm/pony) · [📖 Docs ↗](https://docs.ponyorm.org) · [🌐 Site ↗](https://ponyorm.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pony/)</sub>

<a name="pg"></a>
### #&#8288;299 [pg](https://github.com/go-pg/pg) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (52) · Freshness: recent (78) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · BSD-2-Clause · May 2026</sub>

**PostgreSQL client and ORM for Go, now in maintenance mode.**

go-pg is a Go PostgreSQL client with a struct-based ORM, covering relations (has one, belongs to, has many, many to many), transactions, prepared statements, LISTEN/NOTIFY, COPY, bulk operations and connection pooling with a circuit breaker. The README states it is in maintenance mode, with only critical issues fixed and new development moving to Bun.

- **+** Native PostgreSQL types: arrays, hstore, composite types, plus LISTEN/NOTIFY and COPY FROM/TO
- **+** ORM covers has-one, belongs-to, has-many and many-to-many with composite primary keys
- **+** Built-in connection pooling with circuit breaker and retry on network errors
- **+** Query timeouts and cancellation through context.Context
- **−** Maintenance mode: only critical issues fixed, new development happens in Bun
- **−** PostgreSQL only; Bun is the option for MySQL, MariaDB or SQLite
- **−** Go zero values are written as NULL unless tagged use_zero
- **−** Import path needs the /v10 suffix, which the README calls a popular mistake

<sub>no GPU · Needs PostgreSQL · [Repo](https://github.com/go-pg/pg) · [📖 Docs ↗](https://pg.uptrace.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pg/)</sub>

<a name="spring-boot-jwt"></a>
### #&#8288;300 [spring-boot-jwt](https://github.com/murraco/spring-boot-jwt) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Oct 2026</sub>

**Spring Boot JWT auth service with rotating, revocable refresh tokens.**

A Spring Boot 3.5 / Java 17 REST API that implements signup, signin, refresh and logout using Spring Security. Access tokens are stateless HMAC-SHA256 JWTs (JJWT 0.12.x); refresh tokens are opaque, stored as SHA-256 hashes, single-use, with reuse detection that revokes all of a user's tokens. Runs on in-memory H2 by default, with MySQL as an option, and exposes SpringDoc OpenAPI docs.

- **+** Refresh tokens are hashed at rest, single-use, with reuse detection revoking all user tokens
- **+** Ordinary requests need no database lookup for authentication; only refresh hits the DB
- **+** Role checks via @PreAuthorize with ROLE_ADMIN and ROLE_CLIENT, plus OpenAPI docs
- **+** Small, readable code layout with a controller test and CI workflow
- **−** Access tokens cannot be revoked before expiry; only lifetime tuning limits exposure
- **−** Default config is H2 in-memory with create-drop schema, not production-ready
- **−** H2 console is permitted in security config and must be disabled for production
- **−** No tagged releases; it is a demo service, not a packaged library

<sub>no GPU · Docker · Needs Java 17, H2 (default, in-memory), MySQL (optional) · port 8080 · [Repo](https://github.com/murraco/spring-boot-jwt) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spring-boot-jwt/)</sub>

<a name="db"></a>
### #&#8288;301 [db](https://github.com/upper/db) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: known (37) · Freshness: recent (70) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**Go data access layer with one API for SQL databases and MongoDB.**

upper/db is a Go library that provides a common data access API over PostgreSQL, MySQL, MSSQL, CockroachDB, SQLite, QL and MongoDB through per-database adapters. It is not AI-specific; it is a general database layer that sits under any Go backend. The README points to v4 documentation and an in-browser tour.

- **+** One API across seven data sources, including SQL databases and MongoDB
- **+** MIT licensed, with a separate adapter per database
- **+** Browser-based tour with live examples
- **+** Documentation published for v4
- **−** No AI features; only loosely fits a vibe-coding list
- **−** Library only, not a backend, hosting or auth platform
- **−** Last release 2025-03-09, well behind the latest commit
- **−** README gives little detail on the query API

<sub>no GPU · Needs PostgreSQL, MySQL, MSSQL, CockroachDB, MongoDB, QL or SQLite (one of) · [Repo](https://github.com/upper/db) · [▶️ Demo ↗](https://tour.upper.io) · [📖 Docs ↗](https://upper.io/v4) · [🌐 Site ↗](https://upper.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/db/)</sub>

<a name="devise-token-auth"></a>
### #&#8288;302 [devise_token_auth](https://github.com/lynndylanhurley/devise_token_auth) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: known (37) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · WTFPL · Jul 2026</sub>

**Token-based authentication gem for Rails APIs, built on Devise and OmniAuth.**

Devise Token Auth is a Ruby gem that adds token-based authentication to Rails apps serving SPAs and mobile clients. It refreshes tokens on each request, expires them after a short time, and keeps a separate session per client or device. It supports email registration, login, password reset and confirmation through Devise, OAuth2 through OmniAuth, and multiple user models.

- **+** Per-device sessions with tokens refreshed on every request and short expiry
- **+** Email auth via Devise and OAuth2 via OmniAuth in one gem
- **+** Supports multiple user models in a single Rails app
- **+** Documented client libraries for Angular, React/Redux, jQuery and Flutter
- **−** Rails only; no use outside Ruby on Rails apps
- **−** Depends on Devise and OmniAuth, so inherits their configuration surface
- **−** No tagged release is listed for the repository
- **−** Client libraries are separate third-party projects, not maintained here

<sub>no GPU · Needs Rails, Devise, OmniAuth · [Repo](https://github.com/lynndylanhurley/devise_token_auth) · [▶️ Demo ↗](https://stackblitz.com/github/neroniaky/angular-token) · [📖 Docs ↗](https://devise-token-auth.gitbook.io/devise-token-auth) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/devise-token-auth/)</sub>

<a name="dicedb"></a>
### #&#8288;303 [dicedb](https://github.com/dicedb/dicedb) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: popular (67) · Freshness: slowing (48) · Maintenance: weak (8) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Mar 2026</sub>

**Valkey fork that spills evicted keys to disk via RocksDB.**

DiceDB is a fork of Valkey (itself a Redis fork) that stays compatible with Redis and Valkey clients and tooling. Its main addition is the dicedb-spill module, which writes evicted keys to disk with RocksDB and restores them on cache misses, so the working set can exceed the memory limit. The original Go engine is archived as dice-legacy.

- **+** Compatible with Valkey and Redis clients, SDKs and tooling
- **+** Spill module persists evicted keys to disk and reloads them on cache miss
- **+** Builds from source on Linux, macOS, OpenBSD, NetBSD and FreeBSD
- **+** Ships dicedb-server and dicedb-cli; examples use port 6379
- **−** Only one documented extension over Valkey: the spill module
- **−** Logs, metrics and code still reference Valkey
- **−** Legacy Go engine with reactivity is archived; features only gradually ported
- **−** License detected as NOASSERTION, so terms need manual checking

<sub>no GPU · Needs RocksDB (spill module) · [Repo](https://github.com/dicedb/dicedb) · [📖 Docs ↗](https://dicedb.io/docs/conf) · [🌐 Site ↗](https://dicedb.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dicedb/)</sub>

<a name="flask-sqlalchemy"></a>
### #&#8288;304 [flask-sqlalchemy](https://github.com/pallets-eco/flask-sqlalchemy) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: known (42) · Freshness: slowing (45) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · BSD-3-Clause · May 2026</sub>

**Flask extension that integrates SQLAlchemy with app config and sessions.**

Flask-SQLAlchemy is a Flask extension that wires SQLAlchemy into a Flask app. It reads the database URI from app config and exposes a db object with Model, session, select and create_all helpers, scoped to the Flask app context. It is a library for adding a database layer, not an AI project or a runnable starter.

- **+** Configures SQLAlchemy from Flask config via SQLALCHEMY_DATABASE_URI
- **+** Supports SQLAlchemy 2.x style DeclarativeBase with Mapped and mapped_column
- **+** Maintained under Pallets-Eco, with a commit in May 2026
- **+** BSD-3-Clause license
- **−** Library only: no auth, billing, API or AI features included
- **−** Last tagged release is September 2023
- **−** Tied to Flask; not usable with other web frameworks
- **−** Community-maintained, with the README asking for more maintainers

<sub>no GPU · Needs Flask, SQLAlchemy · [Repo](https://github.com/pallets-eco/flask-sqlalchemy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flask-sqlalchemy/)</sub>

<a name="nubase"></a>
### #&#8288;305 [nubase](https://github.com/ottermind/nubase) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 622 · Apache-2.0 · Nov 2026</sub>

**Self-hosted multi-project backend that coding agents drive over MCP.**

Nubase is a Java backend with a Next.js Studio that gives each project its own PostgreSQL database, a PostgREST-compatible REST API, Supabase-style auth, S3-compatible storage, edge functions, static asset hosting, cron, an AI gateway and a Mem0-style memory API. Coding agents operate it through an MCP bridge (nubase_cli) to create tables, deploy functions and publish a generated frontend. One all-in-one Docker image bundles Postgres, Redis, backend and Studio.

- **+** One control plane provisions many isolated projects, each with its own Postgres database
- **+** Agents can deploy functions, publish frontends to /assets/v1 and schedule cron via MCP tools
- **+** Built-in memory API using pgvector, Postgres full-text and entity boost retrieval
- **+** Single docker run starts Postgres, Redis, backend and Studio on port 9999
- **−** Realtime is not implemented
- **−** No backups/PITR, HA or enterprise SSO/SCIM yet
- **−** README calls it early-stage and says to review admin endpoints before public exposure
- **−** REST layer is a Java reimplementation, so PostgREST parity is not guaranteed

<sub>no GPU · Docker · Needs PostgreSQL 15 with pgvector, Redis, S3/R2/MinIO (optional storage), Cloudflare Workers for Platforms (optional), LLM provider (optional, for Memory) · Models: OpenAI, Anthropic, OpenAI-compatible providers · port 9999 · [Repo](https://github.com/ottermind/nubase) · [🌐 Site ↗](https://nubase.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nubase/)</sub>

<a name="buffalo"></a>
### #&#8288;306 [buffalo](https://github.com/gobuffalo/buffalo) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: popular (61) · Freshness: recent (54) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Mar 2026</sub>

**Go web framework that generates a full project with frontend, routing and database.**

Buffalo generates a Go web project with front-end assets (JavaScript, SCSS), routing, templating and an optional database layer already wired together. It builds on gorilla/mux for routing, Plush for templates, Pop/Soda for the ORM and migrations, and Gorilla packages for sessions, cookies and WebSockets. It is a general web framework with no AI features.

- **+** Generates front-end and back-end scaffolding in one project structure
- **+** Reuses established parts: gorilla/mux, Plush templates, Pop ORM with Soda CLI
- **+** Database layer is optional
- **+** Supports the last two Go releases (1.23 and 1.24 per README)
- **−** No AI or LLM functionality; fit for this list is loose
- **−** Requires Go modules; GOPATH mode is likely to break it
- **−** Publishes no benchmarks; README says it uses a router not chosen for speed
- **−** Support is mainly via Slack and Stack Overflow; issues are for bugs only

<sub>no GPU · Docker · Needs Go 1.23 or 1.24, Go modules, Database (optional, via Pop) · [Repo](https://github.com/gobuffalo/buffalo) · [📖 Docs ↗](https://gobuffalo.io/documentation/getting_started/installation) · [🌐 Site ↗](http://gobuffalo.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/buffalo/)</sub>

<a name="incubator-pegasus"></a>
### #&#8288;307 [incubator-pegasus](https://github.com/apache/incubator-pegasus) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (24) · Freshness: recent (70) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

**Distributed key-value store with strong consistency, built on RocksDB.**

Apache Pegasus is a horizontally scalable key-value store written in C++. It uses hash partitioning and the PacificA protocol for strongly consistent replication, and RocksDB as the storage engine. Each write is replicated three ways before the client gets a response. It sits between Redis and HBase and has client drivers for six languages. It is not an AI project, so it fits this list only loosely.

- **+** Strong consistency via PacificA, with three-way replication before write acknowledgement
- **+** Built-in load balancing, cold backup to HDFS or local disk, and cross-cluster duplication
- **+** Clients for Java, C++, Go, Python, Node.js and Scala
- **+** Write path relies only on the local filesystem, unlike HBase
- **−** Not an AI project; no model, embedding or agent features
- **−** Last release is 2023-12-11, and the README warns master may be broken
- **−** Cluster has separate MetaServer and ReplicaServer roles, heavier than a single-node store
- **−** No Docker or compose files detected in the repository

<sub>no GPU · Docker + Compose · Needs RocksDB, HDFS (optional, for backups) · [Repo](https://github.com/apache/incubator-pegasus) · [📖 Docs ↗](https://pegasus.apache.org) · [🌐 Site ↗](https://pegasus.apache.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/incubator-pegasus/)</sub>

<a name="djongo"></a>
### #&#8288;308 [djongo](https://github.com/doableware/djongo) <sub>score [35](../README.md#-how-we-rank "Score 35/100. Adoption: niche (22) · Freshness: recent (70) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · AGPL-3.0 · Oct 2026</sub>

**Django database backend that runs the ORM against MongoDB.**

djongo is a Django database engine that compiles the SQL generated by the Django ORM into MongoDB query documents. Existing models, migrations and contrib apps (admin, auth, sessions) work against MongoDB, and it adds embedded model, embedded array and embedded form fields. Setup is a pip install plus an ENGINE setting in settings.py.

- **+** Keeps the standard Django ORM; no model rewrite to adopt MongoDB
- **+** Django Admin can add and edit MongoDB documents
- **+** Embedded model and embedded array fields for nested documents
- **+** Setup is one pip install and a DATABASES entry
- **−** Translates SQL to MongoDB queries, so complex ORM queries may not map cleanly
- **−** Subqueries and nested querysets require MongoDB 3.6 or higher
- **−** AGPL-3.0 license may restrict use in closed-source network services
- **−** Last tagged release is from 2018 despite recent commits

<sub>no GPU · Needs Django, MongoDB 3.4+, Python 3.6+ · [Repo](https://github.com/doableware/djongo) · [📖 Docs ↗](https://www.djongomapper.com/) · [🌐 Site ↗](https://www.djongomapper.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/djongo/)</sub>

<a name="lowdb"></a>
### #&#8288;309 [lowdb](https://github.com/typicode/lowdb) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: widely used (83) · Freshness: slowing (32) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Mar 2026</sub>

**Local JSON file database for Node.js and browsers, queried with plain JavaScript.**

lowdb is a pure ESM npm library that loads a JSON file into a plain JavaScript object (db.data) and writes it back with db.write() or db.update(). Storage is pluggable through adapters: JSON file, in-memory, localStorage and sessionStorage, plus custom ones for YAML or encryption. It ships TypeScript types and uses atomic file writes.

- **+** No server or external dependency; data lives in a single JSON file
- **+** Queries use native Array methods; optional Lodash extension via a Low subclass
- **+** Adapters allow other formats, encryption or remote storage with two methods
- **+** Memory adapter speeds up tests; TypeScript types check the data shape
- **−** Each write serializes the whole dataset; objects of ~10-100MB can slow down
- **−** Does not support Node's cluster module
- **−** Pure ESM package, which can cause problems in CommonJS projects
- **−** No indexing or query engine; README recommends PostgreSQL or MongoDB for scale

<sub>no GPU · [Repo](https://github.com/typicode/lowdb) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lowdb/)</sub>

<a name="ballcat"></a>
### #&#8288;310 [ballcat](https://github.com/ballcat-projects/ballcat) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (19) · Freshness: active (93) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Jul 2026</sub>

**Java component library for building admin-backend projects quickly.**

BallCat is a set of Java components published to Maven Central that provide base capabilities for building admin-system backends. It sits alongside separate repos for business modules, a code generator, a server template (ballcat-boot) and React and Vue admin frontends. The master branch is the 2.x line, which the README marks as still in development; 1.x lives on its own branch.

- **+** All JARs are published to Maven Central, with changelogs for each version
- **+** Companion repos cover code generation, server template and React, Vue2, Vue3 admin UIs
- **+** Separate documentation sites for 1.x and 2.x
- **+** Apache-2.0 license
- **−** Master branch is 2.x and the README says it is still in development
- **−** No AI features; it is a general Java admin framework
- **−** README and community channels are in Chinese, with a WeChat group for support
- **−** No Docker or Compose files in this repo

<sub>no GPU · Needs Java, Maven · [Repo](https://github.com/ballcat-projects/ballcat) · [📖 Docs ↗](https://v2.ballcat.cn/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ballcat/)</sub>

<a name="vearch"></a>
### #&#8288;311 [vearch](https://github.com/vearch/vearch) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (26) · Freshness: active (83) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · Apache-2.0 · Jul 2026</sub>

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

<a name="foal"></a>
### #&#8288;312 [foal](https://github.com/foalts/foal) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (22) · Freshness: active (88) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Jul 2026</sub>

**TypeScript Node.js web framework with CLI, ORM, auth and GraphQL support.**

FoalTS is a general-purpose Node.js framework written in TypeScript. It bundles a CLI, ORM, authentication, testing tools, GraphQL and Swagger API support, and AWS utilities, so an app does not need separately assembled npm packages. It contains no AI features; it is a conventional backend framework, scaffolded with `npx @foal/cli createapp`.

- **+** Auth, ORM, CLI, GraphQL and Swagger included in one framework
- **+** Written entirely in TypeScript with static typing
- **+** README cites more than 2100 tests (as of December 2020)
- **+** Published LTS schedule: 5.x active, supports Node 22 and 24
- **−** No built-in AI, LLM or agent features
- **−** Not a hosted or self-hosted backend service; you write and deploy the app yourself
- **−** Version 5.x requires Node 22 or 24 and TypeScript 5.5+
- **−** Smaller community than Express or NestJS (about 1.9k stars)

<sub>no GPU · Compose · Compose runs MySQL, PostgreSQL, MongoDB, Redis · port 3001 · [Repo](https://github.com/foalts/foal) · [📖 Docs ↗](https://foalts.org/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/foal/)</sub>

<a name="flask-migrate"></a>
### #&#8288;313 [flask-migrate](https://github.com/miguelgrinberg/flask-migrate) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (27) · Freshness: recent (70) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Aug 2026</sub>

**Flask extension for SQLAlchemy database migrations using Alembic.**

Flask-Migrate wraps Alembic so Flask apps using SQLAlchemy can create, autogenerate and apply schema migrations through `flask db` subcommands such as init, migrate and upgrade. It adds a `migrations` folder to the project that is committed to version control. It is general database tooling, not AI-specific, so it fits this list only as a backend building block.

- **+** Exposes Alembic through `flask db init`, `migrate` and `upgrade` commands
- **+** Migration scripts live in a `migrations` folder versioned with the code
- **+** Installs with a single `pip install Flask-Migrate`
- **+** MIT licensed, with documentation on readthedocs
- **−** Autogenerated migrations must be reviewed and edited by hand
- **−** Alembic does not detect indexes, per the README
- **−** Only for Flask apps using SQLAlchemy
- **−** Last release was 2025-01-10; later commits are unreleased

<sub>no GPU · Needs Flask, SQLAlchemy, Alembic, Flask-SQLAlchemy · [Repo](https://github.com/miguelgrinberg/flask-migrate) · [📖 Docs ↗](https://flask-migrate.readthedocs.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flask-migrate/)</sub>

<a name="ferretdb"></a>
### #&#8288;314 [ferretdb](https://github.com/ferretdb/ferretdb) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: popular (68) · Freshness: slowing (33) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Feb 2026</sub>

**MongoDB-compatible proxy that stores documents in PostgreSQL.**

FerretDB is a Go proxy that accepts MongoDB 5.0+ wire protocol traffic and translates it to SQL against PostgreSQL with the DocumentDB extension. Existing MongoDB drivers and tools connect unchanged, on port 27017 in the quickstart. It can also be embedded as a Go library, and it targets users who want a MongoDB-style API without the SSPL license.

- **+** Works with standard MongoDB drivers and tools, no application changes in many cases
- **+** Apache-2.0 licensed, avoiding MongoDB's SSPL
- **+** Data lives in PostgreSQL, so Postgres tooling and psql access still apply
- **+** Ships binaries, Linux packages, a Docker image and an embeddable Go library
- **−** Not full MongoDB parity; a compatibility page lists known differences and unsupported commands
- **−** Requires PostgreSQL with the DocumentDB extension as the storage engine
- **−** Eval Docker image keeps data inside the container and is not for production
- **−** README advises against building from source; use provided binaries or packages

<sub>no GPU · Compose · Needs PostgreSQL, DocumentDB extension · [Repo](https://github.com/ferretdb/ferretdb) · [📖 Docs ↗](https://docs.ferretdb.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ferretdb/)</sub>

<a name="graphql"></a>
### #&#8288;315 [graphql](https://github.com/redwoodjs/graphql) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: popular (79) · Freshness: quiet (17) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Dec 2025</sub>

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

<sub>no GPU · Needs Node.js, Prisma-supported database · [Repo](https://github.com/redwoodjs/graphql) · [🌐 Site ↗](https://redwoodjs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphql/)</sub>

<a name="sled"></a>
### #&#8288;316 [sled](https://github.com/spacejam/sled) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: popular (63) · Freshness: slowing (34) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · Apache-2.0 · Apr 2026</sub>

**Embedded key-value database for Rust with a BTreeMap-like API.**

sled is an embedded Rust database exposing a thread-safe, ordered byte-key API similar to BTreeMap, with ACID multi-key transactions, compare-and-swap, write batches and prefix subscriptions. It uses a lock-free tree over a log-structured pagecache and fsyncs every 500ms by default. The README states it is beta, the on-disk format will change before 1.0.0, and the README is out of sync with a main branch undergoing a rewrite.

- **+** Serializable transactions across multiple keys and keyspaces
- **+** Ordered range queries with forward and reverse iterators
- **+** Prefix watch subscriptions that can be awaited as a Future
- **+** Optional zstd compression via the `compression` build feature
- **−** Beta; README says to use SQLite if reliability is the primary constraint
- **−** On-disk format will change before 1.0.0, requiring manual migrations
- **−** Can use too much disk space; README points to RocksDB for that
- **−** Only one open instance per process; last release was 2021-09

<sub>no GPU · [Repo](https://github.com/spacejam/sled) · [📖 Docs ↗](https://docs.rs/sled) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sled/)</sub>

<a name="gel"></a>
### #&#8288;317 [gel](https://github.com/geldata/gel) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: popular (72) · Freshness: quiet (21) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Dec 2025</sub>

**Graph-relational database with object types and the EdgeQL query language.**

Gel is a database that models data as object types with properties and links instead of tables and foreign keys. Queries are written in EdgeQL, which returns nested objects rather than flat rows. It ships with a migrations system, a CLI, client libraries in several languages, and an optional managed cloud service.

- **+** EdgeQL returns nested objects, so related data is fetched without JOINs
- **+** Composable queries allow subqueries and nested mutations
- **+** Built-in migrations system, CLI and client libraries in multiple languages
- **+** Schema supports constraints, indexes, computed properties, link properties and mixins
- **−** Requires learning EdgeQL and its schema language instead of SQL
- **−** No Docker or compose setup described in the README
- **−** README quickstart still uses the legacy `edgedb` CLI command
- **−** Managed hosting is a separate cloud service

<sub>no GPU · [Repo](https://github.com/geldata/gel) · [📖 Docs ↗](https://docs.geldata.com) · [🌐 Site ↗](https://www.geldata.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gel/)</sub>

<a name="nodejs-backend-architecture-typescript"></a>
### #&#8288;318 [nodejs-backend-architecture-typescript](https://github.com/afteracademy/nodejs-backend-architecture-typescript) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: known (33) · Freshness: recent (56) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · Apache-2.0 · Jul 2026</sub>

**Express, TypeScript and MongoDB blog API with JWT auth and Redis caching.**

A reference backend for a Medium-style blogging platform, built on Express, TypeScript, Mongoose/MongoDB and Redis. It includes API-key and JWT access/refresh token auth, role-based permissions (learner, writer, editor), zod validation, and centralised error and response handlers. Unit and integration tests run under Jest, and Docker Compose starts the app, MongoDB and Redis.

- **+** Clear layered structure: router, handler, response and error handlers, with feature-grouped files
- **+** Unit tests run with mocks and need no database server
- **+** Docker Compose starts app, MongoDB and Redis with one command
- **+** Postman API docs and video walkthroughs are linked
- **−** Fixed blog domain; reuse as a generic backend means removing blog code
- **−** MongoDB only, through Mongoose; no SQL option
- **−** Last tagged release is from January 2024
- **−** No built-in billing, file storage or admin UI

<sub>no GPU · Docker + Compose · Needs MongoDB, Redis, Docker Compose · port 3000 · [Repo](https://github.com/afteracademy/nodejs-backend-architecture-typescript) · [📖 Docs ↗](https://documenter.getpostman.com/view/1552895/2s8Z6u4a6N) · [🌐 Site ↗](https://afteracademy.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nodejs-backend-architecture-typescript/)</sub>

<a name="1backend"></a>
### #&#8288;319 [1backend](https://github.com/1backend/1backend) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: niche (27) · Freshness: recent (58) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · May 2026</sub>

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

<a name="vectorchord"></a>
### #&#8288;320 [vectorchord](https://github.com/supervc-stack/vectorchord) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: niche (21) · Freshness: recent (61) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · custom license · Apr 2026</sub>

**PostgreSQL extension for vector search with RaBitQ compression.**

VectorChord (vchord) is a Rust-based PostgreSQL extension that adds a vchordrq index and 4-bit and 8-bit RaBitQ vector types, using RaBitQ compression with reranking. It reuses pgvector's data types and syntax, so existing pgvector schemas and queries migrate with little change. The README claims 100M 768-dimensional vectors on one AWS i4i.xlarge and index builds of 100M vectors in 20 minutes.

- **+** Compatible with pgvector types and syntax, so migration is mostly CREATE EXTENSION and a new index
- **+** Native RaBitQ4 and RaBitQ8 types; README says RaBitQ8 loses under 1% recall
- **+** Hierarchical K-means build: 100M vectors indexed in 20 minutes, per the README
- **+** Supports multi-vector retrieval, prefiltering, and external index precomputation
- **−** Depends on pgvector being installed; CASCADE pulls it in
- **−** Dual AGPLv3 or Elastic License v2; neither is a permissive license
- **−** Postgres only; cannot be used as a standalone vector database
- **−** Cost and scale figures are the vendor's own benchmarks on AWS instances

<sub>no GPU · Needs PostgreSQL, pgvector · [Repo](https://github.com/supervc-stack/vectorchord) · [📖 Docs ↗](https://docs.vectorchord.ai/vectorchord/) · [🌐 Site ↗](https://vectorchord.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vectorchord/)</sub>

<a name="framework"></a>
### #&#8288;321 [top-think/framework](https://github.com/top-think/framework) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: known (31) · Freshness: recent (50) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · custom license · Mar 2026</sub>

**PHP 8 web application framework with ORM and PSR support.**

ThinkPHP 8 is a general-purpose PHP web framework requiring PHP 8.0+ and think-orm 3.0+. It follows PSR-2 and PSR-4, installs through Composer, and ships a built-in dev server started with `php think run` on port 8000. It is not an AI project; the README only links to a hosted ThinkChat assistant trained on its manual.

- **+** Installs with one Composer command and runs a built-in dev server
- **+** Follows PSR-2 and PSR-4; PSR dependencies upgraded in v8
- **+** README states 6.0 and 6.1 projects upgrade without code changes
- **+** think-dumper adds remote debugging support
- **−** No AI features in the framework itself
- **−** README and primary docs are in Chinese
- **−** Requires PHP 8.0+, so older PHP 7 apps need migration
- **−** Not a hosted backend: no built-in auth service or storage described

<sub>no GPU · Needs PHP 8.0+, Composer, think-orm 3.0+ · port 8000 · [Repo](https://github.com/top-think/framework) · [📖 Docs ↗](https://doc.thinkphp.cn) · [🌐 Site ↗](https://www.thinkphp.cn) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/framework/)</sub>

<a name="kubefirst"></a>
### #&#8288;322 [kubefirst](https://github.com/konstructio/kubefirst) <sub>score [25](../README.md#-how-we-rank "Score 25/100. Adoption: niche (24) · Freshness: slowing (44) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Feb 2026</sub>

**CLI that provisions Kubernetes clusters with a GitOps stack on cloud or local.**

Kubefirst is a Go CLI that creates a Kubernetes cluster with a GitOps platform on it, using cloud-native tools wired together from scratch. It has per-target install guides for Akamai, AWS, Azure, Civo, DigitalOcean, Google Cloud, Vultr, K3s and local k3d. The commercial Kubefirst Pro management UI is installed onto the new platform by default.

- **+** Nine install targets, from AWS and Azure to local k3d
- **+** Single CLI creates the cluster and GitOps platform together
- **+** MIT licensed, with a release in January 2026
- **−** Commercial Kubefirst Pro UI is installed onto the platform by default
- **−** README lacks prerequisites and commands; they live only in external docs
- **−** Not AI-specific; it provisions infrastructure only
- **−** README does not name the tools in the generated stack

<sub>Needs Akamai, AWS, Azure, Civo, DigitalOcean, Google Cloud, Vultr, K3s, k3d · [Repo](https://github.com/konstructio/kubefirst) · [📖 Docs ↗](https://kubefirst-pro.konstruct.io/docs/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kubefirst/)</sub>

<a name="go-backend-clean-architecture"></a>
### #&#8288;323 [go-backend-clean-architecture](https://github.com/amitshekhariitbhu/go-backend-clean-architecture) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: popular (54) · Freshness: quiet (27) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Feb 2026</sub>

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

<a name="ponzu"></a>
### #&#8288;324 [ponzu](https://github.com/ponzu-cms/ponzu) <sub>score [15](../README.md#-how-we-rank "Score 15/100. Adoption: popular (52) · Freshness: quiet (0) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · BSD-3-Clause · Nov 2025</sub>

**Go CMS and JSON API server with generated content editors.**

Ponzu is a Go HTTP server framework and CMS. A CLI generates content types and admin editor views from field definitions, and it serves a JSON API and admin dashboard from a single binary with embedded BoltDB. It is not an AI project, and the README marks it as abandoned, with the last release in 2019.

- **+** Single binary plus assets with embedded BoltDB, no external database
- **+** CLI generates content structs and editor views via `ponzu gen content`
- **+** Automatic HTTPS via Let's Encrypt, self-signed certificates in development
- **+** HTTP/2 with Server Push; admin and API can run together or separately
- **−** README states the project is abandoned; last release was 2019-09-30
- **−** No AI features; it does not fit an AI-focused list
- **−** Admin and API cannot share one BoltDB across processes without a database copy
- **−** Install relies on GOPATH and `go get`, with Go 1.8+ as the stated requirement

<sub>no GPU · Docker · Needs Go 1.8+, git · port 8080 · [Repo](https://github.com/ponzu-cms/ponzu) · [📖 Docs ↗](https://docs.ponzu-cms.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ponzu/)</sub>

<a name="userbase"></a>
### #&#8288;325 [userbase](https://github.com/smallbets/userbase) <sub>score [15](../README.md#-how-we-rank "Score 15/100. Adoption: niche (27) · Freshness: quiet (23) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Jan 2026</sub>

**Browser SDK for user accounts and encrypted data storage without a backend.**

Userbase is a JavaScript SDK that handles sign-up, login and per-user data persistence directly from a static site. Data is encrypted in the browser with user-controlled keys and queried client-side. The server creates its own AWS resources and can be self-hosted, or the maintainers run it as a paid service.

- **+** Auth and database through one browser SDK, no backend code required
- **+** Database operations are end-to-end encrypted in the browser with user-controlled keys
- **+** MIT licensed; self-host or use the hosted service
- **+** Cypress test suite included in the repo
- **−** Self-hosting requires an AWS account and credentials
- **−** No Docker or compose setup provided
- **−** No AI features; not related to LLM tooling
- **−** Queries run client-side, which limits server-side processing

<sub>no GPU · Needs AWS account, Node.js, npm · port 3000 · [Repo](https://github.com/smallbets/userbase) · [📖 Docs ↗](https://userbase.com/docs/) · [🌐 Site ↗](https://userbase.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/userbase/)</sub>

<a name="merchant"></a>
### #&#8288;326 [merchant](https://github.com/ygwyg/merchant) <sub>score [6](../README.md#-how-we-rank "Score 6/100. Adoption: niche (1) · Freshness: quiet (18) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 376 · MIT · Jan 2026</sub>

**Commerce API for products, inventory, checkout and orders on Cloudflare.**

Merchant is a Hono-based commerce backend for Cloudflare Workers. It keeps data in a SQLite-backed Durable Object and images in R2, and exposes REST endpoints for products, inventory, carts, customers and orders. Payments go through Stripe Checkout with Stripe Tax. It also implements the Universal Commerce Protocol for AI agent checkout, OAuth 2.0 with PKCE, signed webhooks and a WebSocket event feed.

- **+** Durable Objects and R2 are auto-provisioned on first wrangler deploy
- **+** UCP endpoints let AI agents create and complete checkout sessions
- **+** Includes an admin dashboard and a vanilla JS example storefront
- **+** HMAC-SHA256 signed outbound webhooks and WebSocket events for carts, orders, inventory
- **−** Tied to Cloudflare and Stripe; Postgres schema exists but moving is manual
- **−** One Durable Object handles everything; sharding is only suggested for scale
- **−** Stripe Checkout is redirect-based, with no embedded payment flow
- **−** No tagged releases; D1 migration does not re-import orders or API keys

<sub>no GPU · Needs Cloudflare Workers, Durable Objects, R2, Stripe · port 8787 · [Repo](https://github.com/ygwyg/merchant) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/merchant/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
