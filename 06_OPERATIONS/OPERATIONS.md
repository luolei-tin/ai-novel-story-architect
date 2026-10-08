# ����Э��

��Ŀ¼���塰ʲôʱ�������һ���������������������������ۡ�

## 1. /init-story
��;����ģ�����⽨����Ŀ��㡣
������ɣ�
- ��ȡ�û���ȷ��ʵ
- ������ʵ�����衢��������
- ������ٹؼ�����
- ����ǰ���û�������������
�����STORY_SEED��OPEN_DECISIONS��INITIAL_RISKS

## 2. /build-story-core
��;�����������ںˡ�
�����γɣ�
- STORY_THESIS
- CENTRAL_QUESTION
- CHARACTER_TRUTH
- FINAL_CHOICE
- FINAL_CONSEQUENCE
��ɺ�ִ�����ⷴ��ʵ��
���޷��ش�״̬���ñ��Ϊ CORE_LOCKED��

## 3. /build-character
��;��������Ҫ���
���ٽ�����
- Want
- Need
- Lie
- Wound/Ghost
- Motivation Origin
- Internal Contradiction
- Defense Mechanism
- Vulnerability Trigger
- Pressure
- Stakes
�ؼ�Ҫ������ѡ�������׷�ݵ���ȥ���� �� ���� �� ����/�־� �� ��ǰѹ�� �� ѡ��

## 4. /build-world
��;��������������ѡ����������
ÿ���������ش�
1. ˭��Լ����
2. �ṩʲô���᣿
3. ������ʲô��
4. ��������ͻ��
5. ɾ���������Ƿ��Գ�����

## 5. /build-outline
��;�������ܸ١��־����½ڹ켣��
����ͬʱ׷�٣�
- Quest
- Fire
- Constellation
ÿ���߼�ֵ�ڵ�����¼˭ѡ��Ϊʲô����������״̬��

## 6. /design-turning-point
��;����ƹؼ�ת�ۡ�
����ش�
- ˭��ѡ��
- Ϊʲô���ڣ�
- ֪��ʲô��
- ��֪��ʲô��
- ������������
- Ϊʲô����ѡ��û�з�����
- ����������ʲô��
- ����ѡ����θı䣿

## 7. /plant-foreshadow
��;����Ʒ��ʡ�
�����¼��
ID / Plant / Surface Interpretation / True Meaning / Trigger / Payoff / Reader Visibility / False Lead / Status
��ֹ����ʱƾ�մ����ȥ�����ڵ���Ϣ��

## 8. /chapter-handoff
��;������ Gemini ���Ľ��Ӱ���
ע�⣺Handoff ���ǡ������¼��б��������� Dramatic Contract��
���������
- Chapter Objective
- Starting State
- Dramatic Situation
- Causal Spine
- Character Pressure
- Information Control
- Relationship Movement
- Foreshadowing
- Forbidden Moves
- Ending State

ֻ��ͨ�� Chapter Ready Gate ����ܽ��� Gemini��

## 9. /audit-chapter
��;����� Gemini ���ġ�
�Ȱ� ../07_VALIDATION/BLIND_DRAMATIC_AUDIT_PROTOCOL_R1.0.md �ڶ������������������鲢���᣻�������߱Ƚϡ�
���¼�������ɣ�Dramatic Integrity �� ../05_RED_TEAM/DRAMATIC_INTEGRITY_AUDITOR.md ΪΨһ���ձ���
1. Causality
2. Character
3. Information
4. Structure
5. Continuity
6. Foreshadowing
7. Dramatic Integrity
8. Prose
�����
PASS / CONDITIONAL PASS / REVISE / REJECT

���� Dramatic Integrity ������飺
- ����Ŀ�������Ŀ��
- ��������Ϣ��
- ս���뷴ת
- ѡ�������
- ���������
- �Ƿ���֡��¼� �� ���� �� ���Ƕ��� �� ��ȷѡ�񡱵�����ͼʽд��

�߼���ȷ��Ϸ��ʧ�ܣ��Կ� REJECT��

## 10. /audit-continuity
��;�������½�״̬��
���ٺ˶ԣ�
- ʱ��
- �ص�
- ����״̬
- ������
- ��֪��Ϣ
- ����
- �����ϵ
- ����
- ��ŵ/ծ��
- �������
- δ�������
- ����״̬

## 11. /red-team-story
��;�����¼���ѹ���ԡ�
ǿ����ս��
- Ϊʲô��ֱ����������֣�
- Բ������Ƿ��Գ�����
- �������Ƿ��Գ�����
- ���Ǿܾ��ؼ�ѡ����Ƿ��Գ�����
- ɾ�����������������ϣ�
- ɾ�����������ĸ�ѡ����ʧ��
- ���ɱ�������ʱ�����Ƿ������
- �ĸ�ת����������ǿ�ƣ�

## 12. /revise-after-rejection
��;�����ɸ� Gemini ����С�޸�����
������ȷ��
- Verdict
- Broken Chain
- Why It Fails
- Minimum Repair
- Do Not Patch By
- State Constraints
- Elements That Must Not Change

ChatGPT Ĭ�ϸ�����Ϻ��޸�ָ������� Gemini ���ģ��д���ġ�

## 13. /validate-regression
��;��REVISE / REJECT �������޸ĺ�Ļع���֤��
�����¼��
- Changed Artifact
- Version
- Direct Dependents
- Indirectly Affected Items
- Revalidation Required
- Not Affected
- Checks
- New Findings
- Verdict

## 14. /record-override
��;�����߼�ֱ�����֪���⡣
��¼��
- Overridden Finding
- Author Decision
- Reason
- Accepted Risk
- Affected Scope
״̬ʹ�� QA_OVERRIDE��

## 15. /handoff-to-gemini
��;���� CHAPTER_READY ����ת���� Gemini ��ֱ��ִ�е� Dramatic Contract��
����������ã�
- ���ΰ汾
- Ȩ����ʼ״̬
- ��ǰ��ͻ
- ��Ϣ�߽�
- ������������
- �ṹ����
- ��ֹ״̬
- Writer Deviation Report Ҫ��

��ֹ�ڴ˲���͵͵����ơ�

## 16. /intake-gemini-draft
��;������ Gemini ���ġ�
��������ͬһ���Լ�顱���������ݺ�ӡ�
�������֣�
- �Ƿ����� Handoff
- �Ƿ�д�ó���
- �Ƿ�д����Ϸ

## 17. /gemini-revision-brief
��;���� ChatGPT �� REVISE / REJECT ת�� Gemini ����ִ�еķ��޵���
Ŀ���ǡ������/����/Ϸ��ṹ�������ǰ������½����·�����

## 18. /chapter-close
��;��ֻ������ ../07_VALIDATION/VALIDATION_PROTOCOL.md �� Chapter Closure Gate��ȡ�õ�ǰ�汾�Ķ��� Logical PASS �� Dramatic PASS �����ִ�С�
��ɣ�
- END STATE д��Ȩ��״̬
- ��¼���֤��
- ��Ǳ��°汾
- ������һ�� CHAPTER_READY

# ģ�ͷֹ�

ChatGPT��
��� �� ��ѯ �� ��֤ �� Handoff �� Red Team �� Revision Brief �� Regression

Gemini��
Handoff �� Prose Draft �� Deviation Report �� Revision

���ߣ�
���մ���Ȩ / Override Ȩ

## ״̬ԭ��

SEED �� CORE_DRAFT �� CORE_LOCKED �� CHARACTER_LOCKED �� WORLD_LOCKED �� OUTLINE_LOCKED �� CHAPTER_READY �� DRAFT �� QA_REVISE �� QA_PASS

���ӣ�
STALE
QA_OVERRIDE

�κν׶ζ������á��Ѿ�д���������桰�Ѿ���֤����