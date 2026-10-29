---
name: delivery-assurance
description: Assess a fixed software candidate's review, test and real-user-path evidence for handoff; report readiness and gaps separately from user acceptance.
---

# Evidence-based delivery assurance

Own candidate completeness, evidence sufficiency and technical delivery readiness. Consume review and verification results; do not maintain or perform a second Standards/Spec code-review algorithm. A requested code review alone does not activate this workflow. An assurance/readiness-only request ends with supported status and gaps, without repairing, running tests or declaring the product delivered.

## 1. Establish the candidate and requested outcome

Use the accepted requirements/scope, public user paths, current authorization, existing project record and resource limits. Freeze the actual candidate and relevant baseline under the shared [fixed-input contract](../../references/integration.md#fixed-input-and-project-records), including relevant WIP/new files and requirement identities. A complete delivery candidate can be wider than a deliberately narrow earlier review; record that coverage difference.

A receipt must identify what was executed or reviewed and against which requirements. Hashes or file existence alone do not establish completeness or correctness. Writes/snapshots/registration follow current permitted effects; use existing records rather than create a new registry.

## 2. Assess existing evidence first

Map each applicable delivery obligation to actual evidence and classify it PASS, FAIL, UNKNOWN or N/A with the reason/source. Unknown, missing, blocked and unexecuted items cannot become PASS.

- **Review:** look for both separate Standards/Spec outputs covering the actual candidate, agreed requirements and required local Standards, with fresh-context and real-tool evidence. Missing Spec, stale input, a narrower selection or absent required quality coverage limits that receipt. Retain valid covered evidence; do not rerun just because this Skill was selected.
- **Test-first and regression:** for authorized behavior changes/retained demos/bug repairs, inspect the actual meaningful red and matching green, public seam and source/test/input identities. After-the-fact tests or an unrelated green check do not prove test-first. Historical work can be assessed with missing process evidence labelled, not invented. Pure cleanup uses meaningful before/after green.
- **Real user path and effects:** inspect actual accepted UI/CLI/service operations, expected versus observed results, significant state/failure behavior, cleanup and surviving evidence. For a material coverage gap, apply only needed [verification](../../references/verification.md) branches. A CLI check does not certify UI behavior and a generated guide is not an executed path.
- **Candidate state:** assess evidence for the post-cleanup candidate and any later relevant edits, including applicable caller/state/exception risks. Reuse affected proof only when its validity is established; avoid broad code re-review masquerading as an evidence check.

This Skill judges whether review/verification claims are supported and applicable. It does not redo smell analysis, infer correct implementation from a score, or silently adjudicate contradictory code findings. Report the exact unsupported claim and return any necessary content judgment to the single review method.

## 3. Close only authorized evidence gaps

If a necessary review is missing/invalid, use installed `code-review` at its native path only within current execution authority, with the fixed candidate, Spec, required Standards and remaining budget. That method owns the only two-axis dispatch. If valid review evidence already exists, consume it without spawning more reviewers. Do not invoke the legacy compatibility name as another review.

Use existing accepted verification commands/project driver first for an authorized verification gap. New model calls, installations, external effects or broader trials require their actual authority; readiness inspection is no such permission. Missing capability or authorization produces an explicit incomplete result rather than simulated proof.

Code repairs belong to the existing authorized implementation/diagnosis method, not a new delivery implementation loop. For covered repairs, preserve the same candidate/evidence chain, then assess affected checks and any necessary re-review under the [existing review/recheck ceiling](../../references/integration.md#code-review-input-and-runtime-adaptation). Count earlier attempts/rounds; neither this entry nor a new version grants a new budget. At a stop condition retain evidence and report the remaining gap.

## 4. Report readiness, then hand off only when requested

Report what is supported, failed, unverified or inapplicable, citing actual tool/command results and candidate identity. An empty findings list, a review PASS or successful test counts alone do not establish delivery readiness. Necessary missing proof or unresolved substantiated blockers leave delivery incomplete.

For actual behavioral handoff, apply [human-review](../../references/human-review.md) to explain the real architecture, code logic, data/external calls, failure behavior, real example, small diagram, tradeoffs and limits in ordinary Chinese. An evidence-only assessment needs its concise findings and limitations, not a full product explanation.

Technical verification/readiness, the user's explicit acceptance and any adoption/release authorization remain separate. Preserve them in the existing permitted project record; silence, Agent confidence and this Skill's verdict cannot substitute for user acceptance.
