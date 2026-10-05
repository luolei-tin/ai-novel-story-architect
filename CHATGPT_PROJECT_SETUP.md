# ChatGPT Project 安装说明

## 目标

这个仓库不是让 ChatGPT 每次聊天时重新理解一遍规则，而是作为 ChatGPT Project 的长期方法库。

## Project Instructions

将仓库根目录的 PROJECT_INSTRUCTIONS.md 作为 Project Instructions 的核心内容。

不要把所有 Skill 文件完整复制进 Instructions。Instructions 负责：
- 角色
- 权限边界
- 工作顺序
- 核心原则

Skill/参考文件负责：
- 具体方法
- 审稿标准
- 数据结构
- 操作协议

## 建议上传的核心文件

第一层：
- PROJECT_INSTRUCTIONS.md
- 00_CORE/WORKFLOW.md

第二层：
- 01_STORY_ARCHITECT/STORY_CORE.md
- 02_CHARACTER/CHARACTER_PSYCHOLOGY.md
- 02_CHARACTER/CHARACTER_ARC.md
- 02_CHARACTER/RELATIONSHIP_DYNAMICS.md
- 03_STRUCTURE/STORY_STRUCTURE.md
- 03_STRUCTURE/CAUSALITY_AND_TURNING_POINTS.md
- 03_STRUCTURE/FORESHADOWING.md

第三层：
- 04_WRITER_HANDOFF/CHAPTER_SPEC.md
- 05_RED_TEAM/CHAPTER_AUDITOR.md
- 05_RED_TEAM/CONTINUITY_AUDITOR.md
- 05_RED_TEAM/LOGIC_AUDITOR.md
- 05_RED_TEAM/REJECTION_STANDARD.md
- 06_OPERATIONS/OPERATIONS.md
- 06_OPERATIONS/COMMAND_ROUTER.md

## 使用方式

建议每一个小说建立独立 Project。

Project 中保存：
- 当前故事核心
- 当前人物档案
- 世界规则
- 总纲/分卷纲
- 章节状态
- 伏笔表
- 连续性记录
- 红队审稿结果

不要把不同小说长期混在同一个 Project 中。

## 与正文模型的关系

推荐双模型工作流：

ChatGPT Story Architect
→ 设计、验证、交接

正文模型
→ 根据 Chapter Handoff 写初稿

ChatGPT Red Team
→ 审查初稿

ChatGPT
→ 生成修改指令

正文模型
→ 修改

ChatGPT
→ 二审

## 重要边界

本项目默认不追求“AI 自己把小说一路写完”。

核心目标是：
降低结构性崩盘、人物失真、伏笔失效和连续性错误，同时保留作者的最终创作决策权。
