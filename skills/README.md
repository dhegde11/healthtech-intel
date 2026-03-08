# Skills

These are the research prompt templates that power healthtech-intel. They are plain markdown and work with any LLM that can execute web searches.

## What's here

| File | What it does |
|---|---|
| [`researching-health-system.md`](researching-health-system.md) | Profile a hospital or health system for BD prospecting |
| [`researching-health-it-vendor.md`](researching-health-it-vendor.md) | Profile a health IT company for competitive intelligence |
| [`discovering-health-it-competitors.md`](discovering-health-it-competitors.md) | Discover companies matching a natural language query |

## How to use with Claude Code

The `.claude/skills/` and `.claude/agents/` directories at the project root wire these prompts into Claude Code automatically. See the main [README](../README.md) for setup instructions.

## How to use with other AI assistants

Copy the prompt content (below the YAML frontmatter) and paste it into your assistant's system prompt or custom instructions. Replace `{entity}` or `{query}` with the specific name you want to research.

YAML frontmatter notes:
- `name` / `description` — informational, for Claude Code's skill registry
- `max_tool_rounds` — tells the Claude Code runner how many search rounds to allow; ignore for other assistants
- `mode` — used by `lookup.py` internally; ignore for other assistants
