# 🧪 Code review and testing reviews · Best of Vibe Coding

AI tools that review pull requests, write tests or find bugs, run in your CI or on your machine. Back to the [leaderboard](../README.md#-code-review-and-testing).

<sub>🌐 Also on the web: [Code review and testing on archestack.com](https://archestack.com/best-of-vibe-coding/code-review/), each project on its own page.</sub>

<a name="open-code-review"></a>
### 🥇 [open-code-review](https://github.com/alibaba/open-code-review) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · Apache-2.0 · Oct 2026</sub>

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
### 🥈 [react-doctor](https://github.com/millionco/react-doctor) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

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

<a name="pr-agent"></a>
### 🥉 [pr-agent](https://github.com/the-pr-agent/pr-agent) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

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
### #&#8288;4 [e2e](https://github.com/tester-army/e2e) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

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

<a name="hunk"></a>
### #&#8288;5 [hunk](https://github.com/modem-dev/hunk) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · MIT · Oct 2026</sub>

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
### #&#8288;6 [no-mistakes](https://github.com/kunchenguid/no-mistakes) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.9k · MIT · Oct 2026</sub>

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

<a name="front-end-checklist"></a>
### #&#8288;7 [front-end-checklist](https://github.com/thedaviddias/front-end-checklist) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

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

<a name="pr-lens"></a>
### #&#8288;8 [pr-lens](https://github.com/coldteadotai/pr-lens) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · MIT · Oct 2026</sub>

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

<a name="reticle"></a>
### #&#8288;9 [reticle](https://github.com/reticlehq/reticle) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · custom license · Oct 2026</sub>

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

<a name="mantis"></a>
### #&#8288;10 [mantis](https://github.com/google/mantis) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="deepsec"></a>
### #&#8288;11 [deepsec](https://github.com/vercel-labs/deepsec) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · Apache-2.0 · Sep 2026</sub>

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

<a name="kodus-ai"></a>
### #&#8288;12 [kodus-ai](https://github.com/kodustech/kodus-ai) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Oct 2026</sub>

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

<a name="git-lrc"></a>
### #&#8288;13 [git-lrc](https://github.com/hexmostech/git-lrc) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · custom license · Oct 2026</sub>

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

<a name="codegpt"></a>
### #&#8288;14 [codegpt](https://github.com/appleboy/codegpt) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Sep 2026</sub>

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

<a name="chatgpt-codereview"></a>
### #&#8288;15 [chatgpt-codereview](https://github.com/anc95/chatgpt-codereview) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · ISC · Aug 2026</sub>

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

<a name="shippie"></a>
### #&#8288;16 [shippie](https://github.com/mattzcarey/shippie) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: known (36) · Freshness: active (94) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Jul 2026</sub>

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

<a name="ai-codereview-gitlab"></a>
### #&#8288;17 [ai-codereview-gitlab](https://github.com/sunmh207/ai-codereview-gitlab) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="run-gemini-cli"></a>
### #&#8288;18 [run-gemini-cli](https://github.com/google-github-actions/run-gemini-cli) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · Apache-2.0 · Aug 2026</sub>

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

<a name="claude-code-security-review"></a>
### #&#8288;19 [claude-code-security-review](https://github.com/anthropics/claude-code-security-review) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: popular (58) · Freshness: slowing (40) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Feb 2026</sub>

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
