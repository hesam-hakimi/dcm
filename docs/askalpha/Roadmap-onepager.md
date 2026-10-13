AskAlpha — Executive Product Roadmap

**Earn trust → prove repeatable value → scale governed analytics**

**Version:** 1\.0
**Prepared:** 13 October 2026
**Status:** Proposed executive delivery plan; dates and release approvals require confirmation\.
**Product:** A read\-only enterprise analytics assistant, starting with Deposits\.

> **Product promise:** Employees ask questions about approved business data, receive understandable and traceable answers, and turn useful analyses into saved questions, owner-created templates, and scheduled reports.

---

## 1\. Executive roadmap — presentation view

### Current status

**Overall delivery status: TO CONFIRM with the program owner\.**

|Status item                               |Position to present                                                                                                    |
|------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
|Engineering baseline                      |Phase 2F.1 is the checkpoint reported in the product documents. Preserve completed work; this roadmap is not a restart.|
|Deposits readiness                        |Confirm the supported questions, data, personas, reference calculations, and accountable business owners.              |
|Proof-of-concept acceptance               |Completion and business acceptance are not established by the two source documents.                                    |
|Privacy, architecture, and model approvals|Confirm PIA, ABP, ARB, data-access, and MRM decisions individually. Do not present them as a single completed approval.|
|Production readiness                      |Requires evidence for access, serving capacity, monitoring, support, and operational ownership.                        |
|Delivery capacity                         |Four-person team is the planning assumption; start date, availability, and external support remain to be confirmed.    |

### Executive phase bands

|Executive Phase 1                       |Executive Phase 2                 |Executive Phase 3                              |
|----------------------------------------|----------------------------------|-----------------------------------------------|
|**Governed Foundation & Deposits Pilot**|**Everyday Use & Recurring Value**|**Management Reporting & Controlled Expansion**|
|Q4 2026–Q1 2027                         |Q2–Q3 2027                        |Q4 2027+                                       |

**User journey:** ASK → CLARIFY → ANALYZE → EXPLAIN → SAVE / SCHEDULE

*These executive phases group product outcomes\. They do not replace or renumber engineering phases such as 2F\.1\.*

### What each milestone delivers

**All milestone cells below describe proposed deliverables, not completed capabilities\.**

|Workstream                |Q4 2026 — Readiness                                                                                                                 |Q1 2027 — Trusted Pilot                                                                                                        |Q2 2027 — Everyday Use                                                                                                                            |Q3 2027 — Recurring Value                                                                                                                             |Q4 2027+ — Reporting & Expansion                                                                                                |
|--------------------------|------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
|**Business Experience**   |**Deposits Readiness**<br>Agree questions and personas<br>Confirm metrics and filters<br>Select pilot users                         |**Governed Deposits Pilot**<br>Answers, tables, basic charts<br>Clarification and session follow-ups<br>User feedback          |**Everyday Self-Service**<br>Saved chats and questions<br>Explicit personal preferences<br>Owner-created question templates                       |**Scheduled Reports & Suggestions**<br>Recurring report subscriptions<br>Secure delivery and run history<br>Relevant follow-up suggestions            |**Management Reporting**<br>Multi-section reports<br>Approved Excel/PDF exports<br>Richer exploration; optional new source      |
|**Trust, Data & Controls**|**Approved Semantic Scope**<br>Business owners and definitions<br>Registry and recipe references<br>Access and approval requirements|**Pilot Control Evidence**<br>Scope and model-payload checks<br>Business-approved reference answers<br>Required pilot sign-offs|**Controlled Content & Memory**<br>Review and version templates<br>Reauthorize saved history<br>Preference consent and retention                  |**Secure Reporting & Improvement**<br>Owner and recipient access checks<br>Freshness and template-version rules<br>Human-approved content improvements|**Continuous Assurance**<br>Audit and access review<br>Consistency across reports and exports<br>Approval before expanding scope|
|**Platform & Operations** |**Platform Readiness**<br>Runtime identity and connectivity<br>Secure environments<br>Monitoring and support design                 |**Observable Pilot**<br>Health, errors, and correlation<br>Usage and estimated cost metering<br>Named support and basic alerts |**Managed Service**<br>History and preference storage<br>Team usage and allowances<br>Eligible early-cache reuse, if ready                        |**Reliable Report Operations**<br>Scheduler, retries, no duplicates<br>Delivery monitoring and alerts<br>Budget limits and run controls               |**Operational Scale**<br>Latency, concurrency, recovery<br>Reconciled costs and chargeback<br>Support and incident procedures   |
|**Adoption & Value**      |**Pilot Baseline**<br>Acceptance criteria and users<br>Current manual effort<br>Budget and cost assumptions                         |**Pilot Evidence**<br>Answer quality and feedback<br>Repeat use and time saved<br>Cost per successful analysis                 |**Adoption & Service Plans**<br>Train users and template owners<br>Measure saved-question/template reuse<br>Agree subscription or chargeback model|**Repeatable Value**<br>Report adoption and on-time delivery<br>Suggestion and preference usefulness<br>Interactive versus scheduled cost             |**Benefits Review**<br>Productivity and sustained adoption<br>Value against total operating cost<br>Expand, improve, or pause   |

**Gate 1 — Evidence\-ready pilot:** after Q1 2027, before wider everyday use\.
**Gate 2 — Repeatable value and operational readiness:** after Q3 2027, before broader reporting and expansion\.

**Key outcomes:** Answer Quality · Adoption · Control Readiness · Reliability / Latency · Cost / Value

**Legend:** Current / Reported = an existing planning checkpoint, not automatic runtime proof\. Proposed = a delivery target\. Conditional / Future = additional approval or dependency required\.

### Calendar assumption

The source roadmap defines four delivery quarters from the agreed team start, not fixed calendar dates\. To fit the supplied executive template, this document proposes **Q4 2026 for readiness and Q1–Q4 2027 for the four product releases**\.

Readiness is preparatory work, not a completed release\. The “\+” indicates later approved expansion; it is not a promise of autonomous business action\. If the delivery start changes, move the calendar labels while preserving the release sequence\. Confirm dates and capacity before treating this view as a delivery commitment\.

---

## 2\. Milestone outcomes and demonstrations

*Examples are illustrative\. Every supported metric, relationship, and calculation requires business approval\.*

### Q4 2026 — Agree what the Deposits pilot will prove

**Target outcome:** A bounded, owned, and testable pilot scope, built on the existing implementation\.

Business and data owners select the initial questions, permitted datasets, personas, and reference answers\. The team confirms identity and source connectivity, required approvals, support responsibilities, and the monitoring and cost baseline\. Template, conversation\-history, and personalization decisions are recorded without presenting those features as already delivered\.

**Concrete example:** Agree how to answer “What was Ontario’s September month\-end deposit balance, compared with August?” Define the approved metric, region filter, reporting dates, currency, and expected result\.

**Readiness evidence:** Named owners; agreed question set and acceptance criteria; reference calculations; a dependency and approval register; and a realistic team plan\.

**Before any real\-data pilot:** Required access, privacy, payload, and environment approvals must be in place\. If they are not, continue with synthetic fixtures and unaffected engineering work—not unapproved data access\.

### Q1 2027 — Deliver a trusted Deposits pilot

**Target outcome:** Selected users can complete a small set of useful analyses and understand the answers\.

Target approximately **10–15 approved question patterns**, subject to business agreement\. Deliver validated answers, tables, basic charts, clarification, limited same\-conversation follow\-ups, and feedback\. Show the metric, period, filters, units, source, and data freshness\.

The application maintains the active analysis context—such as region, month, metric, and breakdown—so the next message can refine the same analysis\. It checks current access at each turn\. This is session context, not persistent personal memory\.

**Demo:** Ask the monthly balance question, then say “Break that down by product\.” The answer retains the region and dates, changes only the requested breakdown, and displays consistent numbers\. An unauthorized user cannot obtain the protected answer\.

**Acceptance evidence:** Business\-approved results; enabled\-path access and payload checks; working correlation, health monitoring, basic alerts, support, and estimated usage costs\. Without approved real\-data access, label the result a synthetic demonstration, not an operational pilot\.

**Deferred:** Persistent chat history, preference settings, self\-service template editing, and scheduled delivery\.

### Q2 2027 — Make the product useful every day

**Target outcome:** Users can resume useful work, and content owners can publish reusable questions without application\-code changes\.

Users can find saved conversations, reopen permitted content, save questions, and choose **Run again** for fresh results\. Reopening history does not automatically execute queries\. Users can explicitly save presentation preferences, inspect them, change them, or remove them\. A new conversation uses approved preferences without silently inheriting old analytical filters\.

A content owner can define a question’s wording, permitted parameters, defaults, audience, and output layout using existing approved recipes and Registry references\. Publication requires preview, reference\-answer testing, review, and a versioned release\. New KPI definitions and joins remain outside the template editor\.

**Demo:** An owner creates “Monthly Deposit Movement” with a selectable month and authorized region, then publishes it after review\. A user saves “short summary followed by a table” and sees that preference used in a later conversation\.

**Acceptance evidence:** History isolation and reauthorization; agreed retention and deletion behavior; editable preferences; versioned template approvals; unchanged business definitions and access controls\. Administrators see team usage and allowances\. Decide the subscription or internal\-chargeback model; payment processing is not assumed\.

**Conditional optimization:** Introduce early reuse only for eligible, authorized, fresh requests\. It must not require a semantic\-plan hash before planning or force selection of a cache platform\.

### Q3 2027 — Automate recurring reporting, not business decisions

**Target outcome:** Users receive approved reports on a schedule and find useful next questions more easily\.

A report subscription records the approved template version, parameters, reporting\-period rule, timezone, recipients, and delivery channel\. Users can preview, pause, change, or cancel it\. Deliver a secure report link first, with run and delivery history\.

Check the owner’s and recipients’ access before execution and delivery, and current viewer access when the report opens\. Handle data freshness, source failure, timezone changes, retries, and incompatible template versions explicitly\. Do not send duplicate reports or silently substitute old data\.

**Demo:** Schedule a Deposits summary for Monday at 8:00 a\.m\. Toronto time\. A simulated source outage produces a visible delayed or failed run\. A recipient whose access was revoked cannot open the protected report\.

Suggestions remain within authorized analytical scope\. Repeated selections can prompt “Would you like Ontario as your default region?” but do not become permanent preferences without confirmation\. Owners see aggregated unmet demand and feedback, then review any proposed template improvement\.

**Acceptance evidence:** Reliable schedules and secure delivery; tested revocation and retry behavior; useful, consent\-based suggestions; delivery monitoring; and spending limits that distinguish interactive, scheduled, and background work\.

**Deferred:** Source\-system write\-back, autonomous actions, unrestricted attachments, and automatic production\-template rewriting\.

### Q4 2027\+ — Deliver management reports and expand selectively

**Target outcome:** Managers receive consistent reporting, and the service is supportable at its approved operating scale\.

Combine approved analyses into multi\-section reports with related charts and consistent periods and filters\. Provide permitted Excel and PDF exports with source, data date, and classification information\. Expand interactive exploration only along approved relationships\.

An additional source is conditional on business value, definitions, access, runtime readiness, and available capacity\. It must not displace completion of the core Deposits workflow\.

**Demo:** Produce a monthly management report containing balances, trends, and product comparisons\. The chat, report, charts, and export agree\. Operations can trace a delayed report to its source issue and see its associated cost\.

**Acceptance evidence:** Analytical fidelity across formats; no unauthorized export content; agreed latency, concurrency, recovery, support, and budget targets; and cost reporting reconciled to available provider charges\. Offline exports remain subject to organizational controls—do not promise automatic revocation of every downloaded copy\.

**Not committed:** Advanced forecasting, causal analysis, unrestricted cross\-source joins, Genie integration, or autonomous enterprise actions\.

---

## 3\. Decision gates

|Gate                                                   |Decision                                                    |Required evidence                                                                                                                                                                                                                                                                             |
|-------------------------------------------------------|------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|**Gate 1 — Evidence-ready pilot**                      |Expand from selected pilot users to controlled everyday use.|Business owners accept the reference answers and pilot scope. Required privacy, architecture, data-access, and model-risk decisions are recorded. Enabled-path authorization and approved model-payload handling are demonstrated. Monitoring, support, and pilot cost evidence are available.|
|**Gate 2 — Repeatable value and operational readiness**|Expand reporting, users, or approved data scope.            |Sustained use and measurable benefit over an agreed observation period. Stable service and scheduled delivery. Working history, preference, recipient, and template-version controls. Acceptable cost and capacity. Named operations ownership and a recovery/rollback procedure.             |

Gate decisions belong to the relevant business, control, and service owners\. A passing engineering test suite, a successful deployment, or a milestone date alone does not authorize progression\. Mandatory controls for a new feature must be satisfied before that feature is released; they do not wait for the next executive gate\.

---

## 4\. Monitoring, subscriptions, and value measures

### Keep three concepts separate

|Concept                                       |Meaning                                                                                                     |Planned progression                                                                                                                         |
|----------------------------------------------|------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
|**Operating cost**                            |The cost of hosting, model use, query compute, storage, telemetry, delivery, and support.                   |Meter and estimate from Q1; attribute team usage in Q2; control scheduled and background spending in Q3; reconcile costs in Q4.             |
|**Service subscription / internal chargeback**|The organization’s chosen method of funding or charging for AskAlpha access, features, and usage allowances.|Agree the model and allowances by Q2; strengthen budget controls in Q3 and reporting in Q4. Prices and payment processing are not committed.|
|**Report subscription**                       |A user’s instruction to receive a particular approved report on a schedule.                                 |Deliver in Q3 with secure access, pause/cancel controls, and delivery history. It does not grant additional data access.                    |

### Key outcomes — the executive scorecard

|Outcome                  |What to measure                                                                                                                                             |First evidence                                                               |
|-------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
|**Answer Quality**       |Results against business-approved reference calculations; material numeric, scope, or attribution errors; reported inaccuracies; consistency across formats.|Q1 pilot; broaden as templates and reports are released.                     |
|**Adoption**             |Active and returning users, completed analytical tasks, template reuse, report subscribers, and feedback.                                                   |Q1 baseline; team and recurring-use trends from Q2–Q3.                       |
|**Control Readiness**    |Required controls with accepted evidence, unresolved blockers, access-revocation results, and review ownership.                                             |Q4 readiness register; required evidence before each release.                |
|**Reliability / Latency**|Request success, median and 95th-percentile completion time, source failures, on-time report delivery, duplicate deliveries, and recovery time.             |Request monitoring in Q1; scheduled-report monitoring in Q3.                 |
|**Cost / Value**         |Fully attributed operating cost, cost per successful analysis/report, budget variance, and measured effort saved against the manual baseline.               |Estimates in Q1; stronger attribution and reconciliation over later quarters.|

Agree numerical acceptance targets with the responsible owners before each release\. Include failed attempts and retries in cost totals, distinguish estimates from reconciled charges, and keep access denials visible as a separate control measure\. Do not claim financial savings from adoption alone\.

---

## 5\. Commitments that apply across every milestone

**Access follows the data\.** Apply current permissions to questions, protected metadata, history, suggestions, cached results, scheduled reports, and exports\. Service subscriptions and preferences never expand those permissions\. Use application authorization and the approved service identity; do not add cross\-provider user\-ACL synchronization\.

**Business meaning has one governed home\.** The Semantic Registry holds the application’s versioned semantic representation\. Recipes define approved analyses\. Templates reference those IDs and versions rather than redefining metrics\. Deterministic presentation is preferred; any AI\-assisted formatting needs explicit payload eligibility and analytical\-fidelity checks\.

**Memory is controlled\.** Session context supports the next question\. Saved history supports reopening a past conversation\. Explicit preferences support later conversations\. Keep these separate, respect retention and consent, and never treat one question as permission to save a permanent preference\.

**Improvement is reviewed\.** Aggregated usage and feedback can suggest better questions and templates\. Only an approved release changes production content; runtime analytics do not rewrite it\.

**Scale remains bounded and provider\-independent\.** Cache eligible results, plans, matches, or response payloads—not the approximately 5 TB source dataset\. Keep provider\-specific execution outside the core\. An optional new source, cache platform, or future provider requires its own qualification\.

**Scope remains read\-only\.** Scheduled reports automate analysis and delivery, not business actions\. “Autonomous enterprise” is not a committed release outcome in this product definition\.

---

## 6\. Decisions and dependencies to close

|Decision / dependency                                                                                                       |Responsible role to confirm                            |Needed for                                     |
|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|-----------------------------------------------|
|Pilot questions, metrics, datasets, reference answers, and personas                                                         |Deposits business and data owners                      |Real-data pilot acceptance                     |
|Enterprise entitlements, governed access, metadata integration, query-serving performance, and runtime identity/connectivity|Enterprise platform, security, data, and service owners|The affected protected and operational paths   |
|Required privacy, architecture, and model-risk decisions                                                                    |Relevant approval owners                               |Release of the affected data/model capabilities|
|Conversation retention, deletion, and preference consent                                                                    |Product, privacy, records, and security owners         |Persistent history and personalization         |
|Template creator, reviewer, and publication responsibilities                                                                |Product and business content owners                    |Owner-created templates                        |
|Report recipients, channels, freshness, and sharing rules                                                                   |Product, business, privacy, and service owners         |Scheduled reports and exports                  |
|Service targets, support responsibilities, budget, and subscription/chargeback model                                        |Product sponsor, operations, and finance               |Everyday use and operating-scale acceptance    |
|Delivery start and available team capacity                                                                                  |Product and delivery leads                             |Calendar commitments                           |

An external dependency blocks only the affected capability\. If capacity is constrained, reduce question coverage, report layouts, channels, or additional sources—not access controls, answer validation, essential monitoring, or cost visibility\.

---

## 7\. Source alignment and planning notes

This executive view adapts the supplied manager template’s structure: current status, three phase bands, five calendar columns, four workstreams, two decision gates, and five outcome measures\. It does **not** adopt the template’s approval/completion claims or its autonomous\-action scope\.

### Source\-to\-calendar mapping

|Existing product roadmap                                               |Proposed executive calendar                   |
|-----------------------------------------------------------------------|----------------------------------------------|
|Preparatory readiness and open decisions                               |Q4 2026                                       |
|Quarter 1, months 1–3: trusted Deposits pilot                          |Q1 2027                                       |
|Quarter 2, months 4–6: everyday use and owner-created templates        |Q2 2027                                       |
|Quarter 3, months 7–9: scheduled reports and controlled personalization|Q3 2027                                       |
|Quarter 4, months 10–12: management reporting and controlled expansion |Q4 2027; further approved expansion thereafter|

**Source documents reviewed:**

- [AskAlpha Product Definition — English, version 1\.1](https://github.com/hesam-hakimi/dcm/blob/a71ee873ce0fc639844791b456cdf4fff4354879/docs/askalpha/PRODUCT_DEFINITION_EN.md), 13 October 2026\. Product scope, users, templates, session context, history, preferences, suggestions, scheduled reports, monitoring, costs, and controls\.
- [AskAlpha Quarterly Product Roadmap — English, version 1\.1](https://github.com/hesam-hakimi/dcm/blob/a71ee873ce0fc639844791b456cdf4fff4354879/docs/askalpha/QUARTERLY_PRODUCT_ROADMAP_EN.md), 13 October 2026\. Four\-quarter feature sequence, acceptance criteria, exclusions, and dependencies\.
- User\-supplied **“AskTD Executive Roadmap”** image\. Presentation/layout reference only; not independent evidence of completion or approval\.

**Verified documentation baseline:** Repository `hesam-hakimi/dcm`, branch `xdoc`, commit `a71ee873ce0fc639844791b456cdf4fff4354879` at the time of this review\. This is a documentation reference, not the AskAlpha application’s runtime or deployment commit\.

**Proposed additions in this view:** Calendar mapping, executive phase names, readiness column, gate packaging, and the executive scorecard\. These organize the existing product plan; they do not authorize implementation, deployment, feature activation, new data access, or scope expansion\.
