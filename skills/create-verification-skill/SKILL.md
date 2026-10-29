---
name: create-verification-skill
description: Create a project-local verification recipe and feature map for an actual CLI, UI or service when that artifact is requested or its creation is explicitly in scope. Smoke-test it only within authorized validation; a missing driver alone does not authorize creation.
---

# Create a verification skill

Before generation, apply the shared [verification scope and missing-capability boundary](../../references/verification.md#verification-scope-and-missing-capability). Establish whether the requested outcome covers a proposal, recipe creation and/or actual smoke execution; complete only the covered work. Generate `.agents/skills/verify-<app>/` only inside the actual authorized project and only when creation is covered. Read [the generation contract](references/generation-contract.md) before writing. This Codex adaptation preserves pstack's user-path method; provenance and MIT attribution are in [source-lock.json](references/source-lock.json) and [LICENSE](LICENSE).

Inspect the supplied checkout and reuse its accepted requirements, existing tests, fixtures and interaction surfaces. Carry the project's existing goal, research, architecture, implementation and acceptance gates forward. This skill grants no project writes outside the coding task, framework/dependency installation, model/API use, external mutations, production access, or recurring automation. Resolve only consequential new choices through the applicable existing gate.

Discover actual launch, readiness, doctor, drive, evidence and isolation behavior. Generate a concise skill, the feature map and only genuinely useful helpers. Drive one mapped feature through the real accepted user surface, check meaningful expected output and effects, then clean up and prove its evidence survived. Reuse tests as supporting evidence; a CLI or HTTP check alone never establishes UI behavior.

Validate the generated skill with `codex-skill-validate <generated-skill-directory>` and retain actual commands, exit codes, outputs, input/code identity, limitations and remaining map coverage in the project's existing verification record. If launch or smoke is blocked, preserve the attempt and label the output an unexecuted draft. Do not repair application behavior or weaken its journey without the appropriate task authority. User acceptance remains separate from technical verification.

Keep the map updated when an authorized feature change alters its user paths. Do not install a maintenance hook or schedule a recurring check.
