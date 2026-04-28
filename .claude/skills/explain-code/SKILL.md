---
name: explain-code
description: Explain what a file, function, or code block does in plain language. Use when the user asks "what does this do", "explain X", or pastes unfamiliar code.
---

# Explain Code

Output structure:

1. **One-sentence summary** — what the code accomplishes at a high level.
2. **Key pieces** — bullet points, each naming a function/block and its role. Use `file:line` references.
3. **Data flow** — how inputs become outputs (only if non-obvious).
4. **Gotchas** — any subtle behavior, side effects, or assumptions worth flagging.

Keep it tight. Skip sections that don't add value. Match the user's language (中文 / English).
