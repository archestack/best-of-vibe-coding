# 🗄️ Backends, databases and hosting reviews · Best of Vibe Coding

Open-source backends you ship apps on (auth, database, storage, APIs) and self-hosted platforms that deploy them from Git or Docker. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-databases-and-hosting).

<sub>🌐 Also on the web: [Backends, databases and hosting on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="bun"></a>
### 🥇 [bun](https://github.com/oven-sh/bun) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 97k · custom license · Nov 2026</sub>

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
### #&#8288;4 [appwrite](https://github.com/appwrite/appwrite) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · BSD-3-Clause · Nov 2026</sub>

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

<a name="tidb"></a>
### #&#8288;5 [tidb](https://github.com/pingcap/tidb) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · Apache-2.0 · Nov 2026</sub>

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

<a name="medusa"></a>
### #&#8288;6 [medusa](https://github.com/medusajs/medusa) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · custom license · Nov 2026</sub>

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

<a name="compose"></a>
### #&#8288;7 [compose](https://github.com/docker/compose) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · Apache-2.0 · Nov 2026</sub>

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
### #&#8288;8 [nacos](https://github.com/alibaba/nacos) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Nov 2026</sub>

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

<a name="kestra"></a>
### #&#8288;9 [kestra](https://github.com/kestra-io/kestra) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · Apache-2.0 · Nov 2026</sub>

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

<a name="rails"></a>
### #&#8288;10 [rails](https://github.com/rails/rails) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Nov 2026</sub>

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
### #&#8288;11 [directus](https://github.com/directus/directus) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · custom license · Nov 2026</sub>

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

<a name="supabase"></a>
### #&#8288;12 [supabase](https://github.com/supabase/supabase) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 115k · Apache-2.0 · Nov 2026</sub>

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

<a name="novu"></a>
### #&#8288;13 [novu](https://github.com/novuhq/novu) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · custom license · Nov 2026</sub>

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
### #&#8288;14 [dokploy](https://github.com/dokploy/dokploy) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · custom license · Nov 2026</sub>

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

<a name="turborepo"></a>
### #&#8288;15 [turborepo](https://github.com/vercel/turborepo) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Nov 2026</sub>

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

<a name="spacetimedb"></a>
### #&#8288;16 [spacetimedb](https://github.com/clockworklabs/spacetimedb) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · custom license · Nov 2026</sub>

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
### #&#8288;17 [nocobase](https://github.com/nocobase/nocobase) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · custom license · Nov 2026</sub>

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

<a name="payload"></a>
### #&#8288;18 [payload](https://github.com/payloadcms/payload) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

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

<a name="saleor"></a>
### #&#8288;19 [saleor](https://github.com/saleor/saleor) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · BSD-3-Clause · Nov 2026</sub>

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

<a name="nocodb"></a>
### #&#8288;20 [nocodb](https://github.com/nocodb/nocodb) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 65k · custom license · Nov 2026</sub>

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

<a name="graphql-engine"></a>
### #&#8288;21 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Nov 2026</sub>

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
### #&#8288;22 [pulumi](https://github.com/pulumi/pulumi) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

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

<a name="coder"></a>
### #&#8288;23 [coder](https://github.com/coder/coder) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · AGPL-3.0 · Nov 2026</sub>

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
### #&#8288;24 [dokku](https://github.com/dokku/dokku) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Nov 2026</sub>

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

<a name="dapr"></a>
### #&#8288;25 [dapr](https://github.com/dapr/dapr) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Nov 2026</sub>

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

<a name="falkordb"></a>
### #&#8288;26 [falkordb](https://github.com/falkordb/falkordb) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · custom license · Nov 2026</sub>

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

<a name="erupt"></a>
### #&#8288;27 [erupt](https://github.com/erupts/erupt) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · Apache-2.0 · Nov 2026</sub>

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
### #&#8288;28 [parse-server](https://github.com/parse-community/parse-server) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

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

<a name="nhost"></a>
### #&#8288;29 [nhost](https://github.com/nhost/nhost) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (50) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · MIT · Nov 2026</sub>

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

<a name="graphjin"></a>
### #&#8288;30 [graphjin](https://github.com/dosco/graphjin) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Nov 2026</sub>

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

<a name="trailbase"></a>
### #&#8288;31 [trailbase](https://github.com/trailbaseio/trailbase) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · OSL-3.0 · Nov 2026</sub>

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

<a name="kong"></a>
### #&#8288;32 [kong](https://github.com/kong/kong) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Oct 2026</sub>

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

<a name="teable"></a>
### #&#8288;33 [teable](https://github.com/teableio/teable) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

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

<a name="insforge"></a>
### #&#8288;34 [insforge](https://github.com/insforge/insforge) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

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
### #&#8288;35 [encore](https://github.com/encoredev/encore) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MPL-2.0 · Nov 2026</sub>

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
### #&#8288;36 [pixeltable](https://github.com/pixeltable/pixeltable) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="apijson"></a>
### #&#8288;37 [apijson](https://github.com/apijson/apijson) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Nov 2026</sub>

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

<a name="convex-backend"></a>
### #&#8288;38 [convex-backend](https://github.com/convex/convex-backend) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · custom license · Nov 2026</sub>

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

<a name="zenstack"></a>
### #&#8288;39 [zenstack](https://github.com/zenstackhq/zenstack) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Nov 2026</sub>

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

<a name="omnigraph"></a>
### #&#8288;40 [omnigraph](https://github.com/modernrelay/omnigraph) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Nov 2026</sub>

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

<a name="prest"></a>
### #&#8288;41 [prest](https://github.com/prest/prest) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

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

<a name="memgraph"></a>
### #&#8288;42 [memgraph](https://github.com/memgraph/memgraph) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · custom license · Nov 2026</sub>

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

<a name="ihp"></a>
### #&#8288;43 [ihp](https://github.com/digitallyinduced/ihp) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (41) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Nov 2026</sub>

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

<a name="airbyte"></a>
### #&#8288;44 [airbyte](https://github.com/airbytehq/airbyte) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (66) · Freshness: active (82) · Maintenance: patchy (44) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · custom license · Nov 2026</sub>

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

<a name="nitric"></a>
### #&#8288;45 [nitric](https://github.com/nitrictech/nitric) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;46 [serverpod](https://github.com/serverpod/serverpod) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · BSD-3-Clause · Nov 2026</sub>

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
### #&#8288;47 [fusio](https://github.com/apioo/fusio) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;48 [butterbase](https://github.com/butterbase-ai/butterbase) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

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

<a name="classic-jazz"></a>
### #&#8288;49 [classic-jazz](https://github.com/garden-co/classic-jazz) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

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
### #&#8288;50 [matecloud](https://github.com/mateaix/matecloud) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;51 [steedos-platform](https://github.com/steedos/steedos-platform) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (8) · Freshness: active (92) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · AGPL-3.0 · Nov 2026</sub>

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
### #&#8288;52 [amplication](https://github.com/amplication/amplication) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: popular (59) · Freshness: recent (63) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · custom license · Apr 2026</sub>

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

<a name="1backend"></a>
### #&#8288;53 [1backend](https://github.com/1backend/1backend) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (19) · Freshness: recent (62) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · May 2026</sub>

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
### #&#8288;54 [go-backend-clean-architecture](https://github.com/amitshekhariitbhu/go-backend-clean-architecture) <sub>score [23](../README.md#-how-we-rank "Score 23/100. Adoption: known (44) · Freshness: slowing (31) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Feb 2026</sub>

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
