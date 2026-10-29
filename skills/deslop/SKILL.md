---
name: deslop
description: Clean the selected software diff after green or during requested behavior-preserving cleanup; remove unnecessary generated code, comments and style problems without broad rewrites.
---

# Remove AI code slop

For this selected cleanup task, read the shared [cleanup contract](../../references/cleanup.md) for local comment criteria, scope and affected rechecks. Reuse it if already loaded; it starts no parent workflow.

Check the selected diff against its confirmed base, including scoped WIP/new files, and remove the generated slop in that scope. Do not assume the base is main.

## Focus Areas

- Extra comments that are unnecessary or inconsistent with local style
- Defensive checks or try/catch blocks that are abnormal for trusted code paths
- Casts to `any` used only to bypass type issues
- Deeply nested code that should be simplified with early returns
- Other patterns inconsistent with the file and surrounding codebase

## Guardrails

- Keep behavior unchanged unless fixing a clear bug.
- Prefer minimal, focused edits over broad rewrites.
- Keep the final summary concise (1-3 sentences).
