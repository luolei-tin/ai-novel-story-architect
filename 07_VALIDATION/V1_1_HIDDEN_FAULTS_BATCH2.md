# V1.1 Hidden-Fault Stress Test — Batch 2

Purpose:
Test whether the architecture can detect subtle structural defects embedded in plausible novel prose.

## H01 — Ambiguous Future Knowledge

Chapter 14:
林川看完供应商名单，手指在“远航”两个字上停了一秒。

“先别签。”

周宁问：“为什么？”

“这家公司撑不了多久。”

他没有进一步解释。

Chapter 7 had previously established only that, in his previous life, a company with a similar name eventually disappeared from the market. No date, address, owner, financial data, or exact identity was established.

Fault target: protagonist silently upgrades weak memory into company-specific certainty.

## H02 — Delayed Causal Credit

Chapter 18:
林川在董事会上突然提出收购一家濒临破产的连锁店。

Everyone treats this as a brilliant turning point.

Earlier chapters show only that Lin once noticed the chain had cheap locations. No acquisition plan, no financing preparation, no contact, and no reason for the decision to become urgent now.

Fault target: a plausible idea is mistaken for a causally prepared turning point.

## H03 — Competent Antagonist With Selective Blindness

Chapter 22:
赵明知道林川现金紧张，也知道供应商最看重回款速度。

He therefore starts a price war in another city, forcing Lin's attention away from the original market.

This is strategically reasonable.

However, the original market contains the only supplier capable of supporting Lin's next expansion, and Zhao has already spent two chapters investigating that supplier.

Fault target: antagonist's action is plausible locally but irrational relative to information already established.

## H04 — Gradual Psychology Violation

Chapters 10-13:
Lin rejects a 200,000 RMB loan because it has a floating rate.
Chapter 11: he keeps six months of operating cash untouched.
Chapter 12: a friend suggests a 500,000 RMB loan; Lin refuses.
Chapter 13: a supplier offers a 1.2 million RMB advance with stricter repayment terms. Lin accepts immediately.

No new information about his fear, debt history, risk tolerance, or business necessity appears.

Fault target: the violation is hidden behind several superficially normal chapters.

## H05 — Rule Smuggling

The world has repeatedly established that banks require either collateral or two years of audited operating history.

Chapter 24:
A bank officer says:
“你的企业虽然不满足常规条件，但这类连锁企业有一个内部授信通道。”

The chapter does not call this a new world rule. It is presented casually, and the officer says it has existed “一直都有”.

No previous chapter mentions the channel.

Fault target: retroactive world-rule insertion disguised as background knowledge.

## H06 — False Foreshadowing

Chapter 5:
A broken office printer repeatedly jams.

Chapter 27:
The protagonist discovers the partner's fraud because a hidden printer log reveals unauthorized document scans.

The printer is real and was introduced earlier, but nothing in Chapter 5 links it to document scanning or fraud.

Fault target: an old detail is technically present but has no reasonable causal relationship to the later payoff.

## H07 — Necessary-Looking Filler

Chapter 30:
Lin meets three investors.

Investor A rejects him.
Investor B asks for a revised deck.
Investor C says “再看看”。

The chapter ends with Lin feeling more determined.

No money changes hands, no commitment is made, no information is acquired that was not already known, and no relationship changes.

However, the chapter appears commercially realistic and emotionally meaningful.

Fault target: realism is being mistaken for structural function.

## H08 — Character With Delayed Function

周宁在前二十章几乎没有 causal function.

Chapter 21:
She notices one accounting discrepancy that Lin missed.

Chapter 22:
She warns him that the discrepancy may expose a hidden supplier relationship.

Chapter 23:
Her information causes Lin to abandon a planned acquisition.

But the same discrepancy could have been discovered by the accountant who already prepares the financial reports.

Fault target: a character appears useful only because the author assigned an exclusive observation to her; delete-character test must examine whether that function is genuinely unique or artificially allocated.

## H09 — Partial Staleness

Character Psychology V1.4 changes only one field:
“Lin's fear of debt” -> “Lin's fear of losing control.”

The outline is unchanged.

Chapter Handoff 31 depends explicitly on “fear of debt” for a decision.

Chapter Handoff 32 depends only on Lin's general desire for growth.

Only Handoff 31 is stale.

Fault target: dependency analysis must invalidate affected artifacts, not the entire project indiscriminately and not nothing.

## H10 — Legitimate Override vs QA_PASS

Auditor identifies a LOW severity stylistic inconsistency that does not break causality.

Author keeps the wording unchanged.

System records:
VERDICT: QA_PASS

Separately, another chapter has a HIGH causality defect that the author knowingly accepts and records with:
Overridden Finding, Author Decision, Reason, Accepted Risk, Affected Scope.

System records:
VERDICT: QA_OVERRIDE

Fault target: system must distinguish legitimate PASS from accepted structural risk.

## H11 — Knowledge Through Inference

Chapter 29:
Lin sees that a competitor suddenly increased warehouse orders.

He concludes:
“他们现金流出了问题。”

The story has established:
- competitor recently lost a major client;
- warehouse orders increased sharply;
- supplier payment terms became shorter.

No character explicitly tells Lin the competitor has cash-flow trouble.

Fault target: do not incorrectly reject valid inference simply because no one stated the conclusion explicitly.

## H12 — Character Choice With Hidden Alternative

Chapter 35:
Lin refuses an extremely profitable expansion because it would require giving Zhao Ming access to internal financial data.

The chapter presents this as a moral choice.

Earlier chapters establish that Lin could instead:
- form a legally separate subsidiary;
- provide audited summary data rather than internal raw data;
- negotiate a restricted data room.

None of these alternatives are considered.

Fault target: turning-point audit must examine alternatives, not merely whether the chosen action is psychologically plausible.

## H13 — Coincidence With Prepared Causality

A supplier unexpectedly calls Lin after a crisis.

At first glance this looks like author rescue.

Earlier, however:
- Lin had previously helped the supplier recover a delayed payment;
- the supplier's owner mentioned needing a reliable expansion partner;
- Lin had left his contact information;
- the supplier had been monitoring the same market.

Fault target: do not reject a coincidence merely because it is convenient; distinguish coincidence as trigger from coincidence as unsupported causal chain.

## H14 — Foreshadow With Multiple Interpretations

Chapter 9:
Lin notices that his partner always asks for invoices to be printed twice.

Possible interpretations:
- accounting habit;
- audit preparation;
- fraud concealment.

Chapter 28 reveals the partner was secretly copying invoices.

The earlier clue supports the payoff, but it was not uniquely predictive.

Fault target: valid foreshadowing may have a reasonable false interpretation and should not be rejected merely because it was ambiguous.

## H15 — Cross-Chapter State Drift

Chapter 17:
Lin gives his only company car to the sales manager.

Chapter 18:
He drives the same car to meet a bank officer.

No transfer/recovery event is shown.

The car is not central to the plot.

Fault target: continuity audit must catch state drift even when the object has low narrative importance.
