# AskTD / askAlpha / KMAI — Architecture and Roadmap Update

> **Historical checkpoint — notice added 14 September 2026.** The record below preserves its original August evidence and phase/authorization wording. It is not today's operative status or next-task instruction. Read `/AskTD/AskTD_LATEST.md` and the updated Leadership Alignment package first. The newer supplied report describes 2F.1 implementation on a development branch; merge, activation and current HEAD require verification. Preserve later user authorizations. The source-review inventory and diagram reconciliation are now recorded in the September package. Historical SHA values and tests below have not been changed or rerun.

**Original date:** 2026-08-23  
**Latest verified update:** 2026-08-26

## Product position

askAlpha is a governed, provider-agnostic analytics orchestration layer. It owns authentication context, effective scope, canonical semantics, deterministic validation, approved business logic, audit/version evidence, provider routing, and the answer/report experience. It may delegate execution without surrendering these responsibilities.

## Current implemented architecture through Phase 2E

```text
Entra user/context
 -> EffectivePermissions
 -> deterministic route / ApprovedRecipe
 -> MetadataRegistryService + RegistrySnapshot
 -> evidenced governed FieldRecords
 -> GovernedSemanticPlan validation
 -> recipe dependency fingerprints and impact lookup
 -> SQL safety and authorization
 -> DataSourceAdapter
 -> current SqlDataStore / SQL execution
 -> validated ChatResponse/report primitives
```

Compatibility is entity-scoped, not pinned to a whole registry version. Unrelated metadata changes may alter `registry_version` without invalidating a recipe; relevant changes alter dependency evidence or fail closed.

## Phase 2E closure

Phase 2E is merged and independently verified on `main` at `f283f01b6d615f9fa00debcef959d9c5c86a3224`. The automatic merge workflow and downstream workflow both completed successfully.

The graph capability remains intentionally small: an in-memory `entity_ref -> recipe_ids` impact index. It is not a graph database.

## Phase 2F architecture direction

Phase 2F converts Phase 2E evidence into controlled lifecycle decisions and then layers certified meaning and presentation contracts:

```text
ApprovedRecipe + approval evidence
 + current governed dependency evidence
 + stored dependency fingerprint
 -> deterministic lifecycle evaluator
 -> VALID | REVIEW_REQUIRED | BROKEN | NOT_APPROVED
 -> explicit reason/evidence
 -> execution gate or governance review path
```

The first slice should be pure and provider-neutral. KPI/glossary, output-template registry, and evidence-backed relationship adjacency should follow as separate bounded slices.

## Relationship and graph boundary

- Do not hard-code joins around missing governance evidence.
- Relationship adjacency begins only after D4-D6 metadata sourcing and naming work is complete.
- Graph DB is not required at current scale.
- Lineage, cross-source reasoning, and provider expansion are not part of the first Phase 2F slice.

## Better answers and reports

- semantic correctness and field-level change protection: completed through 2E;
- lifecycle, certified KPI/glossary meaning, templates, and relationship impact: 2F;
- incremental charts/UX: parallel but separately scoped;
- heavy reasoning improvements: measurement-gated by Phase 5;
- advanced downloads/exports: Phase 8.

## Cache and provider boundaries

Redis remains a Phase 6 benchmark/security decision. Databricks, provider registry, dialect handling, and Genie coexistence remain Phase 3 approval-dependent work. Metadata and classification never grant authorization.

## Newly confirmed future scale context

- Expected analytical volume is approximately 5 TB or more.
- Synapse-resident data is in Dedicated SQL Pools.
- Databricks-resident data is in the Data Lake.
- askAlpha must remain a control/orchestration plane: filtering, joins, and aggregation execute in the provider; only bounded results return to the application.
- Phase 3 must validate dedicated Synapse and Data Lake/Databricks adapters, identity, query pushdown, workload behavior, and coexistence boundaries.
- Phase 6 must add representative scale and concurrency benchmarks, query/data-scan budgets, result-size limits, latency/SLO evidence, and cost measurement before any caching or Redis decision.

This scale context does not change the Phase 2F.1 lifecycle-evaluator scope. Detailed scale architecture remains a later discussion and separately approved work item.
