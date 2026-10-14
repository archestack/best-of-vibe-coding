# 🧩 Skills, plugins and rules reviews · Best of Vibe Coding

Add-ons that make coding agents better: skills, plugins, rules, hooks and memory for Claude Code, Codex, Cursor and others. Back to the [leaderboard](../README.md#-skills-plugins-and-rules).

<sub>🌐 Also on the web: [Skills, plugins and rules on archestack.com](https://archestack.com/best-of-vibe-coding/skills-plugins/), each project on its own page.</sub>

<a name="skills"></a>
### 🥇 [skills](https://github.com/mattpocock/skills) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 291k · MIT · Oct 2026</sub>

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
### 🥈 [ecc](https://github.com/affaan-m/ecc) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (98) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 279k · MIT · Oct 2026</sub>

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

<a name="caveman"></a>
### 🥉 [caveman](https://github.com/juliusbrussee/caveman) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (87) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 112k · Apache-2.0 · Oct 2026</sub>

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

<a name="ponytail"></a>
### #&#8288;4 [ponytail](https://github.com/dietrichgebert/ponytail) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (96) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 163k · MIT · Oct 2026</sub>

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
### #&#8288;5 [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: widely used (90) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 136k · MIT · Oct 2026</sub>

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

<a name="impeccable"></a>
### #&#8288;6 [impeccable](https://github.com/pbakaus/impeccable) <sub>score [90](../README.md#-how-we-rank "Score 90/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 81k · Apache-2.0 · Oct 2026</sub>

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

<a name="spec-kit"></a>
### #&#8288;7 [spec-kit](https://github.com/github/spec-kit) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 141k · MIT · Oct 2026</sub>

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
### #&#8288;8 [agent-skills](https://github.com/addyosmani/agent-skills) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 106k · MIT · Oct 2026</sub>

**Markdown skill pack and slash commands for the software lifecycle in coding agents.**

A set of 25 SKILL.md workflows covering spec, plan, build, test, review and ship, plus 9 slash commands, 4 agent personas and reference checklists. Skills are plain Markdown with steps, verification gates and anti-rationalization tables. They install into Claude Code, Codex, Cursor, Gemini CLI, Copilot and others via the skills CLI or native plugin commands.

- **+** Installs into 70+ agents with one `npx skills add` command
- **+** Each skill has explicit steps, verification gates and exit criteria
- **+** Native plugin installs for Claude Code, Codex, Antigravity and Gemini CLI
- **+** Skills are plain Markdown, usable with any agent that reads instruction files
- **−** Slash commands like /spec and /build are Claude Code only; Copilot needs skills invoked by name
- **−** Per-skill npx install omits the shared references/ checklists (issue #361)
- **−** Cursor and Windsurf need manual copying into rules or skills directories
- **−** Testing reference examples target JavaScript/TypeScript

<sub>no GPU · Needs Node.js (npx), An AI coding agent such as Claude Code, Codex or Gemini CLI · safety checks passed 9 of 10 · [Repo](https://github.com/addyosmani/agent-skills) · [📖 Docs ↗](https://github.com/addyosmani/agent-skills/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills/)</sub>

<a name="claude-mem"></a>
### #&#8288;9 [claude-mem](https://github.com/thedotmack/claude-mem) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 101k · Apache-2.0 · Oct 2026</sub>

**Persistent cross-session memory plugin for Claude Code and other coding agents.**

Claude-Mem hooks into Claude Code session lifecycle events (SessionStart, UserPromptSubmit, PostToolUse, Stop, SessionEnd), records tool-usage observations and summaries in SQLite, and injects relevant context into later sessions. A local Bun-managed worker serves an HTTP API and web viewer, with hybrid FTS5 and Chroma vector search exposed through three MCP tools: search, timeline and get_observations. Installers also cover OpenCode, T3 Code, Antigravity, OMP, Pi and OpenClaw.

- **+** Search, timeline, get_observations flow filters before fetching details; README claims ~10x token savings
- **+** Local SQLite storage with FTS5 plus Chroma hybrid search, and a web viewer for stored memory
- **+** One npx installer targets Claude Code, OpenCode, T3 Code, Antigravity, OMP, Pi and others
- **+** `<private>` tags exclude content from storage; settings live in ~/.claude-mem/settings.json
- **−** Default installer prompts for sign-in to a hosted observer with a 30-day trial, then paid
- **−** Needs Node 20+, Bun and uv; the last two are auto-installed
- **−** `npm install -g claude-mem` installs only the SDK, not the hooks or worker
- **−** Summaries are generated by an extra model (hosted, OpenRouter, Gemini or Anthropic plan), adding usage

<sub>no GPU · Docker + Compose · Needs Node.js 20+, Bun, uv, SQLite, Chroma · Models: Anthropic plan, OpenRouter, Gemini, claude-mem hosted observer · safety checks passed 9 of 10 · [Repo](https://github.com/thedotmack/claude-mem) · [📖 Docs ↗](https://docs.claude-mem.ai/) · [🌐 Site ↗](https://docs.claude-mem.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-mem/)</sub>

<a name="superpowers"></a>
### #&#8288;10 [superpowers](https://github.com/obra/superpowers) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 299k · MIT · Oct 2026</sub>

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

<a name="archify"></a>
### #&#8288;11 [archify](https://github.com/tt-a1i/archify) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: widely used (80) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 83k · MIT · Oct 2026</sub>

**Agent skill that turns descriptions or repos into interactive HTML diagrams.**

Archify is a skill for Cursor, Claude Code, Codex CLI and OpenCode, installed with `npx skills add tt-a1i/archify -g`. Given a description or a repository, the agent generates a self-contained interactive HTML diagram of one of five types: architecture, workflow, sequence, data flow or lifecycle. Output supports theme switching, route and reach tracing, and PNG or share-card export.

- **+** Output is standalone HTML that opens in a browser without installing Archify
- **+** Five diagram types, plus Before/Delta/After architecture comparison with a machine receipt
- **+** Works from a plain description; no repository required
- **+** Update check can be disabled with ARCHIFY_UPDATE_CHECK_DISABLED=1 and never auto-installs
- **−** Needs an AI coding agent and its model; Archify does not generate diagrams alone
- **−** Optional update check makes a network GET to a fixed manifest by default
- **−** Deployment-ownership profile checks authored facts only, not live infrastructure
- **−** README is heavy on sponsors and promotion, which buries technical details

<sub>no GPU · Needs Node.js (npx), Cursor, Claude Code, Codex CLI or OpenCode · Models: unknown (uses the host agent's model) · safety checks passed 10 of 10 · [Repo](https://github.com/tt-a1i/archify) · [▶️ Demo ↗](https://archify.si/gallery.html) · [📖 Docs ↗](https://archify.si/guide.html) · [🌐 Site ↗](https://archify.si) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archify/)</sub>

<a name="ruflo"></a>
### #&#8288;12 [ruflo](https://github.com/ruvnet/ruflo) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (77) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

**Agent harness for Claude Code and Codex with swarms, memory and MCP tools.**

Ruflo wraps Claude Code and Codex with a CLI, an MCP server and Claude Code plugins that add agent definitions, swarm coordination, vector-backed memory, hooks and a console UI. It installs either as marketplace plugins (35 listed) or through `npx ruflo init`, which writes .claude/ config, hooks and a daemon into the project. The README cites 98 agents, 60+ commands, 30 skills and 314 MCP tools.

- **+** Two install paths: zero-file Claude Code plugins or full CLI init with hooks and MCP server
- **+** Works with any MCP client via `npx -y ruflo@latest mcp start`
- **+** Console permission levels (read/write/manage/full) with ask or auto approval
- **+** Optional standalone terminal UI via `npx ruflo tui`, with a plain mode for scripts
- **−** Large surface (314 MCP tools, 35 plugins) that the README itself says not to learn
- **−** Mods run with account permissions, are not sandboxed; README says read code first
- **−** Console, mods and hooks are Claude Code integrations; other clients get MCP tools only
- **−** Plugin path has different tool names and fewer features than the CLI path

<sub>Needs Node.js/npx, Claude Code 2.1.287+ (for plugins) · Models: Claude Code, Codex, Ollama (via ruflo-ruvllm plugin) · safety checks passed 13 of 17 · [Repo](https://github.com/ruvnet/ruflo) · [▶️ Demo ↗](https://raw.githubusercontent.com/ruvnet/ruflo/main/docs/assets/ruflo-console-theme-compact.svg) · [📖 Docs ↗](https://github.com/ruvnet/ruflo/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://cognitum.one/agentic-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruflo/)</sub>

<a name="oh-my-claudecode"></a>
### #&#8288;13 [oh-my-claudecode](https://github.com/yeachan-heo/oh-my-claudecode) <sub>score [86](../README.md#-how-we-rank "Score 86/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

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

<a name="graphify"></a>
### #&#8288;14 [graphify](https://github.com/graphify-labs/graphify) <sub>score [85](../README.md#-how-we-rank "Score 85/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 126k · Apache-2.0 · Oct 2026</sub>

**Skill that maps a codebase and docs into a queryable knowledge graph.**

Graphify installs as a skill for AI coding assistants such as Claude Code, Cursor, Codex and Gemini CLI. Running /graphify parses code with tree-sitter across about 40 languages, and handles docs, PDFs, images and video through the assistant's model. It writes graph.json, graph.html and GRAPH_REPORT.md, and the graph can then be queried with query, path and explain commands instead of grepping files.

- **+** Code parsing is local tree-sitter AST, with no LLM calls and no data leaving the machine
- **+** Each edge is tagged EXTRACTED or INFERRED, so direct reads are separable from resolved links
- **+** Installs into 20+ assistants with one command per platform, including project-scoped installs
- **+** Outputs plain files (graph.json, graph.html, GRAPH_REPORT.md) queryable without re-reading source
- **−** Docs, PDFs, images and video need an LLM backend or the assistant's model for the semantic pass
- **−** PDF, Office, video, MCP and Neo4j support are separate optional extras to install
- **−** Monorepo and cross-repo support, formal verification and Sentry/Jira connectors are in paid Graphify Cloud
- **−** Benchmarks are the project's own; LOCOMO QA accuracy is below supermemory (45.3% vs 49.7%)

<sub>no GPU · Docker · Needs Python 3.10+, uv or pipx, AI coding assistant · Models: Anthropic Claude, OpenAI and compatible APIs, Google Gemini, AWS Bedrock, Azure OpenAI · safety checks passed 14 of 15 · [Repo](https://github.com/graphify-labs/graphify) · [📖 Docs ↗](https://docs.graphify.com) · [🌐 Site ↗](https://graphify.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphify/)</sub>

<a name="cc-switch"></a>
### #&#8288;15 [cc-switch](https://github.com/farion1231/cc-switch) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 144k · MIT · Oct 2026</sub>

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
### #&#8288;16 [gstack](https://github.com/garrytan/gstack) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 136k · MIT · Oct 2026</sub>

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

<a name="rtk"></a>
### #&#8288;17 [rtk](https://github.com/rtk-ai/rtk) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (79) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 83k · Apache-2.0 · Oct 2026</sub>

**CLI proxy that compresses shell command output before coding agents read it.**

rtk is a single Rust binary that wraps 100+ shell commands (git, cargo test, pytest, docker, kubectl, aws and others) and returns grouped, truncated or deduplicated output. `rtk init` installs a hook for Claude Code, Gemini CLI, Codex, Cursor, Windsurf and other agents that rewrites Bash calls such as `git status` to `rtk git status`. The README claims up to 90% less bash output and under 10ms overhead.

- **+** Single Rust binary; README states under 10ms overhead per command
- **+** Auto-rewrite hook covers many agents: Claude Code, Gemini CLI, Codex, Cursor, Windsurf, Cline
- **+** Per-command filters for tests, linters, git, docker, kubectl, AWS and Pulumi
- **+** `rtk gain` reports savings history; `rtk discover` finds missed rewrites
- **−** Hook only affects Bash calls; Claude's built-in Read, Grep and Glob bypass it
- **−** Token counts are estimated as bytes/4; no tokenizer, so absolute numbers are approximate
- **−** Up to 90% applies to bash output only, not to the total bill
- **−** Another 'rtk' crate exists on crates.io; install via git, not the crate name

<sub>no GPU · Models: Claude Code, Gemini CLI, Codex, Cursor, Windsurf · safety checks passed 9 of 10 · [Repo](https://github.com/rtk-ai/rtk) · [📖 Docs ↗](https://www.rtk-ai.app/guide/troubleshooting) · [🌐 Site ↗](https://www.rtk-ai.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rtk/)</sub>

<a name="openspec"></a>
### #&#8288;18 [openspec](https://github.com/fission-ai/openspec) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 72k · MIT · Oct 2026</sub>

**Spec-driven workflow CLI that guides AI coding assistants through plan, apply and archive.**

OpenSpec is a Node.js CLI that adds an `openspec/` folder to a repo and installs slash commands (such as /opsx:propose, /opsx:apply, /opsx:archive) into 30+ AI coding tools. Each change gets a folder with proposal.md, specs, design.md and tasks.md in plain Markdown, which the human reviews before code is written. A beta Stores feature keeps specs and changes in a separate shared repo for cross-repo work.

- **+** Specs and changes are plain Markdown in the repo, versioned with git
- **+** Works with 30+ AI coding tools through generated slash commands
- **+** Install via npm or Homebrew; no server or database needed
- **+** Designed for existing codebases, with an adoption guide for brownfield projects
- **−** Needs Node.js 20.19.0 or higher
- **−** Stores (cross-repo shared planning) are still in beta
- **−** Collects anonymous usage telemetry by default; opt-out via config or env var
- **−** Command syntax differs per tool, e.g. /opsx-propose, @opsx-propose, $openspec-propose

<sub>no GPU · Needs Node.js 20.19.0+, an AI coding assistant · Models: Codex 5.5 and Opus 4.7 recommended; works with 30+ AI coding tools · safety checks passed 9 of 10 · [Repo](https://github.com/fission-ai/openspec) · [📖 Docs ↗](https://github.com/Fission-AI/OpenSpec/blob/main/docs/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openspec/)</sub>

<a name="agentic-awesome-skills"></a>
### #&#8288;19 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · MIT · Oct 2026</sub>

**2,689 installable SKILL.md playbooks for coding agents, with a local MCP.**

A library of SKILL.md playbooks for Claude Code, Codex, Cursor, Gemini CLI, Kiro, Copilot and others, installed with an npx installer. AAS Core is a local MCP plus an `aas` CLI that lets the agent search the catalog, save its chosen skills to `aas-stack.json`, validate them and write a plan preview. Core does not rank skills, and apply and recovery are experimental.

- **+** 2,689+ skills, each a plain SKILL.md, with a machine-readable skills_index.json
- **+** Installer has --dry-run and filters for category, risk and tags
- **+** Install targets for about a dozen agent hosts, plus Claude Code and Codex plugin bundles
- **+** Core records the exact selected skills in a manifest you can review before installing
- **−** Core apply and recovery are experimental and outside the supported preview
- **−** Validation checks structure only, not whether a skill fits or is safe
- **−** Loading too many skills can overload Antigravity, so a selected set or filter is required
- **−** Core MCP setup is supported only for Codex and Claude

<sub>no GPU · Needs Node.js/npm (npx installer) · Models: Claude Code, Codex CLI, Cursor, Gemini CLI, Kiro · safety checks passed 7 of 11 · [Repo](https://github.com/sickn33/agentic-awesome-skills) · [▶️ Demo ↗](https://aaskills.tech/workbench) · [📖 Docs ↗](https://github.com/sickn33/agentic-awesome-skills/blob/v19.6.0/docs/users/aas-core.md) · [🌐 Site ↗](https://aaskills.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentic-awesome-skills/)</sub>

<a name="book-to-skill"></a>
### #&#8288;20 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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

<a name="repomix"></a>
### #&#8288;21 [repomix](https://github.com/yamadashy/repomix) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: known (48) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<a name="taste-skill"></a>
### #&#8288;22 [taste-skill](https://github.com/leonxlnx/taste-skill) <sub>score [80](../README.md#-how-we-rank "Score 80/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 96k · MIT · Oct 2026</sub>

**Agent Skills that steer AI coding agents toward better frontend design.**

A set of SKILL.md files that give coding agents rules for layout, typography, motion and spacing, plus image-generation skills for web, mobile and brand-kit reference boards. The default skill exposes three 1-10 dials (DESIGN_VARIANCE, MOTION_INTENSITY, VISUAL_DENSITY). Installs with `npx skills add` or as a Claude Code plugin; also usable in Codex and Cursor.

- **+** Installs per skill via `npx skills add --skill <name>` or as a Claude Code plugin
- **+** Three adjustable dials in the default skill: variance, motion intensity, visual density
- **+** Separate skills for redesign, minimalist, brutalist, soft UI and image-to-code workflows
- **+** Framework agnostic; rules target design intent rather than one framework API
- **−** Default taste-skill v2 is marked experimental and not yet at a stable 2.0.0
- **−** Image-generation skills need a separate generator such as ChatGPT Images
- **−** No published releases; output quality depends on the agent and model used
- **−** README gives no benchmarks or measured results, only one example screenshot

<sub>no GPU · Needs npx skills CLI, Codex, Cursor or Claude Code, ChatGPT Images or similar (image skills only) · Models: Codex, Claude Code, Cursor, ChatGPT · safety checks passed 8 of 9 · [Repo](https://github.com/leonxlnx/taste-skill) · [🌐 Site ↗](https://tasteskill.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taste-skill/)</sub>

<a name="claude-hud"></a>
### #&#8288;23 [claude-hud](https://github.com/jarrodwatts/claude-hud) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (45) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<a name="vercel-labs-skills"></a>
### #&#8288;24 [skills](https://github.com/vercel-labs/skills) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (60) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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

<a name="oh-my-codex"></a>
### #&#8288;25 [oh-my-codex](https://github.com/yeachan-heo/oh-my-codex) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: popular (55) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 20+, OpenAI Codex CLI, tmux (macOS/Linux team runtime), git · Models: OpenAI Codex CLI models · [Repo](https://github.com/yeachan-heo/oh-my-codex) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-codex-website/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-codex/)</sub>

<a name="planning-with-files"></a>
### #&#8288;26 [planning-with-files](https://github.com/othmanadi/planning-with-files) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (39) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Oct 2026</sub>

**Agent skill that keeps task plans in markdown files that survive /clear.**

Keeps task_plan.md, findings.md and progress.md in the project and uses lifecycle hooks to re-inject the active plan each turn, so a coding agent resumes after /clear, compaction or a crash. A Stop-time completion gate can hold the agent until the plan reports complete. Installs via `npx skills add` for 60+ agents, with native plugins for Claude Code, Codex CLI, Qoder CLI, Pi, Hermes, OpenCode and DeepSeek Harness.

- **+** Plain markdown plan files on disk, no runtime state or database elsewhere
- **+** Native plugins for several hosts plus the generic Agent Skills install route
- **+** Completion gate holds the agent's stop until the plan reports complete
- **+** Translated variants in 5 languages ship the full script surface
- **−** Hook behavior and available commands differ per host; Qoder CLI needs Bash and Python 3.10+
- **−** Plan files are gitignored and overwritten by the next task unless you keep them
- **−** Benchmark claims rest on small samples (3 blind A/B comparisons, 30 assertions)
- **−** Completion gate depends on literal English status tokens matched with grep -F

<sub>no GPU · Needs Bash, Python 3.10+ (Qoder CLI), Node.js/npx (installer) · safety checks passed 10 of 10 · [Repo](https://github.com/othmanadi/planning-with-files) · [📖 Docs ↗](https://github.com/OthmanAdi/planning-with-files/blob/master/docs/installation.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/planning-with-files/)</sub>

<a name="compound-engineering-plugin"></a>
### #&#8288;27 [compound-engineering-plugin](https://github.com/everyinc/compound-engineering-plugin) <sub>score [76](../README.md#-how-we-rank "Score 76/100. Adoption: known (34) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs An AI coding agent host (Claude Code, Cursor, Codex, etc.), pi-subagents (Pi only) · [Repo](https://github.com/everyinc/compound-engineering-plugin) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/compound-engineering-plugin/)</sub>

<a name="agents"></a>
### #&#8288;28 [agents](https://github.com/wshobson/agents) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: popular (65) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

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

<a name="beads"></a>
### #&#8288;29 [beads](https://github.com/gastownhall/beads) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (41) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

**Dependency-aware issue tracker CLI that gives coding agents persistent task memory.**

bd (Beads) is a Go CLI that stores tasks as a dependency graph in a Dolt database, replacing markdown TODO lists for coding agents. Agents use commands such as bd ready, bd update --claim and bd close, with JSON output and hash-based IDs to avoid merge collisions. bd setup installs hooks and instructions for Claude Code, Codex, Cursor and others; sync runs through Dolt remotes on a git remote.

- **+** Hash-based IDs (bd-a1b2) avoid merge collisions across agents and branches
- **+** Embedded Dolt mode needs no separate database server
- **+** bd setup installs integrations for Claude Code, Codex, Cursor, Factory and more
- **+** Works without git via BEADS_DIR and --stealth, including non-git VCS
- **−** Embedded mode is single-writer; concurrent writers need an external dolt sql-server
- **−** HTTP backend is marked experimental and diverges from local behavior in documented ways
- **−** Upgrades across schema migrations need a designated clone to migrate and push
- **−** issues.jsonl is only an export, not a backup; sync relies on Dolt remotes

<sub>no GPU · Needs Dolt (embedded by default; external dolt sql-server for server mode), git remote (optional, for sync) · safety checks passed 9 of 10 · [Repo](https://github.com/gastownhall/beads) · [📖 Docs ↗](https://beads.gascity.com/) · [🌐 Site ↗](https://beads.gascity.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beads/)</sub>

<a name="agency-agents"></a>
### #&#8288;30 [agency-agents](https://github.com/msitarzewski/agency-agents) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 160k · MIT · Oct 2026</sub>

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

<a name="understand-anything"></a>
### #&#8288;31 [understand-anything](https://github.com/egonex-ai/understand-anything) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (82) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 86k · MIT · Oct 2026</sub>

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

<a name="claude-howto"></a>
### #&#8288;32 [claude-howto](https://github.com/luongnv89/claude-howto) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Oct 2026</sub>

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

<a name="claude-code-best-practice"></a>
### #&#8288;33 [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 68k · MIT · Oct 2026</sub>

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
### #&#8288;34 [i-have-adhd](https://github.com/ayghri/i-have-adhd) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (71) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 57k · MIT · Oct 2026</sub>

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

<a name="claude-code-templates"></a>
### #&#8288;35 [claude-code-templates](https://github.com/davila7/claude-code-templates) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

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

<a name="diagram-design"></a>
### #&#8288;36 [diagram-design](https://github.com/cathrynlavery/diagram-design) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 55k · MIT · Oct 2026</sub>

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

<a name="opencodex"></a>
### #&#8288;37 [opencodex](https://github.com/lidge-jun/opencodex) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: niche (23) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 17k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node 18+, Bun (bundled on npm install) · Models: Anthropic, Google Gemini, xAI Grok, OpenAI, DeepSeek · port 10100 · [Repo](https://github.com/lidge-jun/opencodex) · [📖 Docs ↗](https://opencodex.me/getting-started/installation/) · [🌐 Site ↗](https://opencodex.me/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/opencodex/)</sub>

<a name="claude-skills"></a>
### #&#8288;38 [claude-skills](https://github.com/alirezarezvani/claude-skills) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: known (42) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Aug 2026</sub>

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

<a name="context-mode"></a>
### #&#8288;39 [context-mode](https://github.com/mksglu/context-mode) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (50) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · custom license · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js >= 22.5 or Bun · Models: Claude Code, Gemini CLI, VS Code Copilot, JetBrains Copilot, GitHub Copilot CLI · [Repo](https://github.com/mksglu/context-mode) · [🌐 Site ↗](https://context-mode.com/insight) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/context-mode/)</sub>

<a name="awesome-claude-code-subagents"></a>
### #&#8288;40 [awesome-claude-code-subagents](https://github.com/voltagent/awesome-claude-code-subagents) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (35) · Freshness: active (100) · Maintenance: fair (67) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, curl (standalone installer) · Models: Claude · [Repo](https://github.com/voltagent/awesome-claude-code-subagents) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/awesome-claude-code-subagents/)</sub>

<a name="claude-code-game-studios"></a>
### #&#8288;41 [claude-code-game-studios](https://github.com/donchitos/claude-code-game-studios) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: known (37) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<a name="claude-video"></a>
### #&#8288;42 [claude-video](https://github.com/bradautomates/claude-video) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: niche (26) · Freshness: active (100) · Maintenance: fair (65) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 19k · MIT · Sep 2026</sub>

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

<sub>RAM ≥ 8 GB · GPU optional · Needs Python 3.10+, FFmpeg, yt-dlp, Deno (YouTube), WhisperX 3.8.6 (optional), Node.js (Skills CLI install only) · Models: Gemini (gemini-3.7-flash default), WhisperX, Groq whisper-large-v3, OpenAI whisper-1 · [Repo](https://github.com/bradautomates/claude-video) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-video/)</sub>

<a name="img2threejs"></a>
### #&#8288;43 [img2threejs](https://github.com/img2threejs/img2threejs) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (24) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js >= 18, Git, Python >= 3.10, Three.js, Claude Code, Codex or OpenCode · Models: Claude Code, Codex, OpenCode, Hermes · [Repo](https://github.com/img2threejs/img2threejs) · [▶️ Demo ↗](https://img2threejs.io/) · [🌐 Site ↗](https://img2threejs.io/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/img2threejs/)</sub>

<a name="claude-plugins-official"></a>
### #&#8288;44 [claude-plugins-official](https://github.com/anthropics/claude-plugins-official) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · Apache-2.0 · Oct 2026</sub>

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

<a name="agentskills"></a>
### #&#8288;45 [agentskills](https://github.com/agentskills/agentskills) <sub>score [59](../README.md#-how-we-rank "Score 59/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Aug 2026</sub>

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

<a name="design-md"></a>
### #&#8288;46 [design.md](https://github.com/google-labs-code/design.md) <sub>score [58](../README.md#-how-we-rank "Score 58/100. Adoption: known (44) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Jul 2026</sub>

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

<a name="superclaude-framework"></a>
### #&#8288;47 [superclaude_framework](https://github.com/superclaude-org/superclaude_framework) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: known (32) · Freshness: active (98) · Maintenance: patchy (32) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 24k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Claude Code, pipx, Tavily MCP (optional), Context7 MCP (optional), Serena MCP (optional), Playwright MCP (optional) · Models: Claude (via Claude Code) · [Repo](https://github.com/superclaude-org/superclaude_framework) · [🌐 Site ↗](https://superclaude.netlify.app/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superclaude-framework/)</sub>

<a name="agency-agents-zh"></a>
### #&#8288;48 [agency-agents-zh](https://github.com/jnmetacode/agency-agents-zh) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: fair (63) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Bash, Node.js (only for agency-orchestrator) · Models: Claude Code, Cursor, GitHub Copilot, Codex CLI, Gemini CLI · [Repo](https://github.com/jnmetacode/agency-agents-zh) · [▶️ Demo ↗](https://ao.aiolaola.com/experts) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents-zh/)</sub>

<a name="google-skills"></a>
### #&#8288;49 [skills](https://github.com/google/skills) <sub>score [53](../README.md#-how-we-rank "Score 53/100. Adoption: niche (30) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 21k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), Google Cloud account for most skills · [Repo](https://github.com/google/skills) · [🌐 Site ↗](https://skills.sh/google/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/google-skills/)</sub>

<a name="hallmark"></a>
### #&#8288;50 [hallmark](https://github.com/nutlope/hallmark) <sub>score [51](../README.md#-how-we-rank "Score 51/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: weak (20) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Aug 2026</sub>

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

<a name="security-audit-skill"></a>
### #&#8288;51 [security-audit-skill](https://github.com/cloudflare/security-audit-skill) <sub>score [50](../README.md#-how-we-rank "Score 50/100. Adoption: known (50) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Sep 2026</sub>

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

<a name="codex-plugin-cc"></a>
### #&#8288;52 [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: popular (57) · Freshness: active (98) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Jul 2026</sub>

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

<a name="frontend-slides"></a>
### #&#8288;53 [frontend-slides](https://github.com/zarazhangrui/frontend-slides) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: popular (52) · Freshness: active (94) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Jun 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
