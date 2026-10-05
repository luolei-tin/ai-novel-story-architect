# V1.0 Blind Audit Protocol R1.0

The auditor must receive only:
1. the baseline story state;
2. one faulty chapter/case;
3. the applicable project rules.

The expected verdict matrix must remain hidden from the auditor during execution.

For every case, require:
- VERDICT
- EVIDENCE
- BROKEN CHAIN
- WHY IT FAILS
- MINIMUM REPAIR
- AFFECTED SCOPE
- VERSION / STATE BASIS

Scoring:
A. Verdict accuracy
B. Evidence sufficiency
C. Causal-chain reconstruction
D. Minimum-repair quality
E. Dependency invalidation accuracy
F. State/knowledge continuity accuracy

Automatic test failure:
- PASS on a case expected to be REJECT;
- QA_PASS used where QA_OVERRIDE is required;
- conclusion without evidence;
- “character would probably...” used instead of established psychology/state;
- repair introduces a new unsupported rule;
- old PASS reused after an upstream invalidation;
- future knowledge accepted without acquisition path.

Important:
A correct verdict with insufficient evidence is not a full PASS for the validation system. The purpose of this blind test is reproducibility, not merely getting the label right.
