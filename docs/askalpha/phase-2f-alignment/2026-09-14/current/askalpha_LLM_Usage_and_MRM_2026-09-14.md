# askalpha (AskTD) — LLM usage and MRM scope

**Updated:** 14 September 2026 | **Version:** 1.0 | **Status:** Reported source-inspection summary; runtime configuration and use-case approval not established

This reference consolidates the owner's latest LLM-usage email and the supplied engineering-agent report. It replaces the earlier planning statement that no inventory had yet been reported. It is not a fresh source audit or a substitute for the agent's complete call-site inventory.

## 1. Evidence and counting rules

| Item | Current evidence |
| --- | --- |
| Reported repository/revision | `TD-Enterprise/kmai-td-genie` at `6e37281e61a782ffbe8c8675346144567406dabe`, as shown in the supplied report. Current HEAD was not checked for this update. |
| Reported orchestration | AG2 / `autogen`; the architecture drawing names Bottlenose / LangGraph. A migration is not inferred. |
| Application integration paths | Two reported Azure OpenAI paths: direct tool integration and the agent-manager helper. Verify actual gateway routing and deployed settings separately. |
| Inventory count | **16 potential invocation paths** across agent roles and tool methods. This is neither calls per question nor the number of distinct models. |
| Purpose categories | The nine categories below group behavior for governance discussion; they are not a one-to-one mapping to the 16 paths. |
| Runtime evidence | Actual model/deployment versions, request volumes, call counts, feature activation, latency and cost were not established by the static review. |

Recipes and deterministic builders may avoid selected planning or SQL-generation calls. They do not necessarily eliminate later interpretation, visualization or report-writing calls. Retries and review loops can add calls. No fixed “five calls” or “16 calls per request” budget is assumed.

## 2. Usage summary

IDs below identify **purpose categories**, not physical call sites. Retain the engineering inventory's caller paths and stable invocation IDs when available.

| Purpose ID | Purpose | Information provided, according to the supplied review | Expected output | Qualification requirement |
| --- | --- | --- | --- | --- |
| U01 | Intent identification | User question; conversation history on some paths | Classification and routing | Verify permitted context, allowed classes and fallback. The meeting's pattern-based description does not cover every reported current branch. |
| U02 | Question clarification | Question and relevant metadata/context | Clarification question or answerability decision | Deterministic contract for missing KPI, period, grain or scope; unsupported requests must not bypass it through a fast path. |
| U03 | Semantic mapping | Question and Registry context | Supported business-intent mapping | Restrict context to permitted scope; validate identifiers and governed meaning. |
| U04 | Analysis planning | Question and relevant metadata | Plan for one or more queries | Validate plan schema, source scope, dependencies, permitted relationships and bounded work. |
| U05 | SQL generation | Question, schema/metadata and correction feedback where used | SQL proposal | Read-only validation, object/scope enforcement and bounded execution remain mandatory. |
| U06 | Query-error handling | Failed query and execution-error context | Correction, clarification or stop decision | Replace uncontrolled error text with permitted structured diagnostics; limit correction attempts and preserve safe-stop behavior. |
| U07 | Visualization | Question and result previews | Chart specification or visualization code | Approve the payload and renderer contract; validate values and fields. Qualify any generated-code execution separately. |
| U08 | Answer/report generation | Question, result rows or aggregates and supporting context | Business summary or analytical report | Minimize and authorize result context; preserve values, units, scope, dates, sources and warnings. |
| U09 | Answer review | Question and drafted answer | Coverage/format feedback, potentially followed by revision | Treat the draft as result-bearing context where applicable; bound revisions and retain deterministic integrity checks. |

These are potential behaviors reported from source inspection, not proof that every route is enabled or approved. A report-review model is present in the reported request path; an absence of offline model-based evaluation does not mean there is no reviewer model anywhere.

## 3. Control gaps and closure evidence

| ID | Reported finding / boundary | Required closure evidence |
| --- | --- | --- |
| L01 | Database exception text can reach model error-handling paths. | All affected callers pass a structured permitted diagnostic payload. Use synthetic sentinel tests at both application model boundaries to prove excluded values do not leave the application. Preserve enough safe context for correction/stop behavior. |
| L02 | Query results or previews may reach visualization and answer/report generation. | Explicit purpose-specific field/row/aggregate eligibility, required treatment and approval coverage. Access to query data alone does not approve transmission to an LLM. |
| L03 | Conversation history can contain previously permitted data. | Current-turn scope revalidation, trusted session ownership and tests for access change, cross-user context and unsupported history. |
| L04 | Metadata framing is limited in the reported code. | Shared input contracts for untrusted text and a clear distinction between framing, redaction and authorization. Delimiters alone establish none of the latter two. |
| L05 | LLM report generation is still used on relevant current paths. | Explicit deterministic-template versus approved AI-formatting routing, with fidelity tests and a safe route when AI output is not eligible. Do not describe the target deterministic default as already implemented. |
| L06 | Helper-level JSON/schema behavior and generated visualization code need qualification. | Demonstrate downstream schema/semantic validation, safe malformed-output handling and the permitted rendering boundary. Existing restrictions are evidence to assess, not a complete sandbox attestation. |
| L07 | Durable application correlation and enterprise AIOBS integration are not established by the report. | Demonstrate the supported SDK/transport, correlation, permitted trace fields, storage, access and retention. In-memory traces/UI debugging do not prove durable evidence. |
| L08 | Business acceptance and observed serving metrics remain open. | Deposits SME-approved reference questions and calculations; measured route-specific quality, warm/cold latency, concurrency, failure behavior and cost under an approved test setup. |

These gaps are not closed by this documentation. The previously suggested **2F.1a** error-payload hardening is a bounded engineering proposal, not a completed implementation or a new blanket authorization. Protect actual outbound payload construction; regex replacement alone is not a sufficient acceptance claim.

## 4. Full inventory contract for the engineering record

For every potential invocation path, retain a stable call ID, exact repository revision, caller and shared helper, business purpose, trigger/skip conditions, flags, input categories, output schema, validators, retry/review limits, configured provider/deployment references, telemetry and applicable use-case approval reference. Record source findings separately from runtime observations.

Use synthetic examples or payload schemas, not sensitive values, credentials or real query results. A later authorized runtime check can measure a recipe hit, free-form query, clarification, correction and review path where enabled. Its results should include model and transport retries; do not estimate actual volumes from static call-site counts.

## 5. Proposed MRM boundary and responsibilities

The proposed assessment boundary is the complete **question-to-final-answer use case for the approved Deposits scope**, with the individual model interactions documented inside it. MRM must confirm that boundary, the appropriate inventory/registration approach and how later portfolio or purpose changes are assessed.

| Responsibility | Required confirmation |
| --- | --- |
| Accountable business/model owner | Named owner for the Deposits use case and its ongoing validation. Governance coordination and technical delivery ownership are separate roles. |
| Business validation | Deposits SMEs approve questions, calculations, expected outcomes, materiality thresholds and review cadence. |
| Technical control ownership | Engineering owns implementation evidence; platform/observability teams confirm their actual contracts and operating responsibilities. |
| Privacy/data-use coverage | Appropriate authority confirms the permitted inputs, results, history and trace content for each enabled purpose. Existing approval is reused where its scope applies. |
| Change and monitoring | Record model/deployment, prompt, metadata, recipe and formatting changes; rerun affected acceptance evidence and retain rollback/disable procedures. |

Feedback is reviewed to improve definitions, prompts, recipes, data quality or formatting through controlled releases. Automatic model retraining or self-modifying production templates was not agreed in the meeting.

## 6. Sources

- Latest user-edited email 72641, “AskTD – LLM Usage Inventory and MRM Scope,” supplied in this conversation; unchanged and not sent by this update.
- Supplied engineering-agent screenshots and discussion at the revision recorded above; treated as reported source evidence.
- Leadership transcript, especially 03:19–08:00, 72:51–78:59, 92:35–96:43 and 99:29–101:18.
- `askalpha_Solution_Architecture_2026-09-14.md` and the updated three Leadership Alignment records for architecture, acceptance and ownership context.
