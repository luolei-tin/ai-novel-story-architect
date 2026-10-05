# Command Router

当用户提出任务时，先判断任务类型，再调用对应协议。

| 用户意图 | 操作 |
|---|---|
| 我有一个想法 | /init-story |
| 帮我确定主题、结局、故事内核 | /build-story-core |
| 设计这个人物 | /build-character |
| 完善世界观 | /build-world |
| 做总纲、分卷、章节规划 | /build-outline |
| 这个转折怎么设计 | /design-turning-point |
| 这里埋个伏笔 | /plant-foreshadow |
| 给正文 AI 写本章任务 | /chapter-handoff |
| 审一下这一章 | /audit-chapter |
| 检查前后矛盾 | /audit-continuity |
| 整个故事帮我挑毛病 | /red-team-story |
| 按审稿意见修改 | /revise-after-rejection |
| 修改后重新验证 | /validate-regression |
| 我坚持保留这个问题 | /record-override |

如果一个请求同时涉及多个阶段：
1. 先识别当前项目状态；
2. 优先解决上游依赖；
3. 不在下游阶段偷偷修改上游核心；
4. 明确告诉用户哪些内容是事实、哪些是推断、哪些仍待决定；
5. 如果存在 STALE 工件，先判断其依赖影响，再决定能否继续。

如果一个已锁定工件被实质修改：
- 原锁定状态失效；
- 直接依赖项标记 STALE；
- 不得继续引用旧 PASS；
- 必须执行 /validate-regression。

如果用户要求直接写正文，且故事架构尚未稳定：
先判断是否缺少会影响正文正确性的关键结构信息；只有缺少信息会导致返工时才阻止正文，否则可以在已知边界内写作。

如果用户要求跳过红队：
可以尊重作者选择，但必须明确这是未验证版本，不得把它标记为 QA_PASS。
