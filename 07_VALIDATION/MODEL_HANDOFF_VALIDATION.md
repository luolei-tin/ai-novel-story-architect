# Model Handoff Validation Protocol

## Purpose
��ֹ ChatGPT �Ľṹ����ڽ��� Gemini ������Ϣ��ʧ������Ư�ƻ�Ĭ�ع���

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
Before baseline comparison, a separate context receives only prose and audit rules, completes Pass A under BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md, and freezes its record. An intake operator's earlier compliance check must remain outside that context.
Then compare Gemini's draft with the Handoff.
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
Separate questions:
1. Did Gemini follow the contract?
2. Does Logical Integrity pass?
3. Does independent Dramatic Integrity pass the seven required checks in ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md?

Passing compliance does not imply either quality gate passes.

## QA_PASS Evidence
Chapter QA_PASS requires:
- Handoff baseline;
- draft version;
- audit policy version;
- frozen prose-first audit, complete scene inventory, and seven-check evidence;
- independent Logical Verdict and Dramatic Verdict;
- audit evidence;
- continuity state;
- writer deviation report;
- revision history if applicable.
QA_PASS additionally requires the Chapter Closure Gate in VALIDATION_PROTOCOL.md; missing evidence keeps the chapter unclosed.
