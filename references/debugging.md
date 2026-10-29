# Diagnose the reported bug

Use this local adaptation with installed `diagnosing-bugs` at its native catalogue path when the reported mechanism is unresolved. The installed Skill owns reproduction, hypothesis selection and the diagnosis loop; do not also load the full [archival variant](https://github.com/mattpocock/skills/blob/5beb35b040e3de97e54fa9e386d7e42d15c295c2/skills/engineering/diagnosing-bugs/SKILL.md) as an execution prerequisite. Reuse established diagnosis and valid evidence when proceeding to an authorized repair.

## Local evidence and execution conditions

Build an observable loop for the user's exact failure before claiming a cause or fix: an existing meaningful test, CLI/UI operation, captured trace or mechanism-preserving reproduction can supply it. Keep secrets out of artifacts. Distinguish source-supported hypotheses from actual reproduction; retain observations that distinguish competing explanations.

A flaky failure needs an observed reproduction rate and finite limits, not a claim of determinism. Upstream example iteration counts do not authorize expensive or production instrumentation. Experiments stay within the actual effects and budget.

Retain the archived variant's additional safeguard: if a failing check is forced by changing code or a fixture, diff it against a pristine copy to establish that the intended mutation landed before trusting the red. Record the injected condition as constructed evidence, not an original failure. This requirement is the local difference; it does not require rereading both full methods.

## Transition to repair

For an authorized behavior-changing repair, follow installed `tdd` with [entry requirements](implementation.md#entry-requirements) and [local execution requirements](implementation.md#execute-one-accepted-behavior). Retain a meaningful check failing before the fix and passing after it, then rerun the original user scenario. Missing boundary/reproduction leaves dependent repair unverified; report attempts, failures and the missing fact rather than substituting code-first.

Remove only debugging artifacts created for this task. Use available tools for inspectable facts; do not ask the user to perform checks the agent can actually do. Recording and cleanup remain subject to the current effect limits.
