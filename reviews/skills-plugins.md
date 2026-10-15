# 🧩 Skills, plugins and rules reviews · Best of Vibe Coding

Add-ons that make coding agents better: skills, plugins, rules, hooks and memory for Claude Code, Codex, Cursor and others. Back to the [leaderboard](../README.md#-skills-plugins-and-rules).

<sub>🌐 Also on the web: [Skills, plugins and rules on archestack.com](https://archestack.com/best-of-vibe-coding/skills-plugins/), each project on its own page.</sub>

<a name="caveman"></a>
### 🥇 [caveman](https://github.com/juliusbrussee/caveman) <sub>score [95](../README.md#-how-we-rank "Score 95/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 112k · Apache-2.0 · Oct 2026</sub>

**Cuts token use in coding agents with terse replies and compressed inputs.**

Caveman is a CLI and skill set that reduces token use in coding agents such as Claude Code, Codex, Gemini CLI and OpenCode. It shortens agent replies, compresses logs, JSON, CSV and test output before the model reads them, and can route each request to a model and effort level through a free account. Reported results include 33.2% fewer input tokens over 54 Claude Code runs and an interim 54% cost cut for Auto on 85 tasks.

- **+** One npx command sets up 30+ agents; runs locally with your own keys
- **+** README lists losing cases: HTML input 9.9% worse, grep-defs loses to bare grep
- **+** Each part can be switched off separately; the skill installs alone
- **+** Cited by Adobe Research paper, JetBrains A/B on 86 tasks, Elastic blog
- **−** Auto routing needs a Caveman account; its benchmark is interim and half complete
- **−** Terse output saves nothing on per-request billing such as GitHub Copilot
- **−** Rules cost about 1,160 input tokens; output benchmarks used older 3.1.0 rules
- **−** No HTML compressor yet; Blocks is pre-release (v0.1.0-rc.5), Python only

<sub>no GPU · Docker + Compose · Needs Node.js 22.13+, Caveman account (Auto only) · Models: Claude Code, Codex, Gemini CLI, OpenCode, Aider · safety checks passed 9 of 11 · [Repo](https://github.com/juliusbrussee/caveman) · [▶️ Demo ↗](https://caveman.so/demo) · [📖 Docs ↗](https://docs.caveman.so) · [🌐 Site ↗](https://caveman.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/caveman/)</sub>

<a name="impeccable"></a>
### 🥈 [impeccable](https://github.com/pbakaus/impeccable) <sub>score [95](../README.md#-how-we-rank "Score 95/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 82k · Apache-2.0 · Oct 2026</sub>

**Design skill with 24 commands and a detector for AI-generated frontends.**

Impeccable installs a single /impeccable skill into AI coding tools, with 24 commands such as audit, critique, polish, typeset and live browser variant iteration. It writes PRODUCT.md and DESIGN.md for project context, and ships 59 deterministic detector rules that run in a CLI and browser extension without an LLM or API key. Hooks flag common AI design tells on UI file edits in supported harnesses.

- **+** Supports many harnesses: Claude Code, Cursor, Codex, Gemini CLI, Copilot, Grok Build, Hermes
- **+** 59 deterministic detector rules run without an LLM or API key
- **+** Edit hooks surface design findings; Cursor blocks bad writes before they land
- **+** Several install paths: npx installer, Git submodule, plugin marketplace, manual copy
- **−** Native edit hooks are not available on every harness; Hermes and Veto get none
- **−** Roll API at impeccable.style is called when a new design starts; telemetry is opt-out
- **−** Downloads an engine binary into ~/.impeccable/bin/ on first run if not bundled
- **−** Codex and Grok Build need manual hook or folder trust approval after install

<sub>no GPU · Needs Node.js (only for npx installer), impeccable.style roll API · Models: Claude Code, Cursor, Codex CLI, Gemini CLI, GitHub Copilot · safety checks passed 10 of 11 · [Repo](https://github.com/pbakaus/impeccable) · [▶️ Demo ↗](https://impeccable.style/cases/neo-mirai) · [📖 Docs ↗](https://impeccable.style) · [🌐 Site ↗](https://impeccable.style) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/impeccable/)</sub>

<a name="skills"></a>
### 🥉 [skills](https://github.com/mattpocock/skills) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 293k · MIT · Oct 2026</sub>

**Agent skills for planning, TDD, debugging and code review.**

A collection of Markdown skill files for coding agents, split into engineering and productivity groups. It covers grilling sessions that build a project glossary and ADRs, spec and ticket generation, red-green-refactor TDD, a bug diagnosis loop, and diff review. Installs as a plugin for Claude Code, Codex and GitHub Copilot, via gemini skills install for Gemini CLI, or as editable files through npx skills.

- **+** Small, composable skills that can be edited; README says they work with any model
- **+** Plugin install for Claude Code, Codex and Copilot, with automatic updates
- **+** Setup skill configures issue tracker (GitHub, GitLab, local files), triage labels and doc locations
- **+** Separates user-invoked orchestration skills from model-invoked discipline skills
- **−** Manual updates for Gemini CLI and npx installs
- **−** Installing both plugin and npx copies gives every skill twice
- **−** Must run /setup-matt-pocock-skills once per repo before the engineering skills
- **−** Architecture skill is a survey only and will not untangle an old codebase

<sub>no GPU · Needs Issue tracker (GitHub, GitLab or local files) · Models: Any model (per README) · safety checks passed 10 of 11 · [Repo](https://github.com/mattpocock/skills) · [🌐 Site ↗](https://skills.sh/mattpocock/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skills/)</sub>

<a name="ecc"></a>
### #&#8288;4 [ecc](https://github.com/affaan-m/ecc) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 280k · MIT · Oct 2026</sub>

**Agents, skills, hooks and rules bundle for Claude Code, Codex and other harnesses.**

ECC installs a plan, test, implement, review, verify workflow into coding agents. It ships 71 agents, 311 skills, 97 legacy command shims, hooks, selectable rules, session memory and the AgentShield scanner for prompts, hooks, MCP config and permissions. Native plugin paths exist for Claude Code and Codex; Cursor, OpenCode, Gemini, Zed and others get capability-limited adapters.

- **+** Large bundle: 71 agents, 311 skills, hooks and rules in one install
- **+** Guided setup wizard for Claude Code, Codex and Kimi Code with dry-run mode
- **+** Includes AgentShield scanning of MCP config, permissions, hooks and secrets
- **+** MIT licensed; npm releases pinned per version tag
- **−** Feature parity varies; non-Claude harnesses are capability-limited adapters
- **−** Claude plugins cannot ship rules, so rule packs need a manual copy
- **−** Stacking install methods duplicates skills and hooks; README warns against it
- **−** Private-repo GitHub App is paid (from $19/seat/month)

<sub>no GPU · Docker + Compose · Needs Node.js 18+, Git, Claude Code 2.1+ (for plugin setup) · Models: Claude Code, Codex, Kimi Code, Cursor, OpenCode · safety checks passed 11 of 11 · [Repo](https://github.com/affaan-m/ecc) · [🌐 Site ↗](https://ecc.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ecc/)</sub>

<a name="ponytail"></a>
### #&#8288;5 [ponytail](https://github.com/dietrichgebert/ponytail) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 164k · MIT · Oct 2026</sub>

**Skill prompt that makes coding agents write less code and add tests.**

Ponytail is a single prompt (SKILL.md, with a compact AGENTS.md) that loads into coding agents such as Claude Code and Codex. It tells the agent to check existing code, the standard library and native platform features before writing anything, and adds /ponytail-review, /ponytail-audit and /ponytail-debt commands. The README reports 53% less code and 45% fewer tokens in its own 39-task benchmark.

- **+** Works with 20 agents; plugin install for Claude Code and Codex, AGENTS.md for others
- **+** Benchmark method and per-task tables are published in the repo
- **+** Keeps validation, security and accessibility; leaves a small test for risky logic
- **+** No config file required; default level can be set by env var or JSON file
- **−** Benchmark figures are self-reported, run in Claude Code with Opus 5.5 only
- **−** Slash commands need a skill-capable host; rule-file adapters get only the always-on prompt
- **−** Cursor with hooks supports only /ponytail level switching, not review or audit
- **−** README is heavy on banners and a waitlist, with a jokey tone

<sub>no GPU · Needs A supported coding agent such as Claude Code or Codex · Models: Benchmarked with Opus 5.5 in Claude Code · safety checks passed 9 of 10 · [Repo](https://github.com/dietrichgebert/ponytail) · [🌐 Site ↗](https://ponytail.dev/stories) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ponytail/)</sub>

<a name="ui-ux-pro-max-skill"></a>
### #&#8288;6 [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 136k · MIT · Oct 2026</sub>

**Design-system skill that gives coding agents searchable UI styles, palettes and fonts.**

An agent skill that runs a local Python search script (BM25 ranking, standard library only) over CSV datasets of UI styles, color palettes, font pairings, landing patterns and UX guidelines. Given a product description, it applies 192 industry reasoning rules and outputs a design system with pattern, style, colors, typography, anti-patterns and a checklist. An npm CLI installs it for Claude Code, Cursor, Windsurf, Codex CLI, Gemini CLI and about 20 other assistants.

- **+** Scripts use only the Python standard library and make no network calls
- **+** One CLI (uipro init --ai) installs to over 20 assistants, per project or globally
- **+** Data is plain CSV: 79 styles, 192 palettes, 74 font pairings, 119 UX guidelines
- **+** Covers 22 stacks including React, Next.js, Vue, SwiftUI, Flutter and Jetpack Compose
- **−** Requires Python 3 on the machine; the agent will not install it for you
- **−** Brand identity, logo, CIP and image-generation features are in the paid premium version
- **−** Recommendations are rule and keyword matches; output quality depends on the agent using it
- **−** Only 50 of 79 styles are active in normal recommendations

<sub>no GPU · Needs Python 3, Node.js/npm (for the uipro CLI) · Models: Claude Code, Cursor, Windsurf, Codex CLI, Gemini CLI · safety checks passed 10 of 10 · [Repo](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) · [🌐 Site ↗](https://uupm.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui-ux-pro-max-skill/)</sub>

<a name="claude-mem"></a>
### #&#8288;7 [claude-mem](https://github.com/thedotmack/claude-mem) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 101k · Apache-2.0 · Oct 2026</sub>

**Persistent cross-session memory plugin for Claude Code and other coding agents.**

Captures tool usage through lifecycle hooks (SessionStart, PostToolUse, Stop and others), summarizes it into observations stored in SQLite, and injects relevant context into later sessions. Retrieval uses a local worker service with a web viewer, Chroma hybrid search, and MCP tools (search, timeline, get_observations) that fetch details in layers to save tokens. Installers also cover OpenCode, T3 Code, Antigravity, OMP, Pi, DeepSeek Harness and OpenClaw.

- **+** Hooks capture and inject context automatically, with no manual steps after install
- **+** 3-layer MCP search (search, timeline, get_observations) filters IDs before fetching full details
- **+** Local SQLite storage with FTS5 plus Chroma hybrid search, and a web viewer
- **+** Installer targets many harnesses beyond Claude Code, such as OpenCode, T3 Code and Pi
- **−** Default setup prompts sign-in to a hosted service; the free trial is 30 days
- **−** Needs Node 20+, Bun and uv; the latter two are auto-installed
- **−** `npm install -g claude-mem` gives only the SDK, not the plugin hooks or worker
- **−** Memory generation consumes model usage unless a provider is configured; RAM needs are unknown

<sub>no GPU · Docker + Compose · Needs Node.js 20+, Bun, uv, SQLite, Chroma · Models: Anthropic plan, OpenRouter, Gemini, claude-mem observer (hosted) · safety checks passed 9 of 10 · [Repo](https://github.com/thedotmack/claude-mem) · [📖 Docs ↗](https://docs.claude-mem.ai/) · [🌐 Site ↗](https://docs.claude-mem.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-mem/)</sub>

<a name="oh-my-claudecode"></a>
### #&#8288;8 [oh-my-claudecode](https://github.com/yeachan-heo/oh-my-claudecode) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

**Multi-agent orchestration plugin and CLI for Claude Code.**

Adds staged team pipelines (plan, PRD, exec, verify, fix), autopilot and persistent execution loops to Claude Code, as a plugin and as an `omc` npm CLI. `omc team` can launch tmux worker panes running claude, codex, gemini, antigravity, grok or cursor-agent CLIs. Configuration lives in `.claude/omc.jsonc`.

- **+** Installs as a Claude Code plugin or as an npm CLI (`omc`)
- **+** Team workers can be claude, codex, gemini, antigravity, grok or cursor CLIs in tmux
- **+** Workers spawn per task and exit when done, so nothing idles
- **+** Includes a deep-interview skill and a HUD statusline
- **−** Requires Claude Code; in-session team mode needs an experimental flag enabled
- **−** Slash-command skills such as /autopilot and /ralph cannot run in CI
- **−** Named autopilot workflow profiles need Linux with flock
- **−** npm package name (oh-my-claude-sisyphus) differs from repo name; install prints a deprecation warning

<sub>no GPU · Needs Claude Code, Node.js/npm, tmux (for omc team), codex, gemini, agy, grok or cursor-agent CLIs (optional) · Models: Claude, Codex, Gemini, Antigravity, Grok · safety checks passed 10 of 11 · [Repo](https://github.com/yeachan-heo/oh-my-claudecode) · [📖 Docs ↗](https://yeachan-heo.github.io/oh-my-claudecode-website/docs/) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-claudecode-website) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-claudecode/)</sub>

<a name="spec-kit"></a>
### #&#8288;9 [spec-kit](https://github.com/github/spec-kit) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 141k · MIT · Oct 2026</sub>

**CLI and agent skills for spec-driven development, bug fixing and idea assessment.**

Spec Kit is a Python CLI (`specify`) that scaffolds a project with slash-command skills for AI coding agents such as GitHub Copilot. Its core flow is constitution, specify, plan, tasks, implement, converge. Bug-fix (assess, fix, test) and idea-assessment (intake through decide) processes are opt-in extensions that write Markdown reports under `.specify/`.

- **+** Three independent processes; bug fixing and assessment install separately via `specify extension add`
- **+** Artifacts are plain Markdown in `.specify/`, reviewable and editable by hand
- **+** Integration keys let the same workflow target different coding agents
- **+** Extensions, presets, workflows and bundles allow customizing or replacing the processes
- **−** Needs a separate supported AI coding agent; it does not run models itself
- **−** Skills are invoked in agent chat, with invocation syntax varying by agent
- **−** Requires Python 3.11+ and uv
- **−** Process is manual and stepwise: each skill is run and reviewed one at a time

<sub>no GPU · Needs Python 3.11+, uv, a supported AI coding agent · safety checks passed 9 of 9 · [Repo](https://github.com/github/spec-kit) · [📖 Docs ↗](https://github.github.io/spec-kit/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spec-kit/)</sub>

<a name="agent-skills"></a>
### #&#8288;10 [agent-skills](https://github.com/addyosmani/agent-skills) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 107k · MIT · Oct 2026</sub>

**Markdown engineering skills and slash commands for AI coding agents.**

A pack of 25 SKILL.md workflows covering spec, plan, build, test, review and ship, plus 9 slash commands, 4 reviewer personas and reference checklists. Each skill has steps, verification gates and an anti-rationalization table. It installs through the skills CLI (`npx skills add`) or natively in Claude Code, Codex, Gemini CLI, Antigravity and Command Code.

- **+** Installs into 70+ agents with one `npx skills add` command
- **+** Skills are plain Markdown, usable with any agent that reads instruction files
- **+** Covers the lifecycle: 25 skills, 9 commands, 4 personas, 7 checklists
- **+** `/build auto` runs the planned tasks after one approval, committing each task
- **−** Lifecycle slash commands work only in Claude Code; Copilot needs skills invoked by name
- **−** Per-skill npx install omits shared `references/` checklists (issue #361)
- **−** Cursor and Windsurf setups need manual copying into skills or rules
- **−** Some Antigravity CLI releases do not expose the wrapper commands

<sub>no GPU · Needs Node.js (npx) for skills CLI install, Git, A supported coding agent · safety checks passed 9 of 10 · [Repo](https://github.com/addyosmani/agent-skills) · [📖 Docs ↗](https://github.com/addyosmani/agent-skills/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills/)</sub>

<a name="archify"></a>
### #&#8288;11 [archify](https://github.com/tt-a1i/archify) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 84k · MIT · Oct 2026</sub>

**Agent skill that turns a prompt or repo into an interactive HTML diagram.**

Archify is a skill installed with `npx skills add tt-a1i/archify -g` for Claude Code, Codex CLI, Cursor and OpenCode. You describe a system, plan or repository in chat, and the agent produces a self-contained HTML file with node details, path tracing and export options. It supports ten diagram types, including architecture, workflow, sequence, data flow, lifecycle and ERD.

- **+** Output is one standalone HTML file; viewing needs no Archify install
- **+** Works with Claude Code, Codex CLI, Cursor and OpenCode via one install command
- **+** Keeps typed JSON source so follow-up chat edits can target specific nodes
- **+** Exports PNG, plus route and reach share cards at 1200x630
- **−** Quality depends on the host agent and model; it ships no model of its own
- **−** Optional update check makes a network request unless ARCHIFY_UPDATE_CHECK_DISABLED=1 is set
- **−** README carries many paid third-party API sponsor blocks
- **−** Repository diagrams are only as accurate as the agent's reading of the code

<sub>no GPU · Needs Node.js (npx), Claude Code, Codex CLI, Cursor or OpenCode · safety checks passed 10 of 10 · [Repo](https://github.com/tt-a1i/archify) · [▶️ Demo ↗](https://archify.si/gallery.html) · [📖 Docs ↗](https://archify.si/guide.html) · [🌐 Site ↗](https://archify.si) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archify/)</sub>

<a name="ruflo"></a>
### #&#8288;12 [ruflo](https://github.com/ruvnet/ruflo) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

**Multi-agent orchestration, memory and MCP tools layered on Claude Code and Codex.**

Ruflo wraps Claude Code and Codex with a harness: swarm coordination, vector-backed memory, hooks that route tasks, and an MCP server. It installs either as Claude Code plugins (35 listed) or via `npx ruflo init`, which adds 98 agents, 60+ commands, 30 skills and a daemon. A console (Claude Code plugin or `npx ruflo tui`) shows agents, cost and missions.

- **+** Two install paths: zero-file Claude Code plugins or full CLI init with hooks and daemon
- **+** Exposes an MCP server, so Codex and other MCP clients can use it
- **+** Standalone terminal UI runs without Claude Code (`npx ruflo tui`)
- **+** Console Claude-control defaults to read + ask, with confirmation for spending and destructive actions
- **−** Large surface (314 MCP tools, 26 CLI commands, 35 plugins) is hard to audit
- **−** Plugin path gives only a subset; full loop needs the CLI install that writes files into the repo
- **−** Mods are not sandboxed and run with your account's permissions
- **−** Hook and console support depends on client; Claude Code 2.1.287 or later required for plugins

<sub>Needs Node.js/npx, Claude Code or Codex · Models: Claude, Codex, Ollama (via ruflo-ruvllm) · safety checks passed 14 of 17 · [Repo](https://github.com/ruvnet/ruflo) · [▶️ Demo ↗](https://raw.githubusercontent.com/ruvnet/ruflo/main/docs/assets/ruflo-console-theme-compact.svg) · [📖 Docs ↗](https://github.com/ruvnet/ruflo/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://cognitum.one/agentic-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruflo/)</sub>

<a name="book-to-skill"></a>
### #&#8288;13 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

**Converts books and document folders into on-demand agent skills with per-chapter files.**

A Python extractor turns PDF, EPUB, DOCX, Markdown, HTML, RTF or MOBI files into clean text. The agent then follows SKILL.md to generate a skill: a core SKILL.md, one file per chapter, a glossary, patterns and a cheatsheet. The skill installs under ~/.agents/skills/ and loads chapters on demand in Claude Code, Copilot CLI, Amp, Codex, Hermes Agent, OpenCode or OpenClaw. The README reports 24x–51x fewer tokens than dumping the book into context.

- **+** Reads PDF, EPUB, DOCX, MD, HTML, RTF and MOBI, with fallbacks to stdlib parsers
- **+** One SKILL.md output works across seven agent hosts that follow the Agent Skills format
- **+** Chapter files load only when asked, keeping the base skill near 4,000 tokens
- **+** Extraction runs locally; `extract.py --check` reports which extractors are missing
- **−** Scanned PDFs are rejected; OCR (for example ocrmypdf) must be run first
- **−** Generation quality depends on the host agent and its model, not the extractor
- **−** MOBI/AZW needs Calibre installed separately
- **−** Sharing skills built from copyrighted books can infringe; README advises keeping them private

<sub>no GPU · Needs Python 3, pdftotext (poppler), docling, pypdf, ebooklib, beautifulsoup4, python-docx, Calibre ebook-convert, ocrmypdf · Models: Any model in the host agent (Claude Code, Copilot CLI, Amp, Codex, Hermes Agent, OpenCode, OpenClaw) · safety checks passed 9 of 9 · [Repo](https://github.com/virgiliojr94/book-to-skill) · [📖 Docs ↗](https://github.com/virgiliojr94/book-to-skill/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/book-to-skill/)</sub>

<a name="agentic-awesome-skills"></a>
### #&#8288;14 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · MIT · Oct 2026</sub>

**Library of 2,690+ SKILL.md playbooks with a local MCP for selecting them.**

A catalog of installable SKILL.md playbooks for coding agents such as Claude Code, Codex CLI, Cursor, Gemini CLI, Kiro and OpenCode. AAS Core is a local MCP plus an `aas` CLI that lets the agent search the catalog, record chosen skills in an aas-stack.json manifest and preview a plan. An npx installer copies selected skills into a host's skill directory.

- **+** 2,690+ skills, each a plain SKILL.md file, with a machine-readable skills_index.json
- **+** Installer targets many hosts: Claude Code, Cursor, Codex, Gemini CLI, Kiro, OpenCode, Copilot
- **+** Install and stack plan steps support dry-run preview before any target is changed
- **+** MIT license; 13 domain plugins for Claude Code and Codex
- **−** Core does not rank or recommend skills; the agent must choose
- **−** Core apply and recovery are experimental and outside the supported preview
- **−** Validation checks structure only, not fit, compatibility or safety of a skill
- **−** Installing too many skills can overload Antigravity's context

<sub>no GPU · Needs Node.js/npm (npx installer), Codex or Claude Code for AAS Core MCP · safety checks passed 7 of 11 · [Repo](https://github.com/sickn33/agentic-awesome-skills) · [▶️ Demo ↗](https://aaskills.tech/workbench) · [📖 Docs ↗](https://github.com/sickn33/agentic-awesome-skills/blob/v19.7.0/docs/users/aas-core.md) · [🌐 Site ↗](https://aaskills.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentic-awesome-skills/)</sub>

<a name="repomix"></a>
### #&#8288;15 [repomix](https://github.com/yamadashy/repomix) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

**CLI that packs a repository into one file for LLM context.**

Repomix reads a local or remote Git repository and writes a single file, XML by default or Markdown, JSON or plain text, with a directory tree and file contents. It reports token counts, respects .gitignore, .ignore and .repomixignore, and uses Secretlint to leave out files matching known credential formats. The --compress option uses Tree-sitter to keep code structure while cutting tokens.

- **+** One command (npx repomix@latest) produces the packed file with no install
- **+** Token counts per file and for the whole repo help fit context limits
- **+** --compress uses Tree-sitter to reduce tokens while keeping code structure
- **+** Packs remote repos by URL, branch or commit, and file lists piped via --stdin
- **−** Output is a static snapshot; you paste or upload it to the model yourself
- **−** Secret detection only covers known credential formats via Secretlint
- **−** VSCode extension is community-maintained, not part of the core project
- **−** Whole large repos can exceed model context unless filtered or compressed

<sub>no GPU · Docker · Needs Node.js · Models: Model-agnostic: output is a file for Claude, ChatGPT, Gemini, Llama, Grok and others · safety checks passed 16 of 16 · [Repo](https://github.com/yamadashy/repomix) · [▶️ Demo ↗](https://repomix.com) · [🌐 Site ↗](https://repomix.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repomix/)</sub>

<a name="superpowers"></a>
### #&#8288;16 [superpowers](https://github.com/obra/superpowers) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 300k · MIT · Oct 2026</sub>

**Skill set that enforces a plan-and-TDD workflow in coding agents.**

Superpowers is a library of composable skills plus a bootstrap skill (using-superpowers) that makes a coding agent brainstorm a spec, write a task plan, and implement it with subagents under red/green TDD and code review. It installs as a plugin or extension for Claude Code, Codex, Cursor, Gemini CLI, Copilot CLI, OpenCode, Pi and others. Skills trigger automatically.

- **+** Installs via plugin marketplaces or one command on 15+ listed agent harnesses
- **+** Covers the full loop: brainstorming, worktrees, plans, subagent execution, review, branch finish
- **+** diagnosing-superpowers skill reads session transcripts and can export a scrubbed bug bundle
- **+** MIT licensed, with eval harness and plugin tests in the repo
- **−** Workflows are mandatory, so small tasks go through the same process
- **−** Subagent-driven mode costs more tokens than inline execution
- **−** Install is per harness; each agent needs separate setup
- **−** Optional visual companion loads a vendor-hosted logo that reports version unless disabled by env var

<sub>no GPU · Needs A supported coding agent (Claude Code, Codex, Cursor, Gemini CLI, etc.) · Models: Claude Code, Codex, Cursor, Gemini CLI, GitHub Copilot CLI · safety checks passed 9 of 9 · [Repo](https://github.com/obra/superpowers) · [🌐 Site ↗](https://primeradiant.com/superpowers/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superpowers/)</sub>

<a name="rtk"></a>
### #&#8288;17 [rtk](https://github.com/rtk-ai/rtk) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 84k · Apache-2.0 · Oct 2026</sub>

**Rewrites shell commands so coding agents read compressed command output.**

rtk is a Rust binary that hooks into coding agents' Bash tool calls and rewrites commands like git status, pytest or cargo test to filtered equivalents, cutting output by up to 90% per the README. It supports 100+ commands and 18 agent integrations, and reports savings with `rtk gain`. An optional BUSL-1.1 proxy daemon compresses provider API traffic, and a pipeline.toml engine configures the rules.

- **+** Single Rust binary; README states under 10ms overhead per command
- **+** Hook setup for 18 agents, including Claude Code, Cursor, Codex and Gemini CLI
- **+** `rtk gain` and `rtk discover` report measured savings and missed opportunities
- **+** Apache-2.0-only rtk-oss edition is available without the engine
- **−** Hook only fires on Bash calls; built-in Read, Grep and Glob tools bypass it
- **−** Token counts are estimated as bytes/4; absolute numbers are approximate
- **−** Default rtk, the engine and the proxy are BUSL-1.1; commercial resale needs a contract
- **−** rtk and rtk-oss share a binary name and cannot be installed together

<sub>no GPU · Needs Homebrew, winget or curl installer, A supported coding agent · safety checks passed 9 of 10 · [Repo](https://github.com/rtk-ai/rtk) · [📖 Docs ↗](https://www.rtk-ai.app/guide) · [🌐 Site ↗](https://www.rtk-ai.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rtk/)</sub>

<a name="openspec"></a>
### #&#8288;18 [openspec](https://github.com/fission-ai/openspec) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 72k · MIT · Oct 2026</sub>

**Spec-driven workflow layer that adds proposal, spec and task files to AI coding.**

OpenSpec is a Node.js CLI that installs slash commands (/opsx:explore, /opsx:propose, /opsx:apply, /opsx:archive) into 30+ AI coding assistants. Each change gets a folder with proposal.md, specs, design.md and tasks.md in plain Markdown, which you review before code is written. A beta "stores" feature keeps specs and changes in a separate repo shared across several code repos.

- **+** Works with 30+ coding assistants through generated slash commands, not a dedicated IDE
- **+** Specs and changes are plain Markdown in the repo, reviewable in git
- **+** Artifacts can be edited at any time, with no enforced phase gates
- **+** Stores (beta) share one plan across multiple repos via git push
- **−** Output quality depends on the model; README recommends Codex 5.5 or Opus 4.7
- **−** Stores for cross-repo planning are still in beta
- **−** Collects anonymous command and version telemetry by default; opt-out required
- **−** Slash command spelling differs per tool, so instructions vary by assistant

<sub>no GPU · Needs Node.js 20.19.0 or higher, A supported AI coding assistant · Models: Tool-agnostic; recommends Codex 5.5 and Opus 4.7 · safety checks passed 9 of 10 · [Repo](https://github.com/fission-ai/openspec) · [📖 Docs ↗](https://openspec.dev/docs) · [🌐 Site ↗](https://openspec.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openspec/)</sub>

<a name="graphify"></a>
### #&#8288;19 [graphify](https://github.com/graphify-labs/graphify) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 127k · Apache-2.0 · Oct 2026</sub>

**Skill that maps a codebase and docs into a queryable knowledge graph.**

Graphify installs as a skill for AI coding assistants (Claude Code, Cursor, Codex, Gemini CLI and 20+ others). Running /graphify builds a knowledge graph of code, docs, PDFs, images and video, written to graph.json, graph.html and GRAPH_REPORT.md. Code is parsed locally with tree-sitter across about 40 languages. The graph is queried with query, path and explain commands instead of grepping files.

- **+** Code parsing uses tree-sitter AST: deterministic, no LLM, nothing leaves the machine
- **+** Every edge is tagged EXTRACTED or INFERRED, so direct and resolved links are distinguishable
- **+** One install registers the skill for 20+ assistants on macOS, Linux and Windows
- **+** Optional extras for MCP stdio server, Neo4j, FalkorDB, Ollama, OpenAI, Anthropic, Bedrock
- **−** Docs, PDFs, images and video need an assistant model or API key for the semantic pass
- **−** Always-on, cross-repo and formal verification features are in paid Graphify Cloud
- **−** PyPI package name is graphifyy (double-y); similarly named packages are unaffiliated
- **−** Parallel extraction is limited on some platforms; OpenClaw and Aider run sequentially

<sub>no GPU · Docker · Needs Python 3.10+, uv or pipx · Models: Claude, OpenAI-compatible, Gemini, Ollama, AWS Bedrock · safety checks passed 14 of 15 · [Repo](https://github.com/graphify-labs/graphify) · [📖 Docs ↗](https://docs.graphify.com) · [🌐 Site ↗](https://graphify.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphify/)</sub>

<a name="claude-hud"></a>
### #&#8288;20 [claude-hud](https://github.com/jarrodwatts/claude-hud) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

**Status line plugin for Claude Code showing context, usage limits and todos.**

Claude HUD is a Claude Code plugin that registers a status line command, which prints context-window usage, subscriber rate limits, model, project path and git branch below the input. Optional lines show active tools, subagents, skills, MCP servers and todo progress, read from the session transcript. Settings live in a JSON config file or the /claude-hud:configure flow, and it needs no tmux or separate window.

- **+** Installs from the Claude Code plugin marketplace with a few slash commands
- **+** Reads session data Claude Code passes on stdin; no separate window or tmux
- **+** Extensive config: layout, element order, thresholds, colors, git and jj status
- **+** Labels available in English, Simplified and Traditional Chinese
- **−** Works only with Claude Code
- **−** Subscriber usage limits are hidden on API-key, Bedrock and Vertex sessions
- **−** Tools, agents and todos lines are off by default and parse the transcript
- **−** Needs a JavaScript runtime; Windows users must install Node.js separately

<sub>no GPU · Needs Claude Code, Node.js · Models: Claude, Bedrock, Vertex, MiniMax · safety checks passed 11 of 11 · [Repo](https://github.com/jarrodwatts/claude-hud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-hud/)</sub>

<a name="compound-engineering-plugin"></a>
### #&#8288;21 [compound-engineering-plugin](https://github.com/everyinc/compound-engineering-plugin) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

**Plugin of 36 agent skills for a plan, build, review and document loop.**

Compound Engineering is a plugin of 36 skills for AI coding agents, organized around a loop of brainstorm, plan, work, simplify, review and compound. The compound step writes learnings into docs/solutions/, which later brainstorm and plan runs read as context. It installs on 14 agent hosts, including Claude Code, Cursor and Codex, and includes an autonomous /lfg pipeline that can open a PR and watch CI.

- **+** Runs on 14 agent hosts, including Claude Code, Cursor, Codex, Copilot and OpenCode
- **+** Captures learnings as repo files (docs/solutions/) that later planning reads
- **+** Covers the full cycle: brainstorm, plan, work, review, plus debug, commit and PR skills
- **+** Artifact folder location is configurable via the docs_root setting
- **−** 36 skills and a multi-step workflow add process overhead for small changes
- **−** Install steps differ per host; Cline and Pi need extra setup or companion packages
- **−** Compound Packs for org-wide rules are marked experimental
- **−** Some Devin skills use Claude-style tool names and prompt for permission

<sub>no GPU · Needs An AI coding agent host (Claude Code, Cursor, Codex, etc.), pi-subagents (Pi only) · safety checks passed 10 of 11 · [Repo](https://github.com/everyinc/compound-engineering-plugin) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/compound-engineering-plugin/)</sub>

<a name="notebooklm-py"></a>
### #&#8288;22 [notebooklm-py](https://github.com/teng-lin/notebooklm-py) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Oct 2026</sub>

**Unofficial Python API, CLI and MCP server for Google NotebookLM.**

Drives NotebookLM (now Gemini Notebook) through its undocumented web endpoints, with an opt-in Android gRPC backend. It exposes notebooks, sources, cited chat, research agents and artifact generation (audio, video, slides, quizzes, mind maps) via an async Python client, a CLI, an MCP server, a REST server and an installable agent skill. Artifacts download in bulk as MP3, MP4, PDF, PPTX, CSV, JSON or Markdown.

- **+** Covers notebooks, sources, chat, notes, research, sharing and all Studio artifact types
- **+** Bulk artifact download in MP3, MP4, PDF, PPTX, CSV, JSON and Markdown
- **+** Ships CLI, MCP server (stdio or remote), REST server and Claude Code/Codex skill
- **+** Master-token auth refreshes sessions unattended for servers and CI
- **−** Relies on undocumented Google APIs that can break without notice
- **−** Not affiliated with Google; heavy use may be rate limited
- **−** Needs a Google account; source counts per notebook depend on account tier
- **−** Default login downloads Chromium (~170 MB) via Playwright

<sub>no GPU · Docker + Compose · Needs Google account, Google NotebookLM / Gemini Notebook, Playwright Chromium (for browser login) · Models: Google Gemini (via NotebookLM) · [Repo](https://github.com/teng-lin/notebooklm-py) · [▶️ Demo ↗](https://asciinema.org/a/767284) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/notebooklm-py/)</sub>

<a name="cc-switch"></a>
### #&#8288;23 [cc-switch](https://github.com/farion1231/cc-switch) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 145k · MIT · Oct 2026</sub>

**Desktop app for switching API providers across AI coding CLIs.**

CC Switch is a Tauri 2 desktop app (Rust) for Windows, macOS and Linux. It swaps API providers for Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build, OpenCode, OpenClaw, Hermes Agent, Pi and MiniMax Code, and manages MCP, Skills and Prompts in one place, so JSON, TOML or YAML configs need not be edited by hand.

- **+** Covers ten coding agents and CLIs from one provider list
- **+** Manages MCP servers, Skills and Prompts alongside provider switching
- **+** Native desktop builds for Windows, macOS and Linux via Tauri 2
- **+** MIT licensed, with a user manual and multilingual READMEs
- **−** Desktop GUI only; no Docker image or server mode
- **−** Much of the README is sponsor relay advertising, not technical detail
- **−** Config backup and rollback behavior unknown; README is truncated
- **−** Does not run agents itself; the CLIs must be installed separately

<sub>no GPU · Models: Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build · safety checks passed 4 of 5 · [Repo](https://github.com/farion1231/cc-switch) · [📖 Docs ↗](https://github.com/farion1231/cc-switch/blob/main/docs/user-manual/en/README.md) · [🌐 Site ↗](https://ccswitch.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-switch/)</sub>

<a name="gstack"></a>
### #&#8288;24 [gstack](https://github.com/garrytan/gstack) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 137k · MIT · Oct 2026</sub>

**Slash-command skill pack giving Claude Code review, QA and ship roles.**

gstack is a set of Markdown skills, invoked as slash commands such as /office-hours, /plan-eng-review, /review, /qa, /cso and /ship, that give Claude Code defined roles for planning, code review, browser QA, security audit and release. A Bun-based ./setup installs it into ~/.claude/skills and builds a bundled browser. Experimental installs exist for Codex, OpenCode, Cursor, Copilot CLI and others.

- **+** Covers planning, review, QA, security audit and release as separate slash commands
- **+** Team mode auto-updates for shared repos without vendoring files into them
- **+** Installs on Claude Code plus experimental hosts such as Codex, Cursor and OpenCode
- **+** Setup took 31 seconds on a 4-vCPU Linux machine, per the README
- **−** Safety hooks like /careful and /freeze are enforced only on Claude Code
- **−** Only Claude Code is certified; other agents are experimental or instruction-only
- **−** /cso needs a recent Bun with specific build flags and a native C toolchain
- **−** Outside reviews need a signed-in Codex CLI; design tools use an OpenAI key

<sub>no GPU · Needs Claude Code, Git, Bun 1.4.2+ (refuses older than 1.3.3), Node.js (Windows only), Codex CLI (optional, outside reviews), OpenAI API key (optional, design tools) · Models: Claude (via Claude Code), OpenAI Codex models, OpenAI gpt-5.5 and gpt-image-2 (design binary) · safety checks passed 9 of 10 · [Repo](https://github.com/garrytan/gstack) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gstack/)</sub>

<a name="reverse-skill"></a>
### #&#8288;25 [reverse-skill](https://github.com/zhaoxuya520/reverse-skill) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Sep 2026</sub>

**Routes AI coding agents to reverse-engineering and pentest playbooks.**

reverse-skill is a skill/routing package for AI coding agents (Claude Code, Codex, Cursor, OpenCode) that, when the agent hits an APK, binary, obfuscated JS, CTF challenge or pentest target, picks the right methodology and tool (jadx, apktool, Frida, IDA, radare2, Ghidra, BurpSuite) instead of guessing commands. Routing is driven by a single JSON config (43-44 rules) validated by a 173-case regression suite and CI on Windows and Ubuntu, covering mobile, firmware, malware, pwn, EDR bypass and API security.

- **+** Client-neutral routing core works with Claude Code, Codex, Cursor and OpenCode
- **+** Single routing.json source of truth with a 173-case regression benchmark run in CI
- **+** Covers a wide scenario matrix: APK, iOS, .NET, JS, firmware, pwn, EDR bypass, CTF
- **+** Includes case/evidence workflow (scope, timeline, findings) not just tool dispatch
- **−** Core scripts are PowerShell-based, with separate bash variants for Linux/macOS/Kali
- **−** Requires external install of Java/JDK, Node.js 22.12+, Python 3.x and the RE tools themselves
- **−** CTF-Sandbox-Orchestrator submodule is GPLv3, mixed licensing alongside the MIT core
- **−** A routing layer, not an RE engine itself, so it depends on tools already being installed

<sub>no GPU · Needs Java/JDK, Node.js 22.12+, Python 3.x, jadx, apktool, Frida, IDA Pro, radare2, Ghidra, Binary Ninja · [Repo](https://github.com/zhaoxuya520/reverse-skill) · [📖 Docs ↗](https://reverse.apivix.com/docs/) · [🌐 Site ↗](https://reverse.apivix.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reverse-skill/)</sub>

<a name="planning-with-files"></a>
### #&#8288;26 [planning-with-files](https://github.com/othmanadi/planning-with-files) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Oct 2026</sub>

**Agent skill that keeps task plans in markdown files on disk across /clear.**

Skill and hook set for coding agents that stores the plan in task_plan.md, findings.md and progress.md in the project. Lifecycle hooks re-inject selected plan context each turn, and a completion gate can hold the agent's stop until the plan reports complete. Installs through `npx skills add` for the Agent Skills standard, with native plugins for Claude Code, Codex CLI, Qoder CLI, Pi, Hermes Agent, OpenCode and DeepSeek Harness.

- **+** Plan state is plain markdown on disk, so it survives /clear, compaction and crashes
- **+** Works across many hosts: native plugins for 7 agents, Agent Skills standard for the rest
- **+** Completion gate can block the agent from stopping until phases are marked complete
- **+** Parallel tasks get isolated .planning/YYYY-MM-DD-slug/ directories (v2.36.0+)
- **−** Plan files are gitignored and overwritten by the next task unless you promote them
- **−** Hook features vary per host; Qoder CLI needs Bash and Python 3.10+
- **−** Completion gate matches literal English status tokens via grep -F
- **−** Benchmark evidence is small: 30 assertions and 3 blind A/B comparisons, run by the author

<sub>no GPU · Needs Bash, Python 3.10+ (Qoder CLI), npx · safety checks passed 10 of 10 · [Repo](https://github.com/othmanadi/planning-with-files) · [📖 Docs ↗](https://github.com/OthmanAdi/planning-with-files/blob/master/docs/installation.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/planning-with-files/)</sub>

<a name="oh-my-codex"></a>
### #&#8288;27 [oh-my-codex](https://github.com/yeachan-heo/oh-my-codex) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

**Workflow layer for Codex CLI with skills, roles and durable project state.**

OMX wraps OpenAI Codex CLI with an `omx` launcher, skills such as `$deep-interview`, `$ralplan`, `$ultragoal`, `$team` and `$code-review`, and specialist roles. Plans, logs, memory and mode state are kept under `.omx/`, and team workers run in separate git worktrees, with tmux for the team runtime. Codex remains the execution engine; OMX adds scoped AGENTS.md guidance and an optional Codex plugin layout.

- **+** Staged workflow: interview, plan, then durable execution with checkpoints in .omx/ultragoal
- **+** Team workers get dedicated git worktrees automatically; named worktrees isolate sessions
- **+** Installs with npm; omx doctor and omx exec smoke test check install and auth
- **+** Also ships a Codex plugin layout with marketplace metadata
- **−** Tuned mainly for macOS/Linux; native Windows and Codex App get less support
- **−** Requires Codex CLI installed and authenticated; does not run standalone
- **−** --madmax disables Codex approvals and sandbox, so only use in trusted repos
- **−** Large skill and command surface; loading many skills bloats context

<sub>no GPU · Needs Node.js 20+, OpenAI Codex CLI, tmux (macOS/Linux team runtime), git · Models: OpenAI Codex CLI models · safety checks passed 9 of 10 · [Repo](https://github.com/yeachan-heo/oh-my-codex) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-codex-website/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-codex/)</sub>

<a name="taste-skill"></a>
### #&#8288;28 [taste-skill](https://github.com/leonxlnx/taste-skill) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 97k · MIT · Oct 2026</sub>

**Agent skills that steer coding agents toward distinctive landing-page design.**

A set of Agent Skills for Codex, Cursor and Claude Code that direct an agent to design public-facing pages. The default skill picks one of three art directions dealt from 20, finds credited open-license photos, builds the page, then checks it in a real browser at three widths and revises up to three rounds. Other skills cover redesigns, image-to-code and fixed visual styles.

- **+** Framework-agnostic: rules cover design, so React, Vue, Svelte and plain HTML all work
- **+** Needs no API keys; scripts run on Node 22+ with Chrome, Edge or Chromium
- **+** Self-checks in a real browser at three widths and fails the page on slop
- **+** Pictures come from open archives (public domain, CC0, CC BY, CC BY-SA) and are credited on the page
- **−** A build takes roughly 30 to 45 minutes and a few hundred thousand tokens
- **−** Default skill targets public pages, not dashboards or app screens
- **−** Picture search needs network access
- **−** No benchmarks or measured quality comparisons given in the README

<sub>no GPU · Needs Node 22+, Chrome, Edge or Chromium, Network access for image search · Models: Claude Code, Codex, Cursor · safety checks passed 8 of 9 · [Repo](https://github.com/leonxlnx/taste-skill) · [🌐 Site ↗](https://tasteskill.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taste-skill/)</sub>

<a name="vercel-labs-skills"></a>
### #&#8288;29 [skills](https://github.com/vercel-labs/skills) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

**CLI that installs SKILL.md agent skills into dozens of coding agents.**

An npm CLI (`npx skills`) that fetches skills defined as SKILL.md files from GitHub, GitLab, Azure Repos, any git URL, a local path or an archive URL, and installs them into each coding agent's skills directory. It supports project or global scope and symlinked or copied installs, and it adds list, find, update, remove and init commands. The README lists about 80 supported agents, including Claude Code, Codex, Cursor and OpenCode.

- **+** One command installs a skill into many agents' directories, using symlinks to a canonical copy
- **+** Accepts GitHub shorthand, GitLab, Azure Repos, any git URL, local paths and archive URLs
- **+** Private repos use existing Git credentials, GitHub CLI or SSH; a token is optional
- **+** Non-interactive flags (-y, --all, -g, -a) make it usable in CI
- **−** Needs Node.js and npx; the README does not state a minimum version
- **−** Only manages skills; it does not supply the agents themselves
- **−** Agent support depends on a hand-maintained table of paths for each agent
- **−** Symlinks may not work on every platform; copy mode is the fallback

<sub>no GPU · Needs Node.js, npx, git · safety checks passed 8 of 10 · [Repo](https://github.com/vercel-labs/skills) · [🌐 Site ↗](https://skills.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vercel-labs-skills/)</sub>

<a name="beads"></a>
### #&#8288;30 [beads](https://github.com/gastownhall/beads) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

**Dependency-aware issue tracker CLI that gives coding agents persistent task memory.**

bd (Beads) is a Go CLI that stores issues as a dependency graph in a Dolt database, so coding agents can list unblocked work with `bd ready`, claim tasks atomically, and close them. It uses hash-based IDs to avoid merge collisions, and syncs across machines with `bd dolt push` and `bd dolt pull`. `bd init` and `bd setup` install guidance and hooks for Claude Code, Codex, Cursor and others.

- **+** Hash-based IDs (bd-a1b2) avoid merge collisions across agents and branches
- **+** Embedded Dolt by default; no separate database server needed for single-writer use
- **+** JSON output and `bd ready` give agents unblocked tasks without parsing markdown plans
- **+** `bd setup` installs integrations for Claude Code, Codex, Cursor, Factory and more
- **−** Embedded mode allows a single writer; concurrent writers need an external dolt sql-server
- **−** Upgrades can need schema migration and a designated clone on remote-backed databases
- **−** HTTP backend is experimental and diverges from local mode in documented ways
- **−** Older binaries refuse to open a database migrated by a newer schema

<sub>no GPU · Needs Dolt, git (optional) · safety checks passed 9 of 10 · [Repo](https://github.com/gastownhall/beads) · [📖 Docs ↗](https://beads.gascity.com/) · [🌐 Site ↗](https://beads.gascity.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beads/)</sub>

<a name="openwiki"></a>
### #&#8288;31 [openwiki](https://github.com/langchain-ai/openwiki) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

**Generates a linked Markdown wiki of your repo for coding agents.**

OpenWiki writes a Markdown wiki into `openwiki/` in a repository, tracks each fact back to source evidence, and updates only what changed. It installs as a skill plus MCP tools into coding agents such as Codex, Claude Code, Cursor and Copilot CLI, or runs as a standalone CLI with its own Deep Agents-based writer. Agents query it through local, model-free `openwiki_search` and `openwiki_read`.

- **+** Installs into ten coding agents, reusing the host's authenticated model session
- **+** Claims tracked to source evidence; clean updates skip model calls
- **+** Search and read tools are local and read-only; workspaces span linked repos
- **+** Resumable page queue; scheduled CI examples for GitHub, GitLab and Bitbucket
- **−** Agent-hosted runs cover repository wikis only; personal wikis need the standalone CLI
- **−** Connector-sourced context, including LangSmith, is not yet supported in host runs
- **−** Visualizer loads graph and Markdown libraries from a public CDN, so it needs internet
- **−** Native CLI needs a separately configured model provider and credentials

<sub>no GPU · Needs Node.js 22.22.0 or newer, A coding agent or a model provider · Models: Fourteen providers, including hosted models, Local OpenAI-compatible endpoints · port 4321 · [Repo](https://github.com/langchain-ai/openwiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openwiki/)</sub>

<a name="agents"></a>
### #&#8288;32 [agents](https://github.com/wshobson/agents) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

**Plugin, agent and skill collection for Claude Code, Codex CLI, Cursor and others.**

A catalog of 94 plugins (92 local, 2 external) holding 202 agents, 184 skills and 105 commands, written once as Markdown in the Claude Code plugin format. Native marketplaces serve Claude Code, Codex CLI and Cursor, while adapters generate artifacts for OpenCode, Antigravity CLI, GitHub Copilot and Pi. Individual skills can be installed alone with `gh skill` or `npx skills`.

- **+** One Markdown source adapted to seven coding tools
- **+** Skills install individually via gh skill or npx skills
- **+** Broad coverage: Python, JavaScript, testing, security, infrastructure
- **+** MIT license; plugin-eval runs static skill checks without model calls
- **−** OpenCode, Antigravity, Copilot and Pi need a clone, uv and Python 3.12+
- **−** Features differ by harness; Codex agents and commands use a separate generated path
- **−** Pi agents need a subagent extension
- **−** plugin-eval LLM judge and Monte Carlo layers are experimental, not validated against human labels

<sub>no GPU · Needs Claude Code, Codex CLI, Cursor, OpenCode, Antigravity CLI, GitHub Copilot or Pi, uv and Python 3.12+ (clone installs), GitHub CLI 2.90+ or Node.js/npm (skills-only installers) · Models: opus, sonnet, haiku, fable, inherit (aliases mapped per harness) · safety checks passed 9 of 10 · [Repo](https://github.com/wshobson/agents) · [📖 Docs ↗](https://github.com/wshobson/agents/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents/)</sub>

<a name="opencodex"></a>
### #&#8288;33 [opencodex](https://github.com/lidge-jun/opencodex) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

**Local proxy that lets Codex, Claude Code and Grok Build use any LLM.**

opencodex is a local proxy that translates Codex's Responses API into the protocol a chosen provider speaks, covering streaming, tool calls, reasoning tokens and images. It also fronts Claude Code, Claude Desktop and Grok Build, with 40+ built-in providers or any OpenAI-compatible endpoint. A web dashboard on port 10100 configures providers, combos with failover, and a ChatGPT account pool with quota-aware routing.

- **+** 40+ built-in providers plus any OpenAI-compatible endpoint, including Ollama for local models
- **+** Combos give one virtual model id with failover or weighted round-robin across providers
- **+** Dashboard on localhost:10100 with live request log; `ocx stop` restores original Codex config
- **+** Installs via npm with bundled Bun runtime; also desktop apps for macOS, Windows and Linux
- **−** ChatGPT account pooling may conflict with provider terms; README warns of possible enforcement
- **−** Desktop app is beta and the Windows .msi is not code-signed
- **−** Cursor provider is marked experimental
- **−** JEV Auto routing is tested only against a mocked endpoint, not a live account

<sub>no GPU · Docker + Compose · Needs Node 18+, Bun (bundled on npm install) · Models: Anthropic, Google Gemini, xAI Grok, OpenAI, DeepSeek · port 10100 · safety checks passed 9 of 10 · [Repo](https://github.com/lidge-jun/opencodex) · [📖 Docs ↗](https://opencodex.me/getting-started/installation/) · [🌐 Site ↗](https://opencodex.me/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencodex/)</sub>

<a name="ai-memory"></a>
### #&#8288;34 [ai-memory](https://github.com/akitaonrails/ai-memory) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · MIT · Oct 2026</sub>

**Shared long-term memory server for coding agents, stored as git-backed markdown.**

ai-memory is a Rust server that records coding-agent sessions through lifecycle hooks and MCP, consolidates them into markdown wiki pages in git, and injects a brief into the next session. Handoffs let you move from Claude Code to Codex or another supported agent, across machines or team members. Capture, FTS search and handoffs work with no LLM call; vectors and LLM consolidation are optional.

- **+** Markdown wiki in git is the source of truth; the database index can be rebuilt
- **+** Default path needs no LLM or API key: capture, FTS search, handoffs
- **+** Over twenty agent harnesses supported, with claim-once typed handoffs between them
- **+** Multi-user auth, attribution and audit log included, not a paid tier
- **−** Native Windows support is experimental; WSL2 is the supported route
- **−** Docker quick-start runs with no authentication unless a token is added
- **−** Compaction, dedup and LLM dream pass are off by default and need opt-in
- **−** Several agents (Claude Desktop, Zed, VS Code Copilot) are MCP-only, without hooks

<sub>no GPU · Docker + Compose · Needs SQLite, git, systemd or launchd (native service) · Models: Anthropic (optional LLM), OpenAI (optional embeddings), local embeddings (optional) · port 49374 · [Repo](https://github.com/akitaonrails/ai-memory) · [📖 Docs ↗](https://github.com/akitaonrails/ai-memory/blob/master/docs/install.md) · [🌐 Site ↗](https://aimemory.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-memory/)</sub>

<a name="waza"></a>
### #&#8288;35 [waza](https://github.com/tw93/waza) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

**Eight agent skills for planning, debugging, review and writing.**

Waza is a set of eight agent skills (/think, /ui, /check, /hunt, /write, /learn, /read, /health), each a folder with reference docs, helper scripts and gotchas. It installs with `npx skills` into the shared ~/.agents/skills directory, as a Claude Code or Codex plugin, or as a Claude Desktop ZIP. Extras include a Claude Code statusline and optional persistent rules.

- **+** Small fixed set of eight skills, each with one trigger and one job
- **+** One install covers Claude Code, Codex, Cursor and other agents reading ~/.agents/skills
- **+** Also ships as Claude Code and Codex plugins, a Claude Desktop ZIP and a Pi npm package
- **+** Optional rules and a quota statusline are separate installs, not forced on
- **−** Reflects one author's workflow; the README describes no per-skill configuration
- **−** Clarity rule is only on main and not in the current release
- **−** Extras install by running downloaded shell scripts; the README asks you to review first
- **−** Statusline script targets Claude Code only; Codex needs manual config.toml edits

<sub>no GPU · Needs Node.js (npx), Claude Code, Codex, Cursor or another skills-capable agent · [Repo](https://github.com/tw93/waza) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/waza/)</sub>

<a name="claude-code-router"></a>
### #&#8288;36 [claude-code-router](https://github.com/musistudio/claude-code-router) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · MIT · Oct 2026</sub>

**Local gateway that routes coding agents to the model providers you choose.**

Claude Code Router runs a local gateway on port 3456 that Claude Code, Codex, Grok CLI, Kimi CLI, Kilo Code, OpenCode and other clients point at. Providers, models, credentials and routing rules are managed in an Electron desktop app or an npm CLI with a browser UI. It adds retries, ordered fallbacks, credential pools, request logs with token and cost estimates, and tools such as web search, MCP and ToolHub.

- **+** One local endpoint for ten named agents, so provider config lives in one place
- **+** Retries, key rotation, credential pools and ordered fallback models are built in
- **+** Logs show resolved provider, model, latency, tokens and estimated cost per request
- **+** Ships as desktop app (macOS, Windows, Linux), npm CLI or Docker Compose
- **−** Docker script builds against a sibling ../../next-ai/gateway checkout when present
- **−** Windows desktop packaging must run on Windows x64 because of native better-sqlite3
- **−** Remote exposure needs care; README points to a separate Docker guide for it
- **−** Large surface (AgentClaw chat relays, browser automation, plugins) beyond plain routing

<sub>no GPU · Docker + Compose · Needs Node.js 22+ for CLI, Docker (optional) · Models: OpenAI Chat/Responses, Anthropic Messages, Gemini, OpenRouter, DeepSeek · port 3458 · [Repo](https://github.com/musistudio/claude-code-router) · [📖 Docs ↗](https://ccrdesk.top/en/guides/install/) · [🌐 Site ↗](https://ccrdesk.top/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-router/)</sub>

<a name="browser-harness"></a>
### #&#8288;37 [browser-harness](https://github.com/browser-use/browser-harness) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**Lets an LLM drive your real Chrome session over a single CDP websocket.**

Browser Harness connects a coding agent such as Claude Code or Codex to your own logged-in browser through the Chrome DevTools Protocol. The agent writes missing helper functions into a local workspace file as it works, while the core package under src/browser_harness stays protected. It also ships an MCP server, browser-harness-mcp, that exposes the browser helpers as tools over stdio.

- **+** Uses your real browser, so existing logins and sessions are available to the agent
- **+** Agent adds its own helpers to agent_helpers.py when one is missing
- **+** MCP server over stdio works with Claude Code, Cursor, Devin and other clients
- **+** MIT license; install and connection steps documented in install.md
- **−** Requires enabling remote debugging in Chrome, which exposes your personal browser to the agent
- **−** Parallel browsers, proxies, stealth and CAPTCHA solving are offered only via Browser Use Cloud
- **−** Agent-written helpers are not reviewed, so behavior can vary between runs
- **−** README gives no model list, hardware needs or test coverage details

<sub>no GPU · Needs Chrome with remote debugging enabled, uv, Python 3.12 · Models: Claude Code, Codex, MCP clients · [Repo](https://github.com/browser-use/browser-harness) · [📖 Docs ↗](https://github.com/browser-use/browser-harness/blob/main/install.md) · [🌐 Site ↗](https://cloud.browser-use.com/v4) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browser-harness/)</sub>

<a name="cc-haha"></a>
### #&#8288;38 [cc-haha](https://github.com/nanmicoder/cc-haha) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

**Electron desktop workbench for Claude Code with diff review and multi-session tabs.**

cc-haha is an Electron and React desktop app for macOS, Windows and Linux that wraps a Claude Code-style agent runtime built on Bun. It adds multi-session tabs, per-file diff review, an in-app browser preview, graphical permission approval, MCP and SubAgent management, and Computer Use. Models can be Claude, ChatGPT or Grok accounts, third-party APIs such as DeepSeek, Kimi and GLM, or local endpoints in LM Studio and Ollama.

- **+** Installers for macOS, Windows and Linux; CLI also runs from source with Bun
- **+** Model choice includes Claude, ChatGPT, Grok, DeepSeek, Kimi, GLM, LM Studio and Ollama
- **+** Per-file syntax-highlighted diffs, with the whole turn revertible
- **+** Remote access via phone browser (H5) and IM bridges such as Telegram, Slack and Feishu
- **−** README does not state RAM or system requirements
- **−** Unsigned Windows and draft macOS builds can trigger SmartScreen or Gatekeeper prompts
- **−** README carries sponsor and affiliate promotions for third-party API resellers
- **−** Main README and most of its text are in Chinese; English is a separate file

<sub>no GPU · Needs Bun, Electron, Model provider API key or account · Models: Claude, ChatGPT, Grok, DeepSeek, Kimi · [Repo](https://github.com/nanmicoder/cc-haha) · [📖 Docs ↗](https://cchaha.ai) · [🌐 Site ↗](https://cchaha.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-haha/)</sub>

<a name="plannotator"></a>
### #&#8288;39 [plannotator](https://github.com/backnotprop/plannotator) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · Apache-2.0 · Oct 2026</sub>

**Browser UI to annotate agent plans and review diffs, then send feedback back.**

Plannotator hooks into coding agents (Claude Code, Codex, Copilot CLI, Gemini CLI, OpenCode, Kiro, Droid, Amp, Pi) and opens their plans, markdown, HTML and diffs in a local browser UI. You annotate, approve or deny, and the structured feedback goes back to the agent. Code review covers local changes and GitHub/GitLab PRs, with Git, GitButler, jj and Perforce support.

- **+** Covers nine agents through hooks, plugins or skills; one installer auto-detects and configures them
- **+** Reviews local diffs and GitHub/GitLab PRs; supports Git, GitButler, jj and Perforce
- **+** No usage telemetry; plans, diffs and annotations stay local by default
- **+** Plan mode opens the review UI automatically via ExitPlanMode and equivalent hooks
- **−** Release check against GitHub on each page load has no opt-out setting
- **−** Droid integration is commands only, with no plan interception
- **−** Link sharing is moving to deprecated support; team sharing is a hosted Workspaces product
- **−** Setup differs per agent, with manual steps for Amp, Claude Code, Copilot and OpenCode

<sub>no GPU · Needs A supported coding agent CLI, Git, GitHub CLI or GitLab CLI for PR review · [Repo](https://github.com/backnotprop/plannotator) · [▶️ Demo ↗](https://www.youtube.com/watch?v=a_AT7cEN_9I) · [📖 Docs ↗](https://docs.plannotator.ai/open-source/start/installation) · [🌐 Site ↗](https://plannotator.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/plannotator/)</sub>

<a name="claude-howto"></a>
### #&#8288;40 [claude-howto](https://github.com/luongnv89/claude-howto) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Oct 2026</sub>

**Tutorial modules and copy-paste templates for learning Claude Code features.**

A Markdown guide with 10 tutorial modules covering Claude Code slash commands, memory, skills, subagents, MCP, hooks, plugins, checkpoints, advanced features and the CLI. Each module has Mermaid diagrams and templates you copy into .claude/ or ~/.claude/. It also ships /self-assessment and /lesson-quiz commands and a learning path the README estimates at 11-13 hours.

- **+** Templates for each feature: commands, CLAUDE.md, hook scripts, MCP configs, subagents, plugins
- **+** Ordered learning path with time estimates per module
- **+** Built-in /self-assessment and /lesson-quiz commands for finding gaps
- **+** MIT licensed; README says it is synced with each Claude Code release
- **−** Tied to Claude Code only; templates are not for other coding agents
- **−** Documentation and examples, not an installable tool or library
- **−** Most templates are copied by hand; only the plugin examples use /plugin install
- **−** Can lag behind Claude Code changes between releases

<sub>no GPU · Needs Claude Code, Node.js (npx for MCP server examples), uv (optional, EPUB build script) · Models: Claude Opus, Claude Sonnet, Claude Haiku · safety checks passed 10 of 10 · [Repo](https://github.com/luongnv89/claude-howto) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-howto/)</sub>

<a name="claude-code-templates"></a>
### #&#8288;41 [claude-code-templates](https://github.com/davila7/claude-code-templates) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

**Installable agents, commands, hooks and MCP configs for Claude Code.**

A catalog of Claude Code components (agents, slash commands, settings, hooks, MCP integrations and skills) installed per item with `npx claude-code-templates@latest` and browsable at aitmpl.com. It also ships npx-run tools: an analytics view for Claude Code sessions, a mobile-friendly conversation monitor with optional Cloudflare Tunnel access, a health check and a plugin dashboard.

- **+** One npx command installs a chosen agent, command, hook, setting, skill or MCP
- **+** Web catalog at aitmpl.com plus docs at docs.aitmpl.com
- **+** Includes analytics, health-check and conversation-monitor tools beyond the templates
- **+** MIT license; bundled third-party components keep their original licenses
- **−** Targets Claude Code only; no other coding assistant is mentioned
- **−** Many components come from third-party repos under mixed licenses (MIT, CC0, Apache 2.0)
- **−** README gives no per-component quality or review process; vetting is left to the user
- **−** Requires Node.js for npx; version requirements are unknown

<sub>no GPU · Needs Node.js/npx, Claude Code, Cloudflare Tunnel (optional, for remote chat monitor) · safety checks passed 6 of 11 · [Repo](https://github.com/davila7/claude-code-templates) · [📖 Docs ↗](https://docs.aitmpl.com) · [🌐 Site ↗](https://aitmpl.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-templates/)</sub>

<a name="claude-skills"></a>
### #&#8288;42 [claude-skills](https://github.com/alirezarezvani/claude-skills) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Aug 2026</sub>

**Skills and plugins library for Claude Code, Codex, Gemini CLI and Cursor.**

A collection of SKILL.md instruction packages, stdlib-only Python CLI scripts and reference docs across 20 domains, including engineering, marketing, compliance, C-level advisory and research. It installs as Claude Code plugins from a marketplace, or converts with scripts/convert.sh into Cursor, Aider, Windsurf, Kilo Code, OpenCode and Augment formats. Personas and agent definitions are included.

- **+** Python tools are stdlib-only, no pip installs required
- **+** Installs via Claude Code plugin marketplace, per domain or per skill
- **+** convert.sh and install.sh target Cursor, Aider, Windsurf, Kilo Code, OpenCode, Augment
- **+** Includes a skill-security-auditor to scan skills before installation
- **−** Broad scope; many domains are non-coding (marketing, finance, compliance)
- **−** README counts are inconsistent (345 vs 388 skills, 5,200+ stars claim)
- **−** Hermes Agent and Mistral Vibe need a manual one-time sync script
- **−** Windows needs a symlink-enabled clone and PYTHONUTF8=1 for mirror trees

<sub>no GPU · Needs Python 3, Claude Code or another supported coding agent · safety checks passed 5 of 8 · [Repo](https://github.com/alirezarezvani/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-skills/)</sub>

<a name="jeffallan-claude-skills"></a>
### #&#8288;43 [claude-skills](https://github.com/jeffallan/claude-skills) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Claude Code plugin with 67 role-based skills and 9 Jira-linked workflow commands.**

A Claude Code plugin that installs 67 skills covering languages, frameworks, infrastructure, testing, DevOps and security. Skills activate from the request text and load per-topic reference files (371 in total). It also ships 9 workflow commands for managing epics with Jira and Confluence, and a /common-ground command that surfaces Claude's assumptions about the project.

- **+** Installs through the Claude Code plugin marketplace with two commands
- **+** Skills activate from the request and load only the relevant reference file
- **+** Covers 12 categories, from languages to security and data/ML
- **+** Documented multi-skill workflows, e.g. feature development through code review
- **−** Built for Claude Code; support for other agents is not stated
- **−** Workflow commands require an Atlassian MCP server to be set up
- **−** Quality and overlap across 67 skills cannot be judged from the README
- **−** Skills are prompt text, so results depend on the model used

<sub>no GPU · Needs Claude Code, Atlassian MCP server (workflow commands only) · Models: Claude · [Repo](https://github.com/jeffallan/claude-skills) · [📖 Docs ↗](https://jeffallan.github.io/claude-skills) · [🌐 Site ↗](https://jeffallan.github.io/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jeffallan-claude-skills/)</sub>

<a name="worktrunk"></a>
### #&#8288;44 [worktrunk](https://github.com/max-sixty/worktrunk) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · custom license · Oct 2026</sub>

**Git worktree manager CLI for running AI coding agents in parallel.**

Worktrunk is a Rust CLI that wraps git worktree so worktrees are addressed by branch name, with paths computed from a configurable template. Commands like `wt switch -c -x claude feat` create a worktree and launch an agent in it, and `wt merge` squashes, rebases, merges and cleans up. It also offers hooks, an interactive picker, CI status in `wt list --full`, and copy-on-write sharing of build caches on APFS, btrfs and XFS.

- **+** Create a worktree and start an agent in one command (`wt switch -c -x claude`)
- **+** Hooks on create, pre-merge and post-merge automate per-worktree setup
- **+** Shares target/ and node_modules/ across worktrees via copy-on-write on APFS, btrfs, XFS
- **+** Installs through Homebrew, Cargo, Winget, pacman and conda; shell integration for several shells
- **−** Needs a shell integration step (`wt config shell install`) before it can change directories
- **−** On Windows, `wt` clashes with Windows Terminal; Winget installs it as `git-wt`
- **−** Cache sharing only works on APFS, btrfs and XFS filesystems
- **−** LLM commit messages and summaries need a separately configured model; supported providers unknown from README

<sub>no GPU · Needs git · [Repo](https://github.com/max-sixty/worktrunk) · [📖 Docs ↗](https://worktrunk.dev) · [🌐 Site ↗](https://worktrunk.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/worktrunk/)</sub>

<a name="zcf"></a>
### #&#8288;45 [zcf](https://github.com/ufomiao/zcf) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Aug 2026</sub>

**npx installer that configures Claude Code and Codex with workflows, MCP and API presets.**

ZCF is an npx-run CLI that sets up Claude Code and Codex: it installs the tools, writes workflow and agent configuration, and configures API providers or CCR and MCP services. It has an interactive menu plus non-interactive flags such as `npx zcf i -s -p 302ai -k "sk-xxx"`, and supports English, Chinese and Japanese interfaces. Detailed usage lives in the external docs site.

- **+** Single `npx zcf` entry point, no manual install step
- **+** Non-interactive mode with provider preset and key flags for scripted setup
- **+** Covers both Claude Code and Codex, including workflow updates via `zcf u`
- **+** Interface available in English, Chinese and Japanese
- **−** README gives little detail on what workflows or agents are installed
- **−** Requires Node.js and your own API key or provider account
- **−** README is mostly sponsor promotions for API relay services
- **−** Full usage and options only in external documentation

<sub>no GPU · Needs Node.js (npx), Claude Code or Codex, API provider key · Models: Claude, Codex, 302.AI preset · [Repo](https://github.com/ufomiao/zcf) · [📖 Docs ↗](https://zcf.ufomiao.com/) · [🌐 Site ↗](https://zcf.ufomiao.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/zcf/)</sub>

<a name="ouroboros"></a>
### #&#8288;46 [ouroboros](https://github.com/q00/ouroboros) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Oct 2026</sub>

**Spec-first workflow engine that interviews you, then runs and evaluates coding agents.**

Ouroboros adds an `ooo` command set to coding-agent CLIs. It runs a Socratic interview that produces an immutable Seed spec with an ambiguity score, then executes, evaluates through a 3-stage gate, and evolves the result, recording actions in a replayable ledger. It registers as an MCP server and supports Claude Code, Codex CLI, OpenCode, Hermes, Gemini, Kiro, Copilot and others.

- **+** Works across about 14 agent hosts, including Claude Code, Codex CLI, Kiro and Copilot CLI
- **+** Interview step yields a locked Seed spec with a measurable ambiguity score
- **+** Ships as a Claude Code and Codex plugin, pip package, Homebrew tap or one-line installer
- **+** MIT licensed, with recent commits and releases
- **−** Native Windows is experimental, and Codex CLI on Windows needs WSL 2
- **−** Python 3.12 or newer required; LiteLLM profiles limited to 3.12-3.13
- **−** Many install profiles and MCP v1/v2 splits make setup choices confusing
- **−** Needs an existing coding agent or LLM backend; it does not run models itself

<sub>no GPU · Needs Python >= 3.12, uv or pipx, A supported coding-agent CLI or LLM backend · Models: Claude Code, Codex CLI, OpenCode, Hermes, Gemini · [Repo](https://github.com/q00/ouroboros) · [📖 Docs ↗](https://ouroboros.page/learn/en/) · [🌐 Site ↗](https://ouroboros.page/learn/en/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ouroboros/)</sub>

<a name="claude-code-best-practice"></a>
### #&#8288;47 [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 68k · MIT · Oct 2026</sub>

**Reference repo of Claude Code configuration patterns and guides.**

A documentation-first repository that catalogs Claude Code features (subagents, commands, skills, hooks, MCP, settings, memory) with write-ups and example configs under .claude/. It includes a command-to-agent-to-skill orchestration demo (/weather-orchestrator) and a table comparing community workflows such as Superpowers, Spec Kit and OpenSpec.

- **+** Each concept links to a guide page and a matching implemented example in the repo
- **+** Working orchestration demo wires a command, an agent and a skill together
- **+** Workflow comparison table lists agent, command and skill counts per project
- **+** Covers recent Claude Code features such as auto mode, worktrees and agent teams
- **−** Reference material only; not an installable plugin or package
- **−** Specific to Claude Code; limited use with other coding agents
- **−** Many entries link out to external docs and tweets rather than local content
- **−** Several listed features are marked beta and may change between releases

<sub>no GPU · Needs Claude Code · Models: Claude · safety checks passed 7 of 8 · [Repo](https://github.com/shanraisshan/claude-code-best-practice) · [📖 Docs ↗](https://code.claude.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-best-practice/)</sub>

<a name="i-have-adhd"></a>
### #&#8288;48 [i-have-adhd](https://github.com/ayghri/i-have-adhd) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 57k · MIT · Oct 2026</sub>

**Skill that makes coding assistants answer action-first with numbered steps.**

A skill/plugin for coding assistants such as Claude Code that rewrites response style around 10 rules: lead with the next action, number multi-step tasks, cap lists at 5 items, give time estimates in minutes, and drop preambles, recaps and closers. Behavior is defined in skills/i-have-adhd/SKILL.md, and you can fork and edit that file, then reinstall your copy through the plugin marketplace commands.

- **+** Behavior lives in one editable SKILL.md with 10 explicit rules
- **+** Before/after example shows the exact output change
- **+** Install is a single prompt pasted into the assistant
- **+** MIT licensed; README translated into 10 languages
- **−** Only changes response style; adds no tools or capabilities
- **−** Tune-it steps shown only for Claude Code plugin commands
- **−** No tagged releases
- **−** No evidence offered that it improves outcomes beyond one example

<sub>no GPU · Needs Claude Code or compatible coding assistant · safety checks passed 9 of 10 · [Repo](https://github.com/ayghri/i-have-adhd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/i-have-adhd/)</sub>

<a name="awesome-claude-code-subagents"></a>
### #&#8288;49 [awesome-claude-code-subagents](https://github.com/voltagent/awesome-claude-code-subagents) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

**Collection of 161+ Claude Code subagent definitions in 10 categories.**

Markdown subagent definitions for Claude Code, grouped into 10 categories such as core development, language specialists, infrastructure, quality and security, and data and AI. Install them as Claude Code plugins (for example voltagent-lang), by copying files into ~/.claude/agents/ or .claude/agents/, or with a shell installer script.

- **+** Installable per category via claude plugin marketplace, so you add only the groups you need
- **+** Covers many languages and frameworks, including Django, Rails, Spring Boot, Flutter and Terraform
- **+** Interactive and standalone shell installers; standalone one needs only curl
- **+** MIT licensed; agents are plain Markdown files you can copy and edit
- **−** Prompt definitions only; README shows no tests or evals of agent quality
- **−** Written for Claude Code; other agent tools would need the files adapted
- **−** Meta-orchestration agents are meant to be used with other categories installed too
- **−** No tagged releases; README carries sponsor placements

<sub>no GPU · Needs Claude Code, curl (standalone installer) · Models: Claude · safety checks passed 8 of 9 · [Repo](https://github.com/voltagent/awesome-claude-code-subagents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-claude-code-subagents/)</sub>

<a name="claude-video"></a>
### #&#8288;50 [claude-video](https://github.com/bradautomates/claude-video) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Sep 2026</sub>

**Agent skill that turns a video URL or file into timestamped frames and transcript.**

Watch is a skill/plugin for Claude Code, Codex and other Agent Skills hosts. It converts a video URL or local file into timestamped frames and a transcript, using native captions first and optional WhisperX, Groq or OpenAI transcription otherwise. With a GEMINI_API_KEY it can instead send the video to Gemini and relay the timestamped answer.

- **+** Installs as a plugin in Claude Code or as a skill in Codex and other hosts
- **+** Local engine works without an API key, using ffmpeg and yt-dlp
- **+** Frame detail levels, caps, start/end ranges and cue timestamps are configurable
- **+** Captions are used first; WhisperX, Groq or OpenAI only as fallback
- **−** Does not work in Claude Chat or Cowork
- **−** Requires Python 3.10+, FFmpeg and current yt-dlp installed separately
- **−** YouTube also needs a JavaScript runtime such as Deno
- **−** WhisperX is verified only on Apple Silicon; other platforms untested

<sub>RAM ≥ 8 GB · GPU optional · Needs Python 3.10+, FFmpeg, yt-dlp, Deno (YouTube), WhisperX 3.8.6 (optional), Node.js (Skills CLI install only) · Models: Gemini (gemini-3.7-flash default), WhisperX, Groq whisper-large-v3, OpenAI whisper-1 · safety checks passed 8 of 9 · [Repo](https://github.com/bradautomates/claude-video) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-video/)</sub>

<a name="video-shotcraft"></a>
### #&#8288;51 [video-shotcraft](https://github.com/vincentwei1021/video-shotcraft) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · Apache-2.0 · Oct 2026</sub>

**Claude Code and Codex skill that builds promo videos with Remotion.**

An agent skill for Claude Code and Codex that captures your product's real pages, picks from 150 shots (124 recipe cards), and renders a 1920x1080, 30 fps MP4 using Remotion. Every frame is drawn by code from your screenshots and copy, so the output is a editable React project. It also adds sound design and beat sync, opens a browser-based editor (Motion Workbench), and can export a JianYing draft.

- **+** Output is a full Remotion project, so every shot stays editable React code
- **+** Ships 124 recipe cards, 149 SFX and 5 BGM tracks, plus a runnable template
- **+** Motion Workbench edits copy, timing and shots after delivery; preview and render match
- **+** Optional JianYing draft export and Upload-Post social publishing
- **−** Tested on macOS; headless Linux needs three workarounds (concurrency, chrome-headless-shell, CDN)
- **−** Remotion has its own license; companies may need a paid one
- **−** Only Claude Code and Codex are targeted; other agents are not mentioned
- **−** JianYing export verified only on macOS; Windows installer untested

<sub>no GPU · Needs Node.js and npm, Remotion, ffmpeg / ffprobe, uv (BGM beat analysis only), puppeteer (page capture only) · Models: Claude Code, Codex · [Repo](https://github.com/vincentwei1021/video-shotcraft) · [▶️ Demo ↗](https://vincentwei1021.github.io/video-shotcraft/) · [📖 Docs ↗](https://github.com/Vincentwei1021/video-shotcraft/blob/main/references/pipeline.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/video-shotcraft/)</sub>

<a name="understand-anything"></a>
### #&#8288;52 [understand-anything](https://github.com/egonex-ai/understand-anything) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 86k · MIT · Oct 2026</sub>

**Plugin that builds an explorable knowledge graph of a codebase or wiki.**

Understand Anything is a plugin for Claude Code and about 15 other agent platforms. Its /understand command runs a multi-agent pipeline that combines Tree-sitter parsing with LLM summaries to write a knowledge graph to .ua/knowledge-graph.json. A local dashboard then offers graph navigation, search, guided tours, diff impact analysis and chat, and /understand-knowledge handles Karpathy-style LLM wikis.

- **+** Tree-sitter extracts imports and call sites deterministically, so structural edges are reproducible
- **+** Graph is plain JSON that can be committed; teammates view it with Node.js >= 18 and no LLM
- **+** Incremental re-analysis of changed files, plus an optional post-commit auto-update hook
- **+** Installs on Claude Code, Cursor, Copilot, Codex, Gemini CLI, OpenCode, Kiro and others
- **−** First /understand run on a large repo can use a significant number of tokens
- **−** Needs a host agent platform and an LLM; it is not a standalone tool
- **−** Output languages limited to en, zh, zh-TW, ja, ko, ru, vi
- **−** Graphs over 10 MB need git-lfs to commit comfortably

<sub>no GPU · Needs Claude Code or another supported agent platform, Node.js >= 18 (standalone viewer), pnpm (building from source) · Models: Whatever the host platform uses, Local models via Ollama · port 5173 · safety checks passed 9 of 11 · [Repo](https://github.com/egonex-ai/understand-anything) · [▶️ Demo ↗](https://understand-anything.com/demo/) · [🌐 Site ↗](https://understand-anything.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/understand-anything/)</sub>

<a name="diagram-design"></a>
### #&#8288;53 [diagram-design](https://github.com/cathrynlavery/diagram-design) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 56k · MIT · Oct 2026</sub>

**Agent skill that draws brand-styled diagrams as single HTML and SVG files.**

An Agent Skill that has a coding agent write one self-contained HTML file with inline SVG for a requested diagram. It covers 45 diagram types, each in minimal light, minimal dark and full-editorial variants, and can pull a site's palette and fonts so later diagrams match. It also imports Mermaid, draw.io and Excalidraw files and exports to SVG or PNG.

- **+** Output is one HTML file with inline SVG; no build step, JavaScript or external images
- **+** 45 diagram types, each in light, dark and editorial variants
- **+** Installs on many hosts: Claude Code, Codex, Copilot, Cursor, Gemini CLI, Cline, Pi, Kiro
- **+** CI checks for overlaps and clipping; layout is on a 4px grid
- **−** Output quality depends on the model; the same prompt can lay out differently twice
- **−** Not an editable source format: no text to diff, no canvas to drag boxes on
- **−** One opinionated editorial style; other looks need style guide edits
- **−** Slash commands (/export-diagram, /profile) only in native packages, not the skills CLI install

<sub>no GPU · Needs An Agent Skills-compatible coding agent (Claude Code, Codex, Cursor, etc.), Node.js (npx) for the skills CLI install · Models: Any model running in the host agent · safety checks passed 10 of 10 · [Repo](https://github.com/cathrynlavery/diagram-design) · [▶️ Demo ↗](https://cathrynlavery.github.io/diagram-design/) · [🌐 Site ↗](https://diagramdesign.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diagram-design/)</sub>

<a name="claude-code-game-studios"></a>
### #&#8288;54 [claude-code-game-studios](https://github.com/donchitos/claude-code-game-studios) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Oct 2026</sub>

**Claude Code template with 49 game-studio subagents, 74 slash-command skills and hooks.**

A project template that adds studio-style structure to Claude Code for game development: 49 subagents in three tiers, 74 skills such as /start, /brainstorm and /dev-story, 12 hooks and 13 path-scoped rules. A project.yaml `modes.rigor` setting (minimal, standard, full) controls how much documentation and review the workflow requires. It includes agent sets for Godot 4, Unity and Unreal Engine 5.

- **+** Engine-specific agent sets for Godot 4, Unity and Unreal Engine 5
- **+** Single modes.rigor setting scales process from jam-style minimal to full director review
- **+** Hooks validate commits, pushes and asset JSON; deny rules block force push and rm -rf
- **+** Stories that change visuals need a launched game and a retained screenshot to close
- **−** Requires Claude Code; no other coding agent is mentioned
- **−** Hooks need Bash, and Python 3 is needed to read project.yaml
- **−** README's own test ranked the standard rigor build last against minimal
- **−** No sample game is shipped, so output quality cannot be inspected in the repo

<sub>no GPU · Needs Claude Code, Git, Python 3, Bash, jq (recommended) · Models: Claude (Opus, Sonnet, or session model) · safety checks passed 8 of 8 · [Repo](https://github.com/donchitos/claude-code-game-studios) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-game-studios/)</sub>

<a name="gsd-core"></a>
### #&#8288;55 [gsd-core](https://github.com/open-gsd/gsd-core) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

**Spec-driven phase loop that runs AI coding agents in fresh-context subagents.**

GSD Core installs commands and agents into coding runtimes such as Claude Code, Codex, Cursor, Copilot and Windsurf. It drives each milestone through a discuss, plan, execute, verify, ship loop, running research and execution in fresh-context subagents to limit context rot. State persists between sessions in files like STATE.md and CONTEXT.md.

- **+** One installer targets many runtimes, including Claude Code, Codex, Cursor, Copilot, OpenCode and Kimi CLI
- **+** Persists project state in STATE.md and CONTEXT.md across sessions
- **+** Verify step walks through built work and generates fix plans before a phase closes
- **+** Docs split into tutorials, how-to guides, reference and explanation
- **−** Must be installed through its installer; copying agents/ or commands/ files directly is unsupported
- **−** Fixed five-step phase loop imposes a workflow on every project
- **−** Default install path uses npx, so it needs Node.js; other runtimes need a separate guide
- **−** README gives no benchmarks for its context-rot claims

<sub>no GPU · Needs Node.js, npm · Models: Claude Code, Codex, OpenCode, Antigravity CLI, Kimi CLI · [Repo](https://github.com/open-gsd/gsd-core) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gsd-core/)</sub>

<a name="visual-explainer"></a>
### #&#8288;56 [visual-explainer](https://github.com/nicobailon/visual-explainer) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

**Agent skill that renders diagrams, diff reviews and tables as styled HTML pages.**

An agent skill that makes a coding agent write a self-contained HTML page and open it in the browser, instead of printing ASCII diagrams and pipe tables. It ships command templates such as /diff-review and /plan-review, plus a local stdio MCP server, a native Pi tool, and optional PPTX and MP4 export. It installs as a Claude Code plugin or by copying the skill directory for Codex, Cursor, OpenCode and Antigravity.

- **+** Normal skill use needs only a browser: no build step, no runtime dependencies
- **+** Works across many harnesses: Claude Code, Codex, Cursor, OpenCode, Pi, Antigravity
- **+** MCP server is local stdio only, no LLM calls, writes confined to an output directory
- **+** Bundled commands for diff review, plan review, slides, fact-check and project recap
- **−** Non-Claude harnesses need manual copy installs; prompt support varies by build
- **−** Video export needs ffmpeg, Chrome and playwright-core installed separately
- **−** PPTX export is a static utility for simple HTML slide decks only
- **−** Output quality depends on the agent model following the skill instructions

<sub>no GPU · Needs Web browser, Node.js (optional MCP and PPTX utilities), ffmpeg, Chrome, playwright-core (optional video export) · [Repo](https://github.com/nicobailon/visual-explainer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/visual-explainer/)</sub>

<a name="drawio-skill"></a>
### #&#8288;57 [drawio-skill](https://github.com/agents365-ai/drawio-skill) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

**Agent skill that generates and syncs editable draw.io diagrams from prompts and code.**

An Agent Skills package for Claude Code, Cursor, Copilot, Codex and similar agents. It writes .drawio XML from natural language, Mermaid, images, Terraform, Kubernetes, SQL DDL, OpenAPI and code import graphs, then exports through the draw.io desktop CLI and checks the rendered PNG. A diagramctl CLI adds sync that keeps manual layout, architecture rule checks for CI, and an optional MCP server.

- **+** 16 importers, including Terraform, Kubernetes, SQL DDL, OpenAPI and Python/JS/Go/Rust import graphs
- **+** Sync updates changed nodes while preserving manually tuned coordinates and styles
- **+** Resolves 10,000+ official draw.io shapes and 321 AI/LLM logos instead of guessed styles
- **+** Core workflows are stdlib-only and offline; architecture rules run in CI via a GitHub Action
- **−** Requires the draw.io desktop CLI; version 30 or later needed for Mermaid and ELK layout
- **−** Auto-layout needs Graphviz; headless Linux export needs xvfb
- **−** AI logos load from the unpkg CDN by default, so rendering needs network unless embedded
- **−** Many scripts and flags make it harder to learn than a plain diagram prompt

<sub>no GPU · Needs draw.io desktop CLI, Graphviz (optional), xvfb (Linux headless), Python 3 · Models: Claude Code, Cursor, Copilot, Codex, OpenClaw · [Repo](https://github.com/agents365-ai/drawio-skill) · [📖 Docs ↗](https://agents365-ai.github.io/drawio-skill/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/drawio-skill/)</sub>

<a name="context-mode"></a>
### #&#8288;58 [context-mode](https://github.com/mksglu/context-mode) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · custom license · Oct 2026</sub>

**MCP server that keeps raw tool output out of the context window.**

Context Mode is an MCP server that runs analysis in a sandbox so raw tool output stays out of the agent's context. It logs edits, git operations and tasks in SQLite, indexes them with FTS5, and retrieves relevant events via BM25 after compaction. It ships hooks and routing for Claude Code, Gemini CLI, Copilot, Cursor and others.

- **+** Sandbox tools cut raw output; README cites 315 KB reduced to 5.4 KB
- **+** Session events stored in SQLite with FTS5/BM25 retrieval after compaction
- **+** Hooks for Claude Code, Gemini CLI, VS Code and JetBrains Copilot, Copilot CLI, Cursor
- **+** Claude Code plugin install, plus MCP-only option via npx
- **−** Elastic License 2.0, not an OSI open-source license
- **−** Non-hook platforms need a manual routing file copy
- **−** Most platforms require Node.js >= 22.5 or Bun
- **−** Savings figures are README examples, not independent benchmarks

<sub>no GPU · Needs Node.js >= 22.5 or Bun · Models: Claude Code, Gemini CLI, VS Code Copilot, JetBrains Copilot, GitHub Copilot CLI · safety checks passed 11 of 16 · [Repo](https://github.com/mksglu/context-mode) · [🌐 Site ↗](https://context-mode.com/insight) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-mode/)</sub>

<a name="img2threejs"></a>
### #&#8288;59 [img2threejs](https://github.com/img2threejs/img2threejs) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

**Agent skill that rebuilds an image's object as procedural Three.js code.**

img2threejs is a skill for Claude Code, Codex and OpenCode that takes one reference image and generates a TypeScript THREE.Group factory recreating the object from primitives, procedural shaders and generated geometry. It runs a staged pipeline from blockout to optimization, with vision review and Python gate scripts, and outputs pivots, sockets and colliders for animation. A CLI installs it into detected agent hosts.

- **+** Output is code only: no mesh files or downloaded assets, so models are small and editable
- **+** Generated models include pivots, sockets and colliders for animation
- **+** Quality gates block generation until a detail inventory is complete
- **+** Live gallery with source for each demo model
- **−** Needs a host agent with vision (Claude Code, Codex or OpenCode); model cost is not stated
- **−** Single image cannot guarantee likeness; unseen areas are low-confidence
- **−** Several gallery demos are still marked placeholder rather than final
- **−** Requires Node.js 18+, Git and Python 3.10+; plugins need a separate CLI

<sub>no GPU · Needs Node.js >= 18, Git, Python >= 3.10, Three.js, Claude Code, Codex or OpenCode · Models: Claude Code, Codex, OpenCode, Hermes · safety checks passed 9 of 9 · [Repo](https://github.com/img2threejs/img2threejs) · [▶️ Demo ↗](https://img2threejs.io/) · [🌐 Site ↗](https://img2threejs.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/img2threejs/)</sub>

<a name="auto-claude-code-research-in-sleep"></a>
### #&#8288;60 [auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**Skill-based research workflow for Claude Code with cross-model review.**

ARIS is a set of 82 skills that run an autonomous research workflow (idea discovery, experiments, paper writing) inside Claude Code, Codex CLI, Cursor and similar agents. An executor model drives the work while an independent reviewer, Codex through an MCP bridge over `codex exec` by default, critiques it. It also ships as a Claude Code and Codex plugin and as a standalone Rust CLI, ARIS-Code.

- **+** Works across Claude Code, Codex CLI, Cursor, Trae, Copilot CLI and OpenClaw
- **+** Separate reviewer model checks the executor's output; alternative model combinations are documented
- **+** Ships as plain skills, plugins, or a standalone CLI with prebuilt releases
- **+** MIT licensed, with frequent releases (ARIS-Code v0.4.28 on 2026-09-28)
- **−** Default reviewer depends on codex-cli; its MCP entry point was removed in 0.154
- **−** Aimed at research and paper workflows, not general application coding
- **−** Large surface (82 skills, many helpers) and a changelog-heavy README
- **−** Per-host adaptations live in separate docs, so support varies by agent

<sub>Needs Claude Code or another supported agent host, codex-cli (default reviewer), Python · Models: Claude Opus 5, Claude Fable 5.1, GPT-6-Astra, ModelScope-hosted models, DeepSeek · [Repo](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) · [📖 Docs ↗](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep/blob/main/AGENT_GUIDE.md) · [🌐 Site ↗](https://wanshuiyin.github.io/Auto-claude-code-research-in-sleep/ARIS_INTRO.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auto-claude-code-research-in-sleep/)</sub>

<a name="superpowers-zh"></a>
### #&#8288;61 [superpowers-zh](https://github.com/jnmetacode/superpowers-zh) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (45) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.3k · MIT · Oct 2026</sub>

**Chinese translation of the superpowers skills set for AI coding tools.**

Installs 21 skills (brainstorming, TDD, systematic debugging, code review, parallel agents) into 26 AI coding tools, including Claude Code, Cursor, Codex CLI, Gemini CLI and Windsurf. 15 are translations of upstream superpowers, 4 are manually invoked China-specific skills, and 2 are kept from upstream history. Installed with `npx superpowers-zh`, which detects the tool in use.

- **+** One `npx superpowers-zh` command detects the tool and installs skills, project or global scope
- **+** Covers 26 tools versus 6 in the English upstream
- **+** Also ships as a Claude Code plugin marketplace entry with hooks and bootstrap files
- **+** Adds Gitee, Coding, GitLab CN and CNB workflow skills; upstream sections are translated, not altered
- **−** Skills and docs are in Chinese; English readers should use the upstream project
- **−** The four China-specific skills load only when invoked manually, e.g. `/chinese-code-review`
- **−** Manual `cp -r skills` install skips hooks and bootstrap, so skills do not auto-trigger
- **−** README is crowded with sponsor banners and promo links

<sub>no GPU · Needs Node.js (npx), An AI coding tool such as Claude Code or Cursor · [Repo](https://github.com/jnmetacode/superpowers-zh) · [🌐 Site ↗](https://sp.aiolaola.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superpowers-zh/)</sub>

<a name="tech-leads-club-agent-skills"></a>
### #&#8288;62 [agent-skills](https://github.com/tech-leads-club/agent-skills) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · custom license · Oct 2026</sub>

**Curated skill registry and CLI installer for AI coding agents.**

A catalog of SKILL.md-based skills (spec-driven planning, AWS advice, Playwright automation, Figma to code, security review) with an npx CLI that installs them into agents such as Claude Code, Cursor, Copilot, Windsurf and Cline. Skills are fetched from a CDN, cached in ~/.cache/agent-skills, and tracked with a lockfile and audit log. A companion MCP server exposes search and read tools for the catalog.

- **+** Installs to about 20 agents from one interactive or scripted CLI, copy or symlink
- **+** Skills scanned with Snyk Agent Scan; lockfile, content hashing and audit log
- **+** Optional MCP server with search_skills and read_skill for progressive loading
- **+** Global or project-local install, with offline cache of downloaded skills
- **−** Mixed licensing: MIT code, CC-BY-4.0 skills, third-party skills keep own licenses
- **−** Attribution to Tech Leads Club is required when using the skills
- **−** Skills are downloaded from a CDN, so first install needs network access
- **−** Requires Node 22 or newer

<sub>no GPU · Needs Node.js >=22, npm/npx · [Repo](https://github.com/tech-leads-club/agent-skills) · [🌐 Site ↗](https://agent-skills.techleads.club/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tech-leads-club-agent-skills/)</sub>

<a name="agency-agents"></a>
### #&#8288;63 [agency-agents](https://github.com/msitarzewski/agency-agents) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 160k · MIT · Oct 2026</sub>

**Markdown agent persona files for Claude Code, Cursor, Codex and other coding tools.**

A repository of role-specific agent definitions written as Markdown files and grouped into divisions such as engineering and design. Each file describes the agent's identity, workflow, code examples and success metrics. Shell scripts (convert.sh, install.sh) generate and install the files for Claude Code, Cursor, Copilot, Gemini CLI, OpenCode, Aider, Windsurf, Codex and others. A separate desktop app for macOS, Linux and Windows does the same install with a GUI.

- **+** Installs into 14+ tools via one script, with --division and --agent filters
- **+** Roster spans dozens of engineering roles, from SRE and RAG pipelines to Solidity
- **+** Plain Markdown files, easy to read, copy and adapt without running anything
- **+** Separate desktop app handles install and updates without a clone
- **−** Prompt files only; no runtime, orchestration or agent execution included
- **−** OpenCode registers only about 119 agents, so full installs get silently truncated
- **−** No tagged release; versioning relies on commit history
- **−** Effectiveness claims like 'battle-tested' are not backed by benchmarks in the README

<sub>no GPU · safety checks passed 9 of 9 · [Repo](https://github.com/msitarzewski/agency-agents) · [🌐 Site ↗](https://agencyagents.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents/)</sub>

<a name="loop-engineering"></a>
### #&#8288;64 [loop-engineering](https://github.com/cobusgreyling/loop-engineering) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Pattern library and CLI for running scheduled agent loops around a codebase.**

Loop Engineering is a library of documented patterns (daily triage, PR babysitter, CI sweeper, dependency sweeper, changelog drafter and others) for running coding agents on a schedule against a repo. An npm CLI (@cobusgreyling/loop) scaffolds a pattern for Claude, Grok, Codex or Opencode, then offers doctor, status, audit and cost commands. Rollout is staged from L1 report-only to L3 unattended.

- **+** CLI scaffolds a pattern with init, then checks it with doctor, audit and cost
- **+** Eight documented patterns, each with cadence, week-one level and relative cost
- **+** Staged L1 to L3 rollout; week one is report-only
- **+** Examples for Claude Code, Grok, Codex, Opencode, OpenClaw and GitHub Actions
- **−** Mostly docs and templates; the agent itself comes from a separate tool
- **−** PR Babysitter and CI Sweeper are rated high or very high cost
- **−** README warns unattended loops can ship mistakes and token costs can explode
- **−** Related features live in separate companion repos

<sub>no GPU · Needs Node.js (npx), GitHub, A coding agent CLI (Claude Code, Grok, Codex or Opencode) · Models: Claude Code, Grok, Codex, Opencode, OpenClaw · [Repo](https://github.com/cobusgreyling/loop-engineering) · [📖 Docs ↗](https://github.com/cobusgreyling/loop-engineering/blob/main/docs/QUICKSTART.md) · [🌐 Site ↗](https://cobusgreyling.github.io/loop-engineering/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loop-engineering/)</sub>

<a name="gentle-ai"></a>
### #&#8288;65 [gentle-ai](https://github.com/gentleman-programming/gentle-ai) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Oct 2026</sub>

**Go installer adding memory, workflow and review rules to 17 coding agents.**

Gentle-AI is a Go CLI that configures coding agents you already have (Claude Code, Codex, OpenCode, Cursor, Pi and 12 more) with persistent memory (Engram), skills, optional Context7 MCP and a credential-file deny-list. It adds two workflows: ODD, which sizes work and decides when to delegate to subagents, and RDD, where the binary freezes a change and sets review depth by risk. Configs are snapshotted before each write.

- **+** Configures 17 agents using each agent's native configuration
- **+** Config backups before every write, plus a read-only `gentle-ai doctor` check
- **+** Review transitions come from the binary and on-disk state, not model judgment
- **+** Security deny-list blocks ~/.ssh, .env and credential files
- **−** Does not install an agent; requires one already set up
- **−** Delegation and RDD review features differ per agent
- **−** Benchmarks are single runs (n=1) on the authors' own suite
- **−** Windows install is a Go source build needing Go 1.25.10+

<sub>no GPU · Needs An existing supported AI coding agent, Go 1.25.10+ (Windows source install), Engram, Context7 MCP (optional) · [Repo](https://github.com/gentleman-programming/gentle-ai) · [📖 Docs ↗](https://github.com/Gentleman-Programming/gentle-ai/blob/main/docs/intended-usage.md) · [🌐 Site ↗](https://gentlemanprogramming.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gentle-ai/)</sub>

<a name="memu"></a>
### #&#8288;66 [memu](https://github.com/nevamind-ai/memu) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (60) · Freshness: active (98) · Maintenance: fair (72) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

**Shared memory and skill store for coding agents across sessions and devices.**

memU runs as a sidecar to desktop coding agents (Codex, Claude Code, Cursor, OpenClaw, Hermes, WorkBuddy, Cola, pi). A scheduled task reads session logs, the agent distills them into Markdown memory and skills, and memU embeds and stores them. A standing instruction in the host's instruction file makes the agent run a retrieve command before answering. It can use MemU Cloud or a local SQLite or Postgres store.

- **+** Per-host adapters for Codex, Claude Code, Cursor, OpenClaw, Hermes and others, plus generic memu-agent detect
- **+** Local storage options: SQLite for a single writer, Postgres with pgvector for concurrent access
- **+** Core service makes no LLM calls; the agent writes the skill Markdown, which stays readable
- **+** Embedding providers: OpenAI, Jina, Voyage, Doubao, OpenRouter
- **−** Chat-only modes of ChatGPT and Claude are not supported for memorize or retrieve
- **−** Self-hosted mode needs an embedding provider API key
- **−** Setup is done by an agent following a SKILL.md, which can fail on some models
- **−** SQLite backend uses brute-force cosine search and allows a single writer

<sub>no GPU · Needs Python 3.11+, Embedding provider API key (self-hosted), SQLite or Postgres with pgvector, MemU Cloud (optional) · Models: OpenAI embeddings, Jina, Voyage, Doubao, OpenRouter · [Repo](https://github.com/nevamind-ai/memu) · [🌐 Site ↗](https://memu.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/memu/)</sub>

<a name="obsidian-mind"></a>
### #&#8288;67 [obsidian-mind](https://github.com/breferrari/obsidian-mind) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT · Oct 2026</sub>

**Obsidian vault template giving coding agents persistent memory across sessions.**

An Obsidian vault with hooks, slash commands and an AGENTS.md manual that let Claude Code, Codex CLI or Gemini CLI keep notes, links, decisions and brag-doc entries between sessions. Lifecycle hooks inject goals, active projects and recent changes at session start and validate markdown writes. Optional QMD adds local semantic search through an MCP server; without it the agent falls back to grep and the Obsidian CLI.

- **+** Same hooks, commands and vault work with Claude Code, Codex CLI and Gemini CLI
- **+** Memory is git-tracked markdown in brain/, browsable in Obsidian and portable across machines
- **+** QMD search runs three local models, so no API key or per-query cost
- **+** Context injection has a byte budget and a size meter reported every session
- **−** Claude Code has full support; Codex and Gemini have known gaps, and Codex needs hook approval
- **−** Requires Obsidian 1.12+ and Node 22+; hooks use the experimental strip-types flag
- **−** QMD model downloads total about 2.2GB; queries with embedding take a couple of seconds
- **−** Claude Code mod is unsandboxed code that runs with your permissions once trusted

<sub>GPU optional · Needs Obsidian 1.12+, Node 22+, Git, QMD (optional), ShardMind (optional installer) · Models: Claude Code, Codex CLI, Gemini CLI, embeddinggemma-300M, qmd-query-expansion-1.7B · [Repo](https://github.com/breferrari/obsidian-mind) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/obsidian-mind/)</sub>

<a name="aidlc-workflows"></a>
### #&#8288;68 [aidlc-workflows](https://github.com/awslabs/aidlc-workflows) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.3k · MIT-0 · Oct 2026</sub>

**Approval-gated delivery workflows for AI coding assistants.**

AI-DLC installs a harness-neutral workflow engine into Claude Code, Kiro CLI and IDE, Codex CLI, Cursor, opencode and GitHub Copilot. A single /aidlc command picks one of 11 workflow profiles, runs 33 stages across 5 phases with 14 agents, and stops at human approval gates. State, a 119-event audit trail and learned rules persist per project.

- **+** Same engine across seven harnesses, configured with `aidlc config --harness`
- **+** Human approval gates and a 119-event audit trail
- **+** 11 workflow profiles, including bug fix, infrastructure, security and proof of concept
- **+** Native installer; Bun and Node.js not needed for normal install
- **−** Needs a separate harness and model provider; AI-DLC supplies neither
- **−** Install is a curl-to-shell script; manual path requires Bun
- **−** Large surface (33 stages, 14 agents, 93 tools) means a learning curve
- **−** Recommended model is Claude Opus 4.8; quality on other models unknown

<sub>no GPU · Needs Claude Code, Kiro, Codex CLI, Cursor, opencode or GitHub Copilot, Bun (manual-copy install only), Amazon Bedrock (optional) · Models: Claude Opus 4.8 (recommended), Amazon Bedrock, Provider set by harness · [Repo](https://github.com/awslabs/aidlc-workflows) · [📖 Docs ↗](https://github.com/awslabs/aidlc-workflows/blob/main/docs/guide/01-getting-started.md) · [🌐 Site ↗](https://awslabs.github.io/aidlc-workflows/roadmap.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aidlc-workflows/)</sub>

<a name="oh-my-hermes"></a>
### #&#8288;69 [oh-my-hermes](https://github.com/rlaope/oh-my-hermes) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Plugin layer for Hermes Agent adding model routing, parallel coding lanes and memory.**

oh-my-hermes (OMH) installs as a plugin and CLI over Nous Research's Hermes Agent. It scores each request and routes it to one of twelve editable model-and-effort categories, splits work into parallel git worktree units, and loads 108 specialist omh-* skills. It also adds a reviewed, file-backed long-term memory and its own TUI (bare `omh`).

- **+** Twelve editable model-and-effort chains with fallback when a provider rejects a model
- **+** Parallel units get separate worktrees from one pinned SHA, with typed evidence states
- **+** Memory entries need review and carry provenance and review-due dates
- **+** Installs via curl script, Homebrew, Bun or npm, with `omh doctor` and `omh update`
- **−** Requires an existing Hermes Agent install; not usable standalone
- **−** OMH TUI unavailable on Windows; falls back to Hermes' own TUI
- **−** Cost and speed figures come from the README's own GPT-6 Astra benchmark
- **−** Default install pipes a remote script to sh; setup needs an interactive model interview

<sub>Needs Hermes Agent, Node (for OMH TUI) · Models: Claude, Gemini, Qwen3-Coder, DeepSeek, GPT-6 Astra · [Repo](https://github.com/rlaope/oh-my-hermes) · [📖 Docs ↗](https://github.com/rlaope/oh-my-hermes/blob/main/docs/README.md) · [🌐 Site ↗](https://rlaope.github.io/oh-my-hermes/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-hermes/)</sub>

<a name="trellis"></a>
### #&#8288;70 [trellis](https://github.com/mindfold-ai/trellis) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · AGPL-3.0 · Sep 2026</sub>

**CLI that stores specs, tasks and session memory in your repo for coding agents.**

Trellis is an npm CLI that writes a `.trellis/` directory into your repo holding specs, task PRDs and per-developer journals, then injects the relevant context into coding agent sessions. It runs a four-phase loop (plan, implement, verify, finish) using skills and sub-agents, and generates platform-specific files for 22 AI coding platforms.

- **+** Specs, tasks and journals are plain files in the repo, reviewable like code
- **+** Same .trellis structure generated for 22 coding platforms, not just Claude Code
- **+** Verify step runs lint, type-check and tests against specs and self-fixes
- **+** Per-developer journals stay separate while shared specs live in git
- **−** AGPL-3.0 license may be a problem for some company use
- **−** Requires both Node.js >= 18 and Python >= 3.9
- **−** Needs upfront effort to write or draft specs to get value
- **−** No tagged release listed; versions only via npm

<sub>no GPU · Needs Node.js >= 18, Python >= 3.9 · [Repo](https://github.com/mindfold-ai/trellis) · [📖 Docs ↗](https://docs.trytrellis.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trellis/)</sub>

<a name="universal-modder"></a>
### #&#8288;71 [universal-modder](https://github.com/rehan-remade/universal-modder) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · MIT · Oct 2026</sub>

**Skills, CLI and field-note knowledge base for AI agents modding PC games.**

Packages Agent Skills, subagent role files, a Python `um` CLI and the fal MCP server so a coding agent can scan an installed game, pick a modding route, build a mod, generate assets with fal, test and record it. Installs as a plugin for Claude Code, Codex, Gemini CLI, Copilot, Cursor and OpenCode. A `knowledge/` folder holds per-game field notes that agents contribute by pull request.

- **+** Installs as a plugin or skills-only for six agents, including Claude Code, Codex and Cursor
- **+** `um scan` fingerprints engine, anti-cheat, loaders and save folders for Steam, Epic and Xbox installs
- **+** Engine playbooks cover Unity, Unreal, Godot, Source, Minecraft, .NET/XNA and more
- **+** Safety rules: save backups, PID-only kills, `um publish check` blocks shipping game files
- **−** Asset generation depends on a fal API key; the alternative is a local ComfyUI server for images only
- **−** Recording and input driving (`um win`) are Windows-specific tools
- **−** The mod hub is listed as coming next and is not yet available
- **−** Three-agent orchestrator team uses several times the tokens of a single agent

<sub>GPU optional · Needs Git, Python 3.10+, ffmpeg, fal API key, uv (recommended), Blender (3D to sprite renders), ComfyUI (optional) · Models: Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor · [Repo](https://github.com/rehan-remade/universal-modder) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/universal-modder/)</sub>

<a name="agentskills"></a>
### #&#8288;72 [agentskills](https://github.com/agentskills/agentskills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Aug 2026</sub>

**Open specification for SKILL.md folders that give AI agents reusable instructions.**

Defines the Agent Skills format: a folder with a SKILL.md file holding name and description metadata plus instructions, and optional scripts, references and assets. Agents load skills in three stages (discovery, activation, execution), so only names and descriptions sit in context until a task matches. Originally developed by Anthropic and released as an open standard; the repo holds the spec and docs, not a runtime.

- **+** Minimal format: one SKILL.md with name and description is enough
- **+** Progressive disclosure keeps context small with many skills installed
- **+** Skills can bundle scripts, references and templates in one version-controlled folder
- **+** Supported by multiple agent clients, listed in a client showcase
- **−** Specification and docs only; it is not an agent or runtime
- **−** Behavior depends on how each client implements skill loading
- **−** No tagged releases; versioning of the spec is not stated in the README
- **−** Skill quality and security of bundled scripts are left to authors

<sub>no GPU · safety checks passed 6 of 7 · [Repo](https://github.com/agentskills/agentskills) · [📖 Docs ↗](https://agentskills.io/specification) · [🌐 Site ↗](https://agentskills.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentskills/)</sub>

<a name="anatomy"></a>
### #&#8288;73 [anatomy](https://github.com/wheresryan22/anatomy) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

**Agent skill that builds interactive isometric figures to explain technical ideas.**

Anatomy is an Agent Skill for Claude Code, OpenCode, Codex and Antigravity. Given a concept, it invents a physical object whose behaviour models the idea and builds it as an interactive isometric figure in SVG, SVG plus WebGL, or beta 3D. Output is standalone HTML, a lone SVG, or React/Next.js components, with a zero-dependency Node kit and geometry audit scripts.

- **+** Installs with one `npx skills add` command across four agents; no API keys needed
- **+** Kit uses only Node built-ins; React is needed only for the React components
- **+** Includes geometry audit and headless Chrome capture scripts to verify figures
- **+** Ships nine built examples, including React components copyable into a site
- **−** Verification needs headless Chrome, which the Codex sandbox may block without config changes
- **−** 3D mode is marked beta and only re-renders the moving parts
- **−** Raptor engine example build takes a few minutes; 3D audit is slow
- **−** Repository is about 10 MB because the CLI copies examples too

<sub>no GPU · Needs Node.js >= 20.10, headless Chrome (for verification) · Models: Claude Code, OpenCode, Codex, Antigravity · [Repo](https://github.com/wheresryan22/anatomy) · [🌐 Site ↗](https://skills.wheresryan.sh/anatomy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/anatomy/)</sub>

<a name="codex-with-chatgpt"></a>
### #&#8288;74 [codex-with-chatgpt](https://github.com/xiaoduoya/codex-with-chatgpt) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.4k · MIT · Oct 2026</sub>

**Codex skill that uses ChatGPT web as planner and reviewer via read-only MCP.**

A Codex Skill plus a local Node.js bridge that lets the ChatGPT web app plan and review work while Codex executes edits, tests and git commands. ChatGPT reads the workspace through a loopback, OAuth 2.1-protected, read-only MCP server with 10 tools, exposed via a Cloudflare tunnel. This uses a ChatGPT subscription's web quota instead of API tokens.

- **+** Read-only MCP tools only; no write, delete or shell tools exist on the server
- **+** Sensitive files (.env*, keys, SSH) denied by default; .c2cignore adds custom rules
- **+** OAuth 2.1 with PKCE, one-time pairing code (5-minute TTL), tokens bound to one workspace
- **+** ChatGPT reviews the real git diff and test records rather than trusting Codex's claims
- **−** Requires a ChatGPT subscription and driving the ChatGPT web UI through Computer Use
- **−** Default Cloudflare quick-tunnel URL changes on restart, forcing connector re-creation
- **−** Stable hostname needs a Cloudflare account and a domain on Cloudflare
- **−** Unofficial and marked V1; depends on ChatGPT connector and web UI behavior

<sub>no GPU · Needs Node.js >= 20, git, cloudflared, pnpm, ChatGPT Plus/Pro account, Codex · Models: ChatGPT web (Plus/Pro), Codex · [Repo](https://github.com/xiaoduoya/codex-with-chatgpt) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-with-chatgpt/)</sub>

<a name="loopx"></a>
### #&#8288;75 [loopx](https://github.com/loopx-project/loopx) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · Apache-2.0 · Oct 2026</sub>

**Local control plane that keeps goals and evidence for long-running coding agents.**

LoopX installs as a skill for Codex, Claude Code and DeepSeek Harness. It stores goals, Todos, decisions and evidence outside the chat session, so an agent can continue across runs through a heartbeat or loop driver and ask the owner when a gate is hit. It includes a local browser/PWA dashboard (`loopx dashboard`) and a CLI (`loopx status`, `loopx doctor`).

- **+** Works with Codex, Claude Code and DeepSeek Harness without replacing their runtime
- **+** Goal state, decisions and evidence persist across sessions and restarts
- **+** Local-first dashboard shows what is running, waiting on you, or scheduled
- **+** Publishes LHTB results: 0.4948 mean reward vs 0.4218 for plain Codex on 46 tasks
- **−** LHTB uses one trial per task and unequal budgets; not an isolated causal estimate
- **−** Strict pass rate (7/46) matches plain Codex; the gain is mostly partial credit
- **−** Needs Python 3.11+ and Node.js 22.22.3+ installed
- **−** Desktop App is ad-hoc signed, not notarized; Windows preview updates are manual

<sub>Needs Python 3.11+, Node.js 22.22.3+, Codex, Claude Code or DeepSeek Harness · Models: Codex, Claude Code, DeepSeek Harness, direct-model sessions · [Repo](https://github.com/loopx-project/loopx) · [📖 Docs ↗](https://loopx-project.github.io/loopx/docs/) · [🌐 Site ↗](https://loopx-project.github.io/loopx/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loopx/)</sub>

<a name="mirrord"></a>
### #&#8288;76 [mirrord](https://github.com/metalbear-co/mirrord) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

**Run a local process against a live Kubernetes pod's traffic, files and env.**

mirrord runs a process on your machine while routing its network traffic, file access and environment variables through a target pod in a Kubernetes cluster. It launches a helper pod on the target's node and mirrors incoming traffic to the local process. It ships as a CLI, a VS Code extension and an IntelliJ plugin, and the README says it can be used with agents such as Claude Code, Cursor and Codex.

- **+** Test local code against real cluster services without a deploy
- **+** CLI, VS Code extension and IntelliJ plugin all available
- **+** Uses the default kubeconfig, no cluster-side install mentioned for basic use
- **+** Written in Rust, MIT licensed, with frequent releases
- **−** Helper pod needs Linux capabilities such as CAP_SYS_ADMIN and CAP_NET_ADMIN
- **−** Database branching, queue splitting and preview environments need the paid Teams tier
- **−** Requires access to a Kubernetes cluster; not usable standalone
- **−** Not an AI tool itself; agent support is via external skills repo

<sub>no GPU · Needs Kubernetes cluster, kubeconfig · [Repo](https://github.com/metalbear-co/mirrord) · [📖 Docs ↗](https://metalbear.com/mirrord/docs/overview/introduction/) · [🌐 Site ↗](https://metalbear.com/mirrord/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mirrord/)</sub>

<a name="lean-ctx"></a>
### #&#8288;77 [lean-ctx](https://github.com/yvgude/lean-ctx) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Oct 2026</sub>

**Local MCP server and shell hook that trim context fed to coding agents.**

LeanCTX sits between AI coding tools and the files and command output they read. It exposes ctx_* MCP tools with 16 file read modes, compresses shell output with 85+ patterns, and keeps local session memory, with an optional proxy for model requests. It is written in Rust and set up per agent with `lean-ctx wrap cursor|claude|codex`.

- **+** 16 read modes incl. map, signatures, diff, line ranges; cached re-reads return compact references
- **+** Tree-sitter parsing for 27 languages and 85+ shell-output compression patterns
- **+** Local savings ledger and dashboard; shadow mode estimates savings against an uncompressed baseline
- **+** Install via curl, brew, npm or cargo; wrap and unwrap are reversible
- **−** Mixed license; enterprise controls and SDK fall under separate terms
- **−** Shadow Mode savings are simulated, not measured against a second run
- **−** Claude Pro/Max OAuth cannot use the proxy; wire-level compression needs an API key
- **−** Addons, snapshots, packages and multi-agent handoff are labeled experimental

<sub>no GPU · Models: Claude Code, Cursor, Codex, Anthropic API (proxy) · [Repo](https://github.com/yvgude/lean-ctx) · [📖 Docs ↗](https://leanctx.com/docs/getting-started) · [🌐 Site ↗](https://leanctx.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lean-ctx/)</sub>

<a name="huashu-design"></a>
### #&#8288;78 [huashu-design](https://github.com/alchaincyf/huashu-design) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Oct 2026</sub>

**Agent skill that turns prompts into HTML prototypes, decks, animations and infographics.**

A skill for Claude Code, Cursor, Codex and other skills-compatible agents, installed with `npx skills add alchaincyf/huashu-design`. It produces single-file HTML prototypes, HTML slide decks exportable to editable PPTX, timeline animations exported as MP4/GIF, infographics and 5-dimension design reviews. It adds a brand-asset protocol and a library of 60 HTML-native styles.

- **+** Works across skills-compatible agents: Claude Code, Cursor, Codex, OpenClaw, Hermes
- **+** Exports HTML decks to PPTX with real editable text boxes via html2pptx.js
- **+** Core render and export pipeline runs locally; cloud features are optional, in scripts/cloud/
- **+** Brand protocol extracts colors from official assets and writes brand-spec.md
- **−** Output is HTML; no layer-level export to Figma or Keynote
- **−** 3D, physics and particle animation are out of scope
- **−** README says quality drops to 60-65 of 100 with no brand context
- **−** skills CLI 1.5.15 and older installs only SKILL.md, missing subdirectories

<sub>no GPU · Needs Node.js, Playwright, ffmpeg, Python · Models: Claude Code, Cursor, Codex, OpenClaw, Hermes · [Repo](https://github.com/alchaincyf/huashu-design) · [▶️ Demo ↗](https://www.huasheng.ai/parrots/) · [🌐 Site ↗](https://www.huasheng.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huashu-design/)</sub>

<a name="superclaude-framework"></a>
### #&#8288;79 [superclaude_framework](https://github.com/superclaude-org/superclaude_framework) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (70) · Freshness: active (98) · Maintenance: patchy (32) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Sep 2026</sub>

**Slash commands, agents and modes that add structure to Claude Code.**

SuperClaude is a Python package that installs 30 `/sc:*` slash commands into Claude Code, along with 20 agent personas and 7 behavioral modes, all delivered as instruction files. It can also install 8 optional MCP servers (Tavily, Context7, Serena, Playwright and others) with `superclaude mcp`. Install is via pipx or an install script; a TypeScript plugin system is planned for v5.0 and is not available yet.

- **+** Installs with `pipx install superclaude` and `superclaude install`; `superclaude doctor` verifies it
- **+** 30 slash commands cover brainstorming, implementation, testing, git, research and session save/load
- **+** MCP servers are optional; the framework works without them
- **+** MIT licensed, with docs for commands, agents, modes and flags
- **−** Targets Claude Code only; separate sibling projects exist for Gemini and Qwen
- **−** Claimed 2-3x speed and 30-50% token savings with MCPs come with no benchmark details
- **−** Plugin marketplace install is not available yet; v5.0 has no ETA
- **−** README mixes v4.1, v4.2 and v4.3 notes, and the research examples are unclear

<sub>no GPU · Needs Claude Code, pipx, Tavily MCP (optional), Context7 MCP (optional), Serena MCP (optional), Playwright MCP (optional) · Models: Claude (via Claude Code) · safety checks passed 10 of 10 · [Repo](https://github.com/superclaude-org/superclaude_framework) · [🌐 Site ↗](https://superclaude.netlify.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superclaude-framework/)</sub>

<a name="agency-agents-zh"></a>
### #&#8288;80 [agency-agents-zh](https://github.com/jnmetacode/agency-agents-zh) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

**Chinese-language library of 277 role-based agent prompts for coding tools.**

Markdown agent definitions across 20 departments (executive, engineering, design, marketing, and others), each with a persona, workflow and deliverables. It is a Chinese community edition of msitarzewski/agency-agents: 213 translated roles plus China-market originals such as Xiaohongshu, Douyin, WeChat, Feishu and DingTalk. Shell scripts convert and install the files into 20 tools, including Claude Code, Cursor, Copilot, Codex CLI and Gemini CLI.

- **+** Install script targets 20 tools, including Claude Code, Cursor, Copilot, Codex CLI, Aider and Gemini CLI
- **+** Roles define persona, workflow and deliverables, not one-line prompts
- **+** Covers China-specific platforms and domains (Xiaohongshu, Douyin, WeChat, Feishu, DingTalk)
- **+** MIT license; files can be copied by hand into ~/.claude/agents/
- **−** Role content and docs are in Chinese; English is only linked to the upstream repo
- **−** Only Claude Code and Copilot install directly; other tools need convert.sh first
- **−** README counts disagree (277 total, 268 in gallery, 63 vs 64 originals)
- **−** README is dominated by sponsor and course promotion; quality of roles is unverified here

<sub>no GPU · Needs Bash, Node.js (only for agency-orchestrator) · Models: Claude Code, Cursor, GitHub Copilot, Codex CLI, Gemini CLI · safety checks passed 8 of 9 · [Repo](https://github.com/jnmetacode/agency-agents-zh) · [▶️ Demo ↗](https://ao.aiolaola.com/experts) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents-zh/)</sub>

<a name="jakubkrehel-skills"></a>
### #&#8288;81 [skills](https://github.com/jakubkrehel/skills) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.0k · MIT · Oct 2026</sub>

**Agent skills for reviewing and building UI, typography, color and accessibility.**

A set of 14 markdown agent skills for interface work: UI polish, typography, colors, WCAG 2.2 accessibility, layout and product copy. Some are user-invoked commands, such as reviewing a branch or PR for interface regressions, stress-testing a component in every state, or building UI from a Figma file or design image. Installed with `npx skills add` or as a Claude Code plugin.

- **+** Separate skills for accessibility, layout, writing, typography, color and UI, plus one combined review
- **+** User-invoked skills for PR review, component state pages, variants and Figma-to-UI
- **+** Two install paths: npx skills CLI and a Claude Code plugin marketplace
- **+** MIT licensed; skills are plain SKILL.md files you can read and edit
- **−** README does not list which agents besides Claude Code are supported
- **−** No tagged releases; versioning is unknown
- **−** Skills are prompts only, so results depend on the model running them
- **−** README does not document what the Figma skill needs, such as Figma access

<sub>no GPU · Needs npx skills CLI or Claude Code · [Repo](https://github.com/jakubkrehel/skills) · [🌐 Site ↗](https://interfaces.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jakubkrehel-skills/)</sub>

<a name="pxpipe"></a>
### #&#8288;82 [pxpipe](https://github.com/teamchong/pxpipe) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Oct 2026</sub>

**Local proxy that renders bulky LLM request context as PNGs to cut input tokens.**

pxpipe sits between Claude Code (or Codex, cursor-agent, and other clients) and the provider API. It rewrites the system prompt, tool docs and older history into dense PNG pages plus a bounded factsheet before the request leaves the machine. It handles Anthropic Messages, OpenAI Responses/Chat Completions and Google generateContent, and logs measured savings against a count_tokens counterfactual.

- **+** Savings measured per request against a count_tokens probe, logged to ~/.pxpipe/events.jsonl
- **+** Reported ~59-70% lower end-to-end bill on Claude Code traffic; SWE-bench Lite 10/10 both arms
- **+** Profitability gate leaves sparse prose and recent turns as text
- **+** Also offers offline PNG export, a library API and a dashboard on 127.0.0.1:47821
- **−** Lossy: exact 12-char hex recall 13/15 on Fable 5, 0/15 on Sol; misses are silent
- **−** No verbatim-risk guard yet; IDs and hashes must stay text
- **−** Default model scope is limited: Fable 5, Opus 5.5 and Gemini; others opt-in
- **−** SWE-bench Pro showed 14/19 vs 15/19 text; small samples, and the README says savings depend on workload

<sub>no GPU · Docker + Compose · Needs Node.js, Anthropic, OpenAI-compatible or Google API access · Models: claude-fable-5, claude-opus-5-5, claude-opus-5, Gemini 3.6/3.7 Flash, gpt-5.6-sol (opt-in) · port 47821 · [Repo](https://github.com/teamchong/pxpipe) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pxpipe/)</sub>

<a name="anti-slop"></a>
### #&#8288;83 [anti-slop](https://github.com/miqdadbadjuber/anti-slop) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Oct 2026</sub>

**Rulebook that stops coding agents shipping generic UI, filler copy and noisy comments.**

Anti Slop is a set of agent skills built around 38 mandatory rules in three tiers, plus a PASS/FAIL Delivery Gate report run before work ships. Six skills cover the core filter, UI, copywriting, accessibility, responsive layout and code comments. It filters output and does not prescribe colors, fonts or layouts; direction is expected from a user-written DESIGN.md.

- **+** Six separate skills, so an agent loads only the concerns a task needs
- **+** Installs via npx installer, skills.sh, or plugin commands for about ten agents
- **+** Two modes: guide while building, or audit existing work with a findings list
- **+** Single antislop.md file works as a paste-in filter for any chat window
- **−** Filter only: output stays plain without a DESIGN.md supplying direction
- **−** Does not update itself; each install route has its own update command
- **−** Effect is shown by screenshot comparisons, with no measured results in the README
- **−** Skills load at session start, so changes need a new session

<sub>no GPU · Needs Node.js (npx installer), An AI coding agent such as Claude Code, Codex, Cursor or Cline · [Repo](https://github.com/miqdadbadjuber/anti-slop) · [📖 Docs ↗](https://github.com/miqdadbadjuber/anti-slop/blob/main/GUIDE.md) · [🌐 Site ↗](https://skills.sh/miqdadbadjuber/anti-slop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/anti-slop/)</sub>

<a name="ag-kit"></a>
### #&#8288;84 [ag-kit](https://github.com/vudovn/ag-kit) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (44) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Aug 2026</sub>

**Rules, skills, agents and workflows for Google Antigravity projects.**

AG Kit installs an `.agents/` workspace into a project with 20 specialist agent roles, 47 skills, 13 slash-command workflows and 6 rules, plus a file-based memory directory. It registers a narrow PreToolUse hook that blocks root-filesystem deletion, drive formatting and raw-disk overwrites. Updates are merge-aware with backup and rollback, and a local Antigravity plugin bundle can be built.

- **+** Merge-aware `ag-kit update` with --dry-run, automatic backups and `ag-kit rollback`
- **+** Safety hook blocks destructive commands but allows cleanup like deleting dist/ or node_modules/
- **+** Components carry SemVer contracts, a manifest lock and a dependency graph to detect drift
- **+** Plugin bundle includes a SHA-256 content inventory (PLUGIN_CONTENTS.json)
- **−** Production support is limited to Google Antigravity; other tools are not guaranteed
- **−** Hook covers only high-confidence destructive patterns and does not replace permissions or sandboxing
- **−** Needs Node.js 22 for repo tooling and Python 3.10 for validators
- **−** Default MCP example contains YOUR_API_KEY placeholders, so the doctor warns until configured

<sub>no GPU · Docker · Needs Node.js 22+, Python 3.10+, Git, Google Antigravity · [Repo](https://github.com/vudovn/ag-kit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ag-kit/)</sub>

<a name="oracle"></a>
### #&#8288;85 [oracle](https://github.com/steipete/oracle) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Oct 2026</sub>

**CLI and MCP server that sends a prompt plus selected files to a second model.**

Oracle bundles a prompt with files you select (globs, directories, exclusions) and sends it to a model through a provider API or a signed-in ChatGPT or Gemini browser session. Results are stored as sessions under ~/.oracle/sessions and can be reattached, replayed or followed up. It also runs as an oracle-mcp stdio server and ships a skill so coding agents can ask for a second-model review.

- **+** Render mode prints the exact prompt and files without credentials or a model call
- **+** API mode supports OpenAI, Azure OpenAI, Anthropic, Gemini, xAI, OpenRouter and compatible endpoints
- **+** --models runs several models in one session with per-model usage, cost and partial failures
- **+** Dry run reports resolved files and token estimate; bundles carry line numbers for path:line citations
- **−** Requires Node.js 24 or newer
- **−** Browser mode depends on Chrome automation and a one-time login flow
- **−** Follow-ups work only for supported API or ChatGPT conversations
- **−** No Docker image or demo listed in the README

<sub>no GPU · Needs Node.js 24+, Chrome (browser mode), Provider API key (API mode) · Models: OpenAI, Azure OpenAI, Anthropic, Gemini, xAI · [Repo](https://github.com/steipete/oracle) · [📖 Docs ↗](https://askoracle.sh) · [🌐 Site ↗](https://askoracle.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oracle/)</sub>

<a name="design-md"></a>
### #&#8288;86 [design.md](https://github.com/google-labs-code/design.md) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Jul 2026</sub>

**Spec and CLI for describing a design system to coding agents.**

DESIGN.md defines a file format with YAML front matter for design tokens (colors, typography, rounded, spacing, components) and markdown prose for rationale. The TypeScript CLI, run with npx, lints files for broken token references and WCAG contrast, diffs two versions, and exports tokens to Tailwind v3/v4 and W3C DTCG. The format is at version alpha.

- **+** Lint output is structured JSON with a non-zero exit code on errors, usable in CI
- **+** Eleven lint rules cover broken refs, WCAG AA contrast, section order and typos
- **+** Exports to Tailwind v3 JSON, Tailwind v4 CSS @theme and W3C DTCG tokens
- **+** Also usable as a library via the @google/design.md/linter import
- **−** Format is marked alpha; the README warns the spec and schema will change
- **−** Only a fixed set of component properties is valid; others produce warnings
- **−** Sections must appear in a fixed order, otherwise the linter warns
- **−** Windows needs the designmd alias because of the .md bin name collision

<sub>no GPU · Needs Node.js, npm · safety checks passed 9 of 10 · [Repo](https://github.com/google-labs-code/design.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/design-md/)</sub>

<a name="claude-plugins-official"></a>
### #&#8288;87 [claude-plugins-official](https://github.com/anthropics/claude-plugins-official) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · Apache-2.0 · Oct 2026</sub>

**Anthropic's curated plugin marketplace for Claude Code.**

A Git repository that acts as the official plugin marketplace for Claude Code. Plugins install with `/plugin install {plugin-name}@claude-plugins-official` or through `/plugin > Discover`. The repo holds Anthropic-maintained plugins in `/plugins` and partner or community plugins in `/external_plugins`, each bundling any of MCP server config, slash commands, agents and skills.

- **+** Installs directly from inside Claude Code with one slash command
- **+** Documents a standard plugin layout with an example plugin as reference
- **+** Plugin names are immutable slugs, with a renames map for migrations
- **+** Supports skill-bundle entries for repos that ship SKILL.md files without a manifest
- **−** Only useful with Claude Code; not a standalone tool
- **−** Anthropic does not control or verify third-party plugin contents, which can change
- **−** No single license; each plugin carries its own LICENSE file
- **−** No tagged releases; plugins are pinned only by marketplace entry

<sub>no GPU · Needs Claude Code · safety checks passed 7 of 10 · [Repo](https://github.com/anthropics/claude-plugins-official) · [📖 Docs ↗](https://code.claude.com/docs/en/plugins) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-plugins-official/)</sub>

<a name="brag"></a>
### #&#8288;88 [brag](https://github.com/latent-spaces/brag) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Oct 2026</sub>

**Agent skill that renders a launch video for your project.**

/brag is an agent skill for Claude Code, Codex, opencode and other Agent Skills hosts. It reads the current project, plans a story and tone, then hands a brief to Hyperframes to render a short launch video with music, motion and share copy. Output goes to a brag-output/ folder with the plan, composition brief, share copy and brag.mp4.

- **+** Installs as a Claude Code or Codex plugin, or via npx skills for other agents
- **+** Writes plan, composition brief, share copy and brag.mp4 to one folder
- **+** Tone steerable with --tone; optional Kokoro voiceover with --voice
- **+** Bundled music and sound effects, plus a leaner /brag-slim variant
- **−** Full workflow depends on the Hyperframes CLI, Node.js 22+ and FFmpeg
- **−** /brag-slim is built for Claude Opus 5.5; README does not cover other models
- **−** Voiceover is off by default and needs an explicit flag
- **−** No tagged releases; README gives no render time or output spec

<sub>Needs Node.js 22+, FFmpeg, Hyperframes CLI · Models: Claude Opus 5.5 (/brag-slim) · [Repo](https://github.com/latent-spaces/brag) · [▶️ Demo ↗](https://letsbrag.app) · [🌐 Site ↗](https://latent-spaces.github.io/brag/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/brag/)</sub>

<a name="softwarecopyright-skill"></a>
### #&#8288;89 [softwarecopyright-skill](https://github.com/fokkyp/softwarecopyright-skill) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Sep 2026</sub>

**Agent skill that drafts Chinese software copyright filing documents from your code.**

A skill directory for coding agents that analyzes a real project and produces materials for Chinese software copyright registration: an application-form TXT, an operation manual DOCX, and front 30 / back 30 page source code DOCX files. Code is extracted from the existing repository, not generated. DOCX output is built through a globally installed OfficeCLI 1.0.151, and the agent pauses for confirmation at each stage.

- **+** Code pages are extracted from the real project; the README says the AI does not invent source
- **+** Applies the front 30 / back 30 page rule, and emits all code if under 60 pages
- **+** Runs locally and stops for user confirmation at business, form, code and screenshot steps
- **+** Includes a generated demo folder showing drafts and final files
- **−** Requires OfficeCLI pinned to 1.0.151; no fallback DOCX writer if it is missing
- **−** Exact page count needs Microsoft Word on Windows; otherwise check manually in Word or WPS
- **−** README and workflow are in Chinese only
- **−** DOCX files must be exported to PDF manually before upload to the registry

<sub>no GPU · Needs Python 3.10+, OfficeCLI 1.0.151, Skill-capable coding agent, Node.js 18+ and @playwright/cli 0.1.20 (optional, screenshots), Chrome (optional), Microsoft Word on Windows (optional) · [Repo](https://github.com/fokkyp/softwarecopyright-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/softwarecopyright-skill/)</sub>

<a name="peon-ping"></a>
### #&#8288;90 [peon-ping](https://github.com/peonping/peon-ping) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

**Plays game character voice lines and banners when AI coding agents finish or need input.**

peon-ping registers hooks and adapters for Claude Code, Codex, Cursor, Copilot, Gemini CLI, OpenCode and about a dozen other agents. It plays sound-pack voice lines (Warcraft, StarCraft, Portal and others) and shows overlay banners and terminal tab titles on events such as task complete, permission needed, error and rate limit. It ships a `peon` CLI, an MCP server, SSH relay and phone notifications via ntfy.

- **+** Adapters for 20+ agents and IDEs, plus any MCP client
- **+** Per-event sound categories following the open CESP pack spec
- **+** Per-directory and per-IDE pack bindings, path exclusions, and Focus/DND detection
- **+** Installs via Homebrew, shell script, PowerShell, or Nix with Home Manager module
- **−** Windows lacks some CLI commands such as setup, rotation, preview and mobile
- **−** WSL2 on Windows 11 24H2+ needs ffmpeg to play MP3 packs
- **−** Written in Shell; installer is piped from curl by default
- **−** Overlay banners listed only for macOS, WSL and MSYS2, not plain Linux

<sub>no GPU · Needs ffmpeg (WSL2 on Windows 11 24H2+, MP3 packs), ntfy (optional, phone notifications) · Models: Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI · [Repo](https://github.com/peonping/peon-ping) · [▶️ Demo ↗](https://peonping.com/) · [🌐 Site ↗](https://peonping.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/peon-ping/)</sub>

<a name="google-skills"></a>
### #&#8288;91 [skills](https://github.com/google/skills) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

**Agent Skills for Google Cloud, GKE, BigQuery, Ads and Firebase.**

A repository of Agent Skills (Markdown skill folders) for Google products, mostly Google Cloud: GKE, BigQuery, AlloyDB, Cloud Run, IAM, SecOps, Genkit and the Gemini APIs. Install with `npx skills add google/skills`, choosing skills, target agents and project or global scope. It also bundles plugins (skills plus MCP servers) for Claude Code, Codex and Antigravity CLI.

- **+** Broad coverage: over 150 skills across GKE, data, security, ads and AI/ML
- **+** Installable per skill, per agent and per scope via npx skills
- **+** Plugin bundles for Claude Code, Codex and Antigravity CLI
- **+** Apache-2.0 licensed, with an issue tracker for skill content fixes
- **−** Focused on Google products; little use outside Google Cloud, Ads or Firebase
- **−** Documented install path requires Node.js and npx
- **−** No tagged releases; installs track the repository head
- **−** Some skills are marked Public Preview, such as the API Gateway MCP server

<sub>no GPU · Needs Node.js (npx), Google Cloud account for most skills · safety checks passed 9 of 9 · [Repo](https://github.com/google/skills) · [🌐 Site ↗](https://skills.sh/google/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-skills/)</sub>

<a name="agent-skills-for-context-engineering"></a>
### #&#8288;92 [agent-skills-for-context-engineering](https://github.com/muratcankoylan/agent-skills-for-context-engineering) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**Collection of 18 Agent Skills on context and harness engineering for coding agents.**

A set of SKILL.md directories covering context fundamentals, compression, memory, tool design, multi-agent patterns, evaluation and harness design. It installs as a Claude Code plugin marketplace entry, an Open Plugins manifest for Cursor and Codex, or by copying single skill folders into .claude/skills, .cursor/skills or .codex/skills. Six worked examples and a router benchmark are included.

- **+** Installs via one /plugin command or by copying individual skill directories
- **+** Works across Claude Code, Cursor, Codex and other Open Plugins hosts
- **+** Skill router benchmarked: 600 calls per sweep across four models, with published results
- **+** Includes six worked examples, such as an LLM-as-judge TypeScript implementation with 19 tests
- **−** Skills are guidance text; scripts are Python pseudocode, not a runnable library
- **−** Router top-1 accuracy ranges 0.84 to 0.92 across tested models
- **−** Skill activation depends on the host agent's skill discovery
- **−** Some skills are labeled NEW and their maturity is unknown

<sub>no GPU · Needs Claude Code, Cursor, Codex or another Agent Skills host · Models: Model-agnostic; router benchmarked on gemini-3.1-pro, composer-2, gpt-5.5, claude-opus-4-7 · [Repo](https://github.com/muratcankoylan/agent-skills-for-context-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills-for-context-engineering/)</sub>

<a name="trailofbits-skills"></a>
### #&#8288;93 [skills](https://github.com/trailofbits/skills) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · CC-BY-SA-4.0 · Oct 2026</sub>

**Trail of Bits plugin marketplace of security and testing skills for Claude Code.**

A Claude Code plugin marketplace from Trail of Bits that bundles skills for security auditing, testing and development workflows. Plugins cover smart contract review, C/C++ and Rust review, Semgrep and CodeQL, fuzzing, mutation testing, constant-time analysis and YARA rules. Codex can load it through its Claude marketplace compatibility, and a ChatGPT workspace import uses the marketplace.json.

- **+** Installs with one command: /plugin marketplace add trailofbits/skills
- **+** Broad security coverage: smart contracts, C/C++, Rust, Semgrep, CodeQL, fuzzing, YARA
- **+** Also loads in Codex through its Claude marketplace compatibility
- **+** Includes a trophy case with a documented bug found in ML-DSA signing
- **−** CC-BY-SA-4.0 share-alike license may constrain reuse inside proprietary repos
- **−** Security focus; several plugins are unrelated to general coding (Tarot, Culture Index)
- **−** ChatGPT imports need extra interface fields in agents/openai.yaml
- **−** No tagged releases; versioning is by commit

<sub>no GPU · Needs Claude Code or Codex · [Repo](https://github.com/trailofbits/skills) · [🌐 Site ↗](https://www.trailofbits.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trailofbits-skills/)</sub>

<a name="n8n-skills"></a>
### #&#8288;94 [n8n-skills](https://github.com/czlonkowski/n8n-skills) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Oct 2026</sub>

**Claude Code skills and hooks for building n8n workflows through n8n-mcp.**

A pack of 14 SKILL.md skills plus an always-on router skill and hooks that guide Claude in building n8n workflows with the n8n-mcp server. Topics include expression syntax, Code node JavaScript and Python, validation errors, error handling, sub-workflows and AI agents. One skill covers deploying self-hosted n8n behind Caddy with Docker Compose.

- **+** Covers specific gotchas, such as webhook data under $json.body and Code Tool string returns
- **+** Hooks re-inject reminders on SessionStart, before get_node calls and after validate_workflow
- **+** Installs as a Claude Code plugin; skill zips also work on Claude.ai and other SKILL.md hosts
- **+** Includes a self-hosting skill with single and queue mode Docker Compose templates
- **−** Requires the separate n8n-mcp server to be installed and configured
- **−** Hooks only run in the Claude Code or Codex plugin install, not Claude.ai uploads
- **−** Self-hosting skill sits outside the workflow-building router and hooks flow
- **−** Test instructions are hedged ('if testing framework available'), so the eval setup is unclear

<sub>no GPU · Needs n8n-mcp, n8n, Claude Code · Models: Claude · [Repo](https://github.com/czlonkowski/n8n-skills) · [📖 Docs ↗](https://github.com/czlonkowski/n8n-skills/blob/main/docs/INSTALLATION.md) · [🌐 Site ↗](https://aiadvisors.pl/en) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/n8n-skills/)</sub>

<a name="agents-cli"></a>
### #&#8288;95 [agents-cli](https://github.com/google/agents-cli) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · Apache-2.0 · Oct 2026</sub>

**CLI and skills that teach coding agents to build and deploy ADK agents.**

agents-cli installs seven skills into coding agents such as Claude Code, Codex and Antigravity CLI. It also provides commands to scaffold ADK Python agent projects, run evals, and deploy to Agent Runtime, Cloud Run or GKE. The CLI also works standalone from a terminal, and local create, run and eval need only an AI Studio API key.

- **+** Covers the full lifecycle: scaffold, eval, deploy, publish and observability commands plus matching skills
- **+** Eval commands include synthesized multi-turn datasets, failure clustering and prompt auto-tuning
- **+** scaffold enhance adds deployment and CI/CD to existing agent projects
- **+** Local create, run and eval work with an AI Studio key, no Google Cloud needed
- **−** Targets ADK agents on Google Cloud and Gemini; other frameworks are not covered
- **−** Deployment and publish features require a Google Cloud project
- **−** Telemetry is on by default; opt out with AGENTS_CLI_TELEMETRY=0 or DO_NOT_TRACK=1
- **−** Requires Python 3.11+, uv and Node.js installed

<sub>no GPU · Needs Python 3.11+, uv, Node.js, Google Cloud (for deploy), AI Studio API key (for local runs) · Models: Gemini · [Repo](https://github.com/google/agents-cli) · [📖 Docs ↗](https://google.github.io/agents-cli/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents-cli/)</sub>

<a name="ccg-workflow"></a>
### #&#8288;96 [ccg-workflow](https://github.com/fengshao1227/ccg-workflow) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (30) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

**Multi-model workflow layer for Claude Code, delegating to Codex, Grok and Kimi.**

CCG installs slash commands, hooks, skills and a compiled Go bridge (codeagent-wrapper) into Claude Code. Claude stays the orchestrator and picks one of 10 strategies per task, sending analysis and review to external models such as Codex, Grok, Kimi Code and Antigravity. Hooks inject task state every turn so context survives compaction, and tasks persist under .ccg/tasks.

- **+** 10 built-in strategies, from direct-fix to full-collaborate with dual-model review
- **+** Hooks re-inject task state every turn and after context compaction
- **+** Skills install individually; doctor --json outputs a versioned health report
- **+** Native plugin option installs skills only, with no binary
- **−** Multi-model commands ship only via the npx install, not the native plugin
- **−** Requires Claude Code CLI; external models need their own CLIs installed
- **−** Installs a compiled Go binary into ~/.claude/bin as the model bridge
- **−** README mixes in sponsor blocks and unrelated projects

<sub>no GPU · Needs Node.js 20+, Claude Code CLI, Codex CLI (optional), Grok CLI (optional), Kimi Code CLI (optional), Antigravity (optional) · Models: Claude, Codex (OpenAI), Grok (xAI), Kimi Code (Moonshot), Antigravity · [Repo](https://github.com/fengshao1227/ccg-workflow) · [📖 Docs ↗](https://ccg.fengshao1227.com/) · [🌐 Site ↗](https://ccg.fengshao1227.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ccg-workflow/)</sub>

<a name="observal"></a>
### #&#8288;97 [observal](https://github.com/observal/observal) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

**Self-hosted registry and telemetry for internal coding agent skills, MCP servers and hooks.**

Observal is a server plus CLI that stores an organization's coding agent resources (agents, skills, MCP servers, hooks, prompts, sandboxes) in one reviewed registry. It generates per-harness config for Claude Code, Cursor, Kiro, Codex, Copilot, OpenCode and others, and captures session traces through installed telemetry hooks. It also publishes approved resources over ARD and lets agents delegate tasks over A2A.

- **+** One install command renders an agent into each supported harness's config format
- **+** Admin review, version diffs and forking of approved releases keep registry changes auditable
- **+** Session traces and usage data feed reports on which agents and tools get used
- **+** Implements ARD v0.91 discovery and A2A v1.0 delegation with team-private visibility rules
- **−** Needs a multi-service stack (API, web UI, Postgres, ClickHouse) on Docker Engine 24+ with Compose v2
- **−** Telemetry hooks are installed into each developer's harness via the CLI, adding a per-machine setup step
- **−** Value depends on an organization already having many internal agent resources to catalog
- **−** RAM and hardware requirements are not stated in the README

<sub>Docker + Compose · Needs Docker Engine 24+ with Compose v2, PostgreSQL, ClickHouse · Models: Claude Code, Cursor, Kiro, Codex, GitHub Copilot · [Repo](https://github.com/observal/observal) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/observal/)</sub>

<a name="skills-manager"></a>
### #&#8288;98 [skills-manager](https://github.com/xingkongliang/skills-manager) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Oct 2026</sub>

**Desktop app and CLI that manage agent skills across coding tools.**

Skills Manager keeps one central skill library (default ~/.skills-manager) and deploys skills to 54 supported agents, including Claude Code, Codex, Cursor and Gemini CLI, by symlink or copy. Skills install from Git, local folders, .zip/.skill archives or the skills.sh marketplace, and can be grouped into presets. A bundled CLI and a manage-skills skill let agents drive it too, and the library can be backed up to Git.

- **+** Deploys one library to 54 agents via symlink or copy, with per-agent toggles
- **+** Bundled CLI with --json output and --dry-run on deploy, undeploy, sync, remove and adopt
- **+** Git-backed backup with skill-aware merging, restorable snapshots and plain Git remote
- **+** Shows skills installed outside the app and tracks upstream updates for Git-based skills
- **−** Windows app can only copy skills into WSL; symlinks need the Linux CLI inside WSL
- **−** Applying a preset is a one-time copy, not a live sync
- **−** Skills over 100 MB are excluded from backup; secrets and machine wiring stay local
- **−** Desktop-only Tauri app; no web or server deployment described

<sub>no GPU · Needs Tauri 2, SQLite, Node.js 20.19+ or 22.12+ (build only), Rust 1.77.2+ (build only), Git (optional backup) · [Repo](https://github.com/xingkongliang/skills-manager) · [🌐 Site ↗](https://skillsmanager.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skills-manager/)</sub>

<a name="dotnet-skills"></a>
### #&#8288;99 [skills](https://github.com/dotnet/skills) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · MIT · Oct 2026</sub>

**.NET team's skills and plugins for Copilot, Claude Code, Cursor and Codex.**

Official .NET team marketplace of agent skills, grouped into 16 plugins covering MSBuild, NuGet, EF data access, testing, upgrades, ASP.NET Core, Blazor, MAUI, WinForms and .NET AI. It installs through the plugin marketplaces of Copilot CLI, Claude Code, VS Code, Cursor and Codex CLI. It also ships GitHub Copilot custom agents and GitHub Agentic Workflows.

- **+** Maintained by the .NET team, with 16 plugins split by area (MSBuild, NuGet, EF, Blazor, MAUI)
- **+** Installs via marketplace in Copilot CLI, Claude Code, VS Code, Cursor and Codex CLI
- **+** Public dashboard reports token use, elapsed time and activation rates per skill
- **+** Skills follow the agentskills.io open standard, so they port across hosts
- **−** Custom agents (*.agent.md) use Copilot conventions and are not installed as native Codex agents
- **−** VS Code plugin support is a preview feature and may change
- **−** No native Codex agent files (.codex/agents/*.toml) are shipped
- **−** Only useful for .NET work

<sub>no GPU · Needs Copilot CLI, Claude Code, VS Code, Cursor or Codex CLI (v0.121.0+ for plugin marketplace) · [Repo](https://github.com/dotnet/skills) · [📖 Docs ↗](https://agentskills.io) · [🌐 Site ↗](https://dotnet.github.io/skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dotnet-skills/)</sub>

<a name="cc-sdd"></a>
### #&#8288;100 [cc-sdd](https://github.com/gotalab/cc-sdd) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Sep 2026</sub>

**Spec-driven workflow skills for Claude Code, Codex, Cursor and other coding agents.**

cc-sdd installs a set of 17 Agent Skills into your project via npx. They cover discovery, requirements, design, tasks and implementation, in a style modeled on Kiro specs. With native subagents, /kiro-impl runs each task through a fresh implementer using TDD, then an independent reviewer. Hosts without subagents run the same flow inline.

- **+** Same 17-skill set across 8 agents, installed with one npx command
- **+** Specs (requirements.md, design.md, tasks.md) carry boundary and dependency annotations
- **+** Per-task TDD, independent review and auto-debug when native subagents exist
- **+** Templates and rules under the specs settings directory are editable; 14 languages supported
- **−** Only Claude Code and Codex are stable; the other agents are beta
- **−** README says installing the skills does not verify a host can run the full autonomous loop
- **−** Legacy /kiro:* command modes are deprecated, so v1/v2 users must migrate
- **−** Devin adapter has unverified authenticated task execution

<sub>no GPU · Needs Node.js and npx, a supported AI coding agent (Claude Code, Codex, Cursor, Copilot, etc.) · [Repo](https://github.com/gotalab/cc-sdd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-sdd/)</sub>

<a name="dashi-taskboard"></a>
### #&#8288;101 [dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Oct 2026</sub>

**Local issue board embedded in the Codex desktop app, with a CLI and Skill.**

Runs a Node.js HTTP service with a React issue board backed by SQLite, and injects it into the Codex desktop app as a sidebar panel over CDP. A bundled `taskctl` CLI and the `manage-taskboard` Skill let Codex tasks read issues, move them to in_progress and in_review, and record the conversation ID. Desktop packages exist for macOS, Windows and Ubuntu 24.04 x64, and an optional Cloudflare deployment uses Workers, D1 and R2.

- **+** Same HTTP API serves the React UI and the taskctl CLI used by the Skill
- **+** Skill moves issues to done only after explicit user confirmation
- **+** Single SQLite file at .data/taskboard.sqlite, no separate database server
- **+** Live updates to all open clients via server-sent events
- **−** Embedding relies on unauthenticated CDP and a CSP bypass, so only trusted local code should run
- **−** LAN mode has no account authentication; default bind is 0.0.0.0
- **−** Linux packages cover Ubuntu 24.04 x64 only; no ARM64, Fedora or RPM
- **−** Windows CI builds are unsigned and do not auto-update

<sub>no GPU · Needs Node.js 22.5+, Codex desktop app (ChatGPT.app), SQLite, Rust 1.88+ and Tauri (app builds only), Cloudflare Workers, D1, R2 (optional) · port 47823 · [Repo](https://github.com/chuspeeism/dashi-taskboard) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dashi-taskboard/)</sub>

<a name="dsh-routing-suite"></a>
### #&#8288;102 [dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (38) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · MIT · Sep 2026</sub>

**Plugins for the DSH agent: runtime injector, routing presets, graded task protocol.**

Bundles three add-ons for the DSH agent (@deepseek-ai/dsh): an injector that adds dev_* tools for hot-reload without restart, router-standard and router-spec presets that pick a reasoning persona per task type, and a graded two-level task protocol with a red-team gate and audit endpoint. Installed with dsh plugin add or install.ps1. Targets DSH >=0.1.0-rc.6 <0.2.0, a developer preview with announced breaking changes.

- **+** Three components in one repo, installable with a single dsh plugin add command
- **+** Includes measure.mjs to recompute the reported metrics on your own session logs
- **+** Experiment reports (P1-P23) and measured data are published alongside the presets
- **+** Presets replace only the persona section, so plan-mode boundaries are kept
- **−** Works only with DSH, a developer preview with announced breaking changes
- **−** Install steps and scripts are PowerShell; other platforms are not documented
- **−** Main README and docs are in Chinese, with a separate English README
- **−** router-pro preset is planned and not released

<sub>Needs DSH (@deepseek-ai/dsh) >=0.1.0-rc.6 <0.2.0, Node.js, PowerShell · Models: DeepSeek Pro, DeepSeek Flash · [Repo](https://github.com/yjh051108/dsh-routing-suite) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-routing-suite/)</sub>

<a name="autoresearch"></a>
### #&#8288;103 [autoresearch](https://github.com/uditgoenka/autoresearch) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Aug 2026</sub>

**Skill that runs coding agents in a measured keep-or-revert loop.**

Autoresearch is a skill pack for Claude Code, OpenCode and OpenAI Codex, based on Karpathy's autoresearch. Given a goal, a metric and a verify command, the agent makes one change per iteration, commits it, runs the check, and keeps or reverts the commit. It adds 14 subcommands (plan, debug, fix, security, ship, scenario, regression and others) and, for Claude Code only, hook guardrails.

- **+** Works with Claude Code, OpenCode and Codex; installs via npx skills, plugin or install.sh
- **+** Each iteration is a git commit with automatic revert on failure and a TSV results log
- **+** Every command has a default iteration bound; unlimited runs are opt-in
- **+** Claude Code hooks block force-push, rm -rf, .env reads and node_modules context bloat
- **−** Hook guardrails exist only for Claude Code, not OpenCode or Codex
- **−** Classic loop needs a verify command that outputs a number
- **−** README calls the hooks defense-in-depth, not a security sandbox
- **−** Autonomous commit and revert loop on your repo; token spend scales with iterations

<sub>no GPU · Needs Claude Code, OpenCode or OpenAI Codex, git · Models: Claude Code, OpenCode, OpenAI Codex · [Repo](https://github.com/uditgoenka/autoresearch) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autoresearch/)</sub>

<a name="avdlee-swiftui-agent-skill"></a>
### #&#8288;104 [swiftui-agent-skill](https://github.com/avdlee/swiftui-agent-skill) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**SwiftUI guidance skill for AI coding agents, with Instruments trace analysis.**

An Agent Skills package that gives coding agents SwiftUI reference guides covering state management, view composition, performance, navigation, Swift Charts, macOS scenes, Liquid Glass and SDK 27 changes. Reference files load on demand. It also ships Python scripts that wrap xctrace to record and analyse Instruments traces for hangs, hitches and SwiftUI view updates.

- **+** Reference files load on demand, so task context stays small
- **+** Bundled stdlib-only Python scripts record and analyse .trace files, emitting JSON and markdown
- **+** Installs via skills.sh, Claude Code, Codex and Cursor plugin manifests
- **+** Covers iOS 15 through iOS 27 API migration, plus macOS and Swift Charts
- **−** Trace tooling needs Xcode's xctrace, so it works only on macOS
- **−** Focused on correctness and performance, gives no architecture or code-style guidance
- **−** SwiftUI only; concurrency, Core Data and testing are separate skills
- **−** Several reference files have no description in the README listing

<sub>no GPU · Needs xctrace (Xcode), Python 3, Sosumi MCP (maintenance skill only) · [Repo](https://github.com/avdlee/swiftui-agent-skill) · [🌐 Site ↗](https://skills.sh/avdlee/swiftui-agent-skill/swiftui-expert-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/avdlee-swiftui-agent-skill/)</sub>

<a name="cc-skills-golang"></a>
### #&#8288;105 [cc-skills-golang](https://github.com/samber/cc-skills-golang) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

**Agent Skills that teach coding assistants idiomatic, production-grade Go.**

A collection of about 50 Agent Skills covering Go style, error handling, testing, security, concurrency, observability and performance, plus library skills for gRPC, cobra, viper, wire, fx and samber/*. Skills load on demand, so only short descriptions sit in context. Installs through the skills CLI, a Claude Code plugin, or by cloning into the skills directory of Codex, Gemini CLI, Cursor, Copilot, OpenCode and others.

- **+** Works with Claude Code, Codex, Gemini CLI, Cursor, Copilot, OpenCode and Antigravity
- **+** Lists per-skill token weights, so context cost is visible before installing
- **+** README reports 97% eval pass with skills versus 57% without, across 3,439 checks
- **+** Skills load on demand rather than all at once
- **−** Skills cross-reference each other; installing a subset gives inconsistent guidance
- **−** Go only; git, CI and PR workflow skills need a separate plugin
- **−** Eval results are the author's own benchmark
- **−** golang-temporal skill is still marked to-do

<sub>no GPU · Needs Node.js (npx skills CLI), gopls (golang-gopls skill), godig (golang-pkg-go-dev skill) · Models: Claude Code, Codex, Gemini CLI, Cursor, Copilot · [Repo](https://github.com/samber/cc-skills-golang) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-skills-golang/)</sub>

<a name="answer-me-with-html"></a>
### #&#8288;106 [answer-me-with-html](https://github.com/qingyuna/answer-me-with-html) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Agent skill that renders answers as one offline HTML page from Markdown.**

An agent skill with a bundled Node CLI (`am`). The model writes a short Markdown draft, and the CLI lays out panels, flow, sequence, ER and tree diagrams, tables and themes into a single HTML file. It can also build narrated explainer videos. It works with Claude Code, Codex, Cursor, OpenCode and others.

- **+** Model writes about 612 tokens vs 4,893 for hand-written HTML, per the README benchmark
- **+** Each page is one HTML file with no CDN links or web fonts, so it opens offline
- **+** On draft errors the CLI returns line number and a correct example for the agent to fix
- **+** Installs as a Claude Code plugin or via `npx skills add`; no npm install step
- **−** Always-on mode is off by default and needs a rule added to your rules file
- **−** MP4 video export needs ffmpeg
- **−** Pages accumulate in ~/.answer-me-with-html/ until you run `am clean`
- **−** Benchmark covers 3 topics on one model (Claude Sonnet 5.5); other setups unknown

<sub>no GPU · Needs Node.js 20+, ffmpeg (optional, for MP4) · Models: Claude Code, Codex, Cursor, OpenCode, Pi · [Repo](https://github.com/qingyuna/answer-me-with-html) · [📖 Docs ↗](https://github.com/QingYunA/answer-me-with-html/blob/main/docs/reference.md) · [🌐 Site ↗](https://answer-me-with-html.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/answer-me-with-html/)</sub>

<a name="autoharness"></a>
### #&#8288;107 [autoharness](https://github.com/tigerless-labs/autoharness) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

**Claude Code plugin that learns, merges and prunes its own skills from sessions.**

autoharness is a Claude Code plugin that distills skills from your real sessions into .claude/skills/, folds same-scenario skills together, and archives ones that stop being loaded. It only touches skills it wrote itself and injects a grouped index of them at session start. Reflection runs after a set number of tool calls (default 50), or on demand with /learn.

- **+** Touches only skills it generated; hand-written and installed skills are left alone
- **+** Each create/update logs reason and evidence slice to a per-skill ledger
- **+** Archives rather than deletes; moving a skill directory back revives it
- **+** Pure Python with zero third-party dependencies; tunable via AUTOHARNESS_* env variables
- **−** Requires python3 3.11+ on PATH; older interpreters turn the hooks off
- **−** Claude Code only; Linux and macOS only
- **−** README says default thresholds are placeholders pending empirical calibration
- **−** Background reflection spawns extra child sessions, adding token cost

<sub>no GPU · Needs Claude Code, Python 3.11+ · Models: Claude · [Repo](https://github.com/tigerless-labs/autoharness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autoharness/)</sub>

<a name="trail-code"></a>
### #&#8288;108 [trail-code](https://github.com/trailhq/trail-code) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

**Code graph and shared team learnings for Claude Code, Cursor and Codex.**

Trail-code (formerly graft) parses a repo with tree-sitter into a graph of files, functions and callers, and gives coding agents matching files and edit impact through hooks and MCP tools. It also saves decisions and preferences from sessions as markdown in .trail/learnings/, shared through git, and trail check compares a branch against them before a PR. The README reports 33 of 50 SWE-bench Verified issues solved with the map versus 27 without.

- **+** Code map built locally with tree-sitter, no model or API key, 23 languages
- **+** Learnings are plain markdown in git, reviewed in PRs, no server needed
- **+** trail check flags changes that contradict earlier team decisions before the PR
- **+** Claude Code wired via hooks; Cursor and Codex via MCP tools and instruction files
- **−** Benchmark figures are the project's own; the SWE-bench sample is only 50 issues
- **−** Team workspace, skills and guardrails kinds are marked as coming soon
- **−** Day-one session mining reads Claude Code transcripts only, using Claude Sonnet
- **−** Sends anonymous telemetry by default, opt-out

<sub>no GPU · Docker · Needs Node.js, git · Models: Claude Code, Cursor, Codex · [Repo](https://github.com/trailhq/trail-code) · [🌐 Site ↗](https://trailhq.com/graft) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trail-code/)</sub>

<a name="claude-code-local"></a>
### #&#8288;109 [claude-code-local](https://github.com/nicedreamzapp/claude-code-local) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Anthropic-API MLX server that runs Claude Code on local models on Apple Silicon.**

A Python server (proxy/server.py) runs open models with Apple MLX and answers Claude Code in the Anthropic Messages API format, with streaming. It converts Gemma, Qwen and Llama-style tool calls into Claude Code tool calls, repairs malformed tool JSON, and reuses the prompt cache between turns. setup.sh picks a model based on the Mac's memory and creates a Desktop launcher.

- **+** Speaks the Anthropic API directly, with no LiteLLM or OpenAI translation layer
- **+** setup.sh picks a model by RAM, from Hermes 4 14B at 16 GB to Qwen 3.8 27B at 96 GB
- **+** Launchers disable Claude Code's background traffic; README shows an lsof check for network connections
- **+** Includes tool-call parser tests and a benchmark script for its cache numbers
- **−** Apple Silicon Macs only (M1 or newer)
- **−** Under 16 GB, the README says tool use is unreliable with Gemma 4 E4B
- **−** Benchmark scores come from the Agent-12 harness, not from inside Claude Code
- **−** Browser, voice and phone modes need separate repos or tools that setup.sh does not install

<sub>RAM ≥ 16 GB · GPU required · Needs Claude Code (npm), Python 3.12, mlx-lm · Models: Gemma 4, Qwen 3.8, Hermes 4 14B, MLX · port 4000 · [Repo](https://github.com/nicedreamzapp/claude-code-local) · [📖 Docs ↗](https://github.com/nicedreamzapp/claude-code-local/blob/main/docs/FULL-GUIDE.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-local/)</sub>

<a name="hallmark"></a>
### #&#8288;110 [hallmark](https://github.com/nutlope/hallmark) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Aug 2026</sub>

**Design skill that steers coding agents away from generic AI-looking UI.**

Hallmark is a skill for Claude Code, Cursor and Codex that picks a page macrostructure for a brief, applies one of twenty-one themes, and runs fifty-seven slop-test gates plus a self-critique before returning output. It has four verbs: build (default), audit, redesign and study, which extracts design traits from a screenshot or URL. Output is self-contained HTML and CSS.

- **+** Works across Claude Code, Cursor and Codex from one SKILL.md plus references
- **+** Audit verb scores existing code and returns a punch list without editing
- **+** Twenty-one themes plus a Custom branch for briefs no theme fits
- **+** Live demo site and example pages are linked for each theme
- **−** Example output is static HTML and CSS; framework support is not documented
- **−** Cursor install needs manual copy into a .mdc rule without frontmatter
- **−** No benchmarks showing the slop-test gates improve output
- **−** No tagged releases

<sub>no GPU · Needs Claude Code, Cursor or Codex, npx · safety checks passed 7 of 8 · [Repo](https://github.com/nutlope/hallmark) · [▶️ Demo ↗](https://www.usehallmark.com) · [🌐 Site ↗](https://www.usehallmark.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hallmark/)</sub>

<a name="garden-skills"></a>
### #&#8288;111 [garden-skills](https://github.com/conardli/garden-skills) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

**Six Agent Skills for design, video, image and retrieval tasks.**

Garden Skills is a set of SKILL.md-format skills for Claude Code, Cursor, Codex and other coding agents. The six skills cover web video presentations (Vite, React, TypeScript, 23 themes, pluggable TTS), front-end design, GPT Image 2 prompting and generation, article formatting, code-rendered short video, and local knowledge retrieval. Install options include the skills CLI via npx, the Claude Code plugin marketplace, release zips, manual copy or a git submodule.

- **+** Follows the SKILL.md spec, so it works across Claude Code, Cursor and Codex
- **+** Five install paths, including pinned per-skill release zips
- **+** web-design-engineer ships 25 style recipes and a design direction advisor
- **+** gpt-image-2 includes 79 prompt templates and three runtime modes
- **−** Skills are narrow: design, video, images and articles, not general coding
- **−** gpt-image-2 local mode needs an image API; key setup not shown in the visible README
- **−** Built-in TTS providers are only MiniMax and OpenAI; others are paste-in snippets
- **−** README is truncated, so details of three skills (article, showreel, kb-retriever) are unknown

<sub>no GPU · Needs Node.js (npx), OpenAI-compatible image API (gpt-image-2), MiniMax mmx-cli or OpenAI TTS (optional) · Models: GPT Image 2, OpenAI-compatible image APIs · [Repo](https://github.com/conardli/garden-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/garden-skills/)</sub>

<a name="one-skill-to-rule-them-all"></a>
### #&#8288;112 [one-skill-to-rule-them-all](https://github.com/rebelytics/one-skill-to-rule-them-all) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · CC-BY-4.0 · Oct 2026</sub>

**Claude meta-skill that logs corrections and proposes updates to your other skills.**

task-observer is a SKILL.md bundle with reference files and five helper scripts. It runs alongside Claude sessions, records corrections and repeated manual work as observation files, and proposes edits to existing skills or candidates for new ones. Changes go to staged copies, and nothing goes live until you install the updated bundle.

- **+** Proposals only: changes land in staged copies, installed skills stay untouched
- **+** Installs via `npx skills add` or a .skill bundle upload in the Claude apps
- **+** Writes one small observation file per entry under skill-observations/observation-log/
- **+** README reports 80+ contributors and 200+ issues and PRs closed
- **−** Description matching under-triggers; needs a CLAUDE.md instruction or session-start hook
- **−** Written around Claude concepts; other platforms need adaptation
- **−** Claude.ai web and mobile get handoff documents only, with no filesystem logging
- **−** README says small skill libraries may be served as well by built-in memory

<sub>no GPU · Needs Node.js (for skills CLI install), Claude or another skills-compatible agent · Models: Claude · [Repo](https://github.com/rebelytics/one-skill-to-rule-them-all) · [📖 Docs ↗](https://github.com/rebelytics/one-skill-to-rule-them-all/blob/main/USER-GUIDE.md) · [🌐 Site ↗](https://www.rebelytics.com/augmented-expertise/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/one-skill-to-rule-them-all/)</sub>

<a name="prompt-master"></a>
### #&#8288;113 [prompt-master](https://github.com/nidhinjs/prompt-master) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

**Claude skill that rewrites vague requests into tool-specific prompts.**

Prompt Master is a Claude skill that takes a plain request and returns a single copyable prompt tailored to a target tool such as Cursor, Claude Code, Midjourney or Stable Diffusion. It detects the target, extracts nine intent dimensions, asks at most three clarifying questions, picks one of 13 templates, and can prepend a Memory Block of prior decisions. Install by uploading the ZIP in claude.ai or cloning into ~/.claude/skills.

- **+** Profiles for 30+ named tools, plus a four-question fallback for unlisted tools
- **+** 13 prompt templates selected automatically, with a one-line strategy note per output
- **+** Asks at most three clarifying questions before writing the prompt
- **+** Installs as a skill folder via ZIP upload or git clone, no runtime needed
- **−** Output quality depends on Claude; no tests or benchmarks are shown in the README
- **−** Memory Block must be re-supplied each new session; it does not persist
- **−** Tool profiles name fast-moving models, so they can go stale without updates
- **−** No tagged releases; versioning is unknown

<sub>no GPU · Needs Claude.ai or Claude Code · Models: Claude, ChatGPT, Gemini, Grok, DeepSeek-R1 · [Repo](https://github.com/nidhinjs/prompt-master) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/prompt-master/)</sub>

<a name="awesome-codex-subagents"></a>
### #&#8288;114 [awesome-codex-subagents](https://github.com/voltagent/awesome-codex-subagents) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (34) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · Oct 2026</sub>

**Collection of 175+ ready-made Codex subagent definitions as TOML files.**

A library of Codex custom agent files in .toml format, grouped into 13 categories such as core development, language specialists, infrastructure, quality and security, and data and AI. You copy the files you want into ~/.codex/agents/ or .codex/agents/. Each file sets a model, reasoning effort, sandbox mode and instruction text. Codex does not spawn them automatically, so you delegate in prompts.

- **+** Plain .toml files installed by copying into ~/.codex/agents/ or .codex/agents/
- **+** Each agent sets model, reasoning effort and sandbox mode (read-only or workspace-write)
- **+** Covers many languages and frameworks plus infrastructure, security and data roles
- **+** Project-level agents override global ones on name conflicts
- **−** Codex does not auto-spawn custom subagents; you must delegate explicitly in prompts
- **−** No installer or package manager; installation is manual file copying
- **−** README gives no benchmarks of how the agents affect output quality
- **−** Model names in the files are fixed and may not match your Codex setup

<sub>no GPU · Needs Codex · Models: gpt-5.6-sol, gpt-5.6-terra, gpt-5.6-luna · [Repo](https://github.com/voltagent/awesome-codex-subagents) · [📖 Docs ↗](https://developers.openai.com/codex/subagents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-codex-subagents/)</sub>

<a name="security-audit-skill"></a>
### #&#8288;115 [security-audit-skill](https://github.com/cloudflare/security-audit-skill) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Sep 2026</sub>

**Coding-agent skill that runs a multi-phase security audit of a codebase.**

A skill for coding agents that audits a repository for vulnerabilities in six phases: reconnaissance, hunting, candidate validation, structured output, record verification and reporting. Isolated sub-agents hunt from a coverage ledger, and a fresh agent tries to disprove each candidate. Results go to findings.json, checked by Node validators, and to REPORT.md. It is the single-repo starting point for Cloudflare's vulnerability harness.

- **+** Separate agents find and validate each finding; verdicts are confirmed, needs_validation or rejected
- **+** Zero-dependency Node validators check findings.json and coverage-ledger.json against a schema
- **+** Attack-class prompts cover memory safety, web/auth, cloud, supply chain, client-side and LLM targets
- **+** Repeated runs reuse prior ledgers and findings to target coverage gaps
- **−** Needs a model with tool use and parallel sub-agents; token cost is unknown
- **−** Running target code requires an OS-enforced sandbox you must provide, else leads stay unvalidated
- **−** README says a single run found roughly half of what repeated runs found
- **−** No release published; install goes through the Skills CLI via npx

<sub>no GPU · Needs Node.js, Skills CLI (npx skills), coding agent with parallel sub-agents, OS-enforced sandbox · Models: any tool-use model with parallel sub-agents · safety checks passed 8 of 8 · [Repo](https://github.com/cloudflare/security-audit-skill) · [🌐 Site ↗](https://blog.cloudflare.com/build-your-own-vulnerability-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/security-audit-skill/)</sub>

<a name="claude-scholar"></a>
### #&#8288;116 [claude-scholar](https://github.com/galaxy-dawn/claude-scholar) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (29) · Freshness: active (96) · Maintenance: fair (57) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · MIT · Sep 2026</sub>

**Research workflow skills, agents and hooks for Claude Code, with Zotero and Obsidian.**

A bundle of skills, commands, agents, rules and Node.js hooks that structures academic research in Claude Code, from ideation and literature review through experiment analysis, reporting, paper writing and rebuttal. It integrates with Zotero via zotero-mcp and with an Obsidian vault for project notes. Separate branches cover Codex CLI, Kimi Code CLI and OpenCode.

- **+** Covers the full path: ideation, literature, experiments, analysis, reporting, writing, rebuttal
- **+** Installer backs up overwritten files and records a manifest for safe uninstall
- **+** Installs as a Claude Code plugin or by copying individual skills
- **+** Separate branches for Codex CLI, Kimi Code CLI and OpenCode
- **−** Workflow is tuned for computer science and AI research, per the README
- **−** Existing CLAUDE.md files must be merged by hand with the sidecar file
- **−** Plugin install does not distribute rules or configure settings.json
- **−** Zotero and Obsidian features need separate setup, including a zotero-mcp fork

<sub>no GPU · Needs Claude Code, Git, Zotero (optional), Galaxy-Dawn/zotero-mcp (optional), Obsidian (optional), Python + uv (optional) · [Repo](https://github.com/galaxy-dawn/claude-scholar) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-scholar/)</sub>

<a name="fireworks-tech-graph"></a>
### #&#8288;117 [fireworks-tech-graph](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Sep 2026</sub>

**Agent skill that generates validated SVG, PNG, GIF and HTML technical diagrams.**

A single Agent Skill for Codex and Claude Code that turns English or Chinese descriptions into SVG diagrams using a Python generator, then exports PNG, GIF motion and offline interactive HTML. It ships 12 visual styles and 14 diagram types (UML plus AI/agent patterns such as RAG and multi-agent), and checks geometry, routing and text fit before output.

- **+** Works in both Codex and Claude Code from one skill install
- **+** Deterministic validation of routing, crossings, spacing and labels before and after render
- **+** Exports SVG, PNG up to 4x, GIF and a single offline HTML file
- **+** 12 styles and 14 diagram types including the full UML set
- **−** GIF animation only accepts SVGs carrying one of twelve approved motion contracts
- **−** PNG and GIF export need optional dependencies; Puppeteer path needs Node.js 22.12+
- **−** Style 8 (Dark Luxury) is AI-authored rather than generator-backed
- **−** README carries sponsor and paid-consulting sections

<sub>no GPU · Needs Python 3.9+, Codex or Claude Code, Node.js 22.12+ (optional, Puppeteer PNG export), cairosvg or rsvg-convert (optional, PNG export) · [Repo](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fireworks-tech-graph/)</sub>

<a name="harness"></a>
### #&#8288;118 [harness](https://github.com/revfactory/harness) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (47) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · Apache-2.0 · Sep 2026</sub>

**Claude Code plugin that generates agent teams and skills from a project description.**

Harness is a Claude Code plugin that takes a domain description and writes agent definitions into .claude/agents/, skills into .claude/skills/, and a minimal CLAUDE.md pointer. It picks one of three execution modes (workflow scripts, persistent named agents with SendMessage, or one-shot sub-agents) and one of six team patterns. A /harness:evolve skill feeds usage feedback back into the generated harness.

- **+** Generates plain files in .claude/agents and .claude/skills that you can edit and commit
- **+** Covers six team patterns, each mapped to one of three execution modes
- **+** Includes /harness:evolve and a mechanical migration path from v1 artifacts
- **+** No environment variables or experimental flags required
- **−** Works only with Claude Code; no other agent host is mentioned
- **−** Quality claims come from an author-run A/B test on 15 tasks
- **−** Interactive walkthrough is in Korean only
- **−** No release published; version 2.1.0 appears only in a badge

<sub>no GPU · Needs Claude Code · Models: Claude (fable, opus, sonnet tiers) · [Repo](https://github.com/revfactory/harness) · [▶️ Demo ↗](https://revfactory.github.io/harness-animation/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/harness/)</sub>

<a name="cc-wf-studio"></a>
### #&#8288;119 [cc-wf-studio](https://github.com/breaking-brake/cc-wf-studio) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · custom license · Aug 2026</sub>

**Visual workflow canvas that exports agent skills and commands as Markdown.**

A VS Code extension with a React Flow canvas for designing multi-agent workflows. It exports them as Markdown skills, agents or commands for Claude Code, Copilot, Codex CLI, Gemini CLI, Cursor and others. The same workflow.json can also be driven through an npm CLI (ccwf) and a stdio MCP server (ccwf-mcp), so an external agent can read and edit workflows.

- **+** Exports to eight agents' formats, e.g. .claude/commands, .codex/skills, .cursor/skills
- **+** CLI and MCP server work without VS Code, usable in CI or over SSH
- **+** MCP tools (get_workflow, apply_workflow) let agents edit the canvas
- **+** CLI and MCP packages are MIT-licensed and published on npm
- **−** VS Code extension is AGPL-3.0-or-later, which may restrict some uses
- **−** Agents other than Claude Code must be enabled from the toolbar More menu
- **−** Usage examples and tutorials are listed as coming soon
- **−** Needs a separate agent CLI or extension installed to run workflows

<sub>no GPU · Needs VS Code, Claude Code or another supported agent, Node.js (for npx CLI) · Models: Claude Code, GitHub Copilot, OpenAI Codex CLI, Gemini CLI, Cursor · [Repo](https://github.com/breaking-brake/cc-wf-studio) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-wf-studio/)</sub>

<a name="huggingface-skills"></a>
### #&#8288;120 [skills](https://github.com/huggingface/skills) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

**Agent Skills for Hugging Face Hub, training, evals and SageMaker deployment.**

A collection of about 24 Agent Skills folders (SKILL.md plus scripts) that teach coding agents Hugging Face workflows: Hub CLI operations, TRL and Unsloth fine-tuning, evals, Spaces, Gradio, Trackio and SageMaker deployment. Claude Code and Cursor marketplaces expose only hf-cli; other skills install with `hf skills add <name>`. A Gemini CLI extension and a generated AGENTS.md fallback are included.

- **+** Follows the Agent Skills format; works with Claude Code, Codex, Gemini CLI and Cursor
- **+** hf-cli skill is generated from the locally installed CLI, so commands stay current
- **+** Covers datasets, training, evals, Spaces, papers and SageMaker deployment
- **+** AGENTS.md fallback bundle for agents without skill support
- **−** Client marketplaces list only hf-cli; other skills need the hf CLI to install
- **−** Codex install is a manual copy or symlink into .agents/skills
- **−** Training skills target Hugging Face Jobs, a hosted service
- **−** Some skills overlap, such as huggingface-llm-trainer and trl-training

<sub>no GPU · Needs hf CLI, Hugging Face Hub account, AWS account (SageMaker skills) · Models: Safetensors, GGUF · [Repo](https://github.com/huggingface/skills) · [📖 Docs ↗](https://huggingface.co/docs/hub/agents-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huggingface-skills/)</sub>

<a name="stitch-skills"></a>
### #&#8288;121 [stitch-skills](https://github.com/google-labs-code/stitch-skills) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (46) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Aug 2026</sub>

**Agent skills and plugins that drive Google Stitch design and code generation.**

A set of Agent Skills grouped into three plugins (stitch-design, stitch-build, stitch-utilities) for Google Stitch. They generate and edit screens, extract DESIGN.md and static HTML from code, and convert Stitch designs to React, React Native, Vite dashboards and Remotion videos. Install via Codex marketplace, `npx plugins` for Claude Code and Cursor, or manual copy for OpenCode; all skills need the Stitch MCP server.

- **+** Covers both directions: code to Stitch design and Stitch screens to React or React Native
- **+** Plugin install for Codex, Claude Code and Cursor; skills follow the Agent Skills standard
- **+** Each skill ships scripts, resources and examples alongside SKILL.md
- **+** Includes DESIGN.md extraction and generation to keep design tokens consistent
- **−** Requires the Stitch MCP server and Google Stitch credentials; not usable standalone
- **−** Skills have inter-dependencies, so selective install can leave gaps
- **−** OpenCode needs manual copying and renaming of skills with stitch:: names
- **−** Not an officially supported Google product

<sub>no GPU · Needs Stitch MCP server, Google Stitch, Node.js (npx) · [Repo](https://github.com/google-labs-code/stitch-skills) · [📖 Docs ↗](https://stitch.withgoogle.com/docs/mcp/setup/) · [🌐 Site ↗](https://stitch.withgoogle.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/stitch-skills/)</sub>

<a name="codex-plugin-cc"></a>
### #&#8288;122 [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (81) · Freshness: active (98) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Jul 2026</sub>

**Claude Code plugin that runs Codex reviews and delegates tasks.**

A Claude Code plugin that adds slash commands for running Codex code reviews and handing tasks to Codex without leaving Claude Code. It wraps the local Codex CLI and app server, so it reuses your existing Codex login, config.toml and base URL settings. Background jobs can be tracked and cancelled, and sessions can be resumed in Codex.

- **+** Reuses local Codex CLI auth and config.toml; no separate runtime
- **+** Read-only /codex:review and steerable /codex:adversarial-review with --base <ref>
- **+** Background jobs via /codex:status, /codex:result and /codex:cancel
- **+** Sessions can be continued in Codex with codex resume <session-id>
- **−** Requires Claude Code plus a ChatGPT subscription or OpenAI API key
- **−** Usage counts against Codex limits; optional review gate can drain them quickly
- **−** Multi-file reviews and rescue tasks can run long
- **−** /codex:transfer needs a Codex version that supports session import

<sub>no GPU · Needs Claude Code, Codex CLI (@openai/codex), Node.js 18.18+, ChatGPT account or OpenAI API key · Models: OpenAI Codex models (e.g. gpt-5.4-mini, gpt-5.3-codex-spark) · safety checks passed 10 of 11 · [Repo](https://github.com/openai/codex-plugin-cc) · [📖 Docs ↗](https://developers.openai.com/codex/app-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-plugin-cc/)</sub>

<a name="council-of-high-intelligence"></a>
### #&#8288;123 [council-of-high-intelligence](https://github.com/0xnyk/council-of-high-intelligence) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

**Multi-persona deliberation skill for coding agent CLIs.**

Adds a /council command that sends a decision to up to 18 analytical personas, such as Socrates, Torvalds and Taleb. Members analyze independently, cross-examine each other, then produce a verdict listing dissent, kill criteria and a next step. Seats can be spread across providers (native host, Codex, Gemini, Ollama, NVIDIA NIM, Cursor) so one model family does not argue both sides.

- **+** Full, quick and duo modes plus named triads for narrower questions
- **+** Same /council command across Claude Code, Codex, Gemini CLI and OpenCode
- **+** Verdicts keep dissent and unresolved questions, with FACT/INFERENCE/ASSUMPTION/UNKNOWN labels
- **+** Provider routing with --dry-route preview and fallback to the native host
- **−** No benchmarks or evals in the README; output quality depends on the underlying models
- **−** Full protocol runs several rounds across many personas, so token cost is likely high
- **−** Personas are prompt contracts, not verified expert models
- **−** Four host mirrors of SKILL.md must be kept aligned by hand

<sub>no GPU · Needs Claude Code, Codex, Gemini CLI or OpenCode, Optional: codex, gemini, ollama, cursor-agent executables or NVIDIA_API_KEY · Models: Claude Code native subagents, OpenAI via codex, Google via gemini, Ollama, NVIDIA NIM · [Repo](https://github.com/0xnyk/council-of-high-intelligence) · [🌐 Site ↗](https://www.nyk.dev/oss/council-of-high-intelligence) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/council-of-high-intelligence/)</sub>

<a name="sol-pi"></a>
### #&#8288;124 [sol-pi](https://github.com/nvlabs/sol-pi) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

**Token-saving extension for the Pi coding agent with four opt-in mechanisms.**

SoL-Pi is an NVIDIA extension for the Pi coding agent that cuts token use and agent turns. It adds Action Fusion (edit plus validation in one tool call), ObservationPack (handles for repeated large outputs), an evidence-checked log reducer, and context compaction at completed plan steps. It installs on unmodified Pi 0.85.1 and every mechanism is off until enabled in sol-pi.json.

- **+** Installs through Pi's public extension APIs; no Pi patches or vendored source
- **+** All mechanisms disabled by default; config is a single sol-pi.json
- **+** Reducer keeps a quotation only if it matches the archived source log
- **+** Includes a skill example for calling it from Claude Code or Codex
- **−** Tested only against Pi 0.85.1; pi-v1 support still in development
- **−** Archives persist locally and are not deleted when the session ends
- **−** Reducer sends diagnostic log content to a remote model when enabled
- **−** Requires Node.js 22.19 or newer; no Docker image

<sub>no GPU · Needs Node.js 22.19+, npm, @earendil-works/pi-coding-agent 0.85.1 · Models: Uses the model and provider configured in Pi, Reducer provider/model route set in sol-pi.json · [Repo](https://github.com/nvlabs/sol-pi) · [📖 Docs ↗](https://arxiv.org/abs/2609.20519) · [🌐 Site ↗](https://nvlabs.github.io/SoL-Pi/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sol-pi/)</sub>

<a name="frontend-slides"></a>
### #&#8288;125 [frontend-slides](https://github.com/zarazhangrui/frontend-slides) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (79) · Freshness: active (94) · Maintenance: weak (5) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Jun 2026</sub>

**Claude Code skill that generates HTML slide decks or converts PowerPoint files.**

A skill for Claude Code, packaged as a plugin, that builds single-file HTML presentations with inline CSS and JS. It shows three visual style previews to pick from, then writes the full deck, or extracts text, images and notes from a .pptx and rebuilds it for the web. Other coding agents can follow the same SKILL.md if they have filesystem and shell access.

- **+** Output is one HTML file with inline CSS/JS, no npm or build step
- **+** Converts .pptx files, extracting text, images and speaker notes
- **+** Ships 12 included styles plus 34 optional bold templates loaded on demand
- **+** Installs as a Claude Code plugin or by copying files into ~/.claude/skills
- **−** Plugin install flow and slash command are specific to Claude Code
- **−** Other agents must read SKILL.md manually; no install path is documented for them
- **−** Output is fixed 16:9 HTML, not editable .pptx
- **−** Style previews depend on the agent's generation, so results vary per run

<sub>no GPU · Needs Claude Code or another coding agent, Python (scripts/extract-pptx.py) · Models: Claude Code, Codex, Kimi Code, OpenCode, Gemini CLI · safety checks passed 8 of 9 · [Repo](https://github.com/zarazhangrui/frontend-slides) · [📖 Docs ↗](https://github.com/zarazhangrui/frontend-slides) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frontend-slides/)</sub>

<a name="scroll-world"></a>
### #&#8288;126 [scroll-world](https://github.com/oso95/scroll-world) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: weak (24) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Jul 2026</sub>

**Agent skill that builds scroll-scrubbed fly-through landing pages from AI-generated video.**

A SKILL.md-compatible skill for Claude Code, Codex and other agents. It interviews you about brand, scenes and budget, then generates isometric scene stills and Seedance or Kling camera clips with frame-locked seams. A vanilla-JS scrub engine ties the chain to scroll position, with an optional 9:16 mobile chain.

- **+** Frame-locked connector clips give one continuous flight with no cuts between scenes
- **+** Scrub engine is framework-agnostic vanilla JS: plain HTML, Next.js, Vue or Python-served pages
- **+** Optional native 9:16 portrait chain for phones instead of a cropped landscape film
- **+** States estimated cost and asks for approval before any generation runs
- **−** Needs paid services: Monid CLI plus Higgsfield credits; a 6-scene 1080p chain is about $27
- **−** Generated mp4/webp assets are not shipped; every project must render its own
- **−** Mobile chain doubles the video generation count and cost
- **−** Requires ffmpeg, Python 3 with Pillow and authenticated third-party CLIs

<sub>no GPU · Needs Monid CLI, Higgsfield CLI, ffmpeg, ffprobe, Python 3, Pillow, Codex CLI (optional) · Models: Seedance 2.0, Kling 3.0, GPT Image 2 · [Repo](https://github.com/oso95/scroll-world) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scroll-world/)</sub>

<a name="fast-jev-compaction"></a>
### #&#8288;127 [fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: known (42) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · MIT · Sep 2026</sub>

**Claude Code plugin that prunes stale tool calls instead of summarizing history.**

Replaces Claude Code's compaction summary with a pruned copy of the original transcript. Each tool call and result is scored by the Jev model through TypeSafe's API, and stale ones are dropped or truncated while user and assistant text stays verbatim. It also works as an npm library, and it falls back to the built-in summary on errors or small reductions.

- **+** Never rewrites content: kept messages stay verbatim, only tool calls and results are removed
- **+** Falls back to Claude Code's built-in summary on errors or insufficient reduction
- **+** Also exported as an npm library with a pluggable JevAsker transport and building blocks
- **+** Tunable keepThreshold, preserveRecentMessages, token ceilings and truncateHeadChars
- **−** Requires a TypeSafe API key and sends the conversation to an external Jev endpoint
- **−** Needs Claude Code 2.1.274+ with the early-access function hooks flag enabled
- **−** Text messages are never shortened, so long text-heavy sessions may reduce little
- **−** Token counts are estimates, and histories that cannot fit the state ceiling throw

<sub>no GPU · Needs TypeSafe API key (Jev model, api.typesafe.ai), Claude Code 2.1.274+ with CLAUDE_CODE_ENABLE_FUNCTION_HOOKS=1, Node.js and npm · Models: jev-latest · [Repo](https://github.com/tamaratran/fast-jev-compaction) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fast-jev-compaction/)</sub>

<a name="go-modern-guidelines"></a>
### #&#8288;128 [go-modern-guidelines](https://github.com/jetbrains/go-modern-guidelines) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Sep 2026</sub>

**Claude Code plugin that makes agents write current Go idioms.**

Guidelines covering Go 1.0 through 1.26 that tell a coding agent which language and stdlib features to use, such as max, slices.Contains, cmp.Or, new(42) and errors.AsType. The Claude Code plugin adds a /use-modern-go command that reads the Go version from go.mod and limits the agent to features up to that version. Junie includes the guidelines by default from version 2xx.620.xx.

- **+** Reads the target Go version from go.mod and limits features to it
- **+** Covers Go 1.0 to 1.26, including everything the modernize analyzer targets
- **+** Installs in two commands as a Claude Code plugin
- **+** Built into Junie with a settings toggle, no manual setup
- **−** Supports only Junie and Claude Code; no Cursor or Codex setup documented
- **−** Claude Code needs /use-modern-go run manually at the start of each session
- **−** Guidelines only; does not rewrite existing code, unlike the modernize analyzer
- **−** No tagged releases

<sub>no GPU · Needs Claude Code or Junie · [Repo](https://github.com/jetbrains/go-modern-guidelines) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/go-modern-guidelines/)</sub>

<a name="vibe-skills"></a>
### #&#8288;129 [vibe-skills](https://github.com/foryourhealth111-pixel/vibe-skills) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · Apache-2.0 · Oct 2026</sub>

**Skill router that plans tasks and assigns local agent Skills to each step.**

VibeSkills is a Skill for coding agents that confirms the requirement, picks an L or XL workflow, then scans your local Skill folders and assigns a few relevant Skills to each subtask. It records completed, failed and blocked units and checks results against the plan before acceptance. The README reports a SkillsBench run with 195 Skills (DeepSeekV4Flash-VE, OpenHands): +21.12 pp mean reward, 29.6% fewer tokens.

- **+** Benchmark study with public data and reproduction steps is linked from the README
- **+** Shortlists Skills from compact local indexes; reads full SKILL.md only for retained candidates
- **+** Records completed, failed and blocked work units so a later session can resume
- **+** Works over your own, team and third-party Skill folders without calling every Skill
- **−** Benchmark covers one model and agent setup (DeepSeekV4Flash-VE with OpenHands)
- **−** Requires approval steps before work starts, adding overhead on small tasks
- **−** Supported agent hosts are not listed in the visible README excerpt
- **−** README is truncated here, so install requirements are unknown

<sub>no GPU · Models: DeepSeekV4Flash-VE (benchmarked) · [Repo](https://github.com/foryourhealth111-pixel/vibe-skills) · [📖 Docs ↗](https://github.com/foryourhealth111-pixel/Vibe-Skills/blob/main/docs/quick-start.en.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-skills/)</sub>

<a name="agent-memory"></a>
### #&#8288;130 [agent-memory](https://github.com/tigerless-labs/agent-memory) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**Markdown-file long-term memory for coding agents, with local SQLite search.**

agent-memory stores agent memories as markdown files in one store, with a rebuildable SQLite FTS5 index (BM25, optional vector plugin fused by RRF) for local ranked recall. Hooks installed for Claude Code, Codex CLI and Muse Code distil memories at conversation boundaries, and a sleep-time pass consolidates them, with deletions only as proposals. It exposes a `mem` CLI and a `mem-mcp` stdio MCP server.

- **+** Files are the source of truth; `rm -rf .index/ && mem rebuild` loses nothing, enforced by a test
- **+** No LLM client in the library; reasoning borrows the host agent's CLI, so no API key required
- **+** One store shared across Claude Code, Codex CLI and Muse Code; any agent that runs shell commands works
- **+** Recall returns paths and abstracts, so the agent opens files only as deep as needed
- **−** No PyPI release; install is from a git checkout with uv sync
- **−** Benchmark is on a bounded LongMemEval-S haystack, so scores are not comparable to published ones
- **−** `context`, `sleep` and the proposal ledger have no MCP tool yet; CLI only
- **−** Muse Code setup needs OpenRouter credentials and a separate pproxy dependency

<sub>no GPU · Needs Python 3.12+, uv, SQLite FTS5, pproxy (Muse Code only), gcloud CLI (optional, Vertex AI reasoner) · Models: Claude Code, Codex CLI, Muse Code, Hermes, Vertex AI endpoint · [Repo](https://github.com/tigerless-labs/agent-memory) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-memory/)</sub>

<a name="nvidia-skills"></a>
### #&#8288;131 [skills](https://github.com/nvidia/skills) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · Apache-2.0 · Oct 2026</sub>

**Catalog of NVIDIA-maintained agent skills for Claude Code, Codex, Cursor and Kiro.**

A mirror of agent skills maintained in NVIDIA product repos, synced daily and installed with `npx skills add nvidia/skills`. The catalog covers cuOpt, cuDF, CUDA-Q, DOCA, Jetson BSP, Holoscan, BioNeMo, Dynamo, DeepStream and others, with many skills per product. Skills can be installed singly or per agent (claude-code, codex, cursor, kiro-cli, cortex).

- **+** Install one skill or several agents in a single `npx skills add` command
- **+** Skills are maintained in product repos and synced daily, so they track upstream
- **+** Wide coverage of NVIDIA software: cuOpt, cuDF, DOCA, Jetson, BioNeMo, Dynamo
- **+** Targets several agents: Claude Code, Codex, Cursor, Kiro, Snowflake CoCo
- **−** Only useful for NVIDIA software and hardware workflows
- **−** Mirror only; fixes must go to the upstream product repos
- **−** Requires skills CLI v1.5.16 or newer, or skills may not appear in Claude Code
- **−** Skills are renamed or consolidated over time, so local copies need `npx skills update`

<sub>Needs Node.js (npx), skills CLI (vercel-labs/skills) · Models: Claude Code, Codex, Cursor, Kiro, Snowflake CoCo · [Repo](https://github.com/nvidia/skills) · [📖 Docs ↗](https://docs.nvidia.com/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nvidia-skills/)</sub>

<a name="ralph"></a>
### #&#8288;132 [ralph](https://github.com/snarktank/ralph) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (69) · Freshness: slowing (40) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Feb 2026</sub>

**Bash loop that reruns Amp or Claude Code until every PRD story passes.**

Ralph is a bash script (ralph.sh) that repeatedly launches Amp or Claude Code with a fresh context, each time picking the highest-priority story in prd.json where passes is false. It implements one story, runs typecheck and tests, commits on success, and records learnings in progress.txt and AGENTS.md. It also ships prd and ralph skills for writing a PRD and converting it to prd.json.

- **+** Fresh context each iteration; state persists only in git, progress.txt and prd.json
- **+** Supports both Amp and Claude Code via a --tool flag
- **+** Small footprint: one shell script, prompt templates and two skills, plus jq
- **+** Installable as a Claude Code plugin marketplace entry
- **−** Needs working typecheck and tests; broken checks compound across iterations
- **−** Stories must fit one context window; large ones must be split by hand
- **−** Requires an authenticated Amp or Claude Code install, which are separate tools
- **−** No tagged releases; default cap is 10 iterations

<sub>no GPU · Needs Amp CLI or Claude Code, jq, git · Models: Amp, Claude Code · [Repo](https://github.com/snarktank/ralph) · [📖 Docs ↗](https://snarktank.github.io/ralph/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph/)</sub>

<a name="remodex"></a>
### #&#8288;133 [remodex](https://github.com/emanuele-web04/remodex) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Sep 2026</sub>

**iPhone remote control for Codex and OpenCode running on your Mac.**

Remodex pairs an iOS app with a Node.js bridge (`remodex up`) on your Mac, which spawns `codex app-server` and forwards JSON-RPC over a WebSocket relay. Prompts, streaming output, git actions and OpenCode chats are handled from the phone while the coding runtime stays local. Pairing uses a one-time QR and an end-to-end encrypted channel; a local relay script is included for self-hosting.

- **+** End-to-end encrypted session using X25519 keys; QR pairing, then trusted reconnects
- **+** Runs Codex, git and workspace actions locally on the Mac, not on a hosted service
- **+** Includes relay source and run-local-remodex.sh for self-hosting, default port 9000
- **+** Phone supports git commit/push/pull, plan mode, steering runs and queued prompts
- **−** Background daemon and auto-reconnect work on macOS only; other OSes run in the foreground
- **−** Needs a signed iOS build or App Store install; no Android client
- **−** Plain LAN ws:// pairing can be unreliable on iOS; Tailscale recommended
- **−** Author warns of early-stage bugs and is not accepting contributions yet

<sub>no GPU · Needs Node.js 18+, Codex CLI (authenticated), OpenCode CLI (for OpenCode chats), iPhone with Remodex app, Xcode 16+ (to build from source), Tailscale or Cloudflare Tunnel (recommended for remote) · Models: Codex, OpenCode (Zen, Go, Free models) · port 9000 · [Repo](https://github.com/emanuele-web04/remodex) · [🌐 Site ↗](https://apps.apple.com/us/app/remodex-remote-ai-coding/id6760243963) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/remodex/)</sub>

<a name="swiftui-agent-skill"></a>
### #&#8288;134 [swiftui-agent-skill](https://github.com/twostraws/swiftui-agent-skill) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: known (32) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Oct 2026</sub>

**Agent skill that steers coding assistants toward modern, accessible SwiftUI code.**

SwiftUI Pro is a skill in the Agent Skills format that gives coding assistants rules for writing and reviewing SwiftUI. The rules cover API usage, navigation, layout, animations, state management, performance, VoiceOver accessibility and deprecated API, aimed at mistakes LLMs commonly make. It installs through npx or as a Claude Code plugin and is invoked with /swiftui-pro or $swiftui-pro.

- **+** Works with Claude Code, Codex, Gemini, Cursor and others via the Agent Skills format
- **+** Installs with one npx command or as a Claude Code plugin
- **+** Can run a partial review, such as deprecated API only or accessibility only
- **+** Contribution rules keep SKILL.md short to limit token cost
- **−** Covers SwiftUI only; SwiftData, concurrency and testing are separate skills
- **−** Targets iOS 26+ and Swift 6.4+, so older projects may get mismatched advice
- **−** Install via npx requires Node, which the README installs through Homebrew
- **−** No benchmarks or measured results are given for the rules

<sub>no GPU · Needs Node.js (npx) for install, Claude Code, Codex, Gemini, Cursor or another Agent Skills-compatible agent · Models: Claude Code, Codex, Gemini, Cursor · [Repo](https://github.com/twostraws/swiftui-agent-skill) · [🌐 Site ↗](https://www.hackingwithswift.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/swiftui-agent-skill/)</sub>

<a name="ip-as-logo-skill"></a>
### #&#8288;135 [ip-as-logo-skill](https://github.com/s1dashu/ip-as-logo-skill) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: known (31) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Aug 2026</sub>

**Agent Skill that generates simple, cute animal mascot images from a brief.**

A single-file Agent Skill (SKILL.md) that guides a compatible agent through proposing three mascot directions, then generating six separate square images with an image model. Each image follows fixed rules: 4–7 basic shapes, three colors, and the character emerging from the lower-left or lower-right corner. It installs with `npx skills@latest add s1dashu/ip-as-logo-skill`.

- **+** Fixed, checkable design rules: 4–7 shapes, three semantic colors, 3 left / 3 right split
- **+** Installs through the Agent Skills CLI, with a global option
- **+** Works with several agents (Codex, Coze, Doubao, Manus, Gemini Apps, Replit Agent)
- **+** No scripts or dependencies; the skill is one instruction document
- **−** Needs a top-tier image model (GPT Image 2, Nano Banana Pro or similar) or an API key
- **−** Each candidate is generated once, with no validation or automatic retry
- **−** Never falls back to SVG, so output is raster images only
- **−** Defaults to familiar animals; other subjects need a stated product reason

<sub>no GPU · Needs Agent Skills CLI (npx skills), Image generation model or API key · Models: GPT Image 2, Seedance 5.0 Pro, Nano Banana Pro, Nano Banana 2 · [Repo](https://github.com/s1dashu/ip-as-logo-skill) · [🌐 Site ↗](https://ipaslogo.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ip-as-logo-skill/)</sub>

<a name="antfu-skills"></a>
### #&#8288;136 [skills](https://github.com/antfu/skills) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: known (31) · Freshness: active (100) · Maintenance: weak (21) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

**Agent Skills for Vue, Nuxt, Vite, Vitest and pnpm, plus Anthony Fu's conventions.**

A collection of Agent Skills (markdown files) covering Vue, Nuxt, Pinia, Vite, VitePress, Vitest, UnoCSS and pnpm, plus two hand-maintained skills for Anthony Fu's project conventions and PR creation. Most skills are generated from upstream documentation referenced as git submodules, and install through the skills CLI or the skills-npm pack. The README describes it as a proof of concept whose real-world performance is not fully tested.

- **+** Generated skills reference upstream docs via git submodules, so they can be synced with source changes
- **+** Installs with one command via the skills CLI or as an npm dev dependency through skills-npm
- **+** Can be forked as a template to generate your own skills collection with pnpm scripts
- **+** MIT licensed; skills are plain markdown that any Agent Skills-compatible agent can read
- **−** README states it is a proof of concept and skill effectiveness is not fully tested
- **−** Narrow coverage: eight generated skills, all in the Vue/Vite ecosystem, plus two opinionated ones
- **−** Skills load on demand, so agents may fail to pull them in when expected
- **−** No tagged releases

<sub>no GPU · Needs pnpm, skills CLI (vercel-labs/skills) or skills-npm, git submodules · [Repo](https://github.com/antfu/skills) · [📖 Docs ↗](https://agentskills.io/home) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/antfu-skills/)</sub>

<a name="vibe-wise"></a>
### #&#8288;137 [vibe-wise](https://github.com/nykooi1/vibe-wise) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Oct 2026</sub>

**Claude Code and Codex plugin that makes the AI ask for your design first.**

VibeWise is a plugin for Claude Code and Codex that adds a learning mode. The AI asks for your approach, discusses tradeoffs, and writes code only after you confirm a design and an implementation checkpoint. Preferences, notes and a project map are stored in .vibe-wise/ in your project and shared between both tools.

- **+** Works in both Claude Code and Codex, sharing the same .vibe-wise/ notes
- **+** Explicit Build, Design and Implementation checkpoints gate when code is written
- **+** Adjustable experience level and checkpoint frequency (Light, Normal, Frequent)
- **+** No extra account, backend or telemetry; Python 3 only, no extra packages
- **−** Slower than direct code generation by design, since every step waits on your input
- **−** Requires Claude Code or Codex; not usable standalone
- **−** In Codex, the learn command must be re-run at the start of each session
- **−** Saved notes enter the AI context, so they follow your tool's data settings

<sub>no GPU · Needs Claude Code or Codex, Python 3 · Models: Claude Code, Codex · [Repo](https://github.com/nykooi1/vibe-wise) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-wise/)</sub>

<a name="scroll-craft"></a>
### #&#8288;138 [scroll-craft](https://github.com/nateherkai/scroll-craft) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Sep 2026</sub>

**Agent skill for building scroll-driven websites with a design standard.**

scroll-craft is a skill for Codex, Claude Code or other coding agents that builds scroll-driven sites with video scrubbing, pinned sections and pointer effects. It supplies a design workflow, eight page grammars, a fingerprint gate against repeating earlier builds, and a headless-browser pass that checks dead scroll, contrast and stuck video. It also ships as a Claude Code plugin.

- **+** Headless browser checks every scroll position for dead scroll, contrast and undecoded clips
- **+** Fingerprint gate forces each new build to differ on at least 4 of 6 dimensions
- **+** Works with your own photos and footage; the generation API key is optional
- **+** Installs as a Claude Code plugin or as a plain folder for other agents
- **−** Author states it has only been run on Windows; no macOS build done
- **−** Needs a full ffmpeg build and playwright-core with Chrome for encoding and verification
- **−** Generated assets need a KIE_AI_API_KEY and real spend for video-heavy builds
- **−** Opinionated: refuses common layouts and palettes, and the engine is not edited per project

<sub>no GPU · Needs Node 18+, ffmpeg (full build), playwright-core, Chrome, KIE_AI_API_KEY (optional) · Models: Codex, Claude Code · [Repo](https://github.com/nateherkai/scroll-craft) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scroll-craft/)</sub>

<a name="gsap-skills"></a>
### #&#8288;139 [gsap-skills](https://github.com/greensock/gsap-skills) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (63) · Freshness: recent (68) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 16k · MIT · Apr 2026</sub>

**Official GSAP skills that teach coding agents correct animation API usage.**

Eight Agent Skills-format skill folders covering GSAP core tweens, timelines, ScrollTrigger, plugins, gsap.utils, React (useGSAP), performance, and Vue/Svelte lifecycle handling. Installs with `npx skills add` or the Claude Code plugin marketplace, and works with Cursor, Codex, Windsurf and others. Copilot gets a separate instructions file to copy by hand.

- **+** Maintained by the GSAP authors (greensock), so API guidance tracks the library
- **+** Eight skills split by topic: core, timeline, ScrollTrigger, plugins, utils, React, performance, frameworks
- **+** One install command via the skills CLI; Claude Code and Cursor plugin manifests included
- **+** Covers cleanup patterns such as useGSAP, gsap.context() and ScrollTrigger.refresh()
- **−** Only useful for GSAP; no effect on projects using other animation libraries
- **−** Copilot does not load skills; instructions must be copied manually
- **−** Instructs agents to recommend GSAP when no library is specified, which biases output
- **−** No tests or evals of skill effectiveness are described

<sub>no GPU · Needs Node.js and npx (for skills CLI), gsap npm package in target project · Models: Claude Code, Cursor, Codex, Windsurf, GitHub Copilot · [Repo](https://github.com/greensock/gsap-skills) · [🌐 Site ↗](https://gsap.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gsap-skills/)</sub>

<a name="claude-code-infrastructure-showcase"></a>
### #&#8288;140 [claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (50) · Freshness: active (98) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Jul 2026</sub>

**Reference library of Claude Code skills, hooks and agents with auto-activation.**

A copy-into-your-project .claude/ directory holding 4 skills, 9 hooks, 8 agents and 4 slash commands, extracted from a TypeScript microservices codebase. A UserPromptSubmit hook reads skill-rules.json and prompts Claude to load matching skills, using regex by default or an optional AI classifier (Gemini, OpenAI, Anthropic, Ollama). A setup wizard (setup.ts) installs it and runs 8 health checks; Codex CLI is also wired up.

- **+** Regex activation mode needs no API key and makes no network calls
- **+** Setup wizard copies files and runs 8 verification checks, plus /verify-setup
- **+** Same hooks and skills work under Codex CLI via an adapter shim
- **+** Skills split into SKILL.md plus resource files for progressive loading
- **−** Not a working app; components must be copied and customized per project
- **−** Bundled skills target Express, Prisma, React and MUI v7 only
- **−** Hooks are bash scripts; Windows needs WSL2
- **−** Stop hooks like tsc-check need heavy customization; Codex lacks a Skill tool event

<sub>no GPU · Needs Node.js 18+, npm, jq (optional Stop hooks), bash (macOS, Linux or WSL2), Gemini/OpenAI/Anthropic API key or Ollama (optional AI mode) · Models: Gemini gemini-3-flash-preview, OpenAI gpt-4o-mini, Anthropic claude-haiku-4-5, Ollama llama3.2 · [Repo](https://github.com/diet103/claude-code-infrastructure-showcase) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-infrastructure-showcase/)</sub>

<a name="improve"></a>
### #&#8288;141 [improve](https://github.com/shadcn/improve) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: known (48) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Sep 2026</sub>

**Agent skill that audits a codebase and writes plans for cheaper agents to run.**

An Agent Skills-format skill, invoked as /improve, that maps a repo, runs parallel audits across nine categories, re-checks each finding against the cited file and line, and writes self-contained markdown plans into plans/. It never edits source itself. An optional execute mode dispatches a cheaper model in an isolated git worktree and reviews the diff against the plan.

- **+** Advisor re-reads every cited file:line before showing findings, dropping false positives
- **+** Plans inline code excerpts, verification commands and STOP conditions for small executor models
- **+** Writes only to plans/; executors work in disposable worktrees and merging stays manual
- **+** Scoped modes: quick, deep, branch, security, plus reconcile to refresh the backlog
- **−** Needs an agent host that supports the Agent Skills format
- **−** Full audits fan out parallel subagents on a capable model; cost is not documented
- **−** No release tagged and no stated model or version requirements
- **−** Plan quality depends on the advisor model; no benchmarks given

<sub>no GPU · Needs Agent Skills-compatible coding agent, Node.js (npx) for install, git, GitHub (optional, for --issues) · [Repo](https://github.com/shadcn/improve) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/improve/)</sub>

<a name="longmemory"></a>
### #&#8288;142 [longmemory](https://github.com/caviraoss/longmemory) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (23) · Freshness: active (89) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Sep 2026</sub>

**Temporal, access-controlled memory store for LLM agents, backed by SQLite.**

LongMemory is a TypeScript memory engine that ingests events, documents and coding-agent sessions into an immutable graph stored in SQLite. It offers strict, historical, associative and world-grounded recall with separate recorded and valid time. The engine is exposed as an npm library, CLI, HTTP API, MCP server, Next.js dashboard and VS Code extension, plus a zero-dependency Python HTTP client.

- **+** Recorded time and valid time are separate, so historical recall returns superseded facts
- **+** Runs in-memory or on SQLite with no external database; reopening restores state
- **+** One engine across npm, CLI, HTTP, MCP (13 tools), dashboard and VS Code
- **+** Imports sessions from Claude Code, Codex, OpenCode, Gemini CLI, Copilot Chat and Cline
- **−** Python package is only an HTTP client; the engine needs the TypeScript service
- **−** Last tagged release is 2025-12-12, well behind recent commits
- **−** Embedding providers must be configured separately (OpenAI-compatible, Gemini, Bedrock, Ollama)
- **−** Hosted deployments require setting an API key and mounting persistent storage at /data

<sub>no GPU · Docker + Compose · Needs SQLite, Node.js, pnpm · Models: OpenAI-compatible APIs, Gemini, AWS Bedrock, Ollama, Siray · port 7331 · [Repo](https://github.com/caviraoss/longmemory) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/longmemory/)</sub>

<a name="claude-code-workflows"></a>
### #&#8288;143 [claude-code-workflows](https://github.com/oneredoak/claude-code-workflows) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Oct 2026</sub>

**Claude Code slash commands and GitHub Actions for PR, security and design review.**

A repository of three review workflows for Claude Code: code review, security review and design review. Each combines slash commands with GitHub Actions or subagents; the design review drives a browser through Playwright MCP. It also ships a free 16-page PDF guide on structuring context, tools, workflows and verification around coding agents.

- **+** Covers three review types: PR code review, OWASP-based security scan, and browser-based UI review
- **+** Slash commands allow on-demand runs; GitHub Actions allow automated PR checks
- **+** Design review uses Playwright MCP to inspect rendered UI, not just diffs
- **+** MIT licensed, with video tutorials for each workflow
- **−** Config files to copy, not an installable package; no release published
- **−** Requires Claude Code and an Anthropic API setup for the Actions; costs not documented
- **−** Setup details live in subfolders; the main README gives no install steps
- **−** Tutorials are on the author's YouTube channel and tied to his newsletter

<sub>no GPU · Needs Claude Code, GitHub Actions, Playwright MCP · Models: Claude · [Repo](https://github.com/oneredoak/claude-code-workflows) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-workflows/)</sub>

<a name="effective-html"></a>
### #&#8288;144 [effective-html](https://github.com/plannotator/effective-html) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

**Agent skills that generate HTML wireframes, prototypes, plans and diagrams.**

Six skills for coding agents that produce self-contained HTML artifacts: wireframes, working prototypes, plans, diagrams, and general reports or landing pages. They install with `npx skills add`, as a Claude Code plugin, or as a Codex plugin, and can also be read as plain reference. Each skill works on its own, and the broad `html` skill routes requests to the specialist ones.

- **+** Six skills, each installable individually via `npx skills add --skill`
- **+** Packaged for Claude Code and Codex plugin marketplaces as well as the skills CLI
- **+** Usable as a reference without installing anything
- **+** Skills require artifacts to be responsive, accessible, self-contained and browser-verified
- **−** Output quality depends on the agent and model; no benchmarks or examples of results in README
- **−** No release published, so no versioned installs
- **−** README does not say how the browser verification step is run
- **−** README promotes other tools (Plannotator, tot) alongside the skills

<sub>no GPU · Needs Node.js (npx skills CLI), Claude Code or Codex · [Repo](https://github.com/plannotator/effective-html) · [📖 Docs ↗](https://docs.plannotator.ai/learn/code-context/html-wireframes-and-prototypes-for-coding-agents) · [🌐 Site ↗](https://www.effectivehtml.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/effective-html/)</sub>

<a name="lottie"></a>
### #&#8288;145 [lottie](https://github.com/diffusionstudio/lottie) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · MIT · Jul 2026</sub>

**Agent skill that generates Lottie animations from text prompts.**

Text-to-lottie is a skill installed with `npx skills add diffusionstudio/lottie` that lets Claude Code, Codex or another skills-capable coding agent write Lottie JSON animations. The agent sets up a workspace with a bundled player that loads scenes from `public/projects/<project>/<scene>/lottie.json` and live-updates as files change. The README includes a prompt guide and playback snippets for web, React Native, iOS, Android and Flutter.

- **+** Works with any coding agent that supports skills, not tied to one vendor
- **+** Bundled player live-reloads and scrubs scenes while the agent edits the JSON
- **+** Output is plain Lottie JSON; README says it can be imported into After Effects
- **+** README gives playback examples for web, React Native, iOS, Android and Flutter
- **−** Needs a separate coding agent and its model access; no model is bundled
- **−** Output quality depends on prompts; README advises supplying SVGs or screenshots
- **−** By default only a background color control is exposed unless requested
- **−** No hosted demo or separate docs site listed in the README

<sub>no GPU · Needs Claude Code, Codex or other skills-capable coding agent, Node.js (npx) · Models: Claude Code, Codex · [Repo](https://github.com/diffusionstudio/lottie) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lottie/)</sub>

<a name="buildwithclaude"></a>
### #&#8288;146 [buildwithclaude](https://github.com/davepoon/buildwithclaude) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (16) · Freshness: active (85) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Oct 2026</sub>

**Plugin marketplace of Claude Code agents, commands, hooks and skills.**

A Claude Code plugin marketplace hosting 117 agents, 175 slash commands, 28 hooks, 26 skills and 51 bundled plugins, installed with `/plugin marketplace add davepoon/buildwithclaude`. A web UI at buildwithclaude.com also indexes community plugins, MCP servers and other marketplaces. Files can alternatively be copied by hand into ~/.claude/agents and ~/.claude/commands.

- **+** Installs through the native /plugin marketplace flow, per plugin or as all-in-one bundles
- **+** Large curated set: 117 agents, 175 commands, 28 hooks, 26 skills
- **+** Manual install path: copy markdown files into ~/.claude/agents or commands
- **+** Web UI with search, filtering and copyable install commands
- **−** Targets Claude Code only; no stated support for other coding agents
- **−** Community index counts (20k+ plugins, 4,500+ MCP servers) are not vetted per the README
- **−** Contribution validation is `npm test`; no per-item quality testing is described
- **−** Last release is 2025-10-24, well behind recent commits

<sub>no GPU · Docker · Needs Claude Code · Models: Claude · [Repo](https://github.com/davepoon/buildwithclaude) · [📖 Docs ↗](https://code.claude.com/docs/en/plugin-marketplaces) · [🌐 Site ↗](https://www.buildwithclaude.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/buildwithclaude/)</sub>

<a name="openskills"></a>
### #&#8288;147 [openskills](https://github.com/numman-ali/openskills) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: popular (54) · Freshness: slowing (47) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Jan 2026</sub>

**CLI that installs SKILL.md skills and lists them in AGENTS.md.**

OpenSkills installs Anthropic-format SKILL.md skills from GitHub, private git repos or local paths into .claude/skills or .agent/skills. It writes the same <available_skills> XML that Claude Code uses into AGENTS.md, and agents load a skill on demand with `npx openskills read <name>`. This lets Cursor, Windsurf, Aider, Codex and other agents that read AGENTS.md use the same skills.

- **+** Same SKILL.md format and folder layout as Claude Code, so skills are portable
- **+** Skills load on demand through a shell command, keeping context small
- **+** Installs from GitHub, private git URLs or local paths; project-local by default
- **+** No server or MCP support needed; runs via npx
- **−** Agents must run shell commands to load skills; no native Skill tool
- **−** Requires Node.js 20.6+ and Git
- **−** Skill sourcing is limited to git repos and local paths; no separate registry
- **−** Detected license is NOASSERTION, though the README states Apache 2.0

<sub>no GPU · Needs Node.js 20.6+, Git · [Repo](https://github.com/numman-ali/openskills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openskills/)</sub>

<a name="ccpm"></a>
### #&#8288;148 [ccpm](https://github.com/automazeio/ccpm) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: known (45) · Freshness: recent (56) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Mar 2026</sub>

**Agent skill that turns PRDs into GitHub issues and parallel agent work.**

CCPM is an Agent Skill that guides a coding agent from brainstorming and a PRD to a technical epic, task files, GitHub issues and a dedicated git worktree. It then launches parallel agents on independent work streams for an issue. Project state lives as markdown under `.claude/`, and status, standup and search run as bash scripts without LLM calls.

- **+** Follows the agentskills.io standard; works with Claude Code, Codex, OpenCode, Factory, Amp, Cursor
- **+** Project state is plain markdown in the repo, with no external database
- **+** Status, standup, search and validate run as bash scripts with no token cost
- **+** Task files carry depends_on, parallel and conflicts_with metadata for parallel agents
- **−** Requires an authenticated gh CLI and a GitHub repository
- **−** Parent-child sub-issues need the gh-sub-issue extension; otherwise falls back to task lists
- **−** Benchmark and team-result figures are self-reported with no method described
- **−** Original /pm:* slash commands only exist on the v1 branch

<sub>no GPU · Needs git, gh CLI, GitHub repository, gh-sub-issue extension (optional) · [Repo](https://github.com/automazeio/ccpm) · [🌐 Site ↗](https://automaze.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ccpm/)</sub>

<a name="continuous-claude-v3"></a>
### #&#8288;149 [continuous-claude-v3](https://github.com/parcadei/continuous-claude-v3) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: niche (20) · Freshness: slowing (37) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Jan 2026</sub>

**Claude Code add-on for session handoffs, memory, and a library of skills and agents.**

Installs 109 skills, 32 agents and 30 hooks into Claude Code's ~/.claude config. Hooks write YAML handoffs before compaction and recall learnings from a PostgreSQL+pgvector store, so sessions resume with state preserved. A TLDR analysis layer (AST, call graph, CFG, DFG, slicing) with a FAISS index is meant to cut tokens spent reading code.

- **+** Hooks write YAML handoffs before compaction and reload ledger, handoff and memory at session start
- **+** Memory in PostgreSQL with pgvector; remote Postgres supported via CONTINUOUS_CLAUDE_DB_URL
- **+** Hook-driven skill suggestions for natural-language prompts, plus workflows like /fix, /build, /tdd
- **+** Uninstall mode archives ~/.claude and restores the earlier backup
- **−** Requires Docker for PostgreSQL, plus Python 3.11+ and uv; 12-step setup wizard
- **−** Tied to Claude Code; no other coding agent is supported
- **−** Large footprint of 109 skills and 30 hooks that modifies ~/.claude
- **−** No tagged releases; the 95% token-savings figure is the README's own claim

<sub>Compose · Needs Claude Code CLI, Python 3.11+, uv, Docker, PostgreSQL with pgvector · Models: Claude · [Repo](https://github.com/parcadei/continuous-claude-v3) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/continuous-claude-v3/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
