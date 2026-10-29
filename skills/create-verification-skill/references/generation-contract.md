# Generation contract

## Inspect before generating

Read the actual project instructions, existing approved scope/design, run commands, package/build metadata, tests and fixture contracts. Identify every user surface (CLI/TUI, browser, desktop, mobile, service or library); name the primary surface and explicitly list surfaces not exercised. Determine exact local run/build commands, required environment-variable names without reading/copying secret values, readiness, seed/migration state, authorization and disposable-state options. Prefer existing browser/PTY/HTTP/test helpers to a new harness. Use existing dependencies; a missing tool is a stated gap, not permission to install it. Default to deterministic local operation without models, cloud APIs or new dependencies. A mocked system is evidence only for the boundary that the production architecture already isolates.

Check whether simultaneous runs can isolate ports, profiles and data. Refuse to drive an unowned shared instance when isolation is unavailable. If startup fails, retain the real error and report the blocked draft. Fixing app code or scaffolding must stay within approved coding scope; document any required verification-only scaffolding and remove only that scaffolding afterward.

## Generated skill

Write `.agents/skills/verify-<app>/SKILL.md` with valid YAML name/description identifying the actual app, surface and intended use. Do not advertise an unproved recipe as verified. Include:

- **Launch:** literal commands, cwd, required existing runtime/dependencies, disposable state, fixture/migration preparation and a usable readiness condition. A listening process or database ping alone is insufficient. For a short-lived CLI, explain that each invocation launches and exits; do not invent a server or PTY requirement when ordinary argv is the accepted interface.
- **Doctor:** a read-only health/identity check for the exact build, inputs, owned instance, readiness and required auth. Run it before driving and whenever behavior is suspicious. Never disclose credentials.
- **Drive:** exact existing commands or stable user-facing handles. Exercise the accepted surface; do not substitute internal setters or test-only endpoints. Preserve preconditions and exceptions. Use browser/computer tools available to Codex only when the real UI requires them; no source-specific agent names or tool assumptions.
- **Evidence:** named durable location outside scratch cleanup; capture action plus resulting state, actual argv/cwd/environment names, input/code identities, stdout/stderr/exit, screenshots when relevant, and independent meaningful expected results. Check visible output and actual side effects via a second read when applicable. Observe dry-run/test-mode effects; a flag name is not proof of no writes/network/browser actions. Do not claim a complete map, UI, remote deployment, real authentication, model or business outcome from a narrower smoke.
- **Cleanup:** stop only processes started by this run using their recorded identities, and remove only owned scratch resources on success or failure. Never kill by process name. Preserve evidence and confirm it exists after teardown. State absent persistent processes/effects explicitly for a short-lived read-only CLI.
- **Helpers:** ship only helpers that improve reuse/reliability; make executable scripts executable, show literal invocations and describe inputs/outputs/failure behavior. Validate scripts by actual execution.

## Feature map

Create `features/README.md` as the maintained index, with shared baseline preconditions, driving conventions, evidence locations, feature IDs and per-entry coverage state. Seed real identifiable features (usually the top three to five, fewer if the actual project has fewer). Never invent features to reach a count.

Create one file per feature. Start with its user-visible purpose and use these four H2 sections:

1. `Sub-features`: short behavior IDs, meaningful observable expected results.
2. `How to get to it (user POV)`: each real supported user entry point.
3. `Driving it with <actual harness>`: explicit `Preconditions:`, exact actions/commands or stable selectors and expected results, including how evidence is captured.
4. `Gotchas`: missing seed state, known timing/auth/isolation constraints and unreachable paths. An unmet precondition is a failed/blocked journey; never weaken it to force success.

Use only known real values in runnable recipes, with named run paths supplied by the launch step. Keep each entry point's evidence distinct; exercising one convenient path does not cover other entries. Existing upstream Notes examples are illustrations, not runnable fixtures for a different app.

## Prove and hand off

Execute launch → doctor → one mapped feature → evidence → cleanup once using the generated instructions. Check expected content/meaning, input/build identity and load-bearing effects, not only exits or file counts. Add an appropriate actual boundary/negative case when it tests a material safety or contract fact. Always run generated cleanup after failed attempts too. Confirm durable evidence survives cleanup and validate the generated skill. Preserve failed iterations.

Record mapped versus exercised paths and limitations. A stand-in/isolation copy proves only the supplied copy and surface: list setup it received and what the actual deployment still lacks. Retain current candidate hashes alongside the record; hashes identify the candidate and do not establish correctness or user acceptance. Missing execution leaves a draft. Maintenance is an update to this same map within future authorized coding work, not a new automation.
