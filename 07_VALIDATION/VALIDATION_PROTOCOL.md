# Validation Protocol

���ļ��ѡ�������������Ϊ����֤�Ĺ���״̬����������ͨ���顣

## 1. Validation Principle

�κι��¹������У�

- State����ǰ״̬
- Version���汾
- Upstream Dependencies�����������ι���
- Evidence��֧�ֵ�ǰ���۵�֤��
- Verdict����֤���

���Ѿ�д�����������ڡ��Ѿ���֤����

## 2. Lock Rule

����״ֻ̬���ڶ�Ӧ���ι����ȶ��������������

SEED �� CORE_DRAFT �� CORE_LOCKED �� CHARACTER_LOCKED �� WORLD_LOCKED �� OUTLINE_LOCKED �� CHAPTER_READY �� DRAFT �� QA_REVISE �� QA_PASS

�κ���������������ʵ���޸ģ�

1. ԭ����״̬����ʧЧ��
2. ����ֱ�������������ι������ STALE��
3. ���ü���ʹ�þɵ� QA_PASS��
4. ����������֤��Ӱ�췶Χ��

## 3. Dependency Invalidation

�޸ģ�

- Story Core �� �������¼�� Character / World / Outline / Turning Points / Chapter Handoff��
- Character Psychology �� �������¼����� Turning Points / Outline / Chapter Handoff��
- World Rule �� �������¼����Ӱ�� Causality / Outline / Foreshadowing / Chapters��
- Outline / Turning Point �� �������¼����Ӱ�� Chapter Handoff / Foreshadowing��
- Chapter prose �� ��������ִ�� Chapter Audit + ���� Dramatic Audit + Continuity Audit��������޸��Ƿ��ȱ��ת�Ƶ�����������
- ���չ���汾�ı� �� ����鲻��ֱ��֤���¹����µ� QA_PASS��Ϊ��Ӱ��Ļ������¼��������֤��Χ��

������Ϊ���Ķ���������С�������������жϡ�

## 4. Evidence Rule

ÿ���ش� Verdict �����ܻش�

- �����ʲô��
- �����ĸ��汾��
- ������ʲô��ʵ��
- �������������Υ����
- ������ʲô��

��ֹֻ������о�������������û���⡱�������޸ġ���

## 5. Regression Rule

REVISE / REJECT ��

DRAFT �� QA_REVISE �� �޸� �� ��Ӱ��������� �� ������ FATAL/HIGH������ REVISE/REJECT �� ȫ����Ҫ���ͨ�� �� QA_PASS

���ô� REJECT ֱ������ PASS��

## 6. Scope of Revalidation

���������޸Ķ�Ҫ������С˵����

����˱�����ȷ��

- Changed Artifact
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected

����޷�֤��ĳ�����Ӱ�족��Ĭ�ϱ��Ϊ��Ҫ��顣

## 7. Validation Record

����ÿ����鱣�棺

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

PASS ���ǡ�Ŀǰû�з������⡱��

PASS �ĺ����ǣ�

> �������ļ�鷶Χ�������汾�Ϳ���֤���£�û�з���������ֹ�����ƽ������⡣

���ð����޷�Χ�� PASS �������Ϊ���������¾��Գ�������

## 9. Chapter Closure Gate

Ϸ�������� ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md ΪΨһ�ж����ߡ�
ʹ�� AUDIT_RECORD.md �� Chapter Closure Record��

ֻ����������ͬʱ�������ſɽ��� QA_PASS��
1. ��ǰ���İ汾�� Logical Verdict = PASS��
2. ��ǰ���İ汾�� Dramatic Verdict = PASS���������������������Ǿ���֤�ݡ�
3. ��Ҫ�������ԡ����ʡ�ƫ���������ɣ��ṹƫ���ѻ���ȷ������
4. û����ֹ�ƽ���δ�ر����⣬û�б����鴦�� FAIL / INCOMPLETE��
5. ���ġ����λ��ߺ����չ���汾���¼ƥ�䣬��¼δ STALE��

CONDITIONAL PASS ����������ż��� PASS��
ȱ�����ȱ֤��ʱ����δ�رգ�����ƾ�˱��� REJECT ������ PASS��
���߱�����֪ȱ����ʹ�� QA_OVERRIDE�������� QA_PASS��
��ʷ������������¹��������Զ�ת����
