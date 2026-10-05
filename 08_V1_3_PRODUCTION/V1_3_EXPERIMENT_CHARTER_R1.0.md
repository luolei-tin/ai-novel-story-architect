# V1.3 Actual Novel Production Experiment — R1.0

## 1. Purpose

V1.3 is the first production experiment of the Story Architect system.

It is not a prose benchmark and not a speed benchmark.

The goal is to verify whether the existing architecture can drive a real long-form novel from seed to chapter production while preserving:

- causal integrity;
- character-choice-driven turning points;
- psychological continuity;
- information integrity;
- world-rule integrity;
- foreshadow lifecycle;
- relationship state;
- long-form state;
- dependency invalidation;
- regression validation;
- red-team rejection when the story does not actually work.

## 2. Experiment Novel

Working title:

> 《重生后，我把一家旧商场做成了现金流》

Genre:

- 重生
- 都市
- 商业
- 长线经营

Target length:

- 30–50 chapters for V1.3
- expansion only after the first production loop proves stable

## 3. Production Rules

### 3.1 Architect Authority

The Story Architect controls:

- Story Core
- character logic
- world constraints
- causal turning points
- outline dependencies
- chapter handoff
- red-team verdicts
- validation state

### 3.2 Writer Authority

The prose writer controls:

- wording
- scene texture
- dialogue expression
- paragraph rhythm
- sensory detail

The writer must not silently redesign:

- final choice;
- core character truth;
- core world rules;
- major causal chain;
- foreshadow timing;
- irreversible state.

### 3.3 Red-Team Independence

The auditor is allowed to issue:

- PASS
- CONDITIONAL PASS
- REVISE
- REJECT

A commercially exciting chapter can still be REJECTED if the causality or character logic does not hold.

## 4. Mandatory Production Loop

For every chapter:

1. snapshot START STATE;
2. generate CHAPTER HANDOFF;
3. produce prose;
4. run Chapter Audit;
5. run Continuity Audit;
6. update END STATE;
7. record dependencies;
8. mark downstream work stale when upstream material changes.

Required loop:

`START STATE + CHAPTER DELTAS = END STATE`

## 5. Mandatory Red-Team Counterfactuals

At every major structural checkpoint, test:

- protagonist refuses the decision;
- protagonist chooses the obvious alternative;
- antagonist remains rational;
- key supporting character is removed;
- one important world rule is removed;
- the ending is changed to a conventional happy ending;
- the ending is changed to a tragedy.

A counterfactual is not automatically a flaw. It is evidence used to test necessity.

## 6. Success Criteria

V1.3 is successful only if a real chapter sequence demonstrates:

- at least one turning point caused by a protagonist choice;
- at least one turning point caused by a relationship change;
- at least one commercial obstacle resolved through constrained trade-offs rather than luck;
- at least one rejected chapter or revision;
- at least one upstream change producing targeted STALE states;
- successful regression validation after that change;
- a final choice that is not interchangeable with a generic happy ending.

## 7. Failure Policy

The experiment must not protect the story from rejection.

If a chapter fails:

`DRAFT → QA_REVISE / REJECT → REPAIR → TARGETED REVALIDATION → REVIEW`

Never:

`REJECT → PASS`

## 8. Current State

V1.3 starts at:

`SEED`

The next required state is:

`CORE_DRAFT`

No chapter writing is authorized before the core reaches the required validation threshold.
