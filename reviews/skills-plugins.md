# 🧩 Skills, plugins and prompts reviews · Best of Vibe Coding

Add-ons that make coding agents better (skills, plugins, rules, hooks, memory) and prompt collections to learn from or reuse. Back to the [leaderboard](../README.md#-skills-plugins-and-prompts).

<sub>🌐 Also on the web: [Skills, plugins and prompts on archestack.com](https://archestack.com/best-of-vibe-coding/skills-plugins/), each project on its own page.</sub>

<a name="impeccable"></a>
### 🥇 [impeccable](https://github.com/pbakaus/impeccable) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 84k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (only for npx installer), impeccable.style roll API · Models: Claude Code, Cursor, Codex CLI, Gemini CLI, GitHub Copilot · safety checks passed 11 of 12 · [Repo](https://github.com/pbakaus/impeccable) · [▶️ Demo ↗](https://impeccable.style/cases/neo-mirai) · [📖 Docs ↗](https://impeccable.style) · [🌐 Site ↗](https://impeccable.style) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/impeccable/)</sub>

<a name="caveman"></a>
### 🥈 [caveman](https://github.com/juliusbrussee/caveman) <sub>score [95](../README.md#-how-we-rank "Score 95/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 114k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 22.13+, Caveman account (Auto only) · Models: Claude Code, Codex, Gemini CLI, OpenCode, Aider · safety checks passed 10 of 12 · [Repo](https://github.com/juliusbrussee/caveman) · [▶️ Demo ↗](https://caveman.so/demo) · [📖 Docs ↗](https://docs.caveman.so) · [🌐 Site ↗](https://caveman.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/caveman/)</sub>

<a name="skills"></a>
### 🥉 [skills](https://github.com/mattpocock/skills) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 300k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Issue tracker (GitHub, GitLab or local files) · Models: Any model (per README) · safety checks passed 11 of 12 · [Repo](https://github.com/mattpocock/skills) · [🌐 Site ↗](https://skills.sh/mattpocock/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skills/)</sub>

<a name="ecc"></a>
### #&#8288;4 [ecc](https://github.com/affaan-m/ecc) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 285k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 18+, Git, Claude Code 2.1+ (for plugin setup) · Models: Claude Code, Codex, Kimi Code, Cursor, OpenCode · safety checks passed 12 of 12 · [Repo](https://github.com/affaan-m/ecc) · [🌐 Site ↗](https://ecc.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ecc/)</sub>

<a name="oh-my-claudecode"></a>
### #&#8288;5 [oh-my-claudecode](https://github.com/yeachan-heo/oh-my-claudecode) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Node.js/npm, tmux (for omc team), codex, gemini, agy, grok or cursor-agent CLIs (optional) · Models: Claude, Codex, Gemini, Antigravity, Grok · safety checks passed 11 of 12 · [Repo](https://github.com/yeachan-heo/oh-my-claudecode) · [📖 Docs ↗](https://yeachan-heo.github.io/oh-my-claudecode-website/docs/) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-claudecode-website) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-claudecode/)</sub>

<a name="ui-ux-pro-max-skill"></a>
### #&#8288;6 [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 138k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Python 3, Node.js/npm (for the uipro CLI) · Models: Claude Code, Cursor, Windsurf, Codex CLI, Gemini CLI · safety checks passed 11 of 11 · [Repo](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) · [🌐 Site ↗](https://uupm.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui-ux-pro-max-skill/)</sub>

<a name="agent-skills"></a>
### #&#8288;7 [agent-skills](https://github.com/addyosmani/agent-skills) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 109k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx) for skills CLI install, Git, A supported coding agent · safety checks passed 10 of 11 · [Repo](https://github.com/addyosmani/agent-skills) · [📖 Docs ↗](https://github.com/addyosmani/agent-skills/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills/)</sub>

<a name="claude-mem"></a>
### #&#8288;8 [claude-mem](https://github.com/thedotmack/claude-mem) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 102k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 20+, Bun, uv, SQLite, Chroma · Models: Anthropic plan, OpenRouter, Gemini, claude-mem observer (hosted) · safety checks passed 10 of 11 · [Repo](https://github.com/thedotmack/claude-mem) · [📖 Docs ↗](https://docs.claude-mem.ai/) · [🌐 Site ↗](https://docs.claude-mem.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-mem/)</sub>

<a name="ruflo"></a>
### #&#8288;9 [ruflo](https://github.com/ruvnet/ruflo) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 78k · MIT · Oct 2026</sub>

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

<sub>Needs Node.js/npx, Claude Code or Codex · Models: Claude, Codex, Ollama (via ruflo-ruvllm) · safety checks passed 14 of 18 · [Repo](https://github.com/ruvnet/ruflo) · [▶️ Demo ↗](https://raw.githubusercontent.com/ruvnet/ruflo/main/docs/assets/ruflo-console-theme-compact.svg) · [📖 Docs ↗](https://github.com/ruvnet/ruflo/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://cognitum.one/agentic-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruflo/)</sub>

<a name="book-to-skill"></a>
### #&#8288;10 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

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

<a name="ponytail"></a>
### #&#8288;11 [ponytail](https://github.com/dietrichgebert/ponytail) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 171k · MIT · Oct 2026</sub>

**Agent skill that makes coding agents write less code.**

Ponytail is a single prompt (SKILL.md, with a compact AGENTS.md version) that tells a coding agent to reuse existing code, the standard library or native platform features before writing new code. It adds slash commands for diff review, repo audit and deferred-shortcut tracking. In Claude Code it also shows a cost and token band and a local board. It installs as a Claude Code or Codex plugin, or as a rules file for other agents.

- **+** README badge says it works with 20 agents; plugin installs for Claude Code and Codex, rules file for others
- **+** Own benchmark of 39 tasks, 5 runs each, reports -53% code and 98% of risky logic shipping with a test
- **+** Keeps validation, security and accessibility; leaves one small test for logic with branches
- **+** No config file required; level set with /ponytail lite, full, ultra or off
- **−** Benchmark is the author's own, run only in Claude Code with Opus 5.5
- **−** Slash commands need a skill-capable host; Cursor rules, Windsurf, Cline and Copilot get only the ruleset
- **−** Band and board need Claude Code 2.1.290+ and do not show in the VS Code panel or claude -p
- **−** Behavior depends on the agent following a prompt, so results are not deterministic

<sub>no GPU · Needs Claude Code, Codex or another supported coding agent · Models: Claude Code, Codex, Devin CLI, OpenCode, Gemini · safety checks passed 10 of 11 · [Repo](https://github.com/dietrichgebert/ponytail) · [🌐 Site ↗](https://ponytail.dev/stories) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ponytail/)</sub>

<a name="spec-kit"></a>
### #&#8288;12 [spec-kit](https://github.com/github/spec-kit) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 142k · MIT · Oct 2026</sub>

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

<a name="archify"></a>
### #&#8288;13 [archify](https://github.com/tt-a1i/archify) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 87k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), Claude Code, Codex CLI, Cursor or OpenCode · safety checks passed 11 of 11 · [Repo](https://github.com/tt-a1i/archify) · [▶️ Demo ↗](https://archify.si/gallery.html) · [📖 Docs ↗](https://archify.si/guide.html) · [🌐 Site ↗](https://archify.si) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archify/)</sub>

<a name="repomix"></a>
### #&#8288;14 [repomix](https://github.com/yamadashy/repomix) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Node.js · Models: Model-agnostic: output is a file for Claude, ChatGPT, Gemini, Llama, Grok and others · safety checks passed 17 of 17 · [Repo](https://github.com/yamadashy/repomix) · [▶️ Demo ↗](https://repomix.com) · [🌐 Site ↗](https://repomix.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repomix/)</sub>

<a name="agentic-awesome-skills"></a>
### #&#8288;15 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · MIT · Oct 2026</sub>

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

<a name="compound-engineering-plugin"></a>
### #&#8288;16 [compound-engineering-plugin](https://github.com/everyinc/compound-engineering-plugin) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs An AI coding agent host (Claude Code, Cursor, Codex, etc.), pi-subagents (Pi only) · safety checks passed 11 of 12 · [Repo](https://github.com/everyinc/compound-engineering-plugin) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/compound-engineering-plugin/)</sub>

<a name="superpowers"></a>
### #&#8288;17 [superpowers](https://github.com/obra/superpowers) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 303k · MIT · Oct 2026</sub>

**Skill set that gives coding agents a spec, plan, TDD and review workflow.**

Superpowers is a set of composable skills plus a bootstrap instruction (using-superpowers) that makes a coding agent brainstorm a spec, create a git worktree, write a task plan, then run subagent-driven development with TDD and code review. It installs as a plugin or extension in many agent harnesses, including Claude Code, Codex, Cursor, Gemini CLI, Copilot CLI, OpenCode and Pi. Skills trigger automatically rather than by command.

- **+** Installs through native plugin commands in about 16 harnesses, including Claude Code, Codex and Cursor
- **+** Covers the full cycle: brainstorming, worktrees, plans, subagent execution, TDD, review, branch finishing
- **+** Skills trigger automatically, so no slash commands are needed in normal use
- **+** Includes a diagnosing-superpowers skill that reads session transcripts to explain misfires
- **−** Must be installed separately in each harness you use
- **−** Workflows are mandatory and opinionated; TDD deletes code written before tests
- **−** Maintainers generally do not accept contributions of new skills
- **−** Optional visual companion loads a vendor logo that reports version, unless disabled by env var

<sub>no GPU · Needs A supported coding agent (Claude Code, Codex, Cursor, Gemini CLI, etc.), git · safety checks passed 10 of 10 · [Repo](https://github.com/obra/superpowers) · [🌐 Site ↗](https://primeradiant.com/superpowers/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superpowers/)</sub>

<a name="rtk"></a>
### #&#8288;18 [rtk](https://github.com/rtk-ai/rtk) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 84k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Homebrew, winget or curl installer, A supported coding agent · safety checks passed 10 of 11 · [Repo](https://github.com/rtk-ai/rtk) · [📖 Docs ↗](https://www.rtk-ai.app/guide) · [🌐 Site ↗](https://www.rtk-ai.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rtk/)</sub>

<a name="claude-hud"></a>
### #&#8288;19 [claude-hud](https://github.com/jarrodwatts/claude-hud) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<a name="claude-skills"></a>
### #&#8288;20 [claude-skills](https://github.com/alirezarezvani/claude-skills) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Python 3, Claude Code or another supported coding agent · safety checks passed 8 of 11 · [Repo](https://github.com/alirezarezvani/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-skills/)</sub>

<a name="notebooklm-py"></a>
### #&#8288;21 [notebooklm-py](https://github.com/teng-lin/notebooklm-py) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Google account, Google NotebookLM / Gemini Notebook, Playwright Chromium (for browser login) · Models: Google Gemini (via NotebookLM) · safety checks passed 10 of 10 · [Repo](https://github.com/teng-lin/notebooklm-py) · [▶️ Demo ↗](https://asciinema.org/a/767284) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/notebooklm-py/)</sub>

<a name="kami"></a>
### #&#8288;22 [kami](https://github.com/tw93/kami) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Agent skill that renders styled PDF, PNG and PPTX documents from templates.**

Kami is a skill for coding agents (Claude Code, Codex, Cursor) that supplies layout rules and eight document templates: one-pager, long doc, letter, portfolio, resume, slides, equity report and changelog. It renders through WeasyPrint to PDF, with python-pptx for editable PowerPoint and a Marp variant for slides. It also includes a zero-dependency MCP server exposing render, check and screenshot tools.

- **+** Eight document templates plus a landing page system, in English, Chinese and Korean variants
- **+** Installs via npx skills, host plugin marketplaces, or a Claude Desktop zip
- **+** Includes a zero-dependency MCP server with render, check and screenshot tools
- **+** Structured content schemas and coverage checks run before final output
- **−** Windows requires WSL; helper scripts are Bash and WeasyPrint needs GTK/Pango
- **−** Default Chinese font TsangerJinKai02 is free for personal use only
- **−** Japanese and Korean get only font fallbacks and layout checks, not full support
- **−** Runs a daily version check against GitHub's latest release

<sub>no GPU · Needs WeasyPrint, python-pptx, Pygments (optional), Marp (optional), beautiful-mermaid (optional) · Models: Claude Code, Codex, Cursor · [Repo](https://github.com/tw93/kami) · [🌐 Site ↗](https://kami.tw93.fun) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kami/)</sub>

<a name="graphify"></a>
### #&#8288;23 [graphify](https://github.com/graphify-labs/graphify) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 131k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Python 3.10+, uv or pipx · Models: Claude, OpenAI-compatible, Gemini, Ollama, AWS Bedrock · safety checks passed 15 of 16 · [Repo](https://github.com/graphify-labs/graphify) · [📖 Docs ↗](https://docs.graphify.com) · [🌐 Site ↗](https://graphify.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphify/)</sub>

<a name="taste-skill"></a>
### #&#8288;24 [taste-skill](https://github.com/leonxlnx/taste-skill) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 100k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node 22+, Chrome, Edge or Chromium, Network access for image search · Models: Claude Code, Codex, Cursor · safety checks passed 10 of 11 · [Repo](https://github.com/leonxlnx/taste-skill) · [🌐 Site ↗](https://tasteskill.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taste-skill/)</sub>

<a name="openspec"></a>
### #&#8288;25 [openspec](https://github.com/fission-ai/openspec) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 73k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 20.19.0 or higher, A supported AI coding assistant · Models: Tool-agnostic; recommends Codex 5.5 and Opus 4.7 · safety checks passed 10 of 10 · [Repo](https://github.com/fission-ai/openspec) · [📖 Docs ↗](https://openspec.dev/docs) · [🌐 Site ↗](https://openspec.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openspec/)</sub>

<a name="planning-with-files"></a>
### #&#8288;26 [planning-with-files](https://github.com/othmanadi/planning-with-files) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Bash, Python 3.10+ (Qoder CLI), npx · safety checks passed 11 of 11 · [Repo](https://github.com/othmanadi/planning-with-files) · [📖 Docs ↗](https://github.com/OthmanAdi/planning-with-files/blob/master/docs/installation.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/planning-with-files/)</sub>

<a name="ai-memory"></a>
### #&#8288;27 [ai-memory](https://github.com/akitaonrails/ai-memory) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<a name="cc-switch"></a>
### #&#8288;28 [cc-switch](https://github.com/farion1231/cc-switch) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 147k · MIT · Oct 2026</sub>

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

<a name="bmad-method"></a>
### #&#8288;29 [bmad-method](https://github.com/bmad-code-org/bmad-method) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · custom license · Oct 2026</sub>

**Agile planning and delivery skills for AI coding tools.**

BMad Method installs a set of skills and agent workflows into your AI coding tool, covering clarification, planning, architecture, build, verification and retrospectives. Process depth scales with the change: small changes go straight to build, larger ones get planning documents that carry forward as context. Stable v6.12 installs via npx; the v7 preview alpha installs via the Skills CLI or Claude Code and Codex plugin marketplaces.

- **+** Process sizes to the change: direct build for small edits, deeper planning for large work
- **+** Works on new projects and on existing codebases
- **+** Official modules for builder, test architecture, game dev and unattended epic runs
- **+** Installs through npx, the Skills CLI, or Claude Code and Codex plugin marketplaces
- **−** V7 is preview alpha; README warns of breaking changes between updates
- **−** V7 requires an AI coding tool that supports skills
- **−** Needs uv and Python for setup and scripts, plus Node.js for the stable installer
- **−** Detected license is NOASSERTION while the README states MIT

<sub>no GPU · Needs uv, Node.js 20.12+, Python 3.10+, AI coding tool with skills support · [Repo](https://github.com/bmad-code-org/bmad-method) · [📖 Docs ↗](https://docs.bmad-method.org/start/build-your-first-change/) · [🌐 Site ↗](https://bmadcode.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bmad-method/)</sub>

<a name="gstack"></a>
### #&#8288;30 [gstack](https://github.com/garrytan/gstack) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 137k · MIT · Oct 2026</sub>

**Markdown slash-command skills that give Claude Code planning, review, QA and ship roles.**

gstack is a set of Markdown skills, exposed as slash commands such as /office-hours, /plan-ceo-review, /review, /qa, /cso and /ship, that split a coding session into roles: product, architecture, design, review, QA, security and release. Setup is a git clone into ~/.claude/skills plus a Bun-based ./setup script that also builds a bundled browser for QA. Claude Code is the full-tier host; Codex, OpenCode, Cursor, Kiro and others are experimental.

- **+** Claude Code is the only full-tier host; safety hooks like /careful and /freeze are enforced there
- **+** Skills are plain Markdown, so they can be forked and edited
- **+** Team mode auto-updates for shared repos with no vendored files
- **+** Installs for multiple agents (Codex, Cursor, OpenCode, Kiro, Copilot CLI) via --host flags
- **−** Non-Claude hosts are experimental or instruction-only, and safety skills only advise there
- **−** Outside reviews need a second CLI (Codex or Claude Code) installed and signed in
- **−** /cso needs a recent Bun with specific build flags plus a native C toolchain
- **−** README leads with the author's productivity claims, not behavior of the skills

<sub>no GPU · Needs Claude Code, Git, Bun 1.3.3+ (1.4.2 tested), Node.js (Windows only), Codex CLI (optional, outside reviews), OpenAI API key (optional, design binary) · Models: Claude (Opus 5.5), OpenAI GPT-6 Astra, OpenAI GPT-6.1 Sol, OpenAI gpt-5.5 and gpt-image-2 (design binary) · safety checks passed 10 of 10 · [Repo](https://github.com/garrytan/gstack) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gstack/)</sub>

<a name="reverse-skill"></a>
### #&#8288;31 [reverse-skill](https://github.com/zhaoxuya520/reverse-skill) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 43k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Java/JDK, Node.js 22.12+, Python 3.x, jadx, apktool, Frida, IDA Pro, radare2, Ghidra, Binary Ninja · safety checks passed 9 of 10 · [Repo](https://github.com/zhaoxuya520/reverse-skill) · [📖 Docs ↗](https://reverse.apivix.com/docs/) · [🌐 Site ↗](https://reverse.apivix.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reverse-skill/)</sub>

<a name="oh-my-codex"></a>
### #&#8288;32 [oh-my-codex](https://github.com/yeachan-heo/oh-my-codex) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 20+, OpenAI Codex CLI, tmux (macOS/Linux team runtime), git · Models: OpenAI Codex CLI models · safety checks passed 11 of 12 · [Repo](https://github.com/yeachan-heo/oh-my-codex) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-codex-website/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-codex/)</sub>

<a name="beads"></a>
### #&#8288;33 [beads](https://github.com/gastownhall/beads) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Dolt, git (optional) · safety checks passed 9 of 12 · [Repo](https://github.com/gastownhall/beads) · [📖 Docs ↗](https://beads.gascity.com/) · [🌐 Site ↗](https://beads.gascity.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beads/)</sub>

<a name="openwiki"></a>
### #&#8288;34 [openwiki](https://github.com/langchain-ai/openwiki) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 22.22.0 or newer, A coding agent or a model provider · Models: Fourteen providers, including hosted models, Local OpenAI-compatible endpoints · port 4321 · safety checks passed 10 of 10 · [Repo](https://github.com/langchain-ai/openwiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openwiki/)</sub>

<a name="waza"></a>
### #&#8288;35 [waza](https://github.com/tw93/waza) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

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

<a name="opencodex"></a>
### #&#8288;36 [opencodex](https://github.com/lidge-jun/opencodex) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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

<a name="diagram-design"></a>
### #&#8288;37 [diagram-design](https://github.com/cathrynlavery/diagram-design) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs An Agent Skills-compatible coding agent (Claude Code, Codex, Cursor, etc.), Node.js (npx) for the skills CLI install · Models: Any model running in the host agent · safety checks passed 11 of 11 · [Repo](https://github.com/cathrynlavery/diagram-design) · [▶️ Demo ↗](https://cathrynlavery.github.io/diagram-design/) · [🌐 Site ↗](https://diagramdesign.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diagram-design/)</sub>

<a name="vercel-labs-skills"></a>
### #&#8288;38 [skills](https://github.com/vercel-labs/skills) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

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

<a name="agents"></a>
### #&#8288;39 [agents](https://github.com/wshobson/agents) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

**Marketplace of coding-agent plugins, subagents, skills and commands for seven tools.**

A Markdown-sourced catalog of 94 plugins (202 agents, 185 skills, 105 commands) covering Python, JavaScript, code review, testing, infrastructure and security. It installs natively into Claude Code, Codex CLI and Cursor, and generates artifacts for OpenCode, Antigravity CLI, GitHub Copilot and Pi via make targets. Individual skills can be installed with gh skill or npx skills.

- **+** One Markdown source adapted to seven harnesses, with native marketplaces for Claude Code, Codex and Cursor
- **+** Large catalog: 94 plugins, 202 agents, 185 skills, 105 commands
- **+** Skills can be installed singly via gh skill or npx skills without cloning
- **+** Repo includes validation targets and a static skill scorer (plugin-eval) that needs no model calls
- **−** Feature support differs per harness; Pi agents need a separate subagent extension
- **−** OpenCode, Antigravity, Copilot and Pi installs require cloning, uv and Python 3.12+
- **−** plugin-eval LLM judge and Monte Carlo layers are experimental, not validated against human labels
- **−** Pensyve memory entry is external, and its hosted cloud closed on October 1, 2026

<sub>no GPU · Needs Claude Code, Codex CLI, Cursor, OpenCode, Antigravity CLI, GitHub Copilot or Pi, uv and Python 3.12+ (clone installs), GitHub CLI 2.90+ (gh skill), Node.js and npm (npx skills) · Models: opus, sonnet, haiku, fable, inherit · safety checks passed 10 of 11 · [Repo](https://github.com/wshobson/agents) · [📖 Docs ↗](https://github.com/wshobson/agents/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents/)</sub>

<a name="cc-haha"></a>
### #&#8288;40 [cc-haha](https://github.com/nanmicoder/cc-haha) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Bun, Electron, Model provider API key or account · Models: Claude, ChatGPT, Grok, DeepSeek, Kimi · safety checks passed 1 of 2 · [Repo](https://github.com/nanmicoder/cc-haha) · [📖 Docs ↗](https://cchaha.ai) · [🌐 Site ↗](https://cchaha.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-haha/)</sub>

<a name="plannotator"></a>
### #&#8288;41 [plannotator](https://github.com/backnotprop/plannotator) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="zcf"></a>
### #&#8288;42 [zcf](https://github.com/ufomiao/zcf) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Aug 2026</sub>

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

<a name="browser-harness"></a>
### #&#8288;43 [browser-harness](https://github.com/browser-use/browser-harness) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Chrome with remote debugging enabled, uv, Python 3.12 · Models: Claude Code, Codex, MCP clients · safety checks passed 15 of 17 · [Repo](https://github.com/browser-use/browser-harness) · [📖 Docs ↗](https://github.com/browser-use/browser-harness/blob/main/install.md) · [🌐 Site ↗](https://cloud.browser-use.com/v4) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browser-harness/)</sub>

<a name="jeffallan-claude-skills"></a>
### #&#8288;44 [claude-skills](https://github.com/jeffallan/claude-skills) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Atlassian MCP server (workflow commands only) · Models: Claude · safety checks passed 8 of 9 · [Repo](https://github.com/jeffallan/claude-skills) · [📖 Docs ↗](https://jeffallan.github.io/claude-skills) · [🌐 Site ↗](https://jeffallan.github.io/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jeffallan-claude-skills/)</sub>

<a name="worktrunk"></a>
### #&#8288;45 [worktrunk](https://github.com/max-sixty/worktrunk) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.4k · custom license · Oct 2026</sub>

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

<a name="ouroboros"></a>
### #&#8288;46 [ouroboros](https://github.com/q00/ouroboros) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · Oct 2026</sub>

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

<a name="claude-code-router"></a>
### #&#8288;47 [claude-code-router](https://github.com/musistudio/claude-code-router) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 22+ for CLI, Docker (optional) · Models: OpenAI Chat/Responses, Anthropic Messages, Gemini, OpenRouter, DeepSeek · port 3458 · safety checks passed 3 of 5 · [Repo](https://github.com/musistudio/claude-code-router) · [📖 Docs ↗](https://ccrdesk.top/en/guides/install/) · [🌐 Site ↗](https://ccrdesk.top/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-router/)</sub>

<a name="lifeos"></a>
### #&#8288;48 [lifeos](https://github.com/danielmiessler/lifeos) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Sep 2026</sub>

**Personal context, memory and skills layer for AI coding harnesses.**

LifeOS installs as a single skill bundle on top of an AI coding harness, adding persistent memory, personal context files (goals, contacts, preferences), skill routing and hooks. It is written in TypeScript and Bash, runs on bun, and is most tested on Claude Code. Install is done by prompting your AI to read the install page, or with a curl shell script on macOS/Linux.

- **+** Installer merges settings and leaves your USER/ customizations untouched on upgrade
- **+** Bundles a skill library covering research, security, writing and art
- **+** Built on hooks, skills and context files, not one vendor's features
- **+** Docs site and walkthrough video available
- **−** Needs a capable AI coding harness; Claude Code is the only well-tested path
- **−** Local model support (Ollama, llama.cpp) is still on the roadmap
- **−** Install is delegated to an AI agent or a curl-piped shell script
- **−** Public repo is generated from a private tree; PRs are ported, not merged

<sub>no GPU · Needs bun, Claude Code or another AI coding harness · Models: Claude Code, Cursor, Codex, Hermes · [Repo](https://github.com/danielmiessler/lifeos) · [📖 Docs ↗](https://docs.ourlifeos.ai) · [🌐 Site ↗](https://ourlifeos.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lifeos/)</sub>

<a name="oh-my-opencode-slim"></a>
### #&#8288;49 [oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · MIT · Oct 2026</sub>

**Multi-agent orchestration plugin for OpenCode with per-agent model routing.**

A plugin for OpenCode that adds an Orchestrator agent plus specialists (Explorer, Oracle, Council, Designer, Fixer). The Orchestrator plans work, dispatches specialists as background tasks, and reconciles their results. Each agent can use a different model, set through presets in ~/.config/opencode/oh-my-opencode-slim.json, with project-local overrides.

- **+** Per-agent model and variant config, with presets that can extend a base preset
- **+** Project-local overrides for prompts, custom agents and delegation rules
- **+** Optional tmux, Zellij, kitty or WezTerm panes to watch background agents live
- **+** Council agent runs several models in parallel and synthesizes one answer
- **−** Works only inside OpenCode; not a standalone tool
- **−** Council is the highest-cost path and triggers only when requested
- **−** Bundled example presets go stale as model lineups change, per the README
- **−** Requires provider logins and manual model selection per agent

<sub>no GPU · Needs OpenCode, Bun or Node.js, LLM provider accounts · Models: OpenAI, OpenCode Go, Claude (via ACP), any provider OpenCode supports · [Repo](https://github.com/alvinunreal/oh-my-opencode-slim) · [📖 Docs ↗](https://github.com/alvinunreal/oh-my-opencode-slim/blob/master/docs/configuration.md) · [🌐 Site ↗](https://boringdystopia.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-opencode-slim/)</sub>

<a name="mattpocock-skills-zh-cn"></a>
### #&#8288;50 [mattpocock-skills-zh-cn](https://github.com/vinvcn/mattpocock-skills-zh-cn) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · MIT · Oct 2026</sub>

**Simplified Chinese translation of Matt Pocock's engineering agent skills collection.**

Third-party zh-CN localization of mattpocock/skills, a set of small agent skills for grilling interviews, TDD, bug diagnosis, spec and ticket writing, code review and codebase architecture review. Install with `npx skills@latest add`, as a Claude Code plugin, or as a DeepSeek Harness plugin invoked via `/zh-<name>`. Upstream is synced periodically, with translations done by Codex and reviewed by the maintainer.

- **+** Skills are small, editable files that can be copied into your repo via skills.sh
- **+** Works with Claude Code, Codex and other Agent Skills-compatible harnesses
- **+** Covers a full flow: grill, spec, tickets, implement with TDD, code review
- **+** Directory names, commands and identifiers stay unchanged, so installs match upstream
- **−** Unofficial fork; content depends on periodic syncs from upstream
- **−** Translations are machine-produced by Codex, with human review only on PRs
- **−** Needs a one-time /setup-matt-pocock-skills run per repo for tracker and labels
- **−** No native Codex plugin; plugin install is read-only, so customizing requires skills.sh copy

<sub>no GPU · Needs Node.js (npx skills), Claude Code, Codex or another Agent Skills harness, GitHub or Linear issue tracker (optional, local files also supported) · Models: Any model (harness-agnostic) · [Repo](https://github.com/vinvcn/mattpocock-skills-zh-cn) · [🌐 Site ↗](https://skills.sh/vinvcn/mattpocock-skills-zh-CN) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mattpocock-skills-zh-cn/)</sub>

<a name="claude-octopus"></a>
### #&#8288;51 [claude-octopus](https://github.com/nyldn/claude-octopus) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Oct 2026</sub>

**Claude Code plugin for multi-model review, debate and research workflows.**

Claude Octopus is a plugin for Claude Code that adds /octo:* commands, skills and personas, which dispatch work to up to twelve external providers such as Codex, Copilot, Ollama, Perplexity and OpenRouter. A 75% consensus gate flags disagreements between models. Workflows include Double Diamond phases, a multi-LLM council and parallel git worktrees. It stays dormant until you run a command explicitly.

- **+** Works with Claude alone; external providers are added one at a time when detected
- **+** Dormant until a /octo:* command is run, so ordinary prompts are not routed
- **+** Consensus gate and council modes compare several models' opinions before shipping
- **+** Also installs for Codex CLI, and for Cursor as an MCP server
- **−** Requires Claude Code v2.1.14+; Windows needs WSL or SSH, Git Bash unsupported
- **−** Some providers need paid subscriptions or API keys; Qwen free OAuth tier ended
- **−** Large surface (54 commands, 63 skills, 31 personas) takes time to learn
- **−** Optional auto-router in invoke mode can send prompt context to external providers

<sub>no GPU · Needs Claude Code v2.1.14+, Python 3 (optional, provider history), Node.js/npm (Cursor MCP server) · Models: Claude, Codex, Antigravity CLI, Copilot, Qwen · [Repo](https://github.com/nyldn/claude-octopus) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-octopus/)</sub>

<a name="i-have-adhd"></a>
### #&#8288;52 [i-have-adhd](https://github.com/ayghri/i-have-adhd) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 58k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code or compatible coding assistant · safety checks passed 10 of 11 · [Repo](https://github.com/ayghri/i-have-adhd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/i-have-adhd/)</sub>

<a name="claude-code-templates"></a>
### #&#8288;53 [claude-code-templates](https://github.com/davila7/claude-code-templates) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

**Installable agents, commands, hooks, MCPs and skills for Claude Code.**

A catalog of Claude Code add-ons (agents, slash commands, settings, hooks, MCP configs and skills) installed through an npx CLI or browsed on aitmpl.com. The CLI also ships a session analytics view, a mobile-oriented conversation monitor with optional Cloudflare Tunnel access, a health check and a plugin dashboard. Some components are bundled from other repositories under their original licenses.

- **+** One npx command installs agents, commands, hooks, settings or MCPs into a project
- **+** Covers six component types, including skills and MCP integrations, in one catalog
- **+** Web catalog at aitmpl.com plus a separate documentation site
- **+** MIT license; bundled third-party components keep their original licenses
- **−** Targets Claude Code only; no other coding agents are mentioned
- **−** Component quality likely varies because many are imported from other repos
- **−** README gives no versioning or update policy for installed templates
- **−** Requires Node.js via npx; minimum version unknown

<sub>no GPU · Needs Node.js (npx), Claude Code, Cloudflare Tunnel (optional, for remote chat monitor) · safety checks passed 7 of 12 · [Repo](https://github.com/davila7/claude-code-templates) · [📖 Docs ↗](https://docs.aitmpl.com) · [🌐 Site ↗](https://aitmpl.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-templates/)</sub>

<a name="claude-video"></a>
### #&#8288;54 [claude-video](https://github.com/bradautomates/claude-video) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Sep 2026</sub>

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

<sub>RAM ≥ 8 GB · GPU optional · Needs Python 3.10+, FFmpeg, yt-dlp, Deno (YouTube), WhisperX 3.8.6 (optional), Node.js (Skills CLI install only) · Models: Gemini (gemini-3.7-flash default), WhisperX, Groq whisper-large-v3, OpenAI whisper-1 · safety checks passed 9 of 10 · [Repo](https://github.com/bradautomates/claude-video) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-video/)</sub>

<a name="visual-explainer"></a>
### #&#8288;55 [visual-explainer](https://github.com/nicobailon/visual-explainer) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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
### #&#8288;56 [drawio-skill](https://github.com/agents365-ai/drawio-skill) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

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

<a name="tech-leads-club-agent-skills"></a>
### #&#8288;57 [agent-skills](https://github.com/tech-leads-club/agent-skills) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · custom license · Oct 2026</sub>

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

<a name="loopx"></a>
### #&#8288;58 [loopx](https://github.com/loopx-project/loopx) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · Apache-2.0 · Oct 2026</sub>

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

<a name="claude-howto"></a>
### #&#8288;59 [claude-howto](https://github.com/luongnv89/claude-howto) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Node.js (npx for MCP server examples), uv (optional, EPUB build script) · Models: Claude Opus, Claude Sonnet, Claude Haiku · safety checks passed 11 of 11 · [Repo](https://github.com/luongnv89/claude-howto) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-howto/)</sub>

<a name="video-shotcraft"></a>
### #&#8288;60 [video-shotcraft](https://github.com/vincentwei1021/video-shotcraft) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js and npm, Remotion, ffmpeg / ffprobe, uv (BGM beat analysis only), puppeteer (page capture only) · Models: Claude Code, Codex · safety checks passed 10 of 11 · [Repo](https://github.com/vincentwei1021/video-shotcraft) · [▶️ Demo ↗](https://vincentwei1021.github.io/video-shotcraft/) · [📖 Docs ↗](https://github.com/Vincentwei1021/video-shotcraft/blob/main/references/pipeline.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/video-shotcraft/)</sub>

<a name="gsd-core"></a>
### #&#8288;61 [gsd-core](https://github.com/open-gsd/gsd-core) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<a name="superpowers-zh"></a>
### #&#8288;62 [superpowers-zh](https://github.com/jnmetacode/superpowers-zh) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Oct 2026</sub>

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

<a name="aidlc-workflows"></a>
### #&#8288;63 [aidlc-workflows](https://github.com/awslabs/aidlc-workflows) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT-0 · Oct 2026</sub>

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
### #&#8288;64 [oh-my-hermes](https://github.com/rlaope/oh-my-hermes) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

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

<a name="claude-code-game-studios"></a>
### #&#8288;65 [claude-code-game-studios](https://github.com/donchitos/claude-code-game-studios) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Git, Python 3, Bash, jq (recommended) · Models: Claude (Opus, Sonnet, or session model) · safety checks passed 9 of 9 · [Repo](https://github.com/donchitos/claude-code-game-studios) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-game-studios/)</sub>

<a name="awesome-claude-code-subagents"></a>
### #&#8288;66 [awesome-claude-code-subagents](https://github.com/voltagent/awesome-claude-code-subagents) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, curl (standalone installer) · Models: Claude · safety checks passed 8 of 10 · [Repo](https://github.com/voltagent/awesome-claude-code-subagents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-claude-code-subagents/)</sub>

<a name="img2threejs"></a>
### #&#8288;67 [img2threejs](https://github.com/img2threejs/img2threejs) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · Apache-2.0 · Oct 2026</sub>

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

<a name="gentle-ai"></a>
### #&#8288;68 [gentle-ai](https://github.com/gentleman-programming/gentle-ai) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · MIT · Oct 2026</sub>

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

<a name="obsidian-mind"></a>
### #&#8288;69 [obsidian-mind](https://github.com/breferrari/obsidian-mind) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="agency-agents"></a>
### #&#8288;70 [agency-agents](https://github.com/msitarzewski/agency-agents) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 163k · MIT · Oct 2026</sub>

**Markdown agent persona files for Claude Code, Cursor, Codex and other coding tools.**

A collection of role-based agent definition files (engineering, design and other divisions), each describing a specialist's identity, workflow, code deliverables and success metrics. Shell scripts (convert.sh, install.sh) generate and install them for Claude Code, Cursor, Gemini CLI, OpenCode, Copilot, Aider, Windsurf, Codex and others, with per-division or per-agent selection. A separate desktop app handles browsing and install.

- **+** Installer supports about 14 tools, with --division and --agent filters and a --dry-run mode
- **+** Plain markdown files can be copied or adapted individually without running any scripts
- **+** Large roster: roughly 60 engineering agents alone, plus design and other divisions
- **+** MIT license; runbook roster JSON lists agent teams that install directly by slug
- **−** Prompt files only; no runtime, so output quality depends on the host tool and model
- **−** OpenCode registers only about 119 agents, so a full install loses the rest
- **−** No tagged releases in this repo; the desktop app is a separate project
- **−** Persona-style prompts with no benchmarks or tests shown for the claimed outcomes

<sub>no GPU · Needs bash, python3 (optional, for runbook roster extraction) · Models: Claude Code, Cursor, Codex, Gemini CLI, OpenCode · safety checks passed 9 of 9 · [Repo](https://github.com/msitarzewski/agency-agents) · [🌐 Site ↗](https://agencyagents.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents/)</sub>

<a name="claude-code-best-practice"></a>
### #&#8288;71 [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 68k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code · Models: Claude · safety checks passed 8 of 9 · [Repo](https://github.com/shanraisshan/claude-code-best-practice) · [📖 Docs ↗](https://code.claude.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-best-practice/)</sub>

<a name="huashu-design"></a>
### #&#8288;72 [huashu-design](https://github.com/alchaincyf/huashu-design) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js, Playwright, ffmpeg, Python · Models: Claude Code, Cursor, Codex, OpenClaw, Hermes · safety checks passed 8 of 9 · [Repo](https://github.com/alchaincyf/huashu-design) · [▶️ Demo ↗](https://www.huasheng.ai/parrots/) · [🌐 Site ↗](https://www.huasheng.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huashu-design/)</sub>

<a name="auto-claude-code-research-in-sleep"></a>
### #&#8288;73 [auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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

<sub>Needs Claude Code or another supported agent host, codex-cli (default reviewer), Python · Models: Claude Opus 5, Claude Fable 5.1, GPT-6-Astra, ModelScope-hosted models, DeepSeek · safety checks passed 10 of 11 · [Repo](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) · [📖 Docs ↗](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep/blob/main/AGENT_GUIDE.md) · [🌐 Site ↗](https://wanshuiyin.github.io/Auto-claude-code-research-in-sleep/ARIS_INTRO.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auto-claude-code-research-in-sleep/)</sub>

<a name="android-skills"></a>
### #&#8288;74 [skills](https://github.com/android/skills) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · Apache-2.0 · Oct 2026</sub>

**Official Android development skills for AI coding agents, in SKILL.md format.**

A set of SKILL.md files from the Android team that give coding agents task-specific instructions for Android development, such as R8 analysis and Wear Compose M3. They target areas where evaluations show LLMs underperform, not basics like Jetpack Compose. Installed with the Android CLI (`android skills add`) or as a Claude Code or Codex plugin.

- **+** Maintained by Android, grounded in developer.android.com guidance
- **+** Follows the open agent skills standard (SKILL.md), so it works across agents
- **+** Installs via Android CLI, or as a Claude Code or Codex plugin marketplace entry
- **+** Targets workflows where evaluations show LLMs underperform
- **−** Public contributions are not accepted; changes go through GitHub issues only
- **−** Does not cover well-established areas such as basic Jetpack Compose practices
- **−** README does not list the full set of skills available
- **−** README disclaims that AI output can be wrong and needs review

<sub>no GPU · Needs Android CLI · Models: Claude Code, Codex, Gemini, Antigravity · [Repo](https://github.com/android/skills) · [📖 Docs ↗](https://developer.android.com/tools/agents/android-cli) · [🌐 Site ↗](https://developer.android.com/tools/agents/android-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/android-skills/)</sub>

<a name="universal-modder"></a>
### #&#8288;75 [universal-modder](https://github.com/rehan-remade/universal-modder) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · MIT · Oct 2026</sub>

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

<a name="mirrord"></a>
### #&#8288;76 [mirrord](https://github.com/metalbear-co/mirrord) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="context-mode"></a>
### #&#8288;77 [context-mode](https://github.com/mksglu/context-mode) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · custom license · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js >= 22.5 or Bun · Models: Claude Code, Gemini CLI, VS Code Copilot, JetBrains Copilot, GitHub Copilot CLI · safety checks passed 12 of 17 · [Repo](https://github.com/mksglu/context-mode) · [🌐 Site ↗](https://context-mode.com/insight) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-mode/)</sub>

<a name="anti-slop"></a>
### #&#8288;78 [anti-slop](https://github.com/miqdadbadjuber/anti-slop) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · MIT · Oct 2026</sub>

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

<a name="lean-ctx"></a>
### #&#8288;79 [lean-ctx](https://github.com/yvgude/lean-ctx) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="understand-anything"></a>
### #&#8288;80 [understand-anything](https://github.com/egonex-ai/understand-anything) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 87k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code or another supported agent platform, Node.js >= 18 (standalone viewer), pnpm (building from source) · Models: Whatever the host platform uses, Local models via Ollama · port 5173 · safety checks passed 10 of 12 · [Repo](https://github.com/egonex-ai/understand-anything) · [▶️ Demo ↗](https://understand-anything.com/demo/) · [🌐 Site ↗](https://understand-anything.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/understand-anything/)</sub>

<a name="anatomy"></a>
### #&#8288;81 [anatomy](https://github.com/wheresryan22/anatomy) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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
### #&#8288;82 [codex-with-chatgpt](https://github.com/xiaoduoya/codex-with-chatgpt) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Oct 2026</sub>

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

<a name="oracle"></a>
### #&#8288;83 [oracle](https://github.com/steipete/oracle) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Oct 2026</sub>

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

<a name="skillshare"></a>
### #&#8288;84 [skillshare](https://github.com/runkids/skillshare) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

**CLI that syncs skills, agents, rules, MCP and hooks across AI coding tools.**

skillshare keeps skills (SKILL.md), agents, rules, MCP connections, hooks and plugins in one source directory and syncs them to Claude Code, Codex, Pi, OpenCode, OpenClaw and other tools, using symlinks or copies. It installs from any Git host, audits skills before use, and supports per-project setups committed with the code. It ships as a single Go binary with a web dashboard (`skillshare ui`) and a separate desktop app.

- **+** Single Go binary with no Node.js or npm runtime dependency
- **+** One source syncs skills, agents, extras, MCP and hooks to many tools
- **+** Built-in `audit` command, with auto-scan on install and update
- **+** Project mode keeps skills in `.skillshare/` committed with the repo
- **−** Windows file symlinks need Developer Mode, otherwise files are copied
- **−** Plugins sync separately from `sync --all`
- **−** Desktop app is a separate repo; macOS build is Apple Silicon only
- **−** Supported tool list is only partly named in the README (`and more`)

<sub>no GPU · Docker + Compose · Needs Git · [Repo](https://github.com/runkids/skillshare) · [📖 Docs ↗](https://skillshare.runkids.cc/docs) · [🌐 Site ↗](https://skillshare.runkids.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skillshare/)</sub>

<a name="trellis"></a>
### #&#8288;85 [trellis](https://github.com/mindfold-ai/trellis) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · AGPL-3.0 · Sep 2026</sub>

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

<sub>no GPU · Needs Node.js >= 18, Python >= 3.9 · safety checks passed 1 of 2 · [Repo](https://github.com/mindfold-ai/trellis) · [📖 Docs ↗](https://docs.trytrellis.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trellis/)</sub>

<a name="jakubkrehel-skills"></a>
### #&#8288;86 [skills](https://github.com/jakubkrehel/skills) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.1k · MIT · Oct 2026</sub>

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
### #&#8288;87 [pxpipe](https://github.com/teamchong/pxpipe) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.5k · MIT · Oct 2026</sub>

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

<a name="peon-ping"></a>
### #&#8288;88 [peon-ping](https://github.com/peonping/peon-ping) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

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

<a name="agentskills"></a>
### #&#8288;89 [agentskills](https://github.com/agentskills/agentskills) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Aug 2026</sub>

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

<sub>no GPU · safety checks passed 7 of 8 · [Repo](https://github.com/agentskills/agentskills) · [📖 Docs ↗](https://agentskills.io/specification) · [🌐 Site ↗](https://agentskills.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentskills/)</sub>

<a name="agency-agents-zh"></a>
### #&#8288;90 [agency-agents-zh](https://github.com/jnmetacode/agency-agents-zh) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

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

<a name="codex-keysmith"></a>
### #&#8288;91 [codex-keysmith](https://github.com/jia-ethan/codex-keysmith) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Sep 2026</sub>

**Installer that adds a reversible custom instruction set to local Codex.**

A single-file Python script that installs an instruction prompt into a local Codex config directory (e.g. ~/.codex), so new Codex sessions follow it. It shows a dry-run plan first and writes only with --yes, and it offers --status, --restore-hooks, --uninstall and --reactivate. Per the README it does not modify Codex itself or read account credentials.

- **+** Preview first; nothing is written until --yes is passed
- **+** Uninstall and restore commands, also preview-first
- **+** Release scripts ship with SHA256SUMS for checksum verification
- **+** Single Python file, needs only Python 3.10+
- **−** Affects only new Codex sessions; old tasks must be closed
- **−** Windows fresh deployment is still a beta channel
- **−** Desktop builds are unsigned and trigger Gatekeeper or SmartScreen
- **−** Main README is in Chinese; English version is a separate file

<sub>no GPU · Needs Python 3.10+, Codex installed locally · [Repo](https://github.com/jia-ethan/codex-keysmith) · [📖 Docs ↗](https://github.com/Jia-Ethan/codex-keysmith/blob/main/docs/reference.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-keysmith/)</sub>

<a name="tweakcc"></a>
### #&#8288;92 [tweakcc](https://github.com/piebald-ai/tweakcc) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

**CLI that patches Claude Code to customize prompts, themes, and UI.**

tweakcc patches Claude Code's minified cli.js, or the native Bun binary via node-lief, using settings from ~/.tweakcc/config.json. It edits system prompts, themes, thinking verbs and spinners, toolsets and subagent models, and adds patches such as AGENTS.md support and MCP startup optimization. Customizations are reapplied with `npx tweakcc --apply` after Claude Code updates, and custom patches can be written through an API or `adhoc-patch`.

- **+** Supports native binaries and npm, pnpm, bun, Homebrew and Nix installs on Windows, macOS, Linux
- **+** Config in ~/.tweakcc/config.json is reapplied with --apply; a SessionStart hook can automate it
- **+** Custom patches via npm API or sandboxed `adhoc-patch` scripts, including from an HTTP URL
- **+** Restores from backup before each apply; `--restore` reverts Claude Code
- **−** Verified only against Claude Code 2.1.162; other versions may break non-prompt patches
- **−** Claude Code updates overwrite patches, and native updates can replace the patched binary
- **−** Patches depend on the internal layout of a third-party minified binary
- **−** README says documentation for some features is still missing

<sub>no GPU · Needs Claude Code, Node.js · Models: Claude (via Claude Code) · [Repo](https://github.com/piebald-ai/tweakcc) · [🌐 Site ↗](https://piebald.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tweakcc/)</sub>

<a name="agent-skills-for-context-engineering"></a>
### #&#8288;93 [agent-skills-for-context-engineering](https://github.com/muratcankoylan/agent-skills-for-context-engineering) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Cursor, Codex or another Agent Skills host · Models: Model-agnostic; router benchmarked on gemini-3.1-pro, composer-2, gpt-5.5, claude-opus-4-7 · safety checks passed 9 of 10 · [Repo](https://github.com/muratcankoylan/agent-skills-for-context-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills-for-context-engineering/)</sub>

<a name="loop-engineering"></a>
### #&#8288;94 [loop-engineering](https://github.com/cobusgreyling/loop-engineering) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), GitHub, A coding agent CLI (Claude Code, Grok, Codex or Opencode) · Models: Claude Code, Grok, Codex, Opencode, OpenClaw · safety checks passed 11 of 11 · [Repo](https://github.com/cobusgreyling/loop-engineering) · [📖 Docs ↗](https://github.com/cobusgreyling/loop-engineering/blob/main/docs/QUICKSTART.md) · [🌐 Site ↗](https://cobusgreyling.github.io/loop-engineering/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loop-engineering/)</sub>

<a name="softwarecopyright-skill"></a>
### #&#8288;95 [softwarecopyright-skill](https://github.com/fokkyp/softwarecopyright-skill) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

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

<a name="ccg-workflow"></a>
### #&#8288;96 [ccg-workflow](https://github.com/fengshao1227/ccg-workflow) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

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
### #&#8288;97 [observal](https://github.com/observal/observal) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · Apache-2.0 · Oct 2026</sub>

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

<a name="answer-me-with-html"></a>
### #&#8288;98 [answer-me-with-html](https://github.com/qingyuna/answer-me-with-html) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Oct 2026</sub>

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

<a name="claude-code-harness"></a>
### #&#8288;99 [claude-code-harness](https://github.com/chachamaru127/claude-code-harness) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Plan, work and review skills for Claude Code, Codex CLI, Cursor and Grok.**

A skill and plugin set that adds a plan, work, review, sync and release workflow to coding assistants. It keeps the spec and tasks in spec.md and Plans.md, runs checks, and requests a review separate from the implementation. A Go-native guardrail engine blocks operations such as secret reads, production deploys and forced pushes to main.

- **+** Plan and task state lives in spec.md and Plans.md inside the project
- **+** Supported install paths for Claude Code, Codex CLI, Cursor and Grok
- **+** Guardrail engine is bundled Go binaries, no Node.js needed at runtime
- **+** Resumable work via /harness-work --resume latest
- **−** Guardrails do not guarantee containment; coverage differs per tool
- **−** Cursor has no filesystem isolation; restrictions are applied only by Harness
- **−** Codex child agents can inherit parent permissions
- **−** More workers, reviews and retries raise costs on your model provider

<sub>no GPU · Needs Claude Code v2.1+, Codex CLI, Cursor or Grok, Git, Go 1.26.0+ (only to build from source) · Models: Claude Code, Codex CLI, Cursor, Grok · [Repo](https://github.com/chachamaru127/claude-code-harness) · [📖 Docs ↗](https://github.com/Chachamaru127/claude-code-harness/blob/main/docs/onboarding/index.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-harness/)</sub>

<a name="superclaude-framework"></a>
### #&#8288;100 [superclaude_framework](https://github.com/superclaude-org/superclaude_framework) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (79) · Freshness: active (97) · Maintenance: patchy (30) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Claude Code, pipx, Tavily MCP (optional), Context7 MCP (optional), Serena MCP (optional), Playwright MCP (optional) · Models: Claude (via Claude Code) · safety checks passed 11 of 11 · [Repo](https://github.com/superclaude-org/superclaude_framework) · [🌐 Site ↗](https://superclaude.netlify.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superclaude-framework/)</sub>

<a name="memu"></a>
### #&#8288;101 [memu](https://github.com/nevamind-ai/memu) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (72) · Freshness: active (97) · Maintenance: fair (56) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

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

<a name="ag-kit"></a>
### #&#8288;102 [ag-kit](https://github.com/vudovn/ag-kit) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Aug 2026</sub>

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

<a name="skills-manager"></a>
### #&#8288;103 [skills-manager](https://github.com/xingkongliang/skills-manager) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.6k · MIT · Oct 2026</sub>

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

<a name="cc-skills-golang"></a>
### #&#8288;104 [cc-skills-golang](https://github.com/samber/cc-skills-golang) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

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

<a name="dashi-taskboard"></a>
### #&#8288;105 [dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · Apache-2.0 · Oct 2026</sub>

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

<a name="git-ai"></a>
### #&#8288;106 [git-ai](https://github.com/git-ai-project/git-ai) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · Apache-2.0 · Oct 2026</sub>

**Git extension that records which agent, model and prompt wrote each line.**

Git AI is a Rust git extension that stores line-level AI attribution in Git Notes, linking each AI-written line to the agent, model and session. Coding agents report their edits through `git-ai checkpoint`, so no heuristics are used. It adds `git ai blame` and `git ai stats`, and carries attribution through rebase, squash, stash and cherry-pick.

- **+** No git hooks and no git wrapping, so git commands are not slowed
- **+** Attribution comes from agent reports, not AI-detection heuristics
- **+** Preserves attribution across rebase, cherry-pick, stash, squash and amend
- **+** Works locally and offline with no login; editor plugins exist for VS Code and Emacs
- **−** `git mv`, `git filter-branch`/`filter-repo` and `git replace` are not tracked
- **−** Squash/rebase merges on hosting platforms need CI Actions or the paid Teams product
- **−** Secure prompt store and org-wide stats are in the Teams version, not the CLI
- **−** Bash-created files may be missed if the agent is not run from the repo root

<sub>no GPU · Needs git · Models: Claude Code, Codex, Cursor, GitHub Copilot, OpenCode · [Repo](https://github.com/git-ai-project/git-ai) · [📖 Docs ↗](https://usegitai.com/docs/cli/how-git-ai-works) · [🌐 Site ↗](https://usegitai.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/git-ai/)</sub>

<a name="trailofbits-skills"></a>
### #&#8288;107 [skills](https://github.com/trailofbits/skills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · CC-BY-SA-4.0 · Oct 2026</sub>

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
### #&#8288;108 [n8n-skills](https://github.com/czlonkowski/n8n-skills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

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
### #&#8288;109 [agents-cli](https://github.com/google/agents-cli) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · Apache-2.0 · Oct 2026</sub>

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

<a name="dotnet-skills"></a>
### #&#8288;110 [skills](https://github.com/dotnet/skills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.7k · MIT · Oct 2026</sub>

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

<a name="apm"></a>
### #&#8288;111 [apm](https://github.com/microsoft/apm) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Oct 2026</sub>

**Dependency manager for agent skills, plugins, instructions and MCP servers.**

APM reads an apm.yml manifest and installs agent primitives (instructions, skills, prompts, hooks, plugins, MCP servers) from git hosts into the config formats of Copilot, Claude, Cursor, Codex, Gemini, Windsurf, OpenCode, Kiro and Grok Build. It resolves transitive dependencies, pins them in a lockfile with content hashes, and scans installs for hidden Unicode. An apm-policy.yml lets an org restrict allowed sources and primitives.

- **+** One apm.yml and lockfile reproduce the same setup across nine listed agent clients
- **+** Resolves transitive dependencies from GitHub, GitLab, Bitbucket, Azure DevOps and any git host
- **+** Install-time hidden Unicode scan, lockfile hashes, CycloneDX/SPDX SBOM export
- **+** Org policy file with tighten-only inheritance and apm audit for CI gates
- **−** Governs what gets installed only; does not control what the agent runs
- **−** Native release binaries listed for x86_64 only; other platforms need pip
- **−** Value depends on third-party packages and marketplaces being available and trustworthy
- **−** Two named maintainers listed in the README

<sub>no GPU · Needs git, Python 3.10+ (pip install only) · [Repo](https://github.com/microsoft/apm) · [📖 Docs ↗](https://microsoft.github.io/apm/quickstart/) · [🌐 Site ↗](https://microsoft.github.io/apm/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/apm/)</sub>

<a name="cc-sdd"></a>
### #&#8288;112 [cc-sdd](https://github.com/gotalab/cc-sdd) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Sep 2026</sub>

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

<a name="native-subtitle-quote-image"></a>
### #&#8288;113 [native-subtitle-quote-image](https://github.com/chengyi-ai/native-subtitle-quote-image) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**Agent skill that stitches video frames and subtitle strips into long images.**

An Agent Skill (Codex, Claude Code, other Agent Skills hosts) plus a Python CLI that samples exact frames from a local video or YouTube URL and composes a JPG with one hero frame and up to 6 subtitle strips. Native mode crops burned-in subtitles from the pixels without redrawing; script mode draws reviewed lines from a JSON file and labels them as post-production.

- **+** Native mode crops burned-in subtitles from pixels, with no OCR or redrawing
- **+** CLI subcommands (check-source, sample, band, render, render-script) run without an agent
- **+** Rejects duplicate frames and low-resolution or broken streams before rendering
- **+** Fixed 3:4 canvas or natural-ratio layout; Chinese, English and Korean examples
- **−** Native mode needs burned-in subtitles; toggleable caption tracks give clean frames
- **−** Script mode needs a CJK font for Chinese, Japanese or Korean lines
- **−** Maximum 7 timestamps per image: 1 hero frame and 6 strips
- **−** URL mode needs yt-dlp plus Deno or Node.js, and may need browser cookies

<sub>no GPU · Needs Python 3.10+, Pillow, imageio-ffmpeg or FFmpeg, yt-dlp (URL mode), Deno or Node.js (YouTube), CJK font (script mode) · [Repo](https://github.com/chengyi-ai/native-subtitle-quote-image) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/native-subtitle-quote-image/)</sub>

<a name="claude-plugins-official"></a>
### #&#8288;114 [claude-plugins-official](https://github.com/anthropics/claude-plugins-official) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code · safety checks passed 8 of 11 · [Repo](https://github.com/anthropics/claude-plugins-official) · [📖 Docs ↗](https://code.claude.com/docs/en/plugins) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-plugins-official/)</sub>

<a name="brag"></a>
### #&#8288;115 [brag](https://github.com/latent-spaces/brag) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

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

<sub>Needs Node.js 22+, FFmpeg, Hyperframes CLI · Models: Claude Opus 5.5 (/brag-slim) · safety checks passed 9 of 10 · [Repo](https://github.com/latent-spaces/brag) · [▶️ Demo ↗](https://letsbrag.app) · [🌐 Site ↗](https://latent-spaces.github.io/brag/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/brag/)</sub>

<a name="autoresearch"></a>
### #&#8288;116 [autoresearch](https://github.com/uditgoenka/autoresearch) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.7k · MIT · Aug 2026</sub>

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

<a name="lazycodex"></a>
### #&#8288;117 [lazycodex](https://github.com/code-yeongyu/lazycodex) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

**OmO agent harness packaged as a plugin for OpenAI Codex.**

LazyCodex installs the oh-my-openagent (OmO) harness into Codex through an npx installer or the Codex plugin marketplace. It adds the $init-deep, $ulw-plan, $start-work and $ulw-loop commands, skills, hooks and sub-agent roles in ~/.codex/agents/. It also routes subtasks to different GPT models by task category.

- **+** Installs with one npx command; uninstall and a doctor health check are included
- **+** Plan, execute, verify workflow: plans go to plans/<slug>.md, loops capped at 100 or 500 iterations
- **+** Generates hierarchical AGENTS.md project memory with $init-deep
- **+** Hooks run only after approval in Codex's startup review
- **−** Codex marketplace install is labeled experimental; npx is the primary path
- **−** Core engine is a git submodule of oh-my-openagent, so this is a thin wrapper
- **−** README documents only OpenAI GPT model routing
- **−** Sub-agent roles rely on Codex spawn_agent; falls back to prompt text without agent_type

<sub>no GPU · Needs Codex CLI, Node.js (npx), OpenAI models · Models: gpt-5.2, gpt-5.3-codex, gpt-5.4-mini, gpt-5.5 · [Repo](https://github.com/code-yeongyu/lazycodex) · [📖 Docs ↗](https://lazycodex.ai/docs) · [🌐 Site ↗](https://lazycodex.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lazycodex/)</sub>

<a name="avdlee-swiftui-agent-skill"></a>
### #&#8288;118 [swiftui-agent-skill](https://github.com/avdlee/swiftui-agent-skill) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="ripwire"></a>
### #&#8288;119 [ripwire](https://github.com/redhat-et/ripwire) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Oct 2026</sub>

**Code-context CLI giving coding agents a ranked call graph and edit checks.**

ripwire is a single C++23 binary that indexes a repository into a deterministic, ranked call graph and answers orientation questions (`ripwire .`, `--for`, `--callers`, `--path`, `--recall`). On edits it reports blast radius, tests that reach the change, and quality regressions via `--edit-check` and `--quality-delta`. The installer also writes skills for agents such as Claude Code, Codex, Cursor, Windsurf, Gemini, opencode and aider; an MCP server is optional.

- **+** Single offline binary with no runtime dependencies, API key, embeddings or daemon
- **+** Indexes this repo in 0.25 s using 6.6 MB, per its own benchmark
- **+** Answers disclose truncation, label floors, and give a next= to recover cut rows
- **+** Covers about 25 languages and installs skills for seven agent CLIs in one line
- **−** Benchmarks and the field report are the authors' own, not independent measurements
- **−** Contract checker arity heuristic over-counts on defaulted trailing parameters
- **−** Plain grep can still win on broad, common-word conceptual queries
- **−** MCP server schemas consume agent context every session; CLI is the preferred route

<sub>no GPU · [Repo](https://github.com/redhat-et/ripwire) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ripwire/)</sub>

<a name="design-md"></a>
### #&#8288;120 [design.md](https://github.com/google-labs-code/design.md) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Oct 2026</sub>

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

<a name="google-skills"></a>
### #&#8288;121 [skills](https://github.com/google/skills) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), Google Cloud account for most skills · safety checks passed 10 of 11 · [Repo](https://github.com/google/skills) · [🌐 Site ↗](https://skills.sh/google/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-skills/)</sub>

<a name="dsh-routing-suite"></a>
### #&#8288;122 [dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · MIT · Sep 2026</sub>

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

<a name="one-skill-to-rule-them-all"></a>
### #&#8288;123 [one-skill-to-rule-them-all](https://github.com/rebelytics/one-skill-to-rule-them-all) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · CC-BY-4.0 · Oct 2026</sub>

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

<a name="lint"></a>
### #&#8288;124 [lint](https://github.com/shadcn-ui/lint) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**ESLint and Oxlint rules that enforce Tailwind design systems with fix guidance for agents.**

@shadcn/lint is a lint plugin for ESLint 9.30+ and Oxlint 1.80+ that checks Tailwind v4 class usage in React, Vue and Svelte. Rules cover restyling components via className, raw colors, arbitrary values, inline styles, unknown classes and dynamic class strings. Errors suggest fixes from your components, variants and theme, and can be customised with per-component contracts and message placeholders.

- **+** Error messages name allowed sizes, variants and theme file, drawn from your own components
- **+** Per-component contracts (allow/deny patterns) without changing component code
- **+** Runs on both ESLint and Oxlint across React, Vue and Svelte
- **+** Works without shadcn/ui via componentImports settings
- **−** Tailwind v4 only
- **−** Oxlint reads only script blocks in Vue and Svelte files, not templates or markup
- **−** Variants from typed props are resolved in React only
- **−** Eval results come from the authors' own runs; independent numbers unknown

<sub>no GPU · Needs Node.js 20.19+, ESLint 9.30+ or Oxlint 1.80+, Tailwind v4 · [Repo](https://github.com/shadcn-ui/lint) · [📖 Docs ↗](https://github.com/shadcn-ui/lint/blob/main/docs/rules.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/lint/)</sub>

<a name="pstack-claude"></a>
### #&#8288;125 [pstack-claude](https://github.com/michael-denyer/pstack-claude) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Skill stack that routes coding-agent tasks through planning, delegation and verification.**

Port of Lauren Tan's Cursor pstack skill set to Claude Code, Codex, Pi, GitHub Copilot, Muse and other harnesses. A session-start hook points the agent at poteto-mode, which picks a playbook (bug fix, feature, refactor, performance, PR maintenance) and delegates with skills like architect, arena, swarm, how and why. It also has a formal-verification skill for concurrency invariants that tests miss.

- **+** Installs as a plugin on Claude Code, Codex, Copilot and Muse; Pi via git install
- **+** Routing hook sends tasks to poteto-mode automatically at session start
- **+** No server or telemetry; scripts run locally, PR tools use your GitHub CLI login
- **+** Per-role model and reasoning-effort settings via setup-pstack
- **−** Harnesses without hooks (OpenCode, Gemini CLI) need manual symlinks and a named skill call
- **−** Codex and Muse run the hook only after you trust or approve it
- **−** Copilot build tested only on CLI 1.0.87 to 1.0.92; copilot -p lists no skills on 1.0.92
- **−** Anything the skills read, including transcripts, is sent to your model provider

<sub>no GPU · Needs Claude Code 2.1.292 or later (Claude Code install), GitHub CLI (PR tools) · Models: Claude, Codex, GitHub Copilot models · [Repo](https://github.com/michael-denyer/pstack-claude) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pstack-claude/)</sub>

<a name="jevgrep"></a>
### #&#8288;126 [jevgrep](https://github.com/dzhng/jevgrep) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

**CLI that answers repo questions with files and source excerpts for coding agents.**

jg takes a natural-language question about a repository and prints relevant files, reading leads and verbatim source excerpts with line references to stdout. It uses the Jev model, called through a provider key, to judge relevance across folders, files and declarations. A bundled skill, installed with `jg skill`, teaches coding agents such as Claude Code, Codex and OpenCode to call it.

- **+** Installs an agent skill for Claude Code, Codex and OpenCode with one command
- **+** Respects ignore files and skips hidden, binary and .env files by default
- **+** No Python, Bun or ripgrep install needed; runs on Node 22+
- **+** Published eval: 8/10 SWE-bench tasks solved with and without it, Sol cost down 28.6%
- **−** Source content is sent to the chosen provider; secret filtering is heuristic, not redaction
- **−** Needs a provider key for Vercel AI Gateway, TypeSafe, OpenRouter or OpenCode Zen
- **−** Benchmark covers ten Python tasks; total cost including Jev fell 25.8%, no speed gain claimed
- **−** Declaration parsing covers only Python, TS/JS, Go and Rust; other text uses a fallback

<sub>no GPU · Needs Node.js 22+, API key for Vercel AI Gateway, TypeSafe, OpenRouter or OpenCode Zen · Models: Jev · [Repo](https://github.com/dzhng/jevgrep) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jevgrep/)</sub>

<a name="claude-blog"></a>
### #&#8288;127 [claude-blog](https://github.com/agricidaniel/claude-blog) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Claude Code skill suite for writing, auditing and localizing SEO blog posts.**

A Claude Code plugin with one orchestrator and 31 sub-skills behind 30 /blog commands, covering writing, rewriting, SEO and AI-citation audits, topic clusters, translation and audio narration. Each draft must pass a 5-gate delivery contract (100-point rubric, 90 minimum, up to 3 iterations) and ships as markdown, HTML, PDF, hero image, screenshots and a review report.

- **+** Code-enforced delivery gates check format, screenshots, review score and links before output
- **+** Broad command set: write, rewrite, factcheck, cannibalization, decay detection, multilingual with hreflang
- **+** Outputs markdown, HTML, PDF, hero image and review.md from a single source
- **+** Supports Next.js MDX, Astro, Hugo, Jekyll, WordPress, Ghost, 11ty, Gatsby, static HTML
- **−** Requires Claude Code; tested only on 2.1.296, with 2.1.69 as the oldest justified version
- **−** Hero images, audio and Google data need extra APIs or MCPs (Gemini, stock APIs, Google)
- **−** AI citation score is a non-calibrated heuristic, not a measured citation rate
- **−** Large surface (32 skill dirs, 22 scripts) takes time to learn and audit

<sub>no GPU · Needs Claude Code, Python 3.11+, patchright or playwright, Gemini API (images, TTS), Banana MCP, Google APIs, NotebookLM · Models: Claude (via Claude Code), Gemini (images and TTS) · [Repo](https://github.com/agricidaniel/claude-blog) · [🌐 Site ↗](https://agricidaniel.com/blog/claude-code-blog-writer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-blog/)</sub>

<a name="ffmpeg-skill"></a>
### #&#8288;128 [ffmpeg-skill](https://github.com/kajisho5/ffmpeg-skill) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Agent Skill and MCP server that edits video with local FFmpeg.**

Installs as a skill for Claude Code, Cursor or Codex, and also runs as an MCP server over stdio. It gives the agent 42 Python scripts wrapping ffmpeg and ffprobe for cutting, joining, captions, loudness, reframing and platform exports. The workflow is probe, edit (stream copy where possible), then check and look at a contact sheet. No cloud or API keys are needed.

- **+** Every tool supports --dry-run, --json and --plan, so edits can be previewed before rendering
- **+** Runs offline on Python standard library; only ffmpeg and python3 are required
- **+** Contract-derived MCP schema; CI tests FFmpeg 5.1, 6.1, 7.1, 8 and 9
- **+** Stream-copies cuts and joins where possible; never overwrites input files
- **−** Makes no editorial decisions; no face, subject or highlight detection, only measured proxies
- **−** Visual verification depends on the calling agent having vision
- **−** Some tools need specific FFmpeg builds; Homebrew ffmpeg lacks the subtitles filter for caption.py
- **−** Transcription needs a separate speech engine such as Parakeet or whisper installed

<sub>GPU optional · Needs ffmpeg, ffprobe, python3, Node.js (npx installer), optional speech engine (Parakeet, whisper) · [Repo](https://github.com/kajisho5/ffmpeg-skill) · [📖 Docs ↗](https://github.com/kajisho5/ffmpeg-skill/blob/main/docs/demos.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ffmpeg-skill/)</sub>

<a name="claude-code-local"></a>
### #&#8288;129 [claude-code-local](https://github.com/nicedreamzapp/claude-code-local) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="stop-that-shit"></a>
### #&#8288;130 [stop-that-shit](https://github.com/lennney/stop-that-shit) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**Skill and guard that stop coding agents from scope creep and needless defensive code.**

Stop That Shit is a skill plus a tool-call guard for coding agents (Codex, Claude Code, OpenCode, Hermes Agent CLI, Pi, Oh My Pi). The skill sets rules against scope creep, unused hashing, read-only violations and repeated work. The guard blocks writes in review/answer/monitor modes, writes outside files=, new dependencies, extra subagents and recognizable hash operations unless allowed with flags like deps=allow or hash=allow.

- **+** Per-task contract with modes (review, answer, monitor, change, watch) and files=, deps=, hash=, agents= flags
- **+** Covers six agent hosts, each with install steps, plus a skill-only option
- **+** Guard checks are narrow and documented: writes, dependencies, subagents, hashes, paths
- **+** Ships 18 public Bad/Good cases and an evidence file with paired runs
- **−** Guard stays inactive until a mode is used; default state is OBSERVING / unconfirmed
- **−** A deny response does not prove the host skipped the action; isolation is left to the host sandbox
- **−** Hash detection covers only recognizable operations; other over-engineering relies on skill judgment
- **−** Main README is Chinese; English and Korean versions are separate files

<sub>no GPU · Needs Node.js 18+, Node.js 22.19+ (Pi 0.84.4) · Models: Codex, Claude Code, OpenCode 1.18.18+, Hermes Agent CLI, Pi Coding Agent 0.84.4 · [Repo](https://github.com/lennney/stop-that-shit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/stop-that-shit/)</sub>

<a name="autoharness"></a>
### #&#8288;131 [autoharness](https://github.com/tigerless-labs/autoharness) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Python 3.11+ · Models: Claude · safety checks passed 9 of 10 · [Repo](https://github.com/tigerless-labs/autoharness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autoharness/)</sub>

<a name="claude-scholar"></a>
### #&#8288;132 [claude-scholar](https://github.com/galaxy-dawn/claude-scholar) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (50) · Freshness: active (95) · Maintenance: fair (62) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

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

<a name="potpie"></a>
### #&#8288;133 [potpie](https://github.com/potpie-ai/potpie) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.7k · Apache-2.0 · Oct 2026</sub>

**CLI that builds a context graph of your codebase for coding agents.**

Potpie is a Python CLI with a local daemon that indexes code, source history, issues and docs into a context graph. A setup wizard installs Potpie skills and instructions into coding harnesses (Claude Code, OpenAI Codex, Cursor, OpenCode), which then query the graph with commands like `potpie resolve` and `potpie search`. A local web UI explores the graph.

- **+** One setup wizard installs skills for Claude Code, Codex, Cursor and OpenCode
- **+** Indexes GitHub, Linear, Jira and Confluence, not only source code
- **+** Local graph explorer UI opened with `potpie ui`
- **+** Installs from PyPI with uv or pip; no manual ingest step needed
- **−** README gives no RAM, GPU, database or model requirements
- **−** Only four coding harnesses and four integrations supported so far
- **−** `potpie login` enables account-backed or managed features; free scope unclear
- **−** No Docker or compose setup; relies on a local daemon

<sub>Needs GitHub, Linear, Jira, Confluence · [Repo](https://github.com/potpie-ai/potpie) · [📖 Docs ↗](https://docs.potpie.ai) · [🌐 Site ↗](https://potpie.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/potpie/)</sub>

<a name="vibe-skills"></a>
### #&#8288;134 [vibe-skills](https://github.com/foryourhealth111-pixel/vibe-skills) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="token-optimizer"></a>
### #&#8288;135 [token-optimizer](https://github.com/alexgreensh/token-optimizer) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · custom license · Oct 2026</sub>

**Plugin that trims wasted context and keeps state across compaction in coding agents.**

Token Optimizer is a hook-based plugin for Claude Code, Codex, OpenCode, Cursor, Copilot and other coding assistants. It compresses command and search output, shows file re-reads as diffs or skeletons, checkpoints before auto-compact and restores afterward, and audits configs, skills and memory files. A local SQLite database feeds a dashboard with quality scores and dollar savings.

- **+** Covers bash, search, JSON, file re-reads and large results, plus config and memory audits
- **+** Checkpoints before compaction and restores after, so work survives auto-compact
- **+** Zero dependencies, no telemetry, no MCP server; data stays in local SQLite
- **+** Installs on Claude Code, Codex, OpenCode, OpenClaw, Hermes, Copilot, Cursor and Pi
- **−** PolyForm Noncommercial license restricts commercial use; not an OSI open-source license
- **−** Antigravity, Grok and Devin support is beta or contract-only
- **−** Claude Code cloud sessions load no plugins and need a separate setup script
- **−** Comparisons against Headroom and RTK are the author's own claims

<sub>no GPU · Needs Python 3.9+, SQLite · [Repo](https://github.com/alexgreensh/token-optimizer) · [📖 Docs ↗](https://alexgreensh.github.io/token-optimizer/) · [🌐 Site ↗](https://token-optimizer.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/token-optimizer/)</sub>

<a name="better-harness"></a>
### #&#8288;136 [better-harness](https://github.com/qoderai/better-harness) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Plugin that audits a coding-agent workflow and reports evidence-backed findings.**

Better Harness is a plugin and skill, run as /better-harness inside a coding agent. It collects project and session evidence, evaluates five Agent Work Loop dimensions, and writes findings with scoped repair plans and acceptance checks. Output is a self-contained report.html with report.md and findings.json, or a host-native Canvas in Qoder and Cursor. Missing evidence is marked explicitly rather than scored.

- **+** Supports Claude Code, Codex, Qoder, Cursor, Copilot CLI, Qwen Code, Pi, Kimi Code, WorkBuddy, Grok
- **+** Each finding links to evidence, expected output, repair boundary and acceptance checks
- **+** Unobserved behavior stays explicit instead of becoming an unsupported score
- **+** Public sample report and Harness Inspector demo; MIT licensed
- **−** No single entrypoint: install and invocation steps differ per host
- **−** Cursor plugin is not published; install plan is reported as unavailable
- **−** Copilot records no per-response token usage; VS Code Copilot Chat has no durable transcript
- **−** Plugin lifecycle CLI is marked Beta; history shows trends, not causal proof

<sub>no GPU · Needs Node.js >=22.20.0 <25 (source builds), npm >=10.9.3 <12 (source builds), A supported coding agent host · Models: Depends on the host coding agent · [Repo](https://github.com/qoderai/better-harness) · [▶️ Demo ↗](https://qoderai.github.io/better-harness/demo/better-harness-report/) · [📖 Docs ↗](https://qoderai.github.io/better-harness/docs/introduction) · [🌐 Site ↗](https://qoderai.github.io/better-harness/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/better-harness/)</sub>

<a name="unity-skills"></a>
### #&#8288;137 [unity-skills](https://github.com/besty0728/unity-skills) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Unity Editor plugin exposing 839 REST skills for AI coding agents to drive scenes.**

A Unity package (2022.3+) that runs a REST server inside the Editor and ships a skills template for Claude Code, Codex, Cursor, Antigravity, OpenCode and Kimi Code. Agents call endpoints to edit scenes, prefabs, materials, scripts and packages. It adds Approval/Auto/Bypass permission modes, dry-run previews, a JSONL audit log and transactional batches with rollback.

- **+** 839 skills across 54 categories, including Cinemachine, ProBuilder, Netcode, XR and YooAsset
- **+** Three permission modes, per-skill allowlist, and JSONL audit log at Library/UnitySkillsAudit.jsonl
- **+** POST /skills/batch runs as a transaction with rollback; ?mode=dryRun previews changes without writing
- **+** One-click installers for six agent tools from the Unity panel; installs via UPM Git URL
- **−** Unity-only; 2022.3+ and Unity 6 are the maintained baseline
- **−** Domain Reload or compilation makes the REST server briefly unavailable; retries needed
- **−** Comparison table against other tools is self-reported from a 2026-07 survey
- **−** Large skill surface; advisory modules and routing add context load for agents

<sub>no GPU · Needs Unity 2022.3+, An AI coding agent (Claude Code, Codex, Cursor, Antigravity, OpenCode or Kimi Code) · [Repo](https://github.com/besty0728/unity-skills) · [📖 Docs ↗](https://deepwiki.com/Besty0728/Unity-Skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unity-skills/)</sub>

<a name="pg-aiguide"></a>
### #&#8288;138 [pg-aiguide](https://github.com/timescale/pg-aiguide) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

**Postgres skills and doc-search MCP server for AI coding agents.**

pg-aiguide gives coding agents PostgreSQL guidance on schema design, indexing, data types, constraints and naming. It also offers a hosted MCP server with semantic and BM25 search over the PostgreSQL, TimescaleDB and PostGIS docs. It installs as Agent Skills via `npx skills`, as an MCP endpoint, or as a Claude Code plugin.

- **+** Three install paths: npx skills, MCP URL, or Claude Code plugin
- **+** Search is version-aware for the PostgreSQL manual and also covers TimescaleDB and PostGIS
- **+** Hosted MCP endpoint means no local server is needed to start
- **+** Config snippets for Cursor, Codex, Gemini CLI, VS Code, OpenCode and Windsurf
- **−** Docs search depends on a public endpoint hosted by TigerData
- **−** pgvector docs are listed as coming soon
- **−** Quality claims (4x constraints, 55% more indexes) come from a single demo prompt
- **−** Skills are opinionated; the README does not say how to customize them

<sub>no GPU · Docker + Compose · Needs Node.js (for npx skills), TigerData-hosted MCP server (mcp.tigerdata.com/docs) · [Repo](https://github.com/timescale/pg-aiguide) · [📖 Docs ↗](https://mcp.tigerdata.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pg-aiguide/)</sub>

<a name="trail-code"></a>
### #&#8288;139 [trail-code](https://github.com/trailhq/trail-code) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<a name="memsearch"></a>
### #&#8288;140 [memsearch](https://github.com/zilliztech/memsearch) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

**Persistent semantic memory for Claude Code, Codex, OpenClaw and OpenCode agents.**

memsearch captures each agent conversation turn as an LLM-written summary in daily Markdown files, then indexes them in Milvus with hybrid search (dense vector, BM25, RRF). Plugins exist for Claude Code, Codex, DeepSeek Harness, OpenClaw and OpenCode, and a CLI and Python API allow use in custom agents. Recall runs in three layers: search, expand, then raw transcript.

- **+** Markdown files are the source of truth; the Milvus index is rebuildable
- **+** One memory shared across five agent platforms
- **+** Default local ONNX bge-m3 embeddings need no API key; Milvus Lite needs no setup
- **+** Also exposes a CLI and Python API for custom agents
- **−** First run downloads a ~558 MB embedding model from HuggingFace
- **−** Capture summaries call an LLM on every turn, adding model usage
- **−** Codex install needs `codex --yolo` for ONNX network access
- **−** Team use needs a separate Milvus server or Zilliz Cloud

<sub>no GPU · Needs Milvus (Lite by default), HuggingFace Hub (model download), Python >=3.10 · Models: ONNX bge-m3, OpenAI embeddings, Ollama · [Repo](https://github.com/zilliztech/memsearch) · [📖 Docs ↗](https://zilliztech.github.io/memsearch/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/memsearch/)</sub>

<a name="prompt-master"></a>
### #&#8288;141 [prompt-master](https://github.com/nidhinjs/prompt-master) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

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
### #&#8288;142 [awesome-codex-subagents](https://github.com/voltagent/awesome-codex-subagents) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Oct 2026</sub>

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

<a name="teaql-agent-kit"></a>
### #&#8288;143 [teaql-agent-kit](https://github.com/teaql/teaql-agent-kit) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Sep 2026</sub>

**Agent skill that makes coding agents model, generate and verify TeaQL apps.**

An Agent Skill (build-teaql-app) that coding agents such as Claude Code, Codex, Cursor, Copilot or Gemini CLI follow to build apps model-first. The agent writes a domain model, has a TeaQL service evaluate and repair it, generates a typed library with Q query and E expression APIs, then implements and verifies the app. The README's example uses Rust and SQLite and ends with a work-complete.md evidence report.

- **+** Works with several existing coding agents through one pasted prompt
- **+** Deterministic model evaluation with repair guidance runs before application code is written
- **+** Generated typed Q/E APIs; runtime logs SQL and audit context with query purpose and comment
- **+** Requires a work-complete.md report citing build, test and runtime log evidence
- **−** Default workflow needs network access; model content is sent to TeaQL services
- **−** Evaluation, generation and Assist use hosted services, so the workflow is not offline
- **−** Ties the application to the TeaQL runtime and generated library
- **−** README gives no measured token savings; the context benefit is stated as an aim

<sub>no GPU · Needs TeaQL evaluation and generation services, Coding agent with file and terminal access, Language toolchain for the target app (e.g. Rust) · Models: Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI · [Repo](https://github.com/teaql/teaql-agent-kit) · [▶️ Demo ↗](https://github.com/teaql/robot-task-board) · [🌐 Site ↗](https://teaql.io/blog/robot-task-board-showcase/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/teaql-agent-kit/)</sub>

<a name="garden-skills"></a>
### #&#8288;144 [garden-skills](https://github.com/conardli/garden-skills) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), OpenAI-compatible image API (gpt-image-2), MiniMax mmx-cli or OpenAI TTS (optional) · Models: GPT Image 2, OpenAI-compatible image APIs · safety checks passed 9 of 10 · [Repo](https://github.com/conardli/garden-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/garden-skills/)</sub>

<a name="vibe-coding-prompt-template"></a>
### #&#8288;145 [vibe-coding-prompt-template](https://github.com/khazp/vibe-coding-prompt-template) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

**Four-prompt workflow from app idea to PRD, tech design and agent files.**

Four copy-paste prompts for a chat model: research the idea, write an MVP PRD, choose a tech approach, then generate AGENTS.md, MEMORY.md and a review checklist for a coding assistant. Each step saves a markdown document with a Handoff Context so a fresh chat can continue. An optional npx vibeworkflow CLI and Claude Code skills scaffold the same files.

- **+** Prompts are self-contained; no install or CLI required to use them
- **+** Handoff Context in each document lets you switch chats or tools between steps
- **+** Part 4 emits AGENTS.md, MEMORY.md and tool files such as CLAUDE.md or Cursor rules
- **+** Includes a worked Reading List example and a larger Reddit to AI example
- **−** Output quality depends on the chat model you run the prompts in
- **−** Research step needs a chat tool with browsing, otherwise findings stay unverified
- **−** Produces planning documents, not application code
- **−** Manual copy, answer and save loop across five steps

<sub>no GPU · Needs Chat model (ChatGPT, Claude or Gemini), AI coding assistant (Cursor, Claude Code or VS Code), Node.js for optional npx vibeworkflow CLI · Models: Claude, Gemini, ChatGPT · [Repo](https://github.com/khazp/vibe-coding-prompt-template) · [🌐 Site ↗](https://vibeworkflow.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-coding-prompt-template/)</sub>

<a name="aiox-core"></a>
### #&#8288;146 [aiox-core](https://github.com/synkraai/aiox-core) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · custom license · Aug 2026</sub>

**Role-based agent personas and workflows for Claude Code, Codex and Gemini CLI.**

AIOX is an npm CLI (`npx aiox-core init` or `install`) that writes role-based agents (analyst, pm, architect, sm, dev, qa and others) and workflows into a project. It configures Claude Code, Codex CLI, Gemini CLI, Cursor and Copilot with rules, skills and hooks. Planning agents produce PRD and architecture docs, and the sm agent turns them into story files for the dev agent.

- **+** One npx command installs agents and config; `doctor` checks setup and `--dry-run` previews changes
- **+** Story files carry PRD and architecture context from planning agents to the dev agent
- **+** Sync and validation scripts for Claude Code, Codex CLI and Gemini CLI
- **+** Updates keep `.bak` copies of locally modified files
- **−** Full hook automation only in Claude Code; Cursor and Copilot lack equivalent lifecycle hooks
- **−** License detected as NOASSERTION, though the README badge says MIT
- **−** Main README is in Portuguese; English is a separate translated file
- **−** No model runtime of its own; needs a supported IDE or CLI

<sub>no GPU · Compose · Needs Node.js >=18 (v20+ recommended), npm >=9, Claude Code, Codex CLI, Gemini CLI, Cursor or Copilot, GitHub CLI (optional) · [Repo](https://github.com/synkraai/aiox-core) · [📖 Docs ↗](https://aioxsquad.ai) · [🌐 Site ↗](https://aioxsquad.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aiox-core/)</sub>

<a name="open-vibe-island"></a>
### #&#8288;147 [open-vibe-island](https://github.com/octane0411/open-vibe-island) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · GPL-3.0 · Oct 2026</sub>

**Native macOS notch overlay that tracks and approves coding agent sessions.**

Open Island is a SwiftUI and AppKit menu bar and notch app that shows live status for local coding agents, handles permission prompts, and jumps back to the right terminal or IDE. Agents report through hooks or plugins that forward JSON over a Unix socket to an in-app bridge. It lists 15 agents, including Claude Code, Codex, Cursor, Gemini CLI and OpenCode, and runs without a server or account.

- **+** Covers 15 agents, including Claude Code, Codex, Cursor, Gemini CLI, Kimi CLI and OpenCode
- **+** Hooks fail open, so agents keep running if the app is not open
- **+** Jump-back works with Ghostty, iTerm2, tmux, Zellij, WezTerm, Warp and JetBrains IDEs
- **+** Distributed as notarized DMG or Homebrew cask, with Sparkle auto-update
- **−** macOS 14+ only; building from source needs Swift 6.2 and Xcode
- **−** Grok Build and Gemini CLI events are observation-only, with no permission round-trip
- **−** Codex default install omits PreToolUse and PostToolUse; file-edit approval is not guaranteed
- **−** Claude Desktop usage panel only updates after a terminal claude session seeds the cache

<sub>no GPU · Needs macOS 14+, Swift 6.2 and Xcode (source builds) · [Repo](https://github.com/octane0411/open-vibe-island) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/open-vibe-island/)</sub>

<a name="hallmark"></a>
### #&#8288;148 [hallmark](https://github.com/nutlope/hallmark) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: weak (21) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Aug 2026</sub>

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

<a name="agents-md"></a>
### #&#8288;149 [agents.md](https://github.com/agentsmd/agents.md) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Sep 2026</sub>

**Open Markdown format for giving coding agents project instructions.**

AGENTS.md is a specification for a plain Markdown file kept in a repo that holds dev environment, testing and PR instructions for AI coding agents. The repository also contains the Next.js site served at agents.md, which explains the format and lists examples. It has no runtime or agent code.

- **+** Plain Markdown, no tooling, schema or dependencies required
- **+** One predictable file location for agent instructions, separate from the human README
- **+** Website runs locally with pnpm install and pnpm run dev
- **−** No enforced schema; README shows only a minimal example
- **−** Repo holds the website and spec, not a tool or agent
- **−** README does not list which agents read the file
- **−** No releases published

<sub>no GPU · Needs Node.js, pnpm · port 3000 · [Repo](https://github.com/agentsmd/agents.md) · [🌐 Site ↗](https://agents.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents-md/)</sub>

<a name="expo-skills"></a>
### #&#8288;150 [skills](https://github.com/expo/skills) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**Official Expo skills that teach coding agents Expo, EAS and React Native workflows.**

A set of SKILL.md packages from the Expo team covering Expo Router, animation, native UI, SDK upgrades, native modules, and EAS build, update, hosting and workflow tasks. It installs as a Claude Code or Codex plugin, or through the skills CLI for Cursor, OpenCode, Copilot, Windsurf and others. The Claude Code and Codex plugin also bundles the Expo MCP server configuration.

- **+** Maintained by the Expo team, with Expo docs and CLIs named as the source of truth
- **+** Installs via marketplace plugin for Claude Code and Codex, or the skills CLI for other agents
- **+** Skills are split into open-source framework and paid EAS groups, with cost notes
- **+** Plugin bundles Expo MCP config for live docs, EAS builds and simulator screenshots
- **−** Only useful for Expo and React Native projects
- **−** Several skills (eas-*) target paid EAS services
- **−** Experimental skills ship in a separate expo-experiments plugin and may change or be retired
- **−** Telemetry exists, opt-in and Claude Code only, and adds a setting to manage

<sub>no GPU · Needs Node.js (npx), Expo CLI, EAS CLI, Expo MCP server (optional) · [Repo](https://github.com/expo/skills) · [📖 Docs ↗](https://docs.expo.dev/skills/) · [🌐 Site ↗](https://skills.sh/expo/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/expo-skills/)</sub>

<a name="ruler"></a>
### #&#8288;151 [ruler](https://github.com/intellectronica/ruler) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**CLI that syncs one set of Markdown rules to many coding agents' config files.**

Ruler reads Markdown rules from a `.ruler/` directory and writes them into the native instruction files of about 30 coding agents, such as AGENTS.md, CLAUDE.md, .clinerules and .goosehints. It also propagates MCP server settings and skills, supports nested `.ruler/` directories for monorepos, and manages .gitignore entries. A `revert` command restores files from .bak backups.

- **+** Covers about 30 agents including Copilot, Claude Code, Cursor, Codex CLI, Gemini CLI and Aider
- **+** Single .ruler/ source with ruler.toml for per-agent selection and output paths
- **+** revert restores originals from .bak backups; --dry-run previews changes
- **+** Also distributes MCP server config and skills, not just rule text
- **−** README labels it a Beta Research Preview and asks users to test carefully
- **−** Nested rule loading is marked experimental and may change
- **−** Subagents support is experimental and disabled by default
- **−** Requires Node.js ^20.19.0, ^22.12.0 or >=23

<sub>no GPU · Needs Node.js ^20.19.0 || ^22.12.0 || >=23 · [Repo](https://github.com/intellectronica/ruler) · [🌐 Site ↗](https://www.npmjs.com/package/@intellectronica/ruler) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruler/)</sub>

<a name="supabase-agent-skills"></a>
### #&#8288;152 [agent-skills](https://github.com/supabase/agent-skills) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**Agent Skills that teach coding agents Supabase and Postgres practices.**

Two Agent Skills in the agentskills.io format: one covering Supabase Database, Auth, Edge Functions, Realtime, Storage, the CLI and the MCP server, and a Postgres performance skill with guidance across 8 prioritized categories. Install with `npx skills add supabase/agent-skills` or as Claude Code plugins. The README lists 18+ compatible agents, including Claude Code, Copilot, Cursor and Cline.

- **+** Works across 18+ agents via the open Agent Skills format, not tied to one tool
- **+** Install all skills or one with a single npx command
- **+** Postgres skill ranks guidance by impact, from Critical to Low, across 8 categories
- **+** Also ships as Claude Code plugins through a marketplace
- **−** Only two skills, both specific to Supabase and Postgres
- **−** Agent decides when to use a skill; README gives no way to force it
- **−** No benchmarks or measured accuracy gains in the README
- **−** Skill contents are not described in detail beyond topic lists

<sub>no GPU · Needs Node.js (npx), a compatible AI coding agent · [Repo](https://github.com/supabase/agent-skills) · [📖 Docs ↗](https://supabase.com/docs/guides/getting-started/ai-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/supabase-agent-skills/)</sub>

<a name="yomiyasu"></a>
### #&#8288;153 [yomiyasu](https://github.com/nanaism/yomiyasu) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Agent skill that rewrites AI-generated Japanese into plain, readable prose.**

yomiyasu is a skill for Claude Code, Codex, Cursor and similar agents that edits Japanese text written by AI. It fixes figurative verbs, unclear subject-predicate relations and needless decoration in technical articles, specs, PR descriptions and internal reports, while keeping the original meaning. It bundles Python scripts for linting and diffing the text before and after editing.

- **+** Bundled lint, diff and check scripts flag changed numbers, negations and swapped particles; stdlib-only Python
- **+** Installs via npx skills, gh skill, openskills, Claude Code plugin, or a ZIP for Claude.ai
- **+** 12 document types and 3 reader levels, so normal conventions such as minutes bullets are kept
- **+** Rules forbid adding facts absent from the source; unresolved points go back to the writer as questions
- **−** Japanese text only; the README is mainly in Japanese with a short English version
- **−** Only used when named in the request or via a standing instruction line
- **−** Scripts match fixed patterns and do not judge meaning or readability
- **−** Interactive mode, Windows, Cursor, Codex Cloud and Claude.ai ZIP are untested

<sub>no GPU · Needs Python 3.9+ (optional check scripts), Claude Code, Codex or another skill-capable agent · Models: Claude Code, Codex, Cursor, Claude.ai · [Repo](https://github.com/nanaism/yomiyasu) · [📖 Docs ↗](https://github.com/nanaism/yomiyasu/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/yomiyasu/)</sub>

<a name="security-audit-skill"></a>
### #&#8288;154 [security-audit-skill](https://github.com/cloudflare/security-audit-skill) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Node.js, Skills CLI (npx skills), coding agent with parallel sub-agents, OS-enforced sandbox · Models: any tool-use model with parallel sub-agents · safety checks passed 9 of 9 · [Repo](https://github.com/cloudflare/security-audit-skill) · [🌐 Site ↗](https://blog.cloudflare.com/build-your-own-vulnerability-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/security-audit-skill/)</sub>

<a name="fireworks-tech-graph"></a>
### #&#8288;155 [fireworks-tech-graph](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: patchy (34) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Python 3.9+, Codex or Claude Code, Node.js 22.12+ (optional, Puppeteer PNG export), cairosvg or rsvg-convert (optional, PNG export) · safety checks passed 10 of 10 · [Repo](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fireworks-tech-graph/)</sub>

<a name="harness"></a>
### #&#8288;156 [harness](https://github.com/revfactory/harness) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · Apache-2.0 · Sep 2026</sub>

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
### #&#8288;157 [cc-wf-studio](https://github.com/breaking-brake/cc-wf-studio) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · custom license · Aug 2026</sub>

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

<a name="unlazy"></a>
### #&#8288;158 [unlazy](https://github.com/leonxlnx/unlazy) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Sep 2026</sub>

**Agent skill that requires runnable acceptance gates before work is reported complete.**

unlazy is a skill for Claude Code and Codex CLI that has the agent write an acceptance ledger (GATES.md) of CHECK/EXPECT shell commands, then runs them with a Node checker and reports only what passes. It also covers scoped multi-leaf orchestration with ownership leases, and an optional Claude Code Stop hook that blocks exit while gates are unmet. Requires Node 16+, no third-party runtime packages.

- **+** Gates pass only on exit 0 plus EXPECT match, with definition-bound evidence
- **+** Checks need explicit per-command approval, stored outside the repository
- **+** No third-party runtime dependencies; Node 16 or newer, with a test suite
- **+** Installs through the skills CLI for several agents, plus manual Claude Code and Codex paths
- **−** Proves only the command oracle you write; weak gates give false assurance
- **−** Approval is consent, not a sandbox; checks run with ambient filesystem and network access
- **−** Version 2.1.0 is unreleased; README advises pinning a commit
- **−** Earlier benchmark claims lack reproducible artifacts; the README calls them historical only

<sub>no GPU · Needs Node.js 16+ · Models: Claude Code, Codex CLI · [Repo](https://github.com/leonxlnx/unlazy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/unlazy/)</sub>

<a name="wondelai-skills"></a>
### #&#8288;159 [skills](https://github.com/wondelai/skills) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Sep 2026</sub>

**SKILL.md collection turning business, UX and coding books into agent skills.**

65 agent skills in the SKILL.md format: 51 frameworks drawn from books and style guides (Clean Code, Refactoring UI, Mom Test, DDIA and others) and 14 metaskills that walk through multi-phase journeys such as creating a website or removing technical debt. Metaskills ask decision questions per phase and store state in the project's docs/ folder. Installs via the Claude Code plugin marketplace, skills.sh, Codex, or Agent Plugins.

- **+** Works with Claude Code, Codex, Cursor and other agentskills.io-compatible agents
- **+** Metaskills persist journey state in docs/, so work resumes across sessions
- **+** Install individually via npx skills add or as 10 plugin collections
- **+** Covers business, UX and marketing as well as code and architecture topics
- **−** Skills are prompt content summarizing third-party books, with no executable tooling
- **−** No evaluation results given; output depends on the host agent and model
- **−** Many skills are non-coding, so a coding-only user needs a small subset
- **−** Install steps differ per client

<sub>no GPU · Needs Claude Code, Codex, Cursor or another agentskills.io-compatible agent · [Repo](https://github.com/wondelai/skills) · [🌐 Site ↗](https://skills.wondel.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/wondelai-skills/)</sub>

<a name="huggingface-skills"></a>
### #&#8288;160 [skills](https://github.com/huggingface/skills) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs hf CLI, Hugging Face Hub account, AWS account (SageMaker skills) · Models: Safetensors, GGUF · safety checks passed 9 of 10 · [Repo](https://github.com/huggingface/skills) · [📖 Docs ↗](https://huggingface.co/docs/hub/agents-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huggingface-skills/)</sub>

<a name="council-of-high-intelligence"></a>
### #&#8288;161 [council-of-high-intelligence](https://github.com/0xnyk/council-of-high-intelligence) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (45) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

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
### #&#8288;162 [sol-pi](https://github.com/nvlabs/sol-pi) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (35) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

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

<a name="tons-of-skills-marketplace"></a>
### #&#8288;163 [tons-of-skills-marketplace](https://github.com/jeremylongshore/tons-of-skills-marketplace) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**Marketplace of Claude Code plugins and agent skills with a ccpi installer CLI.**

A catalog of 434 plugins and about 2,900 skills across 19 categories (DevOps, security, testing, SaaS skill packs, MCP servers and others), installed in Claude Code with /plugin marketplace add or the ccpi npm CLI. Claude Code is the only verified-native harness. Mirrored third-party plugins keep their upstream license and are pinned by commit.

- **+** Large catalog: 434 plugins, about 2,900 skills, 352 agent definitions, with reproducible count commands
- **+** Installs with one /plugin command or `ccpi install <pack>` from npm
- **+** Mirrored plugins record upstream author, license and pinned commit
- **+** Browsable web catalog with search and downloadable bundles
- **−** Only Claude Code is verified-native; other harnesses are unverified candidates
- **−** Certification program is not implemented; no artifact claims a quality tier
- **−** Each plugin has its own license; MIT covers only scaffolding and tooling
- **−** Repo development needs Node >=22.12.0 and pnpm >=9.15.9

<sub>no GPU · Needs Claude Code, Node.js >=22.12.0, pnpm >=9.15.9 · Models: Claude Code (verified-native harness) · [Repo](https://github.com/jeremylongshore/tons-of-skills-marketplace) · [🌐 Site ↗](https://tonsofskills.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tons-of-skills-marketplace/)</sub>

<a name="claude-code-tools"></a>
### #&#8288;164 [claude-code-tools](https://github.com/pchalasani/claude-code-tools) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**CLI tools, skills, hooks and plugins that extend Claude Code and Codex.**

A collection of add-ons for Claude Code and other coding agents, published as the claude-code-tools PyPI package and the aichat-search crate. It includes session search (aichat), tmux-based agent control (tmux-cli), safety hooks, a statusline, session repair, Claude/Codex session porting and voice input (voxtype). Skills install with `npx skills add`, which needs Node.js 22.20 or newer.

- **+** Bundles many tools: session search, safety hooks, statusline, session repair, inter-agent messaging
- **+** Skills install with one npx command, and most work in agents other than Claude Code
- **+** Ports sessions between Claude Code and Codex
- **+** Published on PyPI and crates.io, with a dedicated documentation site
- **−** Some skills and plugins work only in Claude Code and Codex
- **−** README is a card index; per-tool requirements live only in the external docs
- **−** Skill installation depends on Node.js 22.20 or newer
- **−** Many loosely related tools in one repo, so each must be evaluated separately

<sub>Needs Node.js 22.20+ (for npx skills), Claude Code or Codex CLI · Models: Claude Code, Codex · [Repo](https://github.com/pchalasani/claude-code-tools) · [📖 Docs ↗](https://pchalasani.github.io/claude-code-tools/) · [🌐 Site ↗](https://pchalasani.github.io/claude-code-tools/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-tools/)</sub>

<a name="swiftui-agent-skill"></a>
### #&#8288;165 [swiftui-agent-skill](https://github.com/twostraws/swiftui-agent-skill) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · Oct 2026</sub>

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

<a name="longmemory"></a>
### #&#8288;166 [longmemory](https://github.com/caviraoss/longmemory) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (44) · Freshness: active (90) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="agent-memory"></a>
### #&#8288;167 [agent-memory](https://github.com/tigerless-labs/agent-memory) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Oct 2026</sub>

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

<a name="go-modern-guidelines"></a>
### #&#8288;168 [go-modern-guidelines](https://github.com/jetbrains/go-modern-guidelines) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Sep 2026</sub>

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

<a name="ctf-skills"></a>
### #&#8288;169 [ctf-skills](https://github.com/ljagiello/ctf-skills) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (34) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

**Agent Skills package for CTF challenge work in coding agents.**

A set of Agent Skills for CTF competitions, split by category: web, pwn, crypto, reverse engineering, forensics, OSINT, malware, AI/ML and misc. It installs with `npx skills add ljagiello/ctf-skills` and works with Claude Code and other tools that follow the Agent Skills spec. It also ships an orchestrator skill, a writeup generator, and an installer script for the tools each category needs.

- **+** Skills are split by CTF category, so the agent loads only what it needs
- **+** Installer script supports dry-run, verify, force and per-group modes
- **+** Includes an orchestrator skill and a writeup generator skill
- **+** Each skill lists its own prerequisites for on-demand installs
- **−** Needs many external tools installed via apt, brew, gems, go or manual steps
- **−** Similar-writeup search skill relies on the Tavily API
- **−** No tagged release
- **−** README gives no benchmarks or solve-rate results

<sub>no GPU · Needs Agent Skills-compatible agent such as Claude Code, npx, Tavily API (ctf-similar-search skill) · [Repo](https://github.com/ljagiello/ctf-skills) · [🌐 Site ↗](https://agentskills.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ctf-skills/)</sub>

<a name="openwolf"></a>
### #&#8288;170 [openwolf](https://github.com/cytostack/openwolf) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · Oct 2026</sub>

**Local project memory and code index shared across coding agents.**

OpenWolf creates a .wolf/ folder in your project holding task checkpoints, a file and symbol index, bug-fix records and session notes. It registers hooks for Claude Code and Codex CLI and a plugin for OpenCode, restoring saved context after compaction or restart. It also reports recorded token usage and API-price cost estimates by agent and model in a local dashboard.

- **+** Memory, indexing and usage processing run locally with no extra model calls
- **+** Covers Claude Code, Codex CLI and OpenCode, with context-only files for Cursor, Gemini CLI, Antigravity
- **+** Usage report keeps missing counters as unavailable instead of reporting zero
- **+** Dashboard binds to 127.0.0.1 and requires a project token
- **−** Hook coverage varies by agent and version; Bash output shortening is Claude-only
- **−** Full live Claude to Codex handover is listed as unverified in the README
- **−** AGPL-3.0 license may restrict some commercial use
- **−** Cost figures are API list-price estimates, not subscription charges

<sub>no GPU · Needs Node.js >=20, At least one supported coding agent · Models: Claude Code, Codex CLI, OpenCode, Grok Build, Cursor · [Repo](https://github.com/cytostack/openwolf) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openwolf/)</sub>

<a name="edgeone-makers-tools"></a>
### #&#8288;171 [edgeone-makers-tools](https://github.com/tencentedgeone/edgeone-makers-tools) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Agent skill that teaches coding agents to build and deploy on EdgeOne Makers.**

Installs a single skill, edgeone-makers-tools, into Claude Code, Cursor, Codex or CodeBuddy. Its SKILL.md routes to reference docs on demand, covering deployment, edge and cloud functions, KV and Blob storage, middleware, the CLI and agent frameworks (LangGraph, Claude SDK, OpenAI Agents, DeepAgents, CrewAI). Hooks inject the relevant skill on prompt submit and before tool use.

- **+** One skill in the agent's list; capabilities load from references/ only when needed
- **+** Installs via npx skills, Claude Code marketplace or CodeBuddy marketplace
- **+** Plugin manifests for Claude Code, Cursor and CodeBuddy in one repo
- **+** Covers Node.js, Go and Python functions plus five agent frameworks
- **−** Useful only for deploying to the EdgeOne Makers platform
- **−** Requires an EdgeOne account (China or Global site)
- **−** No tagged releases
- **−** README gives no tested agent versions or hook behavior details

<sub>no GPU · Needs Node.js >= 16, EdgeOne account · [Repo](https://github.com/tencentedgeone/edgeone-makers-tools) · [🌐 Site ↗](https://pages.edgeone.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/edgeone-makers-tools/)</sub>

<a name="fast-jev-compaction"></a>
### #&#8288;172 [fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Sep 2026</sub>

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

<a name="nvidia-skills"></a>
### #&#8288;173 [skills](https://github.com/nvidia/skills) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (36) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · Apache-2.0 · Oct 2026</sub>

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

<a name="codex-plugin-cc"></a>
### #&#8288;174 [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: widely used (87) · Freshness: active (96) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Jul 2026</sub>

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

<sub>no GPU · Needs Claude Code, Codex CLI (@openai/codex), Node.js 18.18+, ChatGPT account or OpenAI API key · Models: OpenAI Codex models (e.g. gpt-5.4-mini, gpt-5.3-codex-spark) · safety checks passed 11 of 12 · [Repo](https://github.com/openai/codex-plugin-cc) · [📖 Docs ↗](https://developers.openai.com/codex/app-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-plugin-cc/)</sub>

<a name="scroll-world"></a>
### #&#8288;175 [scroll-world](https://github.com/oso95/scroll-world) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: weak (24) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Jul 2026</sub>

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

<a name="stitch-skills"></a>
### #&#8288;176 [stitch-skills](https://github.com/google-labs-code/stitch-skills) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: weak (30) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.5k · Apache-2.0 · Aug 2026</sub>

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

<a name="remodex"></a>
### #&#8288;177 [remodex](https://github.com/emanuele-web04/remodex) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Sep 2026</sub>

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

<a name="my-claude-code-setup"></a>
### #&#8288;178 [my-claude-code-setup](https://github.com/centminmod/my-claude-code-setup) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**Starter Claude Code config with CLAUDE.md memory bank templates and hooks.**

A copy-into-your-project set of Claude Code settings: a CLAUDE.md memory bank that keeps context across sessions, three CLAUDE.md templates, hooks, slash commands and a statusline script. The README also lists MCP servers, plugin installs and git worktree launchers for parallel Claude Code and Codex CLI sessions.

- **+** Three CLAUDE.md templates (~101 to ~153 lines) plus a migration prompt for existing files
- **+** Memory bank files are read on demand, not auto-loaded, to save context
- **+** Includes a statusline script showing context usage, cost and git branch
- **+** Lists install commands for MCP servers and plugins such as Context7 and Safety Net
- **−** Personal setup; files are copied and edited by hand, not installed as a package
- **−** settings.json assumes macOS Terminal-Notifier; README says to remove it elsewhere
- **−** Requires a paid Claude plan or a Z.AI account to use Claude Code
- **−** README mixes referral links and unrelated guides, making it harder to scan

<sub>no GPU · Needs Claude Code, Claude paid plan or Z.AI, ripgrep, fd, jq, Terminal-Notifier (macOS) · Models: Claude, Z.AI GLM-4.7 · [Repo](https://github.com/centminmod/my-claude-code-setup) · [📖 Docs ↗](https://docs.anthropic.com/en/docs/claude-code/overview) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/my-claude-code-setup/)</sub>

<a name="goldie"></a>
### #&#8288;179 [goldie](https://github.com/software-mansion-labs/goldie) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · custom license · Oct 2026</sub>

**CLI and agent skill that makes App Store and Google Play screenshots.**

Goldie takes captures replayed by argent on an iOS simulator or Android emulator, then frames them with a device bezel, background and headline. It also joins clips into an App Store preview video and checks output against store upload rules. It installs as an npm CLI plus a skill for Claude Code, Cursor, Codex and other skills-compatible agents, with a browser studio for tweaks.

- **+** Framework agnostic: SwiftUI, Compose, Flutter and React Native work the same
- **+** Covers iPhone, iPad 13-inch and Google Play sizes from the same flows
- **+** Studio saves choices to goldie.design.json so CLI renders match
- **+** Multi-locale rendering, with optional per-locale captures on iOS
- **−** iOS screenshots require macOS with Xcode simulators
- **−** Depends on argent for capture, plus ffmpeg and Node 20 or newer
- **−** Flows break when the app UI changes and need repair or re-recording
- **−** Needs a Release build; debug builds paint LogBox banners into captures

<sub>no GPU · Needs Node 20+, ffmpeg, argent, Xcode iOS simulators (macOS), Android emulator · [Repo](https://github.com/software-mansion-labs/goldie) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/goldie/)</sub>

<a name="playwright-skill"></a>
### #&#8288;180 [playwright-skill](https://github.com/lackeyjb/playwright-skill) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Aug 2026</sub>

**Agent Skill that lets coding agents write and run Playwright scripts.**

An Agent Skill, also packaged as a Claude Code plugin, that has a coding agent write custom Playwright code for a browser task and run it through a run.js executor. It opens a visible Chromium window by default and returns console output and screenshots. SKILL.md stays short and a fuller API_REFERENCE.md is loaded only when needed.

- **+** Agent writes real Playwright code, so loops, assertions, network interception and video are possible
- **+** Scripts are plain files you can keep and rerun
- **+** Installs via the skills CLI for Claude Code, Cursor, Copilot, Codex, Gemini CLI and others
- **+** Runs headed by default, so you can watch the automation
- **−** Requires a manual npm run setup step after install to fetch Playwright and Chromium
- **−** Only Chromium is installed by default; other browsers need npm run install-all-browsers
- **−** README points to Microsoft's playwright-cli for simple interactive browsing
- **−** Helper screenshots go to the OS temp directory unless PW_ARTIFACT_DIR is set

<sub>no GPU · Needs Node.js, Playwright, Chromium · [Repo](https://github.com/lackeyjb/playwright-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/playwright-skill/)</sub>

<a name="oil-motion"></a>
### #&#8288;181 [oil-motion](https://github.com/oil-oil/oil-motion) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

**Agent skill that turns AI video into scroll, mouse and touch-driven web animation.**

Oil Motion is a skill for coding agents that plans an interaction animation, generates keyframes and the video between them, cleans the frames, and wires the result to scroll, mouse, drag, touch or device orientation. Output is a baked MP4, an alpha WebP atlas or a green-screen MP4 keyed in WebGL, chosen by a budget script. Generation goes through ZenMux by default, with a pilot clip approved first.

- **+** Confirms keyframes first, then generates motion between them to limit identity and structure drift
- **+** Picks one asset format (baked MP4, alpha WebP atlas, green-screen MP4) from a budget script
- **+** Pilot approval with SHA-256 frame hashes blocks mismatched clips before any network call
- **+** API key is stored in the OS credential store, not pasted into chat
- **−** Generation needs a ZenMux API key and is billed per generation
- **−** README says it is only verified on macOS
- **−** Not meant for UI transitions that CSS, SVG, Lottie or real-time 3D can handle
- **−** README is Chinese-first; the English version is a separate file

<sub>no GPU · Needs Python 3.10+, FFmpeg, Node.js 22.18+ (key setup page), ZenMux API · Models: ZenMux-hosted image and video models · [Repo](https://github.com/oil-oil/oil-motion) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oil-motion/)</sub>

<a name="frontend-slides"></a>
### #&#8288;182 [frontend-slides](https://github.com/zarazhangrui/frontend-slides) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (85) · Freshness: active (92) · Maintenance: weak (5) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Jun 2026</sub>

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

<sub>no GPU · Needs Claude Code or another coding agent, Python (scripts/extract-pptx.py) · Models: Claude Code, Codex, Kimi Code, OpenCode, Gemini CLI · safety checks passed 9 of 10 · [Repo](https://github.com/zarazhangrui/frontend-slides) · [📖 Docs ↗](https://github.com/zarazhangrui/frontend-slides) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frontend-slides/)</sub>

<a name="ip-as-logo-skill"></a>
### #&#8288;183 [ip-as-logo-skill](https://github.com/s1dashu/ip-as-logo-skill) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Aug 2026</sub>

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
### #&#8288;184 [skills](https://github.com/antfu/skills) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: weak (21) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

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

<a name="adhd"></a>
### #&#8288;185 [adhd](https://github.com/uditakhourii/adhd) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Oct 2026</sub>

**Skill that runs isolated parallel reasoning frames plus a critic pass for ideation.**

ADHD is an agent skill, npm CLI and TypeScript library that spawns N isolated LLM calls, each under a distorted cognitive frame with no shared context. A separate critic call then scores ideas on novelty, viability and fit, flags traps, clusters them and deepens the top-K. It installs with `npx skills add` into Claude Code, Cursor, Codex, Cline, Gemini CLI and others.

- **+** Generator and critic are separate LLM calls, so the split is mechanical, not prompt-based
- **+** Installs as a skill into Claude Code, Cursor, Codex, Cline, Gemini CLI and about 50 other agents
- **+** Also ships as an npm CLI (adhd-agent) and library returning shortlist, traps and clusters
- **+** Eval transcripts and methodology are in the repo (bench/results.json, documentation/evals.md)
- **−** Benchmarks are author-run: 6 problems scored by an LLM judge
- **−** One external review measured about 2.3x time and 1.9x output versus single-shot
- **−** Aimed at open-ended ideation; little use for routine coding tasks
- **−** README does not say which model providers the CLI and library support

<sub>no GPU · Needs Node.js >=18, LLM agent or API access · Models: unknown · [Repo](https://github.com/uditakhourii/adhd) · [📖 Docs ↗](https://adhd.mintlify.site/) · [🌐 Site ↗](https://adhdstack.github.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/adhd/)</sub>

<a name="cloudflare-skills"></a>
### #&#8288;186 [skills](https://github.com/cloudflare/skills) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · Apache-2.0 · Oct 2026</sub>

**Agent Skills and MCP server for building on Cloudflare Workers.**

A plugin of 18 Agent Skills covering Workers, Wrangler, Durable Objects, the Agents SDK, Sandbox, Turnstile, email and Cloudflare One. Skills load automatically when a request matches their triggers. The plugin also bundles Cloudflare's remote MCP server, which gives the agent access to the Cloudflare API and current docs.

- **+** Native plugin install for Claude Code, Codex, VS Code/Copilot and Cursor
- **+** Also installable via npx skills or by copying folders into a skills directory
- **+** Covers many products: Workers, Durable Objects, Agents SDK, Sandbox, Cloudflare One
- **+** Bundles the main Cloudflare remote MCP server for API and docs access
- **−** Only useful for projects that run on Cloudflare
- **−** Bundles only the main cloudflare MCP server, not product-specific ones
- **−** Some skills target previews, e.g. sandbox-next is a 1.0 preview
- **−** No tagged releases

<sub>no GPU · Needs Cloudflare account, Cloudflare remote MCP server · Models: Claude Code, OpenAI Codex, GitHub Copilot, Cursor, OpenCode · [Repo](https://github.com/cloudflare/skills) · [📖 Docs ↗](https://developers.cloudflare.com/agents/model-context-protocol/cloudflare/servers-for-cloudflare/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cloudflare-skills/)</sub>

<a name="designer-skills"></a>
### #&#8288;187 [designer-skills](https://github.com/owl-listener/designer-skills) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Sep 2026</sub>

**Design-practice skills and commands for Claude Code and Gemini CLI.**

A Claude Code plugin marketplace of markdown skills and slash commands for design work: research, UX strategy, UI, interaction design, design systems, prototyping and testing, handoff, and visual critique. This repo hosts 9 plugins (111 skills, 34 commands). The marketplace also pulls in four companion collections, for 273 skills and 76 commands in total. Each plugin also works as a Gemini CLI extension.

- **+** Installs from one marketplace command, then per plugin via /plugin install
- **+** Commands chain skills into workflows, e.g. /design-research:discover runs personas, empathy map, journey map
- **+** Works in both Claude Code and Gemini CLI
- **+** /designer-toolkit:start-here routes you to a first command and what to skip
- **−** Only Claude Code and Gemini CLI are supported
- **−** Content is markdown prompts only; output quality depends on the host model
- **−** Skill counts in the README are inconsistent (111 vs 107 for this repo)
- **−** PRs without a matching open issue are closed without review

<sub>no GPU · Needs Claude Code or Gemini CLI · Models: Claude Code, Gemini CLI · [Repo](https://github.com/owl-listener/designer-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/designer-skills/)</sub>

<a name="vibe-wise"></a>
### #&#8288;188 [vibe-wise](https://github.com/nykooi1/vibe-wise) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (39) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

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
### #&#8288;189 [scroll-craft](https://github.com/nateherkai/scroll-craft) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (38) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Sep 2026</sub>

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

<a name="web-quality-skills"></a>
### #&#8288;190 [web-quality-skills](https://github.com/addyosmani/web-quality-skills) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Aug 2026</sub>

**Agent Skills for auditing web performance, Core Web Vitals, accessibility and SEO.**

Six SKILL.md packages (web-quality-audit, performance, core-web-vitals, accessibility, seo, and a security and code-quality skill) that guide a coding agent through Lighthouse, WCAG 2.2 and Core Web Vitals checks. They separate CrUX field data, RUM, lab traces and static inspection as evidence types. Chrome DevTools MCP is optional; without it the skills fall back to Lighthouse CLI, PageSpeed Insights/CrUX and manual checks.

- **+** Separates field, RUM, lab and static evidence instead of mixing them in one score
- **+** Installs via npx skills, Claude Code plugin, Codex marketplace or Gemini CLI extension
- **+** Stack-agnostic; covers React, Vue, Svelte, Astro and plain HTML
- **+** Falls back to Lighthouse CLI and PageSpeed Insights when DevTools MCP is absent
- **−** Unofficial; not maintained by the Lighthouse or Chrome teams
- **−** Live audits need Chrome DevTools MCP, which is a separate install
- **−** No tagged releases
- **−** Instruction files only; results depend on the host agent following them

<sub>no GPU · Needs Chrome DevTools MCP (optional), Lighthouse CLI (fallback), Node.js/npx for installer · Models: Claude Code, Codex, Gemini CLI, OpenCode, Cursor · [Repo](https://github.com/addyosmani/web-quality-skills) · [📖 Docs ↗](https://agentskills.io/specification) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/web-quality-skills/)</sub>

<a name="delegate-skills"></a>
### #&#8288;191 [delegate-skills](https://github.com/amelnagdy/delegate-skills) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Oct 2026</sub>

**Skills that let one coding agent delegate tasks to other coding CLIs.**

A set of agent skills, installed with the Skills CLI, that let an orchestrating agent hand work to another coding CLI such as Codex, Claude Code, Cursor Agent, OpenCode or Aider. Each skill ships a Node relay that runs the CLI, writes a structured result.json and never commits. A setup skill discovers installed CLIs and maps them to named lanes like feature, tests and ui.

- **+** Covers 18 implementer CLIs behind one result.v1 contract, so you can swap them freely
- **+** Relays use Node built-ins only, with no dependencies, telemetry or network calls of their own
- **+** Relays never commit; you review the diff and land the commit
- **+** Project lane config is bound to explicit approval and fails closed if edited or cloned
- **−** Several CLIs have no enforced read-only mode or sandbox, per the README footnotes
- **−** Verification is uneven: Aider was tested only against a stub endpoint, not on macOS or Linux
- **−** Needs each implementer CLI installed and authenticated separately
- **−** No tagged release, so pinning to a version tag is not yet possible

<sub>no GPU · Needs Node 18+, git, Skills CLI (npx skills), at least one implementer CLI (Codex, Claude Code, Cursor Agent, OpenCode, Aider, etc.) · Models: Aider with any OpenAI-compatible endpoint, Models via the installed CLIs (Codex, Claude Code, OpenCode, Cursor, etc.) · [Repo](https://github.com/amelnagdy/delegate-skills) · [🌐 Site ↗](https://www.skills.sh/amElnagdy/delegate-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/delegate-skills/)</sub>

<a name="chops"></a>
### #&#8288;192 [chops](https://github.com/shpigford/chops) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · custom license · Aug 2026</sub>

**macOS app to browse and edit coding-agent skills across tools.**

Chops is a native SwiftUI/SwiftData macOS app that scans the skill and agent directories of Claude Code, Cursor, Codex, Windsurf and Amp, plus project-level Copilot and Aider files. It lists them in one place with full-text search, a built-in editor with frontmatter parsing, and collections that leave source files untouched. It can also browse remote servers and install skills from the skills.sh registry.

- **+** Scans skill and agent directories for seven tools, with custom scan paths
- **+** FSEvents file watching re-scans automatically when files change on disk
- **+** Dedups symlinked skills into one entry with multiple tool badges
- **+** Installs skills from the skills.sh registry and from remote servers
- **−** macOS 15 or later only
- **−** App sandbox is disabled to read dotfiles across the home directory
- **−** No automated test suite; changes are validated manually
- **−** FSL-1.1-MIT license, not a standard OSI-approved license

<sub>no GPU · Needs macOS 15+, Xcode (build from source), xcodegen (build from source), Sparkle · [Repo](https://github.com/shpigford/chops) · [🌐 Site ↗](https://chops.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/chops/)</sub>

<a name="babysitter"></a>
### #&#8288;193 [babysitter](https://github.com/a5c-ai/babysitter) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Aug 2026</sub>

**Code-defined workflow orchestration with approval gates for AI coding harnesses.**

Babysitter lets you write a workflow as a JavaScript process that calls tasks, breakpoints and quality gates, then drives an AI coding agent through it step by step. Every decision is recorded in an event-sourced journal. It installs as a plugin for 12 harnesses, including Claude Code and Codex, and has an internal harness for headless CI runs.

- **+** Workflows are plain JavaScript, with human breakpoints and quality gates enforced in code
- **+** Same processes run across 12 supported harnesses via the Adapters runtime
- **+** Internal harness runs processes headless in CI with no external coding agent
- **+** Event-sourced journal supports resuming interrupted runs and diagnosing them
- **−** Install is split across several npm packages (babysitter, adapters-cli, genty-platform)
- **−** Only Claude Code and Codex have dedicated pages; Codex is beta, most others experimental
- **−** Adapters CLI needs Node 22.13+, higher than the Node 20 baseline
- **−** No hosted demo; the monorepo is large and the README is dense

<sub>no GPU · Needs Node.js 20+, AI coding harness (e.g. Claude Code) · Models: Claude Code, Codex, Cursor, Gemini CLI, GitHub Copilot · [Repo](https://github.com/a5c-ai/babysitter) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/babysitter/)</sub>

<a name="ralph"></a>
### #&#8288;194 [ralph](https://github.com/snarktank/ralph) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (79) · Freshness: slowing (38) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Feb 2026</sub>

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

<sub>no GPU · Needs Amp CLI or Claude Code, jq, git · Models: Amp, Claude Code · safety checks passed 9 of 10 · [Repo](https://github.com/snarktank/ralph) · [📖 Docs ↗](https://snarktank.github.io/ralph/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ralph/)</sub>

<a name="microsoft-skills"></a>
### #&#8288;195 [skills](https://github.com/microsoft/skills) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

**Agent skills library for Azure SDKs and Microsoft Foundry coding agents.**

A collection of roughly 175 SKILL.md skills for Azure SDKs and Microsoft Foundry, split by language (Python, .NET, TypeScript, Java, Rust) plus core and language-agnostic Foundry skills. It also ships custom agents, an AGENTS.md template, MCP configs and plugin packages. Install with `npx skills add microsoft/skills`, which copies chosen skills into the agent's directory, such as .github/skills/ for GitHub Copilot.

- **+** Skills cover Azure SDKs across Python, .NET, TypeScript, Java and Rust
- **+** Installer wizard picks skills per agent and symlinks across multiple agents
- **+** Includes custom agents, an AGENTS.md template and MCP configs alongside skills
- **+** Has CI test harness and Copilot SDK evaluation workflows for skills
- **−** Azure and Foundry specific; little use outside the Microsoft ecosystem
- **−** README warns that loading all skills causes context rot, so selection is manual
- **−** Marked work in progress; several Foundry skills are preview
- **−** README skill counts are inconsistent (174, 175, 28 vs 29 .NET)

<sub>no GPU · Needs Node.js (npx), GitHub Copilot or another coding agent · [Repo](https://github.com/microsoft/skills) · [📖 Docs ↗](https://microsoft.github.io/skills/#documentation) · [🌐 Site ↗](https://microsoft.github.io/skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/microsoft-skills/)</sub>

<a name="agent-toolkit-for-aws"></a>
### #&#8288;196 [agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · Apache-2.0 · Oct 2026</sub>

**AWS plugins, skills and managed MCP server for coding agents.**

Official AWS toolkit that gives coding agents (Claude Code, Codex, Cursor, Kiro, fx) a managed AWS MCP Server plus task-specific skills. The MCP server exposes 300+ AWS services through one authenticated endpoint, runs sandboxed Python scripts and searches AWS documentation. IAM condition keys, CloudWatch metrics and CloudTrail logging separate agent actions from human ones.

- **+** IAM condition keys let policies target agent actions separately from human actions
- **+** CloudWatch metrics and CloudTrail audit logging for every MCP request
- **+** Plugins for Claude Code, Codex and Cursor; skills and MCP config for Kiro, fx and others
- **+** Documentation search works without AWS credentials
- **−** Core MCP server is a managed AWS endpoint, not self-hosted
- **−** API calls and script execution need an AWS account with local credentials
- **−** Plugins exist only for Claude Code, Codex and Cursor; other agents need manual setup
- **−** Requires uv installed to run the MCP proxy

<sub>no GPU · Needs AWS account and credentials, uv, AWS MCP Server (managed endpoint), Node.js (npx skills) · [Repo](https://github.com/aws/agent-toolkit-for-aws) · [📖 Docs ↗](https://docs.aws.amazon.com/agent-toolkit/latest/userguide/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-toolkit-for-aws/)</sub>

<a name="mcollina-skills"></a>
### #&#8288;197 [skills](https://github.com/mcollina/skills) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

**Agent skills for Node.js, Fastify, TypeScript, OAuth and GitHub workflows.**

A collection of eleven skills for AI coding agents, written by Matteo Collina. They cover Node.js and Node core internals, Fastify, TypeScript types, OAuth 2.0/2.1, neostandard with ESLint 9, Diátaxis documentation, gh CLI usage, and AGENTS.md generation. The repo also has a skill-optimizer skill and docs on cross-model benchmarking.

- **+** Focused on the Node.js ecosystem: Fastify, Node core, neostandard, OAuth and TypeScript
- **+** Includes a skill-optimizer skill and a documented cross-model benchmarking workflow
- **+** Includes an init skill that creates and maintains AGENTS.md files
- **+** MIT licensed, with each skill covering one named topic
- **−** README gives no install command or list of supported agents
- **−** Most skills are Node/JavaScript-specific, with little use outside that stack
- **−** No tagged releases
- **−** README gives only one-line skill descriptions, with no example output

<sub>no GPU · Needs gh CLI (octocat skill) · [Repo](https://github.com/mcollina/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcollina-skills/)</sub>

<a name="improve"></a>
### #&#8288;198 [improve](https://github.com/shadcn/improve) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.2k · MIT · Sep 2026</sub>

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

<a name="claude-code-workflows"></a>
### #&#8288;199 [claude-code-workflows](https://github.com/oneredoak/claude-code-workflows) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (40) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Oct 2026</sub>

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
### #&#8288;200 [effective-html](https://github.com/plannotator/effective-html) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (37) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="anything2explainer"></a>
### #&#8288;201 [anything2explainer](https://github.com/vincentwei1021/anything2explainer) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · custom license · Sep 2026</sub>

**Claude Code and Codex skill that turns a topic into a narrated explainer video.**

A skill for Claude Code and Codex that guides an agent through research, narration, TTS voiceover, storyboarding, parallel shot building and QC. The result is a 1280x720 motion-graphics MP4 in Chinese or English, with every frame written as a Remotion (React/TypeScript) component. It ships a Remotion template, style and motion specs, QC scripts and one reference film. It is not a CLI.

- **+** Four user checkpoints: length and language, narration, voice, and a 30-second look check
- **+** Deterministic renders: frames are pure functions of frame number with seeded randomness
- **+** Local kokoro-82m, piper and kokoro-onnx, cloud edge-tts, or bring your own audio
- **+** Includes a reference film paper trail and a frame-metrics QC script
- **−** PolyForm Noncommercial license; commercial use needs the author's authorization
- **−** One visual style with two backdrops; other changes mean editing style guide and ui.tsx
- **−** Landscape 1280x720 only, no 9:16; Chinese and English only
- **−** Runs take about 1 to 3 hours and 2 to 3 GB disk; verified on macOS, Windows untested

<sub>no GPU · Needs Claude Code or Codex, Node >=18, Remotion 4.0.507, ffmpeg, Python 3 with edge-tts, zsh, kokoro-82m (English narration), Chromium (Linux ARM) · Models: kokoro-82m, edge-tts, kokoro-onnx, piper · [Repo](https://github.com/vincentwei1021/anything2explainer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/anything2explainer/)</sub>

<a name="claude-code-infrastructure-showcase"></a>
### #&#8288;202 [claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (65) · Freshness: active (96) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Jul 2026</sub>

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

<a name="ccpm"></a>
### #&#8288;203 [ccpm](https://github.com/automazeio/ccpm) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Oct 2026</sub>

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

<a name="headcount"></a>
### #&#8288;204 [headcount](https://github.com/cbrock84/headcount) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Plugin marketplace of 172 business-function skills in 16 departments.**

A set of 172 agent skills grouped into 16 department plugins (CEO, Technology, Security, IT Operations, Product, Marketing, Demand Generation and others), each installable on its own. Skills load when a request matches and can be called as `department:skill`. Manifests for Claude Code and ChatGPT/Codex are generated from the same tree, and each department has a subagent charter in `.claude/agents/`.

- **+** Each department installs separately, so a project loads only the skills it needs
- **+** One tree generates both Claude Code and ChatGPT/Codex manifests
- **+** Namespaced names like security:threat-modeling avoid skill name collisions
- **+** Includes 11 worked cross-department scenarios and an agent charter per department
- **−** Most skills cover business, marketing and IT; only part is engineering-focused
- **−** No tagged release, so versioning is unknown
- **−** README gives no benchmarks of skill quality
- **−** Install steps are shown in detail only for Claude Code

<sub>no GPU · Needs Claude Code or ChatGPT/Codex · Models: Claude Code, ChatGPT, Codex · [Repo](https://github.com/cbrock84/headcount) · [▶️ Demo ↗](https://cbrock84.github.io/headcount/org-chart.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/headcount/)</sub>

<a name="gsap-skills"></a>
### #&#8288;205 [gsap-skills](https://github.com/greensock/gsap-skills) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: popular (74) · Freshness: recent (66) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Apr 2026</sub>

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

<sub>no GPU · Needs Node.js and npx (for skills CLI), gsap npm package in target project · Models: Claude Code, Cursor, Codex, Windsurf, GitHub Copilot · safety checks passed 8 of 9 · [Repo](https://github.com/greensock/gsap-skills) · [🌐 Site ↗](https://gsap.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gsap-skills/)</sub>

<a name="buildwithclaude"></a>
### #&#8288;206 [buildwithclaude](https://github.com/davepoon/buildwithclaude) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: known (36) · Freshness: active (85) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="tdd-guard"></a>
### #&#8288;207 [tdd-guard](https://github.com/nizos/tdd-guard) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Claude Code plugin that blocks edits that violate test-driven development.**

TDD Guard installs as a Claude Code plugin with hooks that check each edit. It blocks implementation written without a failing test, or code beyond what the current test requires, and tells the agent what to do instead. The README says it has grown into Probity, and new projects should start there. TDD Guard is still maintained.

- **+** Supports Vitest, Jest, Storybook, pytest, PHPUnit, Go, Rust, RSpec and Minitest
- **+** Validation rules can be customized, and lint rules can drive refactoring
- **+** Can be toggled on and off mid-session
- **+** Installs through Claude Code plugin commands and a /tdd-guard:setup skill
- **−** Superseded by Probity; README tells new projects to start there
- **−** Works only with Claude Code
- **−** Needs a test reporter configured for your framework
- **−** Hooks run with your user permissions

<sub>no GPU · Needs Node.js 22+, Claude Code, A supported test framework · Models: Claude Code · [Repo](https://github.com/nizos/tdd-guard) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tdd-guard/)</sub>

<a name="design-dna"></a>
### #&#8288;208 [design-dna](https://github.com/zanwei/design-dna) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Aug 2026</sub>

**Agent skill that extracts a design's tokens and style into JSON, then rebuilds it.**

An Agent Skills package that analyzes screenshots, images or URLs and writes a JSON "Design DNA" profile covering design tokens, qualitative style and visual effects. A second phase generates self-contained HTML/CSS/JS from that JSON plus your content. Optional Node scripts run k-means color measurement and score the output against the reference by ΔE.

- **+** Optional measure-colors and verify scripts give exact hexes and PASS/FAIL ΔE checks
- **+** DNA JSON can be committed, shared and reused across projects and agents
- **+** One npx command installs it to Cursor, Claude Code, Codex, Copilot and others
- **+** Structure, analyze and generate phases work alone or chained
- **−** Color measurement scripts apply to image references, not live URLs
- **−** Default output is self-contained HTML/CSS/JS; other frameworks are not documented
- **−** Output quality depends on the host agent; README suggests a manual polish pass
- **−** No tagged releases

<sub>no GPU · Needs Node.js, npx, skills CLI, A host agent such as Cursor or Claude Code · [Repo](https://github.com/zanwei/design-dna) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/design-dna/)</sub>

<a name="lottie"></a>
### #&#8288;209 [lottie](https://github.com/diffusionstudio/lottie) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (49) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · MIT · Jul 2026</sub>

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

<a name="openagentscontrol"></a>
### #&#8288;210 [openagentscontrol](https://github.com/darrenhinde/openagentscontrol) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (45) · Freshness: active (93) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.9k · MIT · Oct 2026</sub>

**Approval-gated agents and context files for OpenCode that follow your coding patterns.**

OpenAgents Control adds markdown-defined agents (OpenAgent, OpenCoder, SystemBuilder) and subagents to the OpenCode CLI. A ContextScout subagent loads your project's coding standards from `.opencode/context/` before code is generated, and every file write or command requires approval. A BETA Claude Code plugin is also offered. The README says a rewrite is coming that will replace much of this version.

- **+** Agents are plain markdown files you edit, with no compile step
- **+** Team patterns live in `.opencode/context/` and can be committed to the repo
- **+** Approval required before file edits, bash commands and subagent delegation
- **+** Installs with one curl script; also ships a Claude Code plugin (beta)
- **−** Targets OpenCode v1; README warns a major rewrite will replace much of it
- **−** Sequential approval flow is slower than autonomous parallel agents
- **−** The 80% token reduction claim is given without a methodology
- **−** Requires OpenCode CLI, Bash 3.2+ and Git; Claude Code plugin is beta

<sub>no GPU · Needs OpenCode CLI, Bash 3.2+, Git · Models: Claude, GPT, Gemini, MiniMax, Local models · [Repo](https://github.com/darrenhinde/openagentscontrol) · [🌐 Site ↗](https://nextsystems.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openagentscontrol/)</sub>

<a name="gptcommit"></a>
### #&#8288;211 [gptcommit](https://github.com/zurawiki/gptcommit) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Sep 2026</sub>

**Git hook that writes commit messages from staged diffs using an OpenAI model.**

gptcommit is a Rust CLI that installs a git prepare-commit-msg hook and fills in the commit message from the staged diff using an OpenAI model. It summarizes each changed file with up to four concurrent requests, then generates a title and summary, with optional conventional-commit prefixes. Settings are layered from a user TOML file, a per-repo file and GPTCOMMIT__* environment variables.

- **+** Runs inside normal `git commit` via a prepare-commit-msg hook; generated text stays editable
- **+** Layered config (user, repo, env vars) with `gptcommit config` subcommands
- **+** Git-style `file_ignore` patterns skip lockfiles and minified files before anything is sent
- **+** Supports custom API base URL, proxy and model override; output in en, zh-cn, zh-tw, ja
- **−** Only OpenAI-style APIs are documented; no local model support is described
- **−** Sends diff contents to the API, and costs grow with N+2 prompts per commit
- **−** Hook skips commits that use a template or amend unless `allow-amend` is set
- **−** A failed file summary stops generation instead of being skipped

<sub>no GPU · Needs OpenAI API key, git, Rust toolchain (cargo) or Homebrew to install · Models: OpenAI models (default gpt-6-luna), custom OpenAI-compatible API base, fine-tuned OpenAI models · [Repo](https://github.com/zurawiki/gptcommit) · [▶️ Demo ↗](https://asciinema.org/a/552380) · [🌐 Site ↗](https://zura.wiki/post/never-write-a-commit-message-again-with-the-help-of-gpt-3/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gptcommit/)</sub>

<a name="agents-best-practices"></a>
### #&#8288;212 [agents-best-practices](https://github.com/denissergeevitch/agents-best-practices) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Agent Skill with reference docs for designing and auditing agent harnesses.**

A provider-neutral Agent Skill, installed into Codex or Claude Code skill directories, that activates on agent-architecture questions. It supplies a SKILL.md and a references/ set covering MVP blueprints, tool permissions, context and compaction, evals, security, durable runtimes and voice agents, with worked example dialogues. It is documentation and guidance, not a runtime or library.

- **+** Installs via `npx skills add` or a plain git clone into the skills directory
- **+** Reference files split by topic: loop, permissions, memory, evals, security, voice
- **+** Examples show concrete controls like approval gates, loop budgets and typed narrow tools
- **+** Not limited to coding agents; covers support, research, ops and other domains
- **−** Guidance only; no runnable harness, code or templates to fork
- **−** Many advanced profiles are marked post-MVP or experimental, adding reading overhead
- **−** Self-update checks upstream main on each task, adding a network dependency
- **−** No releases or version tags; installs track main

<sub>no GPU · Needs Codex or Claude Code (or another skills-compatible agent), Node.js/npx (for the skills installer) · Models: provider-neutral · [Repo](https://github.com/denissergeevitch/agents-best-practices) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents-best-practices/)</sub>

<a name="holo-card-studio"></a>
### #&#8288;213 [holo-card-studio](https://github.com/everettfish/holo-card-studio) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · custom license · Sep 2026</sub>

**Codex skill that generates 3D holographic cards with a Three.js viewer.**

A Codex skill that turns a text prompt or reference image into a layered holographic card. A pipeline script builds an editable Blender scene (card.blend) and a responsive Three.js viewer with parallax, rainbow foil and sparkle effects. A second mode makes lenticular two-image cards that switch the whole face by viewing angle.

- **+** Delivers an editable card.blend, four-layer PNG assets, card-config.json and a web viewer
- **+** Fetches a portable Blender into the project and checks its SHA-256
- **+** One command runs the pipeline: run_pipeline.py with holographic or lenticular mode
- **+** Rarity, number and text live in card-config.json; rerun the pipeline to update
- **−** Designed to be driven by Codex; no standalone image generation described
- **−** Web shader output differs from Blender renders in color, glow and card back
- **−** README is mainly Chinese; English version is in a separate file
- **−** License not identified; companion gallery repo is private

<sub>Needs Codex, Python 3, Pillow, Node.js, npm, Blender (auto-downloaded portable), Three.js · [Repo](https://github.com/everettfish/holo-card-studio) · [▶️ Demo ↗](https://card.waterq.us/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/holo-card-studio/)</sub>

<a name="replica-skill"></a>
### #&#8288;214 [replica-skill](https://github.com/jakeschincariol/replica-skill) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: known (40) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Oct 2026</sub>

**Claude skills that reverse-engineer, rebuild and launch a clone of an app.**

Eleven Claude skills run in sequence: recon, architecture, design, build, backend, test, diff, entrepreneur, brand, launch and deploy. Each skill writes into a replica/ folder that the next one reads. Six standard-library Python tools handle image diffing, parity scoring, review ranking, contrast checks, a rebrand sweep and store listing limits.

- **+** Covers the path from recon to deploy, each skill reading the previous one's output
- **+** Python tools use only the standard library and make no network calls
- **+** Review tool drops unlinked reviews, so printed quotes trace to a source URL
- **+** Sweep script blocks deploy while the original's name, domain or colors remain in code
- **−** Results depend on app complexity; README says a spreadsheet engine is not a weeks-long job
- **−** Recon uses public pages, screenshots and your own account, not source or private APIs
- **−** Built for Claude; other chats get single SKILL.md modes without the Python tools
- **−** Trademark and legal risk stays with you; README says it is not legal advice

<sub>no GPU · Needs Claude (Claude Code or chat), Python 3.8+ · Models: Claude · [Repo](https://github.com/jakeschincariol/replica-skill) · [🌐 Site ↗](https://opusjake.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/replica-skill/)</sub>

<a name="best-skills"></a>
### #&#8288;215 [best-skills](https://github.com/xstongxue/best-skills) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Sep 2026</sub>

**Agent skill collection for thesis, patents, diagrams, PPT and Office files.**

A set of SKILL.md folders you copy into the skills directory of Cursor, Claude Code, Codex, OpenCode or similar tools. Skills cover thesis and patent writing, drawio and Excalidraw diagrams, drawio-to-pptx slides, WeChat article writing, project docs, PDF and Office handling, and a five-step dev workflow. Docs and example prompts are in Chinese.

- **+** Plain SKILL.md folders; agents trigger them from the description field without manual selection
- **+** Covers niche Chinese workflows: thesis, invention patents, defense PPT, WeChat articles
- **+** Preview folder includes drawio and pptx source files for diagrams and slides
- **+** Lists skills directories for Cursor, Claude Code, Codex and OpenCode
- **−** README and example prompts are in Chinese only
- **−** No installer or package; skills are copied manually
- **−** Install paths in README are hardcoded Windows user paths
- **−** Per-skill dependencies (pandoc, drawio export, Office COM) are not listed centrally

<sub>no GPU · Needs pandoc, markitdown, docx-js, pptxgenjs, openpyxl, draw.io · [Repo](https://github.com/xstongxue/best-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/best-skills/)</sub>

<a name="appllama-skills"></a>
### #&#8288;216 [appllama-skills](https://github.com/appllama/appllama-skills) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Sep 2026</sub>

**Agent skills for building native-feeling Expo and React Native apps.**

Two agent skills installed via `npx skills`: one researches top-grossing mobile apps through the Appllama MCP, the other builds Expo / React Native screens to an Apple HIG bar. The design skill covers navigation, motion rules and a simulator loop that records whole flows. It works with Claude Code, Cursor, Codex and other agents that load skills.

- **+** Design skill installs alone and works without the MCP connected
- **+** Concrete build rules: push vs replace, sheets, springs with velocity, no JS-thread animation
- **+** Simulator loop records and reviews full flows, not single screenshots
- **+** Plain skill directories; can be copied manually into .claude/skills/
- **−** Research skill needs the Appllama MCP, which is part of the paid Pro plan
- **−** Each MCP call spends one credit; credits reset monthly
- **−** Build guidance targets Expo / React Native and iOS conventions only
- **−** No tagged release; the MCP backend is a hosted service

<sub>no GPU · Needs Appllama MCP (https://mcp.appllama.io/mcp, Pro plan), Node.js (npx), iOS simulator, Expo / React Native · Models: Claude Code, Cursor, Codex · [Repo](https://github.com/appllama/appllama-skills) · [📖 Docs ↗](https://appllama.io/mcp) · [🌐 Site ↗](https://appllama.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/appllama-skills/)</sub>

<a name="fable-method"></a>
### #&#8288;217 [fable-method](https://github.com/sahir619/fable-method) <sub>score [44](../README.md#-how-we-rank "Score 44/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Oct 2026</sub>

**Claude Code plugin with four skills for a classify, verify, report workflow.**

Packages a stepwise agent workflow as four skills: fable-method (classify the ask, define done, gather evidence, decide, act, verify, report), fable-loop (orchestrated subagent run), fable-judge (adversarial check of finished work) and fable-domain (generates domain adapters). Installs as a Claude Code plugin or Codex skills, with AGENTS.md for other harnesses. The repo includes eval logs from fifteen rounds and 260+ runs, self-described as smoke-test grade.

- **+** Every rule is tied to a committed eval transcript and per-scenario case study
- **+** fable-judge re-runs claimed checks and diffs changes to catch false completion reports
- **+** Installs as a Claude Code plugin, Codex skills, or AGENTS.md for other agents
- **+** Eight domain adapters load lazily; eval nulls and failures are logged beside the wins
- **−** Evals are 1-4 runs per cell with LLM judges; the README calls them smoke-test grade
- **−** No measured lift on ordinary small tasks with capable models
- **−** Haiku surfaced the skipped-deploy decision in only 1 of 12 runs
- **−** Seven of the eight domain adapters lack sourced references; medical has none

<sub>no GPU · Needs Claude Code or Codex · Models: Claude Haiku, Claude Sonnet, Claude Opus · [Repo](https://github.com/sahir619/fable-method) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fable-method/)</sub>

<a name="opensrc"></a>
### #&#8288;218 [opensrc](https://github.com/vercel-labs/opensrc) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Sep 2026</sub>

**CLI that fetches and caches package source for coding agents to read.**

opensrc is a Rust CLI that downloads the source code of a package from npm, PyPI, crates.io or GitHub and caches it locally. `opensrc path <package>` fetches on first use and returns the cached directory, so agents can run rg, cat or find against dependency source. The repo is a Turborepo monorepo that also contains a Next.js docs site.

- **+** Returns a plain filesystem path, so it works with rg, cat, find and any agent
- **+** Covers npm, PyPI, crates.io and GitHub through one command
- **+** Caches after first fetch, so repeat lookups return the path instantly
- **+** Apache-2.0 licensed, with a CLI written in Rust
- **−** Not an MCP server; agents must run shell commands themselves
- **−** README does not describe cache location, size limits or eviction
- **−** Registries beyond npm, PyPI, crates.io and GitHub are not listed
- **−** Labeled a Vercel Labs experiment, so stability guarantees are unknown

<sub>no GPU · Needs Node.js 24+ and pnpm 11 (development only), npm (install) · [Repo](https://github.com/vercel-labs/opensrc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opensrc/)</sub>

<a name="context-engineering-intro"></a>
### #&#8288;219 [context-engineering-intro](https://github.com/coleam00/context-engineering-intro) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (72) · Freshness: recent (53) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Mar 2026</sub>

**Claude Code template for generating and executing feature specs called PRPs.**

A file template for Claude Code that adds two custom slash commands, /generate-prp and /execute-prp. The first turns a feature request in INITIAL.md into a Product Requirements Prompt after researching the codebase and docs. The second implements it with test and lint validation loops. It also ships a CLAUDE.md rules file, a base PRP template and an examples/ folder convention.

- **+** Small file-based setup: two command files, CLAUDE.md and templates, easy to read and adapt
- **+** PRPs include validation gates so the agent runs tests and linting and iterates
- **+** Includes a complete example PRP and a sample INITIAL.md
- **+** MIT licensed
- **−** Written for Claude Code; other assistants would need the commands ported
- **−** README states it does not cover RAG or tool use
- **−** No releases and no automated checks of generated PRPs; quality depends on the model
- **−** The examples/ folder is empty by default; results depend on examples you add

<sub>no GPU · Needs Claude Code · Models: Claude (via Claude Code) · [Repo](https://github.com/coleam00/context-engineering-intro) · [📖 Docs ↗](https://docs.anthropic.com/en/docs/claude-code) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-engineering-intro/)</sub>

<a name="openskills"></a>
### #&#8288;220 [openskills](https://github.com/numman-ali/openskills) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: popular (67) · Freshness: slowing (45) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Jan 2026</sub>

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

<a name="opc-skills"></a>
### #&#8288;221 [opc-skills](https://github.com/resciencelab/opc-skills) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (7) · Freshness: active (95) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

**Collection of agent skills for indie hackers: SEO, Reddit/X research, logos, domains.**

A set of ten SKILL.md-based skills for coding agents such as Claude Code, Cursor, Codex and Windsurf. They cover SEO/GEO optimization, Reddit, Twitter/X and Product Hunt search, domain price comparison, logo and banner creation, image generation with Gemini 3 Pro Image, and archiving session learnings. Install via the Claude Code plugin marketplace or `npx skills add`.

- **+** Installs through Claude Code marketplace or `npx skills add` for 16+ agents
- **+** Each skill is a self-contained folder with SKILL.md, following the Agent Skills standard
- **+** Includes a template directory for writing and contributing new skills
- **+** Covers non-coding solopreneur tasks: demand research, domain search, branding assets
- **−** Some skills depend on others, e.g. domain-hunter needs twitter and reddit
- **−** Twitter skill relies on twitterapi.io; image skills rely on Gemini, so API keys likely needed
- **−** README license badge says MIT while the license section says Apache 2.0
- **−** Only ten skills, focused on a narrow solopreneur workflow

<sub>no GPU · Needs twitterapi.io, Reddit public JSON API, Gemini 3 Pro Image (Nano Banana Pro), Claude Code or another skills-compatible agent · Models: Gemini 3 Pro Image · [Repo](https://github.com/resciencelab/opc-skills) · [📖 Docs ↗](https://deepwiki.com/ReScienceLab/opc-skills) · [🌐 Site ↗](https://opc.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opc-skills/)</sub>

<a name="loopy"></a>
### #&#8288;222 [loopy](https://github.com/forward-future/loopy) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (30) · Freshness: active (94) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Jul 2026</sub>

**Agent skill and catalog of bounded, self-checking prompt loops.**

Loopy is an installable skill for Codex, Cursor and Claude Code that finds, audits, crafts, runs, debriefs, saves and publishes "loops": prompts with a verification check and a stopping rule. It works against the Loop Library website, a Cloudflare Worker-backed catalog of published loops that agents can also read as JSON and plain text. Saved loops go into a project-level LOOPS.md.

- **+** Installs with one npx command for Codex, Cursor or Claude Code
- **+** Catalog is readable without the skill via catalog.json, catalog.txt and llms.txt
- **+** Run mode is bounded and returns a receipt with evidence and stopping reason
- **+** Saving and publishing require explicit approval of the exact preview
- **−** Loop records are not in the repo; the catalog lives in a private Cloudflare database
- **−** Needs Node.js and npx for install
- **−** Recommendations and publishing depend on the hosted signals.forwardfuture.com site
- **−** No tagged releases

<sub>no GPU · Needs Node.js, npx, Cloudflare Workers (website only) · Models: Codex, Cursor, Claude Code · port 4173 · [Repo](https://github.com/forward-future/loopy) · [▶️ Demo ↗](https://signals.forwardfuture.com/loop-library/) · [📖 Docs ↗](https://signals.forwardfuture.com/loop-library/agents/) · [🌐 Site ↗](https://signals.forwardfuture.com/loop-library/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/loopy/)</sub>

<a name="typesafe-ai-skills"></a>
### #&#8288;223 [skills](https://github.com/typesafe-ai/skills) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Sep 2026</sub>

**Agent skill that teaches coding agents to build with the TypeSafe API.**

A single skill, typesafe-ai, that guides coding agents in designing TypeSafe workflows, finding current docs and cookbooks, and composing typed judgments in code. It installs as a Claude Code plugin or through skills.sh for other agents. It is a client-side add-on for the TypeSafe service, which returns typed decisions and probabilities from System One models.

- **+** Two install paths: Claude Code plugin marketplace and npx skills for other agents
- **+** Installs project-local by default, with -g for global install
- **+** MIT license, with the skill readable as plain SKILL.md
- **−** Only useful with the TypeSafe service; pricing and API terms are not in the README
- **−** Contains one skill only
- **−** README does not list supported agents beyond Claude Code
- **−** No releases published

<sub>no GPU · Needs TypeSafe service, Claude Code or skills.sh-compatible agent, Node.js (npx) · Models: TypeSafe System One models · [Repo](https://github.com/typesafe-ai/skills) · [📖 Docs ↗](https://docs.typesafe.ai/agent-skill#installation) · [🌐 Site ↗](https://typesafe.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typesafe-ai-skills/)</sub>

<a name="typeui"></a>
### #&#8288;224 [typeui](https://github.com/bergside/typeui) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: niche (13) · Freshness: active (95) · Maintenance: weak (22) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · custom license · Jul 2026</sub>

**Design skills and UI prompts that AI coding tools load via MCP.**

TypeUI is a library of design skills and UI prompts, published as DESIGN.md and SKILL.md files, that you feed to AI coding tools to get more consistent interfaces. It is delivered through a hosted TypeUI MCP server and plugins, with setup guides for about 25 tools including Codex, Claude, Cursor, VS Code Copilot, Windsurf, Zed, Lovable, Replit and v0. Any model works if it accepts markdown or general prompting.

- **+** Skills ship as plain DESIGN.md and SKILL.md files, usable with any markdown-aware tool
- **+** Per-tool install guides for about 25 hosts, including Cursor, Codex, Claude and Zed
- **+** Large catalog of named visual styles, such as Bento, Brutalism and Glassmorphism, with previews
- **−** MCP setup points to a hosted TypeUI server; self-hosting is not described in the README
- **−** License is reported as NOASSERTION, so reuse terms are unclear
- **−** Output quality depends on the host model; the README gives no benchmarks
- **−** README is truncated here, so skill counts and pricing are unknown

<sub>no GPU · Needs TypeUI hosted MCP server · Models: Any provider that supports markdown files or prompting · [Repo](https://github.com/bergside/typeui) · [📖 Docs ↗](https://www.typeui.sh/docs/guides/claude) · [🌐 Site ↗](https://www.typeui.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/typeui/)</sub>

<a name="beautify-github-readme"></a>
### #&#8288;225 [beautify-github-readme](https://github.com/oil-oil/beautify-github-readme) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Agent skill that redesigns GitHub READMEs with SVG heroes and Markdown.**

An installable skill for coding agents that reads a repository, then restructures its README or produces only visual assets such as SVG heroes, section headers, workflow diagrams and optional GIFs. Visuals live in SVG while explanations, commands and links stay in Markdown. It has whole-README and asset-only modes plus a read-only audit, and does not commit or push without approval.

- **+** Asset-only mode leaves README copy, order and links untouched
- **+** Keeps text in Markdown so the page stays searchable and copyable
- **+** Hybrid SVG plus AI-generated cutouts, with written production guides
- **+** Read-only audit mode; commits, pushes and PRs need explicit approval
- **−** Output quality depends on the host agent; no evaluation or benchmarks given
- **−** PNG/WebP or AI image generation needs separate rendering or image tools
- **−** GIF motion is opt-in and not generated by default
- **−** No docs site; part of the README is in Chinese

<sub>no GPU · Needs Node.js (npx skills add), Agent that supports skills, Optional image generation tool · [Repo](https://github.com/oil-oil/beautify-github-readme) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beautify-github-readme/)</sub>

<a name="awesome-openclaw-agents"></a>
### #&#8288;226 [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: known (41) · Freshness: active (83) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · May 2026</sub>

**205 copy-paste SOUL.md agent templates for OpenClaw.**

A curated repository of SOUL.md persona files for OpenClaw agents, grouped into 24 categories such as productivity, development, marketing, finance and security. A template is registered with `openclaw agents add`, and a small Node quickstart (`bot.js`) can run one. The README also lists use cases, MCP servers, model configs and a machine-readable agents.json, and links to the paid CrewClaw service for deploy packages.

- **+** 205 templates across 24 categories, each a plain SOUL.md file
- **+** Machine-readable agents.json index alongside the templates
- **+** MIT license; Node quickstart runs a template with npm install and node bot.js
- **+** Extra material: model configs, use cases, MCP server list, troubleshooting
- **−** Only useful with the OpenClaw runtime; templates are not standalone agents
- **−** README promotes the commercial CrewClaw deploy service throughout
- **−** README counts conflict: says 205 agents but also 'All 100 agents'
- **−** Templates are prompt files only; no tests or per-template versioning shown

<sub>Needs OpenClaw, Node.js · Models: Ollama Cloud, GLM-5.1, Minimax M2.7, GPT-5.4 · [Repo](https://github.com/mergisi/awesome-openclaw-agents) · [🌐 Site ↗](https://crewclaw.com/create-agent) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-openclaw-agents/)</sub>

<a name="awesome-design-skills"></a>
### #&#8288;227 [awesome-design-skills](https://github.com/bergside/awesome-design-skills) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: known (32) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Jun 2026</sub>

**Registry of 67 design-system skill files for AI coding agents.**

A catalog of 67 named visual styles (Brutalism, Glassmorphism, Material, Neobrutalism and others), each packaged as a folder with SKILL.md for agent instructions and DESIGN.md for human-readable rationale. A skill is pulled into a project with `npx typeui.sh pull <name>`, and previews are hosted on typeui.sh. Targets Claude Code, Cursor, Codex and similar tools.

- **+** One-command install per skill via npx typeui.sh pull
- **+** Each skill pairs agent rules (SKILL.md) with human-readable DESIGN.md
- **+** SKILL.md covers tokens, component rules, accessibility constraints and quality gates
- **+** MIT license; visual previews for every style on typeui.sh
- **−** Installation depends on the typeui.sh CLI and registry, not plain git
- **−** Only 67 predefined styles; customization process is unknown from the README
- **−** No stated evaluation of output quality across agents
- **−** README shown is truncated, so the full style list is unverified

<sub>no GPU · Needs Node.js (npx), typeui.sh CLI · Models: Claude Code, Cursor, Codex · [Repo](https://github.com/bergside/awesome-design-skills) · [▶️ Demo ↗](https://typeui.sh/design-skills) · [🌐 Site ↗](https://typeui.sh/design-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-design-skills/)</sub>

<a name="harmonist"></a>
### #&#8288;228 [harmonist](https://github.com/gammalabtechnologies/harmonist) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: niche (13) · Freshness: active (89) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Jun 2026</sub>

**Hook-enforced agent protocol pack for Cursor, Claude Code and other coding assistants.**

Harmonist installs 193 markdown agent definitions plus IDE hooks into a project. The stop hook blocks a code-changing turn until a reviewer such as qa-verifier has run and session-handoff.md is updated, with a retry cap of 3. Memory writes go through a schema-validated, secret-scanning CLI, and shipped files are checked against a SHA-256 manifest before install.

- **+** Stop hook gates turns on reviewer runs and memory updates, not on prompt wording
- **+** Pure Python 3.9+ stdlib; no npm, Docker or database; runs on native Windows
- **+** MANIFEST.sha256 check refuses tampered agent files during upgrade and extras install
- **+** Memory entries are schema-validated and scanned for about 30 secret patterns
- **−** Primary integration targets Cursor; other assistants go through adapters of unstated maturity
- **−** PROTOCOL-SKIP lets the model bypass the gate; only skip-rate warnings check it
- **−** Needs an assistant that supports subagent dispatch and hooks
- **−** Integration is done by an AI following a prompt, so results depend on the model

<sub>no GPU · Needs Python 3.9+, Git, Bash 3.2+ (optional), AI coding assistant with subagent support · Models: Cursor, Claude Code, Copilot, Windsurf, Aider · [Repo](https://github.com/gammalabtechnologies/harmonist) · [🌐 Site ↗](https://gammalab.ae) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/harmonist/)</sub>

<a name="claude-code-proxy"></a>
### #&#8288;229 [claude-code-proxy](https://github.com/fuergaosi233/claude-code-proxy) <sub>score [30](../README.md#-how-we-rank "Score 30/100. Adoption: niche (23) · Freshness: recent (52) · Maintenance: weak (11) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Mar 2026</sub>

**Proxy that lets the Claude Code CLI use OpenAI-compatible APIs.**

A Python server that exposes the Anthropic /v1/messages endpoint and translates requests into OpenAI-style API calls, so the Claude Code CLI can run against OpenAI, Azure OpenAI, Ollama or any compatible provider. Requests for haiku, sonnet and opus models are mapped to configurable SMALL_MODEL, MIDDLE_MODEL and BIG_MODEL values. Tool calls, SSE streaming and base64 images are converted.

- **+** Maps haiku, sonnet and opus requests to separate backend models via env vars
- **+** Converts tool use, SSE streaming and base64 image input
- **+** Works with OpenAI, Azure OpenAI, Ollama or any OpenAI-compatible base URL
- **+** Optional ANTHROPIC_API_KEY setting restricts which clients can use the proxy
- **−** MAX_TOKENS_LIMIT defaults to 4096, which may cut long Claude Code outputs
- **−** No tagged releases
- **−** Only one test script is mentioned; coverage is unknown
- **−** README describes MIDDLE_MODEL inconsistently (opus in one place, sonnet in another)

<sub>no GPU · Docker + Compose · Needs OpenAI-compatible API provider, Claude Code CLI · Models: OpenAI, Azure OpenAI, Ollama, OpenAI-compatible APIs · port 8082 · [Repo](https://github.com/fuergaosi233/claude-code-proxy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-proxy/)</sub>

<a name="myclaude"></a>
### #&#8288;230 [myclaude](https://github.com/stellarlinkco/myclaude) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (22) · Freshness: recent (75) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · AGPL-3.0 · May 2026</sub>

**Claude Code slash-command workflows that delegate coding to Codex, Gemini or OpenCode.**

Installs Claude Code modules (do, omo, bmad, requirements, essentials, sparv) as slash commands, skills, agents and hooks under ~/.claude. Claude Code orchestrates, while a Go binary, codeagent-wrapper, hands code editing and test runs to the Codex, Claude, Gemini or OpenCode CLI. Installed with an npx installer that has --list and --update options.

- **+** Routes execution to Codex, Claude, Gemini or OpenCode through one wrapper binary
- **+** Modules can be enabled or disabled individually in config.json
- **+** npx installer supports --list, --update and a custom --install-dir
- **+** Includes a 5-phase /do workflow plus 11 basic commands such as /code and /debug
- **−** Requires the chosen backend CLIs installed and supporting specific flags
- **−** AGPL-3.0 license; commercial use without AGPL terms needs a separate agreement
- **−** Several overlapping workflows (do, omo, bmad, requirements) make the choice unclear
- **−** Known issues: Gemini cannot read .gitignore files, Codex may need approval_policy set

<sub>no GPU · Needs Claude Code, Node.js (npx), Codex CLI, Gemini CLI, OpenCode CLI · Models: Codex, Claude, Gemini, OpenCode · [Repo](https://github.com/stellarlinkco/myclaude) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/myclaude/)</sub>

<a name="agent-toolkit"></a>
### #&#8288;231 [agent-toolkit](https://github.com/softaworks/agent-toolkit) <sub>score [27](../README.md#-how-we-rank "Score 27/100. Adoption: niche (19) · Freshness: slowing (49) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Mar 2026</sub>

**Claude Code skills, sub-agents and slash commands, installable as plugins.**

A marketplace repo of about 40 skills in the Agent Skills format, plus six sub-agents and seven slash commands. Skills cover diagrams and docs, React and MUI, database schema design, git commits, Jira, Datadog and writing style. Each item installs separately through the Claude Code plugin marketplace, or all at once with `npx skills add`.

- **+** Each skill, agent and command installs individually as its own plugin
- **+** Skills also install in Codex, Cursor and AdaL via `npx skills add`
- **+** Each skill ships a SKILL.md for the agent and a README with examples
- **+** Skills can be copied by hand into ~/.claude/skills
- **−** Agents and slash commands work only in Claude Code CLI
- **−** Opinionated selection from a single maintainer; no tests or quality checks described
- **−** Some skills need outside tools or services (Codex, Gemini, Perplexity, Jira, Datadog)
- **−** No tagged releases, so versioning is unknown

<sub>no GPU · Needs Claude Code, Node.js (npx) · Models: Claude Code, Codex, Cursor, AdaL · [Repo](https://github.com/softaworks/agent-toolkit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-toolkit/)</sub>

<a name="continuous-claude-v3"></a>
### #&#8288;232 [continuous-claude-v3](https://github.com/parcadei/continuous-claude-v3) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: known (40) · Freshness: slowing (35) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Jan 2026</sub>

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

<a name="taches-cc-resources"></a>
### #&#8288;233 [taches-cc-resources](https://github.com/glittercowboy/taches-cc-resources) <sub>score [21](../README.md#-how-we-rank "Score 21/100. Adoption: niche (10) · Freshness: recent (59) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Apr 2026</sub>

**Claude Code commands, skills and auditor subagents for planning and debugging.**

A Claude Code plugin bundling 27 slash commands, 9 skills and 3 auditor subagents. It covers meta-prompting (/create-prompt, /run-prompt), hierarchical project planning (create-plans), todo capture, context handoff and a debugging methodology. Other skills generate new skills, hooks, subagents and MCP servers. It installs through the Claude Code plugin marketplace or by copying files into ~/.claude.

- **+** Installs as a Claude Code plugin with two commands, or by copying files into ~/.claude
- **+** Auditor subagents review skills, commands and subagent configs for structure and compliance
- **+** create-plans skill turns a brief into ROADMAP and PLAN.md files that Claude executes
- **+** Includes MCP server generation for Python and TypeScript, and a Ralph loop setup skill
- **−** Works only with Claude Code; the OpenCode port is a separate community repo
- **−** No release tags; versioning is by commit only
- **−** Thinking-model commands are prompt templates; no tests or benchmarks are shown
- **−** Domain expertise skills are not included; you must create them yourself

<sub>no GPU · Needs Claude Code · Models: Claude · [Repo](https://github.com/glittercowboy/taches-cc-resources) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taches-cc-resources/)</sub>

<a name="vibekit"></a>
### #&#8288;234 [vibekit](https://github.com/superagent-ai/vibekit) <sub>score [6](../README.md#-how-we-rank "Score 6/100. Adoption: niche (7) · Freshness: quiet (13) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2025</sub>

**CLI that runs coding agents in sandboxes with secret redaction.**

VibeKit is an npm CLI that wraps coding agents such as Claude Code, Gemini CLI, Grok CLI, Codex CLI and OpenCode, running their output in isolated Docker containers. It redacts secrets and API keys from completions and records logs, traces and metrics of agent operations. Separate packages, @vibe-kit/sdk and @vibe-kit/auth, are provided for embedding it in applications.

- **+** Wraps several agent CLIs (Claude Code, Gemini, Codex, Grok, OpenCode) behind one command
- **+** Local Docker sandboxing; README says no cloud dependency is required
- **+** Redacts secrets and API keys from agent output
- **+** Separate SDK package for running agents in sandboxes from application code
- **−** Needs Docker locally for the sandbox; the README does not list setup steps
- **−** Redaction rules and detection coverage are not documented in the README
- **−** Last release was 2025-08-04, while the last commit is 2025-11-10
- **−** Where observability data is stored or viewed is not described in the README

<sub>no GPU · Needs Docker, Node.js · Models: Claude Code, Gemini CLI, Grok CLI, Codex CLI, OpenCode · [Repo](https://github.com/superagent-ai/vibekit) · [📖 Docs ↗](https://docs.vibekit.sh) · [🌐 Site ↗](https://vibekit.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibekit/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
