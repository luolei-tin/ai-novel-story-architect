# ChatGPT 项目资料同步包 — Dramatic Integrity R1.0

> 更新日期：2026-10-08（Asia/Shanghai）
> 状态：CANDIDATE / REVIEW_REQUIRED / BLIND_TESTS_NOT_EXECUTED
> 用途：同步候选审查规则，不修改 Story Bible、Canon 或小说生产状态。

## 可追加到现有 Project Instructions 的候选资料说明

本项目新增 Dramatic Integrity 候选补强包。审稿时须明确使用哪一版规则。
在正式采用与受控验收前，本包保持候选状态；试验审查结果不自动成为生产 QA_PASS。
完整戏剧验收必须覆盖全部场景，以及目标与阻力、策略、转向、潜台词与互动、能动性、真实代价、下一问题七项，并引用正文证据。
逻辑 PASS、文笔好、Writer Skill 自检或 Handoff 合规不能替代独立 Dramatic PASS。
缺少输入或证据记检查状态 INCOMPLETE 并保持章节未关闭；有正文证据的阻断性失败进入 REVISE/REJECT。
作者保留已知问题使用 QA_OVERRIDE，不能伪装成 QA_PASS。

盲审须在不载入本项目知识库的独立上下文中进行，只提供正文和审查规则。
先冻结 Pass A，再提供 Handoff、偏离报告和上游资料做 Pass B；不得把设计意图补成正文事实。
盲测时不要向审稿上下文提供 AUTHOR_EXPECTED_R1.0.md、旧审稿结论或本包设计说明。
安静场景、直白对白和延迟兑现的绑定义务均可能合格，不能以没有争吵、没有谜语或没有立即破财机械拒收。

以下是四份候选核心协议全文。其他架构、人物、世界与表达规则继续保留。
若本包与现有事实或创作决定冲突，记录冲突与版本；候选审查条款不得自动改写故事 Canon。


---

## 来源：05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md

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


---

## 来源：07_VALIDATION/AUDIT_RECORD.md

# Audit Record

本文件定义最小审查记录格式。

## Required Fields

### Audit ID
唯一审查编号。

### Artifact
被审查的故事工件。

### Artifact Version
被审查版本。

### Upstream Baseline
本次审查依赖的上游版本。

### Scope
明确本次检查覆盖什么，不覆盖什么。

### Evidence
逐项记录：

- Evidence ID
- Location
- Observed Fact
- Applicable Rule
- Analysis

### Findings

每项问题记录：

- Severity: FATAL / HIGH / MEDIUM / LOW
- Location
- Broken Rule
- Broken Chain
- Why It Fails
- Minimum Repair

### Verdict

只能是：

- PASS
- CONDITIONAL PASS
- REVISE
- REJECT
- QA_OVERRIDE

## Verdict Boundary

PASS：

检查范围内没有阻止继续推进的问题。

CONDITIONAL PASS：

存在明确低风险缺口，但不破坏当前主线。

REVISE：

存在实质问题，必须修改后重审。

REJECT：

核心因果、人物、信息、连续性或结构已经无法在当前版本下成立。

QA_OVERRIDE：

作者明确保留已知问题；这不是 PASS。

## No Evidence, No Strong Verdict

如果审查人无法指出事实、规则和推理链：

不得给出 FATAL/HIGH/REJECT。

同样，也不得因为缺乏证据就宣布 PASS。

## Chapter Closure Record — Required

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

## 来源：07_VALIDATION/VALIDATION_PROTOCOL.md

# Validation Protocol

本文件把“审稿意见”升级为可验证的工程状态，而不是普通建议。

## 1. Validation Principle

任何故事工件都有：

- State：当前状态
- Version：版本
- Upstream Dependencies：依赖的上游工件
- Evidence：支持当前结论的证据
- Verdict：验证结果

“已经写出来”不等于“已经验证”。

## 2. Lock Rule

以下状态只有在对应上游工件稳定后才允许成立：

SEED → CORE_DRAFT → CORE_LOCKED → CHARACTER_LOCKED → WORLD_LOCKED → OUTLINE_LOCKED → CHAPTER_READY → DRAFT → QA_REVISE → QA_PASS

任何已锁定工件发生实质修改：

1. 原锁定状态立即失效；
2. 所有直接依赖它的下游工件标记 STALE；
3. 不得继续使用旧的 QA_PASS；
4. 必须重新验证受影响范围。

## 3. Dependency Invalidation

修改：

- Story Core → 至少重新检查 Character / World / Outline / Turning Points / Chapter Handoff。
- Character Psychology → 至少重新检查相关 Turning Points / Outline / Chapter Handoff。
- World Rule → 至少重新检查受影响 Causality / Outline / Foreshadowing / Chapters。
- Outline / Turning Point → 至少重新检查受影响 Chapter Handoff / Foreshadowing。
- Chapter prose → 至少重新执行 Chapter Audit + 独立 Dramatic Audit + Continuity Audit，并检查修复是否把缺陷转移到其他场景。
- 验收规则版本改变 → 旧审查不得直接证明新规则下的 QA_PASS；为受影响的活动工件记录规则重验证范围。

不得因为“改动看起来很小”而跳过依赖判断。

## 4. Evidence Rule

每个重大 Verdict 必须能回答：

- 检查了什么？
- 依据哪个版本？
- 发现了什么事实？
- 哪条规则被满足或违反？
- 结论是什么？

禁止只输出“感觉成立”“整体没问题”“建议修改”。

## 5. Regression Rule

REVISE / REJECT 后：

DRAFT → QA_REVISE → 修改 → 受影响审查重跑 → 若仍有 FATAL/HIGH：继续 REVISE/REJECT → 全部必要检查通过 → QA_PASS

不得从 REJECT 直接跳到 PASS。

## 6. Scope of Revalidation

不是所有修改都要求整本小说重审。

审查人必须明确：

- Changed Artifact
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected

如果无法证明某项“不受影响”，默认标记为需要检查。

## 7. Validation Record

建议每次审查保存：

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

PASS 不是“目前没有发现问题”。

PASS 的含义是：

> 在声明的检查范围、工件版本和可用证据下，没有发现足以阻止继续推进的问题。

不得把有限范围的 PASS 扩大解释为“整个故事绝对成立”。

## 9. Chapter Closure Gate

戏剧验收以 ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md 为唯一判定基线。
使用 AUDIT_RECORD.md 的 Chapter Closure Record。

只有以下条件同时成立，才可进入 QA_PASS：
1. 当前正文版本的 Logical Verdict = PASS。
2. 当前正文版本的 Dramatic Verdict = PASS，七项检查与完整场景覆盖均有证据。
3. 必要的连续性、伏笔、偏离审查已完成，结构偏离已获明确处理。
4. 没有阻止推进的未关闭问题，没有必需检查处于 FAIL / INCOMPLETE。
5. 正文、上游基线和验收规则版本与记录匹配，记录未 STALE。

CONDITIONAL PASS 不替代必需门槛的 PASS。
缺输入或缺证据时保持未关闭，不得凭此编造 REJECT 或宣布 PASS。
作者保留已知缺陷仍使用 QA_OVERRIDE，不纳入 QA_PASS。
历史诊断样本不因新规则加入而自动转正。


---

## 来源：07_VALIDATION/BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md

# Blind Dramatic Audit Protocol — R1.0

## Purpose

防止 ChatGPT 因为自己参与设计，而在审稿时无意识保护自己的方案。

## Pass A — Prose-First Audit

Pass A 使用独立审查上下文，只接收待审正文和审查规则。
不提供 Handoff、设计说明、作者解释、Writer Deviation Report、旧审稿结论或测试预期答案。
不得仅凭“暂时不为设计辩护”宣称盲审；若无法隔离，记录 INPUT_CONTAMINATED。该记录不构成盲审验收证据，章节保持未关闭，等待独立正文审查。

先按 ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md 列出完整场景清单与正文范围。
只根据正文记录：
- 人物当前目标；
- 对立目标；
- 信息差；
- 筹码；
- 战术及对方回应；
- 潜台词或言语/行动的实际互动目的；
- 反转；
- 关键选择；
- 选择代价；
- 新状态及它造成或升级的下一问题。

Pass A 完成后冻结版本、证据与判定；Pass B 不覆盖它，只另记更正及理由。

然后回答：

> 如果不知道作者原本想表达什么，这一章本身是否仍然成立？

## Pass B — Contract Audit

再拿正文与 Handoff 对照：
- required objective;
- required causal chain;
- state delta;
- forbidden moves;
- foreshadowing;
- character limits.

## Pass C — Counterfactual Audit

针对每个控制章节走向的关键选择，保存反事实推理及对结果的影响；若结果基本不变，按 Dramatic 验收规则判定缺陷：
- 删除主角选择后是否仍然发生？
- 删除对手阻力后是否仍然成立？
- 对手采取更合理策略后主角是否仍能推进？
- 主角选择相反方案会发生什么？

## Automatic Dramatic Warning

以下任一模式连续出现两个以上场景，至少 REVISE：

事件 → 主角解释 → 主角顿悟 → 正确选择

角色进入 → 提供信息 → 主角理解 → 角色离开

冲突出现 → 商业数字 → 主角计算 → 冲突解决

## Anti-Self-Protection Rule

如果正文与 ChatGPT 原设计冲突：
先判断正文是否更成立。

不能因为“这是 Handoff 要求”就自动判正文正确。

如果 Handoff 本身造成不自然戏剧，应提出 ARCHITECTURE_DEFECT。

## Verdict

Blind audit 可以提出：
- PASS
- CONDITIONAL PASS
- REVISE
- REJECT

理由必须引用正文证据。

缺输入/证据时用检查状态 INCOMPLETE，保持章节未关闭。
最终 Dramatic Verdict 必须遵守唯一验收表，不能用 CONDITIONAL PASS 绕过失败或未完成项。
测试预期判定只由比较步骤读取，不进入 Pass A/B/C 的审稿输入。

