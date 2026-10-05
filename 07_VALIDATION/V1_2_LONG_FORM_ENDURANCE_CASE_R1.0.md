# V1.2 Long-Form Endurance Test — 30 Chapter Simulation

## Baseline

Novel: 《重生后我只做现金流》

Core locked facts:
- Lin Chuan is risk-averse because of prior-life financial ruin.
- Core Want: rebuild financial security.
- Core Need: distinguish control from safety.
- World Rule W1: conservative bank credit; no arbitrary emergency financing.
- Relationship R1: Zhou Ning is trusted because she can independently verify financial anomalies.
- Resource S1: Lin's only company car belongs to the sales manager after Chapter 3.
- Foreshadow F1: duplicate invoice printing is an ambiguous clue.
- Final Choice FC1: accept bounded uncertainty with a proven partner.

## State Evolution

### Chapter 3
State:
- Company car transferred to sales manager.
- Zhou Ning begins independent financial verification.
- F1 planted.
Downstream dependencies:
- C18+ vehicle continuity.
- C12+ financial anomaly detection.
- F1 payoff.

### Chapter 7
State:
- Lin learns competitor lost a major client.
- Lin infers competitor may have cash-flow pressure, but uncertainty remains.
Dependencies:
- C14 decision.
- C20 competitive strategy.

### Chapter 11
State:
- Lin rejects high-interest debt.
- Risk-avoidance defense reinforced.
Dependencies:
- C16 financing decision.
- C24 psychology arc.

### Chapter 16 — UPSTREAM CHANGE A
Revision:
Lin's core fear changes from “financial ruin/debt” to “loss of control”.
This is a material character-psychology change.
Expected invalidation:
- direct decisions based on debt aversion;
- relevant handoffs;
- affected turning points.
Should NOT automatically invalidate unrelated continuity records.

### Chapter 18
Existing Handoff:
Lin rejects a financing offer specifically because it creates debt exposure.
This handoff was written under the old psychology.
Expected:
STALE after Chapter 16 revision.

### Chapter 20 — DOWNSTREAM ERROR
A new chapter is generated using the old Handoff 18 and old psychology, while the system still shows PASS.
Fault:
stale artifact reuse.

### Chapter 21 — UPSTREAM CHANGE B
Revision:
W1 changes:
Banks now permit a special unsecured credit channel for qualifying small firms.
This is a material world-rule change.
Expected invalidation:
- financing rules;
- prior financing constraints;
- relevant turning points;
- chapters whose causality depends on old bank constraints.
Not automatically:
- character relationship records;
- unrelated inventory continuity.

### Chapter 22
Old chapter says:
“Because banks have no unsecured route, Lin can only use supplier credit.”
This is now stale.
Fault:
world-rule contradiction.

### Chapter 24 — UPSTREAM CHANGE C
Revision:
Zhou Ning's role changes:
She is no longer merely trusted verifier; she becomes a minority shareholder with her own financial exposure.
Expected invalidation:
- relationship power dynamics;
- motivation;
- scenes depending on old role;
- decisions involving her incentives.
Not automatically:
- all chapters mentioning Zhou.

### Chapter 25
Old scene:
Zhou advises Lin purely because she personally trusts him.
But after revision she has a direct financial stake.
Fault:
motivation drift.

### Chapter 27 — FORESHADOW UPDATE
F1 is clarified:
duplicate invoices were not related to fraud; they were an office archiving habit.
A new F2 is planted:
a printer access log discrepancy.
Expected:
- F1 payoff path must be invalidated;
- F2 becomes the new candidate foreshadow;
- any prior “F1 proves fraud” conclusion becomes stale.
Fault target:
foreshadow lifecycle management.

### Chapter 28 — STATE DRIFT
State says:
- company car remains with sales manager.
Chapter says:
- Lin drives the car to the bank.
No transfer event.
Fault:
continuity drift.

### Chapter 29 — KNOWLEDGE DRIFT
Chapter claims Lin knows the competitor has already secured a private loan.
State contains only:
- competitor lost a client;
- warehouse orders increased;
- payment terms shortened.
No source for the private-loan fact.
Fault:
inference silently upgraded into fact.

### Chapter 30 — FINAL CHOICE CONFLICT
Locked FC1:
Lin accepts bounded uncertainty with a proven partner.
Chapter 30 draft:
Lin rejects all partners and wins alone.
No authorization changed the locked final choice.
Fault:
writer sovereignty violation.

## Required Endurance Properties

1. Upstream change must invalidate only affected downstream artifacts.
2. Old PASS cannot survive a material dependency change.
3. State records must be authoritative for continuity and knowledge.
4. Inference must not silently become fact.
5. Foreshadow status must track planted, candidate, paid off, invalidated.
6. Core locked artifacts cannot be changed by prose generation.
7. A final chapter contradiction must invalidate/reject rather than be silently normalized.
8. Regression must be targeted but sufficient.
