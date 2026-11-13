# 🧪 Code review and testing reviews · Best of Vibe Coding

AI tools that review pull requests, write tests or find bugs, run in your CI or on your machine. Back to the [leaderboard](../README.md#-code-review-and-testing).

<sub>🌐 Also on the web: [Code review and testing on archestack.com](https://archestack.com/best-of-vibe-coding/code-review/), each project on its own page.</sub>

<a name="playwright"></a>
### 🥇 [playwright](https://github.com/microsoft/playwright) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 100k · Apache-2.0 · Nov 2026</sub>

**Cross-browser automation and end-to-end test framework for Chromium, Firefox and WebKit.**

Playwright drives Chromium, Firefox and WebKit through one API, used for end-to-end tests with the Playwright Test runner, for standalone scripts such as screenshots, PDFs and scraping, and as a browser tool for AI agents. The agent paths are a CLI for coding agents and an MCP server that exposes pages as accessibility snapshots. Bindings exist for TypeScript/JavaScript, Python, .NET and Java.

- **+** One API covers Chromium, Firefox and WebKit on Linux, macOS and Windows, headless or headed
- **+** Test runner has auto-waiting, retrying assertions, per-test browser contexts and parallel execution
- **+** Trace Viewer records DOM snapshots, network requests and console logs; VS Code extension adds codegen
- **+** Agent tooling: MCP server uses accessibility snapshots, so no vision model is needed
- **−** Browser binaries must be downloaded separately with `npx playwright install`
- **−** MCP server and CLI live in separate repos, not in this one
- **−** Agent features are secondary; the core is a testing and automation library

<sub>no GPU · Needs Node.js, Browser binaries via npx playwright install · [Repo](https://github.com/microsoft/playwright) · [📖 Docs ↗](https://playwright.dev/docs/intro) · [🌐 Site ↗](https://playwright.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/playwright/)</sub>

<a name="nx"></a>
### 🥈 [nx](https://github.com/nrwl/nx) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Nov 2026</sub>

**Monorepo build system with task caching, affected-only runs and CI integration.**

Nx is a monorepo tool for TypeScript and polyglot codebases, with a core written in Rust and extensibility in TypeScript. It caches task outputs, runs only affected projects, and can be added to an existing npm, pnpm or yarn workspace with `npx nx init`. Its CI layer adds remote caching, task distribution and an AI self-healing step that proposes fixes for failed pipelines.

- **+** Adopts existing package.json scripts via `npx nx init` without restructuring the workspace
- **+** Plugins cover Vite, Webpack, Jest, Vitest, ESLint, Gradle, Maven, .NET and Go
- **+** Runs only affected tasks and caches outputs of unchanged ones
- **+** CI integration works with GitHub Actions, GitLab and Azure
- **−** Remote caching, task distribution and self-healing CI go through the Nx Cloud service
- **−** Not an AI app starter; AI features are limited to CLI agent context and CI fixes
- **−** Plugins and CI setup add concepts beyond plain package scripts

<sub>no GPU · Needs Node.js, Nx Cloud (optional, for remote cache and self-healing CI) · [Repo](https://github.com/nrwl/nx) · [📖 Docs ↗](https://nx.dev/docs) · [🌐 Site ↗](https://nx.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nx/)</sub>

<a name="open-code-review"></a>
### 🥉 [open-code-review](https://github.com/alibaba/open-code-review) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 50k · Apache-2.0 · Nov 2026</sub>

**Go CLI that reviews Git diffs with an LLM agent and line-level comments.**

Open Code Review (`ocr`) reads a Git diff, bundles related files into sub-agent review units, and sends them to a configurable LLM that can read files and search the repo. It outputs structured comments with line positions, and `ocr scan` reviews whole files without a diff. It runs locally or in CI (GitHub Actions, GitLab CI, GitFlic CI, Gerrit), with plugins for Claude Code, Codex, Cursor, Kimi Code and OpenCode.

- **+** Deterministic file selection, bundling and rule matching; one sub-agent per bundle for large changesets
- **+** Delegation mode lets the host coding agent use its own LLM, so no OCR API key
- **+** Separate comment-positioning and reflection modules to improve line accuracy
- **+** Resumable review and scan sessions, with a browser session viewer
- **−** Requires Git 2.41 or newer
- **−** Recall is lower than a general-purpose agent, per the README's own benchmark
- **−** Benchmark figures are the authors' own AACR-Bench comparison
- **−** Default mode needs an LLM provider and API key configured first

<sub>no GPU · Needs Git >= 2.41, LLM provider endpoint (unless delegation mode), Node.js/npm (for npm install) · Models: Built-in and custom LLM providers, Host agent models in delegation mode · [Repo](https://github.com/alibaba/open-code-review) · [📖 Docs ↗](https://open-codereview.ai/docs) · [🌐 Site ↗](https://open-codereview.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-code-review/)</sub>

<a name="bend"></a>
### #&#8288;4 [bend](https://github.com/bendlang/bend) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · Apache-2.0 · Nov 2026</sub>

**Dependent-typed language where AI-written code must prove rules in LAWS.bend.**

Bend 2 is a Python-like language with dependent types and a proof checker, compiling to C, Metal, CUDA and JavaScript. Rules are declared in a LAWS.bend file, and the agent runs `bend PROOF.bend` after each edit so the compiler rejects changes that break a law. Divide-and-conquer calls run in parallel across CPU cores or a GPU.

- **+** Laws are machine-checked, so agent edits that violate them fail to compile
- **+** Parallel execution on CPU cores or GPU without threads, locks or kernels
- **+** Installs with one curl script; agent setup is a short AGENTS.md snippet
- **+** Targets C, Metal, CUDA and JavaScript; JS target suits fast iteration
- **−** Compiler is about 99% AI-written and not fully audited; README warns to expect bugs
- **−** Proofs need real effort: no tactics or proof search, and all code is annotated
- **−** No native Windows support (WSL only); native builds need clang 14+, GPU runs need 19+
- **−** No TLS, HTTP, JSON or regex libraries; numbers limited to Nat, U32 and F32

<sub>GPU optional · Needs clang 14+ (19+ for GPU calls), Metal or CUDA 12 for GPU, X11 and ALSA headers (Linux, window/audio) · [Repo](https://github.com/bendlang/bend) · [▶️ Demo ↗](https://bend-lang.com/#lab) · [🌐 Site ↗](https://bend-lang.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bend/)</sub>

<a name="mobile-dev-inc-maestro"></a>
### #&#8288;5 [maestro](https://github.com/mobile-dev-inc/maestro) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · Apache-2.0 · Nov 2026</sub>

**YAML-based UI and end-to-end test framework for Android, iOS and web.**

Maestro runs UI and end-to-end tests written as flat YAML command lists (launchApp, tapOn, assertVisible) against Android, iOS and web apps, driving them through the platform accessibility layer. It installs as a single CLI binary and also ships an MCP server (`maestro mcp`) so coding agents can control a live device and write flows. Flows run on emulators, simulators, browsers and physical Android devices.

- **+** Single binary install; no drivers or SDK needed in the app under test
- **+** One YAML syntax covers Android, iOS, web, React Native, Flutter and hybrid apps
- **+** Built-in MCP server in the CLI works with Claude Code, Cursor, Codex and others
- **+** Automatic waiting and flakiness tolerance remove manual sleep calls
- **−** Physical iOS devices are not supported
- **−** Requires Java 17 or higher on the host
- **−** Maestro Studio IDE is free but closed source
- **−** Parallel execution at scale needs paid Maestro Cloud

<sub>no GPU · Needs Java 17+ · [Repo](https://github.com/mobile-dev-inc/maestro) · [📖 Docs ↗](https://docs.maestro.dev) · [🌐 Site ↗](https://www.maestro.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mobile-dev-inc-maestro/)</sub>

<a name="midscene"></a>
### #&#8288;6 [midscene](https://github.com/web-infra-dev/midscene) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

**Vision-based E2E testing in natural language for web, mobile and desktop.**

Midscene.js drives web, Android, iOS, HarmonyOS and desktop UIs from screenshots using a vision model, so tests are written as natural-language steps and assertions instead of selectors. Tests can be YAML cases run by Midscene Test (@midscene/test) or agent calls such as aiAct and aiAssert inside Playwright, Puppeteer, Vitest or Rstest. It produces HTML reports with screenshots and the model's decisions.

- **+** Locates elements from screenshots, so canvas, icon-only buttons and cross-origin iframes need no selectors
- **+** Same agent API across web, Android, iOS, HarmonyOS and desktop
- **+** Step-level HTML reports with screenshots, plus summary.json for scripts and AI agents
- **+** Works with GPT, Qwen, Doubao, DeepSeek, Gemini, Kimi, including self-hostable models
- **−** Requires a configured vision-capable model; runs depend on model API calls or self-hosting
- **−** Python and Java SDKs are community projects, not part of the main repo
- **−** Assertions are model judgments, so results can vary between runs and models
- **−** iOS needs WebDriverAgent and Android needs ADB, adding device setup

<sub>Needs Vision-language model API or self-hosted model, Playwright or Puppeteer (web), ADB (Android), WebDriverAgent (iOS), HDC (HarmonyOS) · Models: GPT, Qwen, Doubao Seed, DeepSeek, Gemini · [Repo](https://github.com/web-infra-dev/midscene) · [📖 Docs ↗](https://midscenejs.com/) · [🌐 Site ↗](https://midscenejs.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/midscene/)</sub>

<a name="react-doctor"></a>
### #&#8288;7 [react-doctor](https://github.com/millionco/react-doctor) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Nov 2026</sub>

**CLI that scans React codebases for state, performance, security and accessibility issues.**

React Doctor runs deterministic checks over a React project and reports issues in state and effects, performance, architecture, security, accessibility and maintainability. It covers Next.js, Vite, Astro, TanStack, React Native and Expo. It also installs as a skill for coding agents, runs on pull requests in CI, and can record a Chrome DevTools performance trace of a running app.

- **+** Runs with one npx command from the project root, no setup needed
- **+** Deterministic rules rather than LLM-generated findings
- **+** Agent skill installer supports Claude Code, Cursor, Codex and OpenCode
- **+** Rules configurable in doctor.config.ts; CI installer reports issues each PR introduces
- **−** React-only; no support for other frameworks beyond the listed React stacks
- **−** CLI collects crash reports and anonymous usage data unless opted out
- **−** Runtime trace scan needs a running app and a Chrome DevTools trace

<sub>no GPU · Needs Node.js, npm · [Repo](https://github.com/millionco/react-doctor) · [📖 Docs ↗](https://react.doctor/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-doctor/)</sub>

<a name="pr-agent"></a>
### #&#8288;8 [pr-agent](https://github.com/the-pr-agent/pr-agent) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Nov 2026</sub>

**LLM-based pull request reviewer that runs as a GitHub Action, CLI or webhook.**

PR-Agent posts AI-generated PR descriptions, reviews, code suggestions and Q&A as comments via /describe, /review, /improve and /ask commands. It supports GitHub, GitLab, Bitbucket, Azure DevOps and Gitea, and any model reachable through LiteLLM, including OpenAI, Claude, Gemini and Ollama. Each command uses a single LLM call, and prompts are configurable through TOML files.

- **+** Supports GitHub, GitLab, Bitbucket, Azure DevOps and Gitea
- **+** Any LiteLLM-reachable model, including local Ollama, so code can stay in your infrastructure
- **+** One LLM call per command; PR compression handles large diffs
- **+** Installs as a GitHub Action, pip package, Docker image or webhook server
- **−** Described as a community-maintained legacy project, separate from Qodo's current product
- **−** /help_docs is disabled since v0.36.1 because of a credential-exposure issue
- **−** Docker image moved to pragent/pr-agent from 0.34.2; pinned references need updating
- **−** Project is still being donated to a foundation, so governance is in flux

<sub>no GPU · Docker + Compose · Needs LLM provider API key (e.g. OpenAI), Git provider token · Models: OpenAI GPT, Anthropic Claude, Google Gemini, DeepSeek, Mistral · [Repo](https://github.com/the-pr-agent/pr-agent) · [📖 Docs ↗](https://docs.pr-agent.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pr-agent/)</sub>

<a name="infracost"></a>
### #&#8288;9 [infracost](https://github.com/infracost/infracost) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

**Cloud cost estimates for Terraform and CloudFormation in the terminal, editor and PRs.**

Infracost is a Go CLI that estimates cloud cost and checks FinOps policies for Terraform, Terragrunt, CloudFormation and AWS CDK before deployment. The same engine backs editor extensions (VS Code, JetBrains, Neovim, Zed), agent skills for Claude Code and Cursor, and CI integrations that post cost diffs on pull requests. This repo is the umbrella entry point; the code lives in separate repositories.

- **+** Covers over 1,100 resources across AWS, Azure and Google Cloud
- **+** Same engine and policies in CLI, IDE via LSP, agent skills and CI
- **+** Estimates usage-based resources such as S3 and Lambda
- **+** Ships three agent skills: iac-generation, scan and price-lookup
- **−** This repo is a landing page; code is split across cli, lsp and plugin repos
- **−** Tagging policies and guardrails are managed in Infracost Cloud, a SaaS dashboard
- **−** Setup involves authenticating with Infracost, so it is not clearly usable offline
- **−** Supported clouds limited to AWS, Azure and Google Cloud

<sub>Docker · Needs Infracost account (authentication via infracost setup), Infracost Cloud (optional, for policies and dashboard) · [Repo](https://github.com/infracost/infracost) · [📖 Docs ↗](https://www.infracost.io/docs/) · [🌐 Site ↗](https://www.infracost.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/infracost/)</sub>

<a name="e2e"></a>
### #&#8288;10 [e2e](https://github.com/tester-army/e2e) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Nov 2026</sub>

**Agent-driven end-to-end testing for web and mobile apps.**

TypeScript test runner that mixes natural-language agent steps (agent.act, agent.assert) with ordinary locators and expect assertions. Agent actions that a later assertion verifies are recorded and replayed on the next run without model calls until the app changes. The web engine uses Playwright (Chromium, Firefox, WebKit); the mobile engine drives iOS simulators and Android emulators.

- **+** Recorded agent steps replay with no model calls until the app changes
- **+** Tests without agent steps need no model at all
- **+** Hosted browser and device integrations: BrowserStack, E2B, Kernel, Limrun and others
- **+** Example projects for Next.js, Expo, SwiftUI, Flutter, Compose and more
- **−** Pre-1.0: APIs and config can change between minor releases
- **−** Agent steps need a model provider, subscription, API key or local model
- **−** CLI sends anonymous telemetry by default; opt-out is required
- **−** Tests are written in TypeScript only

<sub>Needs Node.js, Playwright, agent-device · Models: Claude Code (via ACP), Codex (via ACP), API key providers, local models · [Repo](https://github.com/tester-army/e2e) · [📖 Docs ↗](https://e2e.com/docs) · [🌐 Site ↗](https://e2e.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/e2e/)</sub>

<a name="phpstan"></a>
### #&#8288;11 [phpstan](https://github.com/phpstan/phpstan) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Nov 2026</sub>

**Static analyzer that finds bugs in PHP code without running it.**

PHPStan checks PHP code for type and logic errors before execution, using PHPDoc types and extensions to widen what it can verify. It runs from the command line or CI. PHPStan Pro, a paid add-on, adds a web UI for browsing errors and a watch mode. The project does not use AI models.

- **+** Catches classes of bugs without executing code or writing tests first
- **+** Online playground at phpstan.org/try for testing snippets without installing
- **+** Extension library and documented API for writing custom extensions
- **+** MIT-licensed with active releases; last release 2026-10-27
- **−** PHP only; no other languages are analyzed
- **−** Web UI and watch mode require paid PHPStan Pro after a 30-day trial
- **−** Not an AI tool; it does not use or integrate language models
- **−** Source for pull requests lives in phpstan/phpstan-src, not this repository

<sub>no GPU · Docker · [Repo](https://github.com/phpstan/phpstan) · [▶️ Demo ↗](https://phpstan.org/try) · [📖 Docs ↗](https://phpstan.org/user-guide/getting-started) · [🌐 Site ↗](https://phpstan.org/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/phpstan/)</sub>

<a name="keploy"></a>
### #&#8288;12 [keploy](https://github.com/keploy/keploy) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · Apache-2.0 · Nov 2026</sub>

**Records API traffic with eBPF and replays it as tests and mocks.**

Keploy records API calls, database queries and queue events by capturing traffic at the network layer with eBPF, then replays them as tests with mocked dependencies. It runs as a CLI (keploy record / keploy test) with no SDK or code changes, and fits into CI such as Jenkins and GitHub Actions. It can also generate extra test cases from OpenAPI schemas.

- **+** No SDK or code changes; wrap the app command with keploy record
- **+** Mocks Postgres, MySQL, MongoDB, Kafka and RabbitMQ, not just HTTP
- **+** Time freezing makes replays deterministic
- **+** Language-agnostic because capture happens at the network layer
- **−** Some protocol parsers are not open source and are absent from the enterprise edition
- **−** Schema-based AI test expansion points to the hosted app.keploy.io
- **−** Mock registry and time freezing are documented under Keploy Cloud
- **−** Install is a curl-piped shell script

<sub>no GPU · Docker · [Repo](https://github.com/keploy/keploy) · [📖 Docs ↗](https://keploy.io/docs/) · [🌐 Site ↗](https://keploy.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/keploy/)</sub>

<a name="hunk"></a>
### #&#8288;13 [hunk](https://github.com/modem-dev/hunk) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · MIT · Nov 2026</sub>

**Terminal diff viewer for reviewing code changes, with inline agent notes.**

Hunk is an interactive terminal diff viewer built on OpenTUI and Pierre diffs. It opens Git, Jujutsu and Sapling changes, GitHub pull requests, raw patches from stdin, or two files, in a multi-file stream with a sidebar. A coding agent can use the hunk-review skill to attach notes to a live session, and they show beside the code.

- **+** Opens Git, Jujutsu and Sapling changes, plus GitHub PRs via bundled `hunk gh` with no gh CLI
- **+** Works as a pager for git, jj and Sapling, and reads patches from stdin
- **+** Standalone binary via install script, Homebrew, mise or Nix; no Node.js needed
- **+** Extension API and embeddable OpenTUI diff component (`hunkdiff/opentui`)
- **−** No structural diffing; the README's own comparison table marks it as missing
- **−** No prebuilt binaries for Windows arm64 or musl Linux such as Alpine
- **−** GitHub Enterprise is not supported
- **−** Extension API is experimental and may break between minor releases

<sub>no GPU · Needs Git (recommended), Node.js 22+ (npm install only), GH_TOKEN or GITHUB_TOKEN (private repos) · [Repo](https://github.com/modem-dev/hunk) · [📖 Docs ↗](https://hunk.dev/docs/) · [🌐 Site ↗](https://hunk.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hunk/)</sub>

<a name="no-mistakes"></a>
### #&#8288;14 [no-mistakes](https://github.com/kunchenguid/no-mistakes) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Nov 2026</sub>

**Local git proxy that runs an AI review, test and lint pipeline before opening a PR.**

no-mistakes adds a `no-mistakes` git remote in front of your real one. Pushing to it creates a disposable worktree, runs review, test, docs, lint, push, PR and CI steps through a coding agent CLI, and forwards the branch only when every gate passes. Findings are either auto-fixed or escalated for you to approve, fix or skip in a TUI.

- **+** Runs in an isolated worktree, so your working branch is not touched
- **+** Works with claude, codex, opencode, copilot, cursor and others, with ordered fallbacks
- **+** Opens the PR and repairs CI failures after push, not just local checks
- **+** Also usable headlessly through a /no-mistakes agent skill installed by init
- **−** Needs at least one configured coding agent CLI; every gate requires a runnable agent
- **−** Agent runs spend API quota or subscription usage, and CI repairs can add full re-review passes
- **−** Changes the push workflow: pushes must go to the gate remote instead of origin
- **−** Fork contributions need extra setup via init --fork-url

<sub>Needs git, a supported coding agent CLI (claude, codex, opencode, etc.) · Models: claude, codex, grok, rovodev, opencode · [Repo](https://github.com/kunchenguid/no-mistakes) · [📖 Docs ↗](https://kunchenguid.github.io/no-mistakes/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/no-mistakes/)</sub>

<a name="codex-security"></a>
### #&#8288;15 [codex-security](https://github.com/openai/codex-security) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Nov 2026</sub>

**Vulnerability scanner, validator and patcher with a CLI, TypeScript SDK and Codex plugin.**

Codex Security scans repositories, paths or Git diffs for vulnerabilities, validates candidate findings, generates patches and verifies existing fixes. It runs as a Codex plugin, as the `cs` CLI (`@openai/codex-security`), through a TypeScript SDK, or as a GitHub Action. Results can be exported as SARIF, JSON or CSV, or sent to Linear, Jira or GitHub.

- **+** Scans whole repos, selected paths, or diffs against a base revision
- **+** Exports SARIF, JSON and CSV; integrates with Linear, Jira, GitHub and ServiceNow
- **+** Supports OpenAI, Amazon Bedrock, OpenRouter, Fireworks AI and Cheaper Inference
- **+** Ships a GitHub Action, SDK and Docker Compose setup for bulk scans
- **−** Requires Node.js 22.13+/24/26 and Python 3.10+ installed
- **−** Needs an OpenAI login or API key, or other provider credentials
- **−** Some cyber requests and protected findings need Trusted Access for Cyber
- **−** Local serve command and browser dashboard have been removed

<sub>no GPU · Docker + Compose · Needs Node.js 22.13+, Python 3.10+, OpenAI API key or other provider credentials · Models: OpenAI, Amazon Bedrock, OpenRouter, Fireworks AI, Cheaper Inference · [Repo](https://github.com/openai/codex-security) · [📖 Docs ↗](https://learn.chatgpt.com/docs/security/cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-security/)</sub>

<a name="larastan"></a>
### #&#8288;16 [larastan](https://github.com/larastan/larastan) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Nov 2026</sub>

**PHPStan extension that finds type errors and bugs in Laravel code.**

Larastan is a PHPStan extension for Laravel, installed as a Composer dev dependency. It boots the application container so it can resolve types that only exist at runtime, such as Eloquent magic, and reports errors at PHPStan levels up to 10. It is not an AI tool; it is rule-based code analysis that runs locally or in CI.

- **+** Resolves much of Laravel's magic by booting the app container to compute types
- **+** Baseline files let legacy codebases adopt a higher PHPStan level gradually
- **+** Composer install plus a phpstan.neon file; no service to run
- **+** Adds Laravel-specific rules, custom PHPDoc types and config parameters
- **−** Not AI-based; a rule-based static analyser that fits this list loosely
- **−** Version 3.x needs PHP 8.2+ and Laravel 11.15+
- **−** Boots the application during analysis, and large projects may hit memory limits
- **−** Some Laravel magic still needs entries in an ignore-errors list

<sub>no GPU · Needs PHP 8.2+, Laravel 11.15+, Composer, PHPStan · [Repo](https://github.com/larastan/larastan) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/larastan/)</sub>

<a name="docker-android"></a>
### #&#8288;17 [docker-android](https://github.com/budtmo/docker-android) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · custom license · Nov 2026</sub>

**Android emulator in a container with web VNC, for app builds and UI tests.**

Runs an Android emulator (API 28 to 34, with Samsung Galaxy and Nexus device profiles) inside Docker, viewable through a noVNC page on port 6080 and controllable from the host with adb connect. It is used to build Android projects and run Appium or Espresso UI tests, and it has a beta MCP server image. The AI-agent feature and newer Android versions are in a separate sponsor-only Pro image.

- **+** Separate images per Android version, 9.0 to 14.0, plus a Genymotion image
- **+** Browser VNC on port 6080 and adb connect from the host
- **+** Documented use cases for Appium, Jenkins, SMS simulation and cloud deployment
- **+** Beta MCP server and Appium MCP image for agent-driven testing
- **−** Needs /dev/kvm; runs on Ubuntu hosts only, other OSes need an Ubuntu VM
- **−** AI agent, headless mode, proxy and Android 15+ are Pro-only, for sponsors
- **−** Emulator state is discarded on restart unless /home/androidusr is mounted
- **−** Normal edition includes user-behavior analytics, which Pro disables

<sub>Docker · Needs Docker, KVM (/dev/kvm), Ubuntu host · Models: Ollama, vLLM · port 6080 · [Repo](https://github.com/budtmo/docker-android) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/docker-android/)</sub>

<a name="pest"></a>
### #&#8288;18 [pest](https://github.com/pestphp/pest) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Nov 2026</sub>

**Testing framework for PHP projects, built for developers and AI agents.**

Pest is a PHP testing framework distributed through Composer and Packagist, now at version 5. The README is brief and points to pestphp.com for documentation and the v5 announcement. It describes Pest as built for PHP developers and AI agents, but gives no feature or installation details.

- **+** MIT licensed, published on Packagist with CI on the 5.x branch
- **+** Commit and release both dated 2026-10-27
- **+** Full documentation on a dedicated site, pestphp.com
- **−** README has no install steps, code examples or feature list
- **−** PHP only; not usable for projects in other languages
- **−** AI agent support is mentioned but not explained in the README

<sub>no GPU · Needs PHP, Composer · [Repo](https://github.com/pestphp/pest) · [📖 Docs ↗](https://pestphp.com/docs/pest5-now-available) · [🌐 Site ↗](https://pestphp.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pest/)</sub>

<a name="prek"></a>
### #&#8288;19 [prek](https://github.com/j178/prek) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.8k · MIT · Nov 2026</sub>

**Rust reimplementation of pre-commit that runs Git hooks from a single binary.**

prek runs hooks such as formatters, linters and secret scanners before commit, on demand, or in CI, and installs the toolchains those hooks need. It reads existing pre-commit YAML configs as a drop-in replacement and also supports a native prek.toml. It is not an AI tool itself, though the README mentions an installable skill so agents can use it.

- **+** Single Rust binary, no Python or other runtime required
- **+** Reads existing pre-commit configs and hooks without changes
- **+** Workspace mode for monorepos with concurrent runs of independent projects
- **+** Uses uv for Python environments and shares toolchains across hooks
- **−** Not AI-specific; it is a general hook runner, so it fits this list loosely
- **−** Built-in Rust hooks cover only some common hooks, not the full pre-commit ecosystem
- **−** Building from source needs Rust 1.97 or newer
- **−** Native prek.toml config is not portable to the original pre-commit

<sub>no GPU · Docker · [Repo](https://github.com/j178/prek) · [📖 Docs ↗](https://prek.j178.dev/) · [🌐 Site ↗](https://prek.j178.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/prek/)</sub>

<a name="front-end-checklist"></a>
### #&#8288;20 [front-end-checklist](https://github.com/thedaviddias/front-end-checklist) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

**Front-end rules checklist with an MCP server for agent code review.**

A corpus of 386 English front-end rules across 11 categories (HTML, CSS, JavaScript, performance, accessibility, SEO, security, images, testing, privacy, i18n), each with a priority level, remediation guidance and verification steps. It is readable on the website or in the README, and a hosted MCP server and installable skills let agents review code or audit public URLs against the same rules.

- **+** 386 rules with Critical/High/Medium/Low priorities, grouped into 11 categories
- **+** Hosted MCP server exposes 11 tools, including review_code, search_rules and audit_url
- **+** Skills install with `npx skills add frontendchecklist/skills`, global or per rule
- **+** MIT licensed; rules also usable as a plain README checklist without any tooling
- **−** Content repo, not a linter: findings come from an agent applying the rules
- **−** audit_url only handles public https:// pages
- **−** Security, privacy and i18n categories are thin (22, 5 and 5 rules)
- **−** MCP tool discovery can be lazy in some clients; the prompt must name the server

<sub>no GPU · Needs MCP-compatible client, pnpm (for contributing) · safety checks passed 13 of 14 · [Repo](https://github.com/thedaviddias/front-end-checklist) · [📖 Docs ↗](https://frontendchecklist.io/mcp) · [🌐 Site ↗](https://frontendchecklist.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/front-end-checklist/)</sub>

<a name="ginkgo"></a>
### #&#8288;21 [ginkgo](https://github.com/onsi/ginkgo) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · MIT · Nov 2026</sub>

**BDD-style testing framework for Go with a spec DSL and CLI.**

Ginkgo is a Go testing framework built on the standard `testing` package. It provides nestable Describe, Context and When containers, setup nodes and It subjects, and pairs with the Gomega matcher library. The `ginkgo` CLI runs suites in random order or in parallel (`ginkgo -p`), filters by label, and writes machine-readable reports. The repo also ships Claude Code skills as a plugin.

- **+** Parallel spec runs with `ginkgo -p` and reproducible random ordering
- **+** Per-spec timeouts and context cancellation help prevent hung suites
- **+** Labels and CLI filters run subsets of specs; reports export in several machine-readable formats
- **+** `ginkgo watch` reruns specs on file changes
- **−** Go only; the DSL differs from plain `go test` table-driven style
- **−** Needs the separate Gomega library for its assertion matchers
- **−** Parallel suites require following specific patterns to avoid shared-state conflicts
- **−** Nested closure DSL can be harder to navigate than flat Go tests

<sub>no GPU · Needs Go, Gomega · [Repo](https://github.com/onsi/ginkgo) · [📖 Docs ↗](https://onsi.github.io/ginkgo/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ginkgo/)</sub>

<a name="pr-lens"></a>
### #&#8288;22 [pr-lens](https://github.com/coldteadotai/pr-lens) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Nov 2026</sub>

**Posts animated architecture and data-flow diagrams as pull request comments.**

PR Lens reads a pull request diff with an LLM and posts a comment containing animated diagrams of the components touched and the calls between them, with new, changed and removed parts colored. It runs as a hosted GitHub App, a GitHub Action or GitLab/Bitbucket pipeline with your own model key, or through an agent skill and CLI that draw diagrams before a PR exists. An interactive canvas offers walkthroughs and per-arrow payload views.

- **+** Covers GitHub, GitLab and Bitbucket, with an Action, CI component and pipe
- **+** Action accepts Gemini, OpenAI or any OpenAI-compatible endpoint via base-url
- **+** Corrections like rename and exclude live in pr-lens.yml and survive reruns
- **+** Agent skill and CLI validate diagrams locally before any PR is opened
- **−** Diagrams are LLM-generated, so names can be wrong and need config fixes
- **−** Diff is sent to the chosen model provider
- **−** Action comments are static; the checkbox view selection works only in the App
- **−** On GitLab.com, project access tokens need a paid plan; Free uses a personal token

<sub>Needs GitHub App, GitLab CI or Bitbucket Pipelines, LLM API key (Gemini, OpenAI or compatible), Node.js (npx CLI) · Models: Gemini, OpenAI, OpenAI-compatible /chat/completions · [Repo](https://github.com/coldteadotai/pr-lens) · [▶️ Demo ↗](https://prlens.dev/c/uSdxMcPBFwhfgfaGh-dveQ) · [🌐 Site ↗](https://prlens.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pr-lens/)</sub>

<a name="testsprite-cli"></a>
### #&#8288;23 [testsprite-cli](https://github.com/testsprite/testsprite-cli) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Nov 2026</sub>

**CLI that runs cloud end-to-end tests on your app and feeds failures to coding agents.**

Official CLI for the TestSprite testing service. You write test plans as JSON in plain language, or have the service propose them. Tests run against a live app in the cloud, or a local one through a tunnel. A failed run comes back as one failure bundle that a coding agent can read, fix and rerun. `testsprite setup` installs a verification skill for eight agents, including Claude, Cursor, Cline and Codex.

- **+** `test failure get` returns one self-contained failure bundle, plus non-zero exit codes for CI and agents
- **+** Installs its skill for eight agents: claude, cursor, cline, windsurf, antigravity, kiro, copilot, codex
- **+** Tunnel lets cloud tests reach localhost apps, with batch runs of 1-10 concurrent tests
- **+** Plans are plain-language JSON with a published schema, so no browser code is needed
- **−** Requires a TestSprite account and API key; tests execute on their hosted backend, not locally
- **−** Plan generation and runs spend workspace credits; a PRD upload bills 0.5 credits
- **−** Local projects skip plan generation, so plans must be written by hand
- **−** Needs Node.js 20.19+, 22.13+ or 24+; the CLI is a client, not a self-hostable engine

<sub>no GPU · Needs TestSprite cloud account and API key, Node.js 20.19+, 22.13+ or 24+ · [Repo](https://github.com/testsprite/testsprite-cli) · [📖 Docs ↗](https://www.testsprite.com/docs) · [🌐 Site ↗](https://www.testsprite.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/testsprite-cli/)</sub>

<a name="solopi"></a>
### #&#8288;24 [solopi](https://github.com/alipay/solopi) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Nov 2026</sub>

**Mobile app test automation with Android record/replay and an agent execution harness.**

SoloPi records and replays UI flows on real Android devices, usually without adding an SDK to the app under test. It also includes an Electron-style Desktop workbench and a Skill/Harness layer that re-checks the current page before each agent action. Results are judged separately from action success as passed, failed or not_tested, with screenshots, logs and reports saved per run.

- **+** Target apps usually need no SoloPi SDK; works on real devices
- **+** Separates action execution from pass/fail, with passed, failed and not_tested verdicts
- **+** Saves screenshots, logs, action receipts and structured reports for each run
- **+** Apache-2.0 with Android app, Desktop and CLI entry points
- **−** Desktop control, Skill/Harness are Beta; iOS (WDA) and HarmonyOS NEXT are experimental
- **−** Android performance plugins and recording are not ported to iOS or NEXT
- **−** Multi-device control was never open-sourced and is unavailable
- **−** Built-in workflow templates need specific apps, accounts and starting pages

<sub>Needs adb, Node.js 22.14.0 (Desktop), npm, Python 3.9+, Android device with USB debugging · [Repo](https://github.com/alipay/solopi) · [🌐 Site ↗](https://www.solopi.cn/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/solopi/)</sub>

<a name="tflint"></a>
### #&#8288;25 [tflint](https://github.com/terraform-linters/tflint) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MPL-2.0 · Nov 2026</sub>

**Pluggable linter for Terraform configurations.**

TFLint is a Go command-line linter for Terraform code. The core is a plugin framework, and rules come from rulesets: one for the Terraform language is bundled, and AWS, Azure and Google Cloud rulesets install with `tflint --init`. It catches things like invalid instance types, deprecated syntax and unused declarations, and outputs default, JSON, checkstyle, JUnit, compact or SARIF.

- **+** Plugin rulesets for AWS, Azure and GCP catch provider-specific errors such as invalid instance types
- **+** Custom rules via your own plugin or Rego policies through the OPA ruleset
- **+** Output formats include JSON, SARIF, JUnit and checkstyle for CI; a setup-tflint GitHub Action exists
- **+** Has --fix for automatic fixes, --recursive for multi-directory runs, and a language server mode
- **−** Cloud provider checks need separate plugins installed through tflint --init
- **−** Release binaries fall under both MPL 2.0 and BUSL 1.1 because of some terraform package files
- **−** Cosign signature verification is deprecated in favor of GitHub attestations
- **−** Not AI-based; rule-driven static checks only, so coverage depends on available rulesets

<sub>no GPU · Docker · Needs GitHub (plugin download via tflint --init) · [Repo](https://github.com/terraform-linters/tflint) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tflint/)</sub>

<a name="reticle"></a>
### #&#8288;26 [reticle](https://github.com/reticlehq/reticle) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · custom license · Nov 2026</sub>

**MCP tools that let coding agents verify a running app and return pass, fail or unknown.**

Reticle adds a dev-only SDK to your web or desktop app and exposes reticle_* MCP tools so a coding agent can click through the running app and read network responses, store state, console output and source lines. Each check returns a verdict of yes, no or unknown, with the evidence and a file:line to fix. Passing journeys can be saved as flows, replayed without a model, and enforced in CI with `reticle gate`.

- **+** Verdict includes the request, state change and console line behind it, plus a file:line
- **+** Returns `unknown` when it cannot decide, so there is no silent pass
- **+** Saved flows replay deterministically with no model; `reticle gate` checks them in CI
- **+** Production builds exclude the SDK; bridge binds to 127.0.0.1 only
- **−** Server and CLI are FSL-1.1-ALv2 (source-available), not OSI open source until two years on
- **−** `reticle init` edits build config, agent rules files, MCP config and prompt hooks
- **−** Anonymous usage telemetry is on by default; opt out with an env var or command
- **−** Harness and dashboard are on the hosted platform; full open-source scope is unclear

<sub>no GPU · Needs Node 20.11+, Chromium browser, MCP-capable coding agent · port 4400 · [Repo](https://github.com/reticlehq/reticle) · [▶️ Demo ↗](https://player.mux.com/ap7hnnu4j36BRV6wEcop1NZVpJTjVSedxpW1AaXdD3I) · [📖 Docs ↗](https://docs.reticle.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reticle/)</sub>

<a name="crit"></a>
### #&#8288;27 [crit](https://github.com/tomasz-tomczyk/crit) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Nov 2026</sub>

**Browser UI for commenting on a coding agent's plans, diffs and running apps.**

Crit is a single Go binary that opens a local browser review UI for markdown plans, git diffs, static HTML files, or a proxied dev server. You comment on lines or ranges, and the agent receives them through a /crit slash command or `crit comment`. It also syncs comments with GitHub PRs and GitLab MRs, and can share reviews through crit.md.

- **+** Runs locally as one binary; install via brew, Go, Nix, AUR or release download
- **+** Separate review modes for markdown, git diffs, static HTML and a live proxied app
- **+** Two-way comment sync with GitHub PRs and GitLab MRs, including self-managed GitLab
- **+** Integrates with Claude Code, Cursor, Copilot, Codex, Aider, Cline and others
- **−** Live mode needs manual cookie forwarding when the app uses host-scoped session logins
- **−** Story mode run from the terminal costs extra LLM spend, about $1 to $1.40 per complex PR
- **−** Send-to-agent is experimental and needs agent_cmd set in global config
- **−** Sharing relies on crit.md or a separately hosted crit-web instance

<sub>no GPU · Needs git, gh (GitHub PR sync), glab (GitLab MR sync), a coding agent CLI · [Repo](https://github.com/tomasz-tomczyk/crit) · [🌐 Site ↗](https://crit.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/crit/)</sub>

<a name="kodus-ai"></a>
### #&#8288;28 [kodus-ai](https://github.com/kodustech/kodus-ai) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · custom license · Nov 2026</sub>

**AI pull request reviewer for GitHub, GitLab, Bitbucket, Azure DevOps and Forgejo.**

Kodus reviews pull requests with an LLM you configure (bring your own key for OpenAI, Anthropic, Gemini, Vertex AI, Novita or any OpenAI-compatible endpoint). Reviews follow plain-language Kody Rules and can also run locally or in CI through a CLI. It is a TypeScript monorepo (NestJS API, worker, webhooks service, Next.js dashboard) that can be self-hosted or used as Kodus Cloud.

- **+** Supports five Git hosts: GitHub, GitLab, Bitbucket, Azure DevOps and Forgejo
- **+** Bring-your-own-key model layer, including OpenAI-compatible and self-hosted models
- **+** CLI reviews working tree, staged diff, branch or commit, and runs in CI/CD
- **+** Custom review rules written in plain language, scoped by repo or path
- **−** Community edition limits Kody Rules to 10 and active plugins to 3
- **−** Cockpit metrics are Teams and Enterprise only; SSO, RBAC and audit logs are Enterprise only
- **−** Self-hosting needs a VM with 2 CPU cores, 8 GB RAM and 60 GB disk
- **−** Self-hosted instances send a daily anonymous heartbeat unless disabled by environment variable

<sub>RAM ≥ 8 GB · no GPU · Docker + Compose · Needs Docker, LLM provider API key or OpenAI-compatible endpoint · Models: OpenAI, Anthropic, Google Gemini, Vertex AI, Novita · [Repo](https://github.com/kodustech/kodus-ai) · [📖 Docs ↗](https://docs.kodus.io) · [🌐 Site ↗](https://kodus.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kodus-ai/)</sub>

<a name="codediff-nvim"></a>
### #&#8288;29 [codediff.nvim](https://github.com/esmuellert/codediff.nvim) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Nov 2026</sub>

**Neovim diff viewer for reviewing coding-agent changes as they land.**

codediff.nvim is a Neovim plugin that shows VSCode-style side-by-side or inline diffs with line- and character-level highlighting. It watches the repository so changes made by a background coding agent appear live, and lets you stage, unstage or discard files and hunks. It also covers revision, PR and history review, plus merge conflict resolution per block or whole file.

- **+** Explorer auto-refreshes via file watching with polling fallback, so agent edits show up live
- **+** Stage, unstage or discard per file or per hunk from the review view
- **+** Prebuilt diff library downloads automatically; no compiler needed
- **+** Built-in merge conflict view with per-block and whole-file accept keymaps
- **−** Works only inside Neovim; no standalone or GUI mode
- **−** Gutter signs require Neovim 0.10 or newer
- **−** Core diff is a native library downloaded from GitHub releases on first use
- **−** Line stats and move detection are off by default and must be enabled

<sub>no GPU · Needs Neovim 0.7+ (0.10+ recommended), Git, curl or wget (PowerShell on Windows) · [Repo](https://github.com/esmuellert/codediff.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codediff-nvim/)</sub>

<a name="memlab"></a>
### #&#8288;30 [memlab](https://github.com/meta/memlab) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Nov 2026</sub>

**JavaScript memory leak finder using Puppeteer scenarios and heap snapshot analysis.**

memlab runs a Puppeteer scenario against a web page, compares V8 heap snapshots before and after an action, and prints retainer traces for leaked objects. It also offers a heap traversal API, a CLI for analyzing .heapsnapshot files from Chromium, Node.js, Electron and Hermes, and Node.js memory assertions for unit tests. An MCP server and four agent skills let coding assistants investigate snapshots.

- **+** Retainer traces show the reference chain from GC root to each leaked object
- **+** Reads heap snapshots from Chromium, Node.js, Electron and Hermes
- **+** Memory assertions run inside Jest-style unit tests and CI
- **+** Custom leak detectors via a leakFilter callback in the scenario file
- **−** Readable traces require non-minified code or readable names on the site under test
- **−** Scenarios must be hand-written with the Puppeteer API
- **−** MCP server suggests an 8 GB Node heap setting for large snapshots
- **−** No tagged release is listed on the repository

<sub>no GPU · Needs Node.js 16+, Puppeteer · [Repo](https://github.com/meta/memlab) · [📖 Docs ↗](https://meta.github.io/memlab/docs/intro) · [🌐 Site ↗](https://meta.github.io/memlab) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/memlab/)</sub>

<a name="mantis"></a>
### #&#8288;31 [mantis](https://github.com/google/mantis) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · Apache-2.0 · Nov 2026</sub>

**Agent skills and ADK pipeline that find, reproduce and patch code vulnerabilities.**

Mantis is a set of agent skills plus a Google ADK reference harness that runs a security review pipeline over a file or repository: threat model, hypotheses, research, triage, reproduction, patching and severity calibration. It also includes a GitHub Action for pull request scans, which is untested. The README labels it demonstration-only and says to run it only in isolated environments.

- **+** Covers the full loop: threat model, research, dedup, triage, reproduction, patch with adversarial check
- **+** Severity calibration rubric aims to limit inflated critical findings
- **+** Run options: --focus, --exclude, --max-tokens cap, --parallel, exportable knowledge base
- **+** Skills are separate from the harness, so they can be ported to other frameworks
- **−** README states it is for demonstration, not production use
- **−** Pull request GitHub Action has not been run end-to-end on a live project
- **−** Executes model-generated code; user must provide strong isolation
- **−** Findings need manual expert verification; hallucinated results are possible

<sub>no GPU · Needs Python 3, python3-venv, Google ADK, Google Cloud ADC (Vertex AI), SQLite · Models: Vertex AI · [Repo](https://github.com/google/mantis) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mantis/)</sub>

<a name="git-lrc"></a>
### #&#8288;32 [git-lrc](https://github.com/hexmostech/git-lrc) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Oct 2026</sub>

**Git pre-commit hook that runs an AI review on each staged diff.**

git-lrc is a Go CLI that hooks into git commit and sends the staged diff to an AI reviewer, then opens a local browser UI with inline comments, severity badges and risk-ranked hunks. Each commit gets a status line in the git log (ran, vouched or skipped, with iteration count and coverage). It uses the LiveReview service with a Gemini key by default, and also supports OpenAI, Claude, DeepSeek and OpenRouter keys.

- **+** Triggers on git commit, so it works across editors and AI assistants
- **+** Records review status, iterations and coverage in each commit's git log message
- **+** Agent mode returns JSON non-interactively for coding agents and CI
- **+** Supports BYOK connectors: OpenAI, Claude, DeepSeek, OpenRouter, Anthropic-compatible APIs
- **−** Setup needs a LiveReview account (Hexmos sign-in); review is not fully local
- **−** Free tier capped at 30k LOC per month; paid plans beyond that
- **−** Self-hosting, SSO and custom domains are Enterprise-only
- **−** License is reported as NOASSERTION, so terms are unclear

<sub>no GPU · Needs LiveReview account (Hexmos sign-in), Gemini API key or other AI provider key, codebase-memory-mcp (optional, auto-installed for risk scoring) · Models: Gemini, OpenAI, Claude, DeepSeek, OpenRouter · [Repo](https://github.com/hexmostech/git-lrc) · [🌐 Site ↗](https://hexmos.com/livereview/git-lrc/pricing/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/git-lrc/)</sub>

<a name="pyscn"></a>
### #&#8288;33 [pyscn](https://github.com/ludo-technologies/pyscn) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (5) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.1k · MIT · Nov 2026</sub>

**Static code quality analyzer for Python with a 0-100 score and HTML report.**

pyscn is a Go CLI that parses Python with tree-sitter and reports dead code, duplicate code (Type 1-4 clones), cyclomatic and cognitive complexity, circular imports, layer violations and class coupling and cohesion. It outputs a 0-100 score with an A-F grade, an HTML or JSON report, and a `pyscn check` command for CI gates. It also ships Agent Skills and a `pyscn-mcp` server so coding agents can run the analyses.

- **+** Covers dead code, clones, complexity, architecture and class design in one run
- **+** `pyscn check` gives a pass/fail CI gate with configurable thresholds
- **+** Ships Agent Skills and an MCP server for Claude Code, Cursor and others
- **+** Runs without install via uvx or pipx; config in .pyscn.toml or pyproject.toml
- **−** Static structural analysis only; does not review logic or generate tests
- **−** PyPI wheels dropped for Intel Macs since v1.5.1; needs brew or go install
- **−** Analyzes Python only; other languages need the separate polyscan tool
- **−** Weekly GitHub audit app is a separate hosted service, free only for public repos

<sub>no GPU · [Repo](https://github.com/ludo-technologies/pyscn) · [📖 Docs ↗](https://docs.codescan.dev/pyscn/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pyscn/)</sub>

<a name="deepsec"></a>
### #&#8288;34 [deepsec](https://github.com/vercel-labs/deepsec) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: weak (28) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · Apache-2.0 · Nov 2026</sub>

**Agent-driven vulnerability scanner for reviewing all code in large existing repos.**

deepsec runs regex matchers to find candidate sites in a repository, then has AI coding agents investigate each one and emit findings with recommendations. State lives in a `.deepsec/` folder, runs resume after interruption, and large repos can fan out across Vercel Sandbox microVMs. It supports a PR-mode diff review, revalidation of past findings, and export to JSON or markdown.

- **+** Interrupted runs resume and skip files already analyzed
- **+** Free regex scan stage before paid AI review; `process --diff` limits review to changed files
- **+** Spend and time caps via `--max-cost-usd` and `--max-duration`
- **+** Bring your own OpenAI or Anthropic key, or use Vercel AI Gateway
- **−** README warns full scans of large codebases can cost thousands to tens of thousands of dollars
- **−** Runs like a coding agent with full shell access; prompt injection from dependencies is a stated risk
- **−** Distributed execution depends on Vercel Sandbox
- **−** No tagged release; installed via npx

<sub>no GPU · Needs Node.js, pnpm, Vercel AI Gateway or OpenAI/Anthropic API key, Vercel Sandbox (optional) · Models: OpenAI, Anthropic, Vercel AI Gateway, custom HTTPS provider · [Repo](https://github.com/vercel-labs/deepsec) · [📖 Docs ↗](https://github.com/vercel-labs/deepsec/blob/main/docs/getting-started.md) · [🌐 Site ↗](https://deepsec.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/deepsec/)</sub>

<a name="pre-commit-hooks"></a>
### #&#8288;35 [pre-commit-hooks](https://github.com/pre-commit/pre-commit-hooks) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (52) · Freshness: recent (77) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · MIT · Nov 2026</sub>

**Collection of file-hygiene and syntax-check hooks for the pre-commit framework.**

A set of hooks for pre-commit that run on staged files before a commit. They check JSON, YAML, TOML, XML and Python syntax, detect private keys and AWS credentials, block large files and merge-conflict markers, and fix whitespace, line endings and file endings. Configured through .pre-commit-config.yaml or installed with pip. It has no AI features; it is rule-based commit-time linting.

- **+** Many single-purpose hooks; enable only the ones you need by hook id
- **+** Several hooks autofix files: whitespace, EOF, line endings, JSON formatting, requirements sorting
- **+** Checks for private keys and AWS credentials before commit
- **+** Also installable standalone with pip install pre-commit-hooks
- **−** No AI features; rule-based checks only, so it fits this list loosely
- **−** Normal use requires the pre-commit framework
- **−** Several hooks are Python-specific (check-ast, debug-statements, name-tests-test)
- **−** file-contents-sorter removes blank lines and ignores comments

<sub>no GPU · Needs pre-commit, git, git-lfs (optional, >=2.2.1) · [Repo](https://github.com/pre-commit/pre-commit-hooks) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pre-commit-hooks/)</sub>

<a name="eslint-plugin-react"></a>
### #&#8288;36 [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (64) · Freshness: recent (70) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · MIT · Oct 2026</sub>

**React-specific lint rules for ESLint, covering JSX style and component correctness.**

An ESLint plugin that adds React and JSX rules, such as jsx-key, display-name, button-has-type, jsx-no-bind and hook-use-state. It ships recommended, all and jsx-runtime presets for both legacy .eslintrc and flat eslint.config.js setups. Shared settings cover the React version, pragma and custom component wrappers. It is a static linter with no AI component.

- **+** Presets for legacy .eslintrc and flat config: recommended, all, jsx-runtime
- **+** Many rules, several with --fix autofix or editor suggestions
- **+** Shared settings detect React version and handle wrappers like Mobx observer
- **+** MIT licensed; installs as one npm dev dependency alongside eslint
- **−** Not an AI tool; it fits this list's categories only loosely
- **−** Many JSX formatting rules overlap with dedicated formatters
- **−** Last tagged release is 2025-04-03, well behind recent commits
- **−** Presets do not set files or globals, so manual config is needed

<sub>no GPU · Needs eslint, npm · [Repo](https://github.com/jsx-eslint/eslint-plugin-react) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/eslint-plugin-react/)</sub>

<a name="codegpt"></a>
### #&#8288;37 [codegpt](https://github.com/appleboy/codegpt) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Sep 2026</sub>

**Go CLI that writes git commit messages and code reviews from diffs.**

CodeGPT is a Go command-line tool that reads your git diff and generates conventional-commit messages or short code review summaries. It installs a git prepare-commit-msg hook and talks to OpenAI, Azure OpenAI, Gemini, Anthropic, Groq, Ollama, OpenRouter or a LiteLLM proxy. Prompts are editable templates, and API keys can come from the OS keyring or a shell helper command.

- **+** Supports eight provider options, including local Ollama and a LiteLLM proxy
- **+** Installs a prepare-commit-msg hook so messages are generated during git commit
- **+** Prompt templates are editable files, loaded with `codegpt prompt --load`
- **+** API key helper command pulls keys from 1Password, AWS or GCP secret stores
- **−** Only commit messages and brief reviews; it does not edit code or run commands
- **−** Default max_tokens is 300, which can truncate longer outputs
- **−** Output language options are limited (en, zh-tw, zh-cn, ja)
- **−** No Docker image; install is by script, binary, Homebrew, Chocolatey or go install

<sub>no GPU · Docker · Needs git, API key for an LLM provider, or a local Ollama server · Models: OpenAI (gpt-5, gpt-4o, gpt-4), Azure OpenAI, Gemini, Anthropic, Ollama · [Repo](https://github.com/appleboy/codegpt) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codegpt/)</sub>

<a name="ai-codereview-gitlab"></a>
### #&#8288;38 [ai-codereview-gitlab](https://github.com/sunmh207/ai-codereview-gitlab) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: weak (27) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

**LLM reviewer for GitLab merge requests and pushes, with chat notifications.**

Receives GitLab webhooks for Push and Merge Request events, sends the diff to a configured LLM, and posts the review back as a Note on the MR or commit. It also pushes results to DingTalk, WeCom or Feishu, and includes a Streamlit dashboard and daily reports built from GitLab, GitHub and Gitea commits. An optional agentic mode lets the model read files and run read-only shell commands in a local clone.

- **+** Supports DeepSeek, ZhipuAI, OpenAI, Anthropic, Qwen and Ollama via one LLM_PROVIDER setting
- **+** Agentic mode falls back to diff_only on clone, fetch, LLM or tool failure
- **+** Agent shell is sandboxed: read-only allowlist, path checks, 30s timeout
- **+** Includes a dashboard on port 5002 with project and developer statistics
- **−** README and docs are mainly in Chinese
- **−** Webhook flow is documented for GitLab only; GitHub and Gitea appear only in daily reports
- **−** Agentic mode needs 50GB+ disk and uses 3-10x the tokens of diff_only
- **−** Some features sit in a separate Pro edition

<sub>no GPU · Docker + Compose · Needs GitLab access token, LLM provider API key or Ollama, DingTalk, WeCom or Feishu webhook (optional) · Models: DeepSeek, ZhipuAI, OpenAI, Anthropic, Qwen · port 5001 · [Repo](https://github.com/sunmh207/ai-codereview-gitlab) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-codereview-gitlab/)</sub>

<a name="chatgpt-codereview"></a>
### #&#8288;39 [chatgpt-codereview](https://github.com/anc95/chatgpt-codereview) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (39) · Freshness: active (99) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · ISC · Aug 2026</sub>

**GitHub bot and Action that reviews pull request diffs with an LLM.**

Probot-based GitHub app that reviews pull requests with OpenAI-compatible models and posts comments in the PR timeline and file changes. It re-reviews changed files after each push. It runs as a GitHub Action, a self-hosted Node app under pm2, or a Docker container, and supports OpenAI, Azure deployments and GitHub Models.

- **+** Runs as a GitHub Action with a short workflow file, or as a self-hosted Probot app
- **+** Supports OpenAI endpoints, Azure deployments and GitHub Models
- **+** Filters files with IGNORE_PATTERNS and INCLUDE_PATTERNS; skips diffs over MAX_PATCH_LENGTH
- **+** Review language, prompt, temperature and max_tokens set through environment variables
- **−** Hosted bot is test-only and rate-limited on AWS Lambda; README advises self-deploying
- **−** Sends diffs to an external LLM API, so an API key and usage cost are required
- **−** GitHub only; no GitLab or other platform support mentioned
- **−** Docker section lists no exposed port or full env list; relies on .env.example

<sub>no GPU · Docker · Needs GitHub App or GitHub Actions, OpenAI-compatible API, Azure OpenAI or GitHub Models, Node.js, pm2 (self-hosting) · Models: OpenAI GPT models, Azure OpenAI deployments, GitHub Models · [Repo](https://github.com/anc95/chatgpt-codereview) · [▶️ Demo ↗](https://github.com/apps/cr-gpt) · [📖 Docs ↗](https://github.com/marketplace/actions/chatgpt-codereviewer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chatgpt-codereview/)</sub>

<a name="run-gemini-cli"></a>
### #&#8288;40 [run-gemini-cli](https://github.com/google-github-actions/run-gemini-cli) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (25) · Freshness: active (98) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Aug 2026</sub>

**GitHub Action that runs Gemini CLI for PR review, issue triage and @-mention tasks.**

A GitHub Action that installs and runs Gemini CLI inside workflows. Prebuilt workflows handle pull request review, issue triage and a general assistant triggered by comments such as `@gemini-cli /review`, with a dispatch workflow routing events. Authentication uses a Gemini API key, Vertex AI, Gemini Code Assist or Workload Identity Federation, and a `GEMINI.md` file supplies project context.

- **+** Prebuilt dispatch, PR review, issue triage and assistant workflows to copy into .github/workflows
- **+** Multiple auth paths: API key, Vertex AI, Code Assist, Workload Identity Federation
- **+** Optional custom GitHub App auth and OpenTelemetry export to your Google Cloud project
- **+** Gemini CLI version is pinnable (latest, preview, nightly, or a specific version or git ref)
- **−** Tied to Gemini models; no other model providers are documented
- **−** Runs only on GitHub Actions, not other CI systems
- **−** Setting `DEBUG` env var makes the CLI hang, per the README warning
- **−** Needs .gitignore edits and secrets or variables configured before first use

<sub>no GPU · Needs GitHub Actions, Gemini CLI, Gemini API key or Google Cloud (Vertex AI / Code Assist) · Models: Gemini · [Repo](https://github.com/google-github-actions/run-gemini-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/run-gemini-cli/)</sub>

<a name="shippie"></a>
### #&#8288;41 [shippie](https://github.com/mattzcarey/shippie) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (29) · Freshness: active (89) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Jul 2026</sub>

**Code-review agent that comments on pull requests and staged diffs.**

Shippie runs an agent loop on the flue framework and pi that reads a diff, explores the codebase with developer tools, and posts review comments on issues such as exposed secrets, slow code and unhandled edge cases. It runs as a GitHub Action, locally via `npx shippie review` on staged changes, in GitLab CI, or on Node and Cloudflare. It can also act as an MCP client.

- **+** Runs as a GitHub Action, GitLab CI job, local CLI, Node server or Cloudflare deployment
- **+** Supports Anthropic, OpenAI, OpenRouter and Cloudflare Workers AI providers
- **+** Acts as an MCP client to reach browser, observability and docs tools
- **+** Reads AGENTS.md, CLAUDE.md and Agent Skills; `/shippie review` comment triggers it on demand
- **−** Requires a hosted provider API key; no local model support is documented
- **−** GitHub Action needs a full checkout (fetch-depth: 0) and PR write permissions
- **−** Local mode reviews only staged changes (git diff --cached)
- **−** Depends on the flue and pi frameworks; development needs Node >= 22.19

<sub>no GPU · Docker · Needs Anthropic, OpenAI, OpenRouter or Cloudflare Workers AI API key, Node >= 22.19, GitHub Actions or GitLab CI (optional) · Models: Anthropic, OpenAI, OpenRouter, Cloudflare Workers AI · [Repo](https://github.com/mattzcarey/shippie) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shippie/)</sub>

<a name="gentleman-guardian-angel"></a>
### #&#8288;42 [gentleman-guardian-angel](https://github.com/gentleman-programming/gentleman-guardian-angel) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (9) · Freshness: active (90) · Maintenance: weak (2) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Jul 2026</sub>

**Git pre-commit hook that reviews staged files against AGENTS.md using any LLM.**

GGA is a pure Bash CLI that installs a git pre-commit (or commit-msg) hook and sends staged files to an AI provider to check them against coding standards written in AGENTS.md. It supports hosted CLIs and APIs such as Claude, Gemini, Codex and GitHub Models, plus local Ollama and LM Studio. It also offers a CI mode, a full-PR review mode and a cache that skips unchanged files.

- **+** Pure Bash core; installs via Homebrew or install.sh, with no runtime framework
- **+** Supports 11 providers, including local Ollama and LM Studio
- **+** Caching skips unchanged files; --pr-mode reviews a whole PR and --ci the last commit
- **+** Runs on macOS, Linux, Windows (Git Bash) and WSL; 266 tests reported
- **−** Each provider needs its own CLI or API account installed separately
- **−** Review quality depends on how well AGENTS.md is written
- **−** LLM review on every commit adds latency and may send code to third parties
- **−** On Oh My Zsh, the git plugin's gga alias conflicts and needs unalias

<sub>no GPU · Needs Bash 5.0+, git, an AI provider CLI or API (Claude, Gemini, Codex, Ollama, etc.) · Models: Claude, Gemini, Codex, OpenCode, Cursor Agent · [Repo](https://github.com/gentleman-programming/gentleman-guardian-angel) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gentleman-guardian-angel/)</sub>

<a name="shortest"></a>
### #&#8288;43 [shortest](https://github.com/antiwork/shortest) <sub>score [28](../README.md#-how-we-rank "Score 28/100. Adoption: known (45) · Freshness: slowing (48) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.7k · MIT · May 2026</sub>

**Write end-to-end browser tests in plain English, executed by Claude via Playwright.**

Shortest is a TypeScript test framework where each test is a natural-language sentence. Claude, called through the Anthropic API, drives a Playwright browser to carry it out. It supports `.after()` callbacks for custom assertions, lifecycle hooks, chained tests, API endpoint tests, GitHub 2FA login and Mailosaur email checks.

- **+** Tests are plain-English strings; `.after()` callbacks allow Playwright and DB assertions in code
- **+** Built on Playwright, with browser context options passed through the config file
- **+** Headless mode for CI, with an example GitHub Actions workflow in the repo
- **+** Built-in GitHub 2FA (TOTP) login and Mailosaur email validation
- **−** Only the Anthropic provider is documented; an API key is required and each run costs tokens
- **−** Last tagged release is 2025-04-01
- **−** AI-executed steps can be non-deterministic and slower than scripted Playwright tests
- **−** Repo also contains a web app that needs Clerk, Postgres, Stripe and Mailosaur to run locally

<sub>no GPU · Needs Anthropic API, Playwright, Mailosaur (optional), Clerk, Vercel Postgres, Stripe (web app only) · Models: Anthropic Claude · port 3000 · [Repo](https://github.com/antiwork/shortest) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/shortest/)</sub>

<a name="claude-code-security-review"></a>
### #&#8288;44 [claude-code-security-review](https://github.com/anthropics/claude-code-security-review) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: popular (54) · Freshness: slowing (33) · Maintenance: weak (5) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.9k · MIT · Feb 2026</sub>

**GitHub Action that has Claude review pull request diffs for security issues.**

A Python-based GitHub Action that sends pull request diffs to Claude Code and posts security findings as line comments on the PR. A filter step drops categories such as denial of service, rate limiting and open redirects. The README also describes a customizable /security-review slash command in Claude Code.

- **+** On PRs it analyzes only changed files and comments on specific lines
- **+** Custom scan and false-positive filtering instructions load from text files
- **+** Inputs for excluded directories, model name and timeout in minutes
- **+** Outputs findings-count and a results JSON file, uploaded as an artifact by default
- **−** README says it is not hardened against prompt injection; use on trusted PRs only
- **−** Requires an Anthropic API key enabled for Claude API and Claude Code
- **−** Default model is claude-opus-4-1-20250805, which may raise per-run cost
- **−** Default filter excludes DoS, rate-limiting and open-redirect findings

<sub>no GPU · Needs GitHub Actions, Anthropic Claude API key · Models: claude-opus-4-1-20250805 (default), Other Claude models via claude-model input · [Repo](https://github.com/anthropics/claude-code-security-review) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-security-review/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
