# Agent Harness

Selected core materials from my Codex Harness for work across projects, shared for reading and archival reference. This snapshot was prepared on 2026-10-29 from `R15+scenario-evaluation-20261029`, recorded as **Trial Adopted**.

## Start here

| Topic | Entry point | What it covers |
|---|---|---|
| Global rules | [global/AGENTS.md](global/AGENTS.md) | Authority, stages, quality, evidence and completion boundaries |
| Shared conventions | [references/integration.md](references/integration.md) | Codex host conventions shared across methods |
| Engineering and delivery | [implementation.md](references/implementation.md), [verification.md](references/verification.md), [human-review.md](references/human-review.md) | Test-first development, real user-path verification and delivery explanations |
| Review and cleanup | [strict-quality.md](references/review/strict-quality.md), [cleanup.md](references/cleanup.md) | Code quality, independent review and scoped cleanup |
| Task methods | [skills/](skills/) | Select the relevant Skill from the table below |
| Sources and licenses | [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) | Upstream sources, pinned revisions and license notices |

```text
global/        Global working rules
references/    Shared conventions and supporting material
skills/        Task methods and their required resources
```

Folders follow reading responsibilities. Selected methods from two local Skill roots are presented together under `skills/`. The original `.codex` and `.agents` locations are not top-level repository categories. There is no payload layer or installation packaging.

## Method entry points

| Task | Skill |
|---|---|
| Factual investigation | [research](skills/research/SKILL.md) |
| Feasibility and architecture decisions | [research-and-architecture](skills/research-and-architecture/SKILL.md) |
| Module and domain terminology design | [codebase-design](skills/codebase-design/SKILL.md), [domain-modeling](skills/domain-modeling/SKILL.md) |
| Resolve consequential open choices | [grilling](skills/grilling/SKILL.md), [grill-with-docs](skills/grill-with-docs/SKILL.md) |
| Implementation and defect diagnosis | [tdd](skills/tdd/SKILL.md), [diagnosing-bugs](skills/diagnosing-bugs/SKILL.md) |
| Independent review and delivery evidence | [code-review](skills/code-review/SKILL.md), [delivery-assurance](skills/delivery-assurance/SKILL.md) |
| Cleanup and agent-facing writing | [deslop](skills/deslop/SKILL.md), [writing-for-agents](skills/writing-for-agents/SKILL.md) |
| Skill evaluation and verification recipes | [test-skill](skills/test-skill/SKILL.md), [create-verification-skill](skills/create-verification-skill/SKILL.md) |
| Decision-specific engineering principles | [pstack-principles](skills/pstack-principles/SKILL.md) |
| Existing review-name compatibility | [independent-code-review](skills/independent-code-review/SKILL.md) |

The selection contains 16 core Skills and direct dependencies. Global rules own authority and quality boundaries; Skills own methods; supporting material is read conditionally. Native invocation metadata is retained, including explicit-only policies. The 24 pstack principles form an on-demand library, not a requirement to load every principle for every task.

## Archive scope and provenance

This is a selected snapshot of the current cross-project setup, not a backup of every installed tool or the whole machine. Installation, conditional availability, observed invocation and verified behavior are distinct facts. This archive does not claim that every Skill, reference, principle or branch has been used or behaviorally verified.

Complete methods, necessary branch resources, version information and source receipts are retained. Private paths are redacted; `<LOCAL_REGRESSION_LIBRARY>` denotes an omitted private location. Some reading links use repository-relative paths or pinned upstream URLs, so this is not a byte-for-byte backup. Original upstream hashes remain recorded; copies with adjusted links have separate `publication_sha256` values. The historical installation profile does not mean that every original package or source archive is included here.

Excluded material includes application/project files, project-local rules, personal memories and cases, raw sessions and run logs, credentials, active configuration, old backups, the evaluation Runner, Memory plugins and the unadopted Memory Lifecycle Candidate. Other independent Skills and optional planning entry points are not included in full.

Preparing this archive did not change the active Harness. Git commits will record this public copy's revisions. No installation workflow, patch mechanism or runtime certification has been added.
