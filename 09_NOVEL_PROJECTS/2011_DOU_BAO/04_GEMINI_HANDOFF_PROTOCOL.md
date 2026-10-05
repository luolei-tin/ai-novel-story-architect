# Gemini 写作交接协议

## Gemini 的角色

`Prose Writer / Scene Executor`

Gemini 的任务不是重新设计整本小说。

## 每次交接必须提供

### A. Starting State

这一章开始时：

- 主角处境；
- 关键人物关系；
- 已知信息；
- 资源；
- 上一章后果。

### B. Dramatic Contract

必须明确：

- 主角想要什么；
- 谁想阻止；
- 双方筹码；
- 信息差；
- 主要策略；
- 可能的反转；
- 必须做出的选择；
- 必须支付的代价；
- Ending State。

### C. Forbidden Moves

明确：

- 不得让豆包获得未定义能力；
- 不得让主角突然拥有未建立的商业资源；
- 不得让配角为了主角自动放弃利益；
- 不得跳过关键谈判/交付/失败过程；
- 不得用旁白宣布人物已经成长。

### D. Prose Freedom

Gemini 可以自由决定：

- 场景调度；
- 句式；
- 对话表达；
- 感官细节；
- 非结构性小事件；
- 叙事节奏。

## Deviation Report

正文完成后，Gemini 应主动返回：

- 哪些 Handoff 被完整执行；
- 哪些地方为了可读性做了调整；
- 是否发现结构冲突；
- 是否新增事实；
- 是否改变人物行为动机；
- 是否改变 Ending State。

## 质量底线

不要把：

“人物说了一句正确的话”

当作：

“人物完成了心理变化”。

人物变化必须通过行为、选择和代价体现。
---

## Writer Skill Integration

`05_GEMINI_WRITER_SKILL.md` 是本项目 Gemini 的长期正文写作规范。

它与本协议的关系：

- `05_GEMINI_WRITER_SKILL.md` = 如何写；
- `04_GEMINI_HANDOFF_PROTOCOL.md` = 如何交接；
- 当前模块 Handoff / Task Prompt = 这一次写什么。

推荐执行顺序：

`Story Bible`
→ `Project Status`
→ `Open Questions`
→ `05_GEMINI_WRITER_SKILL.md`
→ 当前模块 Handoff
→ 当前 Task Prompt
→ 正文

Gemini 不得因为当前 Task Prompt 较短，而忽略 05 的长期写作约束。

同样，05 也不能替代当前 Handoff；它不能自行决定未锁定的剧情事实。