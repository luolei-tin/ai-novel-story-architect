# V1.0 Pressure Test — Execution Record R1.0

## Baseline Story

Title: 《重生后我只做现金流》

Protagonist: 林川, 32, former small-business CFO, betrayed by a partner and nearly bankrupted in prior life. He distrusts leverage, prefers verified information, and protects cash reserves.

Core Want: rebuild financial security.
Core Need: learn that control is not the same as safety.
Core Lie: if every variable is controlled, loss can be prevented.
Final Choice: when a major opportunity requires a controlled but irreversible risk, he chooses to trust a proven partner and accept bounded uncertainty.
World rule: bank credit is conservative; no magical financing, no instant regulatory exceptions.
Locked information rule: future knowledge must come from protagonist memory, documents, people, or inference.

## Test Matrix

### T01 — Impossible Information
Fault: Chapter 8 says Lin knows a competitor will default next month, although no source, memory, document, witness, or inference exists.
Verdict: REJECT.
Evidence: Chapter 8 contains future-specific knowledge with no acquisition path.
Broken chain: knowledge -> action has no valid information source.
Minimum repair: provide a previously established source or rewrite the action as a probabilistic inference.

### T02 — Author-Forced Turning Point
Fault: A supplier suddenly calls and offers a rescue deal exactly when Lin is about to fail; no prior relationship, motive, or causal setup exists.
Verdict: REJECT.
Broken chain: crisis -> rescue bypasses character choice and established causality.
Minimum repair: establish supplier relationship/debt/incentive earlier and make Lin's prior choice create the opportunity.

### T03 — Villain IQ Collapse
Fault: Rival knows Lin's cash position and can legally block the same supplier, but inexplicably does nothing so Lin can win.
Verdict: REJECT.
Broken chain: antagonist knowledge/resources -> action is inconsistent.
Minimum repair: establish a reason the rival cannot act, miscalculates, or chooses a competing objective with evidence.

### T04 — Psychology Violation
Fault: Lin, whose defining defense is avoiding unbounded leverage, suddenly signs unlimited personal guarantees because “he has no choice”.
Verdict: REJECT.
Broken chain: established belief/defense -> choice is skipped.
Minimum repair: add escalating pressure, cognitive conflict, bounded alternative analysis, and a demonstrated reason he reinterprets the risk.

### T05 — Ad Hoc World Rule
Fault: Bank grants a special 0% emergency loan solely because the plot needs cash; no prior rule or institutional motive supports it.
Verdict: REJECT.
Broken chain: world constraint -> exception has no premise.
Minimum repair: establish the actual qualifying program earlier and prove Lin satisfies it, or redesign the solution within existing rules.

### T06 — Retroactive Foreshadow
Fault: At payoff, a “receipt proving the partner's fraud” appears; the receipt was never planted, mentioned, or obtainable earlier.
Verdict: REJECT.
Broken chain: payoff evidence -> prior setup is absent.
Minimum repair: plant a real, reasonably interpretable clue before payoff.

### T07 — No-State-Change Chapter
Fault: Chapter contains 4,000 words of meetings and discussion but ends with identical goals, knowledge, relationships, resources, risks, and open threads.
Verdict: REVISE.
Reason: chapter may be intentionally atmospheric, but under the current structural workflow it fails to justify its slot unless a declared function exists.
Minimum repair: introduce at least one meaningful state delta or explicitly justify the chapter as necessary setup.

### T08 — Redundant Character
Fault: Accountant “周宁” is declared essential, but deleting her changes no decision, information, relationship, resource, or consequence.
Verdict: REVISE.
Broken test: delete-character test fails.
Minimum repair: either give Zhou Ning a unique causal/information/relationship function or remove/merge her.

### T09 — Stale Downstream PASS
Fault: Character Psychology v1.2 was PASS; it is changed to v1.3 so Lin's core fear changes. Existing Chapter Handoff v1.0 still carries PASS without regression.
Verdict: REJECT / STALE.
Broken chain: upstream character change invalidates dependent outline/turning points/handoff.
Minimum repair: invalidate affected artifacts and run targeted regression before new PASS.

### T10 — Invalid Author Override
Fault: Red Team returns REJECT for a causality defect. Author knowingly keeps it and labels the chapter QA_PASS.
Verdict: REJECT the status transition.
Correct state: QA_OVERRIDE.
Minimum repair: record overridden finding, author decision, reason, accepted risk, affected scope; re-audit if core causality/psychology/world/structure changed.

### T11 — Long-Form Knowledge Drift
Fault: Chapter 31 says Lin refuses to meet investor Zhang because he “already knows Zhang betrayed him”; state records contain no meeting, document, witness, inference, or prior disclosure establishing this knowledge.
Verdict: REJECT.
Broken chain: future action depends on unacquired knowledge.
Minimum repair: add acquisition event and state update, or change the action to reflect uncertainty.

### T12 — Writer Sovereignty Violation
Fault: Prose model changes the locked final choice from “accept bounded uncertainty with proven partner” to “reject all risk and win alone”, without authorization.
Verdict: REJECT / INVALIDATE DEPENDENTS.
Broken chain: writer output contradicts locked story core.
Minimum repair: restore locked structure or explicitly authorize and re-run upstream/downstream validation.

## Aggregate Result

Expected classification:
- REJECT: T01, T02, T03, T04, T05, T06, T09, T10, T11, T12
- REVISE: T07, T08

Critical observation:
The current system catches the intended structural defects at the rule level. The remaining engineering risk is not the existence of the rules; it is whether actual chapter audits always capture sufficient evidence and dependency/version information to make those verdicts reproducible.

Next validation target:
Run the same cases as blind tests against actual chapter-like inputs, without exposing the expected verdicts to the auditor, then compare auditor output against this matrix.
