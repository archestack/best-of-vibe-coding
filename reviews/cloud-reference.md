# ☁️ Backend and cloud templates reviews · Best of Vibe Coding

Backend service templates (FastAPI, Express, Hono) that expose models or agents over an API, and vendor reference apps for Azure or Google Cloud. Back to the [leaderboard](../README.md#%EF%B8%8F-backend-and-cloud-templates).

<sub>🌐 Also on the web: [Backend and cloud templates on archestack.com](https://archestack.com/best-of-vibe-coding/cloud-reference/), each project on its own page.</sub>

<a name="trpc"></a>
### 🥇 [trpc](https://github.com/trpc/trpc) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Nov 2026</sub>

**TypeScript library for typesafe APIs without schemas or code generation.**

tRPC lets a TypeScript client call server procedures with inferred types for inputs, outputs and errors, so the client imports only type declarations from the server. It has no code generation step and zero dependencies, and ships adapters for React, Next.js, Express and Fastify, plus subscriptions and request batching. The repo includes example apps, such as a Next.js and Prisma starter.

- **+** No schema files or code generation; types flow from server to client
- **+** Zero dependencies with a small client footprint
- **+** Adapters for React, Next.js, Express and Fastify, plus community adapters
- **+** Supports subscriptions and automatic batching of concurrent requests
- **−** Type sharing assumes a TypeScript client and server, typically in one repo
- **−** Not an AI project; no model or LLM features in the README
- **−** Not a standalone service; it is a library you embed in an existing app
- **−** Starter examples are in the repo, not a dedicated template package

<sub>TypeScript · [Repo](https://github.com/trpc/trpc) · [📖 Docs ↗](https://trpc.io/docs) · [🌐 Site ↗](https://trpc.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trpc/)</sub>

<a name="generator-jhipster"></a>
### 🥈 [generator-jhipster](https://github.com/jhipster/generator-jhipster) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

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

<a name="fastapi"></a>
### 🥉 [fastapi](https://github.com/fastapi/fastapi) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 105k · MIT · Nov 2026</sub>

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
### #&#8288;4 [fiber](https://github.com/gofiber/fiber) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Nov 2026</sub>

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

<a name="echo"></a>
### #&#8288;5 [echo](https://github.com/labstack/echo) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

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

<a name="serverless"></a>
### #&#8288;6 [serverless](https://github.com/serverless/serverless) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · custom license · Nov 2026</sub>

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

<a name="douyin-tiktok-download-api"></a>
### #&#8288;7 [douyin_tiktok_download_api](https://github.com/evil0ctal/douyin_tiktok_download_api) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Nov 2026</sub>

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

<a name="vapor"></a>
### #&#8288;8 [vapor](https://github.com/vapor/vapor) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Nov 2026</sub>

**HTTP web framework for building APIs and websites in Swift.**

Vapor is a server-side HTTP web framework written in Swift, aimed at websites, APIs and cloud services. It requires Swift 6.0 or newer and is MIT licensed. It has no AI-specific features, so it fits this list only as a base for exposing models or agents over an API.

- **+** Written in Swift, so Apple-platform teams can share language and types with the server
- **+** Targets Swift 6.0+, so it is built for current Swift concurrency
- **+** MIT license with CI and code coverage badges
- **+** Active: last release 2026-10-13, last commit 2026-11-13
- **−** No built-in AI, LLM or agent features; model calls must be written by hand
- **−** README has no feature list, so ORM, auth and database support need the docs
- **−** Swift server ecosystem has fewer AI libraries than Python or Node
- **−** Framework only: no starter app or Docker setup in this repository

<sub>Swift · Needs Swift 6.0+ · [Repo](https://github.com/vapor/vapor) · [📖 Docs ↗](https://docs.vapor.codes/4.0/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vapor/)</sub>

<a name="hono"></a>
### #&#8288;9 [hono](https://github.com/honojs/hono) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

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

<a name="gf"></a>
### #&#8288;10 [gf](https://github.com/gogf/gf) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Nov 2026</sub>

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

<a name="aws-cdk"></a>
### #&#8288;11 [aws-cdk](https://github.com/aws/aws-cdk) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: fair (80) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

**Define AWS infrastructure in code and deploy it through CloudFormation.**

AWS CDK is a framework for defining AWS resources as constructs in TypeScript, JavaScript, Python, Java, .NET or Go. The cdk CLI synthesizes CloudFormation templates, deploys stacks and diffs local code against what is deployed. It is general infrastructure tooling with no AI features, so it fits this list only as a cloud deployment option.

- **+** Supports six languages: JavaScript, TypeScript, Python, Java, .NET and Go
- **+** Per-service construct library wraps AWS details and reduces glue code
- **+** CLI offers synth, diff and deploy against CloudFormation
- **+** Stable modules follow semantic versioning
- **−** AWS only; deployment goes through CloudFormation
- **−** Experimental modules may have breaking API changes in any release
- **−** Not an AI project; no model or agent features
- **−** Collects anonymous telemetry; opt-out is documented separately

<sub>TypeScript · Needs AWS account, AWS CloudFormation, Node.js >= 20 · [Repo](https://github.com/aws/aws-cdk) · [📖 Docs ↗](https://docs.aws.amazon.com/cdk/latest/guide) · [🌐 Site ↗](https://constructs.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aws-cdk/)</sub>

<a name="goa"></a>
### #&#8288;12 [goa](https://github.com/goadesign/goa) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Nov 2026</sub>

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

<a name="django-rest-framework"></a>
### #&#8288;13 [django-rest-framework](https://github.com/encode/django-rest-framework) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · custom license · Nov 2026</sub>

**Toolkit for building web APIs on top of Django.**

Django REST framework adds serializers, viewsets, routers, and authentication and permission policies to Django for building HTTP APIs. Serializers work with both ORM models and plain data, and a browsable HTML interface renders each endpoint in the browser. It is a general-purpose API library, not an AI project or starter template.

- **+** Model and non-model serializers, viewsets and routers generate CRUD endpoints with little code
- **+** Browsable API renders endpoints in the browser with login and forms
- **+** Pluggable authentication and permission classes; OAuth1a and OAuth2 via optional packages
- **+** Can fall back to plain function-based views when generic views are too much
- **−** Requires Python 3.10+ and Django 5.2, 6.0 or 6.1; only latest patches supported
- **−** No built-in AI, model serving or LLM features
- **−** OAuth1a and OAuth2 need separate third-party packages
- **−** License is reported as NOASSERTION by detection tools

<sub>Python · Needs Python 3.10+, Django 5.2/6.0/6.1 · [Repo](https://github.com/encode/django-rest-framework) · [📖 Docs ↗](https://www.django-rest-framework.org/) · [🌐 Site ↗](https://www.django-rest-framework.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/django-rest-framework/)</sub>

<a name="go-zero"></a>
### #&#8288;14 [go-zero](https://github.com/zeromicro/go-zero) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Nov 2026</sub>

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

<a name="midway"></a>
### #&#8288;15 [midway](https://github.com/midwayjs/midway) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Nov 2026</sub>

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
### #&#8288;16 [elysia](https://github.com/elysiajs/elysia) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Nov 2026</sub>

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

<a name="falcon"></a>
### #&#8288;17 [falcon](https://github.com/falconry/falcon) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · Apache-2.0 · Nov 2026</sub>

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

<a name="full-stack-fastapi-template"></a>
### #&#8288;18 [full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Nov 2026</sub>

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

<a name="gofr"></a>
### #&#8288;19 [gofr](https://github.com/gofr-dev/gofr) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Nov 2026</sub>

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

<a name="django-ninja"></a>
### #&#8288;20 [django-ninja](https://github.com/vitalik/django-ninja) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · MIT · Nov 2026</sub>

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

<a name="serverless-application-model"></a>
### #&#8288;21 [serverless-application-model](https://github.com/aws/serverless-application-model) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · Apache-2.0 · Nov 2026</sub>

**CloudFormation macro that expands SAM templates into Lambda and API resources.**

The AWS SAM transform is a CloudFormation macro, enabled with `Transform: AWS::Serverless-2016-10-31`, that rewrites shorthand SAM resources such as `AWS::Serverless::Function` into full CloudFormation resources, including the IAM role. It is written in Python and published on PyPI as aws-sam-translator. Deployment and local testing go through the separate AWS SAM CLI.

- **+** Short SAM resources expand to a Lambda function plus IAM role with default tags
- **+** Standard CloudFormation transform, no extra service to run
- **+** Pairs with AWS SAM CLI for sync, local testing and debugging
- **+** Published on PyPI as aws-sam-translator
- **−** Targets AWS CloudFormation only; no support for other clouds
- **−** Not an AI project; README has no model or agent features
- **−** Deploying and local testing need the separate SAM CLI
- **−** Development setup requires Python 3.8+ and make

<sub>Python · Needs AWS CloudFormation, AWS SAM CLI, AWS Lambda · [Repo](https://github.com/aws/serverless-application-model) · [📖 Docs ↗](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/what-is-sam.html) · [🌐 Site ↗](https://aws.amazon.com/serverless/sam/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless-application-model/)</sub>

<a name="oapi-codegen"></a>
### #&#8288;22 [oapi-codegen](https://github.com/oapi-codegen/oapi-codegen) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.7k · Apache-2.0 · Nov 2026</sub>

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

<a name="playframework"></a>
### #&#8288;23 [playframework](https://github.com/playframework/playframework) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

**Stateless, non-blocking web framework for Java and Scala applications.**

Play is a JVM web framework for building REST-style web and mobile backends in Java or Scala. It uses a stateless, non-blocking architecture and includes asset compilers, JSON and WebSocket support, and built-in testing, with a "just hit refresh" development workflow. It has no AI features; it is a general-purpose web framework.

- **+** Supports both Java and Scala APIs, with separate documentation for each
- **+** Built-in JSON, WebSocket, asset compilation and testing support
- **+** Stateless, non-blocking design intended for predictable scaling
- **+** Apache-2.0 licensed, published to Maven Central, with recent releases
- **−** No AI, LLM or agent functionality; it is a generic web framework
- **−** Requires a JVM and Java or Scala build tooling
- **−** No Docker or compose setup in the repository
- **−** Not an AI starter, so it fits this list only loosely

<sub>Scala · Needs JVM, Java or Scala build tool · [Repo](https://github.com/playframework/playframework) · [📖 Docs ↗](https://www.playframework.com/documentation/latest/Installing) · [🌐 Site ↗](https://www.playframework.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/playframework/)</sub>

<a name="powertools-lambda-python"></a>
### #&#8288;24 [powertools-lambda-python](https://github.com/aws-powertools/powertools-lambda-python) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT-0 · Nov 2026</sub>

**Python toolkit for AWS Lambda: logging, tracing, metrics, event handlers, idempotency.**

A Python library of independent utilities for AWS Lambda functions. It covers structured JSON logging, X-Ray tracing, CloudWatch EMF metrics, routing for API Gateway, ALB, AppSync and Bedrock Agents, plus idempotency, batch processing, parameters and validation. Installs from PyPI or a public Lambda layer for x86_64 and arm64, and supports Python 3.10 to 3.14.

- **+** Each utility is independent, designed to keep cold start overhead low
- **+** Idempotency persists to DynamoDB, Redis or Valkey
- **+** Event handler generates OpenAPI schemas and Swagger UI; builds Bedrock Agents action groups
- **+** Public Lambda layer for x86_64 and arm64; ports exist for TypeScript, Java and .NET
- **−** Tied to AWS Lambda and AWS services; not usable as a general backend framework
- **−** Some utilities need extras, such as aws-lambda-powertools[parser] for Pydantic
- **−** Auth utility is marked alpha
- **−** Tracing and parameter utilities depend on X-Ray, Parameter Store, Secrets Manager or AppConfig

<sub>Python · Needs AWS Lambda, AWS X-Ray, CloudWatch, DynamoDB, Redis or Valkey (optional, idempotency), AWS KMS (optional, data masking) · [Repo](https://github.com/aws-powertools/powertools-lambda-python) · [📖 Docs ↗](https://docs.powertools.aws.dev/lambda/python/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/powertools-lambda-python/)</sub>

<a name="chi"></a>
### #&#8288;25 [chi](https://github.com/go-chi/chi) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 23k · MIT · Nov 2026</sub>

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

<a name="gqlgen"></a>
### #&#8288;26 [gqlgen](https://github.com/99designs/gqlgen) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<a name="flask"></a>
### #&#8288;27 [flask](https://github.com/pallets/flask) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (98) · Freshness: active (92) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · BSD-3-Clause · Oct 2026</sub>

**Minimal Python WSGI web framework built on Werkzeug and Jinja.**

Flask is a Python web framework that runs on WSGI and wraps Werkzeug for routing and Jinja for templating. It does not enforce dependencies or project layout, so you pick your own database, auth and AI libraries, with community extensions for more. It has no AI features of its own and is only a base for an API or web backend.

- **+** Small core with no enforced dependencies or project layout
- **+** Built on Werkzeug and Jinja, with a large community extension set
- **+** A working app is one decorated function; `flask run` serves it locally
- **+** BSD-3-Clause license with an active release and commit history
- **−** No built-in AI, model, or agent integration; you wire in every library
- **−** WSGI only per the README, so async and streaming need extra setup
- **−** No bundled auth, database layer or billing; each needs an extension
- **−** No Docker or compose files in the repo

<sub>Python · Needs Werkzeug, Jinja · [Repo](https://github.com/pallets/flask) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flask/)</sub>

<a name="go-clean-template"></a>
### #&#8288;28 [go-clean-template](https://github.com/evrone/go-clean-template) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Nov 2026</sub>

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

<a name="iris"></a>
### #&#8288;29 [iris](https://github.com/kataras/iris) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · BSD-3-Clause · Nov 2026</sub>

**Go web framework with typed routing, dependency injection and built-in middleware.**

Iris is a Go web framework for building APIs and websites. Version 14 uses generics for a compile-checked application builder, typed request binding with self-validation, MVC controllers and a central error map. It ships 31 built-in middleware, WebSockets, gRPC serving, view engines and an `ai` package that relays streamed model output over HTTP without a vendor SDK.

- **+** Typed path parameters ({id:uuid}, {n:int}) reject invalid input before the handler runs
- **+** 31 built-in middleware including JWT, rate limiting, sessions, CORS and accesslog
- **+** In-memory HTTP testing runs full-app tests without ports or network
- **+** Provider-agnostic `ai` package relays streamed text, tool-call fragments and usage
- **−** Go only; v12 applications need the migration guide to move to v14
- **−** A framework, not a starter: no auth, billing or database scaffold included
- **−** AI support is limited to relaying streamed output; no model or agent logic
- **−** Pug and Handlebars view engines live in a separate iris-contrib/views module

<sub>Go · Needs Go · [Repo](https://github.com/kataras/iris) · [📖 Docs ↗](https://pkg.go.dev/github.com/kataras/iris/v14@v14.0.1) · [🌐 Site ↗](https://iris-go.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/iris/)</sub>

<a name="functions-samples"></a>
### #&#8288;30 [functions-samples](https://github.com/firebase/functions-samples) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

**Official Cloud Functions for Firebase samples for each trigger type and use case.**

Google's collection of Cloud Functions for Firebase samples in Node (1st and 2nd gen) and Python (2nd gen), with some Dart quickstarts. It has minimal quickstarts for each trigger type (Firestore, Realtime Database, HTTPS, callable, Storage, Auth, Pub/Sub, Test Lab). It also has use-case samples such as Stripe, FCM, image moderation and BigQuery export.

- **+** Quickstarts for each trigger type, mostly in Node 2nd gen and Python
- **+** Maintained by Google under Apache-2.0
- **+** Includes unit-testing examples with Jest (JS and TypeScript) and Mocha
- **+** Use-case samples for Stripe, FCM, Cloud Vision, BigQuery and Google Sheets
- **−** Most use-case samples exist only for Node 1st gen
- **−** Every sample needs the paid Blaze billing plan to deploy
- **−** Separate sample folders, not a single deployable app
- **−** Only AI use is Vision API moderation and Translate; no LLM samples

<sub>JavaScript · Needs Firebase project (Blaze plan) · [Repo](https://github.com/firebase/functions-samples) · [📖 Docs ↗](https://firebase.google.com/docs/functions) · [🌐 Site ↗](https://firebase.google.com/features/functions) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/functions-samples/)</sub>

<a name="huma"></a>
### #&#8288;31 [huma](https://github.com/danielgtaylor/huma) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Nov 2026</sub>

**Go framework for REST/RPC APIs built from typed handlers and OpenAPI 3.1.**

Huma is a Go micro framework that runs on a router you choose (chi, the Go 1.22+ standard mux, and others) and generates OpenAPI 3.1 and JSON Schema from annotated Go input and output types. It validates requests, returns RFC 9457 errors, negotiates JSON or CBOR, and serves docs through Stoplight Elements. It has no AI features, so it fits this list only as a backend service template.

- **+** Works with existing routers and middleware, so services can adopt it one route at a time
- **+** Generates OpenAPI 3.1 and JSON Schema from Go types, so docs track the code
- **+** Built-in request validation, RFC 9457 problem+json errors, and per-operation body size limits
- **+** Optional CLI with port flag or env var, plus graceful shutdown
- **−** No AI, model or agent functionality; it is a general-purpose HTTP API framework
- **−** Requires Go 1.26 or newer
- **−** A library to import, not a starter app with auth, database or deployment files
- **−** Generated docs UI depends on Stoplight Elements

<sub>Go · Needs Go 1.26+, Go HTTP router such as chi (optional) · [Repo](https://github.com/danielgtaylor/huma) · [📖 Docs ↗](https://pkg.go.dev/github.com/danielgtaylor/huma/v2) · [🌐 Site ↗](https://huma.rocks/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huma/)</sub>

<a name="full-stack-ai-agent-template"></a>
### #&#8288;32 [full-stack-ai-agent-template](https://github.com/vstorm-co/full-stack-ai-agent-template) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="kemal"></a>
### #&#8288;33 [kemal](https://github.com/kemalcr/kemal) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Nov 2026</sub>

**Sinatra-style web framework for Crystal with routing, WebSockets and JSON.**

Kemal is a web framework for the Crystal language with a Sinatra-like routing DSL covering all HTTP verbs, including QUERY. It includes WebSocket routes, ECR templates, static file serving and composable middleware, and compiles to a single native binary. It does not impose an ORM or project layout; sessions come from the separate kemal-session shard.

- **+** Built-in WebSocket routes and ECR templates, no extra shards needed
- **+** Compiles to a single native binary (~2 MB per README)
- **+** No forced ORM or layout; works with any Crystal database library
- **+** Returns 405 with an Allow header for wrong-method requests, per RFC 9110
- **−** Crystal only; requires Crystal 1.19+ and a compile step
- **−** Sessions need the separate kemal-session shard
- **−** General web framework with no LLM or model integration included
- **−** README benchmark figures are self-reported, with no methodology given

<sub>Crystal · Needs Crystal 1.19+ · [Repo](https://github.com/kemalcr/kemal) · [📖 Docs ↗](http://kemalcr.com/guide/) · [🌐 Site ↗](http://kemalcr.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kemal/)</sub>

<a name="api-platform-core"></a>
### #&#8288;34 [core](https://github.com/api-platform/core) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

**PHP library for building hypermedia REST and GraphQL APIs on Symfony.**

API Platform Core is a PHP library that builds REST and GraphQL APIs from resource definitions. A bundle integrates it with Symfony. It supports JSON-LD, Hydra, OpenAPI v2 and v3, JSON:API, HAL and Problem Details, and is one component of the wider API Platform framework.

- **+** Supports JSON-LD, Hydra, OpenAPI v2/v3, JSON:API, HAL and Problem Details
- **+** Serves both hypermedia REST and GraphQL APIs from one library
- **+** Symfony bundle included for direct integration
- **+** MIT license; last release 2026-11-06
- **−** No AI or model features; it is a general API framework
- **−** PHP only; the documented integration is Symfony-specific
- **−** README is brief; features and setup live in the external docs
- **−** A library to add to a project, not a forkable starter

<sub>PHP · Needs PHP, Symfony (optional, via bundle) · [Repo](https://github.com/api-platform/core) · [📖 Docs ↗](https://api-platform.com/docs/core) · [🌐 Site ↗](https://api-platform.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/api-platform-core/)</sub>

<a name="go-openai"></a>
### #&#8288;35 [go-openai](https://github.com/sashabaranov/go-openai) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Sep 2026</sub>

**Unofficial Go client library for the OpenAI API.**

A Go module that wraps the OpenAI API: Responses (with streaming and previous-response chaining), Chat Completions, embeddings, images, audio, moderation, files, fine-tuning, batches and vector stores. The base URL is configurable for compatible endpoints, and there is a default Azure OpenAI config. It is a library to import into Go services, not a runnable app.

- **+** Covers Responses, Chat Completions, embeddings, images, audio, moderation, files, fine-tuning and batches
- **+** Model IDs accepted as strings, so new models work before constants are added
- **+** Configurable BaseURL and DefaultAzureConfig for compatible endpoints and Azure OpenAI
- **+** Runnable examples for Responses, tools, images and speech to text
- **−** Library only: no server, UI or agent loop included
- **−** Unofficial, so it can lag behind OpenAI API changes
- **−** Assistants API support is described as legacy
- **−** Targets the OpenAI API shape; other providers only work through compatible endpoints

<sub>Go, OpenAI GPT-6 and GPT-5 series, GPT-4o, OpenAI-compatible endpoints, Azure OpenAI · Needs OpenAI API key, Go 1.18+ · [Repo](https://github.com/sashabaranov/go-openai) · [📖 Docs ↗](https://pkg.go.dev/github.com/sashabaranov/go-openai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-openai/)</sub>

<a name="podinfo"></a>
### #&#8288;36 [podinfo](https://github.com/stefanprodan/podinfo) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · Apache-2.0 · Nov 2026</sub>

**Go microservice for testing Kubernetes deployments, probes, and fault handling.**

Podinfo is a small Go web service that exposes HTTP and gRPC endpoints for health probes, Prometheus metrics, JWT issuing, Redis caching, fault injection, and echo or delay responses. CNCF projects such as Flux and Flagger use it for end-to-end tests and workshops. It installs with Timoni, Helm, Kustomize, or a plain Docker run on port 9898. It contains no AI or model features.

- **+** Fault injection, configurable delay, panic and status-code endpoints for testing circuit breakers and rollouts
- **+** Readiness and liveness probes, graceful shutdown, Prometheus and OpenTelemetry instrumentation built in
- **+** Installs via Timoni, Helm, Kustomize or docker run; multi-arch image signed with cosign
- **+** Optional SPIFFE mTLS with X.509 SVIDs from the Workload API
- **−** Not an AI project; no model, agent, or LLM functionality
- **−** A test and demo workload, not a starter for real application logic
- **−** Cache endpoints need a separate Redis instance
- **−** Needs Kubernetes v1.23 or newer for the documented installs

<sub>Go · Needs Kubernetes v1.23+ (for Helm, Kustomize, Timoni installs), Redis (optional, for /cache endpoints), SPIRE agent (optional, for SPIFFE mTLS) · Docker · [Repo](https://github.com/stefanprodan/podinfo) · [📖 Docs ↗](https://fluxcd.io/flux/get-started/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/podinfo/)</sub>

<a name="ultimo"></a>
### #&#8288;37 [ultimo](https://github.com/ultimo-rs/ultimo) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 554 · MIT · Nov 2026</sub>

**Rust web framework on Hyper and Tokio that generates TypeScript clients.**

Ultimo is a Rust web framework built on Hyper and Tokio that serves REST routes and JSON-RPC 2.0 from one app. It generates a typed TypeScript client from the Rust API definitions. Auth, sessions, WebSockets, SSE, Prometheus metrics, OpenTelemetry, Redis stores and SQLx/Diesel database integration are opt-in Cargo features.

- **+** Generates a typed TypeScript client from Rust RPC definitions, avoiding hand-written types
- **+** REST and JSON-RPC 2.0 (batch, notifications) served from the same app
- **+** Built-in OAuth2/OIDC, JWT, API-key and CSRF middleware; unsafe code forbidden
- **+** All features opt-in via Cargo flags; CLI scaffolds, hot-reloads and builds releases
- **−** Rust only; backend code cannot be written in other languages
- **−** Requires Rust 1.86+, and the redis feature needs Rust 1.88+
- **−** Not AI-specific: no model or agent integration, only docs aimed at coding agents
- **−** Version 0.10, so the API may still change; stability policy not stated

<sub>Rust · Needs Rust 1.86+, Redis (optional), PostgreSQL/MySQL/SQLite (optional) · [Repo](https://github.com/ultimo-rs/ultimo) · [▶️ Demo ↗](https://basic-example-v4wi.onrender.com/) · [📖 Docs ↗](https://docs.ultimo.dev) · [🌐 Site ↗](https://ultimo.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ultimo/)</sub>

<a name="gin"></a>
### #&#8288;38 [gin](https://github.com/gin-gonic/gin) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (99) · Freshness: active (93) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 90k · MIT · Oct 2026</sub>

**Go HTTP web framework with a zero-allocation router and middleware.**

Gin is a Go HTTP framework built on a customized httprouter. It provides route grouping, middleware, JSON binding and validation, panic recovery, and rendering for JSON, XML and HTML templates. It is a general-purpose library for REST APIs and microservices, not AI-specific, but it can serve as the base for a backend that exposes models or agents over HTTP.

- **+** Router reports 0 B/op and 0 allocs/op in the README's GitHub API benchmark
- **+** Built-in recovery middleware keeps handler panics from crashing the server
- **+** gin-contrib middleware covers JWT, sessions, CORS, rate limiting and tracing
- **+** Docs in 11 languages, plus a go.dev tutorial and a runnable examples repository
- **−** Requires Go 1.26 or newer
- **−** No AI-specific features such as model clients, streaming helpers or agent tooling
- **−** Aero and HttpRouter benchmark faster than Gin in the README's own table
- **−** Library only: auth and other extras come from separate contrib middleware

<sub>Go · Needs Go 1.26+ · [Repo](https://github.com/gin-gonic/gin) · [📖 Docs ↗](https://gin-gonic.com/en/docs/) · [🌐 Site ↗](https://gin-gonic.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gin/)</sub>

<a name="microservices-demo"></a>
### #&#8288;39 [microservices-demo](https://github.com/googlecloudplatform/microservices-demo) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;40 [litestar](https://github.com/litestar-org/litestar) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · MIT · Nov 2026</sub>

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

<a name="javalin"></a>
### #&#8288;41 [javalin](https://github.com/javalin/javalin) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · Apache-2.0 · Oct 2026</sub>

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

<a name="middy"></a>
### #&#8288;42 [middy](https://github.com/middyjs/middy) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Oct 2026</sub>

**Middleware engine for AWS Lambda handlers on Node.js.**

Middy wraps AWS Lambda handlers in a middleware chain so parsing, validation, auth, error handling and AWS service integration live outside business logic. The core depends only on @middy/util, and 56 official packages cover API Gateway, SQS, S3, DynamoDB, SNS, EventBridge, Kinesis, Kafka and WebSockets. It is a general Lambda library with no AI-specific features.

- **+** Small core with only @middy/util as a dependency and no AWS SDK bundled
- **+** 56 official middleware packages for common event sources and AWS services
- **+** Built-in TypeScript types plus routers for HTTP, WebSocket and CloudFormation resources
- **+** Supports Lambda response streaming and durable functions
- **−** Lambda-only; handlers are not portable to other serverless platforms
- **−** Requires Node.js 24 or newer and ESM
- **−** No AI or model features; it is general Lambda plumbing

<sub>JavaScript · Needs AWS Lambda, Node.js >= 24 · [Repo](https://github.com/middyjs/middy) · [📖 Docs ↗](https://middy.js.org/docs/intro/getting-started) · [🌐 Site ↗](https://middy.js.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/middy/)</sub>

<a name="quart"></a>
### #&#8288;43 [quart](https://github.com/pallets/quart) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Sep 2026</sub>

**Async Python web framework, a Flask reimplementation on asyncio.**

Quart is an asyncio reimplementation of Flask for rendering templates, serving JSON APIs and WebSockets, and streaming request and response bodies. It keeps Flask's API, so migrating is mostly renaming imports from flask to quart and adding async and await. It is a general web framework with no AI-specific features.

- **+** Flask-compatible API; migration is mostly find-and-replace plus async/await
- **+** Native WebSocket and streaming request/response support
- **+** Several Flask extensions work with Quart, plus its own extension ecosystem
- **+** Installs with pip; `quart run` starts a dev server on port 5000
- **−** No built-in AI, model or agent integration; you wire that yourself
- **−** Dev server is not for production; deployment needs a separate setup
- **−** Only some Flask extensions work, so compatibility needs checking per extension
- **−** No auth, database or billing scaffolding included

<sub>Python · [Repo](https://github.com/pallets/quart) · [📖 Docs ↗](https://quart.palletsprojects.com/en/latest/tutorials/deployment.html) · [🌐 Site ↗](https://quart.palletsprojects.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/quart/)</sub>

<a name="cloud-foundation-fabric"></a>
### #&#8288;44 [cloud-foundation-fabric](https://github.com/googlecloudplatform/cloud-foundation-fabric) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Nov 2026</sub>

**Terraform modules and landing-zone blueprints for Google Cloud organizations.**

A repository of Terraform modules for Google Cloud covering projects, networking, compute, data, security and serverless, plus FAST, a reference landing zone for bootstrapping an organization. It is meant to be cloned and forked into your own repositories. A small AI section has modules for AI Applications and Gemini Enterprise Agent Platform (Agent Gateway, Agent Runtime, Workbench).

- **+** Modules stay close to provider resources and handle IAM together with resource creation
- **+** Modules have no side effects, such as external commands, so they are easy to fork and audit
- **+** FAST provides a reference organization design with a Terraform implementation
- **+** Wide module coverage: foundational, networking, compute, data, security and serverless
- **−** Google Cloud only; the modules do not target other clouds
- **−** AI coverage is limited to four modules, with no application starters
- **−** Designed to be forked and maintained by you, not consumed as a versioned dependency
- **−** Not an app or agent starter, so it is a poor fit for AI product prototypes

<sub>HCL · Needs Terraform, Google Cloud account · [Repo](https://github.com/googlecloudplatform/cloud-foundation-fabric) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloud-foundation-fabric/)</sub>

<a name="agent-service-toolkit"></a>
### #&#8288;45 [agent-service-toolkit](https://github.com/joshuac215/agent-service-toolkit) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Nov 2026</sub>

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

<a name="userver"></a>
### #&#8288;46 [userver](https://github.com/userver-framework/userver) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Nov 2026</sub>

**Asynchronous C++ framework for microservices with built-in database and protocol drivers.**

userver is a C++ framework for writing asynchronous services. Blocking I/O suspends a coroutine rather than the OS thread, so a small thread pool handles many concurrent requests. It ships drivers for PostgreSQL, MongoDB, Redis/Valkey, ClickHouse, MySQL/MariaDB, YDB and SQLite, plus HTTP, gRPC, Kafka and AMQP. It is a general backend framework with no AI-specific features.

- **+** Coroutine-based I/O keeps thread count small without callback-style code
- **+** Async drivers for PostgreSQL, MongoDB, Redis, ClickHouse, MySQL, YDB, SQLite and more
- **+** Protocols include HTTP/1.1, HTTP/2, gRPC, Kafka, AMQP, WebSocket and TLS
- **+** Runtime config changes, deadline propagation and congestion control are built in
- **−** C++ only, so it needs a C++ toolchain and build setup
- **−** No AI or model-serving functionality; it is a general service framework
- **−** Large API surface with many components to learn before the first service

<sub>C++ · Needs PostgreSQL (optional), MongoDB (optional), Redis/Valkey (optional), ClickHouse (optional), Kafka (optional) · [Repo](https://github.com/userver-framework/userver) · [📖 Docs ↗](https://userver.tech/de/d6a/md_en_2index.html) · [🌐 Site ↗](https://userver.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/userver/)</sub>

<a name="azure-agent-landing-zone"></a>
### #&#8288;47 [agent-landing-zone](https://github.com/azure/agent-landing-zone) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · MIT · Nov 2026</sub>

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

<a name="hyperf"></a>
### #&#8288;48 [hyperf](https://github.com/hyperf/hyperf) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · MIT · Nov 2026</sub>

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

<a name="monid"></a>
### #&#8288;49 [monid](https://github.com/monid-ai/monid) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Nov 2026</sub>

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

<a name="chalice"></a>
### #&#8288;50 [chalice](https://github.com/aws/chalice) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

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

<a name="dropwizard"></a>
### #&#8288;51 [dropwizard](https://github.com/dropwizard/dropwizard) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · Apache-2.0 · Nov 2026</sub>

**Java framework bundling Jetty, Jersey and Jackson for REST services.**

Dropwizard is a Java library that wires Jetty, Jersey, Jackson, Logback, Hibernate Validator, Metrics, JDBI, Hibernate and Liquibase into one opinionated stack for HTTP and REST services. It has no AI features. It fits this list only as a general backend framework you could put in front of a model or agent API.

- **+** Bundles Jetty, Jersey, Jackson, Logback and Metrics in one integrated stack
- **+** Includes Hibernate Validator for validation and Liquibase for schema migrations
- **+** Offers both JDBI and Hibernate for database access
- **+** Published on Maven Central with reproducible builds and Javadocs
- **−** No AI, LLM or agent functionality included
- **−** JVM only; requires Java and a build tool
- **−** Opinionated library choices limit swapping the HTTP or JSON stack
- **−** No Docker image or compose file in the repository

<sub>Java · Needs Java · [Repo](https://github.com/dropwizard/dropwizard) · [📖 Docs ↗](https://www.dropwizard.io/en/stable/) · [🌐 Site ↗](http://www.dropwizard.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dropwizard/)</sub>

<a name="deepkit"></a>
### #&#8288;52 [deepkit](https://github.com/marcj/deepkit) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Nov 2026</sub>

**TypeScript framework with runtime types for validation, ORM, HTTP and RPC.**

Deepkit preserves TypeScript types at runtime through a compiler plugin, so one type definition drives validation, serialization, database mapping, HTTP routing, RPC and dependency injection. It ships as 40+ npm packages, including an ORM for PostgreSQL, MySQL, SQLite and MongoDB, and a binary RPC over WebSocket/TCP. It is a general backend framework with no AI features.

- **+** One type definition serves validation, serialization, ORM, HTTP and DI, with no schema duplication
- **+** Modular: 40+ independent packages, so the HTTP router or injector can be used alone
- **+** ORM supports PostgreSQL, MySQL, SQLite and MongoDB
- **+** Quick start via npm init @deepkit/app@latest
- **−** Depends on a type-compiler transformer; contributors must run a postinstall step to build it
- **−** No AI or LLM features; it is a general backend framework, not an AI starter
- **−** Some integrations (OpenAPI, GraphQL, Remix, Stripe) are community packages outside this repo
- **−** Bundlers like Webpack and Nx need separate setups to apply the type compiler

<sub>TypeScript · Needs Node.js, PostgreSQL, MySQL, SQLite or MongoDB (optional) · Docker · [Repo](https://github.com/marcj/deepkit) · [📖 Docs ↗](https://deepkit.io/documentation/introduction) · [🌐 Site ↗](https://deepkit.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepkit/)</sub>

<a name="typescript-express-starter"></a>
### #&#8288;53 [typescript-express-starter](https://github.com/ljlm0402/typescript-express-starter) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

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

<a name="fastapi-langgraph-agent-production-ready-template"></a>
### #&#8288;54 [fastapi-langgraph-agent-production-ready-template](https://github.com/wassim249/fastapi-langgraph-agent-production-ready-template) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

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
### #&#8288;55 [api-platform](https://github.com/api-platform/api-platform) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Nov 2026</sub>

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

<a name="amber"></a>
### #&#8288;56 [amber](https://github.com/amberframework/amber) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Nov 2026</sub>

**Rails- and Phoenix-inspired web framework for the Crystal language.**

Amber is a server-side web application framework written in Crystal, modeled on Rails, Phoenix, Kemal and Hanami. It ships an `amber` CLI for generating and running apps and is added to a project as a shard. It has no AI features. The 1.x branch only takes fixes for apps that stop compiling or running, and new work goes to Amber V2.

- **+** Compiled Crystal language with Rails-like conventions and a project generator CLI
- **+** Installs via Homebrew, Arch AUR, source build, or as a shard dependency
- **+** MIT licensed, with TechEmpower benchmark results linked (Round 18, 2019)
- **+** Supports PostgreSQL, MySQL and SQLite client libraries per the install packages
- **−** 1.x branch is fix-only; new development moved to Amber V2 in a separate repo
- **−** Linux install is from source only, with a long list of system libraries
- **−** No AI, model or agent features; it is a general web framework
- **−** Benchmark link is from 2019 and the README has no current numbers

<sub>Crystal · Needs Crystal, libreadline, libsqlite3, libpq, libmysqlclient, libssl, libyaml, libpcre3, libevent · Docker · [Repo](https://github.com/amberframework/amber) · [📖 Docs ↗](https://docs.amberframework.org/amber) · [🌐 Site ↗](https://amberframework.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/amber/)</sub>

<a name="backend"></a>
### #&#8288;57 [backend](https://github.com/prod-forge/backend) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 485 · MIT · Nov 2026</sub>

**Production-ready NestJS Todo API with a 16-chapter guide on CI/CD and observability.**

A NestJS, Prisma and PostgreSQL API, using a Todo app as the domain, that is taken from first commit to production and documented in a 16-chapter guide. It covers migrations run as a one-off ECS task before deploy, rollback to one of the last three task revisions, graceful SIGTERM draining, and a local Prometheus, Grafana, Loki and Tempo stack. Tests include 593 unit tests and e2e tests against PostgreSQL and Redis in Testcontainers.

- **+** Migrations run as a separate ECS task; the new version does not start if they fail
- **+** One trace ID shared across logs, Sentry events and Tempo traces
- **+** Redis is optional: cache and rate limiting fall back when it is down
- **+** E2E tests run against real PostgreSQL and Redis via Testcontainers; OpenAPI contract is committed
- **−** Deploy and rollback workflows target AWS ECS; infrastructure lives in a separate Terraform repo
- **−** Todo domain only; no billing or AI features, so it is a reference rather than a product base
- **−** Setup needs Node 24.15+, Docker Compose 2.24+ and jq, plus manual .env edits
- **−** Web and mobile client are in a separate repository

<sub>TypeScript · Needs PostgreSQL, Redis, Docker Compose, Prometheus, Grafana, Loki, Tempo, Sentry, AWS ECS · Docker · [Repo](https://github.com/prod-forge/backend) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/backend/)</sub>

<a name="taotao-cloud-project"></a>
### #&#8288;58 [taotao-cloud-project](https://github.com/shuigedeng/taotao-cloud-project) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 379 · Apache-2.0 · Oct 2026</sub>

**Spring Cloud Alibaba microservice scaffold with a B2B2C mall and big-data modules.**

A Java monorepo on Spring Boot 4.1.2, Spring Cloud Alibaba and JDK 25, built with Gradle. It bundles Nacos, Sentinel, Seata, OAuth2/JWT auth, multi-tenancy, code generation and a gateway, plus a B2B2C mall, a Taro/React front end and Flink/Doris/Paimon/Hudi warehouse modules. The shared starter components are listed as not yet open source.

- **+** Wide middleware coverage: Nacos, Sentinel, Seata, RocketMQ, Kafka, xxl-job, Flowable
- **+** Current stack: Spring Boot 4.1.2, JDK 25, Gradle 9.8.2
- **+** Includes multi-tenancy, RBAC and many third-party login methods
- **+** Documents Shell, Docker, Docker Compose, Kubernetes and CI/CD deployment
- **−** Core taotao-cloud-starter components are marked as not yet open source
- **−** Demo servers have expired; admin, seller and open platform are 5-15% complete
- **−** Single maintainer; README is mainly in Chinese
- **−** Very broad scope; the ai module is not described, so AI features are unclear

<sub>Java · Needs JDK 25, Gradle 9.8.2, Nacos, MySQL, Redis, RocketMQ, Kafka, Elasticsearch · [Repo](https://github.com/shuigedeng/taotao-cloud-project) · [📖 Docs ↗](https://docs.taotaocloud.top) · [🌐 Site ↗](https://start.taotaocloud.top/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taotao-cloud-project/)</sub>

<a name="fastcrud"></a>
### #&#8288;59 [fastcrud](https://github.com/benavlabs/fastcrud) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

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

<a name="pyramid"></a>
### #&#8288;60 [pyramid](https://github.com/pylons/pyramid) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · custom license · Nov 2026</sub>

**Small Python WSGI web framework with explicit route and view configuration.**

Pyramid is a general-purpose Python web framework built on WSGI. Applications use a Configurator to map routes to view callables, and the README example serves one on port 6543 with wsgiref. It has no AI features, so it fits this list only as a generic backend to build on.

- **+** Small core with explicit Configurator-based route and view setup
- **+** Runs on any WSGI server; the README example uses stdlib wsgiref
- **+** Documentation on Read the Docs plus a separate add-on ecosystem
- **+** Active development: last commit 2026-11-10, CI badge on main
- **−** No built-in AI, model or agent integration
- **−** No tagged release listed in the repository metadata
- **−** License is the BSD-derived Repoze Public License, detected as NOASSERTION
- **−** README mentions WSGI only, with no ASGI or async support described

<sub>Python · Needs Python · [Repo](https://github.com/pylons/pyramid) · [📖 Docs ↗](https://docs.pylonsproject.org/projects/pyramid/en/main) · [🌐 Site ↗](https://trypyramid.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pyramid/)</sub>

<a name="golang-gin-realworld-example-app"></a>
### #&#8288;61 [golang-gin-realworld-example-app](https://github.com/realworld-apps/golang-gin-realworld-example-app) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Nov 2026</sub>

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

<a name="eve"></a>
### #&#8288;62 [eve](https://github.com/pyeve/eve) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · custom license · Nov 2026</sub>

**Python REST API framework on Flask with MongoDB support.**

Eve is a Python framework built on Flask that exposes a database as a configurable REST API. Resources are defined in a settings.py file and the app starts with a few lines of code. It supports MongoDB natively and SQL backends through community extensions.

- **+** CRUD, filtering, sorting, pagination and HATEOAS configured from a settings file
- **+** Built-in validation, authentication, rate limiting, CORS and event hooks
- **+** Document and API versioning, plus conditional requests for concurrency control
- **+** Read-only by default, so write access is enabled per resource
- **−** No AI or model-serving features; it is a general REST framework
- **−** SQL support relies on community extensions, not the core
- **−** Only MongoDB is supported natively
- **−** No tagged release listed; license detected as NOASSERTION, README says BSD

<sub>Python · Needs MongoDB, Flask · [Repo](https://github.com/pyeve/eve) · [🌐 Site ↗](http://python-eve.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eve/)</sub>

<a name="generative-ai-project-template"></a>
### #&#8288;63 [generative-ai-project-template](https://github.com/aminedjeghri/generative-ai-project-template) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 118 · MIT · Nov 2026</sub>

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

<a name="examples"></a>
### #&#8288;64 [examples](https://github.com/vercel/examples) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (54) · Freshness: active (86) · Maintenance: patchy (37) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Nov 2026</sub>

**Vercel's collection of Next.js and edge example apps and reference solutions.**

Monorepo of example projects maintained by Vercel, split into solutions (demos and reference architectures) and starter apps meant as starting points. Many entries feed Vercel's template gallery and can be deployed with a Deploy Button. The README covers contribution rules and does not describe any AI-specific features.

- **+** Maintained by Vercel; last commit 2026-11-06
- **+** Examples share one UI package and a consistent README and .env.example layout
- **+** Plop script (pnpm new-example) scaffolds new examples
- **+** MIT licensed
- **−** Not a single app; each example has its own dependencies and setup
- **−** README does not point to which examples involve AI or models
- **−** Examples are oriented to deployment on Vercel
- **−** Mostly Next.js, so less useful for other frameworks

<sub>TypeScript · Needs pnpm, Next.js, Vercel · [Repo](https://github.com/vercel/examples) · [📖 Docs ↗](https://vercel.com/docs) · [🌐 Site ↗](https://vercel.com/templates) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/examples/)</sub>

<a name="node-typescript-boilerplate"></a>
### #&#8288;65 [node-typescript-boilerplate](https://github.com/jsynowiec/node-typescript-boilerplate) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (39) · Freshness: active (100) · Maintenance: patchy (35) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

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

<a name="ack-nestjs-boilerplate"></a>
### #&#8288;66 [ack-nestjs-boilerplate](https://github.com/andrechristikan/ack-nestjs-boilerplate) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 704 · MIT · Sep 2026</sub>

**NestJS API boilerplate with JWT, OAuth, 2FA, RBAC and workspaces.**

NestJS 12 and TypeScript API starter using Prisma on MongoDB (replica set required), Redis and BullMQ. It ships stateful JWT sessions, Google and Apple sign-in, TOTP 2FA, RBAC with CASL policies, multi-workspace tenancy, feature flags, and email, push and in-app notifications. The README targets enterprise apps, auth services, mobile backends and SaaS MVPs.

- **+** Auth included: ES256/ES512 JWT, Redis sessions, Google/Apple login, TOTP 2FA with backup codes
- **+** Workspace-scoped projects, invites, feature flags and CASL policies already wired
- **+** Notifications via AWS SES, Firebase FCM and BullMQ workers, plus S3 presigned uploads
- **+** Zod-validated OpenAPI 3.1 docs, Vitest suite, Sentry and 30+ guides
- **−** MongoDB only; PostgreSQL support is still a TODO item
- **−** Requires a MongoDB replica set for Prisma transactions
- **−** Schema sync uses prisma db push, with no migration history
- **−** Protection decorators must be applied in a fixed order or guards misbehave

<sub>TypeScript · Needs MongoDB 8+ (replica set), Redis 8+, Node.js >= 24.15.0, pnpm, AWS S3, AWS SES, Firebase FCM, Sentry (optional), HashiCorp Vault (optional) · GitHub template · env example file · sign-in: Passport · [Repo](https://github.com/andrechristikan/ack-nestjs-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ack-nestjs-boilerplate/)</sub>

<a name="genlayer-project-boilerplate"></a>
### #&#8288;67 [genlayer-project-boilerplate](https://github.com/genlayerlabs/genlayer-project-boilerplate) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: widely used (83) · Freshness: recent (67) · Maintenance: weak (18) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Jun 2026</sub>

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

<a name="springcloud"></a>
### #&#8288;68 [springcloud](https://github.com/zhoutaoo/springcloud) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · Apache-2.0 · Sep 2026</sub>

**Spring Cloud microservice scaffold with RBAC, OAuth2 gateway and Nacos config.**

Aggregate Maven project for Spring Cloud microservices, with base apps for user, role and organization management. It uses Nacos for registry and config, Spring Cloud Gateway, Spring Security OAuth2 with JWT, Sentinel and OpenFeign. The README says the scaffold was refactored into Opensabre, and tells users to use that newer framework. It has no AI features.

- **+** Covers registry, config, gateway, OAuth2 JWT, Sentinel fault tolerance and Feign in one stack
- **+** Unified REST response and exception handling, with knife4j and Swagger 3 docs by default
- **+** Registers all REST URLs as permission resources at startup for central authorization
- **+** Log trace, sensitive-data masking and encrypted config items are built in
- **−** README tells users to move to the newer Opensabre framework
- **−** Object storage (Minio) and data permissions are marked in progress
- **−** No Docker or compose files detected; Nacos, RabbitMQ and a database must be set up manually
- **−** No AI or LLM functionality; documentation is mostly in Chinese

<sub>Needs Nacos, RabbitMQ, Sentinel, Maven, SQL database (type unknown) · [Repo](https://github.com/zhoutaoo/springcloud) · [📖 Docs ↗](https://opensabre.github.io/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/springcloud/)</sub>

<a name="wild-workouts-go-ddd-example"></a>
### #&#8288;69 [wild-workouts-go-ddd-example](https://github.com/threedotslabs/wild-workouts-go-ddd-example) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (61) · Freshness: recent (70) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Aug 2026</sub>

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

<a name="jupiter"></a>
### #&#8288;70 [jupiter](https://github.com/douyu/jupiter) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (51) · Freshness: active (82) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Sep 2026</sub>

**Go microservice framework with service governance, CLI scaffolding and a console.**

Jupiter is a Go framework for building governed microservices, used in production at Douyu. A CLI toolkit scaffolds projects from the jupiter-layout template and runs them from a TOML config. The separate Juno system provides the governance console, with a hosted demo.

- **+** Used in production at Douyu for years
- **+** CLI scaffolds a project from jupiter-layout and runs it from a TOML config
- **+** Companion Juno console for governance, with a public demo login
- **+** Apache-2.0 licensed, with Go test and codecov badges
- **−** Not an AI project; no model or LLM features
- **−** Main documentation is in Chinese
- **−** Governance console lives in a separate repo (Juno)
- **−** Quick start needs Docker Compose for the example's dependencies

<sub>Go · Needs Go >= 1.19, Docker · [Repo](https://github.com/douyu/jupiter) · [📖 Docs ↗](http://jupiter.douyu.com/) · [🌐 Site ↗](http://jupiter.douyu.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jupiter/)</sub>

<a name="connexion"></a>
### #&#8288;71 [connexion](https://github.com/spec-first/connexion) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (52) · Freshness: active (81) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Nov 2026</sub>

**Python framework that builds REST APIs from an OpenAPI specification.**

Connexion is a Python web framework where the OpenAPI (or Swagger) spec drives the API. It registers routes from operationId, validates requests and responses, parses parameters into function arguments, serializes return values and serves a Swagger UI console. It runs standalone (AsyncApp or FlaskApp) or as middleware around an existing ASGI or WSGI app.

- **+** Routes, parameter parsing and validation come from the OpenAPI spec, no route decorators
- **+** Works standalone or as middleware over any ASGI or WSGI framework
- **+** Authentication is handled separately from application logic
- **+** CLI command `connexion run openapi.yaml` runs and mocks a spec
- **−** Not AI-specific; a general API framework with no model or agent integration
- **−** The OpenAPI spec must be written before the code
- **−** Swagger UI, uvicorn and Flask support need optional extras
- **−** Connexion 3 changed the app model, so upgrading from 2.x takes work

<sub>Python · Needs Python, OpenAPI specification, uvicorn (optional), Flask (optional) · [Repo](https://github.com/spec-first/connexion) · [📖 Docs ↗](https://connexion.readthedocs.io/en/stable/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/connexion/)</sub>

<a name="robyn"></a>
### #&#8288;72 [robyn](https://github.com/sparckles/robyn) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (65) · Freshness: active (96) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.4k · BSD-2-Clause · Aug 2026</sub>

**Async Python web framework with a Rust runtime, with MCP and agent routing.**

Robyn is a Python web framework (3.10+) whose HTTP runtime is written in Rust and exposed through PyO3. It supports sync and async handlers, dynamic routing, WebSockets, SSE streaming, middleware, dependency injection and automatic OpenAPI generation. It also lists built-in agent routing and an MCP server mode, which makes it usable as a backend for AI apps rather than an AI project itself.

- **+** Rust runtime with multi-process and multi-worker scaling set via --processes and --workers flags
- **+** Ships WebSockets, SSE streaming, OpenAPI generation, auth, CORS and dependency injection in the framework
- **+** Installs with pip or conda-forge; hello-world app is a few lines
- **+** Includes MCP server support and agent routing for exposing AI tools
- **−** Building from source needs a Rust toolchain and a C compiler
- **−** io-uring support is marked experimental and needs a custom maturin build
- **−** AI agent and MCP features are listed in one line each, with no examples
- **−** Pydantic and Jinja2 support need the optional robyn[all] install

<sub>Python · Needs Python >=3.10, Rust (source builds only) · [Repo](https://github.com/sparckles/robyn) · [📖 Docs ↗](https://robyn.tech/documentation) · [🌐 Site ↗](https://robyn.tech) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/robyn/)</sub>

<a name="go-zero-looklook"></a>
### #&#8288;73 [go-zero-looklook](https://github.com/mikaelemmmm/go-zero-looklook) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (55) · Freshness: recent (70) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Sep 2026</sub>

**go-zero microservice example app with Kafka, asynq, tracing and CI/CD.**

A reference microservice backend in Go on the go-zero framework. HTTP API services aggregate gRPC RPC services, with message queue, delay queue and scheduled-task code under app/. It also wires in logging (filebeat, Kafka, go-stash, Elasticsearch), Prometheus, Jaeger, DTM and a GitLab/Jenkins/Harbor/k8s deploy flow. It has no AI features.

- **+** Covers API, RPC, Kafka pub/sub, asynq delayed jobs, logging, metrics and tracing in one repo
- **+** Compose dev setup uses direct service links, so no etcd or Nacos is needed locally
- **+** Includes goctl code-generation templates and scripts, plus modd hot-reload config
- **+** Documents a Jenkins, GitLab, Harbor and Kubernetes deployment pipeline
- **−** Contains no AI or model integration, so it is a loose fit for an AI starter list
- **−** Large middleware stack (Kafka, Elasticsearch, Jaeger, MySQL, Redis) is heavy to run locally
- **−** Dev image is based on golang 1.17.7-alpine, which is old
- **−** DTM distributed transactions are listed but not yet used in the project

<sub>Go · Needs MySQL, Redis, Kafka, Elasticsearch, Docker Compose · [Repo](https://github.com/mikaelemmmm/go-zero-looklook) · [📖 Docs ↗](https://github.com/Mikaelemmmm/go-zero-looklook/tree/main/doc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-zero-looklook/)</sub>

<a name="whatsmars"></a>
### #&#8288;74 [whatsmars](https://github.com/javahongxi/whatsmars) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · Apache-2.0 · Nov 2026</sub>

**Java sample modules for Spring Boot, Dubbo, Redis, RocketMQ and Elasticsearch.**

A multi-module Java 17+ repository of example code for the Spring Boot 3.5.x ecosystem: Dubbo 3.3, Redis clients, message queues, Elasticsearch, Nacos, Netty and more. It includes a LangChain4j module and an MCP server module that exposes tools over Streamable HTTP. It is a learning reference rather than an app starter.

- **+** Covers many Java middleware pieces: Dubbo, RocketMQ, Kafka, Nacos, Sentinel, ShardingSphere
- **+** Spring Boot samples module with 20+ examples
- **+** Includes an MCP server module using Streamable HTTP and a LangChain4j module
- **+** Apache-2.0 licensed with recent commits
- **−** Collection of samples, not a deployable template or product
- **−** README is in Chinese and gives no setup or run instructions
- **−** AI content is only two modules out of sixteen
- **−** No Docker or compose files for the required middleware

<sub>Java, LangChain4j · Needs Java 17+, Redis, Dubbo, RocketMQ, Elasticsearch, ZooKeeper, Nacos · [Repo](https://github.com/javahongxi/whatsmars) · [🌐 Site ↗](http://hongxi.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/whatsmars/)</sub>

<a name="fullstack-solution-template-for-agentcore"></a>
### #&#8288;75 [fullstack-solution-template-for-agentcore](https://github.com/awslabs/fullstack-solution-template-for-agentcore) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 608 · Apache-2.0 · Nov 2026</sub>

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

<a name="serverless-express"></a>
### #&#8288;76 [serverless-express](https://github.com/codegenieapp/serverless-express) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (56) · Freshness: recent (64) · Maintenance: patchy (33) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · Apache-2.0 · Apr 2026</sub>

**Run Express, Koa or Hapi apps on AWS Lambda or Azure Functions.**

An npm library (@codegenie/serverless-express) that wraps an existing Node.js web app in a Lambda or Azure Function handler. It maps API Gateway v1/v2, ALB, Lambda@Edge and VPC Lattice events to mock request/response objects, with custom mappers and routes for SNS, SQS and DynamoDB Streams. The repo includes a SAM-based starter example.

- **+** Handler wrapper is a few lines around an existing Express app
- **+** Supports API Gateway v1/v2, ALB, Lambda@Edge and VPC Lattice natively
- **+** Custom request/response mappers cover other Lambda event sources
- **+** Routes SNS, SQS, DynamoDB and EventBridge events to HTTP paths
- **−** Targets AWS Lambda and Azure Functions only
- **−** General HTTP adapter with no AI or model features
- **−** Upgrading from 4.x to 5.x requires following UPGRADE.md
- **−** Binary media types must also be set on API Gateway

<sub>JavaScript · Needs AWS Lambda, Amazon API Gateway, Azure Functions, Node.js · [Repo](https://github.com/codegenieapp/serverless-express) · [🌐 Site ↗](https://codegenie.codes) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/serverless-express/)</sub>

<a name="docker-flask-example"></a>
### #&#8288;77 [docker-flask-example](https://github.com/nickjj/docker-flask-example) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 762 · MIT · Nov 2026</sub>

**Minimal Flask starter with Postgres, Redis, Celery and esbuild/Tailwind assets.**

A small Flask 3.1.3 / Python 3.15.2 app meant as a base for new projects or as a reference for Dockerizing an existing Flask app. It wires up PostgreSQL via SQLAlchemy, Redis, Celery, gunicorn, and an esbuild and TailwindCSS asset build, run through Docker Compose and a ./run helper script. It has no AI features, auth or billing.

- **+** bin/rename-project script renames the app without a generator tool
- **+** Ships ruff linting, pytest with coverage, and GitHub Actions CI
- **+** Health check blueprint, STDOUT logging and env-based config suit containers
- **+** Uses uv for Python dependencies; esbuild leaves JS library choice open
- **−** No auth, user model, billing or AI integration; it is a bare scaffold
- **−** Requires Docker Compose v2 2.20.2+; Windows users are expected to use WSL
- **−** First build takes 5-10 minutes
- **−** Bundled extras (Flask-DB, Flask-Static-Digest) must be swapped out if unwanted

<sub>Python · Needs Docker, Docker Compose v2 2.20.2+, PostgreSQL, Redis · Docker · env example file · [Repo](https://github.com/nickjj/docker-flask-example) · [🌐 Site ↗](https://nickjanetakis.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/docker-flask-example/)</sub>

<a name="practical-cleanarchitecture"></a>
### #&#8288;78 [practical.cleanarchitecture](https://github.com/phongnguyend/practical.cleanarchitecture) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (33) · Freshness: active (84) · Maintenance: weak (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Nov 2026</sub>

**.NET clean architecture sample built as monolith, modular monolith and microservices.**

A C# sample solution (ClassifiedAds) that implements one classified-ads app in monolith, modular monolith and microservices layouts, with diagrams for clean, onion, hexagonal and vertical-slice architecture. It includes an MVC site, Web API, IdentityServer, background workers, and Angular, React, Vue and Blazor clients. Storage, messaging, caching, logging and monitoring providers are switched in appsettings.json. It has no AI features.

- **+** Same app built as monolith, modular monolith and microservices for direct comparison
- **+** Swappable providers: local, Azure Blob or S3 storage; RabbitMQ, Kafka or Azure queues
- **+** Four front ends included (Angular, React, Vue, Blazor) with IdentityServer login
- **+** Observability options: Elasticsearch, OpenTelemetry, Application Insights, health checks UI
- **−** Contains no AI or LLM features, so it is a poor fit for an AI list
- **−** README warns the samples mix several patterns and may not suit every situation
- **−** No Docker or compose files detected; setup is manual edits to appsettings.json
- **−** README publishes a default account username and password

<sub>C# · Needs SQL Server, RabbitMQ, Kafka, Redis, Elasticsearch, Azure Blob Storage, Amazon S3 · [Repo](https://github.com/phongnguyend/practical.cleanarchitecture) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/practical-cleanarchitecture/)</sub>

<a name="express-generator-typescript"></a>
### #&#8288;79 [express-generator-typescript](https://github.com/seanpmaxwell/express-generator-typescript) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 945 · MIT · Oct 2026</sub>

**CLI that scaffolds Express APIs in TypeScript with no build step.**

A command-line generator, like the classic express-generator, that creates an Express project set up for TypeScript as an ES module. The generated app is a small layered CRUD example for a User record, with ESLint, Prettier, Node's built-in test runner, live reload and a `#src/*` import alias. TypeScript runs through Node's type stripping, so there is no compile step in development or production.

- **+** No build step: Node type stripping runs TypeScript directly in dev and production
- **+** Lean output: no view engine, ORM or UI layer, only Express and TypeScript essentials
- **+** Ships ESLint, Prettier, typecheck and Node test runner scripts preconfigured
- **+** Refuses to write into a non-empty folder unless --force is passed
- **−** Requires Node.js 22.18+, 24.x or 26+
- **−** No database or ORM included; the example repo layer is only a demo
- **−** Not AI-specific; contains no model or agent integration
- **−** Layered layout suits small apps; README suggests a domain layout for growth

<sub>TypeScript · Needs Node.js 22.18+ · [Repo](https://github.com/seanpmaxwell/express-generator-typescript) · [🌐 Site ↗](https://www.npmjs.com/package/express-generator-typescript) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/express-generator-typescript/)</sub>

<a name="moderncppstarter"></a>
### #&#8288;80 [moderncppstarter](https://github.com/thelartians/moderncppstarter) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (57) · Freshness: recent (78) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · Unlicense · May 2026</sub>

**CMake template for C++ projects with tests, CI, formatting and docs.**

A GitHub template repository for starting a C++ library or executable with a CMake layout already in place. It separates the library, a standalone executable, a test suite and Doxygen documentation into their own CMake subprojects, with GitHub Actions workflows for macOS, Windows and Ubuntu. It has no AI functionality, so it fits the list's categories only loosely.

- **+** Library, standalone, test and docs live in separate CMake subprojects, with an `all` build for IDEs
- **+** Dependencies are pinned through CPM.cmake, which can fall back to find_package, vcpkg or Conan
- **+** Optional sanitizers, clang-tidy, iwyu, cppcheck and ccache enabled by CMake flags
- **+** CI covers macOS, Windows and Ubuntu, with formatting checks, codecov coverage and Doxygen docs on release
- **−** No AI, model or agent functionality; it is a generic C++ project scaffold
- **−** Renaming the `Greeter` placeholder across CMakeLists and include paths is a manual step
- **−** Uses file GLOB for sources, so adding files requires re-running CMake
- **−** No CPack installer setup; the README says it is out of scope

<sub>CMake · Needs CMake, CPM.cmake, clang-format, cmake-format, Doxygen, codecov · GitHub template · [Repo](https://github.com/thelartians/moderncppstarter) · [📖 Docs ↗](https://thelartians.github.io/ModernCppStarter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/moderncppstarter/)</sub>

<a name="graphene-django"></a>
### #&#8288;81 [graphene-django](https://github.com/graphql-python/graphene-django) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (49) · Freshness: recent (55) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Jun 2026</sub>

**GraphQL API library that maps Django models to Graphene types.**

Graphene-Django is a Python library that exposes Django models as GraphQL types through DjangoObjectType and serves them with a GraphQLView, optionally with the GraphiQL IDE. It integrates with Django's auth, forms and pagination, and ships a GraphQLTestCase helper for testing queries. It is installed into an existing Django project, not run as a standalone app.

- **+** DjangoObjectType generates GraphQL types directly from Django models
- **+** Includes GraphQLTestCase for testing queries with Django's test client
- **+** GraphiQL can be enabled with graphiql=True on the view
- **+** MIT license, installable with pip or conda-forge
- **−** Last release is 2025-03-13, well behind recent commits
- **−** Subscriptions and file uploads need separate third-party packages
- **−** Only works inside a Django project; no standalone server
- **−** No AI or model-serving features; fits this list only as a generic API backend

<sub>Python · Needs Django, Graphene · [Repo](https://github.com/graphql-python/graphene-django) · [📖 Docs ↗](http://docs.graphene-python.org/en/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphene-django/)</sub>

<a name="uwsgi-nginx-flask-docker"></a>
### #&#8288;82 [uwsgi-nginx-flask-docker](https://github.com/tiangolo/uwsgi-nginx-flask-docker) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (40) · Freshness: recent (70) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Oct 2026</sub>

**Base image running Flask under uWSGI and Nginx in one container.**

A Docker base image that runs a Flask app with uWSGI behind Nginx in a single container, published as python3.10, python3.11 and python3.12 tags. Behavior is tuned with environment variables such as UWSGI_PROCESSES, LISTEN_PORT and STATIC_PATH, and an optional /app/prestart.sh runs before startup. The README marks it deprecated: uWSGI is in maintenance mode and no new Python versions will be added.

- **+** Minimal setup: copy an app/main.py exposing `app` onto the image and it serves
- **+** Env vars control uWSGI workers (default 2 up to 16), Nginx workers, port, static path and upload size
- **+** prestart.sh hook runs migrations or scripts before the server starts
- **+** Dated build tags let you pin an exact image version
- **−** Deprecated by the author; no support planned for new Python versions
- **−** uWSGI is in maintenance mode, and the README recommends migrating away
- **−** Per-container worker manager is redundant on Kubernetes or Swarm, where replication happens at the cluster
- **−** Only python3.10 to 3.12 tags remain; older tags are removed from the repo

<sub>Python · Needs Docker, uWSGI, Nginx · [Repo](https://github.com/tiangolo/uwsgi-nginx-flask-docker) · [🌐 Site ↗](https://hub.docker.com/r/tiangolo/uwsgi-nginx-flask/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/uwsgi-nginx-flask-docker/)</sub>

<a name="nunu"></a>
### #&#8288;83 [nunu](https://github.com/go-nunu/nunu) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (36) · Freshness: active (98) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Aug 2026</sub>

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

<a name="nodejs-api-boilerplate"></a>
### #&#8288;84 [nodejs-api-boilerplate](https://github.com/vyancharuk/nodejs-api-boilerplate) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (1) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 164 · MIT · Nov 2026</sub>

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
### #&#8288;85 [get-started-with-ai-agents](https://github.com/azure-samples/get-started-with-ai-agents) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 387 · MIT · Oct 2026</sub>

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

<a name="typescript-action"></a>
### #&#8288;86 [typescript-action](https://github.com/actions/typescript-action) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: known (33) · Freshness: recent (61) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · May 2026</sub>

**Template repo for writing GitHub Actions in TypeScript.**

Official GitHub template for creating a JavaScript action in TypeScript. It ships a sample action with action.yml metadata, a Rollup bundle step that produces dist/, tests, lint and CodeQL workflows, and a release script that syncs major version tags. It contains no AI functionality, so it fits this list only loosely.

- **+** CI workflows cover linting, tests, CodeQL and a check that dist/ is up to date
- **+** script/release tags vX.X.X and moves the matching major tag (v1, v2)
- **+** Local runs via @github/local-action, with a VS Code launch config
- **+** Optional Licensed workflow for dependency license checks, disabled by default
- **−** No AI, model or agent code; the sample action only waits a number of milliseconds
- **−** Bundled dist/ must be rebuilt and committed with npm run all or the action fails
- **−** No tagged releases of its own; versioning is left to your repository
- **−** Requires Node.js 20 or later and a GitHub repository to be useful

<sub>TypeScript · Needs Node.js 20+, GitHub Actions · GitHub template · env example file · [Repo](https://github.com/actions/typescript-action) · [📖 Docs ↗](https://github.com/actions/toolkit/blob/main/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typescript-action/)</sub>

<a name="serverless-rag-demo"></a>
### #&#8288;87 [serverless-rag-demo](https://github.com/aws-samples/serverless-rag-demo) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (2) · Freshness: active (100) · Maintenance: weak (26) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 223 · MIT-0 · Oct 2026</sub>

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

<a name="openai-chat-vision-quickstart"></a>
### #&#8288;88 [openai-chat-vision-quickstart](https://github.com/azure-samples/openai-chat-vision-quickstart) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 224 · MIT · Oct 2026</sub>

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

<a name="fastapi-clean-example"></a>
### #&#8288;89 [fastapi-clean-example](https://github.com/ivan-borovets/fastapi-clean-example) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 601 · MIT · Nov 2026</sub>

**FastAPI example app structured with clean architecture and Alembic migrations.**

A FastAPI reference project organized along clean-architecture lines, with user sign-up, login and role-based access (a super_admin role is set manually in the database). It uses Alembic for migrations, uv for dependencies, and Make targets for Docker and local runs. The README is mid-refactor; architecture docs live on the legacy-2025 branch, and it is not yet a finished template.

- **+** Makefile targets cover Docker start, local start, migrations and tests
- **+** Tests included, with light (make check) and full Docker (make test-docker) runs
- **+** Pre-commit and pre-push hooks set up via prek
- **+** Docker and compose files included
- **−** Refactor in progress; README does not yet explain code or patterns
- **−** Template conversion is unchecked in the README TODO list
- **−** Architecture docs only on the legacy-2025 branch, not the main branch
- **−** Super admin role must be set by hand in the database

<sub>Python · Needs Docker, Alembic, uv · GitHub template · Docker · env example file · [Repo](https://github.com/ivan-borovets/fastapi-clean-example) · [📖 Docs ↗](https://github.com/ivan-borovets/fastapi-clean-example/tree/legacy-2025) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fastapi-clean-example/)</sub>

<a name="openai-chat-app-quickstart"></a>
### #&#8288;90 [openai-chat-app-quickstart](https://github.com/azure-samples/openai-chat-app-quickstart) <sub>score [36](../README.md#-how-we-rank "Score 36/100. Adoption: niche (3) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 254 · MIT · Oct 2026</sub>

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

<a name="symfony-7-es-cqrs-boilerplate"></a>
### #&#8288;91 [symfony-7-es-cqrs-boilerplate](https://github.com/jorge07/symfony-7-es-cqrs-boilerplate) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (17) · Freshness: active (95) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Aug 2026</sub>

**Symfony 7 reference app for DDD, CQRS and event sourcing.**

PHP 8.3 and Symfony 7 boilerplate showing domain-driven design, CQRS and event sourcing with Symfony Messenger. It includes an event store, a read model, async event subscribers, a REST API with Swagger docs, and a user flow (sign up, change email, sign in, logout). It runs through Docker Compose with MySQL, Elasticsearch/Kibana and RabbitMQ. It has no AI features.

- **+** Working event store, read model and async subscribers in one small codebase
- **+** Makefile targets for setup, PHPUnit, PHPStan and code style checks
- **+** Docs cover buses, use cases, projections, async processing and Kubernetes deployment
- **+** Older Symfony 4, 5 and 6 versions kept on separate branches
- **−** Contains no AI or model integration; not an AI starter
- **−** Pinned to Elasticsearch and Kibana 7.11.0, an old release
- **−** README calls the web UI poor UX; the demo use case is only user accounts
- **−** Needs MySQL, Elasticsearch and RabbitMQ running, heavy for a small demo

<sub>PHP · Needs MySQL 8.0, Elasticsearch 7.11.0, Kibana 7.11.0, RabbitMQ 3, Docker Compose · GitHub template · env example file · ⚠️ .env file committed · [Repo](https://github.com/jorge07/symfony-7-es-cqrs-boilerplate) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/symfony-7-es-cqrs-boilerplate/)</sub>

<a name="flask-restx"></a>
### #&#8288;92 [flask-restx](https://github.com/python-restx/flask-restx) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: known (31) · Freshness: slowing (46) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · custom license · Apr 2026</sub>

**Flask extension for building REST APIs with Swagger documentation.**

Flask-RESTX is a Flask extension, forked from Flask-RESTPlus, that provides decorators for routing, request validation and response marshalling in REST APIs. It generates Swagger documentation from the same declarations. It is a general Python library installed with pip, not an AI project or a starter app.

- **+** Swagger docs generated from the same decorators that define routes and models
- **+** Namespaces, field models and marshal decorators keep resources organized
- **+** Installs with pip; requires Python 3.10+ and supports Flask 3
- **+** README includes a Flask/Werkzeug compatibility table per release
- **−** No AI, model or agent functionality; only a general REST API layer
- **−** Flask 2.0 broke compatibility, so older versions need pinning
- **−** Volunteer-maintained; README says trunk addresses issues faster than releases
- **−** License is reported as NOASSERTION by metadata detection

<sub>Python · Needs Flask, Werkzeug · [Repo](https://github.com/python-restx/flask-restx) · [📖 Docs ↗](http://flask-restx.readthedocs.io/en/latest/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/flask-restx/)</sub>

<a name="itty-router"></a>
### #&#8288;93 [itty-router](https://github.com/kwhitley/itty-router) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (29) · Freshness: active (81) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Jun 2026</sub>

**Tiny TypeScript HTTP router for Cloudflare Workers and other serverless runtimes.**

itty-router is a small API router written in TypeScript, with variants from about 450 bytes up to about 970 bytes for AutoRouter. It parses route patterns and query strings, supports middleware, and lets handlers return plain values that become responses. It targets serverless runtimes such as Cloudflare Workers but runs elsewhere.

- **+** Router sizes range from ~450 bytes to ~970 bytes for AutoRouter, per the README
- **+** Handlers can return plain values, promises or arrays without wrapping in a Response
- **+** Typed for TypeScript, with a v4 to v5 migration guide
- **+** README reports 100% test coverage
- **−** No AI, model or agent functionality; it is a general HTTP router only
- **−** Routing and middleware only; auth, database and validation are left to you
- **−** Breaking changes between v4 and v5 require migration
- **−** AutoRouter export needs `{ ...router }` to strip the proxy

<sub>TypeScript · GitHub template · [Repo](https://github.com/kwhitley/itty-router) · [📖 Docs ↗](https://itty.dev/itty-router) · [🌐 Site ↗](https://itty.dev/itty-router) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/itty-router/)</sub>

<a name="go-gin-example"></a>
### #&#8288;94 [go-gin-example](https://github.com/eddycjy/go-gin-example) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (64) · Freshness: slowing (41) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.2k · MIT · Mar 2026</sub>

**Go and Gin blog REST API example with JWT, MySQL, Redis and Swagger.**

A layered Go REST API for a blog, built on Gin and GORM with MySQL storage and Redis caching. It covers article and tag CRUD with soft delete, JWT login, image upload, QR-code article posters and Excel import/export of tags. Swagger UI is served at /swagger. It is a reference example with no AI features.

- **+** Clear handler, service and model layering that is easy to read and copy
- **+** JWT auth, Redis caching, pagination and Swagger docs in one small codebase
- **+** Ships SQL schema, ini config, Makefile and Dockerfile for a quick local run
- **+** MIT licensed, last commit March 2026
- **−** No AI or model features; it is a plain CRUD blog API
- **−** Uses older libraries: jinzhu/gorm, dgrijalva/jwt-go, Go 1.13+ baseline
- **−** Sample config ships JwtSecret = 233 and a root database password
- **−** Needs external MySQL and Redis; the docker run command does not provide them

<sub>Go · Needs MySQL 5.6+, Redis · Docker · [Repo](https://github.com/eddycjy/go-gin-example) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-gin-example/)</sub>

<a name="genai-api"></a>
### #&#8288;95 [genai-api](https://github.com/louisbrulenaudet/genai-api) <sub>score [18](../README.md#-how-we-rank "Score 18/100. Adoption: niche (0) · Freshness: slowing (49) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 113 · Apache-2.0 · Apr 2026</sub>

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

<a name="cookiecutter-django-rest"></a>
### #&#8288;96 [cookiecutter-django-rest](https://github.com/agconti/cookiecutter-django-rest) <sub>score [9](../README.md#-how-we-rank "Score 9/100. Adoption: niche (24) · Freshness: quiet (5) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Dec 2025</sub>

**Cookiecutter template for Django REST Framework APIs with auth and tests.**

A cookiecutter template that scaffolds a Django 5.0+ REST API on Python 3.13+ with PostgreSQL 16.4+. The generated project includes authentication, user accounts, API docs, tests and CI config, so you only add your own resources. It is a general REST API starter with no AI features built in.

- **+** Generates auth, user endpoints, API docs and tests with one cookiecutter command
- **+** Uses Django REST Framework with PostgreSQL 16.4+ on Python 3.13+
- **+** Local development via docker-compose is part of the generated project
- **+** Recent commits (2025-12) and MIT license
- **−** Last tagged release is from 2017-12-28, so there are no recent versions
- **−** Generated CI config is .travis.yml, which many teams no longer use
- **−** No AI or model-serving code; it is only a generic REST API scaffold
- **−** Requires installing cookiecutter first; only the users resource is scaffolded

<sub>Python · Needs cookiecutter, PostgreSQL 16.4+, Docker, docker-compose · [Repo](https://github.com/agconti/cookiecutter-django-rest) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cookiecutter-django-rest/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
