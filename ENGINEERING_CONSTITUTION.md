# Cognous Engineering Constitution

## Scope, authority and roles

EP01–EP23 and DOC-01 set general engineering discipline under the [foundational principles](PRINCIPLES.md). They are static, secular guidance, not the architecture or implementation plan of a particular system. Applicability depends on an authorized adoption of an exact revision. Apply platform and organizational security controls, explicit operator/task authority, the project's controlling architecture and recorded interpretations, these engineering articles, and applicable repository contracts. Repository prose cannot grant missing access, spending, external-effect, deployment or release authority.

The **implementation owner** reconciles contracts, implements the product and supplies developer validation and exact-source handoffs. **Independent qualification** owns expected outcomes, fixtures, oracles and qualification evidence. Implementation cannot self-certify independent qualification; qualification cannot fit its oracle to observed implementation behavior. Separately owned execution or infrastructure capabilities retain their own authority and qualification boundaries.

Use exact source and configuration identities. Preserve distinctions between direct source access, relayed source, observation and inference. A derived summary cannot replace unavailable normative wording. Preserve project terminology and distinguish unrelated identifier namespaces.

## Engineering articles

The seven [foundational principles](PRINCIPLES.md) inform the duties below; the [adoption rules](ADOPTION.md) govern their revision and applicability.

| Article | Required behavior | Prohibited shortcut | Validation |
|---|---|---|---|
| EP01 — Reuse Before Build | Inspect and reuse qualified, versioned components. | Duplicate an owned capability for convenience. | Reuse/source crosswalk. |
| EP02 — Minimum Sufficient Implementation | Deliver the smallest complete authorized capability. | Speculative architecture, infrastructure, dependencies or scope expansion. | Authorization-to-diff review. |
| EP03 — Contract Before Code | Identify the controlling source, external reliance boundary, duties, expected acceptance and the authority by which a proposed change may acquire canonical standing. | Start against an unnamed or mutable contract. | Entry prerequisites. |
| EP04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. | Independent pre-acceptance source/pin record. |
| EP05 — Fail Closed Without Inventing Policy | Apply specified conservative treatment and expose missing semantics. | Invent a cause, grant, floor, deadline, mapping or default. | Negative controls and source audit. |
| EP06 — Preserve Original Evidence | Retain consequential decision ancestry, rejected alternatives, objections, adverse findings and supersession where legitimately relevant, subject to privacy and retention limits. | Delete, relabel, overwrite or silently rescore failures. | Immutable predecessor evidence. |
| EP07 — Exact-Source Reproducibility | Bind claims to exact source, configuration, governing context and transition evidence; reconstruct authoritative pathways when deterministic execution replay is impossible. | Transfer a pass across revisions. | Exact-head manifest and review. |
| EP08 — Independently Qualified Delivery | Optimize authorization-to-independently-qualified outcome; distinguish lifecycle evidence. | Treat PR counts, green CI or documents as delivery or qualification. | Honest PASS/FAIL/BLOCKED and stage timing; active hours remain unknown unless measured. |
| EP09 — Safe Parallelism | Parallelize independent work against pins; serialize conflicting canonical contract, state, schema, admission and integration changes. | Concurrent conflicting authority mutations. | Ownership, pin and dependency review. |
| EP10 — Autonomous Within Authority | Finish routine authorized work and eligible corrections and merges. | Assume new architectural, financial, security or release authority. | Authorization and merge audit. |
| EP11 — Proactive Blocker Management | Check dependencies, resolve routine issues, redirect useful work and isolate one decision package. | Repeat planning loops or wait for routine continuation. | Designated blocker and next-action record. |
| EP12 — No Unqualified Degradation | Protect mandatory floors and legitimate external commitments during internal evolution; use explicit authorized compatibility transitions for justified changes. | Treat lower cost or fallback as equivalent. | Floor and negative-control evidence. |
| EP13 — Observability Before Optimization | Measure baseline cost, latency, refusal, failure, retry, resources and acceptance. | Claim improvement from projection. | Reproducible measurement protocol. |
| EP14 — Secure by Construction | Use least privilege, bounded environments and risk-proportionate assurance. | Treat CI or speculative counts as security qualification. | Enabled-path security review. |
| EP15 — Bounded Changes and Reversible Integration | Keep changes reviewable with migration/rollback and recorded irreversible authority. | Bundle unrelated architecture or erase history. | Scope and migration review. |
| EP16 — No Silent Claim Promotion | Separate proposed, documented, implemented, developer-tested, independently qualified, deployed and production-qualified. | Promote lifecycle labels or substitute them for project-defined claim statuses. | Claim/evidence review. |
| EP17 — Decision Finality and Controlled Reopening | Preserve canonical decision finality while allowing bounded, reasoned challenge and authorized supersession without erasing alternative or adverse evidence. | Reopen from preference or use finality to suppress a defect. | Decision record and reopening assessment. |
| EP18 — Governed Policy and Protected Invariants | Version, authenticate and review governance-critical policy and rule changes; protect established mandatory invariants against configuration override. | Treat unreviewed settings or evaluator changes as governing authority, weaken mandatory checks or introduce an unaccountable decision path. | Policy lineage, completeness, negative tests and proportionate independent review. |
| EP19 — Canonical Integration | Distinguish proposal, inspection, acceptance and integration; only competent authority confers canonical standing. | Treat local success, generated output or merge mechanics as organizational adoption. | Traceable adoption and integration identity. |
| EP20 — Scoped Delegation | Bind delegated work to actor, role, domain, action, context, time, limits and accountable issuer. | Treat technical capability or a subordinate assignment as general transferable authority. | Scope, expiry and revocation audit. |
| EP21 — Boundary Commitments | Preserve relied-upon external semantics or obtain an explicit authorized compatibility transition. | Introduce silent contract, rights, evidence or interface regressions through internal refactoring. | Boundary-focused regression and migration review. |
| EP22 — Reversible Possibility | Preserve proportionate lawful alternatives and permit justified challenge and supersession with ancestry. | Erase dissent or confuse decision rollback with reversal of a committed external effect. | Lineage and recovery review. |
| EP23 — Accountable Certification | Separate contribution, inspection, qualification, certification and integration according to risk and governing independence requirements. | Self-certify generated work or treat nominal human involvement as sufficient authority. | Competence, identity, independence and accountability review. |

EP17 requires authority, source, rationale, scope, version and qualification implications. Reopening is justified by new material evidence, demonstrated inconsistency, a constitutional or security defect, or explicit operator instruction. Corrections supplement rather than rewrite history. Finality must not suppress legitimate defects.

Every authorized coordinator, worker and subordinate assignment applies the adopted EP01–EP23 and DOC-01 with source pins, bounded ownership, acceptance criteria and applicable gates. Adoption creates no architectural semantics and waives no independent qualification or execution boundary.

## EP18: governed policy changes and protected invariants

Where an engineered system uses configurable governance rules, the rules and their authority, effective scope, version and provenance must be explicit, reviewable and reproducible. Mandatory invariants established by the controlling authority must not be weakened by settings, untrusted inputs, model outputs or an undeclared fallback.

Implementations may use tables, typed evaluators, deterministic code, signed configuration or other suitable mechanisms; this constitution does not mandate a registry, a universal policy language, a canonical software kernel or any specific storage scheme. If an implementation separates rule data from evaluator code, it must preserve completeness, authenticity, unambiguous applicability, failure semantics and authorized activation.

Historical evaluations retain the controlling policy/configuration and outcome identities. Reevaluation under changed policy is a new, distinguishable event, never retroactive alteration of the original. Material changes to governance logic require explicit source, impact analysis, suitable adversarial controls and independent qualification where warranted.

## Risk-proportionate review and allocation

Classify changes by the highest applicable risk. This policy replaces blanket review and worker-allocation rules without weakening architecture, qualification, automated checks, repository rules or reserved decisions.

| Tier | Scope | Required treatment |
|---|---|---|
| Tier 1 — routine | Documentation, metadata and minor nonsemantic CI. | Worker self-validation, required automated checks and orchestrator integration. No independent agent review or post-merge audit. |
| Tier 2 — bounded ordinary engineering | Ordinary bounded implementation outside Tier 3 boundaries. | Developer regressions, CI and applicable independent qualification. Add code review only for a concrete identified risk. |
| Tier 3 — critical | Admission, authority, atomic state, trust, authentication, negative-evidence custody, oracle/acceptance or security. | One focused independent verifier when needed for the identified risk; retain applicable Tier 2 gates. No blanket multiple reviewers. |

Maximize useful nonconflicting work against exact pins; serialize shared canonical mutations. Assign concrete disjoint deliverables, not status-only turns. Avoid duplicate manifests, reviews and unchanged reruns. The orchestrator consolidates concise milestone reporting in designated telemetry.

Enforce adopted rules through task instructions, scope/source/ownership review and evidence-stage reporting. Do not create a new automated merge blocker merely to police prose. Automated enforcement is appropriate when an adopted requirement has an objective repository-local test and a reviewed enforcement design.

## DOC-01 — Program/Telemetry Separation

Canonical engineering-program documents define scope, architecture, dependencies, deliverables, acceptance criteria and completion conditions. They must not encode mutable execution state: current authorization, worker assignments, PR status, CI results, qualification outcomes, blockers or operational progress. Those facts belong in designated telemetry and linked evidence.

- **Class A — canonical architecture and engineering program:** stable definitions, registers, plans, dependency graphs, profiles and qualification requirements. Keep these stateless.
- **Class B — execution telemetry:** designated controllers, operational comments, assignments, active PR/CI state, blockers and progress. These change as work proceeds.
- **Class C — immutable historical evidence:** dated decisions, handoffs, qualification reports, logs, manifests, freezes and source/configuration records. These may preserve execution facts, clearly as history rather than current program status.

DOC-01 never suppresses, deletes, rewrites or invalidates historical evidence. A source-pinned requirement, dependency, approval prerequisite or immutable provenance reference may name a PR, commit or authorization. The prohibited content is mutable status presented as canonical program definition.

DOC-01 changes no product architecture or article adoption status. Use the project's existing deterministic statelessness validation where applicable; keep ambiguous language subject to review rather than inventing a new automated prose gate.

## Evidence and claim discipline

Preserve original bytes and identities for failures and negative findings; use linked successors. Missing freshness evidence establishes no freshness. Required checks that are missing, disabled, unsupported or unavailable cannot become PASS or convenient non-applicability. Non-applicability requires the actual source predicate to be absent.

An ambiguous commit acknowledgment is not proof of durable storage. A receipt supplies evidence, not authority. A model's proposed action supplies neither a grant nor permission to execute. Bound historical results to exact source, profile and configuration. A bounded reconstruction result proves only that case.

Source inspection is review, not execution. Developer suites and static analysis are not independent qualification. Integration is not deployment, release or production qualification. Emulator results do not establish real-environment durability, identity or resilience. Planning completion does not establish executable readiness or authorization.

A mismatch against resolved, applicable frozen expectations is FAIL. An unresolved source/profile mapping or unavailable required evidence is BLOCKED or NOT ASSESSED; report setup and attempt status separately. Preserve independent expectations rather than changing them to make a candidate pass. Producer-supplied expected outputs are proposals, not independent certification.

Worker handoffs and relevant PRs identify affected articles, exact evidence and bounded outcomes. Formatting-only work needs no meaningless full matrix. Repository entry guidance should make these rules discoverable; platform instructions and access controls remain higher priority.
