<div align="center">

# ⚡ OpenRouter Chat

**A ChatGPT-style chat UI that runs entirely in your browser.**
No backend. No accounts. No tracking. Just paste your OpenRouter key and go.

[![Made with HTML](https://img.shields.io/badge/Made%20with-HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![No Dependencies](https://img.shields.io/badge/Dependencies-0-10a37f?style=for-the-badge)](#)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=for-the-badge&logo=github)](https://pages.github.com/)
[![License MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](#-license)

[**🚀 Try it live**](https://YOUR-USERNAME.github.io/openrouter-chat/) &nbsp;·&nbsp;
[**🔑 Get an OpenRouter key**](https://openrouter.ai/keys)

</div>

---

## ✨ What is this?

A single-file, zero-dependency web app that gives you a clean, ChatGPT-style chat interface powered by [OpenRouter](https://openrouter.ai). It runs **100% client-side** — there is no server, no database, and no analytics. Your API key never leaves your browser except to talk directly to OpenRouter.

> **TL;DR** — One `index.html`. Paste your key. Chat with GPT-4o, Claude, Gemini, Llama, Mistral, and more.

---

## 🎯 Features

| | |
|---|---|
| 💬 **ChatGPT-style UI** | Dark theme, streaming responses, auto-growing composer, Enter-to-send. |
| 🔐 **Bring your own key** | Your OpenRouter API key is entered at runtime and held **only in memory**. |
| 🧠 **Multi-model** | Switch between GPT-4o, Claude 3.5 Sonnet, Gemini Flash, Llama 3.1, Mistral, and more from a dropdown. |
| ⚡ **Streaming responses** | Tokens appear as they're generated — no waiting for the full reply. |
| 📦 **Single file** | The entire app is one `index.html`. No build step. No npm. No frameworks. |
| 🌐 **Static hosting** | Deploys in seconds on GitHub Pages, Cloudflare Pages, Netlify, or any static host. |
| 🚫 **No storage** | Never touches `localStorage`, `sessionStorage`, cookies, or IndexedDB. |

---

## 🔐 Privacy & Security

This project was designed around one rule: **your key is yours.**

- 🔒 The key lives in a single JavaScript variable.
- 🧹 It is wiped on `pagehide` and `beforeunload` — closing or refreshing the tab destroys it.
- 🚫 It is **never** written to any browser storage.
- 🛰️ Requests go **directly from your browser to `openrouter.ai`**. There is no middleman server.
- 👁️ **Caveat:** as with any web app, browser extensions or DevTools can see the key while the tab is open. Don't paste a key you don't trust on a machine you don't trust.

---

## 🚀 Usage

### Option 1 — Use the live demo

1. Open the [live site](https://YOUR-USERNAME.github.io/openrouter-chat/).
2. Grab a free API key at **[openrouter.ai/keys](https://openrouter.ai/keys)**.
3. Paste it into the gate screen.
4. Pick a model from the top-right dropdown.
5. Chat.

### Option 2 — Run it locally

```bash
git clone https://github.com/YOUR-USERNAME/openrouter-chat.git
cd openrouter-chat
# Open index.html in your browser — that's it.
open index.html       # macOS
# or: start index.html  # Windows
# or: xdg-open index.html  # Linux
