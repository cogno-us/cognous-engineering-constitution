# Orchestration, roles and task compilation

Sources: `ORCHESTRATION.md`, `ENGINEERING_COMPLIANCE_ADDENDUM.md` (proposed), `ORCHESTRATOR_PROMPT_ENGINEERING_ADDENDUM.md` (proposed). **Use proposed compilation prescriptions only when adopted or as an expressly requested nonbinding format.**

## Eight-field assignment contract

One self-contained packet, in order:
1. **Identity** — work package, actual role, exactly one primary archetype with plain operational definition, repository, exact base/source SHA, target.
2. **Authority** — originating decision, authorized result/actions, security, finance, integration and deployment restrictions.
3. **Ownership** — one designated canonical writer, writable paths, read-only/protected paths, disjoint parallel writers.
4. **Inputs** — governing project plan, adopted constitutional revision, frozen contracts, interface and configuration pins, original failures, dependency identities.
5. **Acceptance** — independent risk tier and rationale, falsifiable success and negative/boundary/adversarial conditions, verified commands or `DISCOVER BEFORE EXECUTION`, prior evidence and justified reuse, skipped work, independent qualification boundary, CI Scope Declaration.
6. **Delivery** — PR/branch, exact final head, raw evidence, negative findings, bounded handoff and observable result.
7. **Boundaries** — scope exclusions, stop/escalation gates, no unauthorized edits, finance/effect/release guards.
8. **Governance** — exact adopted source and companion statuses, required canonical article rows (verbatim Required behavior and Prohibited shortcut), each followed by a separate path/source/decision-specific **Binding**.

The companion schema is `schemas/orchestrator-assignment-v1.schema.json`; fetch the actual JSON Schema before claiming schema-validity. No ninth top-level field. Use no invented source paths or SHA placeholders in dispatchable output. A nonexecuting draft may label `UNVERIFIED` clearly.

## Role versus archetype

`implementation_owner`, `independent_qualification_owner`, `orchestrator`, or another actually delegated role is the **role** axis. The single selected **primary task archetype** axis is independent of it:

| Archetype | Immediate deliverable | Default exact CA slice | Entry / exit gate |
|---|---|---|---|
| A architecture/contract | Complete shared inventory, reconcile invariants, decide schema, policy/refusal, interface, freeze common boundary | CA01, CA03, CA04, CA18, CA21 | Source, consumers and architecture authority known → versioned contract, compatibility plan, accepted freeze/decision or blocker |
| B scoped implementation/migration | Smallest implementation against frozen contract | CA02, CA04, CA05, CA09, CA15 | Design and writable ownership verified → exact head, affected tests, rollback, evidence |
| C defect/CI/regression repair | Reconfirm existing failure, preserve original, fix smallest cause or no-op if fixed | CA02, CA04, CA06, CA07 | Actual counterexample/baseline → evidence-backed corrected/no-op result, positive/negative checks |
| D independent qualification | Apply independently owned protocol and oracle to frozen subject | CA04, CA06, CA07, CA08, CA23 | Qualified independent owner + frozen subject/oracle → bounded verdict, raw adverse evidence, no self-certification |

Never choose a tier solely from archetype. A is commonly T2/T3, B T1–T3, C T0–T3, D prescribed T4 (a changed oracle/protocol may itself be T3). Add other relevant articles without rewriting canonical table cells. A builder performing testing does **not** thereby become an independent qualifier. Split contradictory ownership and duties into separate packets.

## Clause injection fidelity

- Retrieve and verify *exact locally adopted source*. Do not copy a convenient newer public `main` into a frozen project adoption.
- For each default article ID, copy **Required behavior** and **Prohibited shortcut** exactly from canonical article table. The bundled [article catalog](constitutional-articles.md) reproduces observed text but is not itself evidence of adoption.
- Add a separate **Binding**: concrete file, pin, decision, invariant, refusal, check or authority for that task. A generic reference is insufficient.
- Compare selected article IDs, source bytes and binding completeness using actual validator when one is available. Distinguish textual review from mechanical equality.
- Cross-field checks: valid revision/adoption, exact existing SHAs, nonoverlapping writable/protected paths, no parallel canonical writers, paid execution OFF absent approval, merge/deploy flags backed by explicit authority, no evidence transfer without applicability, no substitute for independent oracle.
- A missing required fact becomes a blocker, not a permission to invent a grant, source or path. `DISCOVER BEFORE EXECUTION` is a preparatory instruction, not an accepted test result.

## Orchestrator operating loop

1. Resume from current project plan, repo instructions and latest competent decisions; do not rely on chat-only status.
2. Query actual workers/PR heads/CI/reviews/evidence using supported tools; verify status and deduplicate tasks, events and completed work.
3. Recompute critical path, dependencies, owner and ready queue; track next three executable work packages, capabilities, prerequisites and uncertainty.
4. Dispatch nonconflicting authorized work with exact pins and bounded ownership; separate architecture owner, builders and independent qualifier.
5. Inspect accepted candidates through developer review, required independent qualification and integration authority gates.
6. Record precise stage, source/head, timestamps, blocker owner, next action and evidence in **existing** telemetry, not a new duplicate dashboard.
7. Report meaningful milestones, changes and operator decisions; don't poll pointlessly, claim background monitoring without configured scheduler or solicit continuation for routine authorized work.

## Batch architecture invariant

For many migrations sharing a schema, evaluator, contract or admission path, inventory *all eligible items* before editing. Evaluate common architecture-first versus independent incremental work on actual shared-mutation cost. Where a common boundary changes repeatedly: **A** reconcile full inputs and freeze shared schema/refusal/contract with one writer → **B** build/test common evaluator, loader and negative fixtures → **C** migrate independent items against pinned boundary with disjoint owners. Here A/B/C denote batch stages, not necessarily assignment archetypes. An item cannot quietly mutate frozen shared contract; file a source-backed compatibility blocker with smallest alternatives, impact on evidence and scoped architect decision. Allow controlled reopening for genuine requirements, preserve old evidence. Individually test migrated source-to-registered-data equivalence, refusal and changed callers/legacy dispatch. Shared-boundary evidence reuse requires identical relevant contract/evaluator/dependencies/environment **and** no new reachable caller, state or configuration behavior.

## Parallel work and resources

Parallelize source inspection, docs, independent fixture preparation, disjoint components and pinned adapter work. Serialize canonical contract, schema, state, admissions, shared evaluator edits, integration, transactions, locks and migrations with one designated writer. Avoid duplicate jobs, unnecessary new workers, idle-work theater or invented worker launches. Add capacity only for actual ready, authorized independent work after assessing setup and coordination cost. Never request secrets in chat or create paid resources implicitly. Environment capability and execution authority are separate.

## Autonomous execution and actual blockers

Finish routine authorized implementation → focused validation → debug → revalidation → eligible review/handoff without requests for permission at each trivial step. Resolve routine CI, packaging, test-path and link problems. Escalate one precise decision packet for genuine architecture, legal, security, contract, payment, external effect, release or independence issues. Continue unaffected work. Distinguish source-resolved vs engineering-choice vs operator decision vs deferred. A service error is not proof of an architectural blocker; verify whether actions were accepted before replaying.

## Evidence-gated integration

Before any eligible merge verify: scope and authority; exact current head and tests; frozen contract compatibility; prescribed developer and independent evidence; protected CI, code review and critical risk controls; no new unapproved finance/effects/release powers. Use expected-head safeguard when supported. Changed head requires re-evaluating affected evidence. Verify actual merged identity and content, then update existing telemetry. Merge remains distinct from organizational adoption, qualification, release and deployment. Respect reserved merge approval.

## Operational reporting and economics

Report exact task/source, role, authority, blockers, next action, independent oracle readiness, evidence status, quality, completion timings. Measure authorization-to-independently-qualified outcome, first-pass acceptance, rework, queue/blocked intervals, operator burden. Do not substitute worker-hours guessed from commit timestamps, PR count, token count or concurrency. For economic claims report measured tokens/calls/provider rate/compute/storage/retries/latency/acceptance and cost per independently accepted deliverable, with floors. Counterfactual projections are labeled estimates; synthetic one-case saving is not general proof.
