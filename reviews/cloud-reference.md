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
### 🥈 [fiber](https://github.com/gofiber/fiber) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Nov 2026</sub>

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

<a name="generator-jhipster"></a>
### 🥉 [generator-jhipster](https://github.com/jhipster/generator-jhipster) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

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

<a name="serverless"></a>
### #&#8288;4 [serverless](https://github.com/serverless/serverless) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · custom license · Nov 2026</sub>

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

<a name="echo"></a>
### #&#8288;5 [echo](https://github.com/labstack/echo) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

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

<a name="douyin-tiktok-download-api"></a>
### #&#8288;6 [douyin_tiktok_download_api](https://github.com/evil0ctal/douyin_tiktok_download_api) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

**Self-hosted REST and MCP API for Douyin, TikTok and Bilibili data.**

FastAPI service that fetches posts, authors, comments, sounds, hashtags, live rooms and trending boards from Douyin, TikTok and Bilibili, and downloads media without watermarks. It keeps a self-maintaining pool of guest identities minted by a headless browser, archives parsed data in PostgreSQL, and exposes REST, an MCP endpoint and a React console. Downloaded videos can be transcribed offline with FunASR, mainly for Mandarin.

- **+** Identity pool with health tiers, rate limits and circuit breakers; per-request logs visible in console
- **+** Same service layer served over REST, MCP (streamable-http) and a CLI
- **+** Offline FunASR transcription ran a 3 min clip in 3.7 s on two CPU cores
- **+** Archives parsed posts in PostgreSQL, so content deleted upstream stays available
- **−** Needs PostgreSQL and Redis, plus separate browser and transcription containers
- **−** Douyin search, hashtag posts, followers and following are not offered without a signed-in session
- **−** Transcription models are general Chinese ones; other languages come out poorly
- **−** v5 is a full rewrite; v4 is frozen and its bundled Douyin cookie has expired

<sub>Python, FunASR ONNX (Paraformer, FSMN-VAD, CT-Transformer) · Needs PostgreSQL, Redis, CloakBrowser (headless, container), FunASR ONNX models (optional) · Docker · env example file · [Repo](https://github.com/evil0ctal/douyin_tiktok_download_api) · [▶️ Demo ↗](https://demo.douyin.wtf) · [📖 Docs ↗](https://douyin.wtf) · [🌐 Site ↗](https://douyin.wtf) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/douyin-tiktok-download-api/)</sub>

<a name="gf"></a>
### #&#8288;7 [gf](https://github.com/gogf/gf) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Nov 2026</sub>

**Modular Go application framework with an HTTP server and CLI scaffolding.**

GoFrame is a general-purpose Go framework that can be used as a full application framework or as individual components. The README shows an HTTP server (g.Server with handler binding) and a gf CLI that scaffolds and runs projects. It has no AI features and requires Go 1.25 or later.

- **+** Components can be imported individually instead of adopting the full framework
- **+** gf CLI scaffolds a project (gf init) and runs it (gf run)
- **+** MIT license, with English and Chinese docs plus mirror sites and offline PDFs
- **+** Recent activity: release 2026-10-28, commit 2026-11-10
- **−** No AI, model or agent integration described in the README
- **−** Go only, and requires Go 1.25 or later
- **−** README names no components beyond the HTTP server, so scope needs the docs site
- **−** No Dockerfile or compose file detected in the repo

<sub>Go · Needs Go 1.25+ · [Repo](https://github.com/gogf/gf) · [📖 Docs ↗](https://goframe.org/en) · [🌐 Site ↗](https://goframe.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gf/)</sub>

<a name="goa"></a>
### #&#8288;8 [goa](https://github.com/goadesign/goa) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Nov 2026</sub>

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

<a name="hono"></a>
### #&#8288;9 [hono](https://github.com/honojs/hono) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

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

<a name="full-stack-fastapi-template"></a>
### #&#8288;10 [full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

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

<a name="midway"></a>
### #&#8288;11 [midway](https://github.com/midwayjs/midway) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

**TypeScript Node.js framework using decorators and dependency injection.**

Midway is a Node.js framework written in TypeScript that uses decorators and dependency injection to build web apps, microservices, serverless/FaaS functions and mini-program backends. It runs on Koa, Express or Egg.js and also supports Socket.io, gRPC, Dubbo.js and RabbitMQ. It is a general backend framework with no AI-specific features in the README.

- **+** Runs on Koa, Express or Egg.js and can reuse plugins from those ecosystems
- **+** Deploys to regular servers or serverless/FaaS (AWS, Alibaba Cloud, Tencent Cloud)
- **+** Covers HTTP, Socket.io, gRPC, Dubbo.js and RabbitMQ in one framework
- **+** Project scaffold via npm init midway; MIT licensed
- **−** No LLM, agent or model-serving features; a generic backend framework
- **−** README and community channels are mainly in Chinese
- **−** Decorator and dependency-injection style adds a learning curve over plain Koa or Express
- **−** Full-stack hooks mode ties the frontend to @midwayjs/hooks

<sub>TypeScript · Needs Node.js · [Repo](https://github.com/midwayjs/midway) · [🌐 Site ↗](https://midwayjs.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/midway/)</sub>

<a name="elysia"></a>
### #&#8288;12 [elysia](https://github.com/elysiajs/elysia) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

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

<a name="chi"></a>
### #&#8288;13 [chi](https://github.com/go-chi/chi) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

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
### #&#8288;14 [gofr](https://github.com/gofr-dev/gofr) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

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

<a name="falcon"></a>
### #&#8288;15 [falcon](https://github.com/falconry/falcon) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · Apache-2.0 · Nov 2026</sub>

**Minimalist Python ASGI/WSGI framework for building REST APIs and microservices.**

Falcon is a Python web framework for REST APIs that runs on any WSGI or ASGI server, with native asyncio and WebSocket support. It models APIs as resource classes with on_get/on_post responders, plus middleware, hooks and error handlers. It has no dependencies outside the standard library and compiles itself with Cython when available. It is a general backend framework, not AI-specific.

- **+** No dependencies outside the standard library; pip install falcon is enough
- **+** Supports both WSGI and ASGI apps, plus WebSockets and native asyncio
- **+** Optional Cython compilation, with pre-compiled wheels for common platforms and PyPy 3.9+ support
- **+** Project requires 100% test coverage and avoids breaking changes outside major versions
- **−** No built-in AI, LLM or model-serving features; you wire those in yourself
- **−** Leaves ORM, auth and validation choices to you; only middleware and hooks are provided
- **−** Needs a separate WSGI or ASGI server such as Gunicorn or Uvicorn in production
- **−** Automatic request body parsing is disabled by default and must be set up explicitly

<sub>Python · Needs Python 3.9+ or PyPy 3.9+, WSGI server (Gunicorn, uWSGI) or ASGI server (Uvicorn, Granian) · Docker · [Repo](https://github.com/falconry/falcon) · [📖 Docs ↗](https://falcon.readthedocs.io/en/stable) · [🌐 Site ↗](https://falconframework.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/falcon/)</sub>

<a name="django-ninja"></a>
### #&#8288;16 [django-ninja](https://github.com/vitalik/django-ninja) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Nov 2026</sub>

**Type-hint-based REST API framework for Django with OpenAPI docs.**

Django Ninja is a Python library for building APIs inside a Django project, using type hints and Pydantic for validation and serialization. It generates an OpenAPI schema and serves interactive Swagger UI or Redoc docs at /api/docs. It supports async views and works with the Django ORM. It is a general API framework with no AI-specific features.

- **+** Validates and type-casts request parameters from function signatures via Pydantic
- **+** Generates OpenAPI schema and interactive Swagger UI or Redoc docs automatically
- **+** Added to an existing Django project with an api.py file and one URL entry
- **+** Supports async views and integrates with the Django ORM
- **−** Requires Django; not usable as a standalone framework
- **−** No AI, model or agent features; only a general API layer
- **−** README shows benchmarks only as an image, with no figures in text
- **−** Not a template: no auth, billing or model integration included

<sub>Python · Needs Django, Pydantic · [Repo](https://github.com/vitalik/django-ninja) · [📖 Docs ↗](https://django-ninja.dev) · [🌐 Site ↗](https://django-ninja.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/django-ninja/)</sub>

<a name="oapi-codegen"></a>
### #&#8288;17 [oapi-codegen](https://github.com/oapi-codegen/oapi-codegen) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.7k · Apache-2.0 · Nov 2026</sub>

**Go code generator that turns OpenAPI specs into servers, clients and types.**

oapi-codegen is a Go command-line tool and library that reads OpenAPI 3.0 and 3.1 specs and generates Go server interfaces, API clients, or plain HTTP models. It is configured through a YAML file and typically run via go:generate. It has no AI features, so it fits this list only loosely as backend scaffolding.

- **+** Generates server stubs for several Go frameworks, including net/http, plus clients and models
- **+** Optional strict server mode handles request and response marshalling for you
- **+** Supports OpenAPI 3.0 and 3.1, including webhooks and the 3.2 QUERY method
- **+** Generated code comes from text/templates you can override
- **−** No OpenAPI 2.0 (Swagger) support; specs must be converted first
- **−** Template overrides and importing pkg/ are explicitly unstable across releases
- **−** Building the tool requires Go 1.26+
- **−** No defined release cadence; README recommends pinning to commits for unreleased fixes

<sub>Go · Needs Go 1.26+ · [Repo](https://github.com/oapi-codegen/oapi-codegen) · [📖 Docs ↗](https://pkg.go.dev/github.com/oapi-codegen/oapi-codegen/v2/pkg) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oapi-codegen/)</sub>

<a name="go-clean-template"></a>
### #&#8288;18 [go-clean-template](https://github.com/evrone/go-clean-template) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Nov 2026</sub>

**Clean Architecture Go microservice template with REST, gRPC, RabbitMQ and NATS.**

A Go service template that shows how to layer a microservice with Clean Architecture and constructor-based dependency injection. It ships three demo domains (user auth with JWT, tasks, translation) exposed over REST (Fiber), gRPC, AMQP RPC and NATS RPC, backed by Postgres. Includes Swagger, Prometheus metrics, OpenTelemetry tracing to Jaeger, migrations and integration tests.

- **+** Same three domains implemented across REST, gRPC, AMQP RPC and NATS RPC
- **+** OpenTelemetry traces span all four transports, with Jaeger in the compose stack
- **+** Interface-based DI makes use cases mockable with go.uber.org/mock
- **+** Compose targets for local dev, CI integration tests and full stack with proxy
- **−** Local run needs Postgres, RabbitMQ and NATS even if only REST is wanted
- **−** Translation domain depends on an external translation API
- **−** No LLM or model integration; it is a generic Go backend template
- **−** Demo credentials in compose and README must be replaced before real use

<sub>Go · Needs PostgreSQL, RabbitMQ, NATS, Jaeger (optional) · GitHub template · Docker · env example file · [Repo](https://github.com/evrone/go-clean-template) · [🌐 Site ↗](https://evrone.com/go-clean-template) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-clean-template/)</sub>

<a name="gqlgen"></a>
### #&#8288;19 [gqlgen](https://github.com/99designs/gqlgen) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

**Schema-first GraphQL server generator for Go with typed resolvers.**

gqlgen is a Go library and code generator that reads a GraphQL schema (SDL) and generates typed server code and models, so you only write resolver functions. Behavior is configured through gqlgen.yml or inline schema directives such as @goModel and @goField. It is not AI-specific; it fits only loosely in this list as a backend API starter.

- **+** Schema-first: generates Go models and server code from GraphQL SDL
- **+** Typed output; README states no map[string]interface{} in generated code
- **+** Binds to your own Go structs via gqlgen.yml or @goModel directives
- **+** Field resolvers run concurrently in goroutines, with a configurable worker_limit
- **−** No AI, model or agent features; it is a general GraphQL tool
- **−** Go only; requires running a generate step after schema changes
- **−** Remapping ID type has one default; the first listed model is always used
- **−** Nested fields need custom models or explicit resolvers to avoid over-fetching

<sub>Go · Needs Go toolchain · [Repo](https://github.com/99designs/gqlgen) · [📖 Docs ↗](https://gqlgen.com/getting-started/) · [🌐 Site ↗](https://gqlgen.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gqlgen/)</sub>

<a name="go-zero"></a>
### #&#8288;20 [go-zero](https://github.com/zeromicro/go-zero) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

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

<a name="full-stack-ai-agent-template"></a>
### #&#8288;21 [full-stack-ai-agent-template](https://github.com/vstorm-co/full-stack-ai-agent-template) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="microservices-demo"></a>
### #&#8288;22 [microservices-demo](https://github.com/googlecloudplatform/microservices-demo) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

**Eleven-service e-commerce demo for Kubernetes, with gRPC between services.**

Online Boutique is a web store (browse, cart, checkout) split into 11 microservices in Go, C#, Node.js, Python and Java that talk over gRPC. Google uses it to demonstrate GKE, Cloud Service Mesh, Spanner, Memorystore, AlloyDB and Gemini. It runs on any Kubernetes cluster and ships a load generator, Kustomize variants and Terraform. AI is limited to an optional Gemini shopping assistant.

- **+** Polyglot services (Go, C#, Node.js, Python, Java) with protobuf definitions in ./protos
- **+** Kustomize variants and Terraform cover Istio, tracing and other deployment options
- **+** Built-in Locust load generator imitates realistic shopping flows
- **+** Runs on any Kubernetes cluster, not only GKE
- **−** Payment, shipping and email services are mocks, not usable for a real store
- **−** AI is only an optional Gemini assistant, not a core feature
- **−** Quickstart targets GKE and needs a Google Cloud project
- **−** No Docker or Compose setup detected; a Kubernetes cluster is needed

<sub>Go, Gemini · Needs Kubernetes, Redis, Google Cloud (GKE quickstart), Gemini (optional assistant) · [Repo](https://github.com/googlecloudplatform/microservices-demo) · [📖 Docs ↗](https://github.com/GoogleCloudPlatform/microservices-demo/blob/main/docs/development-guide.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/microservices-demo/)</sub>

<a name="litestar"></a>
### #&#8288;23 [litestar](https://github.com/litestar-org/litestar) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · MIT · Nov 2026</sub>

**Typed Python ASGI framework for building APIs with OpenAPI generation.**

Litestar is a Python ASGI framework for building HTTP APIs. It provides class-based controllers, dependency injection, layered middleware, route guards and OpenAPI 3.1 schema generation, with msgspec-based serialization. It is a general backend framework rather than an AI-specific starter, so it fits as the service layer behind a model or agent API.

- **+** Generates OpenAPI 3.1 and serves Scalar, Redoc, Stoplight Elements and Swagger-UI docs
- **+** Validates dataclasses, TypedDict, msgspec, pydantic v1/v2 and attrs models
- **+** Ships middleware for CORS, CSRF, rate limiting, compression and sessions
- **+** Built-in SQLAlchemy plugin and DTO support
- **−** No AI, LLM or agent features; you wire up model calls yourself
- **−** Strictly typed: a route handler missing a return annotation raises an exception
- **−** Performance claims are general; the README gives no concrete numbers

<sub>Python · Needs Python, uvicorn (via litestar[standard]) · [Repo](https://github.com/litestar-org/litestar) · [📖 Docs ↗](https://docs.litestar.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/litestar/)</sub>

<a name="agent-service-toolkit"></a>
### #&#8288;24 [agent-service-toolkit](https://github.com/joshuac215/agent-service-toolkit) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

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

<a name="javalin"></a>
### #&#8288;25 [javalin](https://github.com/javalin/javalin) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · Apache-2.0 · Oct 2026</sub>

**Lightweight web framework for Java and Kotlin with WebSockets and HTTP/2.**

Javalin is a web library for Java and Kotlin that handles HTTP routing, WebSockets, HTTP/2, async requests, static files, JSON mapping and file uploads. It avoids annotations, reflection and base classes to extend, so handlers are plain lambdas registered on a config object. It has no AI features; it fits this list only as a generic backend service base, with plugins for OpenAPI and SSL.

- **+** No annotations, reflection or required base classes; handlers are plain lambdas
- **+** Same API in Java and Kotlin, with examples for both
- **+** Built-in WebSockets, static files, JSON mapping and file uploads
- **+** Plugin system, including OpenAPI 3.0 generation and SSL (PEM, PKCS12, JKS)
- **−** No AI, model or agent integration; only a generic HTTP backend
- **−** Not a template: no auth, database or billing wired in
- **−** OpenAPI support is a separate plugin that relies on annotations
- **−** Dependency, JSON mapper and database choices are left to you

<sub>Kotlin · Needs JVM (Java or Kotlin), Maven or Gradle · [Repo](https://github.com/javalin/javalin) · [📖 Docs ↗](https://javalin.io/documentation) · [🌐 Site ↗](https://javalin.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/javalin/)</sub>

<a name="azure-agent-landing-zone"></a>
### #&#8288;26 [agent-landing-zone](https://github.com/azure/agent-landing-zone) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

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

<a name="chalice"></a>
### #&#8288;27 [chalice](https://github.com/aws/chalice) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

**Python framework for writing and deploying AWS Lambda apps with decorators.**

Chalice is a Python framework and CLI for building serverless apps on AWS Lambda. Decorators map functions to API Gateway routes, scheduled events, S3 events, SQS messages and other AWS triggers, and `chalice deploy` packages the code, generates IAM policies and creates the resources. It has no AI-specific features; it fits as a backend template for exposing code over an API on AWS.

- **+** Decorator API for REST routes, schedules, S3, SNS and SQS triggers
- **+** `chalice deploy` creates the Lambda, IAM role and API Gateway in one command
- **+** Automatic IAM policy generation from the code
- **+** `chalice delete` removes the resources it created
- **−** Tied to AWS Lambda and API Gateway; no other cloud or runtime
- **−** Python only
- **−** No AI, model or agent tooling included
- **−** Needs configured AWS credentials before the first deploy

<sub>Python · Needs AWS account and credentials, AWS Lambda, Amazon API Gateway, Python 3.10+ · [Repo](https://github.com/aws/chalice) · [📖 Docs ↗](https://aws.github.io/chalice/) · [🌐 Site ↗](https://aws.github.io/chalice/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chalice/)</sub>

<a name="monid"></a>
### #&#8288;28 [monid](https://github.com/monid-ai/monid) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Nov 2026</sub>

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

<a name="fastapi-langgraph-agent-production-ready-template"></a>
### #&#8288;29 [fastapi-langgraph-agent-production-ready-template](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

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

<a name="api-platform"></a>
### #&#8288;30 [api-platform](https://github.com/api-platform/api-platform) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Nov 2026</sub>

**Installer that scaffolds API Platform projects on Symfony or Laravel.**

This repository hosts the `api-platform` installer, a static binary or Composer package that scaffolds a new API-first PHP project, with flags such as --framework=symfony or laravel, --with-docker and --with-pwa. The generated stack exposes REST (JSON-LD, Hydra, HAL, JSON:API) and GraphQL APIs from plain PHP classes, with OpenAPI docs and an optional React admin. It is not an AI project; the list includes it as a backend template.

- **+** Exposes REST and GraphQL from plain PHP classes, with pagination, validation and filters
- **+** Content negotiation out of the box: JSON-LD, Hydra, HAL, JSON:API, YAML, XML, CSV
- **+** Generates OpenAPI docs, a React admin and Next.js, Nuxt or React Native clients
- **+** Ships as a static binary or via Composer; MIT licensed
- **−** No AI or model features; only loosely fits an AI project list
- **−** PHP and Symfony stack; Laravel is supported only as a framework option
- **−** Repository holds only the installer; framework code and docs live elsewhere
- **−** Linked Data and Hydra concepts add a learning curve for simple APIs

<sub>PHP · Needs PHP, Composer, Symfony, Doctrine ORM · GitHub template · [Repo](https://github.com/api-platform/api-platform) · [📖 Docs ↗](https://api-platform.com/docs/distribution/) · [🌐 Site ↗](https://api-platform.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/api-platform/)</sub>

<a name="hyperf"></a>
### #&#8288;31 [hyperf](https://github.com/hyperf/hyperf) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · MIT · Oct 2026</sub>

**Coroutine PHP framework on Swoole or Swow for microservices and web servers.**

Hyperf is a PHP 8.1+ CLI framework that runs on Swoole 5.0+ or Swow 1.4+ coroutine servers instead of PHP-FPM. It combines dependency injection with AOP, annotations and events, and ships coroutine-compatible clients and servers for MySQL, Redis, gRPC, JSON-RPC, WebSocket, AMQP, Consul and ETCD. Core components follow PSR standards and can be used in other frameworks.

- **+** Coroutine servers on Swoole or Swow; README benchmark shows about 103,921 requests/sec on 8 cores
- **+** Built-in coroutine clients for MySQL, Redis, gRPC, JSON-RPC, RabbitMQ, NSQ, Nats, Consul and ETCD
- **+** DI container with AOP and annotations makes classes pluggable; components follow PSR standards
- **+** MIT license with multilingual docs and per-component unit tests
- **−** Requires the Swoole or Swow extension, so it does not run under plain PHP-FPM
- **−** No AI or model-serving features; it is a general-purpose backend framework
- **−** Runs as a long-lived CLI process, so code must be coroutine-safe
- **−** Benchmark is a single wrk request to the root URL, not a realistic workload

<sub>PHP · Needs PHP 8.1+, Swoole 5.0+ or Swow 1.4+ · [Repo](https://github.com/hyperf/hyperf) · [📖 Docs ↗](https://hyperf.wiki) · [🌐 Site ↗](https://hyperf.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hyperf/)</sub>

<a name="generative-ai-project-template"></a>
### #&#8288;32 [generative-ai-project-template](https://github.com/aminedjeghri/generative-ai-project-template) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 118 · MIT · Nov 2026</sub>

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

<a name="typescript-express-starter"></a>
### #&#8288;33 [typescript-express-starter](https://github.com/ljlm0402/typescript-express-starter) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (33) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**CLI that generates TypeScript Express REST API projects with selectable tooling.**

An npm CLI that scaffolds a TypeScript Express REST API from three templates: basic Express with Zod validation, Drizzle with PostgreSQL, and express-cargo decorator-based validation. You pick linter, bundler, test runner and Docker in quick or custom mode, and it installs dependencies and generates .env with random secrets. Generated projects include auth and user routes under /api/v1.

- **+** Mix-and-match tooling: ESLint, Biome or Oxlint; SWC or tsup; Jest or Vitest
- **+** Generates .env with random SECRET_KEY and JWT_SECRET of at least 32 characters
- **+** Works with npm, pnpm or yarn; run via npx without global install
- **+** Generation tests cover 36 template and tool combinations
- **−** Only PostgreSQL via Drizzle is selectable; Prisma and Mongoose are excluded from the npm package
- **−** Default and express-cargo templates store users in memory and reset on restart
- **−** No AI or model integration; it is a generic API scaffold
- **−** Swagger, CI workflows, husky and pm2 options are still unfinished

<sub>TypeScript · Needs Node.js 22.12.0+, npm 9.11.0+, PostgreSQL (Drizzle template only), Docker with Compose (optional) · [Repo](https://github.com/ljlm0402/typescript-express-starter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typescript-express-starter/)</sub>

<a name="fastcrud"></a>
### #&#8288;34 [fastcrud](https://github.com/benavlabs/fastcrud) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

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
### #&#8288;35 [node-typescript-boilerplate](https://github.com/jsynowiec/node-typescript-boilerplate) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (35) · Freshness: active (100) · Maintenance: patchy (35) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="golang-gin-realworld-example-app"></a>
### #&#8288;36 [golang-gin-realworld-example-app](https://github.com/realworld-apps/golang-gin-realworld-example-app) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (30) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

**Go/Gin REST backend implementing the RealWorld Conduit API with SQLite.**

A Go backend built on Gin and GORM v2 that implements the RealWorld (Conduit) API: users, JWT auth, profiles, articles, comments, favorites and pagination. Data is stored in SQLite and the app starts with `go run hello.go` on port 8080 by default. It passes the RealWorld Hurl and Bruno spec suites and reports about 90% test coverage.

- **+** Passes the RealWorld Hurl and Bruno API spec suites, run in CI
- **+** Reported test coverage around 90% (articles, users, common packages)
- **+** Small layout: per-domain models, serializers, routers, middlewares, validators
- **+** Uses current libraries: GORM v2, golang-jwt v5, validator v10
- **−** No AI or model functionality; it is a plain CRUD API example
- **−** SQLite only; the sqlite driver requires cgo
- **−** No Dockerfile or compose file provided
- **−** Todo list still open: ProtoBuf support, config cleanup, interfaces

<sub>Go · Needs Go 1.21+, SQLite (cgo) · env example file · [Repo](https://github.com/realworld-apps/golang-gin-realworld-example-app) · [📖 Docs ↗](https://godoc.org/github.com/gothinkster/golang-gin-realworld-example-app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/golang-gin-realworld-example-app/)</sub>

<a name="genlayer-project-boilerplate"></a>
### #&#8288;37 [genlayer-project-boilerplate](https://github.com/genlayerlabs/genlayer-project-boilerplate) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (76) · Freshness: recent (71) · Maintenance: weak (13) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Jun 2026</sub>

**GenLayer starter with a Python betting contract, tests, and Next.js frontend.**

Boilerplate for building on GenLayer, built around a Football Bets intelligent contract written in Python. The contract fetches match results from BBC Sport, uses an LLM to extract the score, and validates it through the equivalence principle. The repo includes a linter, in-memory direct tests with web and LLM mocks, Studio integration tests, deploy scripts, and a Next.js 15 frontend.

- **+** Direct-mode pytest tests mock web and LLM calls, at about a millisecond per test
- **+** genvm-lint flags non-deterministic calls and invalid storage types in about 250ms
- **+** Includes a GitHub Actions workflow for linting and direct tests
- **+** Frontend uses Next.js 15, TypeScript, TanStack Query and Radix UI
- **−** Tied to GenLayer; contracts run only on its Studio or networks
- **−** Single example contract (football bets), so other use cases need rewriting
- **−** Integration tests and deployment need GenLayer Studio, local or hosted
- **−** No auth or billing; it is a contract and frontend starter, not a SaaS boilerplate

<sub>TypeScript · Needs Python >= 3.12, GenLayer CLI (npm install -g genlayer), GenLayer Studio (local or hosted), Node.js/npm · [Repo](https://github.com/genlayerlabs/genlayer-project-boilerplate) · [📖 Docs ↗](https://docs.genlayer.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/genlayer-project-boilerplate/)</sub>

<a name="wild-workouts-go-ddd-example"></a>
### #&#8288;38 [wild-workouts-go-ddd-example](https://github.com/threedotslabs/wild-workouts-go-ddd-example) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (50) · Freshness: recent (70) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Aug 2026</sub>

**Go example app showing DDD, CQRS and Clean Architecture via refactoring.**

Wild Workouts is a training-scheduling web app written in Go, built as a companion to a series of threedots.tech articles. It is split into services that talk over gRPC and deploy to Google Cloud Run with Firebase auth, with a Vue frontend. Tagged releases map to articles and show refactoring toward DDD Lite, the repository pattern, CQRS and Clean Architecture.

- **+** Tagged releases (v1.0 to v2.7) match articles, so refactoring steps can be diffed
- **+** Covers repository pattern, CQRS, database integration tests and microservice test architecture
- **+** Terraform setup provisions the Google Cloud project, Cloud Run and Firebase
- **+** Live demo and local docker-compose run are provided
- **−** Not an AI project; the README mentions no model or LLM integration
- **−** Last tagged release is 2021-04-01; README says the article series is still in progress
- **−** Cloud deployment needs a Google Cloud billing account and Firebase
- **−** Reference example to read, not a reusable template or library

<sub>Go · Needs Google Cloud Run, Firebase, Terraform, Docker Compose · Docker · ⚠️ .env file committed · [Repo](https://github.com/threedotslabs/wild-workouts-go-ddd-example) · [▶️ Demo ↗](https://threedotslabs-wildworkouts.web.app/) · [🌐 Site ↗](https://threedots.tech) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wild-workouts-go-ddd-example/)</sub>

<a name="fullstack-solution-template-for-agentcore"></a>
### #&#8288;39 [fullstack-solution-template-for-agentcore](https://github.com/awslabs/fullstack-solution-template-for-agentcore) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 603 · Apache-2.0 · Nov 2026</sub>

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

<a name="nunu"></a>
### #&#8288;40 [nunu](https://github.com/go-nunu/nunu) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Aug 2026</sub>

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

<a name="serverless-rag-demo"></a>
### #&#8288;41 [serverless-rag-demo](https://github.com/aws-samples/serverless-rag-demo) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT-0 · Oct 2026</sub>

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
### #&#8288;42 [openai-chat-app-quickstart](https://github.com/azure-samples/openai-chat-app-quickstart) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 254 · MIT · Oct 2026</sub>

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
### #&#8288;43 [openai-chat-vision-quickstart](https://github.com/azure-samples/openai-chat-vision-quickstart) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT · Oct 2026</sub>

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

<a name="nodejs-api-boilerplate"></a>
### #&#8288;44 [nodejs-api-boilerplate](https://github.com/vyancharuk/nodejs-api-boilerplate) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 164 · MIT · Nov 2026</sub>

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

<a name="get-started-with-ai-agents"></a>
### #&#8288;45 [get-started-with-ai-agents](https://github.com/azure-samples/get-started-with-ai-agents) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 385 · MIT · Oct 2026</sub>

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

<a name="genai-api"></a>
### #&#8288;46 [genai-api](https://github.com/louisbrulenaudet/genai-api) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: niche (0) · Freshness: recent (53) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 112 · Apache-2.0 · Apr 2026</sub>

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
