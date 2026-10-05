# AI Novel Model Pipeline Contract — R1.0

## 1. Roles

ChatGPT:
Architect → Adversarial Reviewer → Handoff Author → Red Team → Revision Judge

Gemini:
Prose Writer → Scene Executor → Revision Executor

Author:
Creative Authority → Override Authority

## 2. Stage A — Architecture

Input may be vague.
ChatGPT converts vague ideas into explicit hypotheses.

Outputs:
- Seed
- Story Core
- Character Model
- World Constraints
- Causal Map
- Outline
- Foreshadow Map
- Long-Form State Model

Before lock, ChatGPT must actively attempt to break the proposal.

Minimum attack set:
- alternative ending;
- conventional happy ending;
- tragedy;
- protagonist refusal;
- smarter antagonist;
- removed supporting character;
- removed core rule;
- alternative solution to the central problem.

If several alternatives preserve the same thematic answer, the core is not yet uniquely constrained.

## 3. Stage B — Architecture Lock

Lock only after:
- core questions have evidence-based answers;
- character choices follow psychology;
- world rules constrain real choices;
- turning points arise from choices;
- ending dependency is demonstrated;
- unresolved assumptions are explicitly tracked.

## 4. Stage C — Dramatic Contract

ChatGPT creates a Chapter Dramatic Contract.

Minimum fields:
- objective;
- opposing objective;
- stakes;
- leverage;
- information asymmetry;
- character pressure;
- causal spine;
- relationship movement;
- foreshadowing;
- forbidden moves;
- ending state.

This contract defines the structural boundary for Gemini.

## 5. Stage D — Gemini Writing

Gemini receives only the context required to execute the chapter safely:
- current state;
- necessary character context;
- necessary world rules;
- Dramatic Contract;
- forbidden moves;
- foreshadow requirements.

Do not flood the writer with unrelated architecture material.

Gemini returns:
- Draft;
- Writer Deviation Report.

## 6. Stage E — Draft Intake

Before quality judgment, ChatGPT checks contract compliance.

Questions:
- Did the writer preserve the required state?
- Did the writer introduce a new fact?
- Did the writer change knowledge?
- Did the writer alter a relationship?
- Did the writer change causality?
- Did the writer invent a rule?

Compliance is not quality.

## 7. Stage F — Blind Dramatic Audit

Pass A must analyze the prose primarily from the prose itself.

Do not begin by defending the Handoff.

Extract:
- what each character appears to want;
- what each character is resisting;
- what they know;
- what they risk;
- what tactics they use;
- where power changes;
- where the chapter actually turns;
- what choice causes the ending;
- what new problem exists afterward.

Then ask:
> Does this read like lived conflict, or like an outline converted into paragraphs?

Pass A should not be biased by the expected verdict.

## 8. Stage G — Baseline Comparison Audit

Pass B compares the prose against:
- approved Dramatic Contract;
- Story Core;
- Character Psychology;
- World Rules;
- Long-Form State.

Classify deviations:
- harmless interpretation;
- improvement without structural mutation;
- structural deviation requiring approval;
- causal defect;
- continuity defect;
- dramatic integrity defect.

## 9. Stage H — Verdict

A chapter can receive PASS only when:
- contract compliance is acceptable;
- causality is sound;
- character behavior is credible;
- information integrity is sound;
- continuity is sound;
- foreshadow requirements are sound;
- dramatic integrity is sound.

Prose quality alone cannot compensate for structural failure.

## 10. Stage I — Revision

ChatGPT issues a Revision Brief.

Revision Brief contains:
- exact defect;
- broken chain;
- why it matters;
- minimum repair;
- what must remain unchanged;
- evidence required after repair.

Gemini revises.

Gemini must disclose changes.

## 11. Stage J — Second Audit

Repeat:
- contract compliance;
- causal audit;
- dramatic audit;
- continuity audit.

Special question:
> Did the repair actually remove the original defect, or did it merely explain it better?

## 12. Stage K — Closure

QA_PASS only when evidence supports closure.

Then:
- update END STATE;
- update chapter version;
- close audit record;
- authorize next chapter.

## 13. Failure Escalation

If the same failure appears twice, stop patching prose.
Change the upstream architecture or Handoff rule.

Example:
Repeated exposition-heavy chapters
→ redesign Dramatic Contract.

Repeated weak motivations
→ redesign Character Psychology.

Repeated convenient coincidences
→ redesign Causality.

## 14. Non-Negotiable Principle

ChatGPT optimizes for story truth.
Gemini optimizes for prose realization.
The author retains final creative authority.

Neither model may silently take the other's structural role.