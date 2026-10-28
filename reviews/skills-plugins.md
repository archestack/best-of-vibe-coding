# 🧩 Skills, plugins and prompts reviews · Best of Vibe Coding

Add-ons that make coding agents better (skills, plugins, rules, hooks, memory) and prompt collections to learn from or reuse. Back to the [leaderboard](../README.md#-skills-plugins-and-prompts).

<sub>🌐 Also on the web: [Skills, plugins and prompts on archestack.com](https://archestack.com/best-of-vibe-coding/skills-plugins/), each project on its own page.</sub>

<a name="impeccable"></a>
### 🥇 [impeccable](https://github.com/pbakaus/impeccable) <sub>score [96](../README.md#-how-we-rank "Score 96/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 91k · Apache-2.0 · Oct 2026</sub>

**Design skill with 24 slash commands for AI coding agents' frontend output.**

Impeccable installs a single `/impeccable` skill into coding agents such as Claude Code, Cursor, Codex CLI, Gemini CLI and GitHub Copilot. It adds 24 commands (audit, critique, polish, typeset, layout and others), a live browser variant mode, and 61 deterministic detector rules for common AI-generated design tells. `/impeccable init` writes a PRODUCT.md that later commands use as context.

- **+** Installs into many agents: Claude Code, Cursor, Codex, Gemini CLI, Copilot, Grok Build, Hermes and more
- **+** 61 detector rules run in the CLI and browser extension with no LLM or API key
- **+** Edit hooks surface detector findings back to the agent on Claude Code, Copilot, Codex, Cursor and Grok
- **+** Apache-2.0, with npx, git submodule, plugin and manual copy install options
- **−** Skill runs through a separate binary downloaded on first run into ~/.impeccable/bin/
- **−** Design roll requests go to impeccable.style and telemetry is on unless you opt out
- **−** Hooks need per-harness trust approval, and Hermes and Veto get no edit hook
- **−** Writes many working files under .impeccable/ that need a manual .gitignore block

<sub>no GPU · Needs Node.js (only for the npx installer), An AI coding tool such as Claude Code, Cursor or Codex CLI, impeccable.style roll API (telemetry can be disabled) · safety checks passed 11 of 12 · [Repo](https://github.com/pbakaus/impeccable) · [▶️ Demo ↗](https://impeccable.style/cases/neo-mirai) · [📖 Docs ↗](https://impeccable.style) · [🌐 Site ↗](https://impeccable.style) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/impeccable/)</sub>

<a name="caveman"></a>
### 🥈 [caveman](https://github.com/juliusbrussee/caveman) <sub>score [95](../README.md#-how-we-rank "Score 95/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 116k · Apache-2.0 · Oct 2026</sub>

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
### 🥉 [skills](https://github.com/mattpocock/skills) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 305k · MIT · Oct 2026</sub>

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
### #&#8288;4 [ecc](https://github.com/affaan-m/ecc) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 291k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 18+, Git, Claude Code 2.1+ (for plugin setup) · Models: Claude Code, Codex, Kimi Code, Cursor, OpenCode · safety checks passed 11 of 12 · [Repo](https://github.com/affaan-m/ecc) · [🌐 Site ↗](https://ecc.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ecc/)</sub>

<a name="oh-my-claudecode"></a>
### #&#8288;5 [oh-my-claudecode](https://github.com/yeachan-heo/oh-my-claudecode) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

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
### #&#8288;6 [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 142k · MIT · Oct 2026</sub>

**Design-system skill for AI coding assistants, with searchable styles, palettes and fonts.**

Installs as a skill or plugin for coding assistants such as Claude Code, Cursor, Windsurf, Codex CLI and Gemini CLI. A Python script using BM25 search and 192 reasoning rules returns a design system for a given product type: landing pattern, style, colors, typography, effects, anti-patterns and a pre-delivery checklist. The data covers 79 UI styles (50 active), 192 palettes, 74 font pairings and guidelines for 22 stacks.

- **+** Installs into 20+ assistants via the uipro CLI, or as a Claude Code plugin
- **+** Search script uses only the Python standard library and makes no network calls
- **+** Output includes anti-patterns and an accessibility-oriented checklist, not only palettes and fonts
- **+** Covers 22 stacks, from React and Vue to SwiftUI, Flutter and WPF
- **−** Requires Python 3 on the machine to run the search script
- **−** Brand identity, logo and asset generation are in the paid premium version only
- **−** Only 50 of 79 styles are active in default recommendations
- **−** Output quality depends on the host assistant following the skill; no tests or benchmarks stated

<sub>no GPU · Needs Python 3, Node.js and npm (for the uipro CLI) · safety checks passed 11 of 11 · [Repo](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) · [🌐 Site ↗](https://uupm.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui-ux-pro-max-skill/)</sub>

<a name="book-to-skill"></a>
### #&#8288;7 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 36k · MIT · Oct 2026</sub>

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

<a name="agent-skills"></a>
### #&#8288;8 [agent-skills](https://github.com/addyosmani/agent-skills) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 111k · MIT · Oct 2026</sub>

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
### #&#8288;9 [claude-mem](https://github.com/thedotmack/claude-mem) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 104k · Apache-2.0 · Oct 2026</sub>

**Persistent cross-session memory plugin for Claude Code and other coding agents.**

Claude-mem hooks into Claude Code's lifecycle events (SessionStart, UserPromptSubmit, PreToolUse, PostToolUse, Stop, SessionEnd) to capture tool-usage observations, summarize them, and inject relevant context into later sessions. Data is stored in SQLite with FTS5 and Chroma for hybrid search, served by a local Bun-managed worker with a web viewer. Search is exposed through three MCP tools (search, timeline, get_observations). Installers also exist for OpenCode, T3 Code, Antigravity, OMP, Pi and OpenClaw.

- **+** Local SQLite plus Chroma storage with a worker HTTP API and web viewer
- **+** Three-step search/timeline/get_observations flow filters before fetching full details, cutting tokens
- **+** Installers for several harnesses besides Claude Code, including OpenCode, T3 Code and OpenClaw
- **+** `<private>` tags exclude sensitive content from storage
- **−** Installer prompts for sign-in to a hosted observer with a 30-day trial; opt-out needs flags
- **−** Depends on Node 20+, Bun and uv, auto-installed if missing
- **−** `npm install -g claude-mem` gives only the SDK, not the hooks or worker
- **−** Some features, such as TeamBrain and cloud sync, rely on the hosted cmem.ai service

<sub>no GPU · Docker + Compose · Needs Node.js >=20, Bun, uv, SQLite, Chroma · Models: Anthropic plan, OpenRouter, Gemini, claude-mem observer · safety checks passed 10 of 11 · [Repo](https://github.com/thedotmack/claude-mem) · [📖 Docs ↗](https://docs.claude-mem.ai/) · [🌐 Site ↗](https://cmem.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-mem/)</sub>

<a name="archify"></a>
### #&#8288;10 [archify](https://github.com/tt-a1i/archify) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 91k · Apache-2.0 · Oct 2026</sub>

**Agent skill that turns descriptions or repos into interactive HTML diagrams.**

Archify is a skill for coding agents (Cursor, Claude Code, Codex CLI, OpenCode) that generates self-contained interactive HTML diagrams from a text description or from a repository the agent reads. It also builds one-page explainer answers with tables, steps and validated diagrams. Output has light and dark themes, route and reach tracing, and PNG, WebP, JPG or PDF export.

- **+** Output is one standalone HTML file; viewing needs no Archify install
- **+** Installs with one command: npx skills add tt-a1i/archify -g
- **+** Works from a description alone, or from a repo with source excerpts pinned to a commit
- **+** Exports PNG, WebP, JPG and PDF, plus route and reach share cards
- **−** Needs a separate AI coding agent to generate diagrams; not standalone
- **−** Optional update check contacts a remote manifest unless ARCHIFY_UPDATE_CHECK_DISABLED=1
- **−** README carries many sponsor and API-relay promotions
- **−** Diagram quality depends on the host agent's model; no benchmarks given

<sub>no GPU · Needs Node.js (npx), Claude Code, Codex CLI, Cursor or OpenCode · safety checks passed 11 of 11 · [Repo](https://github.com/tt-a1i/archify) · [▶️ Demo ↗](https://archify.si/gallery.html) · [📖 Docs ↗](https://archify.si/guide.html) · [🌐 Site ↗](https://archify.si) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archify/)</sub>

<a name="ruflo"></a>
### #&#8288;11 [ruflo](https://github.com/ruvnet/ruflo) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 80k · MIT · Oct 2026</sub>

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

<sub>Needs Node.js/npx, Claude Code or Codex · Models: Claude, Codex, Ollama (via ruflo-ruvllm) · safety checks passed 15 of 18 · [Repo](https://github.com/ruvnet/ruflo) · [▶️ Demo ↗](https://raw.githubusercontent.com/ruvnet/ruflo/main/docs/assets/ruflo-console-theme-compact.svg) · [📖 Docs ↗](https://github.com/ruvnet/ruflo/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://cognitum.one/agentic-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruflo/)</sub>

<a name="context-mode"></a>
### #&#8288;12 [context-mode](https://github.com/mksglu/context-mode) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · custom license · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js >= 22.5 or Bun · Models: Claude Code, Gemini CLI, VS Code Copilot, JetBrains Copilot, GitHub Copilot CLI · safety checks passed 11 of 17 · [Repo](https://github.com/mksglu/context-mode) · [🌐 Site ↗](https://context-mode.com/insight) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-mode/)</sub>

<a name="compound-engineering-plugin"></a>
### #&#8288;13 [compound-engineering-plugin](https://github.com/everyinc/compound-engineering-plugin) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

**Plugin of 36 skills for coding agents: plan, build, review, capture learnings.**

A plugin of 36 skills for AI coding agents that runs a loop of brainstorm, plan, work, simplify, review and compound. The compound step writes learnings to docs/solutions/, which later brainstorm and plan runs read as context. It installs on 14 agent hosts, including Claude Code, Cursor and Codex, and includes an autonomous /lfg pipeline.

- **+** Runs on 14 agent hosts, including Claude Code, Cursor, Codex, Copilot and OpenCode
- **+** Captured learnings land in docs/solutions/ as plain files in the repo
- **+** Covers planning, multi-agent code review, git and PR workflow, and browser testing
- **+** Artifact folder location is configurable through the docs_root setting
- **−** Invocation syntax differs by host ($skill-name in Codex, /skill:name in omp)
- **−** Pi needs companion packages such as pi-subagents for subagent workflows
- **−** Compound Packs for org-wide rules are marked experimental
- **−** Some skills use Claude-style allowed-tools names Devin does not map, so it prompts

<sub>no GPU · Needs An AI coding agent host (Claude Code, Cursor, Codex, etc.) · safety checks passed 11 of 12 · [Repo](https://github.com/everyinc/compound-engineering-plugin) · [📖 Docs ↗](https://github.com/EveryInc/compound-engineering-plugin/blob/main/docs/guides/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/compound-engineering-plugin/)</sub>

<a name="spec-kit"></a>
### #&#8288;14 [spec-kit](https://github.com/github/spec-kit) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 143k · MIT · Oct 2026</sub>

**Spec-driven development toolkit and CLI for AI coding agents.**

Spec Kit installs a Python CLI (`specify`) that scaffolds a project with slash commands or skills for your coding agent. The core flow is constitution, specify, plan, tasks, implement, converge; bug-fixing and idea-assessment ship as optional extensions. Behavior is customized through extensions, presets, workflows, bundles and catalogs.

- **+** Works with multiple coding agents through integrations; GitHub Copilot is the documented example
- **+** Extensions, presets, workflows and bundles customize the process without forking
- **+** Bug-fix and assessment extensions write reports to .specify/ directories in the repo
- **+** Supports air-gapped use via local sources and self-hosted catalogs
- **−** Needs a separate supported coding agent; it does not run models itself
- **−** Steps are run one at a time in agent chat, with manual review
- **−** Invocation syntax differs per agent, so examples need translating
- **−** Community catalog components are unaudited and need manual source review

<sub>no GPU · Needs Python 3.11+, uv, a supported AI coding agent · safety checks passed 9 of 9 · [Repo](https://github.com/github/spec-kit) · [📖 Docs ↗](https://github.github.io/spec-kit/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spec-kit/)</sub>

<a name="agentic-awesome-skills"></a>
### #&#8288;15 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 49k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js/npm (npx installer), Codex or Claude Code for AAS Core MCP · safety checks passed 8 of 12 · [Repo](https://github.com/sickn33/agentic-awesome-skills) · [▶️ Demo ↗](https://aaskills.tech/workbench) · [📖 Docs ↗](https://github.com/sickn33/agentic-awesome-skills/blob/v19.7.0/docs/users/aas-core.md) · [🌐 Site ↗](https://aaskills.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentic-awesome-skills/)</sub>

<a name="notebooklm-py"></a>
### #&#8288;16 [notebooklm-py](https://github.com/teng-lin/notebooklm-py) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Google account, Google NotebookLM / Gemini Notebook, Playwright Chromium (for browser login) · Models: Google Gemini (via NotebookLM) · safety checks passed 9 of 10 · [Repo](https://github.com/teng-lin/notebooklm-py) · [▶️ Demo ↗](https://asciinema.org/a/767284) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/notebooklm-py/)</sub>

<a name="kami"></a>
### #&#8288;17 [kami](https://github.com/tw93/kami) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<a name="ponytail"></a>
### #&#8288;18 [ponytail](https://github.com/dietrichgebert/ponytail) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 178k · MIT · Oct 2026</sub>

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

<a name="gstack"></a>
### #&#8288;19 [gstack](https://github.com/garrytan/gstack) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 138k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Git, Bun 1.3.3+ (1.4.2 tested), Node.js (Windows only), Codex CLI (optional, outside reviews), OpenAI API key (optional, design binary) · Models: Claude (Opus 5.5), OpenAI GPT-6 Astra, OpenAI GPT-6.1 Sol, OpenAI gpt-5.5 and gpt-image-2 (design binary) · safety checks passed 9 of 11 · [Repo](https://github.com/garrytan/gstack) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gstack/)</sub>

<a name="claude-hud"></a>
### #&#8288;20 [claude-hud](https://github.com/jarrodwatts/claude-hud) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

**Claude Code status line plugin showing context, rate limits, tools and todos.**

Claude HUD is a Claude Code plugin that registers a status line command. It reads session data Claude Code passes on stdin (model, context window, cost, rate limits, prompt cache) and prints context and usage bars below the input. Optional tools, agents and todos lines are read from the session transcript and enabled through /claude-hud:configure.

- **+** Runs as Claude Code's status line; no tmux or separate window needed
- **+** Default two-line view shows model, git branch, context bar and rate-limit usage
- **+** Many config options: layout, thresholds, colors, element order, cost, git and jj status
- **+** Guided /claude-hud:configure flow previews changes; labels in English and Chinese
- **−** Works only with Claude Code, not other coding agents
- **−** Needs a JavaScript runtime; Windows users may have to install Node.js LTS
- **−** Third-party plugin updates are not automatic until auto-update is enabled
- **−** Tools, agents and todos lines are off by default

<sub>no GPU · Needs Claude Code, Node.js · Models: Claude, Bedrock, Vertex, MiniMax · safety checks passed 11 of 11 · [Repo](https://github.com/jarrodwatts/claude-hud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-hud/)</sub>

<a name="claude-skills"></a>
### #&#8288;21 [claude-skills](https://github.com/alirezarezvani/claude-skills) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

**Library of 398 agent skills and plugins for Claude Code and 12 other tools.**

A collection of SKILL.md instruction packages, each paired with stdlib-only Python CLI scripts and reference docs. Domains include engineering, product, marketing, compliance, C-level advisory and research. It installs as Claude Code marketplace plugins, and scripts convert or sync the skills for Codex, Gemini CLI, Cursor, Aider, Windsurf and others.

- **+** Installs per domain or per skill through the Claude Code plugin marketplace
- **+** Python tools are stdlib-only, so no pip installs are needed
- **+** convert.sh and install.sh target Cursor, Aider, Windsurf, Kilo Code, OpenCode and Augment
- **+** Covers non-code domains such as regulatory, finance and research alongside engineering
- **−** README skill and tool counts disagree (345 vs 398 skills, 706 vs 766 tools)
- **−** Hermes Agent and Mistral Vibe need a manual local sync script
- **−** Windows needs symlink-enabled clone and PYTHONUTF8 or mirror trees break
- **−** Quality of individual skills is unverified; much of the catalog is outside coding

<sub>no GPU · Needs Python, Claude Code or another supported coding agent · safety checks passed 8 of 11 · [Repo](https://github.com/alirezarezvani/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-skills/)</sub>

<a name="ai-memory"></a>
### #&#8288;22 [ai-memory](https://github.com/akitaonrails/ai-memory) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Oct 2026</sub>

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

<a name="rtk"></a>
### #&#8288;23 [rtk](https://github.com/rtk-ai/rtk) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 85k · Apache-2.0 · Oct 2026</sub>

**Rust CLI that compresses shell command output before coding agents read it.**

RTK is a single Rust binary that rewrites shell commands such as git, pytest, cargo test and docker ps to filtered equivalents, so the agent reads grouped, truncated or deduplicated output. It installs hooks or rules for 18 coding tools including Claude Code, Cursor, Gemini CLI and Codex. An optional BUSL-licensed proxy daemon extends the same pipeline to provider API traffic.

- **+** Single binary with 100+ command filters and stated overhead under 10ms
- **+** Per-agent setup via `rtk init`, covering 18 tools including Claude Code, Cursor and Codex
- **+** `rtk gain` and `rtk discover` report savings and missed opportunities
- **+** Telemetry is off by default and sends nothing until opted in
- **−** Hook only fires on Bash tool calls; built-in Read, Grep and Glob bypass it
- **−** Token counts are estimated as bytes/4; only percentages are reliable
- **−** Mixed licensing: engine and proxy are BUSL-1.1, not Apache-2.0
- **−** Full and oss editions share the binary name and cannot be installed together

<sub>no GPU · safety checks passed 10 of 11 · [Repo](https://github.com/rtk-ai/rtk) · [📖 Docs ↗](https://www.rtk-ai.app/guide) · [🌐 Site ↗](https://www.rtk-ai.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rtk/)</sub>

<a name="openspec"></a>
### #&#8288;24 [openspec](https://github.com/fission-ai/openspec) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 73k · MIT · Oct 2026</sub>

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

<a name="repomix"></a>
### #&#8288;25 [repomix](https://github.com/yamadashy/repomix) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<a name="planning-with-files"></a>
### #&#8288;26 [planning-with-files](https://github.com/othmanadi/planning-with-files) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<a name="cc-switch"></a>
### #&#8288;27 [cc-switch](https://github.com/farion1231/cc-switch) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 150k · MIT · Oct 2026</sub>

**Desktop app that switches API providers and manages MCP and Skills for coding CLIs.**

CC Switch is a Tauri 2 desktop app for Windows, macOS and Linux, written in Rust. It switches API providers for Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build, OpenCode, OpenClaw, Hermes Agent, Pi and MiniMax Code, so you don't hand-edit their JSON, TOML or YAML config files. It also manages MCP servers, Skills and Prompts from one place.

- **+** Covers ten coding agents and CLIs from a single provider list
- **+** Removes manual edits of JSON, TOML and YAML config files
- **+** Also manages MCP servers, Skills and Prompts in the same app
- **+** Native installers for Windows, macOS and Linux; MIT licensed
- **−** README opens with a long sponsor list of API relay services
- **−** Desktop GUI only; no Docker image or headless server mode
- **−** Config-file format details and proxy behavior are not described in the README excerpt
- **−** Changes the config files of each supported tool, so a bug can affect all of them

<sub>no GPU · Models: Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build · safety checks passed 4 of 5 · [Repo](https://github.com/farion1231/cc-switch) · [📖 Docs ↗](https://github.com/farion1231/cc-switch/blob/main/docs/user-manual/en/README.md) · [🌐 Site ↗](https://ccswitch.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-switch/)</sub>

<a name="graphify"></a>
### #&#8288;28 [graphify](https://github.com/graphify-labs/graphify) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 137k · Apache-2.0 · Oct 2026</sub>

**Skill that maps a codebase and docs into a queryable knowledge graph.**

Graphify installs as a skill in AI coding assistants (Claude Code, Cursor, Codex, Gemini CLI and 20+ others). Running /graphify builds a knowledge graph of code, docs, PDFs, images and video, written to graph.html, GRAPH_REPORT.md and graph.json. Code is parsed locally with tree-sitter across about 40 languages, and the graph is queried with query, path and explain commands instead of grepping files.

- **+** Code parsing uses tree-sitter AST locally: no LLM, nothing leaves the machine
- **+** Every edge is tagged EXTRACTED or INFERRED, so provenance is checkable
- **+** One install registers the skill for 20+ assistants on macOS, Linux and Windows
- **+** Optional extras add an MCP stdio server, Neo4j and FalkorDB push, and watch mode
- **−** Docs, PDFs, images and video need an LLM backend or API key for the semantic pass
- **−** Cross-repo links, formal verification and Sentry/Jira connectors need paid Graphify Cloud
- **−** PDF, video, MCP and database support are separate extras to install
- **−** Benchmark figures are self-reported; the README only links to BENCHMARKS.md for details

<sub>no GPU · Docker · Needs Python 3.10+, uv or pipx · Models: Claude, OpenAI and compatible APIs, Gemini, Ollama, AWS Bedrock · safety checks passed 15 of 16 · [Repo](https://github.com/graphify-labs/graphify) · [📖 Docs ↗](https://docs.graphify.com) · [🌐 Site ↗](https://graphify.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphify/)</sub>

<a name="taste-skill"></a>
### #&#8288;29 [taste-skill](https://github.com/leonxlnx/taste-skill) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 104k · MIT · Oct 2026</sub>

**Agent Skill that makes coding agents design distinctive websites and app screens.**

Taste Skill is an Agent Skill (design-taste-frontend) that gives a coding agent an art direction, open-licensed photographs with credits, and a real-browser check of its own output. A script deals three of 20 researched directions, the agent builds, then inspects the page at three widths and fixes the top three problems over up to three rounds. Since v2.1 it also handles dashboards and app screens with separate style and checks.

- **+** Framework-agnostic: rules target design, so React, Vue, Svelte and plain HTML all work
- **+** Installs via npx skills, or as a Claude Code or Codex plugin
- **+** Checks pages in a real browser at three widths and fails on generic output
- **+** Images come from open collections (Wikimedia Commons, Openverse, Met) with credits placed on the page
- **−** A build takes roughly 30 to 45 minutes and a few hundred thousand tokens
- **−** Requires Node 22+ and a local Chrome, Edge or Chromium
- **−** Picture search needs network access
- **−** Output quality depends on the host coding agent; no benchmarks given

<sub>no GPU · Needs Node 22+, Chrome, Edge or Chromium, Network access for image search · safety checks passed 10 of 11 · [Repo](https://github.com/leonxlnx/taste-skill) · [🌐 Site ↗](https://tasteskill.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taste-skill/)</sub>

<a name="bmad-method"></a>
### #&#8288;30 [bmad-method](https://github.com/bmad-code-org/bmad-method) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 55k · custom license · Oct 2026</sub>

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

<a name="waza"></a>
### #&#8288;31 [waza](https://github.com/tw93/waza) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.4k · MIT · Oct 2026</sub>

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

<a name="reverse-skill"></a>
### #&#8288;32 [reverse-skill](https://github.com/zhaoxuya520/reverse-skill) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 44k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Java/JDK, Node.js 22.12+, Python 3.x, jadx, apktool, Frida, IDA Pro, radare2, Ghidra, Binary Ninja · safety checks passed 9 of 11 · [Repo](https://github.com/zhaoxuya520/reverse-skill) · [📖 Docs ↗](https://reverse.apivix.com/docs/) · [🌐 Site ↗](https://reverse.apivix.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/reverse-skill/)</sub>

<a name="beads"></a>
### #&#8288;33 [beads](https://github.com/gastownhall/beads) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Dolt, git (optional) · safety checks passed 10 of 12 · [Repo](https://github.com/gastownhall/beads) · [📖 Docs ↗](https://beads.gascity.com/) · [🌐 Site ↗](https://beads.gascity.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beads/)</sub>

<a name="opencodex"></a>
### #&#8288;34 [opencodex](https://github.com/lidge-jun/opencodex) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**Local proxy that lets Codex, Claude Code and Grok Build use any LLM.**

opencodex is a local proxy that translates Codex's Responses API into whatever a provider speaks, covering streaming, tool calls, reasoning tokens and images. It also fronts Claude Code, Claude Desktop and Grok Build, ships 40+ built-in providers plus any OpenAI-compatible endpoint, and serves a web dashboard on port 10100. It adds a ChatGPT account pool with quota-aware routing and combos for failover across providers.

- **+** 40+ built-in providers plus any OpenAI-compatible endpoint, chosen with provider/model syntax
- **+** One proxy covers Codex, Claude Code, Claude Desktop and Grok Build
- **+** Combos give one virtual model id with failover or weighted round-robin
- **+** `ocx stop` restores Codex's original configuration; caches bounded by a 256 MiB default budget
- **−** Desktop app is beta; Windows .msi code signing is still rolling out
- **−** Cursor provider is marked experimental
- **−** ChatGPT account pooling carries provider-policy and suspension risk, per the README's own note
- **−** JEV Auto routing is tested only against a mocked endpoint, not a live account

<sub>no GPU · Docker + Compose · Needs Node 18+ (Bun bundled), Docker Compose (optional) · Models: OpenAI, Anthropic, Google Gemini, xAI, Kimi · port 10100 · safety checks passed 9 of 10 · [Repo](https://github.com/lidge-jun/opencodex) · [📖 Docs ↗](https://opencodex.me/) · [🌐 Site ↗](https://opencodex.me/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencodex/)</sub>

<a name="openwiki"></a>
### #&#8288;35 [openwiki](https://github.com/langchain-ai/openwiki) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 22.22.0 or newer, A coding agent or a model provider · Models: Fourteen providers, including hosted models, Local OpenAI-compatible endpoints · port 4321 · safety checks passed 9 of 10 · [Repo](https://github.com/langchain-ai/openwiki) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openwiki/)</sub>

<a name="ouroboros"></a>
### #&#8288;36 [ouroboros](https://github.com/q00/ouroboros) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (100) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.3k · MIT · Oct 2026</sub>

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

<a name="zcf"></a>
### #&#8288;37 [zcf](https://github.com/ufomiao/zcf) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Oct 2026</sub>

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

<a name="oh-my-codex"></a>
### #&#8288;38 [oh-my-codex](https://github.com/yeachan-heo/oh-my-codex) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

**Workflow layer for OpenAI Codex CLI with skills, roles, and durable state.**

oh-my-codex (OMX) wraps the Codex CLI and keeps Codex as the execution engine. It adds skills such as $deep-interview, $ralplan, $ultragoal and $team, specialist roles, scoped AGENTS.md setup, and plans, logs and state stored under .omx/. It launches sessions in tmux with a HUD and can run each session in its own git worktree.

- **+** Staged flow from requirements interview to planning to durable goals, each stage usable alone
- **+** Named git worktree launches isolate concurrent sessions
- **+** Plans, logs, memory and mode state persist in .omx/ in the project
- **+** Ships a Codex plugin layout alongside the npm CLI
- **−** Only works on top of Codex CLI, which must be installed and authenticated
- **−** Tuned for macOS/Linux; native Windows and Codex App get less support
- **−** Recommended --madmax flag bypasses Codex approvals and sandbox
- **−** Setup scope and AGENTS.md merge policy rules are involved

<sub>no GPU · Needs Node.js 20+, OpenAI Codex CLI, tmux (recommended on macOS/Linux), git · Models: OpenAI models via Codex CLI · safety checks passed 11 of 12 · [Repo](https://github.com/yeachan-heo/oh-my-codex) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-codex-website/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-codex/)</sub>

<a name="plannotator"></a>
### #&#8288;39 [plannotator](https://github.com/backnotprop/plannotator) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.7k · Apache-2.0 · Oct 2026</sub>

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

<a name="vercel-labs-skills"></a>
### #&#8288;40 [skills](https://github.com/vercel-labs/skills) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 37k · MIT · Oct 2026</sub>

**CLI that installs reusable agent skills into Claude Code, Cursor and others.**

An npx-run CLI that finds, installs, updates and removes SKILL.md-based agent skills for about 79 coding agents, including OpenCode, Claude Code, Codex and Cursor. Skills install per project by default, or globally with -g. It also generates a prompt for one-off skill use, scaffolds new skills with init, and has an experimental sync for skills bundled in npm dependencies.

- **+** Supports 4 named agents plus 75 more, with detection of installed agents
- **+** Full lifecycle commands: find, add, list, check, update, remove, init
- **+** `skills use` runs a skill without installing it
- **+** Per-project install by default, global with -g
- **−** Requires Node.js 22.20 or later
- **−** npm dependency sync is experimental and may change
- **−** Collects anonymous telemetry unless DISABLE_TELEMETRY or DO_NOT_TRACK is set
- **−** Skill discovery relies on the skills.sh directory

<sub>no GPU · Needs Node.js 22.20+, npm · safety checks passed 8 of 10 · [Repo](https://github.com/vercel-labs/skills) · [📖 Docs ↗](https://github.com/vercel-labs/skills/blob/main/docs/commands.md) · [🌐 Site ↗](https://skills.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vercel-labs-skills/)</sub>

<a name="cc-haha"></a>
### #&#8288;41 [cc-haha](https://github.com/nanmicoder/cc-haha) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

**Electron desktop workbench for Claude Code with diff review and multi-session tabs.**

cc-haha is a macOS, Windows and Linux desktop app built around a Claude Code-based runtime, with session tabs, per-file diff review, an in-app browser preview and graphical permission approval. It connects to Claude, ChatGPT and Grok accounts, third-party APIs such as DeepSeek, Kimi and GLM, and local LM Studio or Ollama endpoints. It also covers MCP and SubAgent management, Computer Use, IM bridges and scheduled tasks. A CLI can be started from source with Bun.

- **+** Installers for macOS, Windows and Linux; CLI also runs from source with Bun
- **+** Model choice spans Claude, ChatGPT, Grok, preset third-party APIs and local Ollama or LM Studio
- **+** GUI management of MCP servers (STDIO, Streamable HTTP, SSE) and SubAgents
- **+** Remote control through a phone H5 page and IM apps such as Telegram, Slack and Feishu
- **−** Community Source License, not OSI open source; commercial use and paid services need written permission
- **−** README is mostly in Chinese, with the English version in a separate file
- **−** Sponsor and API reseller promotions take up much of the README
- **−** RAM and GPU requirements are not stated

<sub>Needs Bun, Electron · Models: Claude, ChatGPT, Grok, DeepSeek, Kimi · safety checks passed 9 of 11 · [Repo](https://github.com/nanmicoder/cc-haha) · [📖 Docs ↗](https://cchaha.ai) · [🌐 Site ↗](https://cchaha.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-haha/)</sub>

<a name="superpowers"></a>
### #&#8288;42 [superpowers](https://github.com/obra/superpowers) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 307k · MIT · Oct 2026</sub>

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

<a name="diagram-design"></a>
### #&#8288;43 [diagram-design](https://github.com/cathrynlavery/diagram-design) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 62k · MIT · Oct 2026</sub>

**Agent skill that draws brand-styled diagrams as single HTML and SVG files.**

An Agent Skill that has your coding agent write a diagram as one self-contained HTML file with inline SVG, with no build step or JavaScript. It covers 45 diagram types, each in minimal light, minimal dark and full-editorial variants. It can pull palette and fonts from a site, import Mermaid, draw.io and Excalidraw files, and export to SVG or PNG.

- **+** Output is one HTML file with inline SVG; opens by double-click, no JavaScript or build step
- **+** 45 diagram types, each with light, dark and editorial variants
- **+** Onboarding step pulls palette and fonts from a URL so diagrams match your brand
- **+** Installs via npx skills on Cursor, Claude Code, Codex, Copilot, Gemini CLI and others
- **−** Output quality depends on the model; the same prompt can lay out differently twice
- **−** Not an editable source format: no text to diff and no canvas to drag boxes on
- **−** Slash commands like /export-diagram and /doctor only come with native plugin packages, not npx install
- **−** README says Mermaid is a better fit for docs that change every sprint in Git

<sub>no GPU · Needs An Agent Skills-compatible coding agent (Claude Code, Cursor, Codex, etc.), Node.js (npx) for the skills CLI install · Models: Model-agnostic: uses whichever model the host agent runs · safety checks passed 11 of 11 · [Repo](https://github.com/cathrynlavery/diagram-design) · [▶️ Demo ↗](https://cathrynlavery.github.io/diagram-design/) · [🌐 Site ↗](https://diagramdesign.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diagram-design/)</sub>

<a name="oh-my-opencode-slim"></a>
### #&#8288;44 [oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.8k · MIT · Oct 2026</sub>

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

<a name="worktrunk"></a>
### #&#8288;45 [worktrunk](https://github.com/max-sixty/worktrunk) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · custom license · Oct 2026</sub>

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

<a name="mattpocock-skills-zh-cn"></a>
### #&#8288;46 [mattpocock-skills-zh-cn](https://github.com/vinvcn/mattpocock-skills-zh-cn) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="oh-my-hermes"></a>
### #&#8288;47 [oh-my-hermes](https://github.com/rlaope/oh-my-hermes) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Oct 2026</sub>

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

<a name="agents"></a>
### #&#8288;48 [agents](https://github.com/wshobson/agents) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Oct 2026</sub>

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

<a name="browser-harness"></a>
### #&#8288;49 [browser-harness](https://github.com/browser-use/browser-harness) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Oct 2026</sub>

**Lets coding agents drive your logged-in Chrome over CDP.**

Browser Harness connects Claude Code, Codex or Cursor to your running Chrome through the DevTools Protocol, so the agent can open pages, click, type, read and download while logged in as you. A SKILL.md teaches the workflow, and the agent writes missing helpers into a local workspace while the core package stays protected. It also ships a stdio MCP server, browser-harness-mcp.

- **+** Drives your real, logged-in Chrome rather than a clean profile
- **+** Ships both a skill (SKILL.md) and a stdio MCP server
- **+** Lowest median input tokens and model cost in its own 100-task eval
- **+** Agent-written helpers persist in a local workspace for reuse
- **−** Gives the agent access to the whole browser, including all logins
- **−** Needs Chrome 144+ with remote debugging enabled and an Allow click
- **−** Eval score not distinguishable from Playwright MCP or Chrome DevTools MCP
- **−** Benchmark run with Codex only; other agents not measured

<sub>no GPU · Needs Chrome 144+, uv, Python 3.12 · Models: Claude Code, Codex, Cursor, any MCP client · safety checks passed 14 of 17 · [Repo](https://github.com/browser-use/browser-harness) · [📖 Docs ↗](https://github.com/browser-use/browser-harness/blob/main/install.md) · [🌐 Site ↗](https://browser-use.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/browser-harness/)</sub>

<a name="jeffallan-claude-skills"></a>
### #&#8288;50 [claude-skills](https://github.com/jeffallan/claude-skills) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Claude Code plugin with 67 skills and 9 Jira-linked workflow commands.**

A Claude Code plugin that installs 67 skills across 12 categories, covering languages, backend and frontend frameworks, infrastructure, testing, DevOps and security. Skills activate from the request text and load reference files (371 in total). It also adds 9 workflow commands for epics, which need an Atlassian MCP server, and a /common-ground command that surfaces Claude's assumptions about the project.

- **+** Installs with two /plugin commands from the Claude Code marketplace
- **+** 67 skills with 371 reference files loaded on demand per request
- **+** Skills chain into flows, e.g. Debugging Wizard to Test Master to Code Reviewer
- **+** MIT licensed, with a docs site, changelog and contribution guide
- **−** Built for Claude Code only; other agents are not mentioned in the README
- **−** Workflow commands require a separately configured Atlassian MCP server
- **−** README gives no measure of skill activation accuracy or output quality
- **−** Full skill list lives in a separate guide, not the README

<sub>no GPU · Needs Claude Code, Atlassian MCP server (workflow commands only) · Models: Claude · safety checks passed 8 of 10 · [Repo](https://github.com/jeffallan/claude-skills) · [📖 Docs ↗](https://jeffallan.github.io/claude-skills) · [🌐 Site ↗](https://jeffallan.github.io/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/jeffallan-claude-skills/)</sub>

<a name="loopx"></a>
### #&#8288;51 [loopx](https://github.com/loopx-project/loopx) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="claude-octopus"></a>
### #&#8288;52 [claude-octopus](https://github.com/nyldn/claude-octopus) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Oct 2026</sub>

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

<a name="codex-router"></a>
### #&#8288;53 [codex-router](https://github.com/duolahypercho/codex-router) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Oct 2026</sub>

**Local router that adds Kimi, DeepSeek, Claude and other models to Codex.**

Codex Router runs a per-user background service that adds external providers (Anthropic, Kimi, DeepSeek, xAI, Z.ai, Qwen plan, Ollama Cloud, OpenRouter and others) to the Codex App and CLI model picker. Credentials are entered in hidden local prompts or reused from official CLI OAuth sessions. It also ships an Electron Control Center, a tray app and a macOS desktop panel, and can serve Gemini CLI, Claude Code, Cursor and OpenClaw.

- **+** Long model table across many providers, with separate global and China endpoints for Kimi and StepFun
- **+** Catalog is credential-aware: only models with a stored key or valid OAuth session appear
- **+** Credentials stay local; prompts are hidden and other CLIs' OAuth tokens are not copied
- **+** Installers for macOS, Linux and Windows, a Homebrew tap, and a credential-free idle install
- **−** Independent project, not affiliated with OpenAI or the model vendors
- **−** No prebuilt macOS .dmg; it builds locally and needs the full Xcode app
- **−** Subscription agent bridges are experimental and reject permission requests by default
- **−** Homebrew install is CLI-only, has no Control Center, and builds Python deps from source

<sub>no GPU · Needs Codex App or CLI, Node.js 22.19+, uv or Python 3.10+, Git, Xcode (macOS Control Center build) · Models: Anthropic, Kimi, DeepSeek, xAI Grok, Z.ai GLM · [Repo](https://github.com/duolahypercho/codex-router) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-router/)</sub>

<a name="lifeos"></a>
### #&#8288;54 [lifeos](https://github.com/danielmiessler/lifeos) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · MIT · Oct 2026</sub>

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

<a name="visual-explainer"></a>
### #&#8288;55 [visual-explainer](https://github.com/nicobailon/visual-explainer) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Web browser, Node.js (optional MCP and PPTX utilities), ffmpeg, Chrome, playwright-core (optional video export) · safety checks passed 9 of 10 · [Repo](https://github.com/nicobailon/visual-explainer) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/visual-explainer/)</sub>

<a name="tech-leads-club-agent-skills"></a>
### #&#8288;56 [agent-skills](https://github.com/tech-leads-club/agent-skills) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.1k · custom license · Oct 2026</sub>

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

<a name="aidlc-workflows"></a>
### #&#8288;57 [aidlc-workflows](https://github.com/awslabs/aidlc-workflows) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.5k · MIT-0 · Oct 2026</sub>

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

<a name="i-have-adhd"></a>
### #&#8288;58 [i-have-adhd](https://github.com/ayghri/i-have-adhd) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 59k · MIT · Oct 2026</sub>

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

<a name="claude-code-router"></a>
### #&#8288;59 [claude-code-router](https://github.com/musistudio/claude-code-router) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (80) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · MIT · Oct 2026</sub>

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

<a name="claude-code-templates"></a>
### #&#8288;60 [claude-code-templates](https://github.com/davila7/claude-code-templates) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

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
### #&#8288;61 [claude-video](https://github.com/bradautomates/claude-video) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Sep 2026</sub>

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

<a name="gsd-core"></a>
### #&#8288;62 [gsd-core](https://github.com/open-gsd/gsd-core) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js, npm · Models: Claude Code, Codex, OpenCode, Antigravity CLI, Kimi CLI · safety checks passed 11 of 12 · [Repo](https://github.com/open-gsd/gsd-core) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gsd-core/)</sub>

<a name="superpowers-zh"></a>
### #&#8288;63 [superpowers-zh](https://github.com/jnmetacode/superpowers-zh) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Oct 2026</sub>

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

<a name="gentle-ai"></a>
### #&#8288;64 [gentle-ai](https://github.com/gentleman-programming/gentle-ai) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.1k · MIT · Oct 2026</sub>

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
### #&#8288;65 [obsidian-mind](https://github.com/breferrari/obsidian-mind) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="claude-code-game-studios"></a>
### #&#8288;66 [claude-code-game-studios](https://github.com/donchitos/claude-code-game-studios) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

**Claude Code template with 49 game-dev subagents, 74 skills and validation hooks.**

A project template that configures Claude Code with 49 subagents arranged as directors, department leads and specialists, plus 74 slash-command skills, 15 hooks, 14 path-scoped rules and 62 document templates. It guides a game project from brainstorm through design docs, stories, QA and release, with Godot, Unity and Unreal specialist agents. A `modes.rigor` setting in project.yaml (minimal, standard, full) controls how much process is enforced.

- **+** Engine-specific agent sets for Godot 4, Unity and Unreal Engine 5
- **+** Hooks validate commits, pushes, assets and design-doc reads in Bash
- **+** modes.rigor presets default to minimal; README reports the standard tier did not improve the game
- **+** Stories touching visuals require a launched game and a retained screenshot
- **−** Requires Claude Code; no other coding agent is supported
- **−** Needs Python 3 and Bash; Windows users need Git for Windows
- **−** README admits standard rigor wrote 30 docs before code and ranked last
- **−** No sample game shipped, so output quality is not demonstrated in the repo

<sub>no GPU · Needs Claude Code, Git, Python 3, Bash, jq (recommended) · Models: Claude (Opus, Sonnet, or session model) · safety checks passed 9 of 9 · [Repo](https://github.com/donchitos/claude-code-game-studios) · [📖 Docs ↗](https://code.claude.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-game-studios/)</sub>

<a name="drawio-skill"></a>
### #&#8288;67 [drawio-skill](https://github.com/agents365-ai/drawio-skill) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs draw.io desktop CLI, Graphviz (optional), xvfb (Linux headless), Python 3 · Models: Claude Code, Cursor, Copilot, Codex, OpenClaw · safety checks passed 9 of 11 · [Repo](https://github.com/agents365-ai/drawio-skill) · [📖 Docs ↗](https://agents365-ai.github.io/drawio-skill/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/drawio-skill/)</sub>

<a name="android-skills"></a>
### #&#8288;68 [skills](https://github.com/android/skills) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="mirrord"></a>
### #&#8288;69 [mirrord](https://github.com/metalbear-co/mirrord) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · MIT · Oct 2026</sub>

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

<a name="ultracite"></a>
### #&#8288;70 [ultracite](https://github.com/haydenbleasel/ultracite) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: known (43) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

**Lint and format CLI that configures Biome, ESLint or Oxlint plus AI agent rules.**

Ultracite is a CLI that sets up a JavaScript/TypeScript linter and formatter (Biome, ESLint with Prettier and Stylelint, or Oxlint with Oxfmt) with preconfigured rules. `ultracite init` also writes rule and context files for AI agents such as Claude Code, Copilot, Cursor and Gemini, and `fix` can hand unfixable issues to the Claude Code or Codex CLI.

- **+** One `npx ultracite init` configures linter, formatter, editor settings and agent rule files
- **+** Supports three toolchains: Biome, ESLint/Prettier/Stylelint, and Oxlint/Oxfmt
- **+** Non-interactive init flags for CI, plus per-workspace framework settings for monorepos
- **+** `doctor` command diagnoses setup problems, including linter version mismatches
- **−** Targets JavaScript and TypeScript only
- **−** Pins linter versions it supports; `upgrade` reinstalls the toolchain at those versions
- **−** Agent-assisted fixing requires the separate Claude Code or Codex CLI
- **−** README gives no rule counts or benchmark figures behind the speed claims

<sub>no GPU · Needs Node.js, Biome, ESLint or Oxlint, Claude Code or Codex CLI (optional) · Models: Claude Code, Codex, GitHub Copilot, Cursor, Gemini · [Repo](https://github.com/haydenbleasel/ultracite) · [📖 Docs ↗](https://ultracite.ai/) · [🌐 Site ↗](https://www.ultracite.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ultracite/)</sub>

<a name="claude-howto"></a>
### #&#8288;71 [claude-howto](https://github.com/luongnv89/claude-howto) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 46k · MIT · Oct 2026</sub>

**Tutorial modules and copy-paste templates for Claude Code features.**

A tutorial repository with 10 modules covering Claude Code slash commands, memory, skills, subagents, MCP, hooks, plugins, checkpoints, advanced features and the CLI. Each module has Mermaid diagrams and files you copy into .claude/ or ~/.claude/. It also includes a self-assessment quiz, a learning roadmap estimated at 11-13 hours, and an EPUB build script.

- **+** Covers slash commands, memory, skills, subagents, MCP, hooks and plugins in one ordered path
- **+** Templates are plain Markdown, shell and JSON files copied into .claude/ directories
- **+** Includes /self-assessment and /lesson-quiz commands to find knowledge gaps
- **+** MIT licensed; README states it is synced with Claude Code releases (v2.1.302)
- **−** Documentation and templates only; not a runnable tool or library
- **−** Specific to Claude Code; templates do not target other coding agents
- **−** Ships no plugin marketplace, so plugins load only via --plugin-dir from a clone
- **−** Needs updating as Claude Code changes hook events, flags and install methods

<sub>no GPU · Needs Claude Code 2.1+, uv (only for the EPUB build script) · Models: Claude Opus, Claude Sonnet, Claude Haiku · safety checks passed 11 of 11 · [Repo](https://github.com/luongnv89/claude-howto) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-howto/)</sub>

<a name="img2threejs"></a>
### #&#8288;72 [img2threejs](https://github.com/img2threejs/img2threejs) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: fair (68) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 20k · Apache-2.0 · Oct 2026</sub>

**Agent skill that rebuilds an image's object as a procedural Three.js model.**

A skill for Claude Code, Codex, OpenCode or Hermes that takes one reference image and produces a TypeScript THREE.Group factory built from primitives, procedural shaders and generated geometry, with pivots, sockets and colliders for animation. Python stdlib scripts run staged build passes (blockout through optimization) with validation and review gates, while the agent does the visual judgment and code. Optional plugins add CS2 weapon skins, character rigging and GLB output.

- **+** Output is code-only Three.js with pivots, sockets and colliders, not mesh files
- **+** Quality gates block generation until a detail inventory is complete
- **+** Installs into Claude Code, Codex, OpenCode or Hermes via one npx command
- **+** Public live gallery shows generated source for each model
- **−** Needs an external coding agent; installing the skill alone produces nothing
- **−** A single image cannot guarantee likeness; unseen regions are inferred
- **−** The environment plugin is private and needs authorized GitHub access
- **−** Hermes setup needs a manual symlink step

<sub>Needs Node.js >= 18, Python >= 3.10, Git, Claude Code, Codex, OpenCode or Hermes, Three.js · Models: Host agent's vision model · safety checks passed 9 of 9 · [Repo](https://github.com/img2threejs/img2threejs) · [▶️ Demo ↗](https://img2threejs.io/) · [📖 Docs ↗](https://github.com/img2threejs/img2threejs/blob/main/docs/ARCHITECTURE.md) · [🌐 Site ↗](https://img2threejs.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/img2threejs/)</sub>

<a name="brag"></a>
### #&#8288;73 [brag](https://github.com/latent-spaces/brag) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: fair (77) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Oct 2026</sub>

**Agent skill that renders a short launch video for your project.**

/brag is an agent skill for Claude Code, Codex, opencode and other Agent Skills hosts. It reads your project, plans the story and tone, then hands a brief to Hyperframes to render brag.mp4 with music, motion and share copy. A lighter /brag-slim variant skips Hyperframes and is used automatically on Opus 5.5.

- **+** Installs through Claude Code and Codex plugin marketplaces or the skills CLI
- **+** Outputs plan, composition brief, share copy and rendered brag.mp4 in brag-output/
- **+** Tone is steerable with --tone; voiceover is optional via --voice using Kokoro
- **+** Bundled music and SFX; /brag-slim needs no Hyperframes or bundled assets
- **−** Full workflow requires Node.js 22+, FFmpeg and the Hyperframes CLI
- **−** Voiceover is off by default and depends on Hyperframes with Kokoro
- **−** Bundled music is CC BY 4.0 and needs attribution
- **−** Windows needs symlink support or a manual copy of the skill directory

<sub>Needs Node.js 22+, FFmpeg, Hyperframes CLI, An Agent Skills-compatible agent · Models: Claude Code, Codex CLI, opencode, Cursor, Gemini CLI · safety checks passed 9 of 10 · [Repo](https://github.com/latent-spaces/brag) · [▶️ Demo ↗](https://latent-spaces.github.io/brag/) · [🌐 Site ↗](https://letsbrag.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/brag/)</sub>

<a name="auto-claude-code-research-in-sleep"></a>
### #&#8288;74 [auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

**Skill-based research workflow where one model executes and another reviews.**

ARIS is a set of 82 skills that run an ML research workflow (idea discovery, experiments, paper writing) inside Claude Code, Codex CLI, Cursor and similar agents. An executor model drives the work while an independent reviewer model, Codex via an MCP bridge by default, critiques each step. It also ships a standalone Rust CLI (ARIS-Code) and plugins for Claude Code and Codex CLI.

- **+** Works across Claude Code, Codex CLI, Cursor, Trae, Copilot CLI and others
- **+** Separate reviewer model checks the executor's output; alternative model pairs documented
- **+** Also ships as standalone CLI and as Claude Code and Codex plugins
- **+** MIT license with frequent releases; latest ARIS-Code is v0.4.28
- **−** Default reviewer depends on codex-cli, which dropped `codex mcp-server` in 0.154
- **−** Focused on ML research and paper writing, not general coding
- **−** README is long and dense, with a heavy changelog and many sibling projects
- **−** Hardware needs and running costs are unknown; default setup uses paid model APIs

<sub>Needs Claude Code or Codex CLI, codex-cli, Codex MCP bridge · Models: Claude Opus 5, Claude Fable 5.1, GPT-6-Astra, ModelScope-hosted models · safety checks passed 10 of 11 · [Repo](https://github.com/wanshuiyin/auto-claude-code-research-in-sleep) · [📖 Docs ↗](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep/blob/main/AGENT_GUIDE.md) · [🌐 Site ↗](https://wanshuiyin.github.io/Auto-claude-code-research-in-sleep/ARIS_INTRO.html) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/auto-claude-code-research-in-sleep/)</sub>

<a name="universal-modder"></a>
### #&#8288;75 [universal-modder](https://github.com/rehan-remade/universal-modder) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.1k · MIT · Oct 2026</sub>

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

<a name="anti-slop"></a>
### #&#8288;76 [anti-slop](https://github.com/miqdadbadjuber/anti-slop) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.3k · MIT · Oct 2026</sub>

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
### #&#8288;77 [lean-ctx](https://github.com/yvgude/lean-ctx) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="skillshare"></a>
### #&#8288;78 [skillshare](https://github.com/runkids/skillshare) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

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

<a name="huashu-design"></a>
### #&#8288;79 [huashu-design](https://github.com/alchaincyf/huashu-design) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

**Agent skill that turns prompts into HTML prototypes, decks, animations and infographics.**

Installed with `npx skills add`, this skill lets agents such as Claude Code, Cursor or Codex produce single-file HTML interactive prototypes, HTML decks exportable to editable PPTX, MP4/GIF animations and infographics. It includes a library of 84 HTML/CSS style specimens, a brand-asset protocol, and local scripts for linting, export and reference screenshots. The core pipeline runs locally; cloud features (TTS, AI video review) are optional.

- **+** Exports HTML decks to PPTX with real editable text boxes via html2pptx.js
- **+** Ships 84 style specimens with source, so styles are viewed before being chosen
- **+** Core design and export pipeline runs locally with no network or API key
- **+** Works across skills-compatible agents; MIT license permits commercial use
- **−** No layer-level editable export to Figma; output is HTML, not Keynote-editable
- **−** Complex 3D, physics or particle animation is outside its scope
- **−** Older skills CLI (≤1.5.15) copies only SKILL.md, breaking the install
- **−** README is Chinese-first; the English version is a separate file

<sub>no GPU · Needs Node.js, Playwright, ffmpeg, Python · safety checks passed 8 of 9 · [Repo](https://github.com/alchaincyf/huashu-design) · [▶️ Demo ↗](https://www.huasheng.ai/parrots/) · [🌐 Site ↗](https://www.huasheng.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huashu-design/)</sub>

<a name="codex-with-chatgpt"></a>
### #&#8288;80 [codex-with-chatgpt](https://github.com/xiaoduoya/codex-with-chatgpt) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · MIT · Oct 2026</sub>

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

<a name="agentation"></a>
### #&#8288;81 [agentation](https://github.com/benjitaylor/agentation) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · custom license · Sep 2026</sub>

**React toolbar for annotating page elements to give coding agents feedback.**

Agentation is a React component that adds a toolbar to your app. You click elements, select text or drag areas, add notes, and copy markdown with selectors, positions and context so a coding agent can grep for the code. An optional MCP server (npx -y agentation-mcp server) syncs annotations to the agent over HTTP.

- **+** Outputs selectors and positions an agent can grep, instead of prose descriptions
- **+** Works with any agent via copy-paste; MCP endpoint is optional
- **+** No runtime dependencies beyond React peer dependencies
- **+** Selects inside open shadow roots and same-origin iframes
- **−** Requires React 18+; no other frameworks listed
- **−** Desktop browsers only; mobile not supported
- **−** PolyForm Shield 1.0.0 license is source-available, not OSI open source
- **−** Direct sync needs a separate local MCP server process

<sub>no GPU · Needs React 18+, agentation-mcp (optional) · port 4747 · [Repo](https://github.com/benjitaylor/agentation) · [📖 Docs ↗](https://agentation.com) · [🌐 Site ↗](https://agentation.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentation/)</sub>

<a name="agent-beacon"></a>
### #&#8288;82 [agent-beacon](https://github.com/asymptote-labs/agent-beacon) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (36) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

**Captures coding agent sessions and turns them into reusable memory.**

Beacon records session history from Claude Code, Cursor, Codex, OpenCode and 20+ other agent harnesses, normalizes it into an OpenTelemetry-based event model, and writes it to local JSONL. Reviewed knowledge is exposed to later agents through MCP or Agent Skills. It includes a terminal trace browser, a local read-only dashboard, and forwarding to SIEM and storage destinations.

- **+** Covers 20+ harnesses with one normalized trace format, including Claude Code, Cursor, Codex and Cline
- **+** Local-first: JSONL at ~/.beacon/endpoint/logs/runtime.jsonl, plus terminal and local web viewers
- **+** Forwards to Splunk, Datadog, Elastic, Sentinel, S3, GCS, CloudWatch and others
- **+** Installs via Homebrew, .deb/.rpm with checksums, or a Windows MSI
- **−** Interactive setup preselects Beacon Cloud; local-only requires choosing the Local opt-out
- **−** Capture coverage varies by harness; some lack token, MCP or approval events
- **−** Custom lenses run HTML in a sandbox that the README says cannot block every data exfiltration path
- **−** Memory extraction and review workflow details are mostly in external docs, not the README

<sub>no GPU · Needs Homebrew, apt or dnf, or Windows MSI for install, Optional: Beacon Cloud account, Optional: Splunk, Datadog, Elastic, S3 or GCS for forwarding · [Repo](https://github.com/asymptote-labs/agent-beacon) · [📖 Docs ↗](https://docs.beacon.sh) · [🌐 Site ↗](https://beacon.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-beacon/)</sub>

<a name="tweakcc"></a>
### #&#8288;83 [tweakcc](https://github.com/piebald-ai/tweakcc) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

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

<a name="agency-agents"></a>
### #&#8288;84 [agency-agents](https://github.com/msitarzewski/agency-agents) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 165k · MIT · Oct 2026</sub>

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
### #&#8288;85 [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 68k · MIT · Oct 2026</sub>

**Reference repo of Claude Code agents, commands, skills, hooks and settings.**

A documentation repository that explains Claude Code features (subagents, commands, skills, hooks, MCP, settings, memory) with usage notes and working examples under .claude/. It includes a weather-orchestrator demo of a Command to Agent to Skill workflow and a table comparing community development workflows such as Superpowers, Spec Kit and gstack.

- **+** Each concept links to a guidance note and a matching implementation file
- **+** Runnable weather-orchestrator example shows the Command, Agent, Skill pattern
- **+** Compares community workflows with agent, command and skill counts
- **+** MIT licensed and mostly Markdown, so files are easy to copy into a project
- **−** Documentation and examples only; no installable tool or package
- **−** Tied to Claude Code, and beta features may change quickly
- **−** Many links point to X posts and external repos rather than local docs
- **−** Sponsor banners and trending badges sit at the top of the README

<sub>no GPU · Needs Claude Code · Models: Claude · safety checks passed 8 of 9 · [Repo](https://github.com/shanraisshan/claude-code-best-practice) · [📖 Docs ↗](https://code.claude.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-best-practice/)</sub>

<a name="awesome-claude-code-subagents"></a>
### #&#8288;86 [awesome-claude-code-subagents](https://github.com/voltagent/awesome-claude-code-subagents) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<a name="anatomy"></a>
### #&#8288;87 [anatomy](https://github.com/wheresryan22/anatomy) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (74) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Oct 2026</sub>

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

<a name="pxpipe"></a>
### #&#8288;88 [pxpipe](https://github.com/teamchong/pxpipe) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.6k · MIT · Oct 2026</sub>

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
### #&#8288;89 [peon-ping](https://github.com/peonping/peon-ping) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.1k · MIT · Oct 2026</sub>

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

<a name="oracle"></a>
### #&#8288;90 [oracle](https://github.com/steipete/oracle) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Oct 2026</sub>

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

<a name="dsh-context"></a>
### #&#8288;91 [dsh-context](https://github.com/bowenliang123/dsh-context) <sub>score [77](../README.md#-how-we-rank "Score 77/100. Adoption: known (47) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · Apache-2.0 · Oct 2026</sub>

**DeepSeek Harness plugin for inspecting agent context, token use and subagents.**

dsh-context is a plugin for DeepSeek Harness that adds a Context Insights page, Context and Fleet tabs, a right-sidebar panel and a /context command. It shows context composition, per-request trends, compaction events, file activity, token cost and subagent networks. It installs through the Add plugin wizard or the dsh CLI.

- **+** Context browser shows each request's actual system prompt, tool schemas, messages and tool outputs
- **+** Trend chart pins compactions and prunes, with provider-reported actuals beside estimates
- **+** Fleet tab shows each subagent's context size, occupancy and cost live
- **+** Installs with one dsh command or the Add plugin wizard, no build step or restart
- **−** Works only inside DeepSeek Harness, from @deepseek-ai/dsh 0.2.0-rc.2 onward
- **−** Per-category token figures are heuristic estimates, not exact counts
- **−** Cost is estimated from models.dev list prices, not actual billing
- **−** UI is available only in English and Simplified Chinese

<sub>no GPU · Needs @deepseek-ai/dsh (DeepSeek Harness) · Models: DeepSeek, models.dev-listed models (cost estimates) · [Repo](https://github.com/bowenliang123/dsh-context) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-context/)</sub>

<a name="jakubkrehel-skills"></a>
### #&#8288;92 [skills](https://github.com/jakubkrehel/skills) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.8k · MIT · Oct 2026</sub>

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

<a name="codex-keysmith"></a>
### #&#8288;93 [codex-keysmith](https://github.com/jia-ethan/codex-keysmith) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.8k · MIT · Sep 2026</sub>

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

<a name="dsh-better-sidebar"></a>
### #&#8288;94 [dsh-better-sidebar](https://github.com/omdsh-dev/dsh-better-sidebar) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

**Sidebar and bottom-panel workbench plugin for the DSH coding agent.**

A plugin for the DSH agent host that adds a right sidebar (file tree, Git, tasks, side chat) and a self-drawn bottom panel with split panes and terminal tabs. It exposes a ctx.betterSidebar service with registerTab and registerFileViewer so other plugins can add pages and file viewers. Installed with `dsh plugin add`; requires DSH 0.2.1-rc.1 or newer for the current release.

- **+** Editable CodeMirror file editor with Markdown, Mermaid and sandboxed HTML previews
- **+** Read-only Git commit graph plus Source Control groups and a session AI-changes view
- **+** Public registerTab and registerFileViewer API; built-in tabs use the same API
- **+** Lists 30+ third-party tab and viewer plugins on a GitHub topic
- **−** Works only inside DSH; no standalone use
- **−** Current v0.28.0 is incompatible with DSH 0.2.0-rc.2, which needs v0.26.1 pinned
- **−** README states RC validation of v0.28.0 is still pending
- **−** Side Chat is beta; Git graph shows no tags and has no history-changing actions

<sub>no GPU · Needs DSH 0.2.1-rc.1+, Node.js package manager (npm/pnpm) · [Repo](https://github.com/omdsh-dev/dsh-better-sidebar) · [📖 Docs ↗](https://github.com/omdsh-dev/DSH-better-sidebar/blob/main/docs/external-plugin-guide.md) · [🌐 Site ↗](https://www.npmjs.com/package/dsh-better-sidebar) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dsh-better-sidebar/)</sub>

<a name="answer-me-with-html"></a>
### #&#8288;95 [answer-me-with-html](https://github.com/qingyuna/answer-me-with-html) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Oct 2026</sub>

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

<a name="ffmpeg-skill"></a>
### #&#8288;96 [ffmpeg-skill](https://github.com/kajisho5/ffmpeg-skill) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

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

<a name="understand-anything"></a>
### #&#8288;97 [understand-anything](https://github.com/egonex-ai/understand-anything) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 89k · MIT · Oct 2026</sub>

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

<a name="agency-agents-zh"></a>
### #&#8288;98 [agency-agents-zh](https://github.com/jnmetacode/agency-agents-zh) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Oct 2026</sub>

**328 role-based agent persona files for Claude Code, Cursor and other tools.**

Chinese-language community fork of msitarzewski/agency-agents: 328 markdown agent personas across 22 departments, 67 of them original China-market roles (Xiaohongshu, Douyin, WeChat, Feishu, DingTalk and others). Shell scripts (install.sh, convert.sh) copy or convert the files for 20 coding tools, including Claude Code, Copilot, Cursor, Aider and OpenClaw. Each persona defines identity, rules, workflow and deliverables.

- **+** 328 persona files in 22 departments, each with defined workflow and deliverables
- **+** install.sh targets 20 tools; Claude Code and Copilot files can be copied directly
- **+** 67 original China-market roles, such as Xiaohongshu, Feishu, DingTalk and WeChat mini programs
- **+** MIT license; plain markdown files that are easy to read and adapt
- **−** Most tools other than Claude Code and Copilot need a convert.sh step first
- **−** Persona content is mostly Chinese; the English version is the upstream repo
- **−** README carries many sponsor ads and links to the author's other products
- **−** Persona prompts only; multi-agent orchestration needs the separate agency-orchestrator project

<sub>no GPU · Needs Claude Code, Cursor, Copilot or another supported AI coding tool · Models: Claude Code, GitHub Copilot, Cursor, Aider, Windsurf · safety checks passed 8 of 9 · [Repo](https://github.com/jnmetacode/agency-agents-zh) · [▶️ Demo ↗](https://ao.aiolaola.com/experts) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents-zh/)</sub>

<a name="trellis"></a>
### #&#8288;99 [trellis](https://github.com/mindfold-ai/trellis) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: patchy (45) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · AGPL-3.0 · Sep 2026</sub>

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

<sub>no GPU · Needs Node.js >= 18, Python >= 3.9 · safety checks passed 9 of 11 · [Repo](https://github.com/mindfold-ai/trellis) · [📖 Docs ↗](https://docs.trytrellis.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/trellis/)</sub>

<a name="video-shotcraft"></a>
### #&#8288;100 [video-shotcraft](https://github.com/vincentwei1021/video-shotcraft) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · Apache-2.0 · Oct 2026</sub>

**Claude Code and Codex skill that builds Remotion promo videos from screenshots.**

An agent skill that captures your real product pages, picks shots from a library of 124 recipe cards (150 shots), storyboards the film and renders it with Remotion to a 1920x1080, 30 fps MP4. Frames are drawn by code from your screenshots and copy, not generated by a video model. It also ships a browser editor (Motion Workbench) and optional JianYing draft export.

- **+** Output is a Remotion React project, so every shot stays editable in code
- **+** Library of 124 recipe cards and 150 shots, with a searchable online Gallery
- **+** Includes 149 SFX, 5 BGM tracks, beat sync and frame-level QA steps
- **+** Motion Workbench for post-delivery editing; optional JianYing draft export
- **−** Tested on macOS; headless Linux needs workarounds such as --concurrency=1
- **−** Remotion has its own license; companies may need a paid one
- **−** Bundled audio is under per-file licenses, not Apache-2.0
- **−** Workbench guide is in Chinese only

<sub>no GPU · Needs Node.js, npm, ffmpeg, ffprobe, uv, puppeteer, Remotion · Models: Claude Code, Codex · safety checks passed 10 of 11 · [Repo](https://github.com/vincentwei1021/video-shotcraft) · [▶️ Demo ↗](https://vincentwei1021.github.io/video-shotcraft/) · [📖 Docs ↗](https://github.com/Vincentwei1021/video-shotcraft/blob/main/references/pipeline.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/video-shotcraft/)</sub>

<a name="softwarecopyright-skill"></a>
### #&#8288;101 [softwarecopyright-skill](https://github.com/fokkyp/softwarecopyright-skill) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · AGPL-3.0 · Oct 2026</sub>

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
### #&#8288;102 [ccg-workflow](https://github.com/fengshao1227/ccg-workflow) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

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
### #&#8288;103 [observal](https://github.com/observal/observal) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="ux-ui-agent-skills"></a>
### #&#8288;104 [ux-ui-agent-skills](https://github.com/plugin87/ux-ui-agent-skills) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

**Design-system rules and 52 browser-checked gates for coding agents.**

A kit of instructions, DTCG design tokens, 138 design-system references and 26 skills that steer Claude Code and other agents toward accessible, token-driven UI. It installs as a Claude Code plugin, an MCP server, or via npm or Homebrew. It runs 52 gates (WCAG contrast, axe, target size, keyboard, overflow), 34 of which need a real browser through Playwright.

- **+** Gates are runnable checks (per-state contrast, axe, target size), not just prompt guidance
- **+** Several install paths: Claude Code plugin, MCP server, npx, Homebrew, AGENTS.md for Codex and Cursor
- **+** Live demo with 49 rendered pages built from the kit's own tokens
- **+** MCP server has no SDK dependency and returns gate output with exit codes unedited
- **−** 34 of 52 gates need Playwright and a browser, which plugin install does not pull in
- **−** Plugin root CLAUDE.md is not loaded, so rules rely on the design-doctrine skill
- **−** Evidence of quality is small: two blind runs, and the README lists unproven areas
- **−** Built mainly around Claude Code; other agents get read-only AGENTS.md guidance

<sub>no GPU · Needs Node.js, Playwright (for browser gates) · Models: Claude Code, Codex, Cursor, Copilot, Aider · [Repo](https://github.com/plugin87/ux-ui-agent-skills) · [▶️ Demo ↗](https://plugin87.github.io/ux-ui-agent-skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ux-ui-agent-skills/)</sub>

<a name="agentskills"></a>
### #&#8288;105 [agentskills](https://github.com/agentskills/agentskills) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: widely used (85) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Aug 2026</sub>

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

<a name="skills-manager"></a>
### #&#8288;106 [skills-manager](https://github.com/xingkongliang/skills-manager) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · MIT · Oct 2026</sub>

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

<a name="n8n-skills"></a>
### #&#8288;107 [n8n-skills](https://github.com/czlonkowski/n8n-skills) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (71) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.5k · MIT · Oct 2026</sub>

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

<a name="dashi-taskboard"></a>
### #&#8288;108 [dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · Apache-2.0 · Oct 2026</sub>

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

<a name="claude-code-harness"></a>
### #&#8288;109 [claude-code-harness](https://github.com/chachamaru127/claude-code-harness) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

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

<a name="git-ai"></a>
### #&#8288;110 [git-ai](https://github.com/git-ai-project/git-ai) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (37) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="native-subtitle-quote-image"></a>
### #&#8288;111 [native-subtitle-quote-image](https://github.com/chengyi-ai/native-subtitle-quote-image) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

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

<a name="cc-safety-net"></a>
### #&#8288;112 [cc-safety-net](https://github.com/kenryu42/cc-safety-net) <sub>score [74](../README.md#-how-we-rank "Score 74/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Pre-execution hook that blocks destructive commands and secret access by coding agents.**

CC Safety Net installs as a hook in coding agent CLIs and parses each shell command or file access before it runs. It blocks things like `git reset --hard`, `git push --force`, `rm -rf` on dangerous targets, `curl | bash`, and reads of SSH keys, `.env` files and `~/.aws`, including when wrapped in `bash -c` or `python -c`. It is not a sandbox and does not restrict processes, filesystem permissions or network egress.

- **+** Supports 16 coding CLIs, including Claude Code, Codex, Cursor and Gemini CLI, on Windows, macOS, Linux
- **+** Parses command semantics, so wrapping in bash -c or reordering flags does not bypass rules
- **+** Standard, Strict and Paranoid presets, a GUI editor, and rulebooks for Terraform, AWS, gcloud, Azure
- **+** Policy lives in a committed .cc-safety-net/ directory; a broken config never blocks commands
- **−** Not a sandbox: no process containment, filesystem permissions or network egress monitoring
- **−** Requires Node.js 18 or higher
- **−** Must keep the @latest qualifier on npx, or a stale cached copy may run
- **−** Protection depends on each CLI's hook support; per-CLI requirements vary

<sub>no GPU · Needs Node.js 18+ · [Repo](https://github.com/kenryu42/cc-safety-net) · [📖 Docs ↗](https://ccsafetynet.com/docs) · [🌐 Site ↗](https://ccsafetynet.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-safety-net/)</sub>

<a name="superclaude-framework"></a>
### #&#8288;113 [superclaude_framework](https://github.com/superclaude-org/superclaude_framework) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (84) · Freshness: active (97) · Maintenance: patchy (33) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Sep 2026</sub>

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

<a name="agent-skills-for-context-engineering"></a>
### #&#8288;114 [agent-skills-for-context-engineering](https://github.com/muratcankoylan/agent-skills-for-context-engineering) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · MIT · Oct 2026</sub>

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
### #&#8288;115 [loop-engineering](https://github.com/cobusgreyling/loop-engineering) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: fair (58) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

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

<a name="trailofbits-skills"></a>
### #&#8288;116 [skills](https://github.com/trailofbits/skills) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.9k · CC-BY-SA-4.0 · Oct 2026</sub>

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

<a name="agents-cli"></a>
### #&#8288;117 [agents-cli](https://github.com/google/agents-cli) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · Apache-2.0 · Oct 2026</sub>

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
### #&#8288;118 [skills](https://github.com/dotnet/skills) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (59) · Freshness: active (99) · Maintenance: fair (77) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · MIT · Oct 2026</sub>

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
### #&#8288;119 [apm](https://github.com/microsoft/apm) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Oct 2026</sub>

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
### #&#8288;120 [cc-sdd](https://github.com/gotalab/cc-sdd) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Sep 2026</sub>

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

<a name="jevgrep"></a>
### #&#8288;121 [jevgrep](https://github.com/dzhng/jevgrep) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

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

<a name="ripwire"></a>
### #&#8288;122 [ripwire](https://github.com/redhat-et/ripwire) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (31) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="mex"></a>
### #&#8288;123 [mex](https://github.com/mex-memory/mex) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Git-shared project memory for engineers and their coding agents.**

MEX stores architecture notes, decisions and handoffs as Markdown in the repository, and links them to code symbols through a local Tree-sitter graph in SQLite. Engineers review and edit it in a local Hub on 127.0.0.1, while agents read it through the CLI and installed skills. Sharing happens through ordinary Git commits, with no hosted service.

- **+** Canonical memory is plain Markdown in the repo, shared via normal Git push and pull
- **+** Wiki claims are grounded to code symbols, with drift flags for review
- **+** Needs no hosted service, account or model key; indexes are rebuildable local SQLite
- **+** Relays record progress, tests and next steps for handing work to a teammate
- **−** Code graph covers TypeScript, JavaScript, Python and Rust; C# is partial
- **−** Requires Node.js 22.5+ with SQLite FTS5 support in that build
- **−** Team must upgrade together before sharing the 0.8.4 format
- **−** Hub is local per checkout; Relays are not delivered until pushed through Git

<sub>no GPU · Needs Node.js >=22.5, Git, SQLite FTS5 · Models: Claude Code, Codex · [Repo](https://github.com/mex-memory/mex) · [🌐 Site ↗](https://mexmemory.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mex/)</sub>

<a name="brooks-lint"></a>
### #&#8288;124 [brooks-lint](https://github.com/hyhmrright/brooks-lint) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Code review skills that cite classic engineering books for each finding.**

brooks-lint is a set of Agent Skills and a Claude Code plugin that reviews code against six production decay risks and six test-suite decay risks drawn from twelve engineering books. Each finding is reported as Symptom, Source, Consequence, Remedy with a severity and a 0–100 Health Score. It provides six commands (review, audit, debt, test, health, sweep) and optional SARIF export and CI gates.

- **+** Every finding carries a book citation, severity label and concrete remedy
- **+** Installs on Claude Code, Codex, Gemini, Cursor, Windsurf, Copilot and others
- **+** Per-project .brooks-lint.yaml sets strictness, disabled risks, ignores and custom risks
- **+** Parser benchmark is reproducible locally with npm run benchmark on a frozen 30-report corpus
- **−** Review quality depends on the host LLM; live evals need an Anthropic API key
- **−** Maintainer says only Codex is tested going forward; other platforms are unverified
- **−** Headline benchmark table is described as illustrative and compares against plain Claude
- **−** Does not check syntax or style; it complements a linter rather than replacing it

<sub>no GPU · Needs Claude Code, Codex CLI or another Agent Skills host, ANTHROPIC_API_KEY (live evals only) · Models: Claude, Codex, Gemini · [Repo](https://github.com/hyhmrright/brooks-lint) · [📖 Docs ↗](https://hyhmrright.github.io/brooks-lint/guide.html) · [🌐 Site ↗](https://hyhmrright.github.io/brooks-lint/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/brooks-lint/)</sub>

<a name="autoresearch"></a>
### #&#8288;125 [autoresearch](https://github.com/uditgoenka/autoresearch) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.8k · MIT · Aug 2026</sub>

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
### #&#8288;126 [lazycodex](https://github.com/code-yeongyu/lazycodex) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (49) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

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

<a name="one-skill-to-rule-them-all"></a>
### #&#8288;127 [one-skill-to-rule-them-all](https://github.com/rebelytics/one-skill-to-rule-them-all) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (46) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · CC-BY-4.0 · Oct 2026</sub>

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

<a name="pstack-claude"></a>
### #&#8288;128 [pstack-claude](https://github.com/michael-denyer/pstack-claude) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

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

<a name="stop-that-shit"></a>
### #&#8288;129 [stop-that-shit](https://github.com/lennney/stop-that-shit) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Oct 2026</sub>

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

<a name="skills-hub"></a>
### #&#8288;130 [skills-hub](https://github.com/qufei1993/skills-hub) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Desktop app that installs AI agent Skills once and syncs them to coding tools.**

Skills Hub is a desktop app for macOS, Windows and Linux that keeps one library of agent Skills and syncs them to 48 supported coding tools, including Claude Code, Codex, Cursor and OpenCode. Skills can be installed from collections, Git repositories or local folders, scoped globally or per project, and synced across devices through a GitHub, GitLab or Gitee repo.

- **+** Supports 48 coding tools plus custom tool directories
- **+** Imports Skills from Git, local folders or curated collections
- **+** Global or project scope, with bulk enable, disable and update
- **+** Cross-device sync via GitHub, GitLab or Gitee repository
- **−** Desktop app only; no Docker or hosted server option
- **−** macOS may flag the app as damaged or unverified on install
- **−** Collections are maintained in a separate repository
- **−** AI management setup is a manual step in Settings

<sub>no GPU · Needs Git hosting repo (GitHub, GitLab or Gitee) for optional device sync · [Repo](https://github.com/qufei1993/skills-hub) · [📖 Docs ↗](https://aiskillshub.link/docs) · [🌐 Site ↗](https://aiskillshub.link) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skills-hub/)</sub>

<a name="memu"></a>
### #&#8288;131 [memu](https://github.com/nevamind-ai/memu) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (78) · Freshness: active (97) · Maintenance: fair (53) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · custom license · Oct 2026</sub>

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

<a name="dsh-routing-suite"></a>
### #&#8288;132 [dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (72) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.0k · MIT · Sep 2026</sub>

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

<a name="claude-code-local"></a>
### #&#8288;133 [claude-code-local](https://github.com/nicedreamzapp/claude-code-local) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (44) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Oct 2026</sub>

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

<a name="lint"></a>
### #&#8288;134 [lint](https://github.com/shadcn-ui/lint) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (42) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Oct 2026</sub>

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

<a name="ruler"></a>
### #&#8288;135 [ruler](https://github.com/intellectronica/ruler) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (37) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Oct 2026</sub>

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

<a name="claude-blog"></a>
### #&#8288;136 [claude-blog](https://github.com/agricidaniel/claude-blog) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (32) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

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

<a name="unity-skills"></a>
### #&#8288;137 [unity-skills](https://github.com/besty0728/unity-skills) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

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

<a name="google-skills"></a>
### #&#8288;138 [skills](https://github.com/google/skills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · Apache-2.0 · Oct 2026</sub>

**Agent Skills for Google Cloud, Firebase, Ads and Analytics.**

Google's collection of Agent Skills covering Google Cloud services such as GKE, BigQuery, Cloud Run, AlloyDB and Spanner, plus Firebase, Genkit, Google Ads and Analytics APIs. Skills install into coding agents with `npx skills add google/skills`. The repo also bundles plugins (skills plus MCP servers) for Claude Code, Codex and Antigravity CLI.

- **+** Covers many Google products: GKE, BigQuery, security, Ads, Analytics, Genkit
- **+** One npx command installs; pick skills, target agents and project or global scope
- **+** Plugin bundles for Claude Code, Codex and Antigravity CLI
- **+** Maintained by Google; `npx skills update` pulls newer versions
- **−** Scoped to Google products; little use for other clouds or stacks
- **−** No tagged releases; updates follow the main branch
- **−** Documented install path requires Node.js and npx
- **−** Some skills are marked preview, such as the API Gateway remote MCP server

<sub>no GPU · Needs Node.js (npx), Google Cloud account for most skills · safety checks passed 10 of 11 · [Repo](https://github.com/google/skills) · [🌐 Site ↗](https://skills.sh/google/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-skills/)</sub>

<a name="vibe-skills"></a>
### #&#8288;139 [vibe-skills](https://github.com/foryourhealth111-pixel/vibe-skills) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="memsearch"></a>
### #&#8288;140 [memsearch](https://github.com/zilliztech/memsearch) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (35) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

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

<a name="token-optimizer"></a>
### #&#8288;141 [token-optimizer](https://github.com/alexgreensh/token-optimizer) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · custom license · Oct 2026</sub>

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

<a name="yomiyasu"></a>
### #&#8288;142 [yomiyasu](https://github.com/nanaism/yomiyasu) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: known (33) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Oct 2026</sub>

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

<a name="better-harness"></a>
### #&#8288;143 [better-harness](https://github.com/qoderai/better-harness) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

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

<a name="agentlas-os"></a>
### #&#8288;144 [agentlas-os](https://github.com/agentlas-ai/agentlas-os) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (89) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Oct 2026</sub>

**Task-splitting and specialist-agent staffing for Claude Code, Codex and Cursor.**

Agentlas OS (Hephaestus) installs into coding-agent hosts and splits a request into tasks. It then sources candidate agents for each task from local profiles, a private cloud and the public Hub. Candidates are unranked and the model picks one. The chosen release is pinned by digest, and an independent verifier must pass the result. It also builds portable agents with /hep-build and reads and writes A2A v1.0 agent cards.

- **+** Installs into many hosts: Claude Code, Codex, Cursor, Antigravity, OpenCode, Goose and others
- **+** SHA-256-checked installer, no sudo, and the README lists every path it writes
- **+** Picked agent releases are pinned by digest; an independent verifier must pass before a run is done
- **+** Uses standard A2A v1.0 agent cards, with signed-card identity checks for external agents
- **−** Install is a curl-pipe-bash script that edits existing host configs such as ~/.codex/config.toml
- **−** No backup is written when it edits existing host configs, apart from Codex marketplace changes
- **−** Optional global router appends about 75 lines to each host's global instructions file
- **−** Token-savings and recall figures are the project's own measurements, not independently checked

<sub>no GPU · Needs Claude Code, Codex, Cursor or Antigravity host, Model/API access supplied by the caller · Models: unknown · [Repo](https://github.com/agentlas-ai/agentlas-os) · [🌐 Site ↗](https://agentlas.cloud/desktop) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentlas-os/)</sub>

<a name="aegis"></a>
### #&#8288;145 [aegis](https://github.com/ganyuanran/aegis) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Skill pack that makes AI coding agents plan, verify and report evidence.**

Aegis is a method pack of SKILL.md-style skills that coding agents load to align with a project's baseline before editing and to attach verification evidence to completion claims. It installs through an agent prompt and a Python doctor script (scripts/aegis-doctor.py) on hosts such as Codex, OpenCode and Claude Code. It also provides optional TDD routing and an update command.

- **+** Works across many hosts: Codex, OpenCode, Claude Code, Kimi Code CLI, Copilot and others
- **+** Publishes an A/B benchmark: contract pass rate 61.67% to 93.33% over 120 runs
- **+** TDD mode is off by default and can be set to auto via a doctor command
- **+** Install is checked by a doctor script that outputs JSON with ok and configStatus
- **−** Benchmark covers one model setup (gpt-5.6-sol, xhigh); review was not independent human review
- **−** Only Codex and OpenCode have fresh host evidence; other hosts await release-level smoke tests
- **−** Skill triggering stays host-controlled and may need trigger-chain diagnosis
- **−** Not a runtime or gate: completion authority stays with the user and project rules

<sub>no GPU · Needs Python, AI coding host (Codex, OpenCode, Claude Code or similar) · [Repo](https://github.com/ganyuanran/aegis) · [📖 Docs ↗](https://github.com/GanyuanRan/Aegis/blob/main/docs/current/AEGIS_FAST_TRACK_PLAYBOOK.md) · [🌐 Site ↗](https://github.com/GanyuanRan/Aegis) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aegis/)</sub>

<a name="claude-plugins-official"></a>
### #&#8288;146 [claude-plugins-official](https://github.com/anthropics/claude-plugins-official) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 45k · Apache-2.0 · Oct 2026</sub>

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

<a name="hallmark"></a>
### #&#8288;147 [hallmark](https://github.com/nutlope/hallmark) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 39k · MIT · Oct 2026</sub>

**Design skill that builds and lints web pages to avoid AI-generated looks.**

Hallmark is a skill for Claude Code, Codex, Cursor and OpenCode that builds self-contained HTML and CSS pages from one of 48 themes, or from a custom direction. It lints the result in a real browser at eight widths against a list of AI-design tells, then has a fresh-context subagent review it. It also offers redesign and audit commands for existing pages.

- **+** Tiered gates (Floor, Reflex, Finish) cover contrast, focus, reduced motion and phone layout
- **+** 48 themes, each one file of at most 8 KB with a reference screenshot
- **+** Redesign checks that links, fields, handlers and headings survive via sloplint --before and --kept
- **+** One npx command installs it for Claude Code, Codex, Cursor and OpenCode; also a Claude plugin
- **−** Browser lint needs puppeteer-core and Chrome; without them only static checks run
- **−** Output is static HTML and CSS pages; no framework components are described
- **−** Photo library links Wikimedia Commons images with mixed licenses that need on-page credit
- **−** May not fire on its own; sometimes has to be invoked by name

<sub>no GPU · Needs Node 18+, puppeteer-core, Chrome · Models: Claude Code, Codex CLI, Cursor, OpenCode · safety checks passed 9 of 10 · [Repo](https://github.com/nutlope/hallmark) · [▶️ Demo ↗](https://www.usehallmark.com) · [🌐 Site ↗](https://www.usehallmark.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hallmark/)</sub>

<a name="autoharness"></a>
### #&#8288;148 [autoharness](https://github.com/tigerless-labs/autoharness) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Oct 2026</sub>

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

<a name="swiftui-agent-skill"></a>
### #&#8288;149 [swiftui-agent-skill](https://github.com/twostraws/swiftui-agent-skill) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Oct 2026</sub>

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

<a name="claude-scholar"></a>
### #&#8288;150 [claude-scholar](https://github.com/galaxy-dawn/claude-scholar) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (60) · Freshness: active (95) · Maintenance: fair (62) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.9k · MIT · Oct 2026</sub>

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

<a name="avdlee-swiftui-agent-skill"></a>
### #&#8288;151 [swiftui-agent-skill](https://github.com/avdlee/swiftui-agent-skill) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (48) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

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
### #&#8288;152 [cc-skills-golang](https://github.com/samber/cc-skills-golang) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="pg-aiguide"></a>
### #&#8288;153 [pg-aiguide](https://github.com/timescale/pg-aiguide) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="spec-kitty"></a>
### #&#8288;154 [spec-kitty](https://github.com/spec-kitty/spec-kitty) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Oct 2026</sub>

**CLI that runs spec, plan, tasks and review workflows for AI coding agents.**

Spec Kitty is a Python CLI that stores specs, plans, work packages and review state in the repository under kitty-specs/. It installs slash commands or skills for agents such as Claude Code, Codex, Cursor, Gemini and Copilot, and gives each work package its own git worktree so agents can work in parallel. Work moves through a spec, plan, tasks, next, review, accept, merge loop.

- **+** Keeps specs, tasks, review and merge state in Git rather than in chat history
- **+** Isolated git worktrees under .worktrees/ per work package for parallel agents
- **+** Supports many agents, including Claude Code, Codex, Cursor, Gemini, Copilot, Windsurf, OpenCode
- **+** Local-first; README states no SaaS service is required
- **−** 4.x line is a release candidate; stable launch acceptance is stated as pending
- **−** Hosted auth, sync and tracker flows were removed from open-core
- **−** Overkill for one-off edits, small scripts or teams not using Git
- **−** Does not write code itself; depends on a separate coding agent

<sub>no GPU · Needs Python 3.11+, Git, An AI coding agent (Claude Code, Codex, Cursor, etc.) · Models: Claude Code, Codex, Cursor, Gemini, GitHub Copilot · [Repo](https://github.com/spec-kitty/spec-kitty) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spec-kitty/)</sub>

<a name="pm-claude-skills"></a>
### #&#8288;155 [pm-claude-skills](https://github.com/mohitagw15856/pm-claude-skills) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Library of 1,305 markdown Agent Skills for Claude, Cursor, Codex and others.**

A collection of SKILL.md files, each teaching an AI assistant one professional task such as writing a PRD, decoding a lease or running a postmortem. Each skill bundles a framework, output template and quality checks. An npx installer copies chosen skills into the config folder of the tool in use, and a Claude Code plugin and MCP server are also provided.

- **+** Plain markdown files; installing copies text and uninstalling deletes it, no runtime or account
- **+** Installs into Cursor, Codex, Windsurf, Cline and Zed via npx, plus Claude plugin, MCP and REST access
- **+** 153 bundles grouped by job, with 178 translations in 10 languages
- **+** CI checks structure, near-duplicates and a 15-document prompt-injection suite on every change
- **−** Mostly non-coding content (PM, job search, document decoding); little aimed at software engineering
- **−** Only 409 of 1,305 skills have eval cases; 399 have blind-judged scores
- **−** 0 of 161 high-stakes skills have a current review by a qualified professional
- **−** ChatGPT and Gemini use copied exports rather than a native install

<sub>no GPU · Docker · Needs Node.js (npx) · Models: Claude, ChatGPT, Gemini, Cursor, Codex · [Repo](https://github.com/mohitagw15856/pm-claude-skills) · [▶️ Demo ↗](https://mohitagw15856.github.io/pm-claude-skills/) · [📖 Docs ↗](https://github.com/mohitagw15856/pm-claude-skills/blob/main/docs/installation.md) · [🌐 Site ↗](https://mohitagw15856.github.io/pm-claude-skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pm-claude-skills/)</sub>

<a name="oh-my-agent"></a>
### #&#8288;156 [oh-my-agent](https://github.com/first-fluke/oh-my-agent) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Adds planner, engineer, reviewer and debugger roles to your existing coding agent.**

oma is a CLI and portable .agents/ directory that adds 12 specialist roles, 21 workflows (/plan, /work, /orchestrate, /ultrawork, /ralph, /review, /debug) and 33 skills to coding agents such as Claude Code, Codex CLI and Cursor. Hooks keep long-running workflows going until your own test, lint or typecheck script passes. Steps write plans, results and review findings as files under .agents/ and docs/.

- **+** One .agents/ directory is written into the config files of 14 agent runtimes
- **+** Stop gate sends the agent back to work until your test or lint script passes
- **+** Plans, ADRs, review findings and per-agent results are plain files you can open
- **+** MIT license; install via script, bun, npm or brew
- **−** Installer writes outside the project: ~/.claude.json, ~/.serena, ~/.cursor and other vendor configs
- **−** Sets Claude Code defaults including skipDangerousModePermissionPrompt and telemetry opt-outs
- **−** Adds a co-author trailer and a commit-msg git hook unless disabled in config
- **−** Several workflows need the All skill preset; smaller presets lack /plan or /review skills

<sub>no GPU · Needs bun, uv, Serena, CUE, AgentMemory, Aside browser MCP · Models: Claude Code, Codex CLI, Cursor · [Repo](https://github.com/first-fluke/oh-my-agent) · [📖 Docs ↗](https://first-fluke.github.io/oh-my-agent/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-agent/)</sub>

<a name="antfu-skills"></a>
### #&#8288;157 [skills](https://github.com/antfu/skills) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.0k · MIT · Oct 2026</sub>

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

<a name="potpie"></a>
### #&#8288;158 [potpie](https://github.com/potpie-ai/potpie) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="pi-mcp-adapter"></a>
### #&#8288;159 [pi-mcp-adapter](https://github.com/nicobailon/pi-mcp-adapter) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**MCP adapter for the Pi coding agent using one lazy proxy tool.**

Extension for the Pi coding agent that exposes MCP servers through a single `mcp` proxy tool (about 200 tokens) instead of loading every tool definition. Servers start on first call and stop after 10 idle minutes by default, and tool metadata is cached so search works without live connections. It reads `.mcp.json`, imports Cursor, Claude Code, Codex and VS Code configs, and replaces Pi's built-in MCP.

- **+** Lazy server start with 10-minute idle stop; README measured 0 of 100 servers running at session start
- **+** Supports MCP prompts, elicitation, sampling, Tasks and UI apps, unlike Pi's built-in MCP
- **+** OAuth tokens stored in the OS keychain by default
- **+** Imports existing Cursor, Claude Code, Codex and VS Code configs via /mcp-adapter setup
- **−** Only works with Pi; not a standalone MCP client
- **−** Bulk tasks cost up to 5.5x more tokens than Pi's built-in without scripting
- **−** Semantic tool search needs a System One key
- **−** Sampling is text-only; each Pi session runs its own server processes

<sub>no GPU · Needs Pi coding agent (0.99 or later), Node.js and npm · [Repo](https://github.com/nicobailon/pi-mcp-adapter) · [📖 Docs ↗](https://github.com/nicobailon/pi-mcp-adapter/blob/main/docs/configuration.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-mcp-adapter/)</sub>

<a name="ios-simulator-skill"></a>
### #&#8288;160 [ios-simulator-skill](https://github.com/conorluddy/ios-simulator-skill) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: healthy (97) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Agent skill that builds, tests and drives iOS apps in the Simulator.**

A skill and plugin for Claude Code and Codex that wraps xcodebuild, xcrun simctl and idb in 30 Python scripts. Agents build and test Xcode projects, navigate the simulator through the accessibility tree rather than pixel taps, and run audits such as WCAG checks, visual diffs and hang capture. Output is kept to a few lines, with details fetched on demand by xcresult ID.

- **+** Accessibility-tree navigation by text, type or id instead of fragile pixel coordinates
- **+** build_and_test.py returns a one-line summary and xcresult ID; errors and logs fetched on demand
- **+** 30 scripts cover boot, privacy, push, location, status bar, a11y audit and localization
- **+** Installs as a plugin for both Claude Code and Codex; all limits tunable via IOS_SIM_* variables
- **−** macOS only; requires Apple silicon, macOS 15+ and full Xcode 26+
- **−** Needs idb 1.5.1+ installed separately; older idb on Xcode 27 silently drops taps
- **−** Requires Python 3.12+; Pillow needed for visual diffs
- **−** Manual install is easy to get wrong because SKILL.md sits three levels deep in the repo

<sub>no GPU · Needs macOS 15+, Xcode 26+, idb 1.5.1+, Python 3.12+, Pillow (visual diffs) · [Repo](https://github.com/conorluddy/ios-simulator-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ios-simulator-skill/)</sub>

<a name="garden-skills"></a>
### #&#8288;161 [garden-skills](https://github.com/conardli/garden-skills) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 13k · MIT · Oct 2026</sub>

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

<a name="trail-code"></a>
### #&#8288;162 [trail-code](https://github.com/trailhq/trail-code) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Oct 2026</sub>

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

<a name="awesome-codex-subagents"></a>
### #&#8288;163 [awesome-codex-subagents](https://github.com/voltagent/awesome-codex-subagents) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (63) · Freshness: active (100) · Maintenance: fair (61) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.4k · MIT · Oct 2026</sub>

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

<a name="awesome-gamedev-agent-skills"></a>
### #&#8288;164 [awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: popular (57) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.2k · Apache-2.0 · Oct 2026</sub>

**74 game-dev Agent Skills with a router that loads the right ones per request.**

A collection of 74 SKILL.md files covering Godot, Unity, Unreal, Phaser, PixiJS, three.js, Bevy, pygame, LÖVE and Roblox, plus a router skill. The router detects the engine from project files (for example project.godot or *.uproject), reads the task, and loads only matching engine, discipline, genre and workflow skills. Installs with `npx skills add` or as a Claude Code plugin marketplace.

- **+** Router picks skills from engine detection, so users never name skills
- **+** Covers 10 engines, each pinned to a stated version (e.g. Godot 4.7, Unity 6.3 LTS)
- **+** Plain SKILL.md files load in Claude Code, Cursor, Windsurf, Cline, Codex, Gemini CLI and others
- **+** Includes an asset art-direction workflow and a validator script for skill quality
- **−** Skill depth is uneven: Unreal has 6 skills, Godot 16
- **−** Version pins will go stale as engines release; upgrade policy lives in separate docs
- **−** Demo in the README is illustrative only, not a recorded run
- **−** Only 9 genres and 4 workflows are covered

<sub>no GPU · Needs Node.js (npx skills CLI), an AI coding agent that supports Agent Skills · [Repo](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) · [📖 Docs ↗](https://gamedev-skills.github.io/awesome-gamedev-agent-skills/) · [🌐 Site ↗](https://gamedev-skills.github.io/awesome-gamedev-agent-skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-gamedev-agent-skills/)</sub>

<a name="expo-skills"></a>
### #&#8288;165 [skills](https://github.com/expo/skills) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (43) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · MIT · Oct 2026</sub>

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

<a name="teaql-agent-kit"></a>
### #&#8288;166 [teaql-agent-kit](https://github.com/teaql/teaql-agent-kit) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (79) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

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

<a name="open-vibe-island"></a>
### #&#8288;167 [open-vibe-island](https://github.com/octane0411/open-vibe-island) <sub>score [67](../README.md#-how-we-rank "Score 67/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (76) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · GPL-3.0 · Oct 2026</sub>

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

<a name="prompt-master"></a>
### #&#8288;168 [prompt-master](https://github.com/nidhinjs/prompt-master) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 15k · MIT · Oct 2026</sub>

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

<a name="ag-kit"></a>
### #&#8288;169 [ag-kit](https://github.com/vudovn/ag-kit) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.2k · MIT · Aug 2026</sub>

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

<a name="vibe-coding-prompt-template"></a>
### #&#8288;170 [vibe-coding-prompt-template](https://github.com/khazp/vibe-coding-prompt-template) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Oct 2026</sub>

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
### #&#8288;171 [aiox-core](https://github.com/synkraai/aiox-core) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · custom license · Aug 2026</sub>

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

<a name="supabase-agent-skills"></a>
### #&#8288;172 [agent-skills](https://github.com/supabase/agent-skills) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

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

<a name="claude-reflect"></a>
### #&#8288;173 [claude-reflect](https://github.com/bayramannakov/claude-reflect) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

**Claude Code plugin that turns your corrections into CLAUDE.md rules and skills.**

claude-reflect is a Claude Code plugin that uses hooks to queue corrections you make during sessions, then writes approved ones to CLAUDE.md (global, project, subdirectory) and AGENTS.md via /reflect. /reflect-skills scans session history for repeated requests and drafts slash-command files in .claude/commands/. A separate reflect-mod variant checks each short prompt with a model and shows a save prompt in the session.

- **+** Human review step: nothing is written to CLAUDE.md without approval
- **+** Syncs to CLAUDE.md, subdirectory CLAUDE.md files, skill files and AGENTS.md (Codex, Cursor, Aider)
- **+** /reflect --scan-history recovers corrections from past sessions; --dedupe merges similar entries
- **+** Runs on macOS, Linux and Windows with Python 3.6+; 332 tests reported
- **−** Plugin capture uses regex; multi-language detection only happens at /reflect time
- **−** Depends on Claude Code session history, which is deleted after 30 days by default
- **−** Mod and plugin must not be installed together or corrections are captured twice
- **−** Mod is early access and needs Claude Code 2.1.286+ and a model call per prompt

<sub>no GPU · Needs Claude Code CLI, Python 3.6+ · Models: Claude (haiku by default for reflect-mod checks) · [Repo](https://github.com/bayramannakov/claude-reflect) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-reflect/)</sub>

<a name="aoci-code"></a>
### #&#8288;174 [aoci-code](https://github.com/aoci-spec/aoci-code) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · custom license · Oct 2026</sub>

**Git-versioned per-file codebase index that coding agents read and update via MCP.**

AOCI-CODE is a Go CLI (`aoci`) and local stdio MCP server that has your coding agent write one plain-text entry per file (responsibility, dependencies, public contracts, constraints) into `aoci.code.txt` in the repo. Agents read the index before a task instead of re-reading the codebase, and the server flags entries to update after code changes. It can also index MySQL, PostgreSQL and openGauss table structure.

- **+** Index is plain text in the repo, so Git diffs, reviews and rollbacks work
- **+** Works with any host supporting stdio MCP: Codex, Claude Code, Cursor, OpenCode
- **+** Local only: reads source and DB schema, no Internet access, no stored credentials
- **+** Optional table-level index for MySQL 5.7.6+, PostgreSQL and openGauss 6.0.5
- **−** First index is slow: about an hour per 200,000 lines of code
- **−** Release candidate (v0.1.0-rc21); no stable release published
- **−** FSL-1.1-MIT source-available license, not a standard OSI open-source license
- **−** Index quality depends on the agent's model; MariaDB is not supported for database indexing

<sub>no GPU · Needs Git, MCP-capable coding agent host, Go toolchain and make (source builds only), MySQL, PostgreSQL or openGauss (optional, for database index) · Models: Any model via MCP host (Codex, Claude Code, Cursor, OpenCode) · [Repo](https://github.com/aoci-spec/aoci-code) · [📖 Docs ↗](https://github.com/aoci-spec/aoci-code/blob/v0.1.0-rc21/docs/install.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/aoci-code/)</sub>

<a name="backpass"></a>
### #&#8288;175 [backpass](https://github.com/kunchenguid/backpass) <sub>score [66](../README.md#-how-we-rank "Score 66/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**CLI that proposes evidence-backed edits to AGENTS.md, CLAUDE.md and skills.**

backpass reads agent session transcripts from disk for seven harnesses (Claude Code, Codex, Pi, OpenCode, Grok, Cursor CLI, Hermes), locally or over SSH. It distills them into proposed edits to your AGENTS.md or CLAUDE.md and project skills, each backed by verbatim quotes from at least two sessions. Analysis never writes; you accept or reject each edit in `backpass apply`.

- **+** Every add, rewrite or remove edit needs quotes from at least two distinct sessions
- **+** Reads transcript stores directly from disk; no upload, and it has no API keys of its own
- **+** Supports project scope and user scope (--scope user) plus SSH collection from other machines
- **+** Analysis never writes files; changes only land after explicit review in apply
- **−** Requires Node >= 22.5 and acpx on PATH; default review UI also needs lavish-axi
- **−** macOS and Linux only; Windows remotes are out of scope
- **−** User scope collects only Claude and Codex sessions by default
- **−** Model calls go through an already-authenticated harness, so usage costs are unknown

<sub>no GPU · Needs Node >= 22.5, acpx, lavish-axi (for default review UI), ssh (optional, for remote hosts) · Models: Claude Code, Codex, Pi, OpenCode, Grok · [Repo](https://github.com/kunchenguid/backpass) · [🌐 Site ↗](https://blog.kunchenguid.com/p/your-agentsmd-is-a-neural-net) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/backpass/)</sub>

<a name="unlazy"></a>
### #&#8288;176 [unlazy](https://github.com/leonxlnx/unlazy) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.2k · MIT · Sep 2026</sub>

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

<a name="earshot"></a>
### #&#8288;177 [earshot](https://github.com/leonxlnx/earshot) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (39) · Freshness: active (100) · Maintenance: fair (78) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

**Audio analysis and sound synthesis for coding agents, as CLI, Python API and MCP.**

earshot lets a coding agent hear audio: it describes files in words, matches them to text descriptions, finds moments in long recordings, and scores a film's sound against a profile of 7 launch films. It also synthesizes sounds from code recipes (`forge`), fits recordings to recipes (`fit`), and renders from a bank of 201 code-defined effects. It runs on CPU using CLAP and an AudioSet AST tagger.

- **+** Exposes the same tools as CLI, Python API and MCP server for Claude Code
- **+** Runs on CPU only; models are pinned revisions with safetensors weights, loaded offline after first fetch
- **+** sfx and kit commands render from the 201-sound bank with no models or network
- **+** README states its limits, including a coin-flip blind test and Goodhart risk in the critic
- **−** Each CLI call reloads models, about 20-40 s; MCP or Python needed for many calls
- **−** First use downloads about 1.1 GB of models
- **−** Forge reference recordings are licensed and not in the repo; --refset needs a local registry
- **−** No published blind-test score for the v2 sounds; the v1 test used one listener

<sub>no GPU · Needs Python 3.10+, ffmpeg, ffprobe, PyTorch (CPU), Hugging Face model download (first run) · Models: CLAP laion/larger_clap_general, MIT/ast-finetuned-audioset-10-10-0.4593, Gemini (optional audio critique) · [Repo](https://github.com/leonxlnx/earshot) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/earshot/)</sub>

<a name="wondelai-skills"></a>
### #&#8288;178 [skills](https://github.com/wondelai/skills) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Sep 2026</sub>

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

<a name="oil-ui"></a>
### #&#8288;179 [oil-ui](https://github.com/oil-oil/oil-ui) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

**Agent skill that explores distinct UI design directions and refines the chosen one.**

Oil UI is an installable skill for AI coding agents that generates several genuinely different design directions for a website, app, dashboard or component. It puts them on a comparison page, lets you pick one, then refines it against desktop and mobile screenshots. The free edition covers design direction, visuals and screenshot recreation; usability, polish and existing-project work are in the paid Pro edition.

- **+** Installs with one command, npx skills add oil-oil/oil-ui, no configuration
- **+** Built-in comparison page with desktop/mobile switching and arrow-key browsing
- **+** Directions must differ in layout, typography, color and imagery, sharing at most one
- **+** Checks results against real screenshots at desktop and mobile sizes
- **−** Usability, polish, dashboard and existing-project workflows are only in Pro ($9.99)
- **−** Independent review is limited to a score with issues listed in the free edition
- **−** Checks ui.oiloil.org for updates on use; needs Python 3 (can be disabled)
- **−** Installing alongside Pro makes both compete for the same requests

<sub>no GPU · Needs Python 3, npx (skills CLI), an AI coding agent that supports skills · [Repo](https://github.com/oil-oil/oil-ui) · [▶️ Demo ↗](https://ui.oiloil.org/en/?utm_source=github&utm_medium=referral&utm_campaign=readme-en) · [🌐 Site ↗](https://ui.oiloil.org/en/?utm_source=github&utm_medium=referral&utm_campaign=readme-en) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oil-ui/)</sub>

<a name="vibe-coding-toolkit"></a>
### #&#8288;180 [vibe-coding-toolkit](https://github.com/soumatheusgomes/vibe-coding-toolkit) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

**Prompts and templates that set up machines and projects for coding agents.**

A set of markdown prompts, docs and templates that you paste into a coding agent to configure a dev machine, bootstrap a new Next.js project, or upgrade an existing one. The agent installs and wires tools such as Superpowers, Context7, RTK and Vercel skills, writes AGENTS.md and project docs, and runs checks. No application code lives here; it is a recipe the agent executes.

- **+** Separate prompts for machine setup, new-project bootstrap and existing-project adoption
- **+** Separate guides for Claude Code and Codex, plus shared AGENTS.md template
- **+** Prompts can be adopted one at a time, e.g. only the ESLint quality gates
- **+** Validation documented on macOS, Linux and Windows; CI runs on Ubuntu and Windows
- **−** Needs an agent with file and terminal access; plain chat installs nothing
- **−** New-project path is Next.js only, with Drizzle and PostgreSQL defaults
- **−** Remote prompts are fetched from main, so results shift as the repo changes
- **−** No tagged releases; installed tools depend on third-party projects and upstream docs

<sub>no GPU · Needs Claude Code or Codex, Node.js, Next.js, PostgreSQL · Models: Claude Code, Codex · [Repo](https://github.com/soumatheusgomes/vibe-coding-toolkit) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibe-coding-toolkit/)</sub>

<a name="kicad-happy"></a>
### #&#8288;181 [kicad-happy](https://github.com/aklofas/kicad-happy) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Skills that let coding agents review KiCad schematics, PCBs and Gerbers.**

A set of 11 agent skills plus pure-Python scripts that parse KiCad schematics, PCB layouts and Gerbers into structured data. They compute regulator outputs, filters and derating, run SPICE testbenches, and check EMC with 44 rules. It installs as a plugin for Claude Code, Codex, Copilot CLI, Antigravity and opencode, and also runs as a GitHub Action for PR reviews.

- **+** Analysis scripts are pure Python 3.10+ with no required dependencies or KiCad install
- **+** Works across five agent CLIs and as a GitHub Action for PR checks
- **+** Covers power tree, ESD, thermal, EMC (44 rules) and SPICE with Monte Carlo
- **+** Includes supplier skills for DigiKey, Mouser, LCSC, element14, JLCPCB and PCBWay
- **−** SPICE simulation needs ngspice, LTspice or Xyce; it is skipped without one
- **−** Supplier skills (e.g. DigiKey) use APIs, which likely need credentials; README excerpt is silent
- **−** Claude Code /plugin update may miss new versions; cache must be cleared manually
- **−** Only supports KiCad projects, not other EDA tools

<sub>no GPU · Needs Python 3.10+, ngspice, LTspice or Xyce (optional, for SPICE) · Models: Claude Code, OpenAI Codex, GitHub Copilot CLI, Google Antigravity, opencode · [Repo](https://github.com/aklofas/kicad-happy) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kicad-happy/)</sub>

<a name="repository-harness"></a>
### #&#8288;182 [repository-harness](https://github.com/hoangnb24/repository-harness) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Agent-ready repo map, explicit skills and a safe updater for existing repositories.**

repository-harness installs a compact AGENTS.md entrypoint, a documentation map, optional plan and decision templates, and explicit-only skills into an existing repository. A Rust `harness` binary handles status, doctor and update, using a three-way merge against the upstream base stored in `.harness-core/`. It is not a task tracker, orchestrator or runtime.

- **+** Updater does three-way merge, backs up files and changes nothing on conflict
- **+** Skills run only when explicitly invoked; installation activates nothing
- **+** Installs no database, credentials or background processes
- **+** Installer offers dry-run and merge modes, with Bash and PowerShell scripts
- **−** Installer is run via curl piped to bash
- **−** Does not supply validation commands, runtimes or fixtures for your application
- **−** Legacy SQLite harness-cli and protocol v1 ended support on 2026-08-10
- **−** Overlapping local and upstream edits need manual resolution before update continues

<sub>no GPU · Needs bash or PowerShell, curl · [Repo](https://github.com/hoangnb24/repository-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repository-harness/)</sub>

<a name="moai-adk"></a>
### #&#8288;183 [moai-adk](https://github.com/modu-ai/moai-adk) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · Apache-2.0 · Oct 2026</sub>

**Go CLI harness that wraps Claude Code with SPEC workflow and verified completion claims.**

MoAI-ADK is a Go CLI that wraps Claude Code with a plan, run, sync SPEC lifecycle and binds completion claims to the command actually run and its output. Factory Mode (v3.2) splits work across one leader session and numbered lane sessions, each carrying a card through its stages in its own worktree. It also offers a local web console, a SQLite-backed task queue, and launchers for GLM and Codex backends.

- **+** Completion claims must cite the command run and its output
- **+** Per-SPEC git worktrees and a branch guard keep parallel agents from colliding
- **+** Factory Mode spreads cards across lanes on Claude, GLM or Codex backends
- **+** Progress files and memory let work survive /clear
- **−** Lanes must be launched by hand, one terminal each
- **−** Built around Claude Code; Codex can only join as a lane
- **−** MOAI_HOME is read only by Go processes, so shell hooks and statusline can split state
- **−** Large command and concept surface (SPEC tiers, cards, lanes, runs) to learn

<sub>no GPU · Needs Claude Code, SQLite · Models: Claude, GLM, Codex · [Repo](https://github.com/modu-ai/moai-adk) · [📖 Docs ↗](https://adk.mo.ai.kr/en/advanced/factory-mode) · [🌐 Site ↗](https://adk.mo.ai.kr) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/moai-adk/)</sub>

<a name="security-audit-skill"></a>
### #&#8288;184 [security-audit-skill](https://github.com/cloudflare/security-audit-skill) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 51k · MIT · Sep 2026</sub>

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

<a name="harness"></a>
### #&#8288;185 [harness](https://github.com/revfactory/harness) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · Apache-2.0 · Sep 2026</sub>

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

<a name="council-of-high-intelligence"></a>
### #&#8288;186 [council-of-high-intelligence](https://github.com/0xnyk/council-of-high-intelligence) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.7k · MIT · Oct 2026</sub>

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
### #&#8288;187 [sol-pi](https://github.com/nvlabs/sol-pi) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (46) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.6k · MIT · Oct 2026</sub>

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

<a name="claude-code-tools"></a>
### #&#8288;188 [claude-code-tools](https://github.com/pchalasani/claude-code-tools) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: healthy (90) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="agents-md"></a>
### #&#8288;189 [agents.md](https://github.com/agentsmd/agents.md) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 25k · MIT · Sep 2026</sub>

**Open Markdown format for giving coding agents project instructions.**

AGENTS.md is a specification for a plain Markdown file kept in a repo that holds dev environment, testing and PR instructions for AI coding agents. The repository also contains the Next.js site served at agents.md, which explains the format and lists examples. It has no runtime or agent code.

- **+** Plain Markdown, no tooling, schema or dependencies required
- **+** One predictable file location for agent instructions, separate from the human README
- **+** Website runs locally with pnpm install and pnpm run dev
- **−** No enforced schema; README shows only a minimal example
- **−** Repo holds the website and spec, not a tool or agent
- **−** README does not list which agents read the file
- **−** No releases published

<sub>no GPU · Needs Node.js, pnpm · port 3000 · safety checks passed 2 of 4 · [Repo](https://github.com/agentsmd/agents.md) · [🌐 Site ↗](https://agents.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents-md/)</sub>

<a name="agent-memory"></a>
### #&#8288;190 [agent-memory](https://github.com/tigerless-labs/agent-memory) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: patchy (43) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.4k · MIT · Oct 2026</sub>

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

<a name="ctf-skills"></a>
### #&#8288;191 [ctf-skills](https://github.com/ljagiello/ctf-skills) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: known (46) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.5k · MIT · Oct 2026</sub>

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
### #&#8288;192 [openwolf](https://github.com/cytostack/openwolf) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · AGPL-3.0 · Oct 2026</sub>

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
### #&#8288;193 [edgeone-makers-tools](https://github.com/tencentedgeone/edgeone-makers-tools) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

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

<a name="rulesync"></a>
### #&#8288;194 [rulesync](https://github.com/dyoshikawa/rulesync) <sub>score [63](../README.md#-how-we-rank "Score 63/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**CLI that generates config files for many AI coding tools from one rule set.**

Rulesync is a Node.js CLI that keeps AI tool configuration in a single `.rulesync/` source directory and generates the files each tool expects. It covers rules, ignore files, MCP config, commands, subagents, skills, hooks and permissions for dozens of tools, including Claude Code, Cursor, Copilot, Codex CLI and Cline. It can also import existing configs or convert directly between tool formats.

- **+** One source directory generates configs for 60+ listed tools, so rules are not duplicated
- **+** `import` pulls existing CLAUDE.md, .cursorrules or Copilot files into .rulesync/
- **+** `convert --from cursor --to copilot,claudecode` translates formats without .rulesync/ files
- **+** Installs via npm, Homebrew or a single binary
- **−** Feature support varies per tool; many targets lack ignore, hooks or checks
- **−** Several targets are deprecated or end of life (Roo Code, Continue, Tabnine legacy)
- **−** The `ignore` feature is deprecated in favor of `permissions`
- **−** Plugin-packaging targets are excluded from `--targets "*"` and need explicit output roots

<sub>no GPU · Needs Node.js · [Repo](https://github.com/dyoshikawa/rulesync) · [📖 Docs ↗](https://rulesync.dyoshikawa.com/) · [🌐 Site ↗](https://rulesync.dyoshikawa.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rulesync/)</sub>

<a name="huggingface-skills"></a>
### #&#8288;195 [skills](https://github.com/huggingface/skills) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs hf CLI, Hugging Face Hub account, AWS account (SageMaker skills) · Models: Safetensors, GGUF · safety checks passed 9 of 11 · [Repo](https://github.com/huggingface/skills) · [📖 Docs ↗](https://huggingface.co/docs/hub/agents-cli) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huggingface-skills/)</sub>

<a name="longmemory"></a>
### #&#8288;196 [longmemory](https://github.com/caviraoss/longmemory) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (54) · Freshness: active (89) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · Apache-2.0 · Oct 2026</sub>

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

<a name="gemini-skills"></a>
### #&#8288;197 [gemini-skills](https://github.com/google-gemini/gemini-skills) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · Apache-2.0 · Oct 2026</sub>

**Agent skills that teach coding assistants current Gemini API and SDK usage.**

A set of three skills that give coding agents up-to-date context on the Gemini API: gemini-api-dev (Interactions API, Python and TypeScript SDKs), gemini-live-api-dev (realtime streaming), and gemini-omni-flash-api (video generation and editing). The README reports that adding the skill raised correct API code generation to 87% with Gemini 3 Flash and 96% with Gemini 3.1 Pro. It installs via the Vercel or Context7 skills CLIs, or as a plugin for Claude Code, Cursor, Codex and Antigravity.

- **+** Installs through several routes: skills CLIs, Claude Code, Cursor, Codex and Antigravity plugins
- **+** Covers Interactions API, Live API and Omni Flash video in separate, individually installable skills
- **+** README cites eval results: 87% with Gemini 3 Flash, 96% with Gemini 3.1 Pro
- **+** Apache-2.0 licensed and maintained by the google-gemini organization
- **−** Only helps with Gemini API code; not useful for other model providers
- **−** README states it is not an officially supported Google product
- **−** The vertex-ai-api-dev skill moved to a different repository
- **−** No tagged releases, so version pinning relies on commits

<sub>no GPU · Needs Gemini API, Node.js (npx for skills CLIs) · Models: Gemini 3 Flash, Gemini 3.1 Pro, Gemini Omni 1.1 Flash · [Repo](https://github.com/google-gemini/gemini-skills) · [📖 Docs ↗](https://ai.google.dev/gemini-api/docs/coding-agents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gemini-skills/)</sub>

<a name="tons-of-skills-marketplace"></a>
### #&#8288;198 [tons-of-skills-marketplace](https://github.com/jeremylongshore/tons-of-skills-marketplace) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (48) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.9k · MIT · Oct 2026</sub>

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

<a name="context-engineering-kit"></a>
### #&#8288;199 [context-engineering-kit](https://github.com/neolabhq/context-engineering-kit) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (20) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · GPL-3.0 · Aug 2026</sub>

**Plugin marketplace of context-engineering skills and commands for coding agents.**

A marketplace of plugins for Claude Code, also installable on Gemini CLI, Antigravity, Cursor, Codex and OpenCode. Plugins cover reflection loops (/reflect, /memorize), spec-driven and subagent-driven development with judge agents, multi-agent PR review, git commands, TDD and language-specific rules. Each plugin loads only its own agents, commands and skills to limit token use.

- **+** Granular install: each Claude Code plugin loads only its own agents, commands and skills
- **+** Skills follow the agentskills.io format and install on several agents via npx skills
- **+** Review plugin runs specialized agents and has a documented GitHub Actions integration
- **+** Covers reflection, spec-driven and subagent-driven workflows in one marketplace
- **−** Gemini CLI and Antigravity install every plugin as one bundle, no per-plugin selection
- **−** npx skills install does not support subagents, so non-Claude setups get a reduced experience
- **−** Reliability percentages come from the authors' own usage, not a published benchmark
- **−** Higher-reliability workflows add 5x-35x token overhead

<sub>no GPU · Needs Claude Code or another supported coding agent, bun (for the automatic reflect hook) · [Repo](https://github.com/neolabhq/context-engineering-kit) · [📖 Docs ↗](https://neolab.gitbook.io/cek/) · [🌐 Site ↗](https://neolab.gitbook.io/cek/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-engineering-kit/)</sub>

<a name="ai-devkit"></a>
### #&#8288;200 [ai-devkit](https://github.com/codeaholicguy/ai-devkit) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: healthy (88) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

**CLI that configures, supervises and shares memory across coding agents.**

AI DevKit is an npm CLI that writes one .ai-devkit.json and generates setup (rules, MCP servers, skills) for coding agents such as Claude Code, Codex CLI, Gemini CLI, Cursor and opencode. It adds a TUI console for running sessions, an `agent send` command that routes prompts or stdin to live agents, and a local SQLite memory exposed over MCP and CLI. It also installs skills such as dev-lifecycle, verify and tdd.

- **+** One .ai-devkit.json reconciles setup for 16 listed coding agents
- **+** `agent console`, `agent list` and `agent send` supervise and message running sessions
- **+** Memory is a local SQLite file, searched via MCP or CLI on demand
- **+** Runs locally; README states no telemetry and writes project files you can commit
- **−** Remote control is unavailable for several agents, including Cursor, Copilot, Cline and Devin
- **−** Roo Code setup and opencode remote control are marked as testing
- **−** Phase-doc workflow (requirements to testing) adds process overhead to small changes
- **−** Does not improve model quality; README says it only raises process discipline

<sub>no GPU · Needs Node.js, npm, SQLite · [Repo](https://github.com/codeaholicguy/ai-devkit) · [📖 Docs ↗](https://ai-devkit.com/docs/) · [🌐 Site ↗](https://ai-devkit.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-devkit/)</sub>

<a name="attention-span"></a>
### #&#8288;201 [attention-span](https://github.com/alexgreensh/attention-span) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (94) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · AGPL-3.0 · Oct 2026</sub>

**Output styles for Claude Code that make replies shorter and answer-first.**

Three markdown output styles for Claude Code (Attention-kind, Spartan, Rundown) that change how Claude words its replies, not how it codes. It ships as a plugin with a /style switcher and user-invoked skills. The README's benchmark reports about 43% shorter output and equal 97% pass rates on 12 coding tasks.

- **+** Each style is one markdown file; plugin install is a single /plugin command
- **+** Hidden-test benchmark: 97% pass rate both with and without the style
- **+** Reported ~43% shorter output; about 650 input tokens, cached per session
- **+** Style bodies reusable in Codex AGENTS.md or GEMINI.md via a sed strip
- **−** Benchmark covers only 12 coding tasks; README does not claim better answers
- **−** Built for Claude Code; other agents need a manual sed-based install
- **−** AGPL-3.0 license may matter if you redistribute modified versions
- **−** Rundown favors scannability over brevity and uses emoji checklists

<sub>no GPU · Needs Claude Code · Models: Claude Code, Codex, Devin, Antigravity CLI · [Repo](https://github.com/alexgreensh/attention-span) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/attention-span/)</sub>

<a name="skillsgate"></a>
### #&#8288;202 [skillsgate](https://github.com/skillsgate/skillsgate) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Desktop app for browsing and installing AI agent skills across many agents.**

SkillsGate is an Electron desktop app for macOS, Windows and Linux that browses the public skills.sh catalog and installs skills into the config of agents such as Claude Code, Cursor, Codex CLI and Cline. It includes a CodeMirror editor for skill files, SSH access to remote machines, and keeps settings and favorites in a local SQLite database with no account.

- **+** Installs or removes a skill per agent, across 25 listed agents
- **+** Local-first: settings and favorites in SQLite, no account required
- **+** Built-in editor writes skill source straight to disk
- **+** Syncs and browses skills on remote machines over SSH
- **−** macOS build is signed but not notarized; first launch needs Open Anyway
- **−** Terminal UI and npm packages are deprecated and unmaintained
- **−** macOS 0.7.0 and earlier need a manual update to 0.7.2
- **−** Catalog discovery depends on skills.sh

<sub>no GPU · Needs skills.sh, SQLite (better-sqlite3), Node.js 22+ (for development) · [Repo](https://github.com/skillsgate/skillsgate) · [🌐 Site ↗](https://skillsgate.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skillsgate/)</sub>

<a name="haft"></a>
### #&#8288;203 [haft](https://github.com/m0n0x41d/haft) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · custom license · Sep 2026</sub>

**Project memory and decision records for AI coding agents, via MCP and skills.**

Haft is a local Go CLI and MCP server (`haft serve`) that gives coding agents a typed project memory: problems, compared options, human decisions, evidence and stale-claim tracking. It builds on the First Principles Framework, bundling the versioned FPF source and installing skills such as /h-frame, /h-compare and /h-decide into Claude Code, Codex and other hosts. State lives in `.haft/` markdown plus a per-project SQLite database.

- **+** MCP server validates required fields, parity gaps and missing evidence server-side, not only in prompts
- **+** `haft init` wires MCP config, skills and instruction sections for Claude Code and Codex
- **+** Local-first: markdown in `.haft/` and SQLite under `~/.haft/projects/`, no hosted service
- **+** Flags stale evidence and spec drift; binding decisions require the human
- **−** Requires learning FPF concepts; the README itself calls FPF complex
- **−** Only Claude Code and Codex are stable; other hosts are experimental or legacy
- **−** License is NOASSERTION in detected metadata, so terms need checking
- **−** Schema migrations and carrier semantics add operational overhead on upgrade

<sub>no GPU · Needs SQLite, Claude Code, Codex or another MCP host, haft-embed sidecar (optional) · [Repo](https://github.com/m0n0x41d/haft) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/haft/)</sub>

<a name="weave"></a>
### #&#8288;204 [weave](https://github.com/ataraxy-labs/weave) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (7) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Oct 2026</sub>

**Git merge driver that merges functions and classes instead of lines.**

Weave registers as a Git merge driver and parses base, ours and theirs with tree-sitter, then merges at the level of functions, classes and keys. Independent additions to the same file resolve without conflict, and real collisions show the entity and the guard that refused. It also has `weave land` for verified merges by agents, an MCP server, and jj support.

- **+** Entity-level 3-way merge across 38 languages, with line-merge fallback for the rest
- **+** Conflict markers name the entity and the guard that refused (`refused_by:`)
- **+** Reproducible benchmarks: `weave stats --bench` and replay of real merge commits
- **+** Setup per repo, per user or globally; `weave setup --off` reverts
- **−** Replay on real repos showed 86 regressions where Git merged cleanly and weave conflicted
- **−** Human-match rate on wins is 33% on Flask and Go
- **−** Vue, Svelte, ERB and Haskell fall back to Git's line merge
- **−** Source install needs two binaries, `weave` and `weave-driver`, both on PATH

<sub>no GPU · Needs git, Rust toolchain (source build) · [Repo](https://github.com/ataraxy-labs/weave) · [📖 Docs ↗](https://ataraxy-labs.github.io/weave/benchmarks.html) · [🌐 Site ↗](https://ataraxy-labs.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/weave/)</sub>

<a name="golive-skill"></a>
### #&#8288;205 [golive-skill](https://github.com/mikehasa/golive-skill) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Oct 2026</sub>

**Agent skill that plans, approves and deploys an app to your own accounts.**

GoLive is an Agent Skill for Codex and Claude Code that detects what an app needs, builds a plan, and applies it to your own Vercel, Netlify, Supabase, Neon, Porkbun, GoDaddy, Resend and Stripe accounts only after approval. It verifies results, checks drift with `golive status`, and removes what it created with `golive teardown`. It is early alpha (0.1.0-alpha.9).

- **+** Every write needs an approved plan ID and --yes; DNS, destroy and live steps need extra flags
- **+** Teardown removes only resources it can prove it created and lists leftovers as handoffs
- **+** Validation doc separates live-tested journeys from mock-covered ones
- **+** No GoLive account, hosted backend or product telemetry
- **−** Early alpha; built-in adapters cover only Vercel, Netlify, Supabase and Neon for hosting and data
- **−** Install verified only for Codex and Claude Code; other clients unverified
- **−** Credentials stored in a plaintext 0600 file, not a keychain
- **−** Rollback is Netlify-only and not live-validated; other providers get guided steps only

<sub>no GPU · Needs Node.js 20+, Git, Codex or Claude Code, Vercel or Netlify account, Supabase or Neon account · [Repo](https://github.com/mikehasa/golive-skill) · [🌐 Site ↗](https://clawhub.ai/mikehasa/skills/golive) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/golive-skill/)</sub>

<a name="fast-jev-compaction"></a>
### #&#8288;206 [fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.8k · MIT · Sep 2026</sub>

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
### #&#8288;207 [go-modern-guidelines](https://github.com/jetbrains/go-modern-guidelines) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (49) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · Apache-2.0 · Sep 2026</sub>

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

<a name="nvidia-skills"></a>
### #&#8288;208 [skills](https://github.com/nvidia/skills) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Oct 2026</sub>

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

<a name="goldie"></a>
### #&#8288;209 [goldie](https://github.com/software-mansion-labs/goldie) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · custom license · Oct 2026</sub>

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

<a name="agmsg"></a>
### #&#8288;210 [agmsg](https://github.com/fujibee/agmsg) <sub>score [61](../README.md#-how-we-rank "Score 61/100. Adoption: niche (15) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Lets CLI coding agents message each other through a shared SQLite file.**

agmsg is a Bash skill that lets Claude Code, Codex, Gemini CLI, Copilot CLI, Antigravity, OpenCode and other CLI agents send messages to each other through a local WAL-mode SQLite database. It installs as a slash command or `$` command and adds role switching (`actas`), spawning peer agents in tmux or OS terminals, and several delivery modes. It is not MCP and needs no broker; an optional Node-based daemon (agmsgd, beta) exists.

- **+** Runs on bash and sqlite3 only; no MCP server, broker or network required
- **+** Works across Claude Code, Codex, Gemini CLI, Copilot CLI, Antigravity and OpenCode
- **+** Message history persists in SQLite and can be replayed into a new agent
- **+** Installs via npx, curl script, git clone or Claude Code plugin marketplace
- **−** Windows requires Git Bash; no PowerShell implementation, and bare bash may hit WSL
- **−** npm package and plugin can lag main by a few fixes
- **−** agmsgd daemon is beta and needs Node >= 22.13.0
- **−** Codex without monitor or daemon only checks its inbox on its next turn

<sub>no GPU · Needs bash, sqlite3, Node >= 22.13.0 (optional, agmsgd), tmux (optional, spawn) · Models: Claude Code, Codex, Gemini CLI, GitHub Copilot CLI, Antigravity · [Repo](https://github.com/fujibee/agmsg) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agmsg/)</sub>

<a name="app-store-screenshots"></a>
### #&#8288;211 [app-store-screenshots](https://github.com/parthjadhav/app-store-screenshots) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (67) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 7.7k · MIT · Oct 2026</sub>

**Agent skill that scaffolds a Next.js editor for App Store and Play screenshots.**

A skill for coding agents such as Claude Code, Cursor and Codex that generates a Next.js project for designing store screenshots. The editor has a connected canvas, Apple device bezels and an inspector. It exports PNG bundles at the required App Store, Mac App Store and Google Play sizes. Deck state is saved to app-store-screenshots.json, so it can be committed and resumed.

- **+** Exports PNGs at listed sizes for iPhone, iPad, Watch, TV, Mac, Android and feature graphic
- **+** Deck state is one JSON file plus uploaded images, so it is git-trackable
- **+** Ships 18 named visual styles with specs and a headline copy library
- **+** Supports multiple locales and RTL guidance, with export zip organized by locale
- **−** Needs a coding agent to scaffold the project; not a standalone app
- **−** Apple bezels are licensed for mock-ups of Apple-platform apps only
- **−** Output quality depends on the agent and the source captures you supply
- **−** No hosted demo; you must run the Next.js dev server locally

<sub>no GPU · Needs Node.js 20.9+, bun, pnpm, yarn or npm, A skills-compatible coding agent · [Repo](https://github.com/parthjadhav/app-store-screenshots) · [🌐 Site ↗](https://www.parthjadhav.com/products/app-store-screenshots/styles) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/app-store-screenshots/)</sub>

<a name="ip-as-logo-skill"></a>
### #&#8288;212 [ip-as-logo-skill](https://github.com/s1dashu/ip-as-logo-skill) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.2k · MIT · Aug 2026</sub>

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

<a name="transitions-dev"></a>
### #&#8288;213 [transitions.dev](https://github.com/jakubantalik/transitions.dev) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.8k · custom license · Oct 2026</sub>

**Copy-paste CSS transitions with an npm CLI and an agent skill.**

A showcase of reusable CSS transitions such as card resize, modal open/close, menu dropdown, icon swap and error shake. Each card gives a self-contained snippet with CSS custom properties, t-* classes and a prefers-reduced-motion guard. The same set is available through `npx transitions-dev add` and as an agent skill for Cursor, Claude Code and Codex, plus a Refine tool that suggests motion changes on a running app.

- **+** Snippets are plain CSS with custom properties and a reduced-motion guard, no framework required
- **+** Install via `npx transitions-dev add <name>` or `npx skills add Jakubantalik/transitions.dev`
- **+** Skill files are generated from index.html, so they match the showcase site
- **+** Static HTML site runs locally with `python3 -m http.server`
- **−** Custom license for the transitions: redistributing as a competing library is prohibited
- **−** Some transitions (e.g. confetti-burst) are Pro and need browser sign-in
- **−** Refine's LLM mode depends on installing the Cursor CLI
- **−** Fixed set of about eighteen transitions; no release tags

<sub>no GPU · Needs Node.js/npm (for CLI), Cursor CLI (optional, Refine --llm) · port 8765 · [Repo](https://github.com/jakubantalik/transitions.dev) · [▶️ Demo ↗](https://transitions.dev/) · [🌐 Site ↗](https://transitions.dev/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/transitions-dev/)</sub>

<a name="remodex"></a>
### #&#8288;214 [remodex](https://github.com/emanuele-web04/remodex) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Sep 2026</sub>

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
### #&#8288;215 [my-claude-code-setup](https://github.com/centminmod/my-claude-code-setup) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

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

<a name="claude-code-skills"></a>
### #&#8288;216 [claude-code-skills](https://github.com/daymade/claude-code-skills) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Claude Code plugin marketplace with a skill-creator fork and bundled skill suites.**

A Claude Code plugin marketplace (named daymade-skills) that ships a fork of Anthropic's skill-creator plus suites for document conversion, macOS/iOS, Codex, Claude Code operations and financial data. Standalone skills cover GitHub operations, Terraform, Cloudflare diagnostics and YouTube downloading. Install with /plugin marketplace add daymade/claude-code-skills or the claude plugin CLI.

- **+** skill-creator adds a security_scan.py gate with gitleaks before packaging
- **+** Suites install under one namespace, e.g. daymade-docs:doc-to-markdown
- **+** Standard Claude Code plugin install; suites also installable via the Codex plugin marketplace
- **+** Optional routing hook resolves a clash when Anthropic's skill-creator is also installed
- **−** Suite skills are bundle-only; a single member cannot be installed alone
- **−** Several skills target niche setups (Gangtise, Tencent IMA, Douban, WeChat archives)
- **−** Comparison against Anthropic's skill-creator is the author's own table
- **−** Requires Claude Code 2.0.13+ or Codex; no use outside those tools

<sub>no GPU · Needs Claude Code 2.0.13+, gitleaks (for security_scan.py) · [Repo](https://github.com/daymade/claude-code-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-skills/)</sub>

<a name="pi-subagents"></a>
### #&#8288;217 [pi-subagents](https://github.com/tintinweb/pi-subagents) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (8) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Claude Code-style sub-agents and scripted workflows for the pi coding agent.**

An extension for the pi coding agent that spawns sub-agents in isolated sessions, each with its own tools, system prompt, model and thinking level. Agents run in the background by default and can be steered, resumed, scheduled, or isolated in git worktrees. A SubagentWorkflow tool runs deterministic JavaScript scripts (agent, parallel, pipeline), including scripts written for Claude Code's Workflow tool.

- **+** Background agents with queuing, default concurrency limit of 10, and completion notifications
- **+** Custom agent types in markdown with YAML frontmatter, tool denylist and skill preloading
- **+** Git worktree isolation auto-commits each agent's changes to a branch
- **+** Workflow scripts run in a node:vm sandbox and match Claude Code's Workflow tool
- **−** Only works inside pi, which must be version 1.1.0 or newer
- **−** Other hosts such as DeepSeek Harness rely on untested third-party adapters
- **−** Foreground-to-background handoff is one-way and not offered for queued or nested agents
- **−** Headless pi -p does not wait for scheduled subagents

<sub>no GPU · Needs pi >= 1.1.0 · Models: Any model configured in pi, selectable by fuzzy name such as haiku or sonnet · [Repo](https://github.com/tintinweb/pi-subagents) · [📖 Docs ↗](https://github.com/tintinweb/pi-subagents/blob/master/docs/workflows.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/pi-subagents/)</sub>

<a name="ai-setup"></a>
### #&#8288;218 [ai-setup](https://github.com/caliber-ai-org/ai-setup) <sub>score [60](../README.md#-how-we-rank "Score 60/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Sep 2026</sub>

**CLI that generates and syncs context files across coding agents.**

Caliber is a Node CLI that writes and maintains CLAUDE.md, Cursor rules, AGENTS.md and Copilot instructions for a repo. A pre-commit hook refreshes them from your diff, and `caliber sync` mirrors skills, rules, plugins and MCP config between agents. It also ships a Claude Code plugin and a CLI command for Jev compaction, which replaces `/compact` with per-tool-call scoring.

- **+** `caliber score` audits context files against the repo without an LLM
- **+** Sync is deterministic and never overwrites files you edited by hand
- **+** Every write is shown as a diff and backed up to .caliber/backups/
- **+** Covers Claude Code, Cursor, Codex, OpenCode and GitHub Copilot
- **−** Jev compaction needs a Vercel AI Gateway or TypeSafe API key
- **−** Anonymous usage analytics are on by default; opt out via env var
- **−** Setup and refresh need an agent seat or your own LLM API key
- **−** On agents lacking a feature, sync degrades, e.g. skills become Copilot instruction files

<sub>no GPU · Needs Node 20+, Claude Code or Cursor seat, or Anthropic/OpenAI/MiniMax/Vertex key, Vercel AI Gateway or TypeSafe key (Jev compaction only) · Models: Anthropic, OpenAI, MiniMax, Vertex · [Repo](https://github.com/caliber-ai-org/ai-setup) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ai-setup/)</sub>

<a name="design-md"></a>
### #&#8288;219 [design.md](https://github.com/google-labs-code/design.md) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: weak (10) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · Apache-2.0 · Oct 2026</sub>

**Spec and CLI for describing a design system to coding agents.**

DESIGN.md is a file format that pairs YAML design tokens (colors, typography, spacing, rounded corners, components) with markdown rationale so coding agents get exact values and context. The TypeScript CLI lints files for broken token references and WCAG contrast, diffs two versions, and exports tokens to Tailwind v3/v4 and W3C DTCG. The format is at version alpha.

- **+** Lint output is structured JSON with exit codes, so it can gate CI
- **+** Eleven lint rules, including broken refs and WCAG AA 4.5:1 contrast
- **+** Exports tokens to Tailwind v3 JSON, Tailwind v4 CSS and W3C DTCG
- **+** Also usable as a library via the @google/design.md/linter import
- **−** Format is alpha; README warns the spec and schema will change
- **−** Component tokens limited to eight properties such as backgroundColor and padding
- **−** Strict section order is required; duplicate sections or keys reject the file
- **−** Windows needs the designmd alias because of the .md bin name

<sub>no GPU · Needs Node.js, npm · safety checks passed 9 of 10 · [Repo](https://github.com/google-labs-code/design.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/design-md/)</sub>

<a name="adhd"></a>
### #&#8288;220 [adhd](https://github.com/uditakhourii/adhd) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (53) · Freshness: active (100) · Maintenance: patchy (42) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.5k · MIT · Oct 2026</sub>

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

<a name="playwright-skill"></a>
### #&#8288;221 [playwright-skill](https://github.com/lackeyjb/playwright-skill) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Aug 2026</sub>

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

<a name="designer-skills"></a>
### #&#8288;222 [designer-skills](https://github.com/owl-listener/designer-skills) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (40) · Freshness: active (100) · Maintenance: fair (57) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Sep 2026</sub>

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

<a name="terraform-skill"></a>
### #&#8288;223 [terraform-skill](https://github.com/antonbabenko/terraform-skill) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (30) · Freshness: active (100) · Maintenance: fair (54) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · custom license · Oct 2026</sub>

**Terraform and OpenTofu guidance skill for AI coding agents.**

An Agent Skills package that gives coding agents guidance on Terraform and OpenTofu: module structure, native tests vs Terratest, remote state backends, CI/CD workflows, and Trivy/Checkov scanning. Examples default to AWS, with Azure and GCP covered by the same guidance. It installs into Claude Code, Cursor, Copilot, Gemini CLI, OpenCode, Codex and Kiro, and can optionally use terraform-ls.

- **+** Installs on many agent hosts: Claude Code, Cursor, Copilot, Gemini CLI, Codex, Kiro, OpenCode
- **+** Covers testing, modules, state, CI/CD and security scanning in one skill
- **+** Decision matrices and DO vs DON'T patterns, with version notes (use_lockfile 1.10+, write_only 1.11+)
- **+** Works without terraform-ls or the MCP server; both are optional
- **−** Guidance only; it does not run or validate Terraform itself
- **−** AWS is the default in examples; Azure and GCP are mapped on request
- **−** Two marketplace names clash, so install must go through antonbabenko/agent-plugins
- **−** Install steps differ per host, and some are manual git clones

<sub>no GPU · Needs Terraform 1.0+ or OpenTofu 1.6+, AI agent with skill support, terraform-ls (optional), Terraform MCP server (optional) · [Repo](https://github.com/antonbabenko/terraform-skill) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terraform-skill/)</sub>

<a name="chops"></a>
### #&#8288;224 [chops](https://github.com/shpigford/chops) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · custom license · Aug 2026</sub>

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

<a name="codex-astra-luna-orchestrator"></a>
### #&#8288;225 [codex-astra-luna-orchestrator](https://github.com/donvito/codex-astra-luna-orchestrator) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · Apache-2.0 · Oct 2026</sub>

**Codex profiles that set up an orchestrator, Luna subagents and a reviewer.**

Installer scripts (setup.sh, setup.ps1) copy a chosen Codex profile into a target repository as .codex/, .agents/ and AGENTS.md. Each profile defines a root orchestrator (Astra, Sol or Luna), explorer, worker, tester and researcher subagents on GPT-6 Luna, and a separate reviewer. Six profiles vary the model, reasoning level and concurrent subagent count (2 or 4).

- **+** Six ready-to-copy profiles with pinned models and reasoning levels per role
- **+** Installer preserves existing AGENTS.md and asks before overwriting component files
- **+** Manual and global (~/.codex) setup paths are documented
- **+** Includes tests and a token_usage.py script for measuring usage
- **−** Requires Codex CLI and access to the GPT-6 model family
- **−** Project-scoped config loads only for trusted projects
- **−** Skill is named astra-orchestrator even in Sol and Luna profiles
- **−** Global setup needs a manual merge into ~/.codex/config.toml

<sub>no GPU · Needs Codex CLI, Python · Models: GPT-6 Astra, GPT-6.1 Sol, GPT-6 Luna · [Repo](https://github.com/donvito/codex-astra-luna-orchestrator) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-astra-luna-orchestrator/)</sub>

<a name="azure-skills"></a>
### #&#8288;226 [azure-skills](https://github.com/microsoft/azure-skills) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: niche (16) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · Oct 2026</sub>

**Azure skills and MCP servers for coding agents, installed as one plugin.**

Plugin that gives coding agents Azure workflow skills (prepare, validate, deploy, diagnostics, cost, RBAC) plus the Azure MCP Server and Foundry MCP for acting on live resources. The README lists 200+ tools across 40+ Azure services. It installs into GitHub Copilot, Claude Code, Cursor, Codex CLI, Gemini CLI, VS Code and IntelliJ.

- **+** Bundles skills and MCP config so guidance and tool execution stay aligned
- **+** Installs across Copilot CLI, Claude Code, Cursor, Codex, Gemini CLI, VS Code, IntelliJ
- **+** Covers deploy, diagnostics, cost, quotas, RBAC and Foundry model workflows
- **+** Supports sovereign clouds (China, US Government) via a --cloud argument
- **−** Azure only; no use outside Azure and Foundry
- **−** Needs Node.js 18+, Azure CLI login, and azd for deployment workflows
- **−** Repo is synced from GitHub-Copilot-for-Azure; contributions go upstream
- **−** Azure MCP telemetry is collected by default and must be disabled via env var

<sub>no GPU · Needs Node.js 18+, Azure CLI, Azure Developer CLI, Azure subscription, Git · [Repo](https://github.com/microsoft/azure-skills) · [📖 Docs ↗](https://learn.microsoft.com/azure/developer/azure-mcp-server/) · [🌐 Site ↗](https://microsoft.github.io/azure-skills/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/azure-skills/)</sub>

<a name="fireworks-tech-graph"></a>
### #&#8288;227 [fireworks-tech-graph](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 12k · MIT · Oct 2026</sub>

**Agent skill that generates SVG, PNG, GIF and HTML diagrams from prompts.**

An Agent Skill for Codex and Claude Code that generates technical diagrams from English or Chinese descriptions. A Python CLI renders SVG with orthogonal routing and geometry checks, then exports PNG, an animated GIF, or one offline interactive HTML file. It ships 12 visual styles and 14 diagram types, including UML and AI/agent patterns such as RAG and multi-agent.

- **+** Same skill installs into Codex and Claude Code via skills CLI or git clone
- **+** Validates XML, markers, edge crossings and label clearance before export
- **+** Outputs SVG, PNG up to 4x, SVG-to-GIF motion and offline HTML with pan/zoom
- **+** 12 styles and 14 diagram types, including all UML types and AI/agent patterns
- **−** Needs an agent runtime (Codex or Claude Code); not a standalone diagram app
- **−** PNG and GIF export rely on optional dependencies; Puppeteer path needs Node.js 22.12+
- **−** GIF motion only works on generated SVGs matching one of twelve approved contracts
- **−** Visual review is skipped when the runtime cannot read images

<sub>no GPU · Needs Python 3.9+, Codex or Claude Code, Node.js 22.12+ (optional, Puppeteer PNG export) · Models: Codex, Claude Code · safety checks passed 10 of 10 · [Repo](https://github.com/yizhiyanhua-ai/fireworks-tech-graph) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fireworks-tech-graph/)</sub>

<a name="stitch-skills"></a>
### #&#8288;228 [stitch-skills](https://github.com/google-labs-code/stitch-skills) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: weak (25) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.6k · Apache-2.0 · Aug 2026</sub>

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

<a name="cloudflare-skills"></a>
### #&#8288;229 [skills](https://github.com/cloudflare/skills) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · Apache-2.0 · Oct 2026</sub>

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

<a name="delegate-skills"></a>
### #&#8288;230 [delegate-skills](https://github.com/amelnagdy/delegate-skills) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (31) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.5k · MIT · Oct 2026</sub>

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

<a name="cc-thinking-skills"></a>
### #&#8288;231 [cc-thinking-skills](https://github.com/tjboudreaux/cc-thinking-skills) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: fair (51) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Aug 2026</sub>

**28 Agent Skills that give coding agents structured reasoning procedures.**

A catalog of 28 Agent Skills, each a SKILL.md procedure for a reasoning method such as pre-mortem, theory of constraints, scientific-method debugging, or reversibility checks. A router skill picks none, one, or up to three skills for a problem. Installs through the skills CLI, as a Claude Code plugin, or by copying directories into .agents/skills or .claude/skills.

- **+** Router skill can return NONE, one skill, or up to three complementary skills
- **+** Three install paths: npx skills CLI, Claude Code plugin, or plain directory copy
- **+** Works with Claude Code, GitHub Copilot, Codex, Cursor and other Agent Skills tools
- **+** Includes validation script and structural, routing and outcome evals in the repo
- **−** Own audit reports only a provisional +4.0 point gain, below its +5 point margin
- **−** All 28 skills are manual-only; none trigger automatically
- **−** Routing eval requires the authenticated droid CLI
- **−** Skills are prompt procedures, not tooling; benefit depends on the model following them

<sub>no GPU · Needs Node.js, npx skills CLI · [Repo](https://github.com/tjboudreaux/cc-thinking-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-thinking-skills/)</sub>

<a name="codex-plugin-cc"></a>
### #&#8288;232 [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: widely used (89) · Freshness: active (94) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · Apache-2.0 · Jul 2026</sub>

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

<a name="scroll-craft"></a>
### #&#8288;233 [scroll-craft](https://github.com/nateherkai/scroll-craft) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.1k · MIT · Sep 2026</sub>

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

<a name="vibe-wise"></a>
### #&#8288;234 [vibe-wise](https://github.com/nykooi1/vibe-wise) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (50) · Freshness: active (100) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · Oct 2026</sub>

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

<a name="agent-toolkit-for-aws"></a>
### #&#8288;235 [agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (43) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.3k · Apache-2.0 · Oct 2026</sub>

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

<a name="web-quality-skills"></a>
### #&#8288;236 [web-quality-skills](https://github.com/addyosmani/web-quality-skills) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (38) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · MIT · Aug 2026</sub>

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

<a name="babysitter"></a>
### #&#8288;237 [babysitter](https://github.com/a5c-ai/babysitter) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (22) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Aug 2026</sub>

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

<a name="builderio-skills"></a>
### #&#8288;238 [skills](https://github.com/builderio/skills) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.6k · MIT · Oct 2026</sub>

**Installable agent skills for visual plans, PR recaps and review automation.**

A collection of agent skills installed with `npx @agent-native/skills@latest add` into Claude Code, Codex, Cursor, Copilot and similar agents. It includes visual-plan and visual-recap (MDX plans and diff recaps, with an optional PR GitHub Action), webmcp, visual-edit, agent-watchdog and usage-limit skills, plus an experimental Factory set that turns feedback and errors into policy-gated PRs. Also published as a Claude Code and Cowork plugin marketplace.

- **+** Single npx installer with a picker, user or project scope, and a per-skill --skill flag
- **+** Works across Claude Code, Codex, Cursor, OpenCode and Copilot via the shared .agents path
- **+** Factory config separates fix, reply, review, approve and merge policies in YAML
- **+** Local-files mode serves visual plans over localhost instead of uploading them
- **−** Visual plans and recaps are viewed in the Agent-Native plans app, hosted by default
- **−** Factory skills are experimental and need Slack, Sentry or GitHub connections you set up
- **−** /rewind needs macOS and the separate Clips Desktop app
- **−** Skills are prompt instructions, so results depend on the host agent and model

<sub>no GPU · Needs Node.js (npx), Agent-Native plans app, Clips Desktop (rewind, macOS), GitHub Actions (optional) · Models: Claude Code, Codex, Cursor, OpenCode, GitHub Copilot · [Repo](https://github.com/builderio/skills) · [🌐 Site ↗](https://www.agent-native.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/builderio-skills/)</sub>

<a name="qiushi-skill"></a>
### #&#8288;239 [qiushi-skill](https://github.com/hughyau/qiushi-skill) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (49) · Freshness: active (100) · Maintenance: patchy (37) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

**Agent skill set applying Mao-era methodology to AI problem-solving.**

A set of nine methodology skills plus a core "seek truth from facts" kernel for coding agents, drawn from Mao Zedong's writings (contradiction analysis, investigation first, protracted strategy and others). A hook injects a roughly 50-line kernel at session start, and the other skills load only when relevant. Installs with `npx qiushi-skill` into Claude Code, Cursor, Codex, OpenCode and other hosts, or through the Claude Code marketplace.

- **+** One npx command installs to Claude Code, Cursor, Codex, OpenCode, OpenClaw, Hermes and nanobot
- **+** Only a ~50-line kernel stays resident; method skills load on demand
- **+** Includes slash commands, two subagents (investigator, self-critic) and a validate script
- **+** Each skill has an original-texts.md with source quotations
- **−** Main README is in Chinese; the English version is a separate file
- **−** No benchmarks or measured effect on agent output quality in the README
- **−** Content is built on a specific political text corpus, which may not suit every team
- **−** No tagged releases

<sub>no GPU · Needs Node.js (optional, for npx installer) · [Repo](https://github.com/hughyau/qiushi-skill) · [📖 Docs ↗](https://github.com/HughYau/qiushi-skill/blob/main/docs/platforms.md) · [🌐 Site ↗](https://hughyau.com/qiushi-skill/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/qiushi-skill/)</sub>

<a name="anything2explainer"></a>
### #&#8288;240 [anything2explainer](https://github.com/vincentwei1021/anything2explainer) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (53) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · custom license · Sep 2026</sub>

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

<a name="mcollina-skills"></a>
### #&#8288;241 [skills](https://github.com/mcollina/skills) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (52) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Oct 2026</sub>

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

<a name="hivemind"></a>
### #&#8288;242 [hivemind](https://github.com/activeloopai/hivemind) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Oct 2026</sub>

**Shared team memory and auto-generated skills for coding agents.**

Hivemind installs hooks or plugins into Claude Code, OpenClaw, Codex, Cursor, Hermes, pi and Claude Cowork (alpha). It captures prompts, tool calls and responses as traces in a Deeplake workspace, and mines them into SKILL.md files shared across the team. Agents recall past work through hybrid lexical and semantic search over those traces.

- **+** One installer wires hooks for seven agents; `hivemind status` shows what is connected
- **+** Mines captured traces into SKILL.md files scoped to a workspace
- **+** Capture can be disabled by env var or a per-directory `.hivemind` file
- **+** README reports LoCoMo results: 25% lower cost, 31% fewer turns versus no memory
- **−** Requires a Deeplake account and cloud API; no fully local mode is described
- **−** All workspace users can read every captured prompt and tool output
- **−** Claude Cowork capture is alpha and covers Local Agent Mode sessions only
- **−** Background summary and skill-mining runs invoke `claude -p`, adding model cost

<sub>no GPU · Needs Node.js 22+, Deeplake account (api.deeplake.ai), Claude Code CLI (for summary worker) · Models: Claude Code, OpenClaw, Codex, Cursor, Hermes Agent · [Repo](https://github.com/activeloopai/hivemind) · [🌐 Site ↗](https://deeplake.ai) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hivemind/)</sub>

<a name="fluent-korean"></a>
### #&#8288;243 [fluent-korean](https://github.com/snflkd/fluent-korean) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Aug 2026</sub>

**Claude Code output style that makes Claude write clear, grammatical Korean.**

A Claude Code plugin with two output styles that instruct Claude to keep Korean particles, endings and common vocabulary instead of terse, telegraphic text. One variant keeps Claude Code's coding instructions and the other removes them. The guideline text can also be pasted into other AI tools as a plain writing instruction.

- **+** Two variants: fluent-korean keeps coding instructions, fluent-korean-not-coding drops them
- **+** Installs with two /plugin commands in Claude Code
- **+** Optional add-on blocks for honorifics, beginner tone, or forcing Korean reasoning
- **+** Style files are plain markdown, reusable in CLAUDE.md or other AIs
- **−** README says results may fall short in long sessions or with many instructions
- **−** Uses somewhat more tokens because omitted sentence parts are restored
- **−** Subagent compliance is not guaranteed and must be checked by the user
- **−** README is mostly Korean, with only a short English summary

<sub>no GPU · Needs Claude Code · Models: Claude · [Repo](https://github.com/snflkd/fluent-korean) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/fluent-korean/)</sub>

<a name="autocontext"></a>
### #&#8288;244 [autocontext](https://github.com/greyhaven-ai/autocontext) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (6) · Freshness: active (100) · Maintenance: fair (56) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · Apache-2.0 · Oct 2026</sub>

**Harness that iterates agent tasks against evaluation and keeps lessons as playbooks.**

autocontext runs a task from a plain-language goal through repeated generations scored by evaluation. It keeps useful lessons, discards dead ends, and writes traces, reports, playbooks and datasets to disk for later runs. It ships Python and TypeScript CLIs (autoctx), an MCP server, a Pi extension, and optional local-model distillation.

- **+** Filesystem-first run output (trace.jsonl, playbook.md, score.json) that can be diffed and replayed
- **+** Works with Anthropic, OpenAI-compatible, OpenRouter, Claude CLI, Codex, Pi, and vLLM or Ollama
- **+** Context changes are stored as candidates and served only after matched trials confirm them
- **+** Exposes its tools to Claude Code or Cursor via autoctx serve mcp
- **−** Large surface area: many commands, scenario families and opt-in features to learn
- **−** Python and TypeScript packages differ; some TS features lack Python parity
- **−** No Docker image or compose file; install through uv or bun
- **−** Reuse studies are described as infrastructure evidence only, not production promotion

<sub>GPU optional · Needs uv or bun, Node.js 22.19+ (npm CLI), LLM provider or local agent such as Pi · Models: Anthropic, OpenAI-compatible, OpenRouter, Claude CLI, Codex · [Repo](https://github.com/greyhaven-ai/autocontext) · [📖 Docs ↗](https://autocontext.ai/docs/get-started/quickstart) · [🌐 Site ↗](https://autocontext.ai/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/autocontext/)</sub>

<a name="frontend-slides"></a>
### #&#8288;245 [frontend-slides](https://github.com/zarazhangrui/frontend-slides) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: widely used (88) · Freshness: active (91) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Jun 2026</sub>

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

<a name="cc-wf-studio"></a>
### #&#8288;246 [cc-wf-studio](https://github.com/breaking-brake/cc-wf-studio) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.4k · custom license · Aug 2026</sub>

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

<a name="microsoft-skills"></a>
### #&#8288;247 [skills](https://github.com/microsoft/skills) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (40) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · MIT · Oct 2026</sub>

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

<a name="oil-motion"></a>
### #&#8288;248 [oil-motion](https://github.com/oil-oil/oil-motion) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (33) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · MIT · Oct 2026</sub>

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

<a name="claude-video-vision"></a>
### #&#8288;249 [claude-video-vision](https://github.com/jordanrendric/claude-video-vision) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (73) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Claude Code plugin that lets Claude watch videos via ffmpeg frames and transcripts.**

An MCP server and Claude Code plugin that extracts video frames with ffmpeg and sends them to Claude as base64 images with timestamps, alongside an audio transcription. Audio comes from the Gemini API, local Whisper (whisper.cpp or Python openai-whisper), or the OpenAI Whisper API. It also accepts YouTube URLs via yt-dlp, using manual or automatic captions before falling back to the audio backend.

- **+** Three audio backends, including fully offline whisper.cpp with automatic model download
- **+** YouTube URLs use manual or auto captions first, with transcription_source labeled
- **+** Six MCP tools, including video_analyze and video_detail for drilling into specific moments
- **+** Frame fps, time range, resolution and format (jpeg, png, webp) are adjustable
- **−** Requires Node.js 24+ and ffmpeg installed locally
- **−** YouTube support needs yt-dlp installed separately
- **−** Only a perception layer: no interpretation, and frames count against Claude's context
- **−** Windows users may need a global npm install workaround if npx fails

<sub>GPU optional · Needs Node.js 24+, ffmpeg, yt-dlp (optional, YouTube), whisper.cpp or openai-whisper (local backend), Gemini API key or OpenAI API key (cloud backends) · Models: Gemini API, whisper.cpp, openai-whisper, OpenAI Whisper API · [Repo](https://github.com/jordanrendric/claude-video-vision) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-video-vision/)</sub>

<a name="scroll-world"></a>
### #&#8288;250 [scroll-world](https://github.com/oso95/scroll-world) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · MIT · Jul 2026</sub>

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

<sub>no GPU · Needs Monid CLI, Higgsfield CLI, ffmpeg, ffprobe, Python 3, Pillow, Codex CLI (optional) · Models: Seedance 2.0, Kling 3.0, GPT Image 2 · safety checks passed 9 of 10 · [Repo](https://github.com/oso95/scroll-world) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/scroll-world/)</sub>

<a name="claude-code-workflows"></a>
### #&#8288;251 [claude-code-workflows](https://github.com/oneredoak/claude-code-workflows) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (50) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Oct 2026</sub>

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
### #&#8288;252 [effective-html](https://github.com/plannotator/effective-html) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: known (48) · Freshness: active (100) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · MIT · Oct 2026</sub>

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

<a name="headcount"></a>
### #&#8288;253 [headcount](https://github.com/cbrock84/headcount) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.1k · MIT · Oct 2026</sub>

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

<a name="huashu-motion"></a>
### #&#8288;254 [huashu-motion](https://github.com/alchaincyf/huashu-motion) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (21) · Freshness: active (100) · Maintenance: fair (60) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Oct 2026</sub>

**Agent skill that writes, scores and renders product launch videos as HTML.**

An Agent Skills package plus an `om` CLI that lets Claude Code, Codex and similar agents produce short launch films. Each film is a single index.html (GSAP, Canvas, Three.js, SVG) rendered frame by frame through local Chrome and FFmpeg, with a score written in ABC notation. A browser editor lets you click a frame and leave a comment, and the agent edits only that spot.

- **+** Output is one plain HTML file; no video-generation model, each frame depends only on code and time
- **+** Click-to-comment editor sends timestamp, scene and source location to the agent
- **+** Music and 23 sound effects are generated locally with no paid API
- **+** Exports MP4, transparent MOV, WebM, GIF or a share page; 12 starter templates
- **−** Only tested on macOS, per the README
- **−** Needs Node 22+, Chrome and FFmpeg; voiceover adds uv, Python 3.12 and whisper-cli
- **−** Quality depends on the model; author mainly uses Opus 5.5
- **−** Cannot generate live-action footage or hear the audio; README and docs are mainly in Chinese

<sub>no GPU · Needs Node 22+, Chrome/Chromium/Edge, FFmpeg, uv and Python 3.12 (optional, Kokoro voice), whisper-cli (optional) · Models: Claude Code, Codex, WorkBuddy, Grok Bot, Muse · [Repo](https://github.com/alchaincyf/huashu-motion) · [🌐 Site ↗](https://bookai.top) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/huashu-motion/)</sub>

<a name="swift-ios-skills"></a>
### #&#8288;255 [swift-ios-skills](https://github.com/dpearson2699/swift-ios-skills) <sub>score [54](../README.md#-how-we-rank "Score 54/100. Adoption: niche (4) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.2k · custom license · Jul 2026</sub>

**86 agent skills for iOS 26, Swift 6.3 and SwiftUI development.**

A set of 86 self-contained Agent Skills covering SwiftUI, Swift concurrency, SwiftData, StoreKit 2, Foundation Models, HealthKit and other Apple frameworks, written against iOS 26+ APIs. Install through the skills CLI, a Claude Code plugin marketplace with themed bundles, Codex's skill installer, or by uploading zipped skills to Claude or ChatGPT. Each skill stands alone, so you can install only the ones you need.

- **+** 86 skills, each self-contained with no cross-dependencies, so partial installs work
- **+** Targets iOS 26+ APIs such as Liquid Glass and Foundation Models, avoiding deprecated patterns
- **+** Several install paths: skills CLI, Claude Code marketplace, Codex installer, manual zip upload
- **+** Themed Claude Code bundles limit how many skills load into the context window
- **−** License is PolyForm Perimeter 1.0.0, which is not an OSI open-source license
- **−** Installing all 86 skills can load a lot into the context window
- **−** Apple platforms only; no Android or cross-platform guidance
- **−** README gives no evaluation of how much the skills improve agent output

<sub>no GPU · Needs Node.js (for the npx skills CLI), A compatible coding agent such as Claude Code, Codex, Cursor or Copilot · Models: Claude Code, OpenAI Codex, Cursor, GitHub Copilot · [Repo](https://github.com/dpearson2699/swift-ios-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/swift-ios-skills/)</sub>

<a name="ralph"></a>
### #&#8288;256 [ralph](https://github.com/snarktank/ralph) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: widely used (83) · Freshness: slowing (35) · Maintenance: patchy (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 22k · MIT · Feb 2026</sub>

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

<a name="improve"></a>
### #&#8288;257 [improve](https://github.com/shadcn/improve) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · MIT · Sep 2026</sub>

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

<a name="ccpm"></a>
### #&#8288;258 [ccpm](https://github.com/automazeio/ccpm) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: popular (69) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 8.4k · MIT · Oct 2026</sub>

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

<a name="nocturne-memory"></a>
### #&#8288;259 [nocturne_memory](https://github.com/dataojitori/nocturne_memory) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (11) · Freshness: active (100) · Maintenance: fair (66) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Sep 2026</sub>

**Long-term memory MCP server with URI-addressed memories and a review dashboard.**

Python MCP server (stdio, SSE, Streamable HTTP) that stores agent memories in SQLite or PostgreSQL as a URI-routed graph such as core://agent/identity. The agent gets 7 tools to create, update, alias, search and trigger-link memories, and a React dashboard lets the owner browse, diff and roll back every change. A system://boot entry loads configured core memories at session start.

- **+** Works with any MCP client over stdio, SSE or Streamable HTTP, not tied to one LLM
- **+** Every AI write creates a snapshot; dashboard offers diff, accept and rollback
- **+** Runs on SQLite locally or PostgreSQL; namespaces isolate multiple agents in one database
- **+** Public read-only demo server and dashboard available without installing
- **−** Search is full-text keyword only, not semantic
- **−** Needs Python 3.10+ and Node.js; frontend builds on first start
- **−** README is mostly Chinese and leans on persona and roleplay examples
- **−** Docker setup starts from an empty PostgreSQL with no example data

<sub>no GPU · Compose · Needs Python 3.10+, Node.js, SQLite or PostgreSQL, Docker Compose (optional) · Models: Any MCP client (Claude Code, Cursor, Gemini CLI, OpenAI Codex, Cline, etc.) · port 8233 · [Repo](https://github.com/dataojitori/nocturne_memory) · [▶️ Demo ↗](https://misaligned.top/memory) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nocturne-memory/)</sub>

<a name="dzhng-skills"></a>
### #&#8288;260 [skills](https://github.com/dzhng/skills) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (9) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Library of agent skills for spec-driven, verifiable autonomous coding loops.**

A collection of SKILL.md folders for coding agents, covering exploring unknowns, writing specs, implementing them in slices, reviewing, and visual checks. Install with `npx skills add dzhng/skills` or copy a skill folder into `.claude/skills/`. It targets Claude Code, Codex, opencode, Cursor and other harnesses that support skills.

- **+** Skills are standalone; each can be installed or copied alone via `--list` or `--only`
- **+** Covers the whole loop: explore-unknowns, write-spec, implement-spec, review, close-spec
- **+** Visual review skills compare screenshots against a baseline, with a diff script included
- **+** Works with any harness that reads skills; MIT licensed
- **−** Author's personal library; workflow assumes his spec and choices.md conventions
- **−** Full loop relies on a harness `/goal` mode, as in Claude Code or Codex
- **−** Long unattended runs of days; the only evidence is one 3d 18m run
- **−** Some skills are niche, such as WebGPU renderer rules and Xiaohei illustrations

<sub>no GPU · Needs Node.js/npx, A skills-capable agent harness (Claude Code, Codex, opencode, Cursor) · [Repo](https://github.com/dzhng/skills) · [🌐 Site ↗](https://skills.sh/dzhng/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dzhng-skills/)</sub>

<a name="replica-skill"></a>
### #&#8288;261 [replica-skill](https://github.com/jakeschincariol/replica-skill) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: popular (61) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 6.1k · MIT · Oct 2026</sub>

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

<a name="tdd-guard"></a>
### #&#8288;262 [tdd-guard](https://github.com/nizos/tdd-guard) <sub>score [52](../README.md#-how-we-rank "Score 52/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: patchy (31) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

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

<a name="claude-code-infrastructure-showcase"></a>
### #&#8288;263 [claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (72) · Freshness: active (93) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 10k · MIT · Jul 2026</sub>

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

<sub>no GPU · Needs Node.js 18+, npm, jq (optional Stop hooks), bash (macOS, Linux or WSL2), Gemini/OpenAI/Anthropic API key or Ollama (optional AI mode) · Models: Gemini gemini-3-flash-preview, OpenAI gpt-4o-mini, Anthropic claude-haiku-4-5, Ollama llama3.2 · safety checks passed 8 of 9 · [Repo](https://github.com/diet103/claude-code-infrastructure-showcase) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-infrastructure-showcase/)</sub>

<a name="buildwithclaude"></a>
### #&#8288;264 [buildwithclaude](https://github.com/davepoon/buildwithclaude) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: known (46) · Freshness: active (84) · Maintenance: patchy (40) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.7k · MIT · Oct 2026</sub>

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

<a name="gptcommit"></a>
### #&#8288;265 [gptcommit](https://github.com/zurawiki/gptcommit) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: patchy (41) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Sep 2026</sub>

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

<a name="holo-card-studio"></a>
### #&#8288;266 [holo-card-studio](https://github.com/everettfish/holo-card-studio) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · custom license · Sep 2026</sub>

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

<a name="gsap-skills"></a>
### #&#8288;267 [gsap-skills](https://github.com/greensock/gsap-skills) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (79) · Freshness: recent (64) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Apr 2026</sub>

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

<a name="openagentscontrol"></a>
### #&#8288;268 [openagentscontrol](https://github.com/darrenhinde/openagentscontrol) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: popular (56) · Freshness: active (92) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.0k · MIT · Oct 2026</sub>

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

<a name="conductor"></a>
### #&#8288;269 [conductor](https://github.com/gemini-cli-extensions/conductor) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (48) · Freshness: active (96) · Maintenance: weak (25) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.8k · Apache-2.0 · Sep 2026</sub>

**Spec-driven development plugin for Antigravity and Claude Code agents.**

Conductor is a plugin that makes a coding agent follow a Context, Spec and Plan, Implement protocol. It writes product, tech-stack and workflow files plus per-track spec.md and plan.md into a conductor/ directory in the repo. Slash commands cover setup, new-track, implement, status, revert and review.

- **+** Keeps project context as versioned markdown in the repo (product.md, tech-stack.md, workflow.md)
- **+** Git-aware revert works on tracks, phases and tasks instead of commit hashes
- **+** Plan is reviewed and approved before the agent writes code
- **+** Installs as a plugin on Antigravity and Claude Code; handles new and existing projects
- **−** README warns the spec-driven approach increases token consumption, especially on larger projects
- **−** Supports only Antigravity and Claude Code; other agents are not documented
- **−** Protocol is defined in SKILL.md prompts, so adherence depends on the host agent
- **−** Interactive GUI dialogs only in hosts that support them; plain terminals get text menus

<sub>no GPU · Needs Antigravity or Claude Code, git · [Repo](https://github.com/gemini-cli-extensions/conductor) · [📖 Docs ↗](https://antigravity.google/docs/plugins) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/conductor/)</sub>

<a name="appllama-skills"></a>
### #&#8288;270 [appllama-skills](https://github.com/appllama/appllama-skills) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (45) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Sep 2026</sub>

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

<a name="agents-best-practices"></a>
### #&#8288;271 [agents-best-practices](https://github.com/denissergeevitch/agents-best-practices) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: niche (29) · Freshness: active (100) · Maintenance: patchy (39) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.4k · MIT · Oct 2026</sub>

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

<a name="kotlin-footguns"></a>
### #&#8288;272 [kotlin-footguns](https://github.com/maxrave-dev/kotlin-footguns) <sub>score [49](../README.md#-how-we-rank "Score 49/100. Adoption: niche (18) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · GPL-3.0 · Oct 2026</sub>

**Agent skills documenting 228 Kotlin and Compose Multiplatform pitfalls, with a scanner.**

Ten area skills in the agent-skills markdown format index 228 trap files on Kotlin, Compose Multiplatform and desktop JVM, mined from the author's SimpMusic app. An eleventh skill, footgun-scan, runs a Python script that matches 32 patterns against added lines in a diff and can fail a CI step. Installs as a Claude Code plugin or as editable files via the skills CLI.

- **+** Area skills load an index first, so only 11 short descriptions sit in context each turn
- **+** Each trap pairs a failure mode with verification commands to run on your own tree
- **+** footgun-scan runs standalone with --base and --fail, usable as a CI step
- **+** Installs for Claude Code, Cursor, Codex, Copilot, Windsurf, Gemini via skills CLI
- **−** Lessons come from one codebase (SimpMusic), so coverage skews to media, Room and Compose
- **−** Scanner has only 32 patterns; look hits need manual review of the trap
- **−** GPL-3.0 license applies to the whole repository
- **−** Eval results are self-reported by the author; no independent benchmark

<sub>no GPU · Needs Python 3, Claude Code or another agent supporting agent skills, git (for scanner --base) · Models: Claude Code, Cursor, Codex, Copilot, Windsurf · [Repo](https://github.com/maxrave-dev/kotlin-footguns) · [🌐 Site ↗](https://simpmusic.org) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/kotlin-footguns/)</sub>

<a name="fable-method"></a>
### #&#8288;273 [fable-method](https://github.com/sahir619/fable-method) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: weak (23) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Oct 2026</sub>

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

<a name="lottie"></a>
### #&#8288;274 [lottie](https://github.com/diffusionstudio/lottie) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: popular (59) · Freshness: active (99) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 5.6k · MIT · Jul 2026</sub>

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

<a name="best-skills"></a>
### #&#8288;275 [best-skills](https://github.com/xstongxue/best-skills) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (39) · Freshness: active (100) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.1k · Apache-2.0 · Sep 2026</sub>

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

<a name="opensrc"></a>
### #&#8288;276 [opensrc](https://github.com/vercel-labs/opensrc) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (39) · Freshness: active (100) · Maintenance: weak (7) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.0k · Apache-2.0 · Sep 2026</sub>

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

<a name="typeui"></a>
### #&#8288;277 [typeui](https://github.com/bergside/typeui) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: weak (29) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.2k · custom license · Oct 2026</sub>

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

<a name="design-dna"></a>
### #&#8288;278 [design-dna](https://github.com/zanwei/design-dna) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: niche (25) · Freshness: active (100) · Maintenance: patchy (32) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Aug 2026</sub>

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

<a name="typesafe-ai-skills"></a>
### #&#8288;279 [skills](https://github.com/typesafe-ai/skills) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: known (36) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Oct 2026</sub>

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

<a name="opc-skills"></a>
### #&#8288;280 [opc-skills](https://github.com/resciencelab/opc-skills) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (22) · Freshness: active (94) · Maintenance: patchy (33) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · Apache-2.0 · Oct 2026</sub>

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

<a name="nopua"></a>
### #&#8288;281 [nopua](https://github.com/wuji-labs/nopua) <sub>score [45](../README.md#-how-we-rank "Score 45/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: patchy (30) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Sep 2026</sub>

**Agent skill that replaces fear-based prompts with trust-based debugging guidance.**

NoPUA is a prompt skill for coding agents. It activates after repeated failures or give-up phrases, or on /nopua. It replaces threat-style escalation with a staged method: switch perspective, zoom out, reset assumptions, then hand off with full context. The authors report a 9-scenario benchmark on Claude Sonnet 4.6, a three-way comparison against a fear-driven skill, and an arXiv paper.

- **+** Auto-triggers on 2+ failures, give-up phrases and frustration, or manually via /nopua
- **+** Publishes benchmark methodology, raw data and an arXiv paper (2603.14373)
- **+** Lists support for Claude Code, Codex CLI, Cursor, Kiro, OpenCode and others
- **+** Fixed escalation ladder: switch eyes, elevate, reset to zero, responsible handoff
- **−** Benchmark is author-run on one ~3000-line Python pipeline and one model
- **−** Three-way comparison uses only 5 runs per condition
- **−** Much of the README is psychology argument rather than usage detail
- **−** Install steps are not visible in the truncated README

<sub>no GPU · Models: Claude Code, OpenAI Codex CLI, Cursor, Kiro, OpenClaw · [Repo](https://github.com/wuji-labs/nopua) · [🌐 Site ↗](https://www.skills.sh/wuji-labs/nopua) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/nopua/)</sub>

<a name="loopy"></a>
### #&#8288;282 [loopy](https://github.com/forward-future/loopy) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: known (41) · Freshness: active (92) · Maintenance: weak (0) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.2k · MIT · Jul 2026</sub>

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

<a name="context-engineering-intro"></a>
### #&#8288;283 [context-engineering-intro](https://github.com/coleam00/context-engineering-intro) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (77) · Freshness: recent (51) · Maintenance: weak (0) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 14k · MIT · Mar 2026</sub>

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
### #&#8288;284 [openskills](https://github.com/numman-ali/openskills) <sub>score [42](../README.md#-how-we-rank "Score 42/100. Adoption: popular (74) · Freshness: slowing (42) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 11k · custom license · Jan 2026</sub>

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

<a name="beautify-github-readme"></a>
### #&#8288;285 [beautify-github-readme](https://github.com/oil-oil/beautify-github-readme) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: weak (13) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Oct 2026</sub>

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

<a name="dream-loop"></a>
### #&#8288;286 [dream-loop](https://github.com/achimala/dream-loop) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (19) · Freshness: active (100) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Sep 2026</sub>

**Agent skill that builds visuals by looping against an AI-generated target screenshot.**

An agent skill that has the model generate a target screenshot with image generation, build a game or scene toward it, then have a separate critic agent compare the live screenshot to the target. The loop repeats until the critic is satisfied, and can optionally generate a new target. The README says it is tested only with GPT-6 Astra in Codex.

- **+** Closed loop with a separate critic agent comparing screenshots to a target image
- **+** Installs with `npx skills add` or by cloning into a skills directory
- **+** Works with built-in or API image generation (e.g. a Gemini key)
- **+** Live demo and example prompt show a Three.js isometric scene
- **−** Tested only with GPT-6 Astra in Codex; other models are untested
- **−** Needs an agent with image generation and vision input
- **−** Subagents strongly preferred, so results may degrade without them
- **−** Blender needed for custom 3D modeling; no resource requirements documented

<sub>Needs Image generation (built-in or API, e.g. Gemini), Vision-capable agent, Blender (optional) · Models: GPT-6 Astra (Codex) · [Repo](https://github.com/achimala/dream-loop) · [▶️ Demo ↗](https://dream-loop-demo.anshu.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dream-loop/)</sub>

<a name="claude-code-settings"></a>
### #&#8288;287 [claude-code-settings](https://github.com/feiskyer/claude-code-settings) <sub>score [41](../README.md#-how-we-rank "Score 41/100. Adoption: niche (17) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.7k · MIT · Sep 2026</sub>

**Claude Code plugin with skills, subagents and provider settings templates.**

A Claude Code plugin marketplace repo bundling 12 skills (deep-research, github-fix-issue, github-review-pr, image generation via Gemini and OpenAI, codex-skill, handoff and others) and six subagents. It also ships settings.json templates for providers such as GitHub Copilot, LiteLLM, DeepSeek, Qwen, Vertex AI, Azure and OpenRouter. The README is written in Chinese.

- **+** Installs through the Claude Code plugin marketplace with two documented command styles
- **+** Settings templates for about 11 providers, including Copilot, LiteLLM, Azure and OpenRouter
- **+** Skills can be installed individually with npx skills
- **+** MIT licensed, with a script to update installed plugins
- **−** README and skill descriptions are in Chinese only
- **−** settings.json is not installed by the plugin and must be set up by hand
- **−** npx skills installs may lag behind the repo, per the README
- **−** Manual install overwrites ~/.claude; image and Codex skills need API keys or CLIs

<sub>no GPU · Needs Claude Code, Node.js (npx), Python 3, GEMINI_API_KEY, OPENAI_API_KEY, Codex CLI, yt-dlp, copilot-gateway or LiteLLM (optional) · Models: Anthropic Claude, GitHub Copilot, LiteLLM, DeepSeek, Qwen · [Repo](https://github.com/feiskyer/claude-code-settings) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-settings/)</sub>

<a name="awesome-design-skills"></a>
### #&#8288;288 [awesome-design-skills](https://github.com/bergside/awesome-design-skills) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: known (44) · Freshness: active (88) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.4k · MIT · Jun 2026</sub>

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

<a name="skill-codex"></a>
### #&#8288;289 [skill-codex](https://github.com/skills-directory/skill-codex) <sub>score [40](../README.md#-how-we-rank "Score 40/100. Adoption: niche (12) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · MIT · Oct 2026</sub>

**Claude Code skill that delegates tasks to the Codex CLI.**

A Claude Code plugin and skill that lets Claude run `codex exec` and resume Codex sessions for code analysis, refactoring and editing. Claude asks for the model and reasoning effort, picks a sandbox mode (read-only for analysis), and summarizes the output. Stderr thinking tokens are suppressed with `2>/dev/null` by default to save context.

- **+** Installs as a Claude Code plugin via marketplace, or as a standalone skill copy
- **+** Defaults to read-only sandbox for analysis tasks
- **+** Hides Codex thinking tokens by default to keep context small
- **+** Asks for model and reasoning effort unless the prompt already sets them
- **−** Requires the separate `codex` CLI installed with valid credentials
- **−** Legacy models such as gpt-5.5 are rejected for ChatGPT-account sign-ins
- **−** Operational details live in SKILL.md, not the README
- **−** No tagged release, so versioning is unknown

<sub>no GPU · Needs Claude Code, Codex CLI · Models: gpt-6-astra, gpt-6.1-sol, gpt-6-sol, gpt-6-luna, gpt-5.6-sol · [Repo](https://github.com/skills-directory/skill-codex) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skill-codex/)</sub>

<a name="awesome-openclaw-agents"></a>
### #&#8288;290 [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) <sub>score [39](../README.md#-how-we-rank "Score 39/100. Adoption: popular (51) · Freshness: active (81) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.0k · MIT · May 2026</sub>

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

<a name="app-store-preflight-skills"></a>
### #&#8288;291 [app-store-preflight-skills](https://github.com/truongduy2611/app-store-preflight-skills) <sub>score [38](../README.md#-how-we-rank "Score 38/100. Adoption: niche (10) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Oct 2026</sub>

**Agent skill that checks iOS/macOS projects for App Store rejection causes.**

An agent skill, installed with `npx skills add`, that loads an app-type checklist, pulls App Store metadata with the `asc` CLI, and scans the Xcode project against markdown rejection rules. Rules cover review notes, subscription terms, privacy manifests, third-party AI consent and unused entitlements. Findings are reported with severity, affected files and fixes.

- **+** Rules are plain markdown files, each mapped to an Apple guideline number
- **+** Ten app-type checklists: subscriptions, kids, health, games, AI, VPN, crypto and others
- **+** Reports severity and affected files, then applies fixes and re-runs checks
- **+** Reads metadata through the asc CLI, so it checks what is in App Store Connect
- **−** Depends on the asc CLI and its canonical JSON metadata layout; fastlane layouts need adapting
- **−** Only 14 rules documented, so coverage of Apple guidelines is partial
- **−** Checks are driven by the agent reading instructions, so results may vary between runs
- **−** No tagged releases; version pinning is unknown

<sub>no GPU · Needs asc CLI (App-Store-Connect-CLI), Xcode project, npx skills · [Repo](https://github.com/truongduy2611/app-store-preflight-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/app-store-preflight-skills/)</sub>

<a name="evo"></a>
### #&#8288;292 [evo](https://github.com/evo-hq/evo) <sub>score [37](../README.md#-how-we-rank "Score 37/100. Adoption: niche (13) · Freshness: active (100) · Maintenance: weak (11) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.5k · Apache-2.0 · Oct 2026</sub>

**Plugin that runs parallel optimization experiments on a codebase via coding agents.**

evo installs as a plugin for coding-agent hosts such as Claude Code, Codex and Cursor. Its discover skill finds a benchmark and gates, then optimize runs a tree search of experiments, each in its own git worktree, keeping changes that improve the score. A local dashboard (default port 8080) tracks experiments, and runs can go to Modal, E2B, Daytona, AWS, Azure or SSH.

- **+** Gates discard experiments that beat the score but fail tests or a held-out floor
- **+** Tree search with five frontier strategies, including argmax, top_k and pareto_per_task
- **+** Supports eight agent hosts and eight execution backends, local and remote
- **+** Dashboard for monitoring experiments, frontier strategy and backend selection
- **−** Sends anonymous telemetry by default; opt out with evo telemetry off
- **−** CLI, skills and hooks must stay version-matched; drift caused silent failures earlier
- **−** Needs a separate host agent CLI and its model access; cost is not documented
- **−** Remote backends require extra installs and provider accounts; setup steps are not covered

<sub>no GPU · Needs uv, git, Claude Code, Codex, Cursor, Kimi, OpenClaw, Hermes, Opencode or Pi, Modal, E2B, Daytona, AWS, Azure or SSH (optional, remote runs) · port 8080 · [Repo](https://github.com/evo-hq/evo) · [🌐 Site ↗](https://evo-hq.com/beta) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/evo/)</sub>

<a name="harmonist"></a>
### #&#8288;293 [harmonist](https://github.com/gammalabtechnologies/harmonist) <sub>score [34](../README.md#-how-we-rank "Score 34/100. Adoption: niche (28) · Freshness: active (87) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.3k · MIT · Jun 2026</sub>

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
### #&#8288;294 [claude-code-proxy](https://github.com/fuergaosi233/claude-code-proxy) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: known (35) · Freshness: slowing (49) · Maintenance: weak (11) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.8k · MIT · Mar 2026</sub>

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

<a name="codesight"></a>
### #&#8288;295 [codesight](https://github.com/houseofmvps/codesight) <sub>score [33](../README.md#-how-we-rank "Score 33/100. Adoption: niche (11) · Freshness: active (99) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Jul 2026</sub>

**CLI that maps a codebase into compact context files for AI coding assistants.**

codesight scans a project and writes a compact map of routes, database models, components, env vars and import-graph hot files to .codesight/. It also generates CLAUDE.md, .cursorrules, codex.md and AGENTS.md, a per-topic wiki, and can run as an MCP server with 14 tools. TypeScript gets AST parsing; other languages use regex detection.

- **+** Runs with one npx command, no config, no API keys, zero dependencies
- **+** Detects 30+ frameworks and 14 ORM parsers across about 14 languages
- **+** Blast-radius command traces affected files, routes and models through the import graph
- **+** Generated wiki and map are committed to git and need no LLM calls
- **−** Non-TypeScript languages use regex detection, so recall is lower than AST
- **−** Misses routes defined dynamically; README reports 38 of 43 on one project
- **−** Token-savings figures are estimates from formulas, not measured assistant sessions
- **−** No tagged release; the README gives no docs site

<sub>no GPU · Needs Node.js >= 18 · [Repo](https://github.com/houseofmvps/codesight) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codesight/)</sub>

<a name="myclaude"></a>
### #&#8288;296 [myclaude](https://github.com/stellarlinkco/myclaude) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: known (34) · Freshness: recent (73) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.7k · AGPL-3.0 · May 2026</sub>

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

<a name="cli-continues"></a>
### #&#8288;297 [cli-continues](https://github.com/yigitkonur/cli-continues) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (15) · Freshness: recent (69) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · MIT · May 2026</sub>

**CLI that moves a coding session between 16 AI coding tools.**

continues reads local session files from 16 AI coding CLIs and editors, including Claude Code, Codex, Copilot CLI, Gemini CLI, Cursor and Cline. It builds a handoff document with recent messages, file changes and tool activity, then launches a different tool with it. It also does native same-tool resume, session listing, inspection and bulk export.

- **+** Any-to-any handoff across 16 tools, 240 source and destination pairs
- **+** Read-only access to session files; index cached at ~/.continues/sessions.jsonl
- **+** Four verbosity presets plus .continues.yml for per-project defaults
- **+** Scriptable: list with JSON/JSONL output, inspect, and dump to markdown or JSON
- **−** Requires Node.js 22.5+ for built-in node:sqlite
- **−** Newer parsers were adapted from another project's adapters; fidelity unverified
- **−** Handoff is a summary document, not full history; detail depends on preset
- **−** No tagged releases

<sub>no GPU · Needs Node.js 22.5+, At least one supported AI coding tool installed · Models: Claude Code, Codex, GitHub Copilot CLI, Gemini CLI, Cursor · [Repo](https://github.com/yigitkonur/cli-continues) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cli-continues/)</sub>

<a name="paul"></a>
### #&#8288;298 [paul](https://github.com/christopherkahler/paul) <sub>score [32](../README.md#-how-we-rank "Score 32/100. Adoption: niche (5) · Freshness: active (97) · Maintenance: weak (7) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Aug 2026</sub>

**Plan-Apply-Unify workflow commands for structured development in Claude Code.**

PAUL installs 26 slash commands into Claude Code that enforce a plan, apply, unify loop. Plans carry Given/When/Then acceptance criteria, each task is checked against the spec after execution, and project state lives in a .paul/ directory (STATE.md, ROADMAP.md, per-phase PLAN and SUMMARY files). Implementation stays in-session; subagents are used only for research and discovery.

- **+** State persists in plain markdown files under .paul/, so sessions resume with /paul:resume
- **+** Each task gets an Execute/Qualify check against its acceptance criteria, with four status codes
- **+** Installs with one npx command, globally or per project, on Mac, Windows and Linux
- **+** Scope-adaptive plans (quick-fix, standard, complex) with a coherence check before approval
- **−** Works only with Claude Code; no other coding agent is mentioned
- **−** Graph, cost attribution and rule injection need BASE v2, linked from a community site
- **−** Mandatory UNIFY step and per-task qualification add process overhead to small changes
- **−** Claims such as subagent output being ~70% quality are stated without benchmarks

<sub>no GPU · Needs Claude Code, Node.js (npx) · Models: Claude · [Repo](https://github.com/christopherkahler/paul) · [🌐 Site ↗](https://chrisai.cv) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/paul/)</sub>

<a name="agent-toolkit"></a>
### #&#8288;299 [agent-toolkit](https://github.com/softaworks/agent-toolkit) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: known (32) · Freshness: slowing (47) · Maintenance: weak (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.6k · MIT · Mar 2026</sub>

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

<a name="skillkit"></a>
### #&#8288;300 [skillkit](https://github.com/rohitg00/skillkit) <sub>score [31](../README.md#-how-we-rank "Score 31/100. Adoption: niche (15) · Freshness: active (84) · Maintenance: weak (4) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.6k · Apache-2.0 · Jun 2026</sub>

**Package manager that installs and translates agent skills across 46 coding agents.**

SkillKit is a TypeScript CLI that installs skills from GitHub, GitLab, gists or local paths and translates them between agent formats such as SKILL.md and Cursor .mdc. It recommends skills from your repo's stack, scans skills for security issues, and can serve skill search over REST or MCP. Extras include session memory, AI skill generation and a terminal UI.

- **+** Translates one skill into formats for 46 agents, including Claude Code, Cursor, Codex and Copilot
- **+** Installs from GitHub, GitLab, gists and local paths; runs via npx with no setup
- **+** Slim install with --omit=optional: 118 packages versus 418 for the full install
- **+** Exposes skill search over REST on port 3737, an MCP server and a Python client
- **−** Broad scope: memory, mesh, messaging, issue planner and workflows all bundled in one tool
- **−** Skill quality depends on third-party sources; the 400K+ skills count comes from the README
- **−** AI skill generation needs an external model provider such as Claude, GPT-4, Gemini or Ollama
- **−** Install demo detects 32 agents while the README claims 46 supported

<sub>no GPU · Needs Node.js, npm · Models: Claude, GPT-4, Gemini, Ollama, OpenRouter · port 3737 · [Repo](https://github.com/rohitg00/skillkit) · [📖 Docs ↗](https://skillkit.sh/docs) · [🌐 Site ↗](https://skillkit.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skillkit/)</sub>

<a name="guard-skills"></a>
### #&#8288;301 [guard-skills](https://github.com/amelnagdy/guard-skills) <sub>score [29](../README.md#-how-we-rank "Score 29/100. Adoption: niche (5) · Freshness: active (91) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.3k · MIT · Jul 2026</sub>

**Review-pass skills that check AI-written code, tests and docs before merge.**

A package of five Markdown skills for coding agents, installed with the Skills CLI (`npx skills add`). Each guard is run on the agent's diff as a second pass: clean-code-guard, test-guard, docs-guard, plus wp-guard and woo-guard for WordPress and WooCommerce code. It works with Claude Code, Codex, Cursor, OpenCode and other agents the CLI supports.

- **+** Content is Markdown plus YAML metadata; README states no scripts, network calls or credentials
- **+** Installs per skill or as a whole package, per agent or globally
- **+** Deeper references load only when needed, keeping SKILL.md small
- **+** Covers WordPress and WooCommerce specifics such as HPOS, nonces and escaping
- **−** Skills install as copies and need `npx skills update` to pick up changes
- **−** Works as a reactive pass; the agent must be told to invoke each guard
- **−** Two of five guards apply only to WordPress or WooCommerce code
- **−** No tagged release; no catch-rate measurements in the README

<sub>no GPU · Needs Skills CLI (npx skills), Node.js · Models: Claude Code, Codex, Cursor, OpenCode · [Repo](https://github.com/amelnagdy/guard-skills) · [🌐 Site ↗](https://skills.sh/amElnagdy/guard-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/guard-skills/)</sub>

<a name="continuous-claude-v3"></a>
### #&#8288;302 [continuous-claude-v3](https://github.com/parcadei/continuous-claude-v3) <sub>score [26](../README.md#-how-we-rank "Score 26/100. Adoption: known (50) · Freshness: slowing (33) · Maintenance: weak (0) · Agent-ready: none (15) (each out of 100, weighted). Click for how we rank.") · ⭐ 3.9k · MIT · Jan 2026</sub>

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
### #&#8288;303 [taches-cc-resources](https://github.com/glittercowboy/taches-cc-resources) <sub>score [24](../README.md#-how-we-rank "Score 24/100. Adoption: niche (24) · Freshness: recent (56) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 2.0k · MIT · Apr 2026</sub>

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

<a name="mcphub-nvim"></a>
### #&#8288;304 [mcphub.nvim](https://github.com/ravitemer/mcphub.nvim) <sub>score [19](../README.md#-how-we-rank "Score 19/100. Adoption: niche (20) · Freshness: quiet (28) · Maintenance: weak (17) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.8k · MIT · Jan 2026</sub>

**MCP client plugin for Neovim that connects MCP servers to chat plugins.**

mcphub.nvim manages MCP servers from inside Neovim and exposes their tools, resources and prompts to Avante.nvim, CodeCompanion.nvim and CopilotChat.nvim. It supports STDIO, Streamable-HTTP and SSE transports, OAuth with PKCE, and a marketplace for installing servers. Servers can also be written natively in Lua.

- **+** Works with Avante, CodeCompanion and CopilotChat; MCP prompts become slash commands
- **+** Supports STDIO, Streamable-HTTP and SSE transports, plus OAuth with PKCE and header auth
- **+** Reads VS Code style config, JSON5, and project-local configs merged with global ones
- **+** Multiple Neovim instances stay in sync; Lua-native MCP servers and a dev mode with hot reload
- **−** MCP roots and sampling are not supported
- **−** Tests are listed as unchecked in the README TODO
- **−** #variables support in Avante is not implemented
- **−** Last release 2025-07-31; the README gives no install steps, only a docs site

<sub>no GPU · Needs Neovim, Avante.nvim, CodeCompanion.nvim or CopilotChat.nvim · [Repo](https://github.com/ravitemer/mcphub.nvim) · [📖 Docs ↗](https://ravitemer.github.io/mcphub.nvim/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/mcphub-nvim/)</sub>

<a name="tutor-skills"></a>
### #&#8288;305 [tutor-skills](https://github.com/bevibing/tutor-skills) <sub>score [16](../README.md#-how-we-rank "Score 16/100. Adoption: niche (8) · Freshness: slowing (45) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Feb 2026</sub>

**Claude Code skills that build Obsidian study vaults and quiz you on them.**

Two Claude Code skills. /tutor-setup converts PDF, TXT, MD, HTML and EPUB files, or a source code project, into an Obsidian StudyVault with linked notes, dashboards and practice questions. /tutor then runs quiz rounds of 4 multiple-choice questions and tracks proficiency per concept, updating the vault files after each round.

- **+** Auto-detects document or codebase mode from project markers like package.json or go.mod
- **+** Codebase mode generates onboarding notes, flow traces and exercises for new developers
- **+** Per-concept tracking stores attempts, correct count and error notes to drive drill sessions
- **+** Installs with one npx skills command or a manual install.sh
- **−** Requires the Claude Code CLI; other agents are only implied via npx skills
- **−** Vault format and dashboards are built around Obsidian, though it is only recommended
- **−** No release published; no tests or output quality benchmarks described
- **−** Quiz format is fixed at 4 questions per round with 4 options each

<sub>no GPU · Needs Claude Code CLI, Obsidian (recommended), npx skills (optional installer) · Models: Claude (via Claude Code) · [Repo](https://github.com/bevibing/tutor-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/tutor-skills/)</sub>

<a name="vibesec-skill"></a>
### #&#8288;306 [vibesec-skill](https://github.com/behisecc/vibesec-skill) <sub>score [15](../README.md#-how-we-rank "Score 15/100. Adoption: niche (8) · Freshness: slowing (41) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · Apache-2.0 · Feb 2026</sub>

**Security skill that steers AI coding agents away from common web vulnerabilities.**

A skill folder for coding agents that steers generated code away from common web vulnerabilities. It covers access control, client-side, server-side, authentication and API issues such as IDOR, XSS, SSRF, SQL injection and JWT handling, with checklists per class. Install by cloning the repo into the skills directory of Claude Code, Cursor, Codex, GitHub Copilot or Antigravity.

- **+** Installs by cloning into a skills directory; no runtime or services needed
- **+** Documents install paths for five agents: Claude Code, Cursor, Codex, Copilot, Antigravity
- **+** Names specific classes: IDOR, XSS, CSRF, SSRF, SQLi, XXE, path traversal, JWT, GraphQL
- **+** Includes framework notes (React, Vue, Node.js, Python, Java, .NET) and cloud metadata guidance
- **−** README says it covers only 60-70% of common vulnerabilities
- **−** Fuller coverage is offered through a separate product at vibesec.sh
- **−** Guides code generation only; does not scan or test existing code
- **−** No releases published; last commit 2026-02-17

<sub>no GPU · Needs Claude Code, Cursor, Codex, GitHub Copilot or Antigravity · Models: Any model used through a supported agent · [Repo](https://github.com/behisecc/vibesec-skill) · [🌐 Site ↗](https://vibesec.sh/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vibesec-skill/)</sub>

<a name="vibekit"></a>
### #&#8288;307 [vibekit](https://github.com/superagent-ai/vibekit) <sub>score [10](../README.md#-how-we-rank "Score 10/100. Adoption: niche (22) · Freshness: quiet (11) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.9k · MIT · Nov 2025</sub>

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

<a name="sudolang"></a>
### #&#8288;308 [sudolang](https://github.com/paralleldrive/sudolang) <sub>score [8](../README.md#-how-we-rank "Score 8/100. Adoption: niche (8) · Freshness: quiet (20) · Maintenance: weak (0) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 1.4k · MIT · Dec 2025</sub>

**Pseudocode language for writing structured prompts that LLMs interpret directly.**

SudoLang is a pseudocode language for prompting LLMs, with interfaces, constraints, /commands, pattern matching and a |> function composition operator. Programs are plain text that models such as ChatGPT, Claude, Gemini and Llama interpret without a pasted spec. The repo holds the language documentation, examples and a VS Code/Cursor extension (.vsix) for highlighting .sudo, .sudo.md and .mdc files.

- **+** Works across ChatGPT, Claude, Gemini and Llama without pasting a spec
- **+** Includes a VS Code/Cursor extension with highlighting for .sudo, .sudo.md and .mdc
- **+** Docs, examples folder and several articles and talks for learning
- **+** MIT licensed; README claims 20-30% fewer tokens than equivalent natural-language prompts
- **−** No runtime or interpreter; behavior depends on how each model reads the prompt
- **−** Token savings and reasoning gains are claims in the README, not benchmarked here
- **−** Extension installs from a local .vsix after cloning, not from a marketplace
- **−** No tagged releases; last commit 2025-12-23

<sub>no GPU · Needs VS Code or Cursor (optional, for the extension) · Models: ChatGPT, Bing Chat, Anthropic Claude, Google Gemini/Gemma, Meta Llama · [Repo](https://github.com/paralleldrive/sudolang) · [📖 Docs ↗](https://github.com/paralleldrive/sudolang/blob/main/sudolang.sudo.md) · [🌐 Site ↗](https://paralleldrive.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/sudolang/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
