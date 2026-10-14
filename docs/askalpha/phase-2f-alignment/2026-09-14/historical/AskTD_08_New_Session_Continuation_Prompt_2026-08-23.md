# askAlpha / KMAI — New ChatGPT Session Continuation Prompt

> **Historical checkpoint — notice added 14 September 2026.** The record below preserves its original August evidence and phase/authorization wording. It is not today's operative status or next-task instruction. Read `/AskTD/AskTD_LATEST.md` and the updated Leadership Alignment package first. The newer supplied report describes 2F.1 implementation on a development branch; merge, activation and current HEAD require verification. Preserve later user authorizations. The source-review inventory and diagram reconciliation are now recorded in the September package. Historical SHA values and tests below have not been changed or rerun.

Copy the block below into a new ChatGPT session.

```text
I want to continue development of the existing AskTD / askAlpha / KMAI project. This is a continuation of a long-running project. Do not redesign it or start coding immediately.

1. Search my ChatGPT Library for `/AskTD/Handoff 2026-08-23/` and read these files completely in order:

- AskTD_00_Library_Index_2026-08-23.md
- AskTD_01_Authoritative_Current_State_2026-08-23.md
- AskTD_02_Implementation_Phase_Status_2026-08-23.md
- AskTD_03_Architecture_and_Roadmap_Update_2026-08-23.md
- AskTD_04_Assumption_Decision_Log_2026-08-23.md
- AskTD_05_Management_Roadmap_and_Feature_Map_2026-08-23.md
- AskTD_06_Session_Continuation_Handoff_2026-08-23.md
- AskTD_09_Phase_2F_Scope_Discovery_2026-08-26.md

The latest 2026-08-26 updates in this package are authoritative where they conflict with earlier status or roadmap statements. `AskTD_07_Phase_2E_Bounded_Implementation_Prompt_2026-08-23.md` is historical and must not be executed again.

2. Reverify the live private repository before proposing any mutation:

Repository: `TD-Enterprise/kmai-td-genie`

Expected evidence to verify, not assume:

- current `main`: `f283f01b6d615f9fa00debcef959d9c5c86a3224`
- PR #17: closed/merged, accepted head `0430613e6a9f1680338d8fc099e7960e5d46cac2`, 12 files, `+1760/-18`
- PR #16 merge: `409fed3fb98fc87547a7d05a68292fc28c3c1e7c`
- PR #15 merge: `9db7e6b86c596bdf613f3180c2a1c927625233a1`
- workflow `32974122120`: success
- downstream workflow `32975418654`: success

3. Reconstruct the current phase state:

- 2A/2B accepted;
- 2C closed/merged/post-merge verified;
- 2C.5, 2D, and 2E merged;
- 2E independently reverified with successful workflows;
- 2F scope discovery complete, implementation not authorized.

4. Exact continuation point:

Phase 2F — Recipe Lifecycle, Certified Semantics, Output Templates, and Evidence-Gated Relationship Impact.

The first proposed implementation slice must be limited to a pure deterministic lifecycle evaluator using existing Phase 2E evidence. It should classify `VALID`, `REVIEW_REQUIRED`, `BROKEN`, and `NOT_APPROVED`, produce explicit reason evidence, remain provider-neutral, fail closed where required, and preserve Phase 2E behavior behind a feature flag.

Do not implement KPI/glossary authoring, templates, relationships, additional recipes, Databricks, Genie, Redis, Graph DB, providers, cross-source, frontend, deployment, or infrastructure in the first slice.

5. Open owner decisions must remain explicit:

- whether `REVIEW_REQUIRED` warns or blocks;
- approval owner/evidence/expiry/reapproval rules;
- D4-D6 metadata and relationship dependencies;
- product-group namespace reconciliation;
- strict-mode runtime activation.

6. First response must contain only:

- documents loaded;
- live repository verification and drift;
- current status in at most 10 bullets;
- exact recommended first Phase 2F slice;
- open decisions and blockers;
- one bounded implementation plan or prompt for approval.

Do not create a branch, worktree, commit, push, PR, or code change until I explicitly approve the exact Phase 2F slice.
```
