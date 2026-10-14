# AskTD / KMAI — Phase 2E Bounded Implementation Prompt

> **Historical checkpoint — notice added 14 September 2026.** The record below preserves its original August evidence and phase/authorization wording. It is not today's operative status or next-task instruction. Read `/AskTD/AskTD_LATEST.md` and the updated Leadership Alignment package first. The newer supplied report describes 2F.1 implementation on a development branch; merge, activation and current HEAD require verification. Preserve later user authorizations. The source-review inventory and diagram reconciliation are now recorded in the September package. Historical SHA values and tests below have not been changed or rerun.

Copy the block below into a new coding-agent session after live base verification.

```text
We are implementing PHASE 2E — GOVERNED FIELD RECORDS AND DEPENDENCY-AWARE RECIPE REFERENCES. This is a continuation of the independently accepted Phase 2D candidate, not a redesign and not Phase 2F.

1. VERIFY BASE
Repository: TD-Enterprise/kmai-td-genie. Expected base `origin/phase2/approved-recipe-pilot` at `5d267fdac75c5e76ab13f93ae0eb2bbb999b08a5`, parent `d5472ae31081879329c224922244d87962737e8c`. Verify main, PR #15/#16, SHAs, files, ancestry. If drift: `PHASE_2E_IMPLEMENTATION_BLOCKED_BASE_DRIFT`. Do not repair/rebase the accepted base.

2. WORKSPACE
Do not use stale `asktd_v2`, touch its dirty files, or use `/tmp`. Create/reuse branch `phase2/governed-field-records` from `origin/phase2/approved-recipe-pilot` in `/home/tag5916/projects/kmai-td-genie-worktrees/phase2e-governed-field-records`. If existing state is unsafe: `PHASE_2E_IMPLEMENTATION_BLOCKED_EXISTING_WORKTREE_STATE`.

3. MUTATION BOUNDARY
Allowed: branch/worktree, ADR 0005, bounded source/tests, local validation, report outside candidate. Forbidden: stage, commit, push, PR, merge, rebase, force-push, changes to PR #15/#16/main/primary checkout, Phase 2F, deployment/config/infrastructure.

4. ADR FIRST
Create `docs/adr/0005-phase2e-governed-field-records.md` and update ADR index before code. Define evidenced fields only, already-governed datasets only, no invented meaning, deterministic IDs, fail-closed evidence, authorization separation, entity-scoped fingerprints, no whole-registry compatibility pin, flag rollback, lifecycle/relationships/providers/cache/reporting/infrastructure deferrals.

5. BOUNDED SOURCE
Expected MODIFY: `available_data/registry_contract.py`, `recipes/approved_recipes.py`. Expected CREATE: `available_data/field_evidence.py`, `recipes/dependency_fingerprint.py`. Do not modify `orchestrator.py`, `semantic_models.py`, `query_recipes.py`, API DTOs, authorization, SQL policy, frontend, deployment, or infrastructure. Stop if required.

6. EVIDENCE
Inspect `data/metadata/json/field.json`, `table.json`, and `relationship.json`. Use field evidence only. Deterministic/order-independent loader; map only to governed datasets; no name inference; no silent coercion; fail closed for governed conflicts; ignore non-governed evidence without creating records; reject duplicate/colliding field IDs. Define and test explicit stable field-ID normalization.

7. SNAPSHOT / FLAG
Integrate at existing legacy-to-canonical boundary. Add default-OFF `GOVERNED_FIELD_RECORDS_ENABLED`. OFF reproduces Phase 2D snapshot semantics and registry version. ON emits valid fields only for governed datasets, includes them in canonical identity, preserves strict validation, emits no relationships. No deployed config change.

8. PILOT FIELD REFS
Add canonical `governed_field_refs` to the single pilot recipe. Inspect actual builder/evidence; do not copy suggested fields blindly. Do not add recipes or modify SQL builders.

9. VALIDATION
Reuse existing GovernedSemanticPlan/service validator. Unknown/removed/renamed referenced fields must fail before factory, adapter, schema probe, builder, SQL construction, or execution. Reuse Phase 2D zero-call harness.

10. FINGERPRINT / INDEX
Implement pure `entity_fingerprint(record)` and `dependency_fingerprint(referenced_records)`. Equivalent content/order variants same; duplicates canonicalized; unrelated edits same; referenced semantic edit different; missing ref deterministic failure; no runtime/path/cache inputs. Add internal in-memory `entity_ref -> recipe_ids` reverse index, no persistence/API.

11. BOUNDARIES
No authorization changes, classification grants, relationships, graph DB, Redis, provider SDK, Databricks, Genie, Unity, Collibra, cross-source, SQL compiler, frontend, or infrastructure. Extend provider-import guard.

12. TESTS
Add `test_governed_field_records.py` and `test_recipe_dependency_fingerprint.py`; extend focused registry/semantic-plan/approved-recipe/provider tests. Prove deterministic emission, ID/collision rules, no invented datasets, governed conflict failure, ON validation, OFF compatibility, real field-scoped plan, unknown field error, valid pilot execution, zero side effects on missing/renamed fields, unrelated-edit fingerprint stability, relevant-edit change, reverse index, Phase 2C/2D/auth/provider/golden regressions, full backend/coverage, `git diff --check`, excluded-tech scan.

13. STRICT MODE / ROLLBACK
Do not enable strict mode in an environment. Test locally. Field flag OFF restores zero fields and Phase 2D identity; pilot flag OFF ignores field refs. No migration.

14. REPORT
Save outside candidate at `/home/tag5916/projects/kmai-td-genie-worktrees/reports/ASKTD_PHASE_2E_IMPLEMENTATION_2026-08-23.md`. Include evidence, diff, ADR, IDs, validation, fingerprints/index, tests, coverage, golden, scans, rollback, hashes/digest, risks, review scope. Leave files unstaged/uncommitted/unpushed.

Return exactly `PHASE_2E_IMPLEMENTATION_READY_FOR_INDEPENDENT_REVIEW` or `PHASE_2E_IMPLEMENTATION_BLOCKED_<REASON>`. Attest primary checkout/dirty files/PR #15/#16/main/deployment/Phase 2F untouched; no stage/commit/push/PR. STOP.
```
