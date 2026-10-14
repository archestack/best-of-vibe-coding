# 🧩 Skills, plugins and rules reviews · Best of Vibe Coding

Add-ons that make coding agents better: skills, plugins, rules, hooks and memory for Claude Code, Codex, Cursor and others. Back to the [leaderboard](../README.md#-skills-plugins-and-rules).

<sub>🌐 Also on the web: [Skills, plugins and rules on archestack.com](https://archestack.com/best-of-vibe-coding/skills-plugins/), each project on its own page.</sub>

<a name="skills"></a>
### 🥇 [skills](https://github.com/mattpocock/skills) <sub>score [94](../README.md#-how-we-rank "Score 94/100. Adoption: widely used (99) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 290k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Issue tracker (GitHub, GitLab or local files) · Models: Any model (per README) · safety checks passed 9 of 10 · [Repo](https://github.com/mattpocock/skills) · [🌐 Site ↗](https://skills.sh/mattpocock/skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/skills/)</sub>

<a name="ecc"></a>
### 🥈 [ecc](https://github.com/affaan-m/ecc) <sub>score [93](../README.md#-how-we-rank "Score 93/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 279k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 18+, Git, Claude Code 2.1+ (for plugin setup) · Models: Claude Code, Codex, Kimi Code, Cursor, OpenCode · safety checks passed 10 of 10 · [Repo](https://github.com/affaan-m/ecc) · [🌐 Site ↗](https://ecc.tools) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ecc/)</sub>

<a name="caveman"></a>
### 🥉 [caveman](https://github.com/juliusbrussee/caveman) <sub>score [92](../README.md#-how-we-rank "Score 92/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 111k · Apache-2.0 · Oct 2026</sub>

**Proxy and skill that cut token use in coding agents.**

Caveman has two parts. A local proxy compresses what coding agents read (logs, CSV, YAML, JSON, test output, web pages), and a skill makes the agent reply in terse, answer-first text while code, paths and numbers stay verbatim. It works with Claude Code, Codex, Gemini CLI, Aider and 30+ other agents, and ships SDK middleware for the Vercel AI SDK, LangChain, OpenAI and Anthropic.

- **+** Proxy cut whole-session input tokens 33.2% in its own 54-run Claude Code benchmark
- **+** Skill-only install via `npx skills add`, no proxy needed
- **+** README lists losing cases: HTML got 9.9% worse, and the per-request billing caveat
- **+** TypeScript and Python middleware wraps existing LLM SDK calls
- **−** No HTML compressor yet; the benchmark HTML session used more tokens
- **−** CLI sends usage telemetry by default; opt out with `caveman telemetry off`
- **−** Proxy needs Node.js 22.13+
- **−** Skill rules add about 1,160 tokens; cost impact with caching not measured

<sub>no GPU · Docker + Compose · Needs Node.js 22.13+, Python 3.11+ (middleware only) · Models: Claude Code, Codex, Gemini CLI, Aider, Cursor · safety checks passed 8 of 10 · [Repo](https://github.com/juliusbrussee/caveman) · [📖 Docs ↗](https://docs.caveman.so) · [🌐 Site ↗](https://caveman.so) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/caveman/)</sub>

<a name="ponytail"></a>
### #&#8288;4 [ponytail](https://github.com/dietrichgebert/ponytail) <sub>score [91](../README.md#-how-we-rank "Score 91/100. Adoption: widely used (95) · Freshness: active (100) · Maintenance: healthy (99) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 163k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs A supported coding agent such as Claude Code or Codex · Models: Benchmarked with Opus 5.5 in Claude Code · safety checks passed 8 of 9 · [Repo](https://github.com/dietrichgebert/ponytail) · [🌐 Site ↗](https://ponytail.dev/stories) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ponytail/)</sub>

<a name="spec-kit"></a>
### #&#8288;5 [spec-kit](https://github.com/github/spec-kit) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (91) · Freshness: active (100) · Maintenance: healthy (95) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 141k · MIT · Oct 2026</sub>

**CLI and agent skills for spec-driven development, bug fixing and idea assessment.**

Spec Kit is a Python CLI (`specify`) that installs templates and slash-command skills into a project so a coding agent follows a fixed process. It ships spec-driven development in core (constitution, specify, plan, tasks, implement, converge). Bug fixing and idea assessment are opt-in extensions that write reports under `.specify/`.

- **+** Works with multiple coding agents via an integration key, e.g. `--integration copilot`
- **+** Process outputs are Markdown artifacts stored in the repo under `.specify/`
- **+** Bug-fix flow separates assess, fix and test, ending in a verified, partial or failed verdict
- **+** Extensions, presets, workflows and bundles let you customize or replace processes
- **−** Needs Python 3.11+ and uv installed
- **−** Skills run in the agent's chat, not the terminal; syntax varies by agent
- **−** Bug fixing and assessment require a separate `specify extension add` step
- **−** Provides no model or agent itself; a supported coding agent is required

<sub>no GPU · Needs Python 3.11+, uv, a supported AI coding agent · safety checks passed 8 of 8 · [Repo](https://github.com/github/spec-kit) · [📖 Docs ↗](https://github.github.io/spec-kit/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/spec-kit/)</sub>

<a name="ui-ux-pro-max-skill"></a>
### #&#8288;6 [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <sub>score [89](../README.md#-how-we-rank "Score 89/100. Adoption: widely used (88) · Freshness: active (100) · Maintenance: healthy (91) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 136k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Python 3, Node.js/npm (for the uipro CLI) · Models: Claude Code, Cursor, Windsurf, Codex CLI, Gemini CLI · safety checks passed 9 of 9 · [Repo](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) · [🌐 Site ↗](https://uupm.cc) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ui-ux-pro-max-skill/)</sub>

<a name="superpowers"></a>
### #&#8288;7 [superpowers](https://github.com/obra/superpowers) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (100) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 299k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs A supported coding agent (Claude Code, Codex, Cursor, Gemini CLI, etc.) · Models: Claude Code, Codex, Cursor, Gemini CLI, GitHub Copilot CLI · safety checks passed 8 of 8 · [Repo](https://github.com/obra/superpowers) · [🌐 Site ↗](https://primeradiant.com/superpowers/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/superpowers/)</sub>

<a name="agent-skills"></a>
### #&#8288;8 [agent-skills](https://github.com/addyosmani/agent-skills) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (83) · Freshness: active (100) · Maintenance: healthy (87) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 106k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), An AI coding agent such as Claude Code, Codex or Gemini CLI · safety checks passed 8 of 9 · [Repo](https://github.com/addyosmani/agent-skills) · [📖 Docs ↗](https://github.com/addyosmani/agent-skills/blob/main/docs/getting-started.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agent-skills/)</sub>

<a name="claude-mem"></a>
### #&#8288;9 [claude-mem](https://github.com/thedotmack/claude-mem) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: widely used (81) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 100k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Docker + Compose · Needs Node.js 20+, Bun, uv, SQLite, Chroma · Models: Anthropic plan, OpenRouter, Gemini, claude-mem hosted observer · safety checks passed 8 of 9 · [Repo](https://github.com/thedotmack/claude-mem) · [📖 Docs ↗](https://docs.claude-mem.ai/) · [🌐 Site ↗](https://docs.claude-mem.ai/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-mem/)</sub>

<a name="impeccable"></a>
### #&#8288;10 [impeccable](https://github.com/pbakaus/impeccable) <sub>score [88](../README.md#-how-we-rank "Score 88/100. Adoption: popular (73) · Freshness: active (100) · Maintenance: healthy (93) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 81k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (only for npx installer), impeccable.style roll API · Models: Claude Code, Cursor, Codex CLI, Gemini CLI, GitHub Copilot · safety checks passed 9 of 10 · [Repo](https://github.com/pbakaus/impeccable) · [▶️ Demo ↗](https://impeccable.style/cases/neo-mirai) · [📖 Docs ↗](https://impeccable.style) · [🌐 Site ↗](https://impeccable.style) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/impeccable/)</sub>

<a name="graphify"></a>
### #&#8288;11 [graphify](https://github.com/graphify-labs/graphify) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: widely used (86) · Freshness: active (100) · Maintenance: healthy (85) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 126k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Python 3.10+, uv or pipx, AI coding assistant · Models: Anthropic Claude, OpenAI and compatible APIs, Google Gemini, AWS Bedrock, Azure OpenAI · safety checks passed 12 of 13 · [Repo](https://github.com/graphify-labs/graphify) · [📖 Docs ↗](https://docs.graphify.com) · [🌐 Site ↗](https://graphify.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/graphify/)</sub>

<a name="archify"></a>
### #&#8288;12 [archify](https://github.com/tt-a1i/archify) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (75) · Freshness: active (100) · Maintenance: healthy (82) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 83k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js (npx), Cursor, Claude Code, Codex CLI or OpenCode · Models: unknown (uses the host agent's model) · safety checks passed 8 of 8 · [Repo](https://github.com/tt-a1i/archify) · [▶️ Demo ↗](https://archify.si/gallery.html) · [📖 Docs ↗](https://archify.si/guide.html) · [🌐 Site ↗](https://archify.si) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/archify/)</sub>

<a name="ruflo"></a>
### #&#8288;13 [ruflo](https://github.com/ruvnet/ruflo) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (72) · Freshness: active (100) · Maintenance: healthy (81) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 75k · MIT · Oct 2026</sub>

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

<sub>Needs Node.js/npx, Claude Code 2.1.287+ (for plugins) · Models: Claude Code, Codex, Ollama (via ruflo-ruvllm plugin) · safety checks passed 12 of 14 · [Repo](https://github.com/ruvnet/ruflo) · [▶️ Demo ↗](https://raw.githubusercontent.com/ruvnet/ruflo/main/docs/assets/ruflo-console-theme-compact.svg) · [📖 Docs ↗](https://github.com/ruvnet/ruflo/blob/main/docs/USERGUIDE.md) · [🌐 Site ↗](https://cognitum.one/agentic-engineering) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/ruflo/)</sub>

<a name="oh-my-claudecode"></a>
### #&#8288;14 [oh-my-claudecode](https://github.com/yeachan-heo/oh-my-claudecode) <sub>score [84](../README.md#-how-we-rank "Score 84/100. Adoption: popular (56) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 40k · MIT · Oct 2026</sub>

**Multi-agent orchestration plugin for Claude Code with staged team pipelines.**

oh-my-claudecode adds skills, slash commands and an `omc` CLI to Claude Code. It runs in-session workflows such as /autopilot, /ralph, /deep-interview and a staged /team pipeline (plan, PRD, exec, verify, fix). The CLI can also start tmux panes running Codex, Gemini, Antigravity, Grok, Cursor or Claude workers.

- **+** Installs as a Claude Code marketplace plugin or via npm (`oh-my-claude-sisyphus`)
- **+** `omc team` spawns tmux workers for Codex, Gemini, Antigravity, Grok, Cursor and Claude
- **+** Autopilot stage profiles are configurable in `.claude/omc.jsonc`
- **+** MIT license; exports TypeScript helpers such as `createOmcSession()`
- **−** Slash-command workflows need an active Claude Code session; not usable in CI
- **−** Named autopilot profiles require Linux with `flock`
- **−** Native team mode needs an experimental Claude Code env flag
- **−** npm install prints a deprecated `prebuild-install` warning

<sub>no GPU · Needs Claude Code, tmux, Node.js/npm, codex/gemini/agy/grok/cursor-agent CLIs (optional) · Models: Claude, Codex, Gemini, Antigravity, Grok · safety checks passed 9 of 10 · [Repo](https://github.com/yeachan-heo/oh-my-claudecode) · [📖 Docs ↗](https://yeachan-heo.github.io/oh-my-claudecode-website/docs/) · [🌐 Site ↗](https://yeachan-heo.github.io/oh-my-claudecode-website) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/oh-my-claudecode/)</sub>

<a name="cc-switch"></a>
### #&#8288;15 [cc-switch](https://github.com/farion1231/cc-switch) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (92) · Freshness: active (100) · Maintenance: healthy (86) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 144k · MIT · Oct 2026</sub>

**Desktop app that switches API providers for coding agents and manages their MCP and skills.**

CC Switch is a Tauri 2 desktop app written in Rust for Windows, macOS and Linux. It switches API providers for Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build, OpenCode, OpenClaw, Hermes Agent, Pi and MiniMax Code. It also manages MCP servers, Skills and Prompts in one place, so JSON, TOML and YAML configs need no hand-editing.

- **+** Covers ten coding agents and CLIs from one provider switcher
- **+** Manages MCP servers, Skills and Prompts alongside provider settings
- **+** Native desktop builds for Windows, macOS and Linux via Tauri 2
- **+** MIT license, with a user manual and translated READMEs
- **−** README opens with a long list of API relay sponsors and referral links
- **−** Desktop GUI only; no Docker image or headless mode detected
- **−** Part of the README was truncated, so install and feature details are unverified
- **−** System requirements such as minimum RAM are unknown

<sub>no GPU · Models: Claude Code, Claude Desktop, Codex, Gemini CLI, Grok Build · safety checks passed 4 of 5 · [Repo](https://github.com/farion1231/cc-switch) · [🌐 Site ↗](https://ccswitch.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/cc-switch/)</sub>

<a name="gstack"></a>
### #&#8288;16 [gstack](https://github.com/garrytan/gstack) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: widely used (89) · Freshness: active (100) · Maintenance: fair (64) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 136k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Git, Bun 1.4.2+ (refuses older than 1.3.3), Node.js (Windows only), Codex CLI (optional, outside reviews), OpenAI API key (optional, design tools) · Models: Claude (via Claude Code), OpenAI Codex models, OpenAI gpt-5.5 and gpt-image-2 (design binary) · safety checks passed 8 of 9 · [Repo](https://github.com/garrytan/gstack) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/gstack/)</sub>

<a name="rtk"></a>
### #&#8288;17 [rtk](https://github.com/rtk-ai/rtk) <sub>score [83](../README.md#-how-we-rank "Score 83/100. Adoption: popular (76) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 83k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Models: Claude Code, Gemini CLI, Codex, Cursor, Windsurf · safety checks passed 8 of 9 · [Repo](https://github.com/rtk-ai/rtk) · [📖 Docs ↗](https://www.rtk-ai.app/guide/troubleshooting) · [🌐 Site ↗](https://www.rtk-ai.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/rtk/)</sub>

<a name="openspec"></a>
### #&#8288;18 [openspec](https://github.com/fission-ai/openspec) <sub>score [82](../README.md#-how-we-rank "Score 82/100. Adoption: popular (70) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 72k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js 20.19.0+, an AI coding assistant · Models: Codex 5.5 and Opus 4.7 recommended; works with 30+ AI coding tools · safety checks passed 8 of 9 · [Repo](https://github.com/fission-ai/openspec) · [📖 Docs ↗](https://github.com/Fission-AI/OpenSpec/blob/main/docs/README.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/openspec/)</sub>

<a name="agentic-awesome-skills"></a>
### #&#8288;19 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (62) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 48k · MIT · Oct 2026</sub>

**Library of 2,671+ SKILL.md playbooks for coding agents, with a local MCP selector.**

A repository of installable SKILL.md instruction files for coding agents, plus AAS Core, a local MCP and `aas` CLI that lets Codex or Claude search the catalog, record chosen skills in aas-stack.json, and preview a plan. A separate npm installer copies selected skills into host directories for Cursor, Gemini CLI, Kiro, OpenCode and others. Core does not rank or recommend skills, and apply and recovery are experimental.

- **+** 2,671+ skills, searchable via skills_index.json and a hosted catalog
- **+** Installer targets Claude Code, Cursor, Codex, Gemini CLI, Kiro, OpenCode and Copilot
- **+** Installer supports --dry-run and filters by skill ID, category, tags and risk
- **+** MIT license; Core stack validate and plan preview are read-only
- **−** Core apply and recovery are experimental; supported preview stops at plan review
- **−** Core setup guides cover only Codex and Claude; other hosts use direct install
- **−** Too many installed skills can overload Antigravity's context
- **−** Validation checks structure only, not whether a skill fits or is safe

<sub>no GPU · Needs Node.js/npm · safety checks passed 7 of 10 · [Repo](https://github.com/sickn33/agentic-awesome-skills) · [▶️ Demo ↗](https://aaskills.tech/workbench) · [📖 Docs ↗](https://github.com/sickn33/agentic-awesome-skills/blob/v19.2.0/docs/users/aas-core.md) · [🌐 Site ↗](https://aaskills.tech/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentic-awesome-skills/)</sub>

<a name="book-to-skill"></a>
### #&#8288;20 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) <sub>score [81](../README.md#-how-we-rank "Score 81/100. Adoption: popular (51) · Freshness: active (100) · Maintenance: healthy (96) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

**Converts books and document folders into on-demand skills for coding agents.**

A Python extractor turns PDF, EPUB, DOCX, Markdown, HTML, RTF or MOBI files into clean text, and the host agent follows SKILL.md to generate a skill. The output is a core SKILL.md, per-chapter files, a glossary, patterns and a cheatsheet, written to ~/.agents/skills/<slug>/. Works with hosts that read the Agent Skills format, including Claude Code, Copilot CLI, Amp, Hermes Agent, OpenCode and OpenClaw.

- **+** Chapter files load on demand; SKILL.md is about 4,000 tokens
- **+** Reads PDF, EPUB, DOCX, HTML, RTF, MOBI, Markdown and plain text
- **+** One skill folder is discovered by several agent hosts
- **+** Reports 24x-51x fewer tokens than putting the book in context
- **−** Scanned PDFs need OCR first (e.g. ocrmypdf); extraction stops otherwise
- **−** MOBI/AZW input requires Calibre's ebook-convert, installed separately
- **−** Skill generation is done by the host agent's model, so quality varies
- **−** Sharing skills made from copyrighted books may infringe the rights holder

<sub>no GPU · Needs Python 3, pdftotext (poppler), docling, ebooklib, beautifulsoup4, Calibre ebook-convert, ocrmypdf · safety checks passed 8 of 8 · [Repo](https://github.com/virgiliojr94/book-to-skill) · [📖 Docs ↗](https://github.com/virgiliojr94/book-to-skill/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/book-to-skill/)</sub>

<a name="taste-skill"></a>
### #&#8288;21 [taste-skill](https://github.com/leonxlnx/taste-skill) <sub>score [79](../README.md#-how-we-rank "Score 79/100. Adoption: popular (80) · Freshness: active (100) · Maintenance: healthy (83) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 96k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs npx skills CLI, Codex, Cursor or Claude Code, ChatGPT Images or similar (image skills only) · Models: Codex, Claude Code, Cursor, ChatGPT · safety checks passed 7 of 8 · [Repo](https://github.com/leonxlnx/taste-skill) · [🌐 Site ↗](https://tasteskill.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/taste-skill/)</sub>

<a name="repomix"></a>
### #&#8288;22 [repomix](https://github.com/yamadashy/repomix) <sub>score [78](../README.md#-how-we-rank "Score 78/100. Adoption: known (40) · Freshness: active (100) · Maintenance: healthy (92) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Oct 2026</sub>

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

<sub>no GPU · Docker · Needs Node.js · Models: Model-agnostic: output is a file for Claude, ChatGPT, Gemini, Llama, Grok and others · [Repo](https://github.com/yamadashy/repomix) · [▶️ Demo ↗](https://repomix.com) · [🌐 Site ↗](https://repomix.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/repomix/)</sub>

<a name="claude-hud"></a>
### #&#8288;23 [claude-hud](https://github.com/jarrodwatts/claude-hud) <sub>score [75](../README.md#-how-we-rank "Score 75/100. Adoption: known (38) · Freshness: active (100) · Maintenance: healthy (100) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Node.js · Models: Claude, Bedrock, Vertex, MiniMax · [Repo](https://github.com/jarrodwatts/claude-hud) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-hud/)</sub>

<a name="agents"></a>
### #&#8288;24 [agents](https://github.com/wshobson/agents) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: popular (58) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 41k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Codex CLI, Cursor, OpenCode, Antigravity CLI, GitHub Copilot or Pi, uv and Python 3.12+ (clone installs), GitHub CLI 2.90+ or Node.js/npm (skills-only installers) · Models: opus, sonnet, haiku, fable, inherit (aliases mapped per harness) · safety checks passed 8 of 9 · [Repo](https://github.com/wshobson/agents) · [📖 Docs ↗](https://github.com/wshobson/agents/blob/main/docs/usage.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agents/)</sub>

<a name="vercel-labs-skills"></a>
### #&#8288;25 [skills](https://github.com/vercel-labs/skills) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (50) · Freshness: active (100) · Maintenance: healthy (84) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 35k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js, npx, git · [Repo](https://github.com/vercel-labs/skills) · [🌐 Site ↗](https://skills.sh) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/vercel-labs-skills/)</sub>

<a name="planning-with-files"></a>
### #&#8288;26 [planning-with-files](https://github.com/othmanadi/planning-with-files) <sub>score [73](../README.md#-how-we-rank "Score 73/100. Adoption: known (30) · Freshness: active (100) · Maintenance: healthy (98) · Agent-ready: minimal (45) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Bash, Python 3.10+ (Qoder CLI), Node.js/npx (installer) · [Repo](https://github.com/othmanadi/planning-with-files) · [📖 Docs ↗](https://github.com/OthmanAdi/planning-with-files/blob/master/docs/installation.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/planning-with-files/)</sub>

<a name="agency-agents"></a>
### #&#8288;27 [agency-agents](https://github.com/msitarzewski/agency-agents) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (94) · Freshness: active (100) · Maintenance: patchy (46) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 160k · MIT · Oct 2026</sub>

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

<sub>no GPU · safety checks passed 8 of 8 · [Repo](https://github.com/msitarzewski/agency-agents) · [🌐 Site ↗](https://agencyagents.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agency-agents/)</sub>

<a name="beads"></a>
### #&#8288;28 [beads](https://github.com/gastownhall/beads) <sub>score [71](../README.md#-how-we-rank "Score 71/100. Adoption: known (32) · Freshness: active (100) · Maintenance: fair (75) · Agent-ready: ready (85) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Dolt (embedded by default; external dolt sql-server for server mode), git remote (optional, for sync) · [Repo](https://github.com/gastownhall/beads) · [📖 Docs ↗](https://beads.gascity.com/) · [🌐 Site ↗](https://beads.gascity.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/beads/)</sub>

<a name="understand-anything"></a>
### #&#8288;29 [understand-anything](https://github.com/egonex-ai/understand-anything) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (78) · Freshness: active (100) · Maintenance: patchy (44) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 86k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code or another supported agent platform, Node.js >= 18 (standalone viewer), pnpm (building from source) · Models: Whatever the host platform uses, Local models via Ollama · port 5173 · safety checks passed 8 of 10 · [Repo](https://github.com/egonex-ai/understand-anything) · [▶️ Demo ↗](https://understand-anything.com/demo/) · [🌐 Site ↗](https://understand-anything.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/understand-anything/)</sub>

<a name="claude-code-best-practice"></a>
### #&#8288;30 [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (68) · Freshness: active (100) · Maintenance: patchy (47) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 68k · MIT · Oct 2026</sub>

**Reference repo of Claude Code configs, guides, and workflow examples.**

A documentation-first repository that catalogs Claude Code features (subagents, commands, skills, hooks, MCP servers, settings, memory, plugins) with written guidance and working examples under `.claude/`. It includes a Command → Agent → Skill orchestration demo run with `/weather-orchestrator`, plus a comparison table of community development workflows such as Superpowers, Spec Kit and gstack.

- **+** Each feature links to both a written guide and a working implementation in the repo
- **+** Runnable orchestration example: Command → Agent → Skill via `/weather-orchestrator`
- **+** Compares community workflows with agent, command and skill counts per project
- **+** MIT license; plain markdown and config files, no services to run
- **−** Covers Claude Code only; other coding agents are not the focus
- **−** Not installable software; it is reference material to read and copy from
- **−** Many listed features are marked beta and may change
- **−** Workflow table figures such as star counts are snapshots that go stale

<sub>no GPU · Needs Claude Code · Models: Claude · safety checks passed 6 of 7 · [Repo](https://github.com/shanraisshan/claude-code-best-practice) · [📖 Docs ↗](https://code.claude.com/docs) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-best-practice/)</sub>

<a name="claude-howto"></a>
### #&#8288;31 [claude-howto](https://github.com/luongnv89/claude-howto) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (59) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 42k · MIT · Oct 2026</sub>

**Tutorials and copy-paste templates for Claude Code features.**

A Markdown guide with 10 modules covering Claude Code slash commands, memory, skills, subagents, MCP, hooks, plugins, checkpoints, advanced features and the CLI. Each module ships templates to copy into .claude/ or ~/.claude/, plus Mermaid diagrams. The README estimates 11-13 hours for the full path and includes quiz commands, /self-assessment and /lesson-quiz.

- **+** Templates copy directly into .claude/commands, .claude/agents and ~/.claude/skills
- **+** Ordered learning path with per-module time estimates
- **+** MIT licensed; README says it is synced with Claude Code releases
- **+** Covers hooks, MCP, subagents and plugins in one place
- **−** Documentation and templates only; no runnable application or service
- **−** Tied to Claude Code; templates are not portable to other coding agents
- **−** Docker support and a hosted demo are not provided
- **−** README leans on promotional claims such as 10x productivity, unsupported by evidence

<sub>no GPU · Needs Claude Code, Node.js (npx for MCP server examples) · Models: Claude · safety checks passed 9 of 9 · [Repo](https://github.com/luongnv89/claude-howto) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-howto/)</sub>

<a name="i-have-adhd"></a>
### #&#8288;32 [i-have-adhd](https://github.com/ayghri/i-have-adhd) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: popular (66) · Freshness: active (100) · Maintenance: fair (55) · Agent-ready: minimal (30) (each out of 100, weighted). Click for how we rank.") · ⭐ 57k · MIT · Oct 2026</sub>

**Skill that makes coding assistants answer with the next action first.**

A skill/plugin for coding assistants that rewrites response style around ten rules: lead with the next action, number multi-step tasks, cap lists at 5 items, and drop preambles, recaps and closers. It installs through Claude's plugin commands and is tuned by editing skills/i-have-adhd/SKILL.md in a fork. The README's before/after example turns a long auth-flow explanation into three numbered steps.

- **+** Ten explicit rules, documented in a single editable SKILL.md
- **+** Fork-and-swap workflow documented with Claude plugin commands
- **+** Before/after example shows the exact change in output style
- **+** MIT license; README translated into nine other languages
- **−** Install and tuning steps are documented only for Claude plugin commands
- **−** No tagged releases
- **−** Changes response style only; no measured effect on answer quality is given
- **−** Hard rules like the 5-item list cap may cut detail you need

<sub>no GPU · safety checks passed 8 of 9 · [Repo](https://github.com/ayghri/i-have-adhd) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/i-have-adhd/)</sub>

<a name="claude-code-templates"></a>
### #&#8288;33 [claude-code-templates](https://github.com/davila7/claude-code-templates) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (47) · Freshness: active (100) · Maintenance: fair (69) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 33k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Node.js/npx, Claude Code, Cloudflare Tunnel (optional, for remote chat monitor) · safety checks passed 5 of 10 · [Repo](https://github.com/davila7/claude-code-templates) · [📖 Docs ↗](https://docs.aitmpl.com) · [🌐 Site ↗](https://aitmpl.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-templates/)</sub>

<a name="diagram-design"></a>
### #&#8288;34 [diagram-design](https://github.com/cathrynlavery/diagram-design) <sub>score [68](../README.md#-how-we-rank "Score 68/100. Adoption: popular (64) · Freshness: active (100) · Maintenance: fair (62) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 54k · MIT · Oct 2026</sub>

**Agent skill that generates editorial HTML/SVG diagrams in your site's style.**

Diagram Design is an Agent Skill, installable as a plugin for Claude Code, Codex, GitHub Copilot, Factory Droid and Pi, that generates diagrams as self-contained HTML and SVG with no build step or JavaScript. It covers more than 40 diagram types, each in minimal light, minimal dark and full-editorial variants, and can match your brand by reading your website. It can also redraw draw.io, Mermaid or Excalidraw sources.

- **+** Output is static HTML and SVG, openable in a browser with no build step
- **+** Over 40 diagram types, each with light, dark and full-editorial variants
- **+** Installs through marketplaces for Claude Code, Codex, Copilot, Droid and Pi
- **+** Imports Mermaid and Excalidraw sources, with export and doctor commands
- **−** Needs an Agent Skills-compatible host; no standalone app or CLI generator
- **−** Attribute-only comparisons are not drawn; the README says to use tables
- **−** Standalone `npx skills` install does not auto-update and omits the command surfaces
- **−** OpenCode has no marketplace package; updates mean replacing the copied directory

<sub>no GPU · safety checks passed 9 of 9 · [Repo](https://github.com/cathrynlavery/diagram-design) · [▶️ Demo ↗](https://cathrynlavery.github.io/diagram-design/) · [🌐 Site ↗](https://diagramdesign.dev) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/diagram-design/)</sub>

<a name="claude-skills"></a>
### #&#8288;35 [claude-skills](https://github.com/alirezarezvani/claude-skills) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: known (34) · Freshness: active (100) · Maintenance: fair (70) · Agent-ready: minimal (40) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · MIT · Aug 2026</sub>

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

<sub>no GPU · Needs Python 3, Claude Code or another supported coding agent · [Repo](https://github.com/alirezarezvani/claude-skills) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-skills/)</sub>

<a name="claude-code-game-studios"></a>
### #&#8288;36 [claude-code-game-studios](https://github.com/donchitos/claude-code-game-studios) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (28) · Freshness: active (100) · Maintenance: fair (59) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · MIT · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code, Git, Python 3, Bash, jq (recommended) · Models: Claude (Opus, Sonnet, or session model) · [Repo](https://github.com/donchitos/claude-code-game-studios) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-code-game-studios/)</sub>

<a name="claude-plugins-official"></a>
### #&#8288;37 [claude-plugins-official](https://github.com/anthropics/claude-plugins-official) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (54) · Freshness: active (100) · Maintenance: patchy (36) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · Apache-2.0 · Oct 2026</sub>

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

<sub>no GPU · Needs Claude Code · safety checks passed 6 of 9 · [Repo](https://github.com/anthropics/claude-plugins-official) · [📖 Docs ↗](https://code.claude.com/docs/en/plugins) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/claude-plugins-official/)</sub>

<a name="agentskills"></a>
### #&#8288;38 [agentskills](https://github.com/agentskills/agentskills) <sub>score [56](../README.md#-how-we-rank "Score 56/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: patchy (38) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 26k · Apache-2.0 · Aug 2026</sub>

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

<sub>no GPU · [Repo](https://github.com/agentskills/agentskills) · [📖 Docs ↗](https://agentskills.io/specification) · [🌐 Site ↗](https://agentskills.io) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/agentskills/)</sub>

<a name="design-md"></a>
### #&#8288;39 [design.md](https://github.com/google-labs-code/design.md) <sub>score [55](../README.md#-how-we-rank "Score 55/100. Adoption: known (36) · Freshness: active (100) · Maintenance: patchy (49) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 28k · Apache-2.0 · Jul 2026</sub>

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

<sub>no GPU · Needs Node.js, npm · [Repo](https://github.com/google-labs-code/design.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/design-md/)</sub>

<a name="hallmark"></a>
### #&#8288;40 [hallmark](https://github.com/nutlope/hallmark) <sub>score [48](../README.md#-how-we-rank "Score 48/100. Adoption: known (43) · Freshness: active (100) · Maintenance: weak (19) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 30k · MIT · Aug 2026</sub>

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

<sub>no GPU · Needs Claude Code, Cursor or Codex, npx · [Repo](https://github.com/nutlope/hallmark) · [▶️ Demo ↗](https://www.usehallmark.com) · [🌐 Site ↗](https://www.usehallmark.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/hallmark/)</sub>

<a name="security-audit-skill"></a>
### #&#8288;41 [security-audit-skill](https://github.com/cloudflare/security-audit-skill) <sub>score [47](../README.md#-how-we-rank "Score 47/100. Adoption: known (41) · Freshness: active (100) · Maintenance: weak (16) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 29k · MIT · Sep 2026</sub>

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

<sub>no GPU · Needs Node.js, Skills CLI (npx skills), coding agent with parallel sub-agents, OS-enforced sandbox · Models: any tool-use model with parallel sub-agents · [Repo](https://github.com/cloudflare/security-audit-skill) · [🌐 Site ↗](https://blog.cloudflare.com/build-your-own-vulnerability-harness) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/security-audit-skill/)</sub>

<a name="codex-plugin-cc"></a>
### #&#8288;42 [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: known (48) · Freshness: active (98) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 34k · Apache-2.0 · Jul 2026</sub>

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

<sub>no GPU · Needs Claude Code, Codex CLI (@openai/codex), Node.js 18.18+, ChatGPT account or OpenAI API key · Models: OpenAI Codex models (e.g. gpt-5.4-mini, gpt-5.3-codex-spark) · safety checks passed 9 of 10 · [Repo](https://github.com/openai/codex-plugin-cc) · [📖 Docs ↗](https://developers.openai.com/codex/app-server) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/codex-plugin-cc/)</sub>

<a name="frontend-slides"></a>
### #&#8288;43 [frontend-slides](https://github.com/zarazhangrui/frontend-slides) <sub>score [43](../README.md#-how-we-rank "Score 43/100. Adoption: known (44) · Freshness: active (94) · Maintenance: weak (6) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 31k · MIT · Jun 2026</sub>

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

<sub>no GPU · Needs Claude Code or another coding agent, Python (scripts/extract-pptx.py) · Models: Claude Code, Codex, Kimi Code, OpenCode, Gemini CLI · [Repo](https://github.com/zarazhangrui/frontend-slides) · [📖 Docs ↗](https://github.com/zarazhangrui/frontend-slides) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/frontend-slides/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
