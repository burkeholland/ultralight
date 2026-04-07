# ultralight

A multi-agent orchestration framework for VS Code. Uses the best AI model for every task — Claude Sonnet 4.6 orchestrates, Claude Opus 4.6 plans and designs, and GPT-5.3-Codex codes.

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
| Orchestrator | Claude Sonnet 4.6 | Breaks requests into phases, delegates to specialists |
| Planner | Claude Opus 4.6 | Researches codebase, produces step-by-step plans |
| Coder | GPT-5.3-Codex | Writes production code |
| Designer | Claude Opus 4.6 | Handles all UI/UX |

Agent definitions live in the [`agents/`](./agents) directory.

## Bundled Tools

The plugin includes these out of the box — no extra setup required:

| Tool | Type | Purpose |
|------|------|---------|
| [Context7](https://context7.com) | MCP Server | Up-to-date documentation lookup for any library |
| [Frontend Design](https://github.com/anthropics/skills) | Skill | Production-grade UI/UX design guidance (Anthropic) |

## Website

Hosted on GitHub Pages at [burkeholland.github.io/ultralight](https://burkeholland.github.io/ultralight).
