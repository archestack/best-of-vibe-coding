# 🧪 Code review and testing reviews · Best of Vibe Coding

AI tools that review pull requests, write tests or find bugs, run in your CI or on your machine. Back to the [leaderboard](../README.md#-code-review-and-testing).

<sub>🌐 Also on the web: [Code review and testing on archestack.com](https://archestack.com/best-of-vibe-coding/code-review/), each project on its own page.</sub>

<a name="open-code-review"></a>
### 🥇 [open-code-review](https://github.com/alibaba/open-code-review) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · Apache-2.0 · Oct 2026</sub>

**CLI that reviews Git diffs with an LLM agent and line-level comments.**

Open Code Review is a Go CLI (`ocr`) that reads a Git diff, groups related files into bundles, and runs each bundle through a tool-using LLM agent that produces structured review comments. File selection, rule matching, comment positioning and reflection are done by deterministic code rather than prompts. `ocr scan` reviews whole files when there is no diff, and delegation mode lets an existing coding agent do the review with its own model.

- **+** Deterministic file selection and bundling; each bundle runs as an isolated sub-agent
- **+** Reviews workspace changes, branch ranges, single commits, or full files via `ocr scan`
- **+** Sessions can be resumed and browsed in a viewer; JSON output for automation
- **+** Plugins for Claude Code, Codex, Cursor, Kimi Code, OpenCode; CI docs for GitHub, GitLab, Gerrit
- **−** Requires Git >= 2.41 and a configured LLM endpoint, unless delegation mode is used
- **−** Recall is lower than general-purpose agents by the README's own benchmark
- **−** Benchmark figures are published by the project itself, not independently verified
- **−** No Docker or Compose files detected

<sub>no GPU · Needs Git >= 2.41, LLM provider API · Models: configurable LLM providers, custom providers · [Repo](https://github.com/alibaba/open-code-review) · [📖 Docs ↗](https://open-codereview.ai/docs) · [🌐 Site ↗](https://open-codereview.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-code-review/)</sub>

<a name="react-doctor"></a>
### 🥈 [react-doctor](https://github.com/millionco/react-doctor) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (95) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

**CLI that scans React codebases for state, performance, security and accessibility issues.**

React Doctor runs deterministic checks over a React project and reports issues in state and effects, performance, architecture, security, accessibility and maintainability. It covers Next.js, Vite, Astro, TanStack, React Native and Expo. It also installs as a skill for coding agents, runs on pull requests in CI, and can record a Chrome DevTools performance trace of a running app.

- **+** Runs with one npx command from the project root, no setup needed
- **+** Deterministic rules rather than LLM-generated findings
- **+** Agent skill installer supports Claude Code, Cursor, Codex and OpenCode
- **+** Rules configurable in doctor.config.ts; CI installer reports issues each PR introduces
- **−** React-only; no support for other frameworks beyond the listed React stacks
- **−** CLI collects crash reports and anonymous usage data unless opted out
- **−** Runtime trace scan needs a running app and a Chrome DevTools trace
- **−** README does not list the number of rules or their names

<sub>no GPU · Needs Node.js, npm · [Repo](https://github.com/millionco/react-doctor) · [📖 Docs ↗](https://react.doctor/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/react-doctor/)</sub>

<a name="hunk"></a>
### 🥉 [hunk](https://github.com/modem-dev/hunk) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · MIT · Oct 2026</sub>

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
### #&#8288;4 [no-mistakes](https://github.com/kunchenguid/no-mistakes) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: easy (50) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · MIT · Oct 2026</sub>

**Local git proxy that runs AI review, tests and lint before opening a PR.**

no-mistakes places a local git remote in front of your real one. Pushing to it creates a disposable worktree and runs a pipeline (review, test, docs, lint, push, PR, CI) driven by a coding agent CLI such as claude or codex. The branch is forwarded to the real remote only after every gate passes, and a PR is opened for you. Safe fixes are applied automatically; other findings wait for approval in a TUI.

- **+** Runs in an isolated worktree, so your working directory is not disturbed
- **+** Works with claude, codex, grok, opencode, copilot, cursor and others, with ordered fallbacks
- **+** Three entry points: git push, a TUI, or a /no-mistakes agent skill
- **+** Watches CI after the PR opens and auto-repairs failures
- **−** Requires a runnable coding agent CLI configured for every gate
- **−** Agent calls spend API quota; RAM and cost figures are unknown
- **−** CI repairs may need another full review pass if revalidate_repairs is set
- **−** Auto PR creation and CI watching are documented only for configured push targets such as GitHub

<sub>Needs git, a coding agent CLI (claude, codex, opencode, etc.) · Models: claude, codex, grok, rovodev, opencode · [Repo](https://github.com/kunchenguid/no-mistakes) · [📖 Docs ↗](https://kunchenguid.github.io/no-mistakes/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/no-mistakes/)</sub>

<a name="pr-agent"></a>
### #&#8288;5 [pr-agent](https://github.com/the-pr-agent/pr-agent) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

**LLM pull request reviewer that comments via /review, /describe and /improve.**

PR-Agent runs as a GitHub Action, CLI, Docker image or webhook service and posts AI-generated descriptions, reviews, code suggestions and Q&A on pull requests. Each tool makes a single LLM call, and a compression strategy handles large diffs. It supports GitHub, GitLab, Bitbucket, Azure DevOps and Gitea, and any model reachable through LiteLLM.

- **+** Supports GitHub, GitLab, Bitbucket, Azure DevOps and Gitea
- **+** Model-agnostic via LiteLLM: OpenAI, Claude, Gemini, Bedrock, Ollama and others
- **+** One LLM call per tool, about 30 seconds per command
- **+** Review behavior is configurable through a TOML settings file and JSON prompts
- **−** Described as a community-maintained legacy project of Qodo
- **−** /help_docs is disabled since v0.36.1 over a credential-exposure issue
- **−** Needs your own LLM API key and per-provider setup
- **−** Docker images moved to pragent/pr-agent from 0.34.2, so pinned references break

<sub>no GPU · Docker + Compose · Needs LLM API key (e.g. OpenAI), Git provider token · Models: OpenAI GPT, Anthropic Claude, Google Gemini, DeepSeek, Mistral · [Repo](https://github.com/the-pr-agent/pr-agent) · [📖 Docs ↗](https://docs.pr-agent.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pr-agent/)</sub>

<a name="e2e"></a>
### #&#8288;6 [e2e](https://github.com/tester-army/e2e) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (94) · Easy to run: some setup (33) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

**AI-driven end-to-end testing framework for web and mobile apps.**

TypeScript test runner where an agent carries out natural-language goals in the app, and ordinary locators and assertions verify the result in the same test. Agent steps that a later assertion checks are recorded and replayed on the next run without model calls until the app changes. Web runs use Playwright (Chromium, Firefox, WebKit); mobile runs use iOS simulators and Android emulators.

- **+** Recorded agent actions replay with no model calls until the app changes
- **+** Tests without agent steps need no model at all
- **+** Web via Playwright; iOS and Android via simulators and emulators
- **+** Examples for Next.js, Vite, Astro, Expo, SwiftUI, Compose, Flutter
- **−** APIs and config can still change between minor releases before 1.0
- **−** CLI sends anonymous telemetry by default; opt-out required
- **−** Agent steps need a model subscription, API key, or local model
- **−** Hosted browser and simulator options depend on third-party services

<sub>no GPU · Needs Node.js, Playwright, agent-device, iOS simulator or Android emulator (mobile) · Models: Bring your own subscription, API key, or local model · [Repo](https://github.com/tester-army/e2e) · [📖 Docs ↗](https://e2e.tester.army/docs) · [🌐 Site ↗](https://tester.army/e2e) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/e2e/)</sub>

<a name="front-end-checklist"></a>
### #&#8288;7 [front-end-checklist](https://github.com/thedaviddias/front-end-checklist) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: patchy (33) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

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

<a name="deepsec"></a>
### #&#8288;8 [deepsec](https://github.com/vercel-labs/deepsec) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (37) · Easy to run: hard (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · Apache-2.0 · Sep 2026</sub>

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

<a name="chatgpt-codereview"></a>
### #&#8288;9 [chatgpt-codereview](https://github.com/anc95/chatgpt-codereview) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: weak (16) · Easy to run: some setup (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · ISC · Aug 2026</sub>

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

<a name="claude-code-security-review"></a>
### #&#8288;10 [claude-code-security-review](https://github.com/anthropics/claude-code-security-review) <sub>score [16](../README.md#-how-we-rank "Score 16/100. Adoption: niche (29) · Freshness: slowing (41) · Maintenance: weak (6) · Easy to run: hard (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Feb 2026</sub>

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
