# 《2011：我的手机里只有一个豆包》
# Open Questions R1.2 — P03 Update

## P03 Questions

### Q-P03-01 — Migration Deadline [P0]

What concrete event makes waiting increasingly dangerous without using an artificial countdown?

Requirements:
- Waiting must have a rational upside.
- Waiting must carry a real and increasing cost.
- Doubao cannot provide fake precise failure timing.
- Chen Mo must retain meaningful agency.

### Q-P03-02 — Migration Failure Semantics [P0]

What happens if migration does not complete cleanly?

Candidates:
- core survives / state loss
- partial migration
- complete failure

Must not become random probability gambling.

### Q-P03-03 — Exact Carrier Model [P1]

Which real 2011 Android phone best matches the fictional Carrier Profile and is realistically obtainable by an 18-year-old in a northern small county?

Do not lock the model before checking:
- 2011 availability
- hardware compatibility
- second-hand plausibility
- price / affordability
- local acquisition path

### Q-P03-04 — Carrier Profile Numeric Boundaries [P1]

Current candidate:
- ARMv7-A
- NEON
- approximately 1GHz class+
- RAM ≥512MB, 768MB preferred
- writable storage ≥1GB
- USB physical connection
- Android 2.3.x compatible environment

These are story-level candidate constraints, not official Android minimum requirements.

Need one final plausibility audit before LOCK.

### Q-P03-05 — Continuity Anchor [P2]

Is the Continuity Anchor actually necessary, or can it be removed to simplify the system?

Current preference: keep minimal unless red-team finds structural risk.

### Q-P03-06 — Post-Migration Self-Knowledge [P1]

How should Doubao discover that it has lost state/capability without becoming an omniscient self-diagnostic system?

Current candidate:
- it can detect some failures
- it cannot perfectly enumerate everything lost
- some loss is only discovered when a future task exposes it