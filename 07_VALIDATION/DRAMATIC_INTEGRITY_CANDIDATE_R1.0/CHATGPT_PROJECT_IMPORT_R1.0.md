# ChatGPT ��Ŀ����ͬ���� �� Dramatic Integrity R1.0

> �������ڣ�2026-10-08��Asia/Shanghai��
> ״̬��CANDIDATE / REVIEW_REQUIRED / BLIND_TESTS_NOT_EXECUTED
> ��;��ͬ����ѡ�����򣬲��޸� Story Bible��Canon ��С˵����״̬��

## ��׷�ӵ����� Project Instructions �ĺ�ѡ����˵��

����Ŀ���� Dramatic Integrity ��ѡ��ǿ�������ʱ����ȷʹ����һ�����
����ʽ�������ܿ�����ǰ���������ֺ�ѡ״̬��������������Զ���Ϊ���� QA_PASS��
����Ϸ�����ձ��븲��ȫ���������Լ�Ŀ�������������ԡ�ת��Ǳ̨���뻥�����ܶ��ԡ���ʵ���ۡ���һ�����������������֤�ݡ�
�߼� PASS���ıʺá�Writer Skill �Լ�� Handoff �Ϲ治��������� Dramatic PASS��
ȱ�������֤�ݼǼ��״̬ INCOMPLETE �������½�δ�رգ�������֤�ݵ������ʧ�ܽ��� REVISE/REJECT��
���߱�����֪����ʹ�� QA_OVERRIDE������αװ�� QA_PASS��

ä�����ڲ����뱾��Ŀ֪ʶ��Ķ����������н��У�ֻ�ṩ���ĺ�������
�ȶ��� Pass A�����ṩ Handoff��ƫ�뱨������������� Pass B�����ð������ͼ����������ʵ��
ä��ʱ��Ҫ������������ṩ AUTHOR_EXPECTED_R1.0.md���������ۻ򱾰����˵����
����������ֱ�׶԰׺��ӳٶ��ֵİ���������ܺϸ񣬲�����û��������û�������û�������Ʋƻ�е���ա�

�������ķݺ�ѡ����Э��ȫ�ġ������ܹ���������������������������
��������������ʵ����������ͻ����¼��ͻ��汾����ѡ���������Զ���д���� Canon��


---

## ��Դ��05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md

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

event �� protagonist calculates �� protagonist understands principle �� protagonist makes correct decision �� protagonist writes lesson

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

## R1.1 �� Binding Acceptance Rules

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


---

## ��Դ��07_VALIDATION/AUDIT_RECORD.md

# Audit Record

���ļ�������С����¼��ʽ��

## Required Fields

### Audit ID
Ψһ����š�

### Artifact
�����Ĺ��¹�����

### Artifact Version
�����汾��

### Upstream Baseline
����������������ΰ汾��

### Scope
��ȷ���μ�鸲��ʲô��������ʲô��

### Evidence
�����¼��

- Evidence ID
- Location
- Observed Fact
- Applicable Rule
- Analysis

### Findings

ÿ�������¼��

- Severity: FATAL / HIGH / MEDIUM / LOW
- Location
- Broken Rule
- Broken Chain
- Why It Fails
- Minimum Repair

### Verdict

ֻ���ǣ�

- PASS
- CONDITIONAL PASS
- REVISE
- REJECT
- QA_OVERRIDE

## Verdict Boundary

PASS��

��鷶Χ��û����ֹ�����ƽ������⡣

CONDITIONAL PASS��

������ȷ�ͷ���ȱ�ڣ������ƻ���ǰ���ߡ�

REVISE��

����ʵ�����⣬�����޸ĺ�����

REJECT��

��������������Ϣ�������Ի�ṹ�Ѿ��޷��ڵ�ǰ�汾�³�����

QA_OVERRIDE��

������ȷ������֪���⣻�ⲻ�� PASS��

## No Evidence, No Strong Verdict

���������޷�ָ����ʵ���������������

���ø��� FATAL/HIGH/REJECT��

ͬ����Ҳ������Ϊȱ��֤�ݾ����� PASS��

## Chapter Closure Record �� Required

Chapter-level records must use ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md.
Record:
- Prose artifact ID, version, and content hash or immutable commit.
- Audit policy ID/version.
- Pass A inputs and contamination disclosure.
- Complete scene inventory: ranges, type, materiality, and exemption reasons.
- DI-01 through DI-07 evidence, observed mechanism, check status, and findings.
- Central-choice counterfactual outcomes.
- Frozen Pass A record and separately recorded baseline comparison.
- Logical Verdict and Dramatic Verdict.
- Required continuity/foreshadow/deviation checks and current status.
- Open findings, repairs, and revalidation scope.
- Closure Decision: QA_PASS / NOT_CLOSED / QA_OVERRIDE.

An uncompleted check uses Check Status: INCOMPLETE, not a fabricated strong Verdict.
A required INCOMPLETE or material FAIL blocks QA_PASS.
PASS / CONDITIONAL PASS on a limited scope is never the chapter's closure decision.
Policy changes affecting acceptance require revalidation of dependent active artifacts.


---

## ��Դ��07_VALIDATION/VALIDATION_PROTOCOL.md

# Validation Protocol

���ļ��ѡ�������������Ϊ����֤�Ĺ���״̬����������ͨ���顣

## 1. Validation Principle

�κι��¹������У�

- State����ǰ״̬
- Version���汾
- Upstream Dependencies�����������ι���
- Evidence��֧�ֵ�ǰ���۵�֤��
- Verdict����֤���

���Ѿ�д�����������ڡ��Ѿ���֤����

## 2. Lock Rule

����״ֻ̬���ڶ�Ӧ���ι����ȶ��������������

SEED �� CORE_DRAFT �� CORE_LOCKED �� CHARACTER_LOCKED �� WORLD_LOCKED �� OUTLINE_LOCKED �� CHAPTER_READY �� DRAFT �� QA_REVISE �� QA_PASS

�κ���������������ʵ���޸ģ�

1. ԭ����״̬����ʧЧ��
2. ����ֱ�������������ι������ STALE��
3. ���ü���ʹ�þɵ� QA_PASS��
4. ����������֤��Ӱ�췶Χ��

## 3. Dependency Invalidation

�޸ģ�

- Story Core �� �������¼�� Character / World / Outline / Turning Points / Chapter Handoff��
- Character Psychology �� �������¼����� Turning Points / Outline / Chapter Handoff��
- World Rule �� �������¼����Ӱ�� Causality / Outline / Foreshadowing / Chapters��
- Outline / Turning Point �� �������¼����Ӱ�� Chapter Handoff / Foreshadowing��
- Chapter prose �� ��������ִ�� Chapter Audit + ���� Dramatic Audit + Continuity Audit��������޸��Ƿ��ȱ��ת�Ƶ�����������
- ���չ���汾�ı� �� ����鲻��ֱ��֤���¹����µ� QA_PASS��Ϊ��Ӱ��Ļ������¼��������֤��Χ��

������Ϊ���Ķ���������С�������������жϡ�

## 4. Evidence Rule

ÿ���ش� Verdict �����ܻش�

- �����ʲô��
- �����ĸ��汾��
- ������ʲô��ʵ��
- �������������Υ����
- ������ʲô��

��ֹֻ������о�������������û���⡱�������޸ġ���

## 5. Regression Rule

REVISE / REJECT ��

DRAFT �� QA_REVISE �� �޸� �� ��Ӱ��������� �� ������ FATAL/HIGH������ REVISE/REJECT �� ȫ����Ҫ���ͨ�� �� QA_PASS

���ô� REJECT ֱ������ PASS��

## 6. Scope of Revalidation

���������޸Ķ�Ҫ������С˵����

����˱�����ȷ��

- Changed Artifact
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected

����޷�֤��ĳ�����Ӱ�족��Ĭ�ϱ��Ϊ��Ҫ��顣

## 7. Validation Record

����ÿ����鱣�棺

- Audit ID
- Date
- Artifact Version
- Upstream Versions
- Checks Performed
- Findings
- Verdict
- Required Repairs
- Revalidation Scope

## 8. PASS Meaning

PASS ���ǡ�Ŀǰû�з������⡱��

PASS �ĺ����ǣ�

> �������ļ�鷶Χ�������汾�Ϳ���֤���£�û�з���������ֹ�����ƽ������⡣

���ð����޷�Χ�� PASS �������Ϊ���������¾��Գ�������

## 9. Chapter Closure Gate

Ϸ�������� ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md ΪΨһ�ж����ߡ�
ʹ�� AUDIT_RECORD.md �� Chapter Closure Record��

ֻ����������ͬʱ�������ſɽ��� QA_PASS��
1. ��ǰ���İ汾�� Logical Verdict = PASS��
2. ��ǰ���İ汾�� Dramatic Verdict = PASS���������������������Ǿ���֤�ݡ�
3. ��Ҫ�������ԡ����ʡ�ƫ���������ɣ��ṹƫ���ѻ���ȷ������
4. û����ֹ�ƽ���δ�ر����⣬û�б����鴦�� FAIL / INCOMPLETE��
5. ���ġ����λ��ߺ����չ���汾���¼ƥ�䣬��¼δ STALE��

CONDITIONAL PASS ����������ż��� PASS��
ȱ�����ȱ֤��ʱ����δ�رգ�����ƾ�˱��� REJECT ������ PASS��
���߱�����֪ȱ����ʹ�� QA_OVERRIDE�������� QA_PASS��
��ʷ������������¹��������Զ�ת����


---

## ��Դ��07_VALIDATION/BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md

# Blind Dramatic Audit Protocol �� R1.0

## Purpose

��ֹ ChatGPT ��Ϊ�Լ�������ƣ��������ʱ����ʶ�����Լ��ķ�����

## Pass A �� Prose-First Audit

Pass A ʹ�ö�����������ģ�ֻ���մ������ĺ�������
���ṩ Handoff�����˵�������߽��͡�Writer Deviation Report���������ۻ����Ԥ�ڴ𰸡�
���ý�ƾ����ʱ��Ϊ��Ʊ绤������ä�����޷����룬��¼ INPUT_CONTAMINATED���ü�¼������ä������֤�ݣ��½ڱ���δ�رգ��ȴ�����������顣

�Ȱ� ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md �г����������嵥�����ķ�Χ��
ֻ�������ļ�¼��
- ���ﵱǰĿ�ꣻ
- ����Ŀ�ꣻ
- ��Ϣ�
- ���룻
- ս�����Է���Ӧ��
- Ǳ̨�ʻ�����/�ж���ʵ�ʻ���Ŀ�ģ�
- ��ת��
- �ؼ�ѡ��
- ѡ����ۣ�
- ��״̬������ɻ���������һ���⡣

Pass A ��ɺ󶳽�汾��֤�����ж���Pass B ����������ֻ���Ǹ��������ɡ�

Ȼ��ش�

> �����֪������ԭ�������ʲô����һ�±����Ƿ���Ȼ������

## Pass B �� Contract Audit

���������� Handoff ���գ�
- required objective;
- required causal chain;
- state delta;
- forbidden moves;
- foreshadowing;
- character limits.

## Pass C �� Counterfactual Audit

���ÿ�������½�����Ĺؼ�ѡ�񣬱��淴��ʵ�������Խ����Ӱ�죻������������䣬�� Dramatic ���չ����ж�ȱ�ݣ�
- ɾ������ѡ����Ƿ���Ȼ������
- ɾ�������������Ƿ���Ȼ������
- ���ֲ�ȡ���������Ժ������Ƿ������ƽ���
- ����ѡ���෴�����ᷢ��ʲô��

## Automatic Dramatic Warning

������һģʽ���������������ϳ��������� REVISE��

�¼� �� ���ǽ��� �� ���Ƕ��� �� ��ȷѡ��

��ɫ���� �� �ṩ��Ϣ �� �������� �� ��ɫ�뿪

��ͻ���� �� ��ҵ���� �� ���Ǽ��� �� ��ͻ���

## Anti-Self-Protection Rule

��������� ChatGPT ԭ��Ƴ�ͻ��
���ж������Ƿ��������

������Ϊ������ Handoff Ҫ�󡱾��Զ���������ȷ��

��� Handoff ������ɲ���ȻϷ�磬Ӧ��� ARCHITECTURE_DEFECT��

## Verdict

Blind audit ���������
- PASS
- CONDITIONAL PASS
- REVISE
- REJECT

���ɱ�����������֤�ݡ�

ȱ����/֤��ʱ�ü��״̬ INCOMPLETE�������½�δ�رա�
���� Dramatic Verdict ��������Ψһ���ձ��������� CONDITIONAL PASS �ƹ�ʧ�ܻ�δ����
����Ԥ���ж�ֻ�ɱȽϲ����ȡ�������� Pass A/B/C ��������롣

