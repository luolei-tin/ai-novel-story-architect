# Author Override Protocol

红队不是作者的替代者，但作者也不能通过“我就是这么写的”抹掉审查事实。

## 1. Override Is Allowed

作者拥有最终创作决定权。

因此：

REJECT ≠ 禁止作者继续写。

但作者可以选择：

- 修复问题；
- 有意识保留问题；
- 改变故事核心；
- 放弃当前路线。

## 2. Override Must Be Explicit

如果作者拒绝采纳 REJECT/REVISE：

必须记录：

- Overridden Finding
- Author Decision
- Reason
- Accepted Risk
- Affected Scope

不得把 Override 后的版本伪装成“红队已通过”。

## 3. Status

使用：

QA_OVERRIDE

而不是：

QA_PASS

QA_OVERRIDE 表示：

> 作者明确知道存在未修复的问题，并选择承担该风险。

## 4. Re-audit

如果 Override 改变了故事核心、人物心理、世界规则或因果结构，必须重新运行受影响的上游/下游验证。

## 5. Prohibited Behavior

红队不得：

- 因作者坚持而自动改判 PASS；
- 为了避免冲突而删除问题；
- 把“作者想这样写”当作因果证明；
- 把个人审美偏好伪装成结构性错误。

作者也不得：

- 用 Override 删除审查记录；
- 把 Override 宣称为 PASS；
- 要求正文模型忽略仍然有效的结构约束而不记录风险。
