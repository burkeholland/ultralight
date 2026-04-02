# ultralight

A multi-agent orchestration framework for VS Code. Uses the best AI model for every task — Claude Opus 4.6 orchestrates and plans, GPT-5.3-Codex codes, and Gemini 3.1 Pro (Preview) designs.

## Install as Plugin (recommended)

Install all four agents in one step:

1. Open the VS Code Command Palette (`⌘⇧P`) and run **Chat: Install Plugin From Source**
2. Paste: `https://github.com/burkeholland/ultralight`
3. All 4 agents install automatically 🎉

**Required VS Code settings:**

```json
"chat.plugins.enabled": true,
"chat.subagents.allowInvocationsFromSubagents": true
```

## Manual Install (individual agents)

You can also install agents one at a time from the [gist](https://gist.github.com/burkeholland/0e68481f96e94bbb98134fa6efd00436), or visit the [website](https://burkeholland.github.io/ultralight) for install buttons.

## Agents

| Agent | Model | Role |
|-------|-------|------|
| Orchestrator | Claude Opus 4.6 | Breaks requests into phases, delegates to specialists |
| Planner | Claude Opus 4.6 | Researches codebase, produces step-by-step plans |
| Coder | GPT-5.3-Codex | Writes production code |
| Designer | Gemini 3.1 Pro (Preview) | Handles all UI/UX |

Agent definitions live in the [`agents/`](./agents) directory.

## Website

Hosted on GitHub Pages.
