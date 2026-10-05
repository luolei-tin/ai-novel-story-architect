# ChatGPT Project 安装说明

## 目标

本仓库是 ChatGPT 的长期故事架构与红队方法库。

推荐采用双模型工作流：

ChatGPT = Story Architect / Chief Editor / Red Team
Gemini = Prose Writer / Scene Executor

ChatGPT 解决“为什么成立”。

Gemini 解决“怎样写出来”。

## Project Instructions

将根目录 PROJECT_INSTRUCTIONS.md 作为 Project Instructions 核心。

Instructions 负责：
- 角色；
- 权限边界；
- 工作顺序；
- 对抗性原则；
- 模型分工。

参考文件负责：
- 故事核心方法；
- 人物模型；
- 结构；
- 伏笔；
- Handoff；
- Red Team；
- Validation。

## 建议文件

### 第一层：ChatGPT 必读
- PROJECT_INSTRUCTIONS.md
- 00_CORE/WORKFLOW.md
- 00_CORE/MODEL_ROLE_PROTOCOL.md

### 第二层：故事设计
- 01_STORY_ARCHITECT/STORY_CORE.md
- 02_CHARACTER/CHARACTER_PSYCHOLOGY.md
- 02_CHARACTER/CHARACTER_ARC.md
- 02_CHARACTER/RELATIONSHIP_DYNAMICS.md
- 03_STRUCTURE/STORY_STRUCTURE.md
- 03_STRUCTURE/CAUSALITY_AND_TURNING_POINTS.md
- 03_STRUCTURE/FORESHADOWING.md

### 第三层：Gemini 交接
- 04_WRITER_HANDOFF/CHAPTER_SPEC.md
- 04_WRITER_HANDOFF/GEMINI_WRITER_PROTOCOL.md

### 第四层：ChatGPT 红队
- 05_RED_TEAM/CHAPTER_AUDITOR.md
- 05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md
- 05_RED_TEAM/CONTINUITY_AUDITOR.md
- 05_RED_TEAM/LOGIC_AUDITOR.md
- 05_RED_TEAM/REJECTION_STANDARD.md

### 第五层：运行与验证
- 06_OPERATIONS/OPERATIONS.md
- 06_OPERATIONS/COMMAND_ROUTER.md
- 06_OPERATIONS/MULTI_MODEL_WORKFLOW.md
- 07_VALIDATION/VALIDATION_PROTOCOL.md
- 07_VALIDATION/MODEL_HANDOFF_VALIDATION.md
- 07_VALIDATION/AUDIT_RECORD.md

## 正式生产方式

### 阶段 A：ChatGPT 设计

用户给出：
- 模糊创意；
- 人物想法；
- 主题；
- 世界；
- 一个结局；
- 或任何局部设想。

ChatGPT 不急着写正文，而是进行：
反事实挑战 → 人物心理 → 世界约束 → 因果结构 → 大纲 → Dramatic Contract。

### 阶段 B：Gemini 写作

ChatGPT 把 CHAPTER_READY 工件交给 Gemini。

Gemini：
- 写正文；
- 保持结构约束；
- 返回 Writer Deviation Report。

### 阶段 C：ChatGPT 红队

ChatGPT 独立审查：
Causality → Character → Information → Structure → Continuity → Foreshadowing → Dramatic Integrity → Prose。

### 阶段 D：返修

REVISE / REJECT：
ChatGPT 输出最小修复单。

Gemini 修改。

### 阶段 E：二审

ChatGPT 检查：
- 原缺陷是否真正关闭；
- 是否产生新缺陷；
- 是否发生未经授权的结构变化；
- 状态是否正确。

只有 QA_PASS 才结束章节。

## 重要纪律

ChatGPT 不应为了“让章节更顺”而提前替 Gemini 写正文。

ChatGPT 的价值主要来自：
- 对抗性思考；
- 心理推演；
- 因果推演；
- 反事实；
- 红队审查。

Gemini 的价值主要来自：
- 场景化；
- 叙事声音；
- 对话；
- 细节；
- 节奏；
- 长篇正文执行。

## 长篇生产

每章都执行：

START STATE
→ Handoff
→ Gemini Draft
→ Deviation Check
→ Red Team
→ Revision
→ Second Audit
→ END STATE

禁止：
- 旧 PASS 跨版本复用；
- 静默改架构；
- 用解释性旁白修因果；
- 用一句主题台词替代人物行为；
- 用“感觉像人”替代心理因果。

## 当前建议

每一本小说使用独立 ChatGPT Project。

Gemini 不需要保存整套架构理论；Gemini 主要接收：
- 当前世界/人物必要上下文；
- Chapter Dramatic Contract；
- State；
- Forbidden Moves；
- Revision Brief。

这样可以减少 Gemini 被大量架构文本干扰，同时保留 ChatGPT 对结构的控制。