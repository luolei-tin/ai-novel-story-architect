# Chapter Red-Team Auditor

## 判定

- PASS：声明范围内的检查完成并成立；章节总体放行还必须满足独立 Dramatic PASS 与全部必要检查。
- 戏剧检查必须引用 DRAMATIC_INTEGRITY_AUDITOR.md，完整场景清单和独立判定不得省略。
- 先执行 ../07_VALIDATION/BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md 的独立正文审查并冻结，再对照 Handoff。
- QA_PASS 只由 ../07_VALIDATION/VALIDATION_PROTOCOL.md 的 Chapter Closure Gate 决定。
- CONDITIONAL PASS：可继续，但存在明确的小缺口。
- REVISE：章节目标或因果链存在实质问题，需要修改。
- REJECT：章节建立在错误因果、人物失真、严重连续性错误或强行推进上。

## 1. Causality
- 本章为什么发生？
- 谁造成了变化？
- 是否存在被作者隐藏的关键前提？
- 如果删除某个人物选择，本章是否仍然发生？

## 2. Character
- 每个人知道什么、不知道什么？
- 当前选择是否符合心理结构？
- 为什么现在做，而不是三章前？
- 是否为了推进剧情而突然降智/升智？

## 3. Structure
本章至少造成一种有效变化：
- 新信息
- 新关系状态
- 新风险
- 新选择
- 新代价
- 新不可逆后果

如果什么都没改变，本章需要重新设计。

## 4. Foreshadowing
对每个伏笔/回收：
- 首次种植在哪里？
- 读者是否有机会注意？
- 回收是否由此前信息支持？
- 是否过早泄底？
- 是否只是事后解释而非真正伏笔？

## 5. Information Integrity
分别列出：
- Reader knows
- Protagonist knows
- Other characters know
- Unknown

禁止审稿时用作者视角替代人物视角。

## 6. Verdict
先列致命问题，再列一般问题，最后给 Verdict。
REJECT 时必须说明“哪条因果链断了”以及“最低修改路径”。
