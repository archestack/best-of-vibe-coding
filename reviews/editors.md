# ⌨️ Editors and IDEs reviews · Best of Vibe Coding

Code editors with AI built in, open source and runnable on your own machine. Back to the [leaderboard](../README.md#%EF%B8%8F-editors-and-ides).

<sub>🌐 Also on the web: [Editors and IDEs on archestack.com](https://archestack.com/best-of-vibe-coding/editors/), each project on its own page.</sub>

<a name="avante-nvim"></a>
### 🥇 [avante.nvim](https://github.com/avante-corp/avante.nvim) <sub>score [70](../README.md#-how-we-rank "Score 70/100. Adoption: popular (74) · Freshness: active (100) · Maintenance: healthy (85) · Easy to run: easy (50) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 18k · Apache-2.0 · Oct 2026</sub>

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

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
