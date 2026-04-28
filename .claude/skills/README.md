# Project Skills

Custom skills available in any Claude Code session opened on this repository,
including **mobile / web sessions** at [claude.ai/code](https://claude.ai/code).

## How to use

Trigger a skill by:

- **Slash command** — type `/<skill-name>` (e.g. `/find-skills`)
- **Natural language** — describe what you want; Claude matches the skill's
  `description` field automatically.

## Skills in this repo

### The "5 必装 skills"

| Skill | Purpose | Source |
|---|---|---|
| `using-superpowers` (+13 sibling skills) | Software-engineering methodology: TDD, debugging, planning, parallel agents, code review | [obra/superpowers](https://github.com/obra/superpowers) |
| `frontend-design` | Build distinctive, production-grade frontend interfaces | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/frontend-design) |
| `planning-with-files` | Manus-style persistent markdown planning for multi-step tasks | [othmanadi/planning-with-files](https://github.com/othmanadi/planning-with-files) |
| `skill-creator` | Interactive Q&A workflow to create new skills | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/skill-creator) |
| `find-skills` | Discover and install agent skills from the ecosystem | [vercel-labs/skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills) |

### Superpowers sub-skills (from `obra/superpowers`)

`brainstorming`, `dispatching-parallel-agents`, `executing-plans`,
`finishing-a-development-branch`, `receiving-code-review`,
`requesting-code-review`, `subagent-driven-development`, `systematic-debugging`,
`test-driven-development`, `using-git-worktrees`, `using-superpowers`,
`verification-before-completion`, `writing-plans`, `writing-skills`.

### Project starters

- `quick-commit` — stage and commit with a conventional message.
- `explain-code` — plain-language explanation of a file/function.

## Adding a new skill

Create `.claude/skills/<skill-name>/SKILL.md`:

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

## Project vs personal skills

- **Project skills** (`.claude/skills/`) — committed to git, shared with the
  team, **available on web/mobile**.
- **Personal skills** (`~/.claude/skills/`) — local only, not available on
  mobile (web sessions run in the cloud).

For mobile use, always put skills in the project directory.

## Licenses & attribution

The bundled skills retain their upstream licenses (see `LICENSE.txt` files
inside each skill folder where present). Credits go to the original authors
linked in the table above.
