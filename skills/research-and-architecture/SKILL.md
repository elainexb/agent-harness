---
name: research-and-architecture
description: Evaluate software feasibility and architecture decisions from evidence, including framework comparison and new-effort alignment.
---

# Research and Architecture

Apply the relevant workflow requirements without changing the user's scope,
authorization, acceptance, or already confirmed decisions. Global AGENTS.md remains
responsible for the lifecycle and approval gates. Domain-specific Skills may
provide tools or methods; they do not waive these applicable requirements.

## Route before dependent work

Own decision analysis: requirements/options, feasibility, tradeoffs, responsibility boundaries and approval-ready proposals. Factual investigation is owned by `research`, not a second local collection method. Consume sufficient current evidence directly. Only when a material factual gap blocks the decision, formulate that bounded question and use the applicable evidence method through native discovery; do not load it merely because this task is architectural. A broad evidence request does not confer design approval.

Enter directly for the requested decision stage. Reuse approved decisions and current dependencies. Read only current-stage guidance; a source-location question is not a decision stage.

- Option comparison or feasibility assessment: read and follow
  [feasibility and evidence requirements](references/research.md) before that decision stage.
- Framework selection, architecture design/review, or a material architecture,
  contract, technology, or scope change: read and follow
  [architecture requirements](references/architecture.md) before that stage.
  For an architecture approval explanation, apply the shared [human-review requirements](../../references/human-review.md) to the proposed design and actual evidence, without presenting it as implemented.
- For a new/changed software module boundary, use installed `codebase-design` and the existing [local module-boundary guidance](../../references/architecture.md) before the boundary decision. That Reference owns concrete caller/state/failure analysis and scoped source guidance; this Skill's architecture Reference owns feasibility/approval requirements. This branch does not apply to a routine location query.
- A task spanning feasibility and architecture loads each reference when its stage begins.
  Do not load both by default. Check documented prior research findings and user
  confirmations before entering architecture; if prerequisites are missing,
  complete the authorized evidence/feasibility gap first.
- An approved routine fix or retest reuses applicable prior research/design;
  load a reference only if a relevant stage or new consequential decision is
  actually being reopened. Do not re-request settled approvals.

For an actual new-software-effort alignment, use shared [startup assessment](../../references/project-start.md#startup-assessment), including the applicable pinned-method assessment. Reuse a valid assessment and settled project decisions; ordinary resumed work needs no startup reload.

For consequential unresolved user decisions that need interviewing, select the
interview through native discovery. Its own entry owns method choice and actual
invocation policy; this Skill supplies the decision frontier, not another router. If the selected method or an applicable reference is unavailable,
disclose that and pause only dependent decisions; continue independent work.

## Evidence and handoff

For complex or cross-session decision work, use the [continuation record convention](../../references/integration.md#fixed-input-and-project-records) with the existing plan/spec/tickets; a bounded answer needs no additional plan or record.

Use the existing authoritative project record. Record the applicable requirements,
inputs, source evidence, findings, gaps, limitations, decisions, and user
confirmations there. For inapplicable items state the reason; do not silently waive
applicable obligations. End each stage with its result, remaining limitations,
approval state, and next allowed action. Written coverage, package validation, or
completion of research does not establish runtime success, user acceptance,
architecture approval, or implementation authorization.
