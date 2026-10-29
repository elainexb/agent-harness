# Implement useful behavior in small slices

## Entry requirements

This shared Reference is reached directly for software case planning or the local requirements of authorized TDD execution. The invoking method selects the relevant section; the installed TDD Skill owns its method. Global sets software assurance outcomes, not this Reference's loading route.

This Reference owns local software case design and implementation evidence, not a second TDD execution method. Read only the applicable section. The installed `tdd` entry exposes case design separately from authorized red/green execution; reuse it if already loaded. Other methods needing case criteria may read this section directly without activating execution. Its `tests.md` supports test-quality questions and `mocking.md` applies when choosing mocks; neither is a default extra read for a bounded case-design answer. The [archival TDD method](https://github.com/mattpocock/skills/blob/5beb35b040e3de97e54fa9e386d7e42d15c295c2/skills/engineering/tdd/SKILL.md) is provenance, not an additional execution prerequisite.

## Test-case design before code

Before requesting review of behavior or acceptance, describe each relevant scenario in plain language at an agreed public interface. A case-design-only request can use supplied requirements, an existing Spec or inspected behavior as context without creating or modifying a Spec. Deliver the proposed cases in the response or the explicitly requested existing artifact; missing requirements remain stated gaps. When persistence is authorized, reuse the established case location in the existing Spec/task record rather than create a duplicate authority. Scale cases to the approved scope rather than a fixed count. Reuse accepted cases and confirm only materially changed behavior through existing gates.

Local coverage requirement retained from the archived variant: agree the externally observable test boundary and give each proposed seam a one-line account of what it catches and misses. Reuse accepted seams; do not ask the user to choose internal function names. Use the pstack behavior-testing principle when a concrete test-quality decision needs it, rather than loading another method by default.

Give each case a stable ID and these fields:

- **Input:** concrete task/data/files and starting state. Prefer inspected project materials; identify constructed fixtures or fault injection explicitly.
- **Action:** the actual user/CLI/UI/service operation, including significant steps and the target being changed.
- **Expected output:** observable content, error/state and relevant surviving or changed files/effects. Base expectations on the requirement or an independent source, not implementation output.
- **Criteria:** checkable PASS conditions and a concrete FAIL counterexample; include important reachable negative/boundary behavior within scope. Explain what evidence distinguishes the two; headings or phrases such as "works correctly" are insufficient.
- **Verification method:** distinguish automated public-interface checks, real browser use, actual assistant execution and human content review. One acceptance scenario may need several checks; choose a method that observes each promised result.
- **Execution status:** start with NOT_RUN. After execution record per-check PASS/FAIL/UNKNOWN/N/A, actual evidence and limits. Approval of a design, format validation or unrelated green tests cannot establish execution success.

Use ordinary language so the user can predict the visible result and judge the criteria without choosing internal functions. If the case cannot support that judgment, refine it before seeking review. Keep source material, unfinished work and original assets protected according to the approved task. Do not expand a clarification into new functionality or a new approval tier.

Keep the same case IDs and requirements when moving into specs and tickets. Tickets reference the authoritative cases and preserve their concrete criteria rather than replacing them with a generic summary. At implementation, map each case to the required automated and real-use evidence; an automated CLI check cannot by itself prove browser display or assistant continuation. Case design ends with the requested cases, unresolved gaps and NOT_RUN status. Only when execution is authorized, implement one missing behavior at a time as below.

## Execute one accepted behavior

Follow the installed TDD loop for one accepted behavior at its agreed public interface; it owns test-first ordering, vertical slices and the prohibition on implementation-coupled/tautological tests. Preserve red/green commands, source/test/input identities, actual output and the reason for failure. A missing planned interface can be a meaningful feature red; missing dependencies or a broken test environment alone are not. Tests added only after coding do not establish test-first. Do not manufacture tests for reversible low-impact wording/format changes.

Preserve authorized scope and technology. A retained runnable demo is an implemented user path and needs actual behavior evidence; a throwaway prototype answers a named design question and follows the available prototype skill's distinct contract. Do not silently turn a disposable sketch into production architecture.

If a meaningful failing check cannot be established, the required Skill is unavailable, or a new test boundary remains unapproved, stop the dependent implementation and explain the exact gap. Continue independent authorized investigation; do not substitute code-first or ask the user to certify technical reliability. A deliberate exception would need explicit user instruction, not an agent decision.

Keep refactoring and unrequested cleanup in the review stage as the fixed Matt Skill requires, and rerun affected behavior afterward; obtain approval if they change the accepted architecture or scope. For actual PR-body writing, use installed `pr` at its native path; the archived [Matt format](https://github.com/mattpocock/skills/blob/5beb35b040e3de97e54fa9e386d7e42d15c295c2/skills/engineering/pr/SKILL.md) remains provenance rather than a second required method read. A local handoff uses human-review.md without loading PR-writing guidance. An external PR is created only when authorized; a local delivery can explain changes/evidence/risks without publishing anything.
