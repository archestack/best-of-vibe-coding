# 🧪 Code review and testing reviews · Best of Vibe Coding

AI tools that review pull requests, write tests or find bugs, run in your CI or on your machine. Back to the [leaderboard](../README.md#-code-review-and-testing).

<sub>🌐 Also on the web: [Code review and testing on archestack.com](https://archestack.com/best-of-vibe-coding/code-review/), each project on its own page.</sub>

<a name="open-code-review"></a>
### 🥇 [open-code-review](https://github.com/alibaba/open-code-review) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (91) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 47k · Apache-2.0 · Oct 2026</sub>

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

<a name="front-end-checklist"></a>
### 🥈 [front-end-checklist](https://github.com/thedaviddias/front-end-checklist) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: patchy (33) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 74k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs MCP-compatible client, pnpm (for contributing) · [Repo](https://github.com/thedaviddias/front-end-checklist) · [📖 Docs ↗](https://frontendchecklist.io/mcp) · [🌐 Site ↗](https://frontendchecklist.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/front-end-checklist/)</sub>

<a name="pr-agent"></a>
### 🥉 [pr-agent](https://github.com/the-pr-agent/pr-agent) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (99) · Easy to run: some setup (33) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
