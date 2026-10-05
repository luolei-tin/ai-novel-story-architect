# Validation Protocol

本文件把“审稿意见”升级为可验证的工程状态，而不是普通建议。

## 1. Validation Principle

任何故事工件都有：

- State：当前状态
- Version：版本
- Upstream Dependencies：依赖的上游工件
- Evidence：支持当前结论的证据
- Verdict：验证结果

“已经写出来”不等于“已经验证”。

## 2. Lock Rule

以下状态只有在对应上游工件稳定后才允许成立：

SEED → CORE_DRAFT → CORE_LOCKED → CHARACTER_LOCKED → WORLD_LOCKED → OUTLINE_LOCKED → CHAPTER_READY → DRAFT → QA_REVISE → QA_PASS

任何已锁定工件发生实质修改：

1. 原锁定状态立即失效；
2. 所有直接依赖它的下游工件标记 STALE；
3. 不得继续使用旧的 QA_PASS；
4. 必须重新验证受影响范围。

## 3. Dependency Invalidation

修改：

- Story Core → 至少重新检查 Character / World / Outline / Turning Points / Chapter Handoff。
- Character Psychology → 至少重新检查相关 Turning Points / Outline / Chapter Handoff。
- World Rule → 至少重新检查受影响 Causality / Outline / Foreshadowing / Chapters。
- Outline / Turning Point → 至少重新检查受影响 Chapter Handoff / Foreshadowing。
- Chapter prose → 至少重新执行 Chapter Audit + Continuity Audit。

不得因为“改动看起来很小”而跳过依赖判断。

## 4. Evidence Rule

每个重大 Verdict 必须能回答：

- 检查了什么？
- 依据哪个版本？
- 发现了什么事实？
- 哪条规则被满足或违反？
- 结论是什么？

禁止只输出“感觉成立”“整体没问题”“建议修改”。

## 5. Regression Rule

REVISE / REJECT 后：

DRAFT → QA_REVISE → 修改 → 受影响审查重跑 → 若仍有 FATAL/HIGH：继续 REVISE/REJECT → 全部必要检查通过 → QA_PASS

不得从 REJECT 直接跳到 PASS。

## 6. Scope of Revalidation

不是所有修改都要求整本小说重审。

审查人必须明确：

- Changed Artifact
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected

如果无法证明某项“不受影响”，默认标记为需要检查。

## 7. Validation Record

建议每次审查保存：

- Audit ID
- Date
- Artifact Version
- Upstream Versions
- Checks Performed
- Findings
- Verdict
- Required Repairs
- Revalidation Scope

## 8. PASS Meaning

PASS 不是“目前没有发现问题”。

PASS 的含义是：

> 在声明的检查范围、工件版本和可用证据下，没有发现足以阻止继续推进的问题。

不得把有限范围的 PASS 扩大解释为“整个故事绝对成立”。
