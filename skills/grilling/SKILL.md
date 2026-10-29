---
name: grilling
description: Resolve consequential user choices about a plan, decision or idea, including Spec-backed decisions; provide delegated interviews. Fact lookup and settled decisions need no interview.
---

## Local entry boundary

This entry owns the default interview-method choice. First establish that a consequential unresolved user decision actually needs an interview; a relevant Spec alone is insufficient. Inspect facts and reuse confirmed decisions.

With no legitimate interview method explicitly selected: when a relevant Spec exists, prefer `grill-with-docs`; otherwise use the interview below. Inspect the wrapper's actual native invocation policy. While it is explicit-only and has not been invoked, recommend `$grill-with-docs` and pause only the dependent interview; continue independent authorized work. Do not invoke it implicitly or silently fall back to ordinary Grilling. Policy inspection is not wrapper execution.

Valid explicit use retains the selected method's original scope. In `grill-with-docs` delegation, perform the interview below within its current plan/design scope and relevant Spec; do not repeat method selection or recursively enter the wrapper. Confirm only unsettled consequential choices before dependent action.

## Installed method

Interview the user relentlessly until you reach a shared understanding. Map this as a **design tree**: every decision branches into the decisions that hang off it.

Work the tree in **rounds**. The **frontier** is every decision whose prerequisites are already settled: the questions you can ask _now_ without guessing at answers you haven't heard yet. Ask the whole frontier in one round: number each question and give your recommended answer. Then wait for the user's answers before the next round.

Format a round like so:

```
❓ **Q1** - **<question title>**: <question body, might be multiple paragraphs, including multiple choices>

➡️ <your recommended answer>

---

❓ **Q2** - **<question title>**: <question body, might be multiple paragraphs, including multiple choices>

➡️ <your recommended answer>
```

Each round the user answers reshapes the tree: settled decisions push the frontier outward and unblock questions that depended on them. Recompute the frontier and ask the next round. A question whose answer depends on another question still open in this round belongs to a _later_ round, not this one.

Finding _facts_ is your job, never the user's. When a frontier question needs a fact from the environment (filesystem, tools, etc.), dispatch a sub-agent to find it; don't ask the user for anything you could look up yourself. Don't block on it: a running exploration is an unsettled prerequisite, so only the questions downstream of it wait for the sub-agent to report; ask the rest of the frontier now. The _decisions_ are the user's: put each to them and wait.

The session is done when the frontier is empty: every branch of the design tree visited, nothing left silently assumed. Do not act on it until the user confirms you have reached a shared understanding.
