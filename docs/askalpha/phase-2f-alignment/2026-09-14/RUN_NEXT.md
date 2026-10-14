# askalpha / AskTD — Phase 2F architecture alignment and continuation

**Revision:** 1.1 — connected-repository continuation after documentation alignment, 14 September 2026.

**Carry-in checkpoint:** `ASKALPHA_20260914_DOCUMENT_ALIGNMENT_COMPLETE_REPOSITORY_ALIGNMENT_BLOCKED`.

## 0. Execute the remaining repository work

Run this task in the existing AskTD development session on `SSH: kmai-13`, or its verified successor environment already used for this repository. This package contains documentation, not an application checkout. Do not create a replacement project from it.

The previous ChatGPT session completed the document-level reconciliation, updated the impact report and handoff, and preserved the original assessment. It had no application checkout; its configured repository access returned 404. That was a limitation of that session, not proof of a problem in your current environment. Do not repeat that access test elsewhere or recreate the documentation investigation if the provided records remain valid.

Use `askalpha_Phase_2F_Repository_Continuation_2026-09-14.zip`. Inspect archive entries and extract them into a fresh documentation staging directory outside the application checkout; reject traversal paths or link entries. All package-relative paths below are under its `askalpha/` directory. The file you are reading is also supplied as `RUN_NEXT.md`.

Read `README.md`, `AskTD_LATEST.md`, the five `current/` references listed below, and the complete `ARCHITECTURE_DELTA_IMPACT_REPORT.md`. Its operative September 14 section supersedes conflicting September 1 planning text, which is preserved as history. The handoff is v0.3. Logical `/AskTD/...` and ChatGPT sandbox paths inside documents are provenance/navigation labels, not paths assumed to exist in your environment. Use the actual extracted package files.

Your concrete deliverables are the **existing repository's** updated impact report, task/phase plan, relevant ADR forward references and continuation notes, plus any necessary small correction within the actual current task's established authority. A new external report alone does not substitute for those repository edits when they are accessible and authorized. If a report is intentionally maintained outside the repository by an applicable instruction, preserve that location and update the repository's reference to it.

Before edits, locate applicable `AGENTS.md` and other repository instructions. Record repository top level, origin, branch, HEAD/tree, tracked/staged/untracked state, current task, existing authorization and acceptance evidence. Inventory user changes without printing secrets. Keep unrelated changes intact; a dirty tree is not by itself a reason to reset or abort. If an active operation owns an overlapping file, coordinate at its next safe boundary without terminating it or writing concurrently. Stop only the genuinely conflicting part of this task.

Locate the already-performed source review and full LLM inventory. Preserve stable call IDs, their reviewed revision and valid tests. Review subsequent changes and unresolved boundaries only. Do not infer that missing evidence here means the task never ran, or that a historical SHA is today's required HEAD. Record PR #18/merge/activation evidence only to resolve an actual continuation question; do not reopen accepted gates or impose a historical merge strategy.

Update the live impact matrix first, then the owning repository references. Map all D01–D18 to exact existing paths/symbols, source revision, current behavior, gap/status, owning task, required change and acceptance/dependency evidence. Resolve the packaged report's missing locations from the source; never turn conceptual contract names into claimed existing files. Preserve distinctions between source defaults, test overrides and observed runtime settings.

Proceed with routine inspection, documentation edits and justified corrections already within the user's granted scope. Do not ask for duplicate authorization. If code authority cannot be established, complete the documentation and propose that code slice without implementing it. This continuation adds no deployment, feature activation, data access, framework migration, permission synchronization or external-communication authority.

Continue the active AskTD engineering session. This is an update to the current work, not a project restart.

All responses and engineering artifacts in this development environment must be in English, including plans, reports, prompts, comments and tests. This overrides older reference text asking the development agent to speak Persian.

Preserve the current checkout, user changes, completed work and previously granted authority. Do not reset to a historical commit, create a replacement project or interrupt an active operation with conflicting edits. Reconcile this update before the next affected implementation step.

## 1. Read the updated references completely

The continuation package contains all original `askalpha_Architecture_Update_2026-09-14.zip` references, the updated handoff/latest pointer and the separately updated impact report. Use the staged files as described in Section 0. The original architecture ZIP remains an unchanged historical input; you do not need a separate download of it. Do not assume that a ChatGPT Library path or sandbox link is accessible from your environment.

Read the archive's `README.md` and `AskTD_LATEST.md`, then these files under `current/`:

1. `askalpha_Solution_Architecture_2026-09-14.md`
2. `AskTD_01_Deposits_MVP_Scope_and_Acceptance_2026-09-10.md`
3. `AskTD_02_Authorization_Decision_Record_2026-09-10.md`
4. `askalpha_LLM_Usage_and_MRM_2026-09-14.md`
5. `AskTD_03_Architecture_Delta_and_Agent_Handoff_2026-09-10.md`

The three September 10 filenames retain their creation date; their latest revision is September 14. Read the repository's applicable `AGENTS.md`, current task, phase plan, relevant ADRs and existing architecture-impact/LLM-inventory reports as well.

Treat August records as historical evidence, not instructions to restart completed phases. If a required attachment is unavailable, identify the exact missing file and complete the source/plan review that remains possible. Do not invent its contents or make dependent changes from assumptions.

## 2. Establish the actual current state

Record the repository, branch, HEAD, dirty state, active phase/subphase and existing acceptance evidence. Distinguish source defaults, test configurations and observed runtime settings.

The supplied review previously referenced `TD-Enterprise/kmai-td-genie`, branch `phase2/recipe-lifecycle-classification`, commit `6e37281e61a782ffbe8c8675346144567406dabe`. It reported 2F.1 implementation and push, without establishing merge or activation. This is a historical checkpoint, not a reset target or today's required HEAD. Preserve any later progress.

The prior source review and LLM inventory were already performed and reported. Locate and update those records incrementally. Verify their actual committed/local state; do not repeat the entire investigation merely because an older document calls it future work.

## 3. Apply these architecture clarifications

**A. Bounded Deposits MVP**

Start with approved Deposits questions, data objects and personas. Deliver governed read-only answers, tables and basic approved charts. Exact business scope and acceptance ownership remain open. One engineering dataset, one recipe and 199 evidenced fields do not establish an approved Deposits inventory. Autonomous actions and advanced what-if analysis remain future work.

**B. Authorization and source identity**

Retain application enforcement of end-user scope and Managed Identity/MSI for source access. Do not implement cross-provider user-ACL synchronization. The authoritative enterprise entitlement mechanism remains open; an existing application mapping does not resolve that ownership question.

Enforce scope before protected metadata discovery and execution, and when reusing history, suggestions, cached results or outputs. Unresolved access must fail closed. An authorized user whose application MSI cannot access the source receives a safe service-access error with a correlation reference, without privilege-expanding fallback.

Inspect the existing SQL AST/object-scope enforcement before proposing another implementation. Verify missing-scope and `not_resolved` behavior on the enabled protected path. Default-off flags are not evidence of deployed enforcement.

**C. Semantic ownership and recipe compatibility**

The Registry is the application's single versioned runtime semantic representation. Business/data owners retain authority over meaning; Collibra coverage and interfaces require confirmation. Unity Catalog provides applicable technical metadata and governance. Do not assume enterprise metadata synchronization already exists.

Templates and suggestions reference governed IDs and versions without duplicating KPI definitions. Recipe compatibility remains dependency-scoped: an unrelated global Registry change must not invalidate a recipe. A cache miss is not a lifecycle failure.

**D. Reported implementation versus target diagrams**

The report identifies AG2/autogen; the drawings show Bottlenose/LangGraph. Record the discrepancy without migrating frameworks. The working MVP returns complete responses; Redis streaming is not an implicit requirement.

Keep the UI behind protected backend APIs. Separate UC governance, workspace context, query-serving compute and physical data. Resolve the approved interim/target route, freshness, workload identity and latency/concurrency requirements. Do not silently hard-code SQL Warehouse or serverless availability.

AI Search, document crawling/chunking VMs, SharePoint, extra channels and future model providers are conditional components. Their appearance in a diagram does not add them to the active 2F scope.

**E. Cache and presentation**

Retain the planned early authorized request/template lookup before avoidable LLM work. Its key must use pre-plan information; it cannot require `semantic_plan_hash`. Keep recipe reuse, result reuse, final-response reuse and physical data materialization distinct. Cache bounded eligible objects, not the approximately 5 TB source dataset. Do not implement a new cache platform solely for this alignment.

The target prefers deterministic approved templates and explicit formatting rules. Reported current paths still use LLM report generation. Treat the difference as an implementation/qualification gap, not a completed control. Result-bearing model paths need purpose-specific payload eligibility and analytical-fidelity checks. Qualify any retained generated-code visualization path; do not assume existing restrictions prove complete isolation.

**F. LLM usage, context and telemetry**

Preserve the reported distinction: 16 potential invocation paths across two Azure OpenAI application integration paths, not 16 calls per question. Actual calls depend on routing, recipes, clarification, retries and review.

Keep separate work items for safe database-error payloads, approved result transmission, current-turn history authorization, untrusted-input handling, output/schema validation and durable audit. Prompt delimiters alone are not redaction or authorization. Verify both application integration paths against the enterprise gateway contract; SDK usage alone does not establish routing.

The previously proposed 2F.1a error-hardening slice is not automatically completed or authorized by this notice. If it is already authorized and still needed, use structured permitted diagnostics and test the actual outbound payload boundary with synthetic fixtures across both model helpers. Do not claim that this one fix closes all model-use gaps.

AIOBS, ADLS trace transport, OTel/LangSmith and the enterprise library are target contracts requiring qualification. Record observable events, safe reason codes, correlation and permitted content; do not promise hidden model reasoning or default raw-payload retention.

**G. Acceptance and ownership**

Bring minimum authorization, payload, business evaluation, trace and serving evidence into pilot acceptance. Clarification must handle ambiguous questions across enabled routes, including fast paths. Bounded multi-turn scope still requires an explicit product decision and current-access checks. Engineering golden tests do not replace Deposits SME-approved calculations and expected answers.

Preserve the five open SpruceX dependencies: enterprise entitlements, metadata integration, governed data access, query-serving performance, and runtime identity/connectivity. PIA/DAC activities are progressing, not automatically complete. ABP approval is reported; ARB and production readiness are separate. Business/model ownership, application/run ownership and MRM acceptance of the proposed question-to-answer assessment boundary remain open.

## 4. Update the actual phase plan

Map D01-D18 from the updated handoff to current code, contracts and owning tasks. Preserve the detailed 2F sequence: lifecycle classification; approval/reapproval policy; certified semantics; templates; relationship impact; relevant hardening.

The reported 2F.1 classifier is trace-only; the existing recipe gate controls execution. Do not silently turn classification into a new execution gate or invent `REVIEW_REQUIRED` warn/block policy. If later authorized work already changed this, document that evidence.

Resolve conflicting older 2F/2G labels with forward references rather than renumbering history. Collibra, Genie and on-premises discovery can inform later integration; they are not default dependencies for completing the active slice. Do not defer basic pilot access, payload, evaluation and trace proof simply because broader hardening is labelled Phase 4–6.

## 5. Complete the alignment work

First update the existing impact report with: delta; current behavior and exact file/symbol evidence; gap or already-satisfied finding; owning phase/task; required change; acceptance evidence; external owner/dependency where applicable.

Then update the repository's task/roadmap/ADR references and continuation notes. Apply small, necessary compatibility corrections within the currently authorized task after recording their impact. Preserve existing behavior outside that scope. Keep broader migrations, integrations and policy changes as explicit proposals or owner decisions. An external dependency should block only the affected work, not unrelated progress.

Do not stop at acknowledging the documents. Complete the review and planning updates, perform any justified corrections within existing authority, and leave a concrete next implementation step.

Reuse valid baseline evidence. Run focused checks for changed behavior; broaden testing only for a concrete remaining risk or an existing required gate. Documentation-only changes do not require rebuilding the application or regenerating the full test output. Use synthetic fixtures and mocked model boundaries; do not invoke live models, query real data or alter deployment settings for this document-alignment task.

Return one English completion report containing:

- Actual current checkpoint and references read.
- Updated impact/phase-plan file paths.
- Changes completed, with verification evidence.
- Remaining target-only capabilities and external decisions.
- The next smallest implementation slice, its acceptance criteria and dependencies.

Clearly distinguish completed changes, proposals, reported source findings and verified runtime evidence. Preserve previous user authorizations without assuming this notice approves new deployments, feature activation, framework migration or additional data access.

## 6. Conditional 2F.1a completion criteria

The first candidate code slice remains structured database-error payload hardening. Establish whether it is already authorized, unfinished and still required. If later work already completed it, reuse the valid evidence and continue the actual owning task; do not reopen it merely to satisfy this prompt.

If it is within established authority and remains necessary:

1. Identify actual callers and both shared model helpers through the original inventory. Preserve their call IDs. Include in-scope correction, retry and review routes where diagnostic content may be forwarded.
2. Construct structured permitted diagnostics from trusted classification. Do not serialize arbitrary exception text, nested provider objects, connection strings, credentials, raw paths or sensitive SQL literals. An unknown diagnostic classification must yield a safe bounded outcome, not a guessed repair instruction.
3. Use synthetic exceptions with distinct sentinel secrets, sensitive values, paths and nested fields. Mock the actual outbound boundary at both model integrations and inspect complete constructed request payloads. Prove forbidden values are absent through every affected path. A sanitizer unit test or regex replacement alone is insufficient.
4. Verify permitted diagnostic categories remain useful for bounded correction or safe stop. Preserve authorization/AST checks, retry limits, correlation and safe user output. Do not add broader-principal, unrestricted-object or alternate-provider fallback.
5. Run focused changed-behavior tests and required existing gates. If broad tests are necessary, state the concrete remaining risk. Keep side-effecting tests/builds out of the live worktree when repository instructions require isolation; preserve any ignored logs/coverage state. Do not regenerate baselines simply to turn a test green.
6. Report exact files/symbols changed, authority, revision and observed test outcomes. Keep result transmission, history reauthorization, untrusted-input handling, formatting/fidelity, schema/renderer validation and durable telemetry as separate gaps. Do not label this one fix as closing all LLM controls or pilot readiness.

If this code slice is not yet authorized, its reviewable proposal must identify the proposed diagnostic schema, exact caller/helper/test locations, compatibility boundary, acceptance tests and the specific decision still required. Do not request live data/model access for synthetic boundary tests.

## 7. Finish and hand back evidence

Complete all unblocked work in the current scope. Review the final diff against the captured user state, check documentation references, and record focused verification results. Do not stage or publish unrelated files. This task requests local alignment and applicable bounded corrections, not PR creation, merge, branch deletion or remote publication.

Return one English completion report with:

- Actual repository/branch/HEAD and active task; references read and source-review baseline reused.
- Exact repository impact, phase-plan, ADR and continuation paths updated, distinguishing them from staging copies.
- D01–D18 disposition and any earlier-phase compatibility correction, with precise evidence.
- Implemented changes, documentation-only changes, proposals, target-only work, and runtime evidence kept separate.
- Verification commands/outcomes and any existing failures; no claimed test run from historical counts.
- Remaining external decisions, affecting only their dependent work.
- Status of 2F.1a: completed now, already completed/reused, proposed without authority, or not applicable; include evidence.
- The next smallest task, acceptance criteria and dependencies.

End with one accurate token:

- `PHASE_2F_REPOSITORY_ALIGNMENT_COMPLETE` — requested repository documentation alignment and all presently authorized applicable corrections completed; this is not pilot/production acceptance.
- `PHASE_2F_REPOSITORY_ALIGNMENT_PARTIAL` — useful changes completed, with exact affected blockers or owner decisions listed.
- `PHASE_2F_REPOSITORY_ALIGNMENT_BLOCKED_ACCESS` — the actual repository cannot be accessed; identify the unavailable location and do not create a replacement project or claim repository edits.
