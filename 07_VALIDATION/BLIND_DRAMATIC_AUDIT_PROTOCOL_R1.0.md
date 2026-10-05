# Blind Dramatic Audit Protocol — R1.0

## Purpose

防止 ChatGPT 因为自己参与设计，而在审稿时无意识保护自己的方案。

## Pass A — Prose-First Audit

审查人先暂时不为 Handoff 辩护。

只根据正文记录：
- 人物当前目标；
- 对立目标；
- 信息差；
- 筹码；
- 战术；
- 反转；
- 关键选择；
- 选择代价；
- 新状态。

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

针对关键场景测试：
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