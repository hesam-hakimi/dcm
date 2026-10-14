# AskTD / askAlpha / KMAI — Assumption and Decision Log

> **Historical checkpoint — notice added 14 September 2026.** The record below preserves its original August evidence and phase/authorization wording. It is not today's operative status or next-task instruction. Read `/AskTD/AskTD_LATEST.md` and the updated Leadership Alignment package first. The newer supplied report describes 2F.1 implementation on a development branch; merge, activation and current HEAD require verification. Preserve later user authorizations. The source-review inventory and diagram reconciliation are now recorded in the September package. Historical SHA values and tests below have not been changed or rerun.

**Original date:** 2026-08-23  
**Latest verified update:** 2026-08-26

## Accepted and validated

- askAlpha remains provider-agnostic.
- SQL Server/Azure SQL remains the current concrete path.
- The orchestrator depends on `DataSourceAdapter`, not `SqlDataStore`.
- `MetadataRegistryService` + `RegistrySnapshot` remain the canonical governance boundary.
- `EffectivePermissions` remains the current entity-level authorization foundation.
- Governed validation precedes adapter, schema, builder, SQL, and execution activity.
- `builder_key` is authoritative.
- Recipe compatibility is entity-scoped, not whole-registry pinned.
- Fields are emitted only for already-governed datasets.
- Classification and metadata never grant authorization.
- Phase 2E graph scope is only an in-memory recipe dependency index.
- Phase 2E / PR #17 is merged and independently reverified.
- Current verified `main` is `f283f01b6d615f9fa00debcef959d9c5c86a3224`.
- Phase 2F is the next planned phase; implementation remains separately authorization-gated.
- Phase 2F should begin with a pure deterministic lifecycle evaluator using existing Phase 2E evidence.
- Redis, Databricks, Genie, Unity Catalog, Collibra, Graph DB, and new provider work are not dependencies of the first Phase 2F slice.

## Phase 2F lifecycle definitions for scope design

- `VALID`: current governed dependencies match accepted evidence and the recipe has valid approval evidence.
- `REVIEW_REQUIRED`: relevant governed evidence changed but remains resolvable; governance policy must decide whether this warns or blocks.
- `BROKEN`: required dependency is missing, renamed without an approved mapping, ambiguous, conflicting, or otherwise invalid.
- `NOT_APPROVED`: approval evidence is missing, invalid, expired, or not applicable to the current recipe/dependency identity.

These are working contract definitions for implementation planning, not authorization to invent approval records or ownership rules.

## Open decisions and dependencies

- D1 strict metadata mode activation — Backend + DevOps; runtime activation, not Core lifecycle logic.
- D4 field evidence for `v_dlv_dep_prty_agmt` — Data Governance; needed for later relationships.
- D5 govern relationship endpoint datasets — Data Governance; needed for multi-dataset graph.
- D6 resolve schema/field naming inconsistencies — Governance + Architecture.
- D7 decide whether `REVIEW_REQUIRED` warns or fails closed — Product + Governance; blocks runtime policy, not pure classification.
- D8 reconcile metadata and authorization product-group namespaces — Architecture; metadata must never grant access.
- D9 define Genie coexistence boundary — Product + Architecture; Phase 3.
- Define authoritative approval owner, approval evidence schema, expiry/reapproval rules, and reason codes — Product + Governance.
- Deferred emitted-table versus governed-scope cross-check — separate hardening slice.
- Newly confirmed scale context: approximately 5 TB or more; Synapse data in Dedicated SQL Pools and Databricks data in the Data Lake — Architecture + Platform owners; requires later Phase 3 adapter/query-pushdown design and Phase 6 representative performance, concurrency, scan-cost, and SLO validation.

The scale item is recorded for later architecture discussion. It does not block or expand the pure Phase 2F.1 lifecycle classification slice.

## Deferred from the first Phase 2F slice

Recipe administration UI/API, additional production recipes, KPI/glossary authoring, output-template rendering, relationship/join graph, lineage, Databricks/Genie/UC/Collibra, Redis/result caching, cross-source execution, provider changes, frontend/deployment/infrastructure, and repository cleanup.

## Do not assume

- merged means the next phase is automatically authorized;
- `REVIEW_REQUIRED` policy can be selected by engineering;
- evidence may invent approval, datasets, joins, ownership, or business meaning;
- whole registry version should lock recipe compatibility;
- Graph DB or Redis is required;
- Genie replaces askAlpha;
- metadata grants access;
- stale `asktd_v2` is a valid base.
