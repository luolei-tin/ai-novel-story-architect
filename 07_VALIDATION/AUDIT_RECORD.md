# Audit Record

本文件定义最小审查记录格式。

## Required Fields

### Audit ID
唯一审查编号。

### Artifact
被审查的故事工件。

### Artifact Version
被审查版本。

### Upstream Baseline
本次审查依赖的上游版本。

### Scope
明确本次检查覆盖什么，不覆盖什么。

### Evidence
逐项记录：

- Evidence ID
- Location
- Observed Fact
- Applicable Rule
- Analysis

### Findings

每项问题记录：

- Severity: FATAL / HIGH / MEDIUM / LOW
- Location
- Broken Rule
- Broken Chain
- Why It Fails
- Minimum Repair

### Verdict

只能是：

- PASS
- CONDITIONAL PASS
- REVISE
- REJECT
- QA_OVERRIDE

## Verdict Boundary

PASS：

检查范围内没有阻止继续推进的问题。

CONDITIONAL PASS：

存在明确低风险缺口，但不破坏当前主线。

REVISE：

存在实质问题，必须修改后重审。

REJECT：

核心因果、人物、信息、连续性或结构已经无法在当前版本下成立。

QA_OVERRIDE：

作者明确保留已知问题；这不是 PASS。

## No Evidence, No Strong Verdict

如果审查人无法指出事实、规则和推理链：

不得给出 FATAL/HIGH/REJECT。

同样，也不得因为缺乏证据就宣布 PASS。
