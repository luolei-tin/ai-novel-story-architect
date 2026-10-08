# Blind Dramatic Audit Protocol — R1.0

## Purpose

防止 ChatGPT 因为自己参与设计，而在审稿时无意识保护自己的方案。

## Pass A — Prose-First Audit

Pass A 使用独立审查上下文，只接收待审正文和审查规则。
不提供 Handoff、设计说明、作者解释、Writer Deviation Report、旧审稿结论或测试预期答案。
不得仅凭“暂时不为设计辩护”宣称盲审；若无法隔离，记录 INPUT_CONTAMINATED。该记录不构成盲审验收证据，章节保持未关闭，等待独立正文审查。

先按 ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md 列出完整场景清单与正文范围。
只根据正文记录：
- 人物当前目标；
- 对立目标；
- 信息差；
- 筹码；
- 战术及对方回应；
- 潜台词或言语/行动的实际互动目的；
- 反转；
- 关键选择；
- 选择代价；
- 新状态及它造成或升级的下一问题。

Pass A 完成后冻结版本、证据与判定；Pass B 不覆盖它，只另记更正及理由。

然后回答：

> 如果不知道作者原本想表达什么，这一章本身是否仍然成立？

## Pass B — Contract Audit

再拿正文与 Handoff 对照：
- required objective;
- required causal chain;
- state delta;
- forbidden moves;
- foreshadowing;
- character limits.

## Pass C — Counterfactual Audit

针对每个控制章节走向的关键选择，保存反事实推理及对结果的影响；若结果基本不变，按 Dramatic 验收规则判定缺陷：
- 删除主角选择后是否仍然发生？
- 删除对手阻力后是否仍然成立？
- 对手采取更合理策略后主角是否仍能推进？
- 主角选择相反方案会发生什么？

## Automatic Dramatic Warning

以下任一模式连续出现两个以上场景，至少 REVISE：

事件 → 主角解释 → 主角顿悟 → 正确选择

角色进入 → 提供信息 → 主角理解 → 角色离开

冲突出现 → 商业数字 → 主角计算 → 冲突解决

## Anti-Self-Protection Rule

如果正文与 ChatGPT 原设计冲突：
先判断正文是否更成立。

不能因为“这是 Handoff 要求”就自动判正文正确。

如果 Handoff 本身造成不自然戏剧，应提出 ARCHITECTURE_DEFECT。

## Verdict

Blind audit 可以提出：
- PASS
- CONDITIONAL PASS
- REVISE
- REJECT

理由必须引用正文证据。

缺输入/证据时用检查状态 INCOMPLETE，保持章节未关闭。
最终 Dramatic Verdict 必须遵守唯一验收表，不能用 CONDITIONAL PASS 绕过失败或未完成项。
测试预期判定只由比较步骤读取，不进入 Pass A/B/C 的审稿输入。
