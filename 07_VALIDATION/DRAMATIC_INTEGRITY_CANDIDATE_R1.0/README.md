# Dramatic Integrity 候选补强包 R1.0

日期：2026-10-08（Asia/Shanghai）。
需求：[issue #3](https://github.com/luolei-tin/ai-novel-story-architect/issues/3)。
源基线：main@2694f2aa0b427ab8abdfd3548c514abf774ed8d3。
状态：CANDIDATE / DRAFT_PR / CONTROLLED_TESTS_EXECUTED / FULL_ACCEPTANCE_PENDING。
本包不声明生产验收通过，不关闭 issue，不改变小说 Canon，也不复活旧四章的历史 PASS。

## 材料

- [正文盲测样本](BLIND_CASES_R1.0.md)：10 个混排缩微章节。只与候选审查规则一起给审稿人。
- [作者侧预期与验收](AUTHOR_EXPECTED_R1.0.md)：七个目标负例、三个正例、两个流程陷阱。不得给盲审人。
- [ChatGPT 项目导入包](CHATGPT_PROJECT_IMPORT_R1.0.md)：候选资料说明与四份核心协议，可同步到现有项目资料。
- [校验清单](MANIFEST_R1.0.json)：文本文件的 SHA-256；用于源版本与同步一致性检查。

答案虽然在仓库公开，执行盲测时仍必须通过输入隔离隐藏。
ChatGPT 的 Pass A 应在不载入本项目知识库的独立上下文进行；不能先读取设计/答案再声称暂时忘记。

## 规则入口

- [七项唯一验收表](../../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md)
- [章节关闭记录](../AUDIT_RECORD.md)
- [关闭与重验证门槛](../VALIDATION_PROTOCOL.md)
- [独立正文盲审协议](../BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md)

同一分支另有 12 个已有协议文件的候选改动。核心标准集中在审稿器；其他文件接通证据记录、关闭门槛、盲审顺序与新项目继承。
每项检查必须有正文位置、事实、机制和判定；不能用平均分、文笔或逻辑通过抵消戏剧失败。

QA_PASS 必须同时满足当前版本的 Logical PASS、独立 Dramatic PASS、全部必要检查完成、无阻断性未关闭问题、场景/七项证据完整和基线版本匹配。
INCOMPLETE 是检查状态，NOT_CLOSED 是关闭决策；并不替换已有 Verdict 枚举。
桥接场景的 N/A 需要证据与作用说明，不能豁免整章。

## 验证情况

已完成：候选补丁在源基线的本地内容副本上通过应用检查，18 处协议相对引用解析成功，10 个样本 ID 完整且唯一。
已完成：A1 独立受控盲测、A2 结构修复与流程门槛回归、A3 原四章正文优先复查。详见实际结果。
未完成：边界条款版本化重测、新 Dramatic Contract 的初稿—返修—二审完整闭环及跨审稿人复核。

缩微样本用于诊断，不是严格的单变量消融；目标缺陷可能伴随其他缺口。
未来测得标签命中但证据不实，仍判本轮未通过；不能事后悄悄改答案制造 PASS。

## 下一步

1. 审阅本分支候选规则及误拒收边界。
2. 冻结独立 Pass A，按作者侧预期核对标签与证据。
3. 修复一个负例并重审，证明结构修复而非解释增补关闭缺陷。
4. 用新的 Dramatic Contract 做生产闭环。
5. 根据真实结果决定采用范围与 issue #3 验收状态。


## 2026-10-08 实际验收进展

- [实际验收结果](ACCEPTANCE_RESULTS_R1.0.md)：A1标签10/10吻合、七个目标缺陷识别、修复与四个流程控制、原四章的两PASS/一REJECT/一REVISE。
- [测试包自身红队](TEST_PACKAGE_REVIEW_R1.0.md)：混合缺陷、显式提示与覆盖不足。
- [边界条款候选R1.2](BOUNDARY_CLARIFICATIONS_R1.2_CANDIDATE.md)：尚未替换有效规则，未用旧测试为它背书。
- [运行输入、原始判定便携副本与哈希](RUNS_R1.0/RUN_MANIFESTS_R1.0.json)。

原始报告在本地保持冻结；仓库副本只将机器路径替换成可追溯的仓库路径并统一行尾，不改判定或证据。
早期输入/预期/导入文件内NOT_EXECUTED是出题或同步前的冻结进度快照；当前执行状态以本节与实际结果为准。
这不表示正式采用、生产QA_PASS或issue关闭。收束、策略与互动边界仍需修订验证。
