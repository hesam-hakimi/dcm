# askAlpha / KMAI — Phase 2F Scope Discovery

> **Historical checkpoint — notice added 14 September 2026.** The record below preserves its original August evidence and phase/authorization wording. It is not today's operative status or next-task instruction. Read `/AskTD/AskTD_LATEST.md` and the updated Leadership Alignment package first. The newer supplied report describes 2F.1 implementation on a development branch; merge, activation and current HEAD require verification. Preserve later user authorizations. The source-review inventory and diagram reconciliation are now recorded in the September package. Historical SHA values and tests below have not been changed or rerun.

**Date:** 2026-08-26  
**Status:** Scope discovery complete; implementation not authorized

## Authoritative Phase 2F definition

**Recipe Lifecycle, Certified Semantics, Output Templates, and Evidence-Gated Relationship Impact.**

This definition supersedes older roadmap wording that described Phase 2F only as “Answer Intelligence & Reporting Experience.” Answer and reporting improvements remain valid roadmap outcomes, but the immediate Phase 2F foundation is lifecycle governance built on Phase 2E evidence.

## Why Phase 2F is now possible

Phase 2D created one deterministic Approved Recipe pilot. Phase 2E added exact governed field dependencies, dependency fingerprints, and reverse impact lookup. Phase 2F can now determine whether a recipe remains usable after governed metadata changes without relying on whole-registry version changes or AI judgment.

## Recommended delivery sequence

### Phase 2F.1 — Deterministic recipe lifecycle evaluator

Recommended next implementation slice:

- introduce a frozen lifecycle result contract;
- classify `VALID`, `REVIEW_REQUIRED`, `BROKEN`, and `NOT_APPROVED`;
- consume only existing recipe approval metadata and Phase 2E dependency evidence;
- emit deterministic reason codes and affected dependency references;
- remain pure, in-memory, provider-neutral, and side-effect free;
- fail closed for missing, ambiguous, conflicting, or invalid required evidence;
- preserve current Phase 2E behavior when the new feature flag is OFF;
- add focused unit, integration, denial-path, flag-off, and mutation-sensitivity tests;
- add an ADR defining the lifecycle boundary and owner decisions that remain external.

### Phase 2F.2 — Approval and reapproval policy integration

Only after Product and Governance decide:

- authoritative approval owner;
- approval evidence schema;
- expiry and renewal rules;
- whether `REVIEW_REQUIRED` warns or blocks;
- who may acknowledge or reapprove a change.

### Phase 2F.3 — Certified semantic catalog

Add governed KPI definitions, glossary terms, business rules, ownership, version identity, and recipe references. These records describe meaning but never grant authorization.

### Phase 2F.4 — Output-template registry

Add governed, versioned template contracts for consistent answer/report layouts. Keep rendering and advanced export work separately bounded.

### Phase 2F.5 — Evidence-backed relationship impact

Add relationship/join adjacency only after D4-D6 are resolved: field evidence, governed endpoint datasets, and naming consistency. Do not invent joins or introduce a Graph DB by default.

### Phase 2F.6 — Deferred hardening and additional recipes

Add emitted-table versus governed-scope cross-check and consider additional recipes only after lifecycle behavior is independently proven.

## Lifecycle contract

| State | Meaning | Minimum deterministic evidence |
|---|---|---|
| `VALID` | Recipe approval and every referenced dependency still match accepted evidence. | Applicable approval evidence; all dependency references resolve; current fingerprint matches. |
| `REVIEW_REQUIRED` | Referenced evidence changed but remains resolvable and requires governance review. | Relevant fingerprint/evidence change with explicit affected references and reason codes. |
| `BROKEN` | The recipe cannot safely resolve required governed evidence. | Missing, renamed without approved mapping, ambiguous, conflicting, or invalid required dependency. |
| `NOT_APPROVED` | No valid approval applies to the current recipe/dependency identity. | Missing, invalid, expired, or non-applicable approval evidence. |

Runtime behavior for `REVIEW_REQUIRED` is an owner decision. The pure evaluator may classify it before the warn-versus-block policy is selected.

## Non-negotiable constraints

- Provider-agnostic core.
- Metadata/classification never grants access.
- Compatibility remains entity-scoped, not whole-registry pinned.
- No provider changes in the first slice.
- No invented approval, business meaning, dataset, field, join, or relationship.
- Fail closed on missing or conflicting governed evidence.
- Preserve governance-before-builder/SQL/execution ordering.
- Maintain feature-flag rollback to exact Phase 2E behavior.
- Use a permanent Phase 2F worktree only after explicit implementation authorization.

## Explicitly outside Phase 2F.1

KPI/glossary authoring, output rendering, relationship graph, lineage, additional production recipes, recipe administration UI/API, Databricks, Genie, Unity Catalog, Collibra, Redis, Graph DB, cross-source execution, provider/dialect work, frontend, deployment, infrastructure, branch deletion, and repository cleanup.

## Recorded future scale context — no Phase 2F.1 scope change

- Expected data volume: approximately 5 TB or more.
- Synapse data location: Dedicated SQL Pools.
- Databricks data location: Data Lake.
- Later Phase 3 work must preserve provider-side query execution and bounded result return through dedicated adapters.
- Later Phase 6 work must prove scale, concurrency, scan cost, latency, result limits, and SLO behavior using representative workloads.

This item is intentionally deferred for a separate architecture discussion. The Phase 2F.1 evaluator processes small governance and dependency evidence only; it does not scan or move analytical data.

## Open decisions and owners

| Decision | Owner | Blocks |
|---|---|---|
| Warn or block on `REVIEW_REQUIRED` | Product + Governance | Runtime policy, not pure classification |
| Approval owner, evidence, expiry, reapproval | Product + Governance | Approval integration |
| D4 field evidence | Data Governance | Relationship slice |
| D5 governed relationship endpoints | Data Governance | Relationship slice |
| D6 naming consistency | Governance + Architecture | Relationship slice |
| Metadata vs authorization product-group namespaces | Architecture | Integration; metadata must not grant access |
| Strict metadata-mode activation | Backend + DevOps | Runtime proof, not pure evaluator |

## Acceptance gates for Phase 2F.1

- deterministic results for identical input;
- order-independent dependency input;
- unrelated entity changes do not alter lifecycle result;
- relevant dependency changes produce explicit `REVIEW_REQUIRED` evidence;
- missing/conflicting required evidence produces `BROKEN` without downstream activity;
- missing/non-applicable approval produces `NOT_APPROVED`;
- unchanged approved candidate produces `VALID`;
- feature flag OFF reproduces Phase 2E behavior exactly;
- no provider, schema-probe, builder, SQL, or execution call before lifecycle acceptance;
- focused tests, full backend regression, golden tests, coverage gate, ADR, and independent review pass.

## Next permitted action

Prepare and review one bounded Phase 2F.1 implementation prompt. Do not create a branch, worktree, code change, commit, push, or PR until the user explicitly authorizes that exact implementation slice.
