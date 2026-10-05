# 《2011：我的手机里只有一个豆包》

本目录是独立小说项目，不等同于通用 Story Architect 方法库，也不继承旧的 V1.3 正文实验作为质量基准。

## 项目定位

类型：重生 / 都市 / 商业 / 互联网 / 人物成长

核心设定：

> 主角从 2026 年重生回 2011 年，身边只剩下一部来自 2026 年的手机，以及手机里唯一还能正常使用的“豆包”。

本项目的目标不是写一部“AI 百科全书式开挂爽文”，而是建立一条经得起长期审查的成长故事：

**知道未来 → 利用未来 → 改变未来 → 失去对未来的确定性 → 学会在未知中做决定。**

## 双模型职责

- ChatGPT：Story Architect / Chief Editor / Red Team
- Gemini：Prose Writer / Scene Executor
- 作者：最终创作决策者

ChatGPT 对结构拥有审查权，但不默认拥有最终创作权。
Gemini 对正文表达拥有自由，但不得静默改变已经锁定的核心因果、人物心理和章节状态。

## 当前状态

`CORE_DRAFT / CORE_RED_TEAM`

P03：`CLOSURE CANDIDATE / NOT_LOCKED`

当前不进入正文量产。

## 当前权威文件

### Current Canon

- `00_PROJECT_STATUS_R1.2.md`：当前项目状态、决策、变更记录
- `01_STORY_BIBLE_R1.1.md`：当前 Story Core 事实基线
- `02_OPEN_QUESTIONS_R1.2.md`：当前未锁定问题
- `P03_PHONE_DOUBAO_SPEC_R1.1.md`：当前 P03 工作基线

### Governance

- `03_CHATGPT_DESIGN_PROTOCOL.md`：ChatGPT 设计、审查与红队协议
- `04_GEMINI_HANDOFF_PROTOCOL.md`：Gemini 写作交接协议

### Working / Archive

- `98_WORKING/`：当前仍在处理、尚未并入 Current Canon 的工作材料
- `99_ARCHIVE/`：历史版本与已被替代的工件

## 新对话读取原则

默认读取：

1. `01_STORY_BIBLE_R1.1.md`
2. `00_PROJECT_STATUS_R1.2.md`
3. `02_OPEN_QUESTIONS_R1.2.md`

涉及具体模块时，再读取对应 Module Spec。

`99_ARCHIVE/` 默认不作为当前 Canon 读取，只有追溯历史版本时才使用。

## 重要原则

1. 不因为设定很爽就认为故事成立。
2. 不因为商业逻辑正确就认为章节有戏。
3. 不让豆包成为万能答案机。
4. 不允许主角只凭“知道历史”自动解决现实问题。
5. 每个重要选择都必须有成本、风险和不可逆后果。
6. 配角不能只是为主角服务。
7. 每章必须产生状态变化，而不是只增加事件数量。
8. 结构修改后，下游章节必须重新审查。
9. ChatGPT 必须主动反驳作者和自己此前的方案。
10. “写出来了”不等于“成立了”。

## 第一原则

> 任何时候都先问：如果把这个设定拿掉，故事还成立吗？

如果答案是“成立”，就说明这个设定可能只是装饰；
如果答案是“完全不成立”，则必须继续检查它是否已经变成过度依赖的外挂。
