---
name: quick-commit
description: Stage all changes and create a concise conventional commit. Use when the user asks to "commit", "save changes", or wants a quick commit without specifying details.
---

# Quick Commit

Steps:

1. Run `git status` and `git diff --staged` (and `git diff` if nothing staged) in parallel to see what changed.
2. Pick a conventional commit type: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`.
3. Write a one-line subject (≤72 chars) describing the *why*, not the *what*.
4. If multiple unrelated changes exist, ask the user before bundling them into one commit.
5. Stage relevant files explicitly (avoid `git add -A` to prevent leaking secrets).
6. Commit with the drafted message.
7. Show `git status` after the commit.

Never push unless the user asks.
