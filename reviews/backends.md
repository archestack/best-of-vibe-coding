# 🗄️ Backends and databases reviews · Best of Vibe Coding

Open-source backends you ship apps on: auth, database, storage and APIs in one, self-hosted or managed. Back to the [leaderboard](../README.md#%EF%B8%8F-backends-and-databases).

<sub>🌐 Also on the web: [Backends and databases on archestack.com](https://archestack.com/best-of-vibe-coding/backends/), each project on its own page.</sub>

<a name="supabase"></a>
### 🥇 [supabase](https://github.com/supabase/supabase) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (72) · Easy to run: some setup (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 112k · Apache-2.0 · Oct 2026</sub>

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
### 🥈 [parse-server](https://github.com/parse-community/parse-server) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (78) · Easy to run: easy (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

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
### 🥉 [graphql-engine](https://github.com/hasura/graphql-engine) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (81) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · Apache-2.0 · Oct 2026</sub>

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

<a name="apijson"></a>
### #&#8288;4 [apijson](https://github.com/apijson/apijson) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (90) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · custom license · Oct 2026</sub>

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
