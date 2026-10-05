# 操作协议

本目录定义“什么时候调用哪一种能力”，而不是新增故事理论。

## 1. /init-story
用途：从模糊创意建立项目起点。
必须完成：
- 提取用户明确事实
- 区分事实、假设、待决定项
- 提出最少关键问题
- 不提前替用户决定核心主题
输出：STORY_SEED、OPEN_DECISIONS、INITIAL_RISKS

## 2. /build-story-core
用途：建立故事内核。
必须形成：
- STORY_THESIS
- CENTRAL_QUESTION
- CHARACTER_TRUTH
- FINAL_CHOICE
- FINAL_CONSEQUENCE
完成后执行主题反事实。
若无法回答，状态不得标记为 CORE_LOCKED。

## 3. /build-character
用途：建立主要人物。
至少建立：
- Want
- Need
- Lie
- Wound/Ghost
- Motivation Origin
- Internal Contradiction
- Defense Mechanism
- Vulnerability Trigger
- Pressure
- Stakes
关键要求：人物选择必须能追溯到过去经历 → 信念 → 欲望/恐惧 → 当前压力 → 选择。

## 4. /build-world
用途：建立真正限制选择的世界规则。
每条规则必须回答：
1. 谁受约束？
2. 提供什么机会？
3. 代价是什么？
4. 如何制造冲突？
5. 删除后主线是否仍成立？

## 5. /build-outline
用途：建立总纲、分卷和章节轨迹。
必须同时追踪：
- Quest
- Fire
- Constellation
每个高价值节点必须记录谁选择、为什么、代价与新状态。

## 6. /design-turning-point
用途：设计关键转折。
必须回答：
- 谁做选择？
- 为什么现在？
- 知道什么？
- 不知道什么？
- 不做会怎样？
- 为什么其他选择没有发生？
- 不可逆后果是什么？
- 后续选项如何改变？

## 7. /plant-foreshadow
用途：设计伏笔。
必须记录：
ID / Plant / Surface Interpretation / True Meaning / Trigger / Payoff / Reader Visibility / False Lead / Status
禁止回收时凭空创造过去不存在的信息。

## 8. /chapter-handoff
用途：生成 Gemini 正文交接包。
注意：Handoff 不是“本章事件列表”，而是 Dramatic Contract。
必须包含：
- Chapter Objective
- Starting State
- Dramatic Situation
- Causal Spine
- Character Pressure
- Information Control
- Relationship Movement
- Foreshadowing
- Forbidden Moves
- Ending State

只有通过 Chapter Ready Gate 后才能交给 Gemini。

## 9. /audit-chapter
用途：审查 Gemini 正文。
固定顺序：
1. Causality
2. Character
3. Information
4. Structure
5. Continuity
6. Foreshadowing
7. Dramatic Integrity
8. Prose
输出：
PASS / CONDITIONAL PASS / REVISE / REJECT

其中 Dramatic Integrity 独立检查：
- 场景目标与对立目标
- 筹码与信息差
- 战术与反转
- 选择与代价
- 配角自主性
- 是否出现“事件 → 解释 → 主角顿悟 → 正确选择”的流程图式写法

逻辑正确但戏剧失败，仍可 REJECT。

## 10. /audit-continuity
用途：检查跨章节状态。
至少核对：
- 时间
- 地点
- 身体状态
- 持有物
- 已知信息
- 秘密
- 人物关系
- 信念
- 承诺/债务
- 世界规则
- 未解决线索
- 伏笔状态

## 11. /red-team-story
用途：故事级高压测试。
强制挑战：
- 为什么结局必须是这个结局？
- 圆满结局是否仍成立？
- 悲剧结局是否仍成立？
- 主角拒绝关键选择后是否仍成立？
- 删除人物后哪条因果链断？
- 删除世界规则后哪个选择消失？
- 反派保持理性时主线是否成立？
- 哪个转折最像作者强推？

## 12. /revise-after-rejection
用途：生成给 Gemini 的最小修改任务。
必须明确：
- Verdict
- Broken Chain
- Why It Fails
- Minimum Repair
- Do Not Patch By
- State Constraints
- Elements That Must Not Change

ChatGPT 默认负责诊断和修改指令，不代替 Gemini 大规模重写正文。

## 13. /validate-regression
用途：REVISE / REJECT 或上游修改后的回归验证。
必须记录：
- Changed Artifact
- Version
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected
- Checks
- New Findings
- Verdict

## 14. /record-override
用途：作者坚持保留已知问题。
记录：
- Overridden Finding
- Author Decision
- Reason
- Accepted Risk
- Affected Scope
状态使用 QA_OVERRIDE。

## 15. /handoff-to-gemini
用途：将 CHAPTER_READY 工件转换成 Gemini 可直接执行的 Dramatic Contract。
输出必须引用：
- 上游版本
- 权威起始状态
- 当前冲突
- 信息边界
- 允许表达自由
- 结构禁区
- 终止状态
- Writer Deviation Report 要求

禁止在此步骤偷偷补设计。

## 16. /intake-gemini-draft
用途：接收 Gemini 正文。
先做“合同一致性检查”，再做内容红队。
必须区分：
- 是否遵守 Handoff
- 是否写得成立
- 是否写得有戏

## 17. /gemini-revision-brief
用途：把 ChatGPT 的 REVISE / REJECT 转成 Gemini 可以执行的返修单。
目标是“修因果/人物/戏剧结构”，不是把整个章节重新发明。

## 18. /chapter-close
用途：只有 QA_PASS 后才能执行。
完成：
- END STATE 写入权威状态
- 记录审查证据
- 标记本章版本
- 开放下一章 CHAPTER_READY

# 模型分工

ChatGPT：
设计 → 质询 → 验证 → Handoff → Red Team → Revision Brief → Regression

Gemini：
Handoff → Prose Draft → Deviation Report → Revision

作者：
最终创作权 / Override 权

## 状态原则

SEED → CORE_DRAFT → CORE_LOCKED → CHARACTER_LOCKED → WORLD_LOCKED → OUTLINE_LOCKED → CHAPTER_READY → DRAFT → QA_REVISE → QA_PASS

附加：
STALE
QA_OVERRIDE

任何阶段都不能用“已经写出来”代替“已经验证”。