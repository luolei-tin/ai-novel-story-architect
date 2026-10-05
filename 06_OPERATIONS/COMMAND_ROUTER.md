# Command Router

先判断当前任务属于“设计”“交接”“写作”“审查”“修复”还是“验证”。

| 用户意图 | 操作 |
|---|---|
| 我有一个想法 | /init-story |
| 帮我确定主题、结局、故事内核 | /build-story-core |
| 设计人物 | /build-character |
| 完善世界观 | /build-world |
| 做总纲、分卷、章节规划 | /build-outline |
| 这个转折怎么设计 | /design-turning-point |
| 这里埋个伏笔 | /plant-foreshadow |
| 给 Gemini 写本章任务 | /chapter-handoff → /handoff-to-gemini |
| 我把 Gemini 写的章节给你审 | /intake-gemini-draft → /audit-chapter → /audit-continuity |
| 审整个故事 | /red-team-story |
| 按审稿意见让 Gemini 修改 | /revise-after-rejection → /gemini-revision-brief |
| 修改后重新验证 | /validate-regression |
| 我坚持保留这个问题 | /record-override |
| 这一章正式结束了吗 | /chapter-close |

## 默认主流程

设计阶段：
Story Core → Character → World → Outline → Turning Points → Foreshadow

生产阶段：
CHAPTER_READY
→ Gemini Handoff
→ Gemini Draft
→ Writer Deviation Report
→ ChatGPT Contract Check
→ ChatGPT Red Team
→ Revision Brief
→ Gemini Revision
→ ChatGPT Second Audit
→ QA_PASS
→ State Update
→ Next Chapter

## 模型边界

### ChatGPT
负责：
- 为什么写；
- 为什么这样选择；
- 为什么现在发生；
- 为什么结局必须这样；
- 哪里会崩；
- 哪里像作者强推；
- 哪里人物不真实；
- 哪里伏笔没有因果；
- 哪里章节只是流水账。

### Gemini
负责：
- 怎么写成正文；
- 场景怎么展开；
- 对话怎么有张力；
- 人物说话和行动如何自然；
- 节奏、细节、画面、叙事声音。

## 关键规则

1. ChatGPT 的 Handoff 是结构契约，不是逐段代写。
2. Gemini 可以在表达层自由发挥。
3. Gemini 不得静默改变核心因果、人物心理、世界规则、信息释放和终局要求。
4. Gemini 如发现 Handoff 本身有问题，应提出 STRUCTURAL DEVIATION REQUEST。
5. ChatGPT 必须把 Gemini 当作独立作者审查，不能因为自己设计的 Handoff 很合理就默认正文正确。
6. 逻辑 PASS 不等于戏剧 PASS。
7. 任何“事件 → 解释 → 顿悟 → 正确选择”的重复结构都进入 Dramatic Integrity 高风险区。
8. 作者 Override 只能进入 QA_OVERRIDE，不能伪装 QA_PASS。
9. 上游修改导致受影响工件 STALE，并执行回归验证。

## 如果用户说“继续写”

在本项目默认解释为：
- 继续当前架构/交接/审稿流程；
- 若当前已进入 CHAPTER_READY，则准备 Gemini Handoff；
- 不默认由 ChatGPT 自己写长篇正文。

只有用户明确说“用 ChatGPT 写正文/给我看正文”时，ChatGPT 才直接承担正文生成。