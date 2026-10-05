# AI 小说总编剧系统

一个面向长篇小说创作的 Story Architect / Chief Editor / Red Team 工作系统。

它不是“一个 AI 把整本小说写完”的工作流，而是一套双模型生产系统：

ChatGPT 负责想明白、质询、设计、审查。
Gemini 负责把成立的设计写成正文。

## 核心生产链

用户创意
→ ChatGPT Story Architect
→ Story Core
→ Character Psychology
→ World Constraints
→ Causal Outline
→ Foreshadowing
→ Dramatic Contract
→ Gemini Writer
→ Writer Deviation Report
→ ChatGPT Red Team
→ Revision Brief
→ Gemini Revision
→ ChatGPT Second Audit
→ QA_PASS
→ State Update
→ Next Chapter

## ChatGPT 的核心价值

ChatGPT 不默认承担长篇正文生产。

重点解决：
- 故事为什么成立；
- 结局为什么必须这样；
- 如果换成另一个结局会怎样；
- 人物为什么会做这个选择；
- 如果主角拒绝会发生什么；
- 反派为什么不会做更聪明的事；
- 删除人物后哪条因果链断裂；
- 删除世界规则后哪个选择消失；
- 伏笔是否真正存在于此前文本；
- 正文是否把正确的结构写坏。

## Gemini 的核心价值

Gemini 负责：
- 场景；
- 对话；
- 叙事声音；
- 细节；
- 节奏；
- 情绪体验；
- 长篇正文执行。

Gemini 拥有表达自由，但不拥有结构主权。

## 两个独立质量门槛

故事不能因为“逻辑正确”就自动通过。

每章必须同时满足：

### Logical Integrity
- Causality
- Character
- Information
- Continuity
- Foreshadowing

### Dramatic Integrity
- 当前目标；
- 对立目标；
- 筹码；
- 信息差；
- 战术；
- 反转；
- 关键选择；
- 选择代价；
- 关系/权力变化；
- 下一问题。

“事件 → 解释 → 主角顿悟 → 正确选择”如果反复出现，应直接进入 REVISE / REJECT。

## 红队工作方式

红队分两步：

Pass A — Blind Prose Audit

先只看正文：
它到底发生了什么？
人物到底想要什么？
谁阻止谁？
谁占优势？
哪里真正发生了反转？
谁做出了不可逆选择？

不先为 ChatGPT 自己的 Handoff 辩护。

Pass B — Baseline Comparison

再拿正文对照：
- Story Core
- Character
- World
- Outline
- Dramatic Contract
- Long-Form State

这样避免“设计者自己设计、自己解释、自己放过”。

## 失败处理

REVISE / REJECT
→ Broken Chain
→ Minimum Repair
→ Gemini Revision
→ Targeted Re-Audit
→ Regression
→ PASS

作者可以 Override。
但已知问题只能进入 QA_OVERRIDE，不能伪装成 QA_PASS。

## 目录
- 00_CORE：系统核心与模型分工
- 01_STORY_ARCHITECT：故事内核
- 02_CHARACTER：人物心理与关系
- 03_STRUCTURE：结构、因果、转折、伏笔
- 04_WRITER_HANDOFF：Gemini 正文交接
- 05_RED_TEAM：红队与拒绝标准
- 06_OPERATIONS：生产流程与命令路由
- 07_VALIDATION：状态、审计、回归
- 08_V1_3_PRODUCTION：实际小说生产实验

## 重要原则
- 先证明故事成立，再写正文。
- 人物选择优先于作者强推。
- 世界规则必须真正限制选择。
- 商业数字必须制造互斥选择，而不是充当教材。
- 配角必须有独立目标。
- 逻辑 PASS 不等于戏剧 PASS。
- 上游修改必须触发受影响工件失效与回归验证。
- 不把“写出来”当成“写对了”。

## 当前定位

这是一个 ChatGPT Story Architect + Gemini Writer + ChatGPT Red Team 的双模型长篇小说生产系统。

当前小说实战实验已经暂停在架构重设计状态。上一轮正文被保留为诊断样本，不作为质量基准。下一次生产应从新的 Dramatic Contract 开始，而不是继续扩写旧的流水账版本。