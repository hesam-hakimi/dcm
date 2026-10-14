CLUE — Build an Interactive System Explorer
Source code + information flow + database lifecycle

OBJECTIVE

Create an interactive HTML teaching application that explains how the
CURRENT CLUE implementation works.

This must connect three things:
1. The actual application source code.
2. The end-to-end movement and transformation of information.
3. The corresponding database reads, writes, relationships and state changes.

Do not merely convert a Markdown document into HTML.
Do not produce only a schema viewer or a generic architecture diagram.

The learner should be able to follow one synthetic input through CLUE and
understand, at each step:
- What information is available?
- Which module, class and function are responsible?
- What does that code do, and why?
- Which database records are read, inserted or updated?
- Which files are created, reused, published or archived?
- What permits or prevents the next step?
- What happens if execution stops here?

This is an educational artifact, not an operational dashboard and not a
replacement for CLUE.

WORKFLOW: PLAN FIRST, THEN IMPLEMENT

While in Plan mode:
- Inspect the current repository and relevant evidence.
- Produce an implementation-ready plan for the complete artifact below.
- Identify the actual source locations, proposed files, page structure,
  scenario model, implementation sequence and verification approach.
- Resolve questions from the repository before asking the owner.
- Surface genuine contradictions or missing evidence.
- Do not claim to have built or tested the page.

After the owner starts implementation:
- Implement the reviewed plan using one sequential implementation writer.
- Deliver a working interactive page, not just another design document.
- Preserve all boundaries and verification requirements in this prompt.


1. SCOPE AND SAFETY BOUNDARIES

This is documentation and educational-UI work only.

Do not:
- Change CLUE application behavior, database schemas or business rules.
- Modify provider integrations, retry policies, recovery behavior,
  identity rules, simulation defaults or compression settings.
- Change YAML, CI/CD, installer behavior or deployment packaging.
- Connect to Symcor, Tungsten, NAS, servers or any live service.
- Open, modify, copy or upload real application state databases.
- Read secrets or embed real account numbers, transaction identifiers,
  customer data, internal endpoint values or credentials.
- Add a runtime web server or API to CLUE.
- Commit, push, deploy, reset, clean or discard existing work.

Record the current repository, branch, HEAD and existing working-tree
changes before implementation. Preserve unrelated changes.

Keep all educational scenarios entirely inside the browser using
synthetic data. The page must never execute operational commands.

Place a visible notice in the interface:
“Synthetic teaching model — no live system access.”

The tutorial's browser simulation is independent of CLUE's actual
simulation configuration. Do not modify that configuration.


2. ESTABLISH THE ACTUAL SOURCE OF TRUTH

Inspect the latest files available in the current workspace.

Start with these candidate references and verify their actual locations:
- Deliverables/docs/CLUE_STATE_DATABASE_GUIDE.md
- The current environment/configuration guide
- The application entry point and orchestration flow
- batch.py, app.py, zip_delivery.py and state.py
- Relevant coordinator, recovery, provider, image-processing,
  workbook-generation, publication and archive implementations
- Relevant tests and operational documentation

These names are navigation hints, not permission to assume that every
file, symbol or behavior still exists.

Trace actual callers and callees. Read relevant function bodies and tests.
Do not derive implementation behavior from filenames or screenshots alone.

Build a compact evidence map:
Teaching topic -> source file -> symbol -> relevant test/document.

Distinguish:
- Behavior implemented in the inspected code.
- Behavior required or described by documentation.
- Behavior exercised by inspected tests.
- Behavior that remains unverified.

When code, tests and documentation disagree:
- Record the discrepancy.
- Explain the observed implementation accurately.
- Do not silently describe a discrepancy as approved behavior.
- Do not fix application code as part of this task.

Record the source snapshot in the tutorial:
- Branch and commit.
- Inspection timestamp.
- Whether relevant files had uncommitted changes.
- File fingerprints or equivalent traceability for embedded excerpts.

Do not imply this snapshot is identical to a deployed environment.


3. DELIVERABLE AND FILE ORGANIZATION

Create a small, maintainable documentation artifact under the repository's
existing documentation structure.

Suggested location, subject to actual repository conventions:
Deliverables/docs/interactive/clue-system-explorer/

Primary deliverable:
- index.html

Supporting engineering documentation:
- A short English README describing how to open, maintain and verify it.
- A compact source-evidence and discrepancy record.

Prefer a self-contained index.html with embedded CSS, JavaScript and
teaching data.

Requirements:
- It opens directly from the filesystem using file://.
- No application startup is required.
- No runtime build step is required for the learner.
- No CDN, remote font, analytics or network dependency.
- No runtime fetch of repository files or external JSON.
- No database engine, backend or live SQL execution.
- No new dependency in CLUE's application runtime.

An optional documentation-only generation/verification helper is acceptable
if it materially improves source-excerpt accuracy. It must not import or
execute CLUE modules with side effects.

Do not interpret this request as requiring integration into CLUE's runtime
or deployment process.


4. CORE EXPERIENCE: SYNCHRONIZED LEARNING WORKBENCH

The central feature must be a synchronized step-by-step explorer.

Selecting a stage, function, record or timeline step must update the
related views together.

A. FLOW AND EXPLANATION VIEW

Show a clickable end-to-end flow.

For the selected stage, explain:
- Purpose in plain language.
- Inputs and outputs.
- Preconditions and decisions.
- The reason this stage exists.
- Its relationship to the preceding and following stages.

Highlight the active stage and its relevant connections.

B. ACTUAL SOURCE-CODE VIEW

Show a small, relevant excerpt from the inspected source:
- Repository-relative file path.
- Class/function name.
- Accurate line range for the recorded snapshot.
- Highlighted lines relevant to the current action.

Explain the code progressively:
- A simple “What this does” explanation.
- Expandable technical detail explaining important conditions,
  parameters, calls and return values.

Clearly distinguish:
“Actual source excerpt”
from
“Simplified teaching pseudocode”.

Never present invented pseudocode as CLUE source.

Embed the excerpts so the page works offline. Label them as a source
snapshot, not a live view of the repository.

Do not dump entire source files into the interface.

C. DATABASE AND FILESYSTEM VIEW

For the current step, show:
- The relevant database and table.
- The records read.
- The records inserted or updated.
- Before/after values for changed fields.
- Identity keys linking the records.
- Files created, referenced, reused or moved.

Visually distinguish:
- Database state.
- Filesystem artifacts.
- In-memory execution state.
- External-provider state.

Show when the selected step makes no database change.

Where evidenced by the source, identify transaction/commit boundaries.
Do not imply that a database transaction also atomically commits a file
operation or an external provider request.

All displayed SQL and database operations must be educational.
No interface control may execute real SQL or shell commands.

DESKTOP AND MOBILE

On desktop, present the flow/explanation, code and data views together.
On narrow screens, stack them or provide accessible tabs while preserving
the selected stage.

The page must be a teaching tool, not a wall of tiny diagrams.


5. GUIDED WALKTHROUGH AND INTERACTIVE CONTROLS

Create one complete synthetic end-to-end walkthrough using a small dataset.

Choose an example that can explain:
- An input file containing multiple rows.
- One row associated with multiple documents.
- A document associated with more than one input row, where supported.
- Front/back images.
- Extraction results.
- Output creation and publication.
- Final archive/cleanup decisions.

Use clearly fictional identifiers such as DEMO-ROW-001 and DEMO-DOC-001.

Trace the actual implemented stages, including where applicable:
- Input discovery and admission.
- ZIP inventory and extraction.
- Loose-file admission.
- Identity and content validation.
- Delivery ownership.
- Source-row registration.
- Work-item creation.
- Credit and Debit discovery paths.
- Document and image retrieval.
- Image preparation and extraction.
- Association/result persistence.
- Workbook generation.
- Output verification and publication.
- Acknowledgment, where actually implemented.
- Archiving and source-deletion evidence.

Do not force an inapplicable ZIP stage onto a loose-file scenario.
Verify the current archive/compression configuration and distinguish
archiving from compression. Do not assume compression is always enabled.

Provide:
- Previous step.
- Next step.
- Play / Pause.
- Reset scenario.
- Direct selection of a timeline step.
- A visible explanation of the current action.

Add an educational “Interrupt and restart” interaction at selected
checkpoints. It must show which simulated state persists and which
in-memory state is lost.

Backward navigation is a teaching rewind of synthetic snapshots,
not an assertion that production database changes can be undone.

Switching scenarios must reset all relevant views and timers.
Repeated playback must be deterministic.


6. FAILURE, RESTART AND RECOVERY SCENARIOS

Implement selectable scenarios, verified against current code:

A. Successful processing and publication.

B. Interrupted execution followed by safe continuation without repeating
   already completed work.

C. A retryable provider failure with attempt counting, backoff and eventual
   retry-budget exhaustion.

D. An external submission whose outcome is unknown.

E. Duplicate/re-delivered input:
   - Same relevant identity and same content.
   - Same filename but different content.
   Explain the actual current identity algorithm, not an assumed
   filename-only or timestamp-only rule.

F. Ownership contention and stale-worker fencing.

G. Missing/unusable artifacts or controlled recovery, where the inspected
   implementation supports these paths.

Reuse the same teaching engine rather than implementing separate pages.

For every scenario explain:
- What happened.
- What the system knows.
- What remains unknown.
- Which records provide evidence.
- Which actions are allowed next.
- Which actions are deliberately blocked.
- Whether continuation is automatic or requires explicit recovery.

Important distinctions to verify and teach:
- Technical completion versus business success.
- An unfinished discovery operation versus a confirmed zero-result search.
- Retryable failure versus unknown external outcome.
- pending_technical versus failed versus held_unknown, if these are the
  current state names.
- Retry allowance versus erasing attempt history.
- A published output versus an acknowledged output.
- A file being absent versus evidence of authorized deletion.

Do not teach “retry every error”.
Do not teach “delete the state database to start over”.
Do not invent a successful reconciliation when the source provides no
implemented mechanism for it.

If a scenario cannot be fully verified, label the unsupported portion
explicitly instead of presenting it as implemented.


7. INTERACTIVE DATABASE AND RELATIONSHIP EXPLORER

Inspect and explain every table actually present in the current schemas.

The supplied guide identifies these candidates:

Inventory database:
- zip_delivery
- zip_member

Processing-state database:
- delivery
- source_item
- work_item
- association
- image_artifact
- page_result
- acquisition_origin
- search_provenance
- stage_attempt
- output_package
- coordinator

Verify this list rather than hard-coding a historical table count.

Clicking a table must show:
- What one row represents.
- Why the table exists.
- Important columns and keys.
- Actual constraints and indexes relevant to understanding it.
- Synthetic example records.
- Functions that read or write it.
- Related walkthrough stages.
- State transitions, where applicable.

Render an interactive relationship map with distinct visual styles for:
- Database-enforced foreign keys.
- Application/conventional relationships.
- Cross-database computed links.
- File references.

Explain the bridge between the two databases using the actual identifier
construction logic.

Provide a “Trace this output to its input” interaction following the
verified identifiers and relationships.

Display separate counters for:
- Input rows.
- Associations.
- Unique documents.
- Images.
- Output packages/versions.

Do not conflate these counts.

Include a small set of predefined read-only investigation examples,
such as outstanding work, unresolved attempts and acquisition origin.
Display their results against synthetic teaching data only.

Explain provenance, lease/fencing, image reuse, schema evolution,
storage limitations and backup/reconciliation responsibilities from
the inspected evidence. Do not overstate local durability or remote
exactly-once guarantees.


8. TEACHING STYLE, LANGUAGE AND ACCESSIBILITY

The learner is technically literate but wants the system explained clearly,
without first having to understand every internal class or database field.

Use progressive disclosure:
- Plain-language explanation first.
- Technical detail second.
- Source code and database detail available on demand.

Provide a searchable glossary for concepts such as delivery, member,
source item, work item, association, lease, fencing, retry, reconciliation,
provenance, publication and archive.

Use Persian for user-facing teaching narration and explanations, with
proper right-to-left layout.

Keep source code, SQL, identifiers, code comments, tests, README and
engineering evidence records in English, with left-to-right code blocks.
Do not translate actual symbols.

Read and respect mandatory repository language instructions. If they
also prohibit Persian instructional UI text, explicitly flag the conflict
in the plan rather than silently changing project policy.

Use:
- Readable typography and generous spacing.
- Keyboard-accessible controls.
- Visible focus states.
- Text labels, not color alone, for states and relationships.
- Responsive layouts.
- Reduced-motion support.
- A clear legend.
- Small knowledge checks with explanations, not just correct/incorrect.

Avoid decorative complexity that makes the information flow harder to
understand.


9. IMPLEMENTATION AND VERIFICATION

Keep the teaching model data-driven:
- Stages.
- Source references.
- Table definitions.
- Synthetic records.
- Scenario steps.
- Expected before/after changes.
- Narrative explanations.

Do not scatter scenario logic and copied descriptions throughout the DOM.
Do not reimplement the production orchestration engine in JavaScript.

Use deterministic educational snapshots or a small pure state-transition
model. Make clear that it illustrates verified behavior rather than
executing CLUE.

Render source excerpts and synthetic values safely as text.

Verify at least:

SOURCE ACCURACY
- Referenced files and symbols exist in the inspected snapshot.
- Embedded excerpts match their recorded source locations.
- Every major stage has source evidence.
- Schema fields, relationships and state names match inspected code.
- Discrepancies are visible and are not silently resolved by invention.

INTERACTION
- Next, Previous, Play, Pause, Reset and direct stage selection work.
- Scenario changes do not leave stale records or highlights.
- Repeated playback produces identical synthetic results.
- Code, explanation and database views remain synchronized.
- Restart demonstrations preserve the intended synthetic durable state.
- Counters remain consistent with the displayed records.

SAFETY
- No network calls.
- No live database access.
- No secrets or real business data.
- No operational commands executed.
- No modification of application/runtime files.

USABILITY
- The page opens directly through file://.
- Essential features work offline.
- No JavaScript errors in exercised interactions.
- Keyboard navigation and narrow-screen layouts work.
- Code/SQL remain readable in the mixed RTL/LTR layout.

Use available browser/DOM testing tools and existing repository tooling.
Do not add unapproved dependencies to CLUE merely to test the tutorial.

Report exactly what was exercised and what was not.
Static checks are not a substitute for browser interaction tests.
Tutorial tests do not establish application or production readiness.


10. REQUIRED OUTPUTS

PLAN PHASE

Return:
- A concise evidence-backed understanding of the current system.
- The proposed page layout and file locations.
- A source-to-teaching coverage map.
- The walkthrough and scenario definitions.
- The bounded implementation sequence.
- The verification plan.
- Genuine unresolved questions or source discrepancies.

IMPLEMENTATION PHASE

Deliver:
- The working offline interactive HTML tutorial.
- The short maintenance/opening README.
- Source-snapshot and evidence metadata.
- Relevant tutorial verification checks.
- A final changed-file summary.
- Exact local opening instructions.
- Actual test commands and observed results.
- Known limitations and any unverified behavior.

Do not claim completion with placeholder panels, disconnected diagrams,
invented source snippets or nonfunctional controls.

SUCCESS CRITERION

A learner can select any important stage of CLUE and understand:

“This is the information entering the stage.
This is the actual code responsible.
These are the records and files it reads or changes.
This is the reason for those changes.
This is what allows the next step.
This is what happens if execution fails here.”

Deliver that connected learning experience without changing CLUE itself.
