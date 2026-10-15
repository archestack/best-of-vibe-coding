# ⌨️ Editors and IDEs reviews · Best of Vibe Coding

Code editors with AI built in, open source and runnable on your own machine. Back to the [leaderboard](../README.md#%EF%B8%8F-editors-and-ides).

<sub>🌐 Also on the web: [Editors and IDEs on archestack.com](https://archestack.com/best-of-vibe-coding/editors/), each project on its own page.</sub>

<a name="avante-nvim"></a>
### 🥇 [avante.nvim](https://github.com/avante-corp/avante.nvim) <sub>score [72](../README.md#-how-we-rank "Score 72/100. Adoption: widely used (84) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

**Neovim plugin that adds Cursor-style AI chat and code edits inside the editor.**

avante.nvim is a Lua Neovim plugin with a Rust-built component. It opens a chat sidebar that answers questions about the current file and applies suggested changes to source files. It supports an agentic mode with tools, ACP agents such as codex and gemini, and many model providers. A per-project avante.md file supplies instructions.

- **+** Runs inside Neovim; suggested changes can be applied to files with one command
- **+** Supports many providers: openai, anthropic, mistral, deepseek, ollama, llama-cpp, copilot
- **+** ACP support lets external agents like codex and gemini drive edits
- **+** Project-level avante.md instructions file; optional local RAG service
- **−** Requires Neovim 0.11+ (badge says 0.12+); README is inconsistent on version
- **−** Install needs a build step: make with curl and tar, or cargo to build from source
- **−** Auto-suggestions are marked experimental and costly because of high request frequency
- **−** Tool permissions are auto-approved by default (auto_approve_tool_permissions = true)

<sub>no GPU · Needs Neovim 0.11+, plenary.nvim, nui.nvim, mega.cmdparse, curl and tar, or cargo, provider API key or local model server · Models: claude, openai, azure, gemini, cohere · [Repo](https://github.com/avante-corp/avante.nvim) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/avante-nvim/)</sub>

<a name="terax-ai"></a>
### 🥈 [terax-ai](https://github.com/crynta/terax-ai) <sub>score [65](../README.md#-how-we-rank "Score 65/100. Adoption: popular (52) · Freshness: active (100) · Maintenance: fair (59) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.3k · Apache-2.0 · Oct 2026</sub>

**Terminal-first desktop workspace with editor, git panel and agentic AI side-panel.**

Terax is a desktop app built on Tauri 2, Rust and React 19 that combines a PTY terminal, CodeMirror editor, file explorer, git graph and web preview. Its AI side-panel runs agents with approval-gated bash and file edits against your own API keys or local Ollama, LM Studio and MLX models. About 7-8 MB on disk, with no telemetry or account.

- **+** Many BYOK providers plus Ollama, LM Studio and MLX for local models
- **+** API keys go to the OS keychain; no telemetry or account
- **+** AI edit diffs can be accepted or rejected hunk by hunk
- **+** Runs on macOS, Linux and Windows, with WSL workspaces
- **−** README says v0.9.0 will replace xterm.js with libghostty and WebGPU, so internals will change
- **−** Language server support is opt-in and needs configuration
- **−** Desktop install only; no Docker or server mode
- **−** Author notes development time went to another product (Zephium)

<sub>GPU optional · Needs Rust (build from source), Node 22+ and pnpm (build from source), Tauri platform prerequisites (build from source) · Models: OpenAI, Anthropic, Google Gemini, Groq, xAI · [Repo](https://github.com/crynta/terax-ai) · [📖 Docs ↗](https://terax.app/docs) · [🌐 Site ↗](https://terax.app) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/terax-ai/)</sub>

<a name="bb"></a>
### 🥉 [bb](https://github.com/get-bb/bb) <sub>score [62](../README.md#-how-we-rank "Score 62/100. Adoption: niche (14) · Freshness: active (100) · Maintenance: healthy (87) · Easy to run: easy (50) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 4.3k · MIT · Oct 2026</sub>

**Agentic IDE with desktop app, web app, CLI and HTTP API.**

bb is an agentic IDE written in TypeScript that runs work in threads you can follow live, steer, or hand off to another agent. It is driven through an Electron desktop app, a web UI on port 38886, a `bb` CLI or an HTTP API, and it uses the provider CLI you have already authenticated. It is marked as in active development, with workflows still changing.

- **+** Same functionality across desktop app, web app, CLI and HTTP API
- **+** Starts with one command: `npx bb-app@latest`
- **+** Reuses your already authenticated provider CLI instead of separate API setup
- **+** Opt-out telemetry (`BB_TELEMETRY=false`) that the README says excludes message content
- **−** Desktop app supports only Apple Silicon macOS; Linux and Windows builds are alpha
- **−** README says workflows and surfaces are still evolving
- **−** Server API is unauthenticated and permits command execution; remote modes need a trusted network
- **−** Native add-ons need install scripts allowed on npm 12 or later

<sub>Needs Node.js, npm, authenticated provider CLI, Git for Windows (native Windows) · Models: provider CLIs (unspecified) · port 38886 · [Repo](https://github.com/get-bb/bb) · [📖 Docs ↗](https://github.com/get-bb/bb/blob/main/docs/configuration.md) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/bb/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
