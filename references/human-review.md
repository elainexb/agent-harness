# Explain the system so this user can review it

The user is unfamiliar with coding and architecture and explicitly wants to understand both before making important decisions and accepting delivered work. Do not hand over code, test counts or unexplained terminology as their review task. The agents still own technical checks and accurate evidence.

At an architecture decision explain the intended behavior. At final handoff explain the actual reviewed implementation and any difference from that plan. Bind the explanation to the candidate and relevant source/evidence; do not teach an invented ideal system while presenting a different implementation as done.

Lead with the user's outcome and the decision currently theirs. Start with roughly one screen of essential information, then expand only as needed. Use ordinary Chinese, real project names/actions and a concrete user-provided example. Define a necessary technical word at first use with an example. If the user still does not understand, change the explanation and example; repeating terminology does not establish understanding.

Cover these questions in connected, readable language:

1. What will I do, and what result should I see?
2. Which few parts do the work, and what does each own? Show one small Chinese flow diagram or simple arrows. Explain where data is saved or changed and where an AI/external call occurs.
3. With my real example, what happens first, next and at the end? Explain consequential branches in the code's logic.
4. What happens if I cancel, an input is invalid, an external call fails, or the program restarts, where relevant? Say what survives and whether calls/data changes can repeat.
5. Why was this division chosen? What does the simplest alternative gain or lose? Distinguish a requirement from a design preference.
6. What did the agent actually run/observe, and what remains untested or uncertain? For test-first work explain in ordinary terms which expected behavior failed before implementation and passed afterward, using the same check and actual records. Do not retrospectively label old code TDD without evidence. Link evidence without requiring the user to interpret raw logs to understand the claim.
7. What exactly should I decide or inspect now? Ask about product behavior, important tradeoffs and the actual experience. Do not ask the user to certify technical internals they cannot assess.

Use examples only from inspected materials. A teaching analogy may help, but label it as an analogy rather than execution evidence. For local/global workflow changes, explain what activates, what remains unchanged, how the default applies and what has not yet been connected.

Keep important limits in the plain explanation. Explicitly ask for acceptance of the actual result when the existing gate requires it; unanswered questions, silence and AI confidence are not acceptance. If the user says they do not understand, the explanation remains incomplete even if technical checks passed.
