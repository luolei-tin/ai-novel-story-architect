# Model Handoff Validation Protocol

## Purpose
防止 ChatGPT 的结构设计在交给 Gemini 后发生信息丢失、语义漂移或静默重构。

## Pre-Write Gate
ChatGPT must verify:
1. Story Core version is known.
2. Character version is known.
3. World-rule baseline is known.
4. Outline/turning-point baseline is known.
5. Starting State is authoritative.
6. Ending State is explicit.
7. Dramatic Situation contains opposing objectives.
8. Information Control is explicit.
9. Forbidden Moves are explicit.
10. Foreshadow requirements are explicit.

If missing information could change the chapter, status = NOT READY.

## Draft Intake
Before auditing quality, ChatGPT compares Gemini's draft with the Handoff.
Check:
- structural deviations;
- new facts;
- changed knowledge;
- changed resources;
- changed relationships;
- changed timing;
- altered causal order;
- omitted required state change.

Classify each deviation:
- Authorized interpretation;
- Benign expression variation;
- Structural deviation requiring approval;
- Causal defect;
- Continuity defect.

A deviation is not automatically wrong. Silent structural deviation is a process defect even if the result is attractive.

## Writer Deviation Report
Gemini must explicitly disclose deviations.
Missing disclosure is a process defect and must be recorded.

## Separate Gates
Two separate questions:
1. Did Gemini follow the contract?
2. Is the resulting chapter good and logically sound?

Passing the first does not imply passing the second.

## QA_PASS Evidence
Chapter QA_PASS requires:
- Handoff baseline;
- draft version;
- audit evidence;
- continuity state;
- writer deviation report;
- revision history if applicable.