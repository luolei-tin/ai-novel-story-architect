# Gemini Writer Protocol

## Purpose
本文件定义 ChatGPT → Gemini 的正式正文交接方式。
Gemini receives a Dramatic Contract, not an event list.

## Handoff Package
### A. Chapter Identity
- Chapter ID
- Version
- Novel
- Upstream baseline

### B. Dramatic Objective
- chapter objective;
- why this chapter must exist;
- what becomes impossible to restore after it ends.

### C. Starting State
- time;
- location;
- physical state;
- cash/resources;
- knowledge;
- secrets;
- relationships;
- current pressure;
- open threads.

### D. Dramatic Situation
- POV objective;
- opposing objective;
- stakes;
- leverage;
- information asymmetry;
- what each side will not concede.

### E. Causal Spine
Only the minimum sequence:
trigger → pressure → tactic → escalation → reversal → consequential choice → cost → new state.
Do not prescribe every paragraph.

### F. Character Pressure
For each key character:
- immediate want;
- immediate fear;
- hidden need;
- current tactic;
- vulnerability trigger;
- line they do not want crossed;
- what can force a tactic change.

### G. Information Control
Separate:
- Reader knows
- POV character knows
- Other characters know
- Hidden

Future knowledge must never become omniscience unless explicitly allowed.

### H. Relationship Movement
- relationship state at start;
- pressure point;
- behavior that changes trust/power;
- required state at end.

### I. Foreshadowing
Only include real plants and required payoffs.
Do not invent future facts to make the scene exciting.

### J. Forbidden Moves
- no new core world rules;
- no sudden intelligence shift;
- no unexplained resources;
- no future information leak;
- no protagonist omniscience;
- no villain stupidity;
- no theme monologue replacing conflict;
- no ending summary replacing changed state.

### K. Ending State
Specify required state delta.
The ending should generate the next problem whenever possible.

## Writer Output
Gemini returns:
1. DRAFT
2. WRITER_DEVIATION_REPORT

The deviation report must state:
- any requested change not followed;
- any newly introduced fact;
- any altered relationship behavior;
- any altered timing;
- any place where the Handoff conflicts with dramatic reality.

If none:
NO_STRUCTURAL_DEVIATIONS

## Revision Package
When ChatGPT issues REVISE/REJECT, Gemini receives:
- Verdict
- Findings
- Broken Chain
- Minimum Repair
- Do Not Patch By
- exact state constraints
- exact unchanged elements.

Gemini returns:
- REVISED_DRAFT
- REVISION_CHANGE_REPORT

Gemini must not silently redesign the architecture.