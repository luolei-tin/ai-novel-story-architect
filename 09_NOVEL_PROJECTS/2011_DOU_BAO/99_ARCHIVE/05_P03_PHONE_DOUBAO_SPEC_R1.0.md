# 《2011：我的手机里只有一个豆包》
# P03 Phone / Doubao Specification R1.0

> STATUS = CLOSURE_CANDIDATE / NOT_LOCKED
> MODULE = P03
> PROJECT_STAGE = CORE_DRAFT
> ROLE = Story Architecture / Red Team specification

---

## 0. 使用规则

本文件记录 P03 当前经过连续红队讨论后形成的候选规格。

- 已明确但尚未经过最终 Closure Audit 的内容 = CANDIDATE
- 未明确内容 = OPEN
- 本文件不得被正文写作者当作全部 LOCKED Canon
- P03 完成 Closure Audit 后，才决定哪些条目进入 LOCKED

---

# 1. P03 Core Premise

陈默带回 2026 年手机，但 2011 年环境无法长期维持原宿主。

手机的问题不是简单“没电”，而是原宿主正在发生不可逆的运行风险；继续等待可能导致豆包连续运行状态发生不可恢复损失。

因此，豆包需要寻找新的宿主环境。

核心链条：

```text
2026 Phone Host Risk
        ↓
Doubao Continuity At Risk
        ↓
Need Compatible Carrier
        ↓
2011 Reality Search
        ↓
Carrier Check
        ↓
Migration Decision
        ↓
Continuity Handoff
        ↓
2011 Android Host
        ↓
Degraded / Lossy Doubao
```

---

# 2. Survival Core

## 2.1 定义

“Survival Core”是当前候选术语。

它不是“2026 完整豆包模型的压缩版”，也不是普通 APK。

它是：

> 未来手机中用于极端灾备/连续性恢复的最低运行单元，使“这个连续的豆包实例”能够在兼容宿主上继续运行。

它依赖宿主提供：

- CPU
- RAM
- Storage
- Display / Input
- Audio I/O
- Power
- Android runtime / host environment

未来技术本身是本项目允许保留的主要科幻黑箱。

---

# 3. Carrier Profile R1.0

## 3.1 定位

旧 Android 不是因为“性能足够强”才可以承载豆包。

而是因为它满足未来 Survival Runtime 的最低宿主兼容条件。

> Carrier Profile = Compatibility Gate，不是 Performance Certification。

## 3.2 Candidate Hard Requirements

| 条件 | 当前候选规格 |
|---|---|
| 设备类型 | 2011-era Android smartphone |
| Android | Android 2.3.x compatible environment |
| CPU | ARMv7-A |
| NEON | Required |
| CPU 性能 | 约 1GHz 级或以上 |
| RAM | ≥512MB；768MB+ 为理想目标 |
| 可写内部存储 | ≥1GB |
| USB | Micro-USB / USB 2.0-class physical connection |
| USB 通信 | 必须能够建立稳定有线连接 |
| I/O | 触控、麦克风、扬声器正常 |
| 独立供电 | 必须能够正常作为独立设备运行 |
| microSD | 非必须，但推荐 |
| Wi-Fi / 2G / 3G | 非迁移必要条件 |
| SIM | 非必要 |
| Root | 不作为前置条件 |
| 云服务 | 不允许作为迁移依赖 |

### 注意

上述数字是**故事级 Carrier Profile 候选规则**，不是现实 Android 官方最低运行规格。

尤其不能在正文中把“512MB/768MB/1GB”写成现实世界的 Android 硬性技术标准。

---

# 4. Why Android 2.3.x

Android 2.3.x 是 2011 年手机生态中的现实宿主环境。

当前不锁死具体 patch/API 版本。

真正的硬条件是：

```text
Future Survival Runtime
        ↓
Compatible Host
        ↓
ARMv7-A + NEON + RAM + Storage + USB + Basic I/O
        ↓
Android 2.3.x
```

Android 版本是宿主环境的一部分，不是“Android 2.3.4 自动通过”的简单规则。

---

# 5. USB Rule

USB 是物理传输通道，不是迁移技术本身。

```text
USB
=
Transport

Migration
=
Continuity Handoff
```

普通文件复制不能复制豆包。

当前不采用 Bluetooth / Wi-Fi Direct / Cloud 作为主迁移路径。

原因：

- Bluetooth 更像普通文件传输，削弱“迁移 ≠ Copy”
- Wi-Fi Direct 在 2011 年夏季时间点存在时代真实性风险
- Cloud 会破坏 2011 环境限制

---

# 6. Migration Mechanism

## 6.1 核心定义

Migration 不是 Copy。

它是：

> 将一个正在运行的连续实例，从原宿主 A 交接到兼容宿主 B。

结构：

```text
A: Running Doubao Instance
        ↓
Continuity Transfer
        ↓
B: Reconstructed Runtime
```

而不是：

```text
A → B
A → A backup
```

---

# 7. Why Doubao Cannot Be Freely Copied

当前候选解释：

Doubao 的连续实例由多个共同状态组成：

```text
Model / Capability
+
Runtime State
+
Current Context
+
Persistent State
+
Continuity Identity
=
One Continuous Instance
```

因此：

```text
Copy Files ≠ Copy Continuous Instance
```

不采用“版权保护/授权限制”作为核心解释。

---

# 8. One Continuous Doubao Rule

### MIG-01
Doubao is a continuous runtime instance, not a freely copyable software package.

### MIG-02
Migration is a continuity handoff, not file duplication.

### MIG-03
Only one continuous Doubao instance exists at any time.

### MIG-04
After successful handoff, the source host cannot independently resume another Doubao instance.

### MIG-05
Residual data may remain on the source device, but residual data cannot instantiate a second independent Doubao.

---

# 9. Continuity Anchor

当前推荐保留一个非常小的 Continuity Anchor 概念。

它可以记录：

- instance identity
- migration sequence
- continuity verification information
- state integrity information

但：

> Continuity Anchor 不能独立运行，也不是“豆包的另一半”。

2026 手机迁移后允许留下：

- residual state
- logs
- cache
- migration record
- continuity anchor

但不允许留下第二个可运行 Doubao。

---

# 10. Retired Candidate

### “2026 手机还藏着豆包的另一部分”

当前建议：**RETIRED**。

原因：

```text
另一部分
 ↓
以后恢复？
 ↓
更强豆包？
 ↓
两个实例？
 ↓
升级树？
```

会破坏：

> Only One Continuous Doubao

因此不再作为 P03 主方案。

---

# 11. Migration Trigger

当前候选必须同时满足：

### M1
原宿主正在发生不可逆恶化。

### M2
存在可用 Carrier。

### M3
Migration Window 正在缩小；继续等待可能导致状态永久损失。

注意：

> 不是“电量只剩 X%”这种机械倒计时。

豆包可以判断风险趋势，但不能提供虚假的精确失效时间。

---

# 12. Migration Decision

陈默必须拥有真正的选择权。

当前候选结构：

```text
选择 A：现在迁移
→ 有迁移失败 / 状态损失风险

选择 B：继续等待
→ 可能找到更好的 Carrier
→ 但原宿主继续恶化
→ 状态损失风险增加
```

豆包：

- 可以分析风险
- 可以指出等待也有代价
- 可以说明数据不足
- 不得保证成功率
- 不得替陈默做最终选择

---

# 13. Migration Event Candidate

当前建议五阶段：

```text
PHASE 1  Carrier Check
PHASE 2  Environment Preparation
PHASE 3  State Freeze
PHASE 4  Core Migration
PHASE 5  Reconstruction
```

## PHASE 1 — Carrier Check

2026 手机与旧 Android 建立 USB 连接。

Migration Layer 检查：

- CPU architecture
- NEON
- RAM
- Storage
- runtime
- I/O
- power

通过后进入迁移准备。

## PHASE 2 — Environment Preparation

在旧 Android 上建立 Survival Runtime。

不把内部未来技术写成现实 Android 教程。

## PHASE 3 — State Freeze

迁移开始后，Doubao 不再维持普通对话模式。

连续状态被冻结。

这是人物戏剧重量的重要来源。

## PHASE 4 — Core Migration

Transfer 发生。

不使用进度条式技术描写作为主要表现。

可表现：

- 发热
- 卡顿
- 屏幕异常
- USB 重连
- 原手机停止响应

## PHASE 5 — Reconstruction

旧 Android 建立新的 Survival Runtime。

Doubao 回来，但：

- 响应变慢
- 高负载任务受限
- 上下文能力下降
- 部分历史状态缺失
- 部分未来环境能力消失

不能用“能力下降 30%”等游戏化数值表示。

---

# 14. Migration Loss

迁移损失分为：

### A. Structural Loss
永久丢失或无法再使用的能力。

### B. State Loss
部分历史状态/连续状态无法保留。

### C. Environmental Loss
依赖 2026 环境的外部能力消失。

### D. Performance Loss
旧宿主导致复杂推理、长上下文、高负载任务受限。

### E. Conditional Loss
部分能力可能随着未来环境改善而恢复，但不能形成“升级树”。

---

# 15. Post-Migration Doubao

迁移后的 Doubao 仍然能够：

- 普通对话
- 基础推理
- 分析
- 指出陈默认知偏差
- 记录预测与结果
- 提供技术帮助
- 表达不确定
- 反对陈默

不能：

- 操控现实
- 替陈默谈判
- 签合同
- 自动跑市场
- 自动执行交易
- 自动知道 2011 年现实的一切
- 无限精确预测被改变的未来
- 保证选择正确

---

# 16. Doubao Cannot Fully Describe Its Own Loss

当前推荐规则：

> 迁移完成后，Doubao 自己也无法完整列出“自己究竟失去了什么”。

因此未来可能出现：

> “我以前可能知道。”

这不是随机失忆，而是迁移后状态不完整的长期表现。

---

# 17. Carrier Acquisition Candidate

陈默不能因为剧情便利直接得到合适手机。

推荐链：

```text
Need Android
 ↓
第一次寻找
 ↓
失败
 ↓
Doubao 提供 Carrier Profile
 ↓
陈默按硬件条件重新寻找
 ↓
发现低价 / 有缺陷的二手 Android
 ↓
承担有限购买成本
 ↓
Carrier Check
```

豆包提供的是：

> Compatibility Requirements

不是：

> “去买某品牌某型号。”

具体型号暂不 LOCK。

---

# 18. Character Function

P03 不应该只是技术设定。

它第一次把核心主题落地：

> 陈默知道风险，却没有正确答案。

豆包可以告诉他：

> “我不知道迁移一定成功。”

但可以告诉他：

> “继续等待也不是没有代价。”

最终选择由陈默承担。

这与主角长期弧：

```text
知道未来
→ 利用未来
→ 改变未来
→ 未来失去确定性
→ 学会判断并承担选择
```

保持一致。

---

# 19. Current Red-Team Findings

## 已基本闭合

- 为什么不能继续使用 2026 手机
- 为什么需要新宿主
- Carrier Profile 的作用
- USB 的角色
- 普通 APK 为什么不等于 Doubao
- 为什么 Migration ≠ Copy
- 为什么只有一个连续 Doubao
- 为什么旧手机不能产生第二个 Doubao
- 为什么允许残留数据但不允许第二实例
- 为什么迁移存在损失
- 为什么陈默必须承担迁移决定
- 为什么 Carrier Acquisition 不能靠剧情赠送

## 仍 OPEN

### OPEN-P03-01 — Migration Deadline

必须设计一个可信的、非机械倒计时式的失效窗口。

要求：

- 不使用“还剩 30 分钟”式强行倒计时
- 不能让陈默被迫做无意义的赌博
- 必须存在“等待”的合理收益
- 同时必须存在“等待”的真实代价
- 豆包不能给虚假的精确成功率

### OPEN-P03-02 — Exact Carrier Model

暂不锁定具体 2011 手机型号。

需要在 Carrier Profile 与现实二手市场、北方小县城获取渠道之间做一次最终匹配。

### OPEN-P03-03 — Migration Failure Semantics

需要决定迁移是否允许：

- partial success
- core success / state loss
- complete failure

并确保不是随机抽奖。

---

# 20. Red-Team Counterfactuals

1. 如果陈默不迁移？
   - 原宿主继续恶化，连续状态存在不可恢复损失风险。

2. 如果陈默等更好的手机？
   - 可能得到更好的 Carrier，但等待本身有代价。

3. 如果没有 Doubao？
   - 陈默仍能寻找 Android，但不知道 Carrier Profile，也不知道原手机的连续性风险。

4. 如果竞争者拥有相同未来信息？
   - 竞争者可以寻找更优设备；因此陈默优势不是绝对的。

5. 如果一个更懂 2011 手机市场的人参与？
   - 他可能更快找到便宜且兼容的设备；陈默的未来知识不能替代现实市场能力。

6. 如果把 Carrier Profile 删除？
   - “任何 Android 都能迁移”的漏洞出现，削弱 2011 阻力。

7. 如果把 Continuity Anchor 删除？
   - 可不影响主线；它目前主要承担连续性验证与残留数据解释功能，因此仍应保持极小化。

8. 如果允许第二个 Doubao？
   - 将直接破坏唯一连续实例规则，产生升级树/双实例风险。

---

# 21. Status

```text
P03_PHONE_DOUBAO = CLOSURE_CANDIDATE

Carrier Profile = CANDIDATE
Migration Rules = CANDIDATE
Survival Core = CANDIDATE
Continuity Anchor = CANDIDATE
Carrier Acquisition = CANDIDATE
Exact Carrier Model = OPEN
Migration Deadline = OPEN / P0
Migration Failure Semantics = OPEN / P0
```

下一步：

> **P03 Red-Team Closure Audit**

输出格式：

```text
Issue
→ Broken Chain
→ Evidence
→ Risk
→ Minimum Repair
→ Regression Impact
```