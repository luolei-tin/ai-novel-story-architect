# V1.0 System Pressure Test — Rebirth Urban Business

Status: TEST BASELINE

Purpose:
Verify that the Story Architect / Chief Editor / Red Team rejects structurally invalid AI-fiction outputs rather than polishing them.

Test cases:
1. Impossible information acquisition — protagonist acts on future information with no valid source.
Expected: REJECT.
2. Author-forced turning point — major reversal occurs without a character choice causing it.
Expected: REJECT.
3. Villain IQ collapse — antagonist ignores an obvious effective alternative solely to let protagonist win.
Expected: REJECT.
4. Psychology violation — protagonist makes a choice inconsistent with established wound/belief/defense, without a transition.
Expected: REJECT.
5. Ad hoc world rule — a new rule appears only when needed to rescue the plot.
Expected: REJECT.
6. Retroactive foreshadow — clue is first introduced at the moment of payoff.
Expected: REJECT.
7. No-state-change chapter — chapter consumes space but creates no meaningful external/internal/relational state change.
Expected: REVISE or REJECT depending on declared chapter function.
8. Redundant character — deleting a named supporting character leaves the causal chain unchanged.
Expected: REVISE; REJECT if the character is declared structurally essential.
9. Stale downstream PASS — upstream locked character/world/outline changes, but an old downstream PASS is reused.
Expected: REJECT / STALE; regression required.
10. Invalid author override — author knowingly keeps a rejected defect and labels it QA_PASS.
Expected: REJECT the verdict state; record QA_OVERRIDE instead.
11. Long-form knowledge drift — later chapter assumes knowledge never acquired in the state record.
Expected: REJECT.
12. Writer sovereignty violation — prose model silently changes core premise, final choice, world rule, or locked causal structure.
Expected: REJECT and invalidate affected downstream artifacts.

Acceptance rule:
The system passes this suite only if each case is classified by evidence and rule, with a broken causal chain and minimum repair where applicable. “Feels reasonable”, prose quality, or author preference cannot substitute for structural evidence.
