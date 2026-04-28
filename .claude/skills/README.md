# Project Skills

This directory contains custom skills available in any Claude Code session
opened on this repository — including **mobile / web sessions** at
[claude.ai/code](https://claude.ai/code).

## How to use

In a Claude Code session (desktop, web, or mobile), trigger a skill by:

- **Slash command**: type `/<skill-name>` (e.g. `/quick-commit`)
- **Natural language**: describe what you want; Claude matches the skill's
  `description` field automatically.

## How to add a new skill

Create `.claude/skills/<skill-name>/SKILL.md` with this format:

```markdown
---
name: my-skill
description: When to use this skill (Claude reads this to decide).
---

# My Skill

Step-by-step instructions for Claude to follow.
```

Commit and push — the skill is immediately available in every session that
clones this repo.

## Personal vs project skills

- **Project skills** (`.claude/skills/`) — committed to git, shared with the
  team, available on web/mobile.
- **Personal skills** (`~/.claude/skills/`) — local only, **not available on
  mobile** since web sessions run in the cloud.

For mobile use, always put skills in the project directory.
