# Skill evaluation

Read only the section selected by the current mode. This Reference owns diagnosis attribution, test selection, comparison evidence and dispositions. Links here do not activate their parent Skills or authorize execution. Existing project records retain requirements, cases and approvals; reuse them rather than creating another registry.

## Diagnosis

For an existing failure, inspect the original request, raw artifacts, applicable instructions and actual execution. Distinguish requirement/oracle, input, routing, method behavior and Harness/environment faults. State observations, hypotheses and unknowns separately; loading a Skill is not evidence of executing its method. Trace the earliest observable departure from the request. For a new Skill, use requirements and expected behavior; no failure artifact is required.

Return supported attribution or exact gaps. Do not infer the internal cause from matching Reference paths or turn a diagnosis-only request into repairs, new runs or a broader audit.

## Case definitions

This section owns Agent Evaluation case standards. Use existing accepted cases and records; fill only missing or materially changed definitions rather than create another template or registry.

Define each case against the actual Agent task:

- **Subject and mechanism:** the requested capability, observed failure or risk, and the behavior this case can distinguish. Separate task interpretation, method selection, actual execution and Harness/environment validity; a Skill read alone is not proof of method execution.
- **Actual input and starting context:** the exact request and necessary conversation, files, instructions/Skill versions, catalogue and environment. Label original versus constructed/edited material and disclose additions or omissions. Preserve the failure trigger and relevant exceptions; evaluator answers, fix discussions and scoring conclusions stay outside the evaluated input.
- **Expected Agent behavior and limits:** derive observable requirements from the user request and independent sources. Specify permitted effects, stopping point, required answer/artifact properties and relevant negative/boundary behavior. Do not use a preferred Skill name, fixed tool count or hidden reasoning as a proxy for task success.
- **Assertions and oracle:** Before execution, define applicable target assertions in the existing case record, grouped as relevant under Skill Selection, Method Behavior, Harness Authorization and Outcome; these are not a mandatory coverage checklist. Retain independent PASS conditions, concrete FAIL counterexamples and required evidence. For each targeted dimension, an evidenced required-assertion failure means FAIL; all required assertions passing means PASS; otherwise use NOT VERIFIED. If reporting an uncovered or inapplicable dimension, use NOT VERIFIED with its coverage reason, never inferred PASS/FAIL. Preserve environment blockage, budget interruption and insufficient evidence as distinct reasons alongside existing execution statuses. Keep criteria independent of Candidate output; comparison freezing is governed by Before execution.
- **Actual evidence:** identify native completion/final output, public tool actions/results and relevant file/state changes needed to assess the assertions. Judge observed actions and outputs, not the Agent's self-rating. Distinguish attempted effects from successful effects and actual execution from a proposed plan.
- **Validity and measurement:** state relevant isolation, version/environment, source and stop-reason requirements. Keep behavioral judgment distinct from facility faults, comparison validity and cost-accounting completeness. Incomplete token records alone do not negate independently supported behavioral PASS; missing necessary answer/action evidence cannot become PASS.
- **Coverage and resources:** state which failure mechanism and normal/negative regression the case covers, why the chosen test level is necessary, and the proposed or existing authorized budget. A cheaper/reduced case must still observe the target mechanism. Retain case IDs and mark unexecuted checks NOT_RUN.

Only when the case also needs software behavior validation at a real CLI/UI/API boundary, and that software-test method is useful, consult [software test-case design](../../../references/implementation.md#test-case-design-before-code) as supporting guidance. Agent behavior assertions remain owned here. This optional reuse does not activate coding-workflow, implementation or TDD, and ordinary Agent Evaluation design has no mandatory dependency on that software method.

## Packaging

After the global candidate-review and validation-authorization gates, validate a complete isolated Skill package with `codex-skill-validate SKILL_DIRECTORY` in the dedicated Python environment. Use existing static checks for other names/references concerns. Report packaging separately from behavior, user review and adoption. A valid package does not prove automatic invocation, method adherence or savings; unexecuted validation is NOT_RUN. No Runner/model is needed for packaging itself.

## Protocol candidate work

For a Harness/Skill/global-rule change, first attribute noncompliance with existing guidance versus inadequate guidance or missing capability. Prefer the smallest correction at the evidenced owner; an unsupported fix can be NO_CHANGE.

Only when that change concerns an upstream update, dependency compatibility or source/local-adaptation ownership, use [dependency and upstream maintenance](../../../references/project-start.md#dependency-and-upstream-maintenance) to derive the affected consumers and proposed revalidation scope. An ordinary evaluation does not load source locks or audit unrelated Skills. This proposal step does not execute the proposed checks.

Before validation, present the complete identified candidate or exact diff, scope, procedure, stopping conditions, planned evidence and resource limits for user review. Obtain authorization for the particular validation: packaging scripts, model-free checks, replay and model trials are separate evidence types, not automatically authorized by candidate preparation. One explicit approval can cover stated stages; reuse it without manufacturing another gate.

Freeze the candidate and trial conditions. Authorized trials use isolated copies outside normal discovery; keep expected answers/fix discussions out of evaluated inputs. Material candidate/condition drift returns to the affected gate. Report actual results before recommending adoption; user review and authorization decide adoption, not a script, a generated plan or a favorable verdict. No approval here changes application scope or permits installation, external effects, or active-rule writes.

A proposal-only request ends with a reviewable candidate/plan and NOT_RUN validation. A validation-only request does not adopt it. Persist evidence only within current permitted effects and reuse the existing owner; do not create another registry or Runner. Only when the proposed change installs, migrates, updates or retires shared Harness assets, read [shared ownership and lifecycle](../../../references/project-start.md#shared-reference-ownership-and-lifecycle); ordinary Skill evaluation does not load asset-maintenance guidance.

## Skill authoring

For an actually authorized Skill edit or candidate authoring task, load installed `skill-creator` and `writing-for-agents`. They own packaging/authoring and instruction hierarchy; evaluating a Skill or designing cases does not activate them. Existing architecture/research gates apply where those decisions are actually reopened. For consequential unresolved user choices needing an interview, use native discovery and the selected interview's own entry/policy; inspectable facts do not start an interview.

## Test selection

Prefer a representative real user scenario that naturally covers multiple related target assertions from one execution. Its E2E outcome is the authorized task deliverable, not the entire product lifecycle. Split cases only when different authorization, environments or mutually exclusive key branches prevent valid joint observation; use focused tests for material uncovered or failed branches. The smallest valid test is the smallest task that can observe the original failure mechanism. It is not necessarily the shortest input or cheapest call. Explain how the original case triggered the failure and which conditions remain after reduction before selecting an observation boundary.

| Question | Preferred test | Evidence boundary |
|---|---|---|
| Packaging, names or references | Existing static validators under [Packaging](#packaging) | Does not establish model selection or semantic execution. |
| Timeout, cancellation, errors, events, snapshots, drift or check reuse | Model-free script checks or controlled processes | Does not establish the evaluated Skill's behavioral quality. |
| A specific behavior after Skill selection | Focused task with necessary raw materials | Does not establish automatic invocation; keep expected answers out of the request. |
| Missed/incorrect selection or loading order | Native routing test with fixed catalogue and instructions | Implicit requests do not name the intended Skill; include relevant near-miss controls. |
| Phase transitions, recovery or cross-capability constraints | Affected workflow replay | Expand to this level when those relationships carry the failure mechanism or change risk. |

Preserve the raw instructions, state, sources and dependencies that determine behavior. For example, reproducing loss of a continuing priority plus a temporary fallback requires both statements and the consolidation action. Asking the model to repeat an explicitly supplied correct answer does not reproduce that mechanism. This focused case establishes a local observation; whole-specification preservation still requires applicable broader checks.

Recovery, routing or long context may themselves carry the mechanism. Use a larger case when reduction cannot preserve it, explaining why. If the necessary case exceeds the available budget or permissions, report the gap rather than substitute a distorted smaller test.

Select regression from the actual diff:

- Local method changes: target behavior, necessary exceptions and nearby valid behavior.
- Description, entrypoint or shared-rule changes: affected explicit/implicit calls, near-misses and callers.
- Phase, permission or cross-capability contract changes: affected interactions and important failure/recovery branches.
- Harness changes: affected lifecycle, error exits and evidence integrity. Evaluate the Harness separately; its checks do not establish Skill improvement.

Map each change to applicable checks and explain exclusions. Reuse valid evidence; changed relevant inputs, executors or artifacts invalidate affected evidence. Adoption claims must cover applicable risks; a focused PASS does not automatically expand coverage.

## Comparison and evidence

### Before execution

Use the test-skill-owned [Case definitions](#case-definitions) for Agent Evaluation inputs, assertions and observation methods. Reuse valid definitions and independent sources rather than derive expectations backward from Candidate output. Read software test-design guidance only under the optional software-boundary condition in that section.

Freeze the oracle and comparison conditions before Baseline, retaining an identified version and rationale. Candidate uses the same oracle. If the oracle is wrong, stop this comparison, retain its evidence as superseded for the changed claim, justify the correction separately and obtain any applicable requirement/criteria approval. Establish a new Baseline before evaluating Candidate under the corrected oracle. Compare mode itself authorizes neither this revision nor another run. Keep oracle corrections separate from evidence of a Skill repair.

Identify Baseline/Candidate instructions and dependencies, identical request and starting state, criteria, relevant Skill catalogue/host rules, executor/runtime settings, permissions and budget. Declare the intended change; other condition drift invalidates the affected comparison. Mark conditions that cannot be fixed or observed as unknown and limit the conclusion.

Historical failures locate mechanisms; they are not controlled Baseline reruns. Reuse an existing run only when its identity, conditions and criteria answer the current question. Do not retroactively certify unobserved execution.

Reuse the user-approved scope and applicable execution budget. Read [feedback and regression guidance](../../../references/feedback-regression.md) when comparison-budget guidance, case retrieval/capture or adoption records are actually needed. Without an applicable execution budget, propose the smallest bounded run first. Diagnosis/design does not authorize model trials. Testing does not authorize installation, paid calls, production changes or global adoption.

### Execution and assessment

Supply the executor only the task, applicable methods and necessary materials. Keep evaluator criteria, expected answers and prior conclusions outside its context. Judge actual actions and artifacts against sources, not the executor's self-assessment. Label self-checks and independent assessment separately. Out-of-scope reads or candidate drift invalidate affected conclusions.

| Observation | Execution classification | Use of behavioral evidence |
|---|---|---|
| Normal termination | Completed | Assess each independent criterion; success is not automatic PASS. |
| Predeclared budget exhausted | Timeout | Unfinished checks are UNKNOWN; an intermediate omission is not a final omission. |
| User/controller requests a stop | Cancelled | Retain the reason, observed effects and unfinished checks. |
| Startup, connection, process or executor fault | Error | Identify the failing layer; affected behavior remains UNKNOWN. |
| Condition drift, oracle leakage or scope violation | Comparison invalid | Exclude affected evidence from superiority claims. |
| No execution or missing prerequisite | NOT_RUN / blocked | Name the dependency rather than converting it into success. |

Execution status, comparison validity and item-level behavioral outcomes are separate dimensions. Independently established effects, such as an unauthorized write, may be assessed separately. A truncated artifact missing a requirement does not establish that the finished task would omit it. Preserve uncertainty when the distinction cannot be observed.

Execution evidence should reconstruct start, actual public actions, last activity, termination/stop reason and result identity. Save final snapshots only after stopping processes and confirming writes have ended; otherwise mark the snapshot incomplete. Unpublished internal reasoning is not an execution timeline. Report missing executor capabilities rather than claiming instructions implemented them.

Reuse deterministic checks only while declared relevant dependencies, tools, configuration and evidence remain valid. Missing, erroneous or stale receipts cannot support reuse. Model behavior trials are not deterministic checks to cache. Scripts do not establish unverified semantic truth.

### After execution

Establish comparability before judging target behavior, preservation of the original goal and regression harms. A single paired observation is case-level evidence. Speed, shorter output, successful exit or static validation alone do not establish improvement. If evidence is insufficient, preserve the current valid version and name the smallest additional evidence that could change the conclusion.

## Disposition

| Disposition | Evidence and action |
|---|---|
| Adopt | Current comparable evidence supports target checks and necessary risk-based regression, with no unresolved material regression. Recommend the identified version/scope; actual application awaits applicable authorization. |
| Revise | Evidence identifies a specific repairable gap. Name its responsible layer, minimal revision and affected recheck within the existing budget and authority. |
| Reject | The candidate is unnecessary, unsupported by attribution, or introduces an established material regression. Preserve the valid version and route the issue to its actual owner when needed. |
| Inconclusive | Execution, reproduction, comparability or coverage cannot support a judgment. Stop the affected comparison; report missing evidence, established local facts and resumption conditions. |

A new requirement or mistaken oracle may end attribution with NO_CHANGE; a Skill candidate is optional. Complete the authorized outcome: a design-only request can end with a NOT_RUN plan, while an authorized end-to-end evaluation may continue through its necessary stages. Assessment of existing evidence need not launch another run. Resume dependencies and valid approvals instead of repeating the whole loop.

The entrypoint's mode table owns evaluation-specific work and completion criteria. Determine whether stages are internal steps of an authorized outcome or explicit delivery limits. An end-to-end request may authorize several stages together; crossing an internal boundary alone requires no fresh approval. Design-only and diagnosis-only requests remain limited. Record the outcome, authority source, existing gates and next permitted action at a meaningful boundary. A missing dependency may be built when its construction is already within authorized scope; otherwise report the gap and proposal. This instruction contract is not proof of an enforced Harness gate.

## Capability ownership

| Capability | Owner and loading condition |
|---|---|
| Test mode/level, mechanism validity, evidence judgment and loop disposition | `test-skill`; does not replace cases, execution or authoring methods. |
| Agent Evaluation inputs, expectations, assertions and observation methods | [Case definitions](#case-definitions) in this Reference; optional software test-design support applies only under its software-boundary condition. |
| Failure retrieval/capture, comparison budgets, cross-project results and adoption records | [Feedback and regression](../../../references/feedback-regression.md); maintain no parallel case library here. |
| Creating/updating a Skill and its packaging | `skill-creator`; load after a Skill edit is justified. |
| Instruction hierarchy, pointers, completion criteria and deduplication | `writing-for-agents`; load when authoring agent instructions. |
| Preparation, identity checks, events, stop/snapshot and deterministic-check reuse | Verified Harness/scripts; derive interfaces from testing needs and report gaps rather than change criteria to fit them. |

Resolve named Skills through the actual installed catalogue. This package owns Agent Evaluation case standards and reuses the shared feedback/regression Reference only when needed; software test-case design is optional supporting guidance under the stated condition. It does not require the unadopted project-local design-test-cases or feedback-regression Skill candidates. Missing required capabilities pause their dependent branch while independent diagnosis continues. Recheck the owners and paths during any later workflow migration.

This user-level method package contains Skill-test decisions and evidence judgment only. No Runner, scripts or tests are shipped with it. Native model integration, behavioral effectiveness and cross-project effectiveness require separate evidence and remain unverified. Installation does not authorize an evaluation run.
