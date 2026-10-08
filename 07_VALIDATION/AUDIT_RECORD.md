# Audit Record

���ļ�������С����¼��ʽ��

## Required Fields

### Audit ID
Ψһ����š�

### Artifact
�����Ĺ��¹�����

### Artifact Version
�����汾��

### Upstream Baseline
����������������ΰ汾��

### Scope
��ȷ���μ�鸲��ʲô��������ʲô��

### Evidence
�����¼��

- Evidence ID
- Location
- Observed Fact
- Applicable Rule
- Analysis

### Findings

ÿ�������¼��

- Severity: FATAL / HIGH / MEDIUM / LOW
- Location
- Broken Rule
- Broken Chain
- Why It Fails
- Minimum Repair

### Verdict

ֻ���ǣ�

- PASS
- CONDITIONAL PASS
- REVISE
- REJECT
- QA_OVERRIDE

## Verdict Boundary

PASS��

��鷶Χ��û����ֹ�����ƽ������⡣

CONDITIONAL PASS��

������ȷ�ͷ���ȱ�ڣ������ƻ���ǰ���ߡ�

REVISE��

����ʵ�����⣬�����޸ĺ�����

REJECT��

��������������Ϣ�������Ի�ṹ�Ѿ��޷��ڵ�ǰ�汾�³�����

QA_OVERRIDE��

������ȷ������֪���⣻�ⲻ�� PASS��

## No Evidence, No Strong Verdict

���������޷�ָ����ʵ���������������

���ø��� FATAL/HIGH/REJECT��

ͬ����Ҳ������Ϊȱ��֤�ݾ����� PASS��

## Chapter Closure Record �� Required

Chapter-level records must use ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md.
Record:
- Prose artifact ID, version, and content hash or immutable commit.
- Audit policy ID/version.
- Pass A inputs and contamination disclosure.
- Complete scene inventory: ranges, type, materiality, and exemption reasons.
- DI-01 through DI-07 evidence, observed mechanism, check status, and findings.
- Central-choice counterfactual outcomes.
- Frozen Pass A record and separately recorded baseline comparison.
- Logical Verdict and Dramatic Verdict.
- Required continuity/foreshadow/deviation checks and current status.
- Open findings, repairs, and revalidation scope.
- Closure Decision: QA_PASS / NOT_CLOSED / QA_OVERRIDE.

An uncompleted check uses Check Status: INCOMPLETE, not a fabricated strong Verdict.
A required INCOMPLETE or material FAIL blocks QA_PASS.
PASS / CONDITIONAL PASS on a limited scope is never the chapter's closure decision.
Policy changes affecting acceptance require revalidation of dependent active artifacts.
