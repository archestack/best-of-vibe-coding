# ☁️ Backend and cloud templates reviews · Best of Vibe Coding

Backend service templates (FastAPI, Express, Hono) that expose models or agents over an API, and vendor reference apps for Azure or Google Cloud. Back to the [leaderboard](../README.md#%EF%B8%8F-backend-and-cloud-templates).

<sub>🌐 Also on the web: [Backend and cloud templates on archestack.com](https://archestack.com/best-of-vibe-coding/cloud-reference/), each project on its own page.</sub>

<a name="fastapi"></a>
### 🥇 [fastapi](https://github.com/fastapi/fastapi) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 105k · MIT · Nov 2026</sub>

**Python web framework for typed REST APIs with automatic OpenAPI docs.**

FastAPI is a Python framework for building HTTP APIs from standard type hints. It uses Starlette for the web layer and Pydantic for validation and serialization, and generates OpenAPI and JSON Schema documentation with Swagger UI at /docs and ReDoc at /redoc. It is a general-purpose framework, not an AI-specific starter.

- **+** Validates path, query, header, cookie, form and JSON body data from type hints alone
- **+** Generates OpenAPI schema plus Swagger UI and ReDoc pages with no extra setup
- **+** Includes dependency injection, OAuth2/JWT, HTTP Basic auth, WebSockets and CORS
- **+** `fastapi dev` gives auto-reload; `fastapi run` is the production command
- **−** No model, agent or other AI functionality included; you wire that in yourself
- **−** No ORM or database layer; persistence is left to other libraries
- **−** Relies on Starlette and Pydantic, so changes in either affect your app
- **−** Productivity figures come from an internal team's estimates, not reproducible benchmarks

<sub>Python · Needs Starlette, Pydantic, Uvicorn · [Repo](https://github.com/fastapi/fastapi) · [📖 Docs ↗](https://fastapi.tiangolo.com/tutorial/) · [🌐 Site ↗](https://fastapi.tiangolo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastapi/)</sub>

<a name="fiber"></a>
### 🥈 [fiber](https://github.com/gofiber/fiber) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Nov 2026</sub>

**Express-style HTTP web framework for Go, built on fasthttp.**

Fiber is a Go web framework with an Express-like API for routing, middleware and handlers, running on top of fasthttp. It ships middleware for static files, logging, CORS and rate limiting, plus WebSocket, Socket.io and Server-Sent Events support, and can adapt net/http handlers. It is a general backend framework, not an AI project.

- **+** Express-like routing, groups and middleware chain, familiar to Node.js developers
- **+** Built-in middleware for static files, logger, CORS, rate limiter, plus WebSocket and SSE
- **+** Runs net/http handlers directly and has an adaptor middleware for net/http middleware
- **+** Zero-allocation design on fasthttp, with TechEmpower benchmark results published
- **−** fiber.Ctx values are reused across requests, so keeping references after the handler returns is unsafe
- **−** Uses unsafe, so it may lag behind the newest Go releases
- **−** Requires Go 1.26 or higher for v3
- **−** Adapted net/http handlers lose fiber.Ctx features and add compatibility overhead

<sub>Go · Needs Go 1.26+, fasthttp · [Repo](https://github.com/gofiber/fiber) · [📖 Docs ↗](https://docs.gofiber.io) · [🌐 Site ↗](https://gofiber.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fiber/)</sub>

<a name="serverless"></a>
### 🥉 [serverless](https://github.com/serverless/serverless) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · custom license · Nov 2026</sub>

**CLI that deploys AWS Lambda code and infrastructure from serverless.yml.**

The Serverless Framework is a Node.js CLI that reads a serverless.yml file and deploys functions, event triggers and supporting AWS resources such as DynamoDB, S3 and API Gateway. V.4 adds web apps on Lambda, MCP server hosting, Bedrock AgentCore definitions, a Dev Mode that runs local code against deployed traffic, and bundled agent skills. The repository root is under a proprietary license, with the MIT code in packages/serverless.

- **+** Declares Lambda functions, events and DynamoDB/S3/API Gateway resources in one serverless.yml
- **+** Dev Mode routes real stage traffic to local code without redeploying
- **+** Supports Node.js, Python, Java, Go, .NET, Ruby and other Lambda runtimes
- **+** Over 1,000 plugins; several popular ones now built in, such as custom domains
- **−** V.4 requires login to Serverless Dashboard; CLI free only for small orgs
- **−** Non-AWS providers deprecated in V.4; focus is AWS only
- **−** Mixed licensing: proprietary root license, MIT only in packages/serverless
- **−** Self-updates automatically every 24 hours by default

<sub>JavaScript, Amazon Bedrock · Needs Node.js 18.17.0+, AWS account, Serverless Dashboard login · [Repo](https://github.com/serverless/serverless) · [📖 Docs ↗](https://serverless.com/framework/docs/) · [🌐 Site ↗](https://serverless.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless/)</sub>

<a name="generator-jhipster"></a>
### #&#8288;4 [generator-jhipster](https://github.com/jhipster/generator-jhipster) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

**Code generator for Java apps with Angular, React or Vue frontends.**

JHipster is a Node.js generator (npm package generator-jhipster) that scaffolds Java application projects with an Angular, React or Vue frontend, built with Maven or Gradle. Its CI matrix covers monolith and microservice layouts, SQL and NoSQL databases, and JWT or OAuth 2.0 authentication. It is a conventional scaffolding tool, and the README describes no AI features.

- **+** Angular, React and Vue variants are each built in CI with Maven and Gradle
- **+** Covers monolith and microservice setups with JWT or OAuth 2.0 auth
- **+** CI also tests Elasticsearch, no-database and Windows variants
- **+** Blueprints let teams extend the generator; Apache-2.0 licensed
- **−** No AI or LLM functionality described in the README
- **−** Only Java 21/25 with Node 22/24 is verified in CI
- **−** Running it on a foreign project executes blueprints declared in .yo-rc.json
- **−** README is mostly badges; usage and features live on the external website

<sub>TypeScript · Needs Node.js 22/24, Java 21/25 · Docker · [Repo](https://github.com/jhipster/generator-jhipster) · [📖 Docs ↗](https://www.jhipster.tech/) · [🌐 Site ↗](https://www.jhipster.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/generator-jhipster/)</sub>

<a name="echo"></a>
### #&#8288;5 [echo](https://github.com/labstack/echo) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

**Minimalist Go web framework with a radix-tree router and middleware.**

Echo is a Go web framework built on net/http. It adds a radix-tree router, route groups, request binding for JSON, XML, form, query and path data, and centralized error handling. It ships middleware such as a log/slog request logger and panic recovery, and supports TLS, HTTP/2, autocert and graceful shutdown. It has no AI-specific features; the README lists NVIDIA's LLM API gateway among its users.

- **+** Built on net/http; interoperates via echo.WrapHandler and echo.WrapMiddleware
- **+** Middleware at root, group or route level, with a single HTTPErrorHandler
- **+** Binding for JSON, XML, form, query and path parameters with pluggable validation
- **+** v5 released 2026-01-18; v4 gets security fixes until 2027-12-31
- **−** No AI, model or agent features; it is a generic HTTP framework
- **−** v5 changes the API from v4; upgrading requires following API_CHANGES_V5.md
- **−** API key/JWT auth, tenant isolation and admin console are in paid Echo Pro
- **−** Library only; no starter app or project scaffold included

<sub>Go · Needs Go · [Repo](https://github.com/labstack/echo) · [📖 Docs ↗](https://echo.labstack.com/guide/quickstart/) · [🌐 Site ↗](https://echo.labstack.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/echo/)</sub>

<a name="goa"></a>
### #&#8288;6 [goa](https://github.com/goadesign/goa) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Nov 2026</sub>

**Design-first Go framework that generates HTTP, gRPC and JSON-RPC services.**

Goa takes a service contract written in a Go DSL and generates server and client code, request validation, CLI clients, OpenAPI specs and protobuf definitions for HTTP, gRPC and JSON-RPC. You implement the generated service interface in plain Go. The repo also ships a coding-agent skill, and a companion project, Goa-AI, covers agents and MCP servers.

- **+** One design generates HTTP, gRPC and JSON-RPC transports plus Go clients and a CLI
- **+** Emits OpenAPI and Protocol Buffer definitions from the same contract
- **+** Supports streaming over WebSocket, SSE and gRPC streams
- **+** Generated interfaces let the Go compiler flag code needing updates after a design change
- **−** Requires Go 1.27.3 or later as of v3.35.0
- **−** gRPC output needs protoc and Go protobuf generators installed
- **−** Upgrading from v3.30.x involves intentional source and transport changes
- **−** Go only; the contract is written in a Go DSL

<sub>Go · Needs Go 1.27.3+, protoc (for gRPC and JSON-RPC example) · [Repo](https://github.com/goadesign/goa) · [📖 Docs ↗](https://goa.design/docs/1-goa/) · [🌐 Site ↗](https://goa.design) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goa/)</sub>

<a name="full-stack-fastapi-template"></a>
### #&#8288;7 [full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

**FastAPI and React starter with JWT auth, PostgreSQL and a generated API client.**

A GitHub template for a full-stack web app: a FastAPI backend using SQLModel and PostgreSQL, and a React/TypeScript frontend built with Vite, Tailwind CSS and shadcn/ui. The frontend is built into the backend and served on the same domain as the API. It includes JWT login, email password recovery, and Docker Compose with Traefik for self-hosting. It has no AI features built in.

- **+** Auto-generated frontend client for the FastAPI API
- **+** Pytest backend tests and Playwright end-to-end tests, with GitHub Actions CI/CD
- **+** Docker Compose with Traefik gives automatic HTTPS for self-hosting
- **+** Mailpit for local email testing and React Email templates
- **−** No AI or model integration; it is a generic app scaffold
- **−** No billing or payments wired in
- **−** Authentication is JWT with email recovery only; no OAuth or social login listed
- **−** PostgreSQL only; other databases are not mentioned

<sub>TypeScript · Needs PostgreSQL, Docker Compose, Traefik, Mailpit · GitHub template · ⚠️ .env file committed · [Repo](https://github.com/fastapi/full-stack-fastapi-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/full-stack-fastapi-template/)</sub>

<a name="hono"></a>
### #&#8288;8 [hono](https://github.com/honojs/hono) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**TypeScript web framework for Workers, Deno, Bun and Node.js.**

Hono is a web framework built on Web Standard APIs, with no dependencies. The same app code runs on Cloudflare Workers, Fastly Compute, Deno, Bun, Vercel, AWS Lambda, Lambda@Edge and Node.js. It ships a RegExpRouter, built-in middleware and TypeScript types, and the hono/tiny preset is under 12kB. It is a general backend framework, not an AI-specific project.

- **+** Same code runs on Workers, Fastly, Deno, Bun, Lambda and Node.js
- **+** Zero dependencies; hono/tiny preset is under 12kB
- **+** Built-in, custom and third-party middleware available
- **+** First-class TypeScript support; scaffold with npm create hono@latest
- **−** No AI, model or agent features; it is a general web framework
- **−** Not a ready-made template; you write routes and handlers yourself
- **−** Speed claims in the README have no benchmark figures

<sub>TypeScript · [Repo](https://github.com/honojs/hono) · [📖 Docs ↗](https://hono.dev) · [🌐 Site ↗](https://hono.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hono/)</sub>

<a name="chi"></a>
### #&#8288;9 [chi](https://github.com/go-chi/chi) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

**Composable HTTP router for Go REST services, built on net/http.**

chi is a Go router built on a Patricia radix trie, with a core under 1000 LOC and no dependencies beyond the standard library. It supports named and regexp URL params, route groups, sub-router mounting and inline middleware, all as plain net/http handlers. It also ships a middleware package (logger, recoverer, timeout, throttle, compress, client IP extraction) and a docgen tool for routing docs.

- **+** Standard net/http handlers and middleware, so any compatible package works unchanged
- **+** No external dependencies; core router is under 1000 lines
- **+** Route groups, Mount and inline With() keep large REST APIs modular
- **+** Bundled middleware covers request IDs, timeouts, throttling, compression and client IP
- **−** Routing only: no ORM, validation or auth; render and docgen are separate packages
- **−** Request-scoped values use context.WithValue with untyped keys and type assertions
- **−** Legacy RealIP middleware is deprecated for spoofing; you must pick a ClientIPFrom* variant
- **−** Not an AI project: no model or agent integration, so it is only a generic backend base

<sub>Go · [Repo](https://github.com/go-chi/chi) · [📖 Docs ↗](https://pkg.go.dev/github.com/go-chi/chi/v5) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chi/)</sub>

<a name="gofr"></a>
### #&#8288;10 [gofr](https://github.com/gofr-dev/gofr) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

**Go microservice framework with built-in observability, gRPC, Pub/Sub and LLM hooks.**

GoFr is a Go framework for building HTTP and gRPC microservices, with logs, traces and metrics, auth middleware, migrations, cron jobs and datasource health checks included. It targets Kubernetes deployment. It can register an OpenAI-compatible LLM with app.AddLLM and expose read-only handlers as MCP tools with app.EnableMCP.

- **+** Tracing, metrics and logs are built in, with health checks for all datasources
- **+** Covers REST, gRPC, WebSockets, Pub/Sub, cron and database migrations in one framework
- **+** app.AddLLM works with OpenAI, Groq, DeepSeek, Together, Ollama or any BaseURL endpoint
- **+** app.EnableMCP exposes only read-only handlers as MCP tools; write handlers are never exposed
- **−** Requires Go 1.26 or newer
- **−** Opinionated structure; you adopt its Context, config and handler conventions
- **−** AI features are add-ons to a general framework, not an agent runtime
- **−** MCP server only exposes GET, HEAD, OPTIONS and QUERY handlers

<sub>Go, OpenAI, Groq, DeepSeek, Together · Needs Go 1.26+ · Docker · [Repo](https://github.com/gofr-dev/gofr) · [📖 Docs ↗](https://gofr.dev/docs) · [🌐 Site ↗](https://gofr.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gofr/)</sub>

<a name="elysia"></a>
### #&#8288;11 [elysia](https://github.com/elysiajs/elysia) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

**TypeScript web framework for Bun with end-to-end type safety.**

Elysia is a TypeScript HTTP server framework built for the Bun runtime. It focuses on end-to-end type safety, so types flow from server routes to the client. It is a general web framework, not an AI-specific project, and the README gives no AI features, install steps beyond `bun create elysia app`, or specs.

- **+** End-to-end type safety between server and client, as described in the README
- **+** Scaffold with `bun create elysia app`
- **+** MIT licensed with a release on 2026-11-05, so actively maintained
- **+** Documentation site and Discord community available
- **−** Not an AI project: no model, agent or LLM integration in the README
- **−** Built around Bun; Node.js support not described in the README
- **−** README is minimal, with no API examples or benchmarks inline
- **−** No Docker or compose files in the repository

<sub>TypeScript · Needs Bun · [Repo](https://github.com/elysiajs/elysia) · [📖 Docs ↗](https://elysiajs.com) · [🌐 Site ↗](https://elysiajs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/elysia/)</sub>

<a name="full-stack-ai-agent-template"></a>
### #&#8288;12 [full-stack-ai-agent-template](https://github.com/vstorm-co/full-stack-ai-agent-template) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Project generator for FastAPI and Next.js apps with agents and RAG.**

CLI (pip install fastapi-fullstack) scaffolding a FastAPI backend and Next.js frontend via a wizard or presets, with Pydantic AI, Pydantic Deep Agents, LangChain, LangGraph or DeepAgents, RAG on Milvus, Qdrant, pgvector or Chroma, WebSocket chat, JWT, OAuth, admin, teams, Stripe billing, Celery, Docker and K8s. make bootstrap starts Postgres, migrations and a seeded admin; projects can pull template upgrades later.

- **+** Wizard and presets pick framework, vector store, auth and billing per project
- **+** Template upgrades merge into generated projects on a branch
- **+** Chat UI renders tool calls, plans, subagents, charts and Python execution
- **+** 100% coverage badge and CI on the generator
- **−** Generator, not a repo to fork; output size depends on options chosen
- **−** Seeds admin@example.com with a fixed password; rotate before exposing
- **−** Optional services (Milvus, Redis, Celery) raise the local footprint
- **−** Windows needs GNU Make or WSL2

<sub>Python, Pydantic AI, Pydantic Deep Agents, LangChain, LangGraph · Needs PostgreSQL, Redis (optional), Milvus, Qdrant, pgvector or ChromaDB (RAG), Stripe (billing), LLM provider API key · [Repo](https://github.com/vstorm-co/full-stack-ai-agent-template) · [📖 Docs ↗](https://vstorm-co.github.io/full-stack-ai-agent-template/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/full-stack-ai-agent-template/)</sub>

<a name="go-zero"></a>
### #&#8288;13 [go-zero](https://github.com/zeromicro/go-zero) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

**Go web and RPC microservice framework with goctl code generation.**

go-zero is a Go framework for HTTP and RPC services. Its goctl tool generates server code from .api or .proto files, and client code for Java, Dart, TypeScript, Kotlin and others. It ships built-in timeout control, rate limiting, adaptive circuit breaking and load shedding. It is not an AI project; the README only links optional guidance repos for AI coding assistants.

- **+** goctl generates Go server code and multi-language clients from one .api file
- **+** Adaptive circuit breaker, load shedding and rate limiting built in, no configuration needed
- **+** Request parameters validated automatically from struct tags in the .api file
- **+** API layer is compatible with net/http; MIT license
- **−** Not AI-specific; AI tooling lives in separate ai-context, zero-skills and mcp-zero repos
- **−** Services are Go only; other languages get generated clients, not servers
- **−** Opinionated project layout and .api DSL to learn before writing handlers
- **−** Benchmark results are given only as an image, no numbers in the README

<sub>Go · Needs Go, goctl · [Repo](https://github.com/zeromicro/go-zero) · [📖 Docs ↗](https://go-zero.dev/) · [🌐 Site ↗](https://go-zero.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-zero/)</sub>

<a name="agent-service-toolkit"></a>
### #&#8288;14 [agent-service-toolkit](https://github.com/joshuac215/agent-service-toolkit) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

**LangGraph agent served by FastAPI with a Streamlit chat front end.**

Python template that wires a LangGraph agent to a FastAPI service with streaming and non-streaming endpoints, a reusable AgentClient, and a Streamlit chat app. It also serves every agent over the AG-UI protocol and includes a ChromaDB RAG agent, chat history via /threads, and LangSmith feedback. Fork it and add agents under src/agents.

- **+** Full path from agent to API, client and UI in one repo
- **+** Multiple agents routed by URL path, listed at /info
- **+** Token and message streaming, plus AG-UI endpoint for CopilotKit-style frontends
- **+** Unit and integration tests, plus smoke tests for Postgres, MongoDB and AG-UI
- **−** Tied to LangGraph; no other agent framework supported
- **−** Streamlit UI must be edited by hand to match new agents
- **−** Content moderation requires a Groq API key
- **−** Solo maintainer, issues triaged roughly biweekly; no tagged releases

<sub>Python, OpenAI, Ollama, VertexAI, vLLM · Needs LLM provider API key (e.g. OpenAI), PostgreSQL (in docker compose), ChromaDB (RAG agent), Groq API key (content moderation), LangSmith (optional) · GitHub template · Docker · env example file · [Repo](https://github.com/joshuac215/agent-service-toolkit) · [▶️ Demo ↗](https://agent-service-toolkit.streamlit.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-service-toolkit/)</sub>

<a name="monid"></a>
### #&#8288;15 [monid](https://github.com/monid-ai/monid) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Oct 2026</sub>

**Declarative connector framework behind a metered catalog of agent tool APIs.**

Monid is the connector layer for a hosted service that gives agents one base URL and key for 2,000+ tools across 72+ providers. Each provider and endpoint is a TypeScript definition (defineProvider, defineEndpoint) with zod input schemas, and the engine meters usage per call from the raw response. The repo lets you run connectors locally with your own vendor keys and add new ones by pull request.

- **+** Declarative connectors: no per-provider client or execution path, so coding agents can write them
- **+** Usage model per endpoint: flat, per result, or per unit, settled on the raw response
- **+** Tests replay recorded fixtures, so CI needs no network or vendor keys
- **+** Same compiled artifact runs locally, in CI, and on the hosted platform
- **−** Repo is only the connector layer; the hosted platform and billing are not included
- **−** Discovery, ranking and health data are described for the hosted service, not this repo
- **−** Requires Deno 2.x and your own vendor keys to run real endpoints
- **−** No Docker or compose setup provided

<sub>TypeScript · Needs Deno 2.x, Vendor API keys per provider · [Repo](https://github.com/monid-ai/monid) · [📖 Docs ↗](https://docs.monid.ai) · [🌐 Site ↗](https://monid.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/monid/)</sub>

<a name="azure-agent-landing-zone"></a>
### #&#8288;16 [agent-landing-zone](https://github.com/azure/agent-landing-zone) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

**Azure Bicep landing zone for deploying enterprise agent apps on Microsoft Foundry.**

Infrastructure-as-code template, deployed with Azure Developer CLI, that provisions a Zero-Trust network foundation on Azure for agent applications running on Microsoft Foundry. It can deploy the full stack with a default UI, orchestrator and optional ingestion component, infrastructure only, or a custom app on the same foundation. It is the renamed GPT-RAG project.

- **+** Three deploy paths: full stack, infrastructure only, or your own application
- **+** Zero-Trust network architecture with IaC-first deployment via azd
- **+** Component versions pinned in manifest.json for each release
- **+** Default UI, orchestrator and ingestion live in separate repos, so they can be swapped
- **−** Azure-only; requires Microsoft Foundry and an Azure subscription
- **−** README is a landing page; setup details live on an external docs site
- **−** No Docker or compose setup for local runs
- **−** Sizing, cost and RAM requirements are unknown from the README

<sub>Python, Azure OpenAI · Needs Azure subscription, Microsoft Foundry, Azure OpenAI, Azure AI Search, Azure Developer CLI · GitHub template · [Repo](https://github.com/azure/agent-landing-zone) · [📖 Docs ↗](https://azure.github.io/AI-Landing-Zones/agent-landing-zone/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-agent-landing-zone/)</sub>

<a name="fastapi-langgraph-agent-production-ready-template"></a>
### #&#8288;17 [fastapi-langgraph-agent-production-ready-template](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**FastAPI backend template for LangGraph agents with memory, auth and tracing.**

A Python backend template that wires a stateful LangGraph agent into FastAPI with JWT sessions, slowapi rate limiting, Alembic migrations and PostgreSQL checkpointing. Long-term memory runs in-process through mem0 and pgvector, and LLM calls go through a service with retries and circular model fallback. Observability comes from Langfuse tracing, Prometheus metrics and Grafana dashboards.

- **+** Circular model fallback with tenacity retries and a total timeout budget
- **+** Per-user long-term memory via mem0 and pgvector in your own PostgreSQL
- **+** Langfuse tracing, Prometheus metrics and Grafana dashboards included
- **+** Custom tools are added by registering a LangChain @tool function
- **−** Ships a single agent; supervisor or sub-agent setups must be wired by hand
- **−** mem0 memory needs an OpenAI API key for fact extraction and embeddings
- **−** Requires PostgreSQL with the pgvector extension
- **−** Non-OpenAI providers need extra packages and registry edits

<sub>Python, OpenAI, Anthropic, Ollama, Google GenAI · Needs PostgreSQL, pgvector, Langfuse (optional), Valkey/Redis (optional), Prometheus and Grafana (optional) · Docker · env example file · [Repo](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastapi-langgraph-agent-production-ready-template/)</sub>

<a name="generative-ai-project-template"></a>
### #&#8288;18 [generative-ai-project-template](https://github.com/aminedjeghri/generative-ai-project-template) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 118 · MIT · Nov 2026</sub>

**FastAPI and NiceGUI chat template using Ollama or LiteLLM cloud models.**

A Python template with a FastAPI backend and a NiceGUI chat frontend. Models come from a local Ollama install or cloud providers through LiteLLM, configured with INFERENCE_* and EMBEDDINGS_* variables in .env. It includes a uv workspace, tests, Docker Compose, MkDocs documentation and GitHub release workflows.

- **+** Switches between local Ollama and cloud providers through LiteLLM config
- **+** Make targets cover install, run, test, Docker Compose and docs preview
- **+** Compose stack runs backend, frontend and Ollama, with a CUDA variant
- **+** Pre-commit hooks, Ruff, tests and release workflow are already set up
- **−** Chat only; README lists no RAG, agent or auth features
- **−** Requires Make, Bash and uv; Windows support is not listed
- **−** Full `make check` needs live LLM, Ollama and API services
- **−** Pinned to Python 3.14.8, which may conflict with older dependencies

<sub>Python, Ollama, LiteLLM cloud providers, OpenAI, Hugging Face · Needs uv, Make, Bash, Git, Ollama (local inference), Docker Compose 2.24+ (optional) · GitHub template · Docker · env example file · [Repo](https://github.com/aminedjeghri/generative-ai-project-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/generative-ai-project-template/)</sub>

<a name="fastcrud"></a>
### #&#8288;19 [fastcrud](https://github.com/benavlabs/fastcrud) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Async CRUD methods and auto-generated endpoints for FastAPI and SQLAlchemy 2.0.**

FastCRUD is a Python library that adds async CRUD operations on SQLAlchemy 2.0 models and a crud_router helper that generates FastAPI endpoints from a model and Pydantic schemas. It supports joins with auto-detected conditions, dynamic filtering and sorting, and offset and cursor pagination. It also ships a bundled agent skill that coding tools can load through library-skills.

- **+** crud_router generates endpoints from a model plus create and update schemas
- **+** Offset and cursor pagination built in, with auto-detected join conditions
- **+** Can be used inside hand-written FastAPI routes via FastCRUD(Model)
- **+** Bundled agent skill covers N+1 avoidance and when to use raw SQLAlchemy
- **−** Aggregates, CTEs, GROUP BY projections and bulk writes need raw SQLAlchemy
- **−** Requires Python 3.10+, SQLAlchemy 2.0.21+ and Pydantic 2.4.1+
- **−** Non-native column types such as sqlalchemy-utils may raise NotImplementedError
- **−** Library only: no auth, billing or frontend included

<sub>Python · Needs FastAPI, SQLAlchemy >=2.0.21, Pydantic >=2.4.1, SQLAlchemy-Utils (optional) · [Repo](https://github.com/benavlabs/fastcrud) · [📖 Docs ↗](https://benavlabs.github.io/fastcrud/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastcrud/)</sub>

<a name="node-typescript-boilerplate"></a>
### #&#8288;20 [node-typescript-boilerplate](https://github.com/jsynowiec/node-typescript-boilerplate) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (42) · Freshness: active (100) · Maintenance: patchy (35) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

**Framework-free Node.js TypeScript starter with Vitest, ESLint and CI.**

A minimal repository template for Node.js 24 projects using TypeScript 6 with strict settings and native ESM. It ships Vitest, ESLint with typescript-eslint, Prettier, a GitHub Actions workflow, Mise toolchain config and an AGENTS.md file with guidance for AI coding agents. It deliberately includes no web framework, database, auth or Docker.

- **+** No framework, database or ORM imposed; small dependency surface
- **+** Native ESM with strict TypeScript 6 config targeting ES2024
- **+** Vitest, ESLint, Prettier and GitHub Actions CI preconfigured
- **+** Includes AGENTS.md so coding agents get project rules from the start
- **−** No HTTP server, auth, database or Docker; all of that is left to you
- **−** ESM only; CommonJS projects must convert, and issues about it are not accepted
- **−** Targets Node.js 24 only; older runtimes are not covered
- **−** AGENTS.md is a generic example that needs rewriting per project

<sub>TypeScript · Needs Node.js 24, npm, Mise (recommended) · GitHub template · [Repo](https://github.com/jsynowiec/node-typescript-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/node-typescript-boilerplate/)</sub>

<a name="nunu"></a>
### #&#8288;21 [nunu](https://github.com/go-nunu/nunu) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Aug 2026</sub>

**Go CLI that scaffolds layered Gin and Gorm projects with Wire injection.**

Nunu is a Go CLI that generates a project from a template repo (basic, advanced or monorepo) and creates handler, service, repository and model files per entity. It wires Gin, Gorm, Wire, Viper, Zap and go-redis into a layered layout, and `nunu run` starts the app with hot reload. It is a general backend scaffold; AI support is limited to an MCP server layout and an agent skill.

- **+** `nunu create all user` generates handler, service, repository and model in the right directories
- **+** `nunu run` gives hot reload; `nunu wire` regenerates Wire dependency injection code
- **+** Built on common libraries (Gin, Gorm, Viper, Zap, Casbin, gocron), so little new to learn
- **+** Separate agent skill and MCP server layout exist for coding agents
- **−** No AI or model-serving functionality in the core tool
- **−** Requires Go 1.25.8 or newer
- **−** README says updates will be infrequent
- **−** Templates are pulled from Git repos at creation time, so network access is needed

<sub>Go · Needs Go 1.25.8+, Git, MySQL 5.7+ (optional), Redis (optional), Docker (optional) · [Repo](https://github.com/go-nunu/nunu) · [📖 Docs ↗](https://github.com/go-nunu/nunu/blob/main/docs/en/guide.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nunu/)</sub>

<a name="fullstack-solution-template-for-agentcore"></a>
### #&#8288;22 [fullstack-solution-template-for-agentcore](https://github.com/awslabs/fullstack-solution-template-for-agentcore) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 602 · Apache-2.0 · Nov 2026</sub>

**React and AgentCore starter for deploying a secured agent chat app on AWS.**

Fork-and-deploy starter that ships a React/TypeScript frontend on Amplify Hosting connected to an Amazon Bedrock AgentCore backend. The baseline is a multi-turn chat agent with a Lambda text-analysis tool behind AgentCore Gateway and a Code Interpreter. Cognito handles login, Cedar policies guard the Gateway, and steering docs guide coding assistants.

- **+** Deploys with a few CDK commands; a Terraform alternative is included
- **+** Agent SDK agnostic: Strands and LangGraph single-agent patterns included
- **+** Cognito JWT auth from frontend through Runtime to Gateway, with Cedar policies
- **+** Steering docs and AGENTS.md rules written for AI coding assistants
- **−** Tied to AWS and AgentCore; the backend does not run elsewhere
- **−** README calls it a proof-of-value, not production-ready
- **−** Baseline tools are minimal: text analysis and Code Interpreter only
- **−** Two infra directories (CDK and Terraform); README advises deleting one

<sub>Python, Strands, LangGraph · Needs AWS account, Amazon Bedrock AgentCore, AWS Cognito, AWS Amplify Hosting, AWS Lambda, AWS CDK or Terraform, Node.js · Docker · [Repo](https://github.com/awslabs/fullstack-solution-template-for-agentcore) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fullstack-solution-template-for-agentcore/)</sub>

<a name="serverless-rag-demo"></a>
### #&#8288;23 [serverless-rag-demo](https://github.com/aws-samples/serverless-rag-demo) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT-0 · Oct 2026</sub>

**AWS CDK sample for document RAG chat and multi-agent workflows on Bedrock.**

Deploys a RAG chat app on AWS with one `sh deploy.sh` wizard that runs `cdk deploy --all`. Documents are indexed through a Bedrock Knowledge Base into OpenSearch Serverless NextGen and queried with hybrid BM25 + KNN search. A Strands Graph multi-agent runtime on Bedrock AgentCore routes requests to specialist nodes for code, presentations, web search, weather and retrieval.

- **+** Hybrid BM25 + KNN search with per-user document isolation
- **+** Demo OCU mode scales to zero, so idle cost is listed as $0
- **+** Full infrastructure as Python CDK stacks, with Cognito auth and CloudFront hosting
- **+** MIT-0 license with no attribution requirement
- **−** AWS only: Bedrock, AgentCore, OpenSearch Serverless and Cognito are all required
- **−** Models fixed to Claude Sonnet/Opus 4.6 and Titan Embed V2; no other providers listed
- **−** Supported in six regions only; us-west-1 and ap-southeast-1 excluded
- **−** No release tags, and tests cover CDK unit checks only

<sub>Python, Claude Sonnet 4.6, Claude Opus 4.6, Amazon Titan Embed Text V2 · Needs AWS account, Amazon Bedrock, OpenSearch Serverless NextGen, Bedrock AgentCore, Amazon Cognito, CloudFront, S3, Docker, AWS CDK CLI · Docker · [Repo](https://github.com/aws-samples/serverless-rag-demo) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless-rag-demo/)</sub>

<a name="openai-chat-app-quickstart"></a>
### #&#8288;24 [openai-chat-app-quickstart](https://github.com/azure-samples/openai-chat-app-quickstart) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 254 · MIT · Oct 2026</sub>

**Minimal Quart chat app on Azure OpenAI with managed identity.**

Python Quart backend using the openai package with a plain HTML/JS frontend that streams JSON Lines over a ReadableStream, plus Bicep for Azure OpenAI, Container Apps, Container Registry, Log Analytics and RBAC roles, deployed with azd up. Authenticates to Azure OpenAI with managed identity, so no API key; the local dev server runs on port 50505 after a first azd deploy. For teams starting a chat service on Azure.

- **+** Managed identity auth; no OpenAI key in config
- **+** Bicep provisions the full Container Apps stack
- **+** Codespaces and Dev Container configs included
- **+** IaC security scan GitHub Action included
- **−** Local run depends on a prior Azure deployment for the endpoint
- **−** No user auth; sibling repos add Entra ID
- **−** Frontend is minimal HTML/JS, not a component framework
- **−** Azure Container Registry has a fixed daily cost

<sub>Bicep, Azure OpenAI (openai package) · Needs Azure subscription with Azure OpenAI access, azd CLI · GitHub template · env example file · [Repo](https://github.com/azure-samples/openai-chat-app-quickstart) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/ai/get-started-securing-your-ai-app?tabs=github-codespaces) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chat-app-quickstart/)</sub>

<a name="openai-chat-vision-quickstart"></a>
### #&#8288;25 [openai-chat-vision-quickstart](https://github.com/azure-samples/openai-chat-vision-quickstart) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT · Oct 2026</sub>

**Quart chat app that answers questions about uploaded images via Azure OpenAI.**

A Python Quart backend uses the openai package to send user messages and uploaded images to a GPT-4o deployment on Azure OpenAI. The frontend is plain HTML/JS that streams JSON Lines responses, with browser speech input and output buttons. Bicep files and azd provision Azure OpenAI, Container Apps, Container Registry and Log Analytics, using managed identity by default.

- **+** One azd up provisions Azure OpenAI, Container Apps, registry, logging and RBAC
- **+** Managed identity by default, so no API key in app config
- **+** Can point at a local OpenAI-compatible endpoint (Ollama doc) for development
- **+** Speech input/output uses free built-in browser APIs
- **−** Deploying needs Azure subscription and role-assignment write permissions
- **−** Basic HTML/JS frontend with no auth or multi-user features
- **−** Container Registry has a fixed daily cost even when idle
- **−** Local dev server still needs Azure credentials or a compatible endpoint

<sub>Jupyter Notebook, GPT-4o (Azure OpenAI), OpenAI-compatible endpoints · Needs Azure OpenAI, Azure Container Apps, Azure Container Registry, Azure Developer CLI · env example file · [Repo](https://github.com/azure-samples/openai-chat-vision-quickstart) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/ai/get-started-app-chat-vision?tabs=github-codespaces) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openai-chat-vision-quickstart/)</sub>

<a name="get-started-with-ai-agents"></a>
### #&#8288;26 [get-started-with-ai-agents](https://github.com/azure-samples/get-started-with-ai-agents) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 385 · MIT · Oct 2026</sub>

**Azure azd template for a Foundry agent chat app with file search.**

Deploys a web chat app on Azure Container Apps backed by a Microsoft Foundry Agent Service agent. The agent answers from uploaded files using file search or optional Azure AI Search and returns citations. Tracing goes to Application Insights, and the repo includes Pytest-based agent evaluation and red-teaming scans.

- **+** Single `azd up` provisions Foundry project, model, Container App, storage and monitoring
- **+** Tracing via Application Insights and Azure Monitor included
- **+** Pytest agent evaluation and AI Red Teaming scans included
- **+** Managed Identity used for deployment and local development
- **−** Requires an Azure subscription and Foundry model quota; no non-Azure path
- **−** README warns the code is a showcase, not production-ready without extra security
- **−** Costs are usage-based and the README gives no estimate
- **−** Deployment takes 7–15 minutes with `azd up`; teardown up to 20

<sub>Bicep, gpt-5-mini (default), other Azure AI models configurable · Needs Microsoft Foundry, Foundry Agent Service, Azure Container Apps, Azure Container Registry, Azure Storage, Azure AI Search (optional), Application Insights (optional), Log Analytics (optional) · [Repo](https://github.com/azure-samples/get-started-with-ai-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/get-started-with-ai-agents/)</sub>

<a name="nodejs-api-boilerplate"></a>
### #&#8288;27 [nodejs-api-boilerplate](https://github.com/vyancharuk/nodejs-api-boilerplate) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 164 · MIT · Nov 2026</sub>

**Express TypeScript CRUD API template with an LLM module generator.**

Express and TypeScript REST API with vertical-slice modules, Zod validation, InversifyJS DI, Knex transactions, ioredis caching, winston trace IDs, node-cron, S3 uploads and Supertest e2e tests, run via docker compose on port 8080. The llm-codegen folder runs three LLM micro-agents (Developer, Troubleshooter, TestsFixer) that generate a new CRUD module, migration, seeds and passing tests from a text description.

- **+** Codegen loop compiles and runs e2e tests until they pass
- **+** Supports OpenAI, Anthropic, DeepSeek and OpenRouter keys for generation
- **+** JWT auth routes, Redis cache and cron already in the base API
- **+** Tests run in Docker or against local SQLite
- **−** AI is a dev-time generator; the API itself has no AI features
- **−** Node badge pins v14 to v20; check against current LTS
- **−** Generated code still needs manual review and integration
- **−** Last commit 2026-04

<sub>TypeScript, OpenAI, Anthropic, DeepSeek, OpenRouter · Needs PostgreSQL or SQLite, Redis, AWS S3 (uploads), LLM API key for codegen · GitHub template · Docker · env example file · [Repo](https://github.com/vyancharuk/nodejs-api-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nodejs-api-boilerplate/)</sub>

<a name="genai-api"></a>
### #&#8288;28 [genai-api](https://github.com/louisbrulenaudet/genai-api) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: niche (1) · Freshness: recent (53) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 112 · Apache-2.0 · Apr 2026</sub>

**Hono API on Cloudflare Workers proxying Gemini with bearer auth.**

Hono TypeScript worker exposing POST /completion that forwards OpenAI-style messages (text and data-URL images) to Gemini 2.0 and 2.5 Flash models through Cloudflare AI Gateway, validated with Zod and returned as plain text. Secured by a BEARER_TOKEN secret, with an optional X-API-Key header to pass a provider key per request; deployed with make deploy. Built for Apple Shortcuts; local dev on port 8788.

- **+** Bearer-token auth and Zod validation on the single endpoint
- **+** Requests route through Cloudflare AI Gateway for caching and logs
- **+** Multimodal input via data-URL images
- **+** Biome lint and Snyk badge
- **−** Google AI Studio provider only; four Gemini Flash models
- **−** Plain-text responses, no streaming
- **−** No tests mentioned; last commit 2026-04
- **−** Needs a Cloudflare account and AI Gateway id

<sub>TypeScript, Gemini 2.5 Flash, 2.5 Flash Lite, 2.0 Flash, 2.0 Flash Lite via Cloudflare AI Gateway, OpenAI SDK client · Needs Cloudflare account with AI Gateway, Google AI Studio API key · GitHub template · [Repo](https://github.com/louisbrulenaudet/genai-api) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/genai-api/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
