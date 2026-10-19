# 🎨 Design to code reviews · Best of Vibe Coding

Tools that turn screenshots, mockups or visual edits into working front-end code. Back to the [leaderboard](../README.md#-design-to-code).

<sub>🌐 Also on the web: [Design to code on archestack.com](https://archestack.com/best-of-vibe-coding/design-to-code/), each project on its own page.</sub>

<a name="screenshot-to-code"></a>
### 🥇 [screenshot-to-code](https://github.com/abi/screenshot-to-code) <sub>score [64](../README.md#-how-we-rank "Score 64/100. Adoption: widely used (97) · Freshness: active (100) · Maintenance: patchy (33) · Easy to run: some setup (33) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 80k · MIT · Oct 2026</sub>

**Turns screenshots and mockups into Tailwind, React or Vue code.**

Takes a screenshot, mockup, Figma export or screen recording and generates HTML with Tailwind or CSS, React, Vue, Bootstrap or Ionic code using Gemini 3, GPT-5.5 or Claude Opus models, with Replicate for image generation and background removal. Runs as a React/Vite frontend on port 5173 and a FastAPI backend on 7001, or via docker-compose. For developers prototyping UIs from designs.

- **+** Six output stacks including React, Vue, Bootstrap and Ionic with Tailwind
- **+** Video mode turns a screen recording into a working prototype (needs Gemini)
- **+** Optional headless Chromium lets the agent render and check its own output
- **+** docker-compose brings up frontend and backend with one env file
- **−** Requires at least one OpenAI, Anthropic or Gemini API key; no bundled local model
- **−** Ollama models are possible but the README calls the results poor quality
- **−** Replicate key must be set in backend/.env, not in the UI
- **−** Docker setup has no hot reload; file changes need a rebuild

<sub>no GPU · Compose · Needs OpenAI, Anthropic or Gemini API key, Replicate API key (optional), Playwright Chromium (optional preview) · Models: Gemini 3 Flash Preview, Gemini 3.1 Pro Preview, GPT-5.5, GPT-5.4 Mini, Claude Opus 4.6/4.8 · port 5173 · [Repo](https://github.com/abi/screenshot-to-code) · [▶️ Demo ↗](https://screenshottocode.com/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/screenshot-to-code/)</sub>

<a name="onlook"></a>
### 🥈 [Onlook](https://github.com/onlook-dev/onlook) <sub>score [57](../README.md#-how-we-rank "Score 57/100. Adoption: popular (63) · Freshness: recent (77) · Maintenance: weak (12) · Easy to run: easy (67) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 27k · Apache-2.0 · Jul 2026</sub>

**Visual editor that edits Next.js and Tailwind apps with AI.**

Browser-based editor that loads a Next.js and Tailwind project into a web container, renders it in an iframe and maps DOM elements back to source so you can drag, restyle and edit visually or through an AI chat. Built on Next.js, tRPC, Supabase, Drizzle and the Vercel AI SDK with OpenRouter for models and CodeSandbox for sandboxes. For designers and front-end developers working on Next.js codebases.

- **+** Edits map directly to code; right-click any element to open its source location
- **+** Branching, checkpoints and a real-time code editor beside the visual canvas
- **+** Apache-2.0 with Dockerfile and compose file for local runs
- **+** Figma-like layers, pages, brand tokens and asset management
- **−** Next.js plus Tailwind only; other frameworks are roadmap items, not supported
- **−** Depends on hosted services: Supabase, OpenRouter, CodeSandbox SDK, Freestyle
- **−** Team comments, MCP support and image references are unchecked roadmap items
- **−** Maintainers are moving to a hosted early-access product; last commit July 2026

<sub>no GPU · Docker + Compose · Needs Supabase (auth, database, storage), OpenRouter API key, CodeSandbox SDK, Bun · Models: OpenRouter-hosted models, Morph Fast Apply, Relace · README: alternative to Lovable, v0, Bolt.new, Replit · [Repo](https://github.com/onlook-dev/onlook) · [▶️ Demo ↗](https://onlook.com) · [📖 Docs ↗](https://docs.onlook.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/onlook/)</sub>

<a name="m3e-canvas"></a>
### 🥉 [m3e-canvas](https://github.com/lnkiai/m3e-canvas) <sub>score [46](../README.md#-how-we-rank "Score 46/100. Adoption: niche (27) · Freshness: active (100) · Maintenance: fair (62) · Easy to run: hard (0) · Agent-ready: partly (70) (each out of 100, weighted). Click for how we rank.") · ⭐ 9.5k · MIT · Oct 2026</sub>

**Browser canvas for sketching linked Material 3 screens and exporting an AI prompt.**

M3E Canvas is a static Next.js app where you drag Material 3 Expressive parts onto phone or desktop screens, link them with tap and swipe transitions, and preview the flow. The design is exported as a prompt in Japanese, English, Chinese or Korean, targeting Android or web, to paste into a coding tool such as Claude Code, Codex, Gemini CLI or Cursor. State is kept in localStorage; there is no backend.

- **+** No backend: static export, designs saved in browser localStorage
- **+** Tap and swipe navigation with transitions, plus a clickable preview
- **+** Prompt output in four languages for Android or web targets
- **+** Optional AI helper sends your own key straight to the provider
- **−** Phone browsers get a one-screen, buttons-only editor
- **−** Output is a text prompt, not generated code
- **−** Design lives in browser storage unless shared by link
- **−** Fonts load from Google Fonts at runtime

<sub>no GPU · Needs Node.js and npm (to build), Google Fonts · Models: OpenAI, Claude, Gemini, DeepSeek · port 3000 · [Repo](https://github.com/lnkiai/m3e-canvas) · [▶️ Demo ↗](https://lnkiai.github.io/m3e-canvas/) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/m3e-canvas/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
