# AskAlpha / KMAI — Architecture Delta Impact Report

## Operative update — 14 September 2026

**Status:** `DOCUMENT_ALIGNMENT_COMPLETE_REPOSITORY_ALIGNMENT_BLOCKED`  
**Scope:** Incremental reconciliation of the September 1 report with the September 14 reference package and current user instructions. No source, deployment or runtime verification is claimed.  
**Language:** All development-environment responses, plans, reports, prompts, comments and tests are English. This overrides conflicting older continuation text.

This update governs planning where it conflicts with the historical assessment preserved below. It does not revoke previously granted task authority, restart completed phases, prove today's checkout, or authorize new runtime work. The original report is retained verbatim below the historical marker. Its former final token is historical, not the verdict of this update.

### U1. Actual available checkpoint and access boundary

| Item | Observation on 14 September | Consequence |
| --- | --- | --- |
| Execution environment | `/workspace/scratch/e7d903170044`; not the permanent `SSH: kmai-13` environment | No remote development session or active operation was controlled. |
| Local checkout | `git rev-parse --show-toplevel` returned exit 128, not a Git repository; the workspace initially contained no files | Actual branch, HEAD, index, dirty state, active task and accepted progress are unavailable, not clean or unchanged attestations. |
| Previously documented locations | `/home/tag5916/projects/kmai-td-genie`, `/home/tag5916/projects/kmai-td-genie-worktrees`, and `/app1/tag5916/projects/kmai-td-genie-worktrees` are absent here | No replacement checkout was created. No SSH credential or unrelated workspace search was attempted. |
| Configured repository access | A read-only request for `TD-Enterprise/kmai-td-genie` returned GitHub API 404 | Source/PR review stopped at the access boundary. This does not prove repository deletion or PR status. |
| Historical checkpoint | Package reports branch `phase2/recipe-lifecycle-classification`, head `6e37281e61a782ffbe8c8675346144567406dabe`, implemented/pushed 2F.1 | Not a reset target, today's required HEAD, proof of merge, or proof of activation. Preserve any later work. |
| Existing source review | Reported as already performed in the current handoff | Do not repeat the entire audit. The original repository-level review and its committed/local state remain unavailable here. |
| LLM inventory | Fully read the current reported-summary reference; 16 potential invocation paths across two application integration paths | Full call IDs, exact callers/helpers and their publication state were not recovered. Nine purpose categories must not be substituted for those 16 paths. |
| Runtime | No enabled flags, deployment, actual model call counts, gateway traffic, source query or trace ingestion was observed | Source defaults, synthetic test settings and deployed settings remain separate evidence classes. |

The requested archive was recovered and extracted into a separate documentation staging directory without overwriting application files. It is available, not missing. Missing inputs are the live checkout and its applicable `AGENTS.md`/task/phase plan/ADRs, the original full source review/call-site inventory, and current authorization/acceptance records. Exact names of those unavailable repository records cannot be invented.

### U2. References read completely

All paths below are relative to the extracted archive root `askalpha/` unless stated otherwise:

1. `README.md`.
2. `AskTD_LATEST.md`.
3. `current/askalpha_Solution_Architecture_2026-09-14.md` — architecture v1.0.
4. `current/AskTD_01_Deposits_MVP_Scope_and_Acceptance_2026-09-10.md` — revised September 14, v0.2; acceptance A01–A10.
5. `current/AskTD_02_Authorization_Decision_Record_2026-09-10.md` — revised September 14, v0.2; AUTH-01–AUTH-07.
6. `current/askalpha_LLM_Usage_and_MRM_2026-09-14.md` — v1.0; purposes U01–U09 and gaps L01–L08.
7. `current/AskTD_03_Architecture_Delta_and_Agent_Handoff_2026-09-10.md` — revised September 14, v0.2; D01–D18, detailed phases and G01–G11.
8. `historical/AskTD_09_Phase_2F_Scope_Discovery_2026-08-26.md` — historical ordering and original D4–D6 prerequisites, not present-day authority.
9. The existing September 1 `ARCHITECTURE_DELTA_IMPACT_REPORT.md`, recovered and updated in place.

The standalone handoff and latest-reference files were compared byte-for-byte with their archive copies before editing; both comparisons passed. The original engineering call-site inventory is not included in these summaries. No transcript, email, approval system or source drawing referenced by these documents is claimed as independently inspected in this run.

### U3. Corrections to the September 1 conclusions

| Older wording or sequencing | Operative correction | Classification |
| --- | --- | --- |
| Registry is the sole authority for business semantics | Registry is the single versioned **application runtime representation**. Business/data owners approve meaning. Collibra coverage/interfaces and UC technical governance require confirmation; no enterprise synchronization is established. | Documentation correction; 2F.3/2F.4 contract impact |
| AI formatting is not current | The preferred deterministic route is a target. Relevant current paths are **reported** to generate reports/summaries with an LLM. Their payload eligibility, deterministic routing and fidelity are qualification gaps, not delivered controls. | Reported implementation gap; 2F.4 and pilot gates |
| Authorization mapping means ownership is resolved | Application enforcement and MSI remain the working direction; enterprise grant authority, mappings, revocation policy and deployed enforcement remain open. No ACL synchronization. | Documentation correction; AUTH gates |
| Safe provider errors can wait for future integration | Existing raw-error-to-model paths are reported. Keep source-access error handling and model-bound diagnostic payloads distinct; qualify the enabled protected path before pilot use. | Bounded proposed gap; D03/D18 |
| SQL physical-object checks remain wholly future | Existing SQL AST/object-scope enforcement is reported. Inspect/reuse it before proposing another implementation, especially missing-scope and `not_resolved` behavior. | Incremental source verification needed |
| Hardening/evaluation/serving proof is future-only | Full Phases 4–6 remain planned, but minimum access, payload, SME evaluation, trace and serving proof are required for pilot acceptance. | Plan correction; A02–A10 |
| A full new live-source inventory must be generated | Recover the already performed review and stable 16-path inventory; validate only subsequent deltas and unresolved boundaries. | Process correction |
| Exact historical main/head/merge shape is today's required gate | Establish the actual current checkout, branch policy and accepted chain without resetting or assuming PR #18's status. Historical SHAs are evidence anchors only. | Process correction |

No source-level incompatibility is newly proven here. The reported 2F.1 design remains compatible in principle: deterministic, dependency-scoped, provider-neutral and trace-only. This is not a fresh verification of the current code. The existing recipe gate owns execution; this update adds no `REVIEW_REQUIRED` warn/block policy.

### U4. D01–D18 impact and ownership matrix

Evidence anchors below refer to the fully read package. Source paths/symbols are **reported/historical anchors**, not freshly verified files. When a helper, test or contract name is missing, the row explicitly requires resolution from the existing inventory. Proposed work labels below organize follow-up; they are not newly created repository tasks or granted implementation authority.

| Delta | Current behavior / evidence anchor | Gap or satisfied decision | Owning work | Required change | Acceptance evidence | External dependency |
| --- | --- | --- | --- | --- | --- | --- |
| D01 Deposits MVP | Scope record: one engineering dataset/recipe and 199 fields do not establish Deposits approval; no current dataset-config path available | Working bounded scope; exact business inventory open | Pilot scope / 2F.3 / additional recipes in 2F.6 | Map approved questions, objects, personas and basic outputs; exclude actions/advanced what-if | A01/A04: owner-approved inventory, calculations, expected answers and exclusions | Deposits owner, Product, SMEs; G08 |
| D02 Semantic ownership | Reported `MetadataRegistryService` / `RegistrySnapshot`; historical `src/backend/app/recipes/approved_recipes.py` | Compatible runtime seam; enterprise provenance/intake contract open | 2F.3; template refs in 2F.4 | Preserve owner/source ID, object and definition versions, publication provenance; no duplicated KPIs | References resolve to governed versions; unauthorized meaning/grants cannot be invented; unrelated dependency changes preserve recipe compatibility | Business/Data Governance; G02 |
| D03 Authorization/MSI | Authorization record reports `dbo.auth_authorization_mappings`, 300-second access cache and existing AST scope checks; historical `EffectivePermissions` / `test/test_authz_no_access_guard.py` | No-sync design retained; source defaults are not enabled-path proof | Existing authorization owner task; relevant 2F hardening | Inspect actual resolver/AST callers, missing scope and `not_resolved`; enforce access before metadata/execution/reuse; safe MSI failure without broader fallback | AUTH-01–AUTH-07, A02/A03: synthetic enabled-path negatives, zero forbidden effects, safe correlation; runtime qualification separately | G01/G03/G05; IAM/Data Owner/Platform |
| D04 Data route/compute | Architecture component table distinguishes UC, workspace, compute and physical data; no endpoint config inspected | Interim/target route and performance open | Pilot serving gate; Phase 3 adapter work | Record approved objects, query vs copy, treatment, freshness, identity and workload envelope; no assumed SQL Warehouse/serverless | A03/A09: approved route and later authorized warm/cold, concurrency and deny evidence | G03/G04/G05 |
| D05 Clarification | LLM U02 and scope A05 report clarification paths; exact fast-path symbols unavailable | Cross-route coverage not proven | Current request-routing owner; pilot acceptance | Map existing enabled routes; add bounded synthetic ambiguous/unsupported cases including recipe/template fast paths | Missing KPI/period/grain/scope produces clarification or safe unsupported result before unsafe execution | Product/QA; A05/G08 |
| D06 Multi-turn scope | LLM L03 reports history reuse; storage/session/caller paths unavailable | Inclusion in pilot open; current-turn authorization required if enabled | History/context owner; relevant pilot hardening | Define included follow-up depth and revalidate current scope, session ownership, filters, periods and dependencies | Revoked-access and cross-user/session fixtures; no previously permitted data leaks into current outbound context | Product/IAM/Privacy; G01 |
| D07 Lifecycle/recipe reuse | Historical `src/backend/app/recipes/lifecycle.py`, `approval_evidence.py`, `orchestrator.py`, `test/test_recipe_lifecycle.py`; reported `evaluate_recipe_lifecycle` | Reported trace-only classification compatible; execution policy not newly authorized | Preserve 2F.1; approval/reapproval in 2F.2 | Retain dependency-scoped identity and existing execution gate; do not turn classifier into a gate | Reuse valid baseline tests; if touched, check unrelated dependency change, reasons, flag-off behavior and execution-boundary preservation | Product/Governance policy owner |
| D08 Cache/reuse | Historical snapshot cache and separately reported permission cache; early/result cache still planned | Not all caching is absent; analytical reuse not delivered | 2F.4 reference compatibility; later bounded cache task | Separate recipe/result/final-response reuse and materialization; early key has no plan hash; bounded eligible payloads; platform TBD | Pre-plan key constructible without LLM, current-scope isolation and freshness; cache miss does not change lifecycle | Freshness/policy owner; platform choice open |
| D09 Formatting | LLM L02/L05/U07–U09 report result-bearing report/visualization/review paths; exact helper/caller paths missing | Deterministic target not implemented evidence; payload and fidelity gap | 2F.4; relevant 2F.6 checks; A07/A08 | Explicit template/policy routing, Registry refs, safe unsupported alternative; purpose-specific approved result context; qualify generated-code renderer | Numeric/KPI/scope/date/source/warning/qualifier invariants; boundary payload tests; malformed-output and renderer tests; SME review for meaning | Privacy/PIA, Product/SMEs; G08 |
| D10 Evaluation | Historical `test/test_recipe_lifecycle.py` and approved-recipe tests; reported 1076/3/87.01% are not SME acceptance | Existing engineering evidence reusable; Deposits benchmark open | Pilot A04/A05/A07 gate; broader Phase 5 retained | Version question/persona/as-of/calculation/expected-outcome suite; no identical-prose requirement | Approved reference calculations and materiality thresholds; affected regression results on exact revision | Deposits SMEs/QA; G08 |
| D11 Telemetry | LLM L07 reports no established durable AIOBS evidence; actual SDK/transport symbols unknown | Application trace does not prove durable enterprise ingestion | Pilot trace task; broader observability later | Specify permitted events/reasons/correlation and storage/retention; select supported enterprise contract or accepted interim arrangement | A08: observable event schema and synthetic redaction checks now; durable delivery/access/retention evidence before route acceptance | Enterprise observability owner; G09 |
| D12 Inventory/MRM | Current LLM reference: 16 potential paths, two integration paths, nine purpose groups; original stable call IDs unavailable here | Review already reported; deployment and MRM boundary open | Existing inventory task; pilot model-use governance | Preserve exact existing IDs/revision/callers/flags/retries/validators; update deltas only; question-to-answer boundary proposed | Static count not presented as calls/question; enabled routes separately reconciled; accountable owner and MRM disposition | Business/MRM; G06 |
| D13 Later integration | Architecture separates conditional Collibra interfaces, Genie evaluation and on-premises discovery; `DataSourceAdapter` historical seam | Provider neutrality retained as direction; integrations unproven | Phase 3/MVP 2; bounded earlier discovery only | Keep `DataGovernanceProvider` / `ExecutionProvider` concepts provider-neutral; no forced integration for active slice | No new provider imports/requirements from alignment; approve later integration scope independently | Data Governance/Platform/Architecture |
| D14 Operating ownership | Scope A09/A10 and handoff G07: registration/build/run/support/economics unresolved | Owners, thresholds and funding not established | Pilot operational acceptance; later scale work | Record confirmed registration, owner/support/disable procedure and workload-based measures | Named authorities and measured cost per correct accepted answer; no assumed estimates/SLAs | G04/G07/G10 |
| D15 Framework/gateway | LLM summary reports AG2/`autogen`; drawings name Bottlenose/LangGraph; direct-tool and agent-manager integration paths | Framework discrepancy and gateway qualification open | ADR forward reference; existing two-helper qualification task | Record discrepancy without migration; inspect configured routing/auth/deployment contract at both actual boundaries | Synthetic request construction validates agreed gateway contract; SDK presence not claimed as runtime routing proof | Architecture/gateway owner; G11 |
| D16 Optional services | Complete-response MVP direction; streaming, AI Search, crawling/chunking, SharePoint and extra channels conditional | Documentation can align without application rebuild | Architecture/roadmap only; later selected work | No Redis streaming or ingestion requirement by diagram inference; separate cache from delivery transport | Status/scope labels consistent; no new platform dependency or deployment | Product/platform owner if selected |
| D17 Protected API/storage | Architecture places UI behind API and separates metadata/results/traces/source; exact current frontend/API/storage symbols unavailable | Target boundary retained; actual paths not proven here | Existing API/storage owner; pilot A02/A08 | Map protected callers and store purposes/content/lifetimes; no browser direct source access or default raw-result retention | Endpoint scope checks, no client source credentials, bounded storage and permitted trace content tests | Security/Operations/data-use owner |
| D18 Model payload boundaries | LLM L01–L08; raw error, results/history/framing/output/trace gaps reported; both exact helper symbols must come from original inventory | Error hardening proposed, not authorized/completed by notice; other gaps stay separate | Proposed 2F.1a only if already authorized; separate payload/context/schema/trace tasks | Structured permitted diagnostics at actual outbound boundaries; synthetic sentinel tests across both helpers; do not conflate framing/redaction/access | Excluded error values absent from captured outbound payloads, safe correction/stop behavior retained; L02–L08 have independent closure evidence | Applicable Privacy/MRM/gateway decisions; authority for active code task |

### U5. Corrected phase sequence and pilot gates

These are updates to planning references, not edits to unavailable repository tasks. Preserve any later completed or authorized work discovered by the development agent.

| Existing slice | Operative plan / entry gate | Acceptance and bounded dependencies |
| --- | --- | --- |
| 2F.1 lifecycle | Preserve reported work; check only source deltas and existing acceptance record | Trace-only classifier, existing recipe execution gate, dependency-scoped compatibility. No new warning/block policy. |
| Proposed 2F.1a | First locate its task, authority, status and existing tests; skip if already completed and still valid | Structured permitted model diagnostics, both outbound boundaries, synthetic fixtures, no live model/source calls. This closes only its error-payload scope. |
| 2F.2 approval/reapproval | Resolve approval authority/evidence/expiry/renewal and `REVIEW_REQUIRED` policy | Product/Governance decisions, deterministic policy tests; no invented policy or automatic scope extension to all template publishing. |
| 2F.3 certified semantics | Governed definitions, enterprise provenance, runtime IDs/versions and ownership | Approved Deposits definitions; owner-approved manual intake can be proposed while G02 remains open. Do not require a live Collibra call per question. |
| 2F.4 templates | Versioned Registry references and suggestion provenance; separately bounded deterministic presentation work | Explicit routing and analytical fidelity, current-access checks, AI payload eligibility and safe no-template/no-approved-AI behavior; no autonomous rewrite. |
| 2F.5 relationship impact | Preserve historical D4–D6 prerequisites for field evidence, endpoints and naming | Do not confuse historical D4–D6 with September D04–D06. No guessed joins or graph database. |
| 2F.6 / relevant hardening | Reuse existing AST/object-scope checks; add only missing enabled-path evidence and scoped corrections | Authorization, payload, fidelity, ambiguity, dependency and additional-recipe regressions appropriate to approved pilot scope. |
| 2G controlled publication | Proposed/roadmap label; locate actual repository contract before relying on it | Separate semantic, recipe, template, formatting-policy and cache-compatibility assets; validate/rollback references. No silent KPI redefinition through templates. |
| Phase 3 and later | Preserve broader integration/evaluation/scale/self-service roadmap | Genie/on-premises/Collibra implementation conditional. Do not defer minimum pilot controls to Phases 4–6. |

Pilot readiness requires A01–A10: approved scope/owners; enabled-route access proof; governed source route; SME reference answers; clarification; correct lifecycle behavior; presentation fidelity/payload eligibility; accounted model/trace paths; serving measurements; scoped governance/operational authorization. No gate is declared passed by this document.

The five High SpruceX dependencies remain open: G01 enterprise entitlements; G02 metadata integration; G03 governed data access; G04 query-serving performance; G05 runtime identity/connectivity. Additional G06–G11 ownership, evaluation, telemetry, production and diagram questions stay as recorded. PIA/DAC are progressing, not complete; ABP approval is reported, not independently checked; ARB and production readiness are separate. Block only work dependent on an unresolved item: synthetic fixtures, documentation and permitted local contract work need not wait for live enterprise provisioning.

### U6. Next smallest implementation slice — conditional, not launched

**Immediate step in the connected development environment:** Reconcile the current task/checkout and already-performed source-review/inventory records, then incorporate this impact mapping into the actual repository plan and ADR forward references. Record exact existing file/symbol/test paths and distinguish source defaults from test overrides and observed runtime values. Preserve dirty/user changes; do not require resetting or a replacement worktree. An active conflicting operation must reach a safe boundary before edits.

**First bounded code candidate:** The previously proposed 2F.1a structured database-error payload hardening, only if the actual current task already authorizes it, it remains unfinished, and source evidence still shows the gap. If later work already resolved it, reuse the validated evidence and continue the actual task; do not reopen it from this report. If authority cannot be established, propose its scope and stop only those code edits.

Acceptance criteria for that candidate:

1. Identify all affected error callers through the preserved inventory, including the direct-tool and agent-manager model integration paths; keep their existing stable IDs.
2. Construct a typed/structured allowlist of permitted diagnostic categories from trusted classification, not wholesale exception serialization or ad hoc regex-only scrubbing. Unknown/unclassifiable failures produce a bounded safe-stop result.
3. Synthetic fixtures place unmistakable secret/token/path/connection-string, SQL-literal and sensitive-value sentinels in exception content and nested diagnostic data. Capture the final outbound request payload at both mocked model boundaries and prove prohibited values are absent, including any retry/review path in scope. Check entire constructed messages, not only a sanitization helper's return value.
4. Preserve sufficient approved diagnostic context for bounded correction or safe stop; retain existing query-safety, scope checks, retry limits and correlation. Do not expand privileges or pass raw provider details to user output.
5. Reuse valid baseline evidence. Run changed-behavior unit/boundary/integration tests and existing required gates; broaden only for a stated risk. No live model call, real data query, deployment change, flag activation or new framework/cache/provider.
6. Report exact changed source/test symbols, revision, authority record and measured test outcomes. L02 result transmission, L03 history authorization, L04 untrusted input, L05 routing/fidelity, L06 schema/renderer, L07 durable trace and L08 business/serving remain separate items.

Required inputs: current checkout/task/authority and full inventory; an agreed permitted-diagnostic schema or a proposal for its owner. Production access, enterprise trace provisioning and live model calls are not prerequisites for synthetic boundary tests. They remain requirements for affected pilot-route qualification.

### U7. Completed edits, verification and limits

Completed documentation edits:

- Updated this existing impact report incrementally; retained the original September 1 report byte-for-byte as historical evidence.
- Updated `AskTD_03_Architecture_Delta_and_Agent_Handoff_2026-09-10.md` to v0.3: English-only continuation, existing-inventory reuse wording, recovered-report reference and a scoped continuation checkpoint.
- Updated `AskTD_LATEST.md` to link the current impact/continuation checkpoint and distinguish these later standalone updates from the original ZIP snapshot.

Repository task, roadmap and ADR edits: **not performed** because the checkout is unavailable and the repository read is access-blocked. No application code correction is reported as complete. The LLM inventory summary was read and reused; its underlying 16-call-site record was not rewritten or fabricated.

Verification record:

- Archive listing and non-overwriting extraction completed, exit 0: 18 entries, 134,962 total uncompressed bytes.
- Archive SHA-256: `cd348fa4cf70c150a2bf4a45ae3dc854b8655eadb28063db8352ee7f05e25cf3`.
- Original impact-report SHA-256: `1f9c22519eadd9135b470317411f92bdfb129c54f879616b2a0aa41f3a029b11`.
- Required archive reads completed; standalone handoff/latest compared equal to archive preimages, exit 0.
- Source-environment diagnostics: `pwd` exit 0; initial scoped file search exit 1 (no matches); `git rev-parse` exit 128; documented-path existence check exit 2; configured GitHub repository GET returned 404. These are blockers, not successful identity/acceptance gates.
- Documentation validation checks the preserved original report hash, complete D01–D18 mapping, unchanged earlier phase table rows in the handoff, English-only operative instructions, required reference presence, and local cross-reference targets. No application build or test output was regenerated for documentation changes.

No repository, branch, index, PR, workflow, deployment, model endpoint, data source or active development operation was modified. This is a statement of actions taken here, not an attestation that an inaccessible remote worktree stayed byte-identical.

**Current disposition:** Documentation reconciliation is complete. Repository planning edits, exact current symbol mapping and any authorized code correction require continuation in the existing connected development checkout. No claim of pilot readiness, merge, activation or code-level compatibility verification is made.

`ASKALPHA_20260914_DOCUMENT_ALIGNMENT_COMPLETE_REPOSITORY_ALIGNMENT_BLOCKED`

---

## Historical September 1 report — preserved verbatim, not operative where superseded

# AskAlpha / KMAI — Architecture Delta Impact Report

**Date:** 2026-09-01  
**Scope:** Phase 2F compatibility review and Phase 2G+ planning impact  
**Mode:** Read-only impact assessment; no repository mutation authorized or performed

## 1. Executive verdict

The architecture updates are compatible with the accepted Phase 2A–2E foundation and with the evidenced Phase 2F.1 design. No completed phase needs to be restarted or redesigned.

The largest impact is forward-looking:

- Phase 2F.3 must make the Semantic Registry the sole authority for business semantics.
- Phase 2F.4 must introduce versioned template references, an explicit response-formatting stage, and deterministic routing.
- Phase 2F.6 must add output-consistency and regression protection.
- Phase 2G+ publishing must version and validate template definitions separately from semantic definitions.
- Early and post-plan cache contracts must be planned without selecting Redis or another platform.

No broad cross-phase code change is justified before a read-only live-source discovery confirms the current `main` state and repository-native extension points.

## 2. Evidence and confidence boundary

### Verified historical baseline

- Phase 2E / PR #17 was merged and independently reverified.
- Phase 2E established `MetadataRegistryService`, `RegistrySnapshot`, governed field evidence, entity-scoped fingerprints, recipe dependency references, reverse impact lookup, `EffectivePermissions`, and the `DataSourceAdapter` boundary.
- The historical current-main identity recorded on 2026-08-26 was `f283f01b6d615f9fa00debcef959d9c5c86a3224`.

### Newer Phase 2F.1 evidence available in this review

The latest supplied PR/review evidence identifies Phase 2F.1 / PR #18 with the following ten-file scope:

**Added**

1. `kmai-td-genie/src/backend/app/recipes/lifecycle.py`
2. `kmai-td-genie/src/backend/app/recipes/approval_evidence.py`
3. `kmai-td-genie/test/test_recipe_lifecycle.py`
4. `kmai-td-genie/docs/adr/0006-phase2f1-recipe-lifecycle-classification.md`

**Modified**

5. `kmai-td-genie/src/backend/app/orchestrator.py`
6. `kmai-td-genie/src/backend/app/recipes/approved_recipes.py`
7. `kmai-td-genie/test/test_approved_recipe_pilot.py`
8. `kmai-td-genie/test/test_authz_no_access_guard.py`
9. `kmai-td-genie/test/test_provider_abstraction_contracts.py`
10. `kmai-td-genie/docs/adr/README.md`

The supplied evidence reports a pure deterministic evaluator, immutable evidence/result contracts, provider separation, default-OFF classification-only behavior, and independent review approval. However, the live private repository could not be read from this environment: authenticated connector requests returned `404 Not Found`. Therefore PR #18 merge state and the current `main` SHA remain **REVERIFY_REQUIRED**, not assumed.

## 3. Architecture delta assessment

| Delta | Current compliance assessment | Required action | Classification |
|---|---|---|---|
| Early cache before semantic planning | No evidenced early request/template cache exists. Current cache baseline is only a bounded in-process metadata snapshot cache. | Define a provider-neutral early-cache contract and key model; keep implementation platform TBD. | Future-phase |
| Post-plan semantic/result cache | No evidenced semantic-plan or result-cache implementation exists. | Plan bounded eligible payloads, authorization scoping, TTL, freshness and invalidation. | Future-phase |
| Semantic Registry as semantic source of truth | Existing `MetadataRegistryService + RegistrySnapshot` is compatible as the governance seam. KPI, term, recipe and relationship ownership must be made explicit in later contracts. | Update architecture terminology; ensure templates contain references, not duplicated definitions. | Documentation + 2F.3/2F.4 |
| No user-ACL synchronization | Existing `EffectivePermissions` and governance-before-execution ordering are compatible. No ACL-sync implementation is evidenced. | Document AskAlpha entity authorization plus MSI source access; add safe provider-access error contract later. | Documentation + future integration |
| Explicit response-formatting stage | Not explicit in the accepted pipeline. Existing response primitives are not sufficient evidence of a formatting contract. | Add `Validated Result -> Formatting Route -> Final Business Output` to architecture; implement in 2F.4. | 2F.4 |
| Deterministic formatting routing | Not evidenced as an existing contract. | Introduce policy-owned routing; the LLM must not choose its own formatting route. | 2F.4 |
| AI formatting privacy boundary | Not current and not approved. | Keep behind an explicit interface and disabled unless PIA approval exists. | Conditional/Open |
| Versioned predefined template library | Not evidenced as implemented. | Add versioned template identity, governed references, provenance and controlled release metadata. | 2F.4 + 2G |
| No autonomous template rewriting | Compatible with the governed architecture; no runtime self-rewrite is evidenced. | Record analytics-to-curation-to-release workflow. | Documentation + 2G |
| Bounded cache for approximately 5 TB sources | Compatible: Core processes bounded metadata/results and provider-side compute handles large queries. | Add cache eligibility and result-size limits; never cache raw datasets. | Future Phase 6 |
| Provider-agnostic Core | `DataSourceAdapter` is established. Additional `DataGovernanceProvider` and `ExecutionProvider` shapes are planned, not verified as implemented. | Preserve seams; do not add provider-specific fields to canonical contracts. | Compatible + future |
| Genie as Future/Evaluation | Compatible with prior decision D9; no Genie dependency is evidenced. | Keep as a possible future `ExecutionProvider` only. | Future/Evaluation |
| Explicit Current/Planned/Conditional/Future labels | Existing documents contain stale statements and need refresh. | Add a capability-status matrix to authoritative documentation. | Documentation-only |

## 4. Phase 2F.1 compatibility

No architecture delta requires redesign of the lifecycle evaluator itself.

The evidenced Phase 2F.1 properties remain correct:

- pure, deterministic, immutable and provider-neutral evaluation;
- already-resolved approval and dependency evidence as inputs;
- no database, provider, cache, network, SQL, Databricks, Synapse or Genie access inside the evaluator;
- all applicable reason codes and affected references preserved;
- precedence `BROKEN > NOT_APPROVED > REVIEW_REQUIRED > VALID`;
- classification-only behavior that does not control runtime execution;
- feature flag default OFF and Phase 2E compatibility;
- orchestration resolves evidence before evaluator invocation.

### Local checks required before accepting full compatibility

1. Confirm `lifecycle.py` and `approval_evidence.py` import no cache, provider SDK, formatter or source-specific module.
2. Confirm `orchestrator.py` does not use lifecycle output to authorize, warn, block, route SQL or select a provider.
3. Confirm `approved_recipes.py` retains registry/dependency references without embedding future template business definitions.
4. Confirm tests still prove deny-all authorization occurs before lifecycle/provider activity.

These are verification gates, not reasons to alter the accepted 2F.1 design.

## 5. Exact Phase 2F areas affected

### Confirmed existing files requiring review, not presumptive modification

| File | Review question | Expected disposition |
|---|---|---|
| `src/backend/app/orchestrator.py` | Where will future early-cache lookup and explicit response formatting attach without bypassing authorization or query safety? | Review now; modify only in separately approved slices. |
| `src/backend/app/recipes/approved_recipes.py` | Are recipe IDs, versions and dependency refs reusable by future template references without duplicated semantics? | Likely compatible; verify. |
| `src/backend/app/recipes/lifecycle.py` | Is lifecycle independent of cache, formatting and providers? | No change expected. |
| `src/backend/app/recipes/approval_evidence.py` | Is approval evidence independent of template release and provider ACLs? | No change expected. |
| `test/test_recipe_lifecycle.py` | Does it remain focused on lifecycle rather than output formatting policy? | No change expected. |
| `test/test_authz_no_access_guard.py` | Does authorization still precede cache, metadata, lifecycle and provider work? | Extend in future cache/formatter slice. |
| `test/test_provider_abstraction_contracts.py` | Are future cache/formatter modules prohibited from provider-specific imports? | Extend with new modules when created. |
| `docs/adr/0006-phase2f1-recipe-lifecycle-classification.md` | Does the ADR clearly exclude cache, template ownership and formatting? | Documentation clarification may be useful; no behavior change. |
| `docs/adr/README.md` | Can new ADRs be added for registry/template/formatting and cache ordering? | Documentation update. |

### New Phase 2F contracts required

Exact repository-native filenames must be selected after source discovery. The following contracts—not filenames—are mandatory:

- `RegistryObjectRef`: stable object ID, object type and version.
- `OutputTemplateDefinition`: template identity/version, supported output shape, formatting rules and governed registry references only.
- `TemplateSuggestion`: template reference, registry version, provenance and deterministic ranking evidence.
- `FormattingPolicy`: approved route and AI-formatting eligibility.
- `ResponseFormatter` port.
- deterministic formatter implementation.
- isolated AI formatter port/adapter, disabled until explicitly approved.
- `FormattedResponseEvidence`: formatter route, template/version, registry version, warnings, source attribution and correlation/audit references.
- future `EarlyCacheKey` and `SemanticResultCacheKey` value contracts without storage-technology dependencies.

## 6. Phase-by-phase impact

### Phase 2F.2 — Approval and reapproval policy

- Retains its original scope.
- Must decide who approves template definitions and formatting policies in addition to recipe approval.
- Must not conflate source-platform ACLs with AskAlpha user authorization.

### Phase 2F.3 — Certified semantic catalog

- Establish the Semantic Registry as the sole business-semantic authority.
- Add versioned KPI, Business Term, Recipe, Relationship and canonical-status identities.
- Definitions describe meaning but never grant access.
- Registry changes and template changes must have separate lifecycle events.

### Phase 2F.4 — Output-template registry

- Largest direct impact.
- Templates reference `RegistryObjectRef` values and never redefine KPIs, terms, recipes or relationships.
- Template selection and formatting routing are deterministic.
- Deterministic formatter is the default route.
- AI formatting remains an optional isolated contract with no active implementation unless PIA-approved.
- Suggestions carry registry version, template version and provenance.
- Early-cache compatibility must not require `semantic_plan_hash`.

### Phase 2F.5 — Evidence-backed relationship impact

- Relationships are registry-owned semantic objects.
- Templates may reference approved relationship IDs but cannot define joins.
- D4–D6 remain blockers; no Graph DB is implied.

### Phase 2F.6 — Hardening and regression

- Add deterministic-vs-AI formatting equivalence checks if the AI route becomes approved.
- Add authorization-scope cache-isolation tests.
- Add registry/template version invalidation tests.
- Preserve existing emitted-table versus governed-scope hardening.

## 7. Earlier-phase compatibility issues

No confirmed earlier-phase incompatibility was found.

Potential integration points requiring verification, not redesign:

- `EffectivePermissions` must generate or support a stable authorization-scope identity suitable for cache keys without exposing raw group/user data.
- Provider access failures need a safe error plus correlation ID at the provider/orchestration boundary.
- Existing `ChatResponse` or report primitives may need an additive formatting-evidence envelope.
- Registry version identity must be usable by templates while recipe compatibility remains entity-scoped; a whole-registry version change must not automatically invalidate unrelated recipes.

Any necessary change should be additive and feature-gated where it could affect accepted behavior.

## 8. Required documentation changes

1. Update the authoritative current-state document with verified Phase 2F.1/PR #18 status after live re-verification.
2. Replace the old single-cache flow with two planned cache stages.
3. Add the explicit response-formatting stage.
4. State that the Semantic Registry is the sole source of business semantics.
5. State that templates contain governed references, presentation rules and routing hints only.
6. Record AskAlpha authorization plus MSI source enforcement and explicitly reject ACL synchronization for the MVP.
7. Label cache platform, Databricks runtime path and provider integrations as Planned/Open.
8. Label AI formatting as Conditional/PIA-dependent.
9. Label Genie as Future/Evaluation.
10. Add separate ADRs for:
    - semantic ownership and template-reference boundary;
    - response-format routing and AI privacy boundary;
    - two-level cache ordering and key/invalidation contracts.

## 9. Test impact

### Required for deterministic templates

- template references resolve only against allowed registry object types and exact versions;
- missing, stale, ambiguous or conflicting refs fail closed;
- template JSON cannot embed independent KPI/term/relationship definitions;
- routing always selects deterministic formatting when an approved applicable template exists;
- identical validated results and contract versions produce identical formatted outputs;
- warnings, as-of date, source attribution and qualifiers are preserved;
- unauthorized requests perform zero cache lookup, registry retrieval, formatting and provider activity.

### Required if AI formatting is later approved

- AI output preserves numeric values, KPI values, signs, units and totals;
- business meaning and material qualifiers remain unchanged;
- authorization scope and masked/redacted fields cannot expand;
- warnings, as-of date and source attribution remain present;
- only approved fields and minimum necessary bounded context reach the adapter;
- deterministic and AI outputs are compared against golden business-result invariants;
- model/provider failure falls back only according to an explicit policy and never changes analytical meaning.

### Required for future cache work

- early keys never use `semantic_plan_hash`;
- keys include authorization scope, normalized intent/template ID, registry/policy/freshness versions and output type;
- cross-scope hits are impossible;
- stale registry, recipe, template, policy or freshness versions invalidate entries;
- raw/unbounded results are ineligible;
- cache failure preserves safe uncached behavior;
- cache implementation imports no provider-specific technology into canonical contracts.

## 10. Documentation-only items

- Revised current/planned/conditional/future capability matrix.
- New pipeline ordering.
- Explicit no-ACL-sync MVP decision.
- Approximately 5 TB bounded-cache position.
- Genie Future/Evaluation status.
- Monthly as the current working template-release cadence, while keeping cadence configurable.
- Separation of semantic lifecycle from template/output lifecycle.

## 11. Future-only items

- Distributed early cache and semantic/result cache implementation.
- Cache platform selection, including any Redis decision.
- Databricks SQL adapter/runtime path.
- Unity Catalog or Collibra governance providers.
- Genie execution-provider evaluation/integration.
- User-identity passthrough or provider-native end-user authorization.
- AI response formatting before PIA approval.
- Scale, concurrency, scan-cost, latency and SLO validation against representative workloads.

## 12. Phase 2G+ plan changes

The publish/validation/rollback lifecycle must treat these as distinct versioned assets:

1. semantic registry objects;
2. recipes and approval evidence;
3. output templates;
4. formatting policies;
5. cache compatibility/invalidation metadata.

A template release may change layout or wording rules but must not redefine a KPI, Business Term or Relationship. A semantic change must use the Semantic Registry lifecycle and trigger impact analysis for dependent recipes/templates. Rollback must preserve reference integrity and must not revive incompatible cached entries.

## 13. Open architecture decisions

1. What exact artifact may the Early Cache return: template match, semantic-plan seed, complete validated result, formatted response, or a controlled subset?
2. Is Early Cache sharing allowed across users with the same authorization-scope hash, or must entries remain user/session-specific?
3. What component owns `data_freshness_version` for Synapse and Databricks sources?
4. What are maximum result rows/bytes, TTLs and cache-eligibility rules?
5. Who approves templates, formatting policies and standard releases?
6. Is monthly release cadence a default policy or a mandatory cadence?
7. Which PIA decision and data classification permit AI-assisted response formatting?
8. What is the approved behavior when deterministic formatting is unavailable and AI formatting is not approved?
9. What stable registry-reference schema and compatibility rules apply across registry versions?
10. Should formatter evidence be included in the public response, audit only, or both?

These questions do not invalidate Phase 2F.1. They gate later implementation slices.

## 14. Recommended implementation sequence

1. **Live-state gate:** In the permanent `SSH: kmai-13` workspace, independently verify current `main`, PR #18 merge state, exact ten-file tree and workflows.
2. **Documentation alignment:** Update authoritative architecture/status/decision documents and add a capability-status matrix. Do not change runtime behavior.
3. **2F.2 decision closure:** Resolve approval owners, evidence/expiry/reapproval rules, `REVIEW_REQUIRED` policy, and template/formatting-policy approvers.
4. **2F.3 certified semantic catalog:** Implement versioned governed semantic objects and stable references.
5. **2F.4a template contracts:** Add versioned template definitions and suggestions containing only registry references and provenance.
6. **2F.4b deterministic formatting:** Add explicit formatting routing and deterministic formatter; keep AI route disabled.
7. **2F.4c conditional AI boundary:** Define or implement only after PIA/product approval.
8. **2F.5 relationship impact:** Proceed only after D4–D6 are resolved.
9. **2F.6 hardening:** Add output consistency, registry/template invalidation, authorization isolation and regression gates.
10. **Phase 2G publishing:** Add controlled publish/validation/rollback for separately versioned semantic and template assets.
11. **Later cache implementation:** After measured requirements and security design, implement provider-neutral cache adapters and select a platform separately.

## 15. Small local correction recommendation

No code correction is currently proven necessary.

The only immediately justified work is documentation alignment plus a bounded read-only repository discovery. Any code edit before that discovery would risk inventing module locations or modifying an already accepted Phase 2F.1 implementation without evidence.

## Final disposition

`ARCHITECTURE_DELTAS_COMPATIBLE_WITH_2F1_FUTURE_SLICES_REQUIRE_ALIGNMENT`
