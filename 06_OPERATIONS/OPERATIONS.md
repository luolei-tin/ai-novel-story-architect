# 操作协议

本目录定义“什么时候调用哪一种能力”，而不是新增故事理论。

## 1. /init-story
用途：从一个模糊创意建立项目起点。
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
完成后必须执行主题反事实：
- 换成圆满结局是否仍成立？
- 换成悲剧结局是否仍成立？
- 主角拒绝最终选择后故事是否仍成立？
- 如果成立，当前主题是否只是表面包装？
若无法回答，状态不得标记为 CORE_LOCKED。

## 3. /build-character
用途：建立主要人物。
每个核心人物至少建立：
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
关键要求：人物选择必须能追溯到“过去经历 → 信念 → 欲望/恐惧 → 当前压力 → 选择”。

## 4. /build-world
用途：建立会真正影响剧情的世界规则。
每条规则必须回答：
1. 谁受约束？
2. 提供什么机会？
3. 代价是什么？
4. 如何制造冲突？
5. 删除规则后主线是否仍成立？
只用于制造气氛、百科知识或作者炫技的设定，不进入核心规则集。

## 5. /build-outline
用途：建立总纲、分卷和章节轨迹。
必须同时追踪：
- Quest：外部行动
- Fire：内部变化
- Constellation：关系变化
每个高价值节点必须检查：
事件 → 认知 → 选择 → 行动 → 反馈 → 新状态
不得只列“发生了什么”，必须记录“谁做了什么选择，以及为什么”。

## 6. /design-turning-point
用途：设计关键转折。
必须回答：
- 谁做选择？
- 为什么现在做？
- 他知道什么？
- 他不知道什么？
- 如果不做这个选择会怎样？
- 为什么其他选择没有发生？
- 选择造成什么不可逆后果？
- 后续选项因此如何改变？
若转折主要依赖作者突然安排的事件，而不是人物选择，应判定为结构风险。

## 7. /plant-foreshadow
用途：设计伏笔。
必须记录：
- ID
- Plant Chapter
- Plant Information
- Surface Interpretation
- True Meaning
- Trigger Condition
- Payoff Chapter
- Payoff Event
- Reader Visibility
- False Lead
- Status
禁止在回收时凭空补充过去不存在的信息，并把它称为伏笔。

## 8. /chapter-handoff
用途：把经过验证的章节任务交给正文模型。
交接包必须包含：
- Chapter Objective
- Starting State
- Required Causal Events
- Character Intent
- Information Control
- Forbidden Moves
- Ending State
- Foreshadow/Payoff Requirements
正文模型拥有表达自由，但没有擅自重写主线、人物核心动机、世界规则和伏笔时间点的权限。

## 9. /audit-chapter
用途：审查正文初稿。
固定顺序：
1. Causality
2. Character
3. Information
4. Structure
5. Continuity
6. Foreshadowing
7. Prose
输出只能是：
- PASS
- CONDITIONAL PASS
- REVISE
- REJECT
REJECT 必须指出：
- 断裂发生在哪里
- 哪条因果链断裂
- 为什么现有文本无法证明成立
- 最小修复方案
不能用“润色建议”掩盖结构性失败。

## 10. /audit-continuity
用途：检查跨章节连续性。
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
如果后章使用了前章尚未获得的信息，属于信息连续性错误。

## 11. /red-team-story
用途：对整个故事做高压压力测试。
强制提出：
- 为什么结局必须是这个结局？
- 如果换成圆满结局，主题还成立吗？
- 如果删除一个主要人物，主线还成立吗？
- 如果删除一条核心世界规则，主线还成立吗？
- 如果主角不做关键选择，故事还成立吗？
- 如果反派突然改变，故事是否失去支撑？
- 哪个转折最像作者强推？
- 哪个伏笔最像事后补丁？
输出：
- FATAL
- HIGH
- MEDIUM
- LOW
其中 FATAL/HIGH 必须优先处理。

## 12. /revise-after-rejection
用途：根据 REJECT/REVISE 结果生成修改任务。
原则：
- 优先修因果，再修人物，再修结构，再修连续性，最后修语言。
- 不允许通过增加解释性对白掩盖因果漏洞。
- 不允许用新设定无成本修补旧漏洞。
- 不允许为了保住原文而牺牲故事核心。
输出必须明确：
- 必须修改
- 可以保留
- 禁止新增
- 修改后的验证标准

## 13. /validate-regression
用途：REVISE / REJECT 或任何上游锁定工件修改后的回归验证。

必须记录：
- Changed Artifact
- Artifact Version
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected
- Checks Performed
- New Findings
- New Verdict

规则：
- 不得从 REJECT 直接跳到 PASS。
- 上游实质修改会使相关下游状态 STALE。
- 无法证明“不受影响”的项目默认进入重新验证范围。
- PASS 只对声明的范围和版本有效。

## 14. /record-override
用途：作者明确选择保留红队指出的问题。

必须记录：
- Overridden Finding
- Author Decision
- Reason
- Accepted Risk
- Affected Scope

状态使用 QA_OVERRIDE，不得伪装成 QA_PASS。
如果 Override 改变核心因果、人物心理、世界规则或结构，必须重新执行受影响验证。

# 状态控制

建议项目使用以下状态：

SEED → CORE_DRAFT → CORE_LOCKED → CHARACTER_LOCKED → WORLD_LOCKED → OUTLINE_LOCKED → CHAPTER_READY → DRAFT → QA_REVISE → QA_PASS

附加状态：
- STALE：上游实质修改导致当前工件需要重新验证。
- QA_OVERRIDE：作者明确保留已知问题，不等于 PASS。

任何阶段都可以退回，但不能把“已经写出来”当成“已经验证”。

# 总原则

故事架构负责证明故事成立；正文模型负责把成立的故事写出来；红队负责证明正文没有把它写坏；回归验证负责证明修改没有把已经成立的部分再次破坏。
