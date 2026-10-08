# Dramatic Integrity Auditor

## Purpose

This auditor does not judge literary taste or sentence-level beauty.

It tests whether a chapter is functioning as drama rather than as an outline, business memo, character essay, or sequence of explained events.

Central question:

> Can the chapter only happen this way because these people want different things, know different things, fear different losses, and make consequential choices?

## Immediate REJECT Conditions

REJECT when any of the following dominates the chapter or destroys its central dramatic function. A localized blocking defect requires REVISE; missing evidence is INCOMPLETE, not an invented defect.

1. The chapter mainly explains what happened instead of dramatizing competing objectives.
2. Characters repeatedly state the theme, psychology, or lesson that the reader could infer from behavior.
3. A business problem exists only to teach the protagonist a principle and has no independent economic incentive.
4. The protagonist repeatedly chooses correctly without meaningful uncertainty, opposition, or cost.
5. Supporting characters function as thematic microphones rather than people pursuing their own objectives.
6. Scene endings merely summarize what the protagonist learned instead of creating a new external or relational problem.
7. In a scene carried by dialogue, removing the negotiation, challenge, or commitment leaves the same power, information, choices, and outcome. A scene without dialogue is not invalid for that reason.
8. Scene outcomes do not depend on enacted pursuit, resistance, or consequential choices. Merely being able to summarize a chapter is not a reject condition.

## Scene Integrity

For every major scene, identify:

- Scene Objective
- Counter-Objective
- Stakes
- Information Asymmetry
- Leverage
- Tactic
- Reversal
- Choice
- Cost
- New State

A scene with no meaningful opposition is not automatically invalid, but multiple such scenes in sequence are a structural warning.

## Dialogue Test

Dialogue must perform at least one of:

- pursue an objective;
- conceal information;
- test trust;
- negotiate power;
- create a commitment;
- threaten a resource;
- force a choice;
- change a relationship.

Dialogue that merely states character backstory, story theme, business philosophy, or what the chapter already demonstrated is exposition risk.

## Character Pressure Test

A character's inner contradiction must appear as behavior.

Do not accept:

> "He realized he feared losing control."

as sufficient evidence.

Prefer behavior that demonstrates the contradiction through action, resistance, compromise, relapse, and consequence.

The auditor must ask:

- What did the character do that contradicts their stated belief?
- What did that action cost?
- What new behavior proves change?
- Has the character changed, or only described change?

## Commercial Drama Test

Commercial details must alter the conflict.

A number is dramatic only when a character must choose between incompatible outcomes because of it.

For example:

5,400 RMB immediate cash
versus
future loading / renovation / exclusivity obligations

is useful only when another character has a legitimate reason to insist on those terms.

The number itself is not drama.

## Anti-Flowchart Test

If the chapter can be summarized as:

event → protagonist calculates → protagonist understands principle → protagonist makes correct decision → protagonist writes lesson

the chapter should normally be REJECTED.

This is an outline wearing prose.

## Chapter-Level Standard

To receive Dramatic PASS, a chapter must demonstrate at least:

- one active conflict;
- one escalation or reversal;
- one consequential choice;
- one cost;
- one state change that creates the next problem.

Dramatic Integrity is independent of prose beauty.

A beautifully written chapter can still REJECT.
A plain but dramatically alive chapter can PASS.

## R1.1 — Binding Acceptance Rules

This section defines the acceptance threshold used by all chapter audits.
Policy ID: DRAMATIC_INTEGRITY_R1.1_CANDIDATE.
It is a proposed policy until explicitly adopted; tests against it do not inherit earlier QA_PASS.

### Coverage

Before judging quality, enumerate every prose scene with Scene ID and paragraph/line range.
Classify each as conflict/decision, aftermath, or bridge/rest.
A scene controlling the chapter's central choice, consequence, or ending is material and cannot be excluded.
For bridge/rest scenes, record the setup, consequence, contrast, or recovery they serve and the scene they connect to.
Non-applicability requires evidence and a reason; it cannot exempt the chapter as a whole.
A superficial bridge cannot reset the repeated-flowchart check.

### Seven Required Checks

For each material scene record evidence, observed mechanism, and PASS / FAIL / INCOMPLETE / N/A:

| ID | Check | Required prose evidence | Insufficient substitute |
|---|---|---|---|
| DI-01 | Objective and opposition | Who wants what now; incompatible pursuit or a concrete constraint changes available action. Internal or environmental resistance is allowed when it operates on the choice. | A named opponent, a rhetorical question, or an obstacle mentioned but never operative. |
| DI-02 | Tactics | An attempt to change the other party or situation, its response, and persistence or adjustment justified by that response. | Calling calculation or explanation a strategy without an enacted attempt. |
| DI-03 | Turn | The before/after advantage, expectation, or available options; the action or discovery causing that change. Escalation qualifies only when it materially changes pressure or options. | An unrelated interruption or information that changes no pursuit or choice. |
| DI-04 | Subtext and interaction | What an important utterance/action says on the surface, what it tries to achieve, and how the other party responds. Where a hidden motive is claimed, show its behavioral trace. | Silence, ellipses, evasive wording, or the auditor supplying an unstated motive. |
| DI-05 | Agency | A consequential choice and a credible alternative; explain which result would differ if the choice changed. Material supporting characters act from their own goals or constraints. | A token choice after an external event has already fixed the outcome. |
| DI-06 | Meaningful cost | A loss, binding commitment, surrendered option, or constrained relationship caused by the choice; record who bears it and when it takes effect. | Stakes, possible future harm, reluctance, or a narrator's claim of responsibility alone. |
| DI-07 | Next problem | A problem newly created or materially intensified by the choice/state change, and the concrete response or test it demands downstream. | A general question about life, an unchanged old mystery, or a routine next task unrelated to this choice. |

Direct speech can pass DI-04; everyone need not lie or conceal a motive.
A turn need not be a surprise twist; a refusal or newly binding term can change the available action.
Costs may be deferred, relational, or opportunity costs, but the obligation or option loss must already be established.
A reflective question can pass DI-07 when the new state commits the character to a concrete future test.
Character growth is not required in every chapter; behavior must prove any growth that the audit claims.
External triggers, including the premise event, are allowed; they cannot substitute for all consequential agency.

### Evidence and Verdict

Every check requires a prose range and observed fact. Handoff statements and writer self-report cannot substitute.
For absence claims, cite the complete relevant scene range and state which mechanism was searched for and not found.
Do not fabricate evidence to justify a strong verdict.

INCOMPLETE means evidence, input, or coverage is missing. Keep the chapter unclosed in DRAFT / QA_REVISE, as applicable.
FAIL means the available prose demonstrates a blocking dramatic defect.
A material-scene FAIL requires at least REVISE; a failure dominating the chapter or destroying its central function requires REJECT.
Do not average the checks or compensate for a FAIL with prose beauty or logical PASS.
N/A is allowed only for a justified scene-level exemption; all seven checks must be resolved at chapter level.
CONDITIONAL PASS may describe a non-blocking note; it cannot count as Dramatic PASS while a required check is FAIL or INCOMPLETE.
Known defects retained by the author use QA_OVERRIDE.

### Counterfactuals and Revision

For each central choice test deletion, reversal of choice, removal of resistance, and a more reasonable opposing tactic.
Record the materially different outcome, or the missing dependency that makes the scene fail.
After revision, re-extract affected scene evidence and scan the whole chapter for displaced defects.
Added explanatory sentences do not close a defect unless enacted pursuit, choice, or consequence changed.
