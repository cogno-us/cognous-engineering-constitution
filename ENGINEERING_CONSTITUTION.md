# Cognous Engineering Constitution

## Purpose and standing

Engineering is the disciplined conversion of proposals into reliable, accountable and legitimately accepted results. This constitution governs that process: what may be attempted, who may decide, how claims are supported, and how changes remain inspectable and revisable.

The constitution is **secular, static and technology-neutral**. It supplies general engineering obligations, not a project architecture, a particular software implementation or a work authorization. The [foundational principles](PRINCIPLES.md) explain its rationale, and the [adoption and amendment rules](ADOPTION.md) govern its applicability and evolution. The [orchestration guidance](ORCHESTRATION.md) describes coordinated practice without adding authority.

Use the exact adopted revision. Controlling law, security controls, competent authority, and valid local obligations retain their precedence. Publication, a technical merge, this text, or a worker instruction cannot confer otherwise missing access, spending, external-effect, deployment, release, certification or adoption authority.

## Responsibilities and boundaries

**Contributors and implementation owners** reconcile obligations, design and build changes, validate their own work, and deliver a source-identifiable candidate. **Independent qualification** establishes and applies expectations that are not retrofitted to a candidate's observed behavior. **Certifiers and adopting authorities** make their respective decisions only where their identity, scope and governing rules permit. **Integrators** establish canonical technical state only within their delegated power.

These functions can sometimes be performed by the same actor, but only where the controlling requirements and risk permit. Assigning a title to a person, agent or service does not manufacture independence or authority. Coordination of work is different from inspection, certification, adoption and deployment.

Every substantive assertion must distinguish authoritative source, relayed source, direct observation, interpretation and inference. Preserve exact source and configuration identities and do not collapse distinct identifier namespaces. An unavailable controlling text cannot be replaced by a plausible summary.

## Engineering articles

The articles are expressed as obligations, prohibited shortcuts and ways to examine compliance. They are grouped conceptually in the explanatory sections that follow; their stable identifiers are retained for precise reference.

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

## How the articles work together

### 1. Proposals, contracts and canonical change

**EP01–EP03 and EP19** require reuse before invention, the minimum sufficient intervention, and contracts before implementation. A proposal must identify its controlling source, intended effect, legitimate reliance boundary, acceptance criteria and integration authority. A local demonstration, signed artifact or successful merge does not itself establish organizational adoption. The right to generate an alternative is broader than the right to make it canonical.

**EP15, EP17, EP21 and EP22** balance decisiveness with evolution. Work should be small enough to inspect, integrate and where possible reverse; changes must not silently violate obligations on which others legitimately rely. Internal architecture may change freely inside those commitments. Otherwise, an authorized compatibility or migration decision is required.

A canonical decision remains operative until lawfully superseded. Reopening requires an identified authority, controlling source, reasons, scope, version and qualification implications. Material new evidence, demonstrated inconsistency, a security or constitutional defect, or explicit competent instruction can justify reconsideration. Mere preference does not. Preserve material alternatives, objections and adverse records proportionately and lawfully. Reversal of a decision or configuration cannot undo an already committed external effect; any compensation needs distinct authority.

### 2. Delegation, coordinated work and accountability

**EP09–EP11 and EP20** support productive parallel engineering without distributing canonical authority indiscriminately. Delegate concrete, bounded work to identifiable actors by role, domain, action, context, time and limits. Serialize conflicting changes to canonical contracts, shared schemas, admission conditions or mutable state; parallelize independent investigations and implementation tasks against fixed inputs.

Workers and coordinators should resolve routine authorized issues, manage dependencies and surface genuine decision points, but cannot infer permission for an architectural change, additional expense, security exception or release from their technical capacity. Delegation does not permit a subordinate to enlarge its authority or transfer it onward silently. Track revocation and expiry where applicable.

### 3. Policy integrity, failure semantics and security

**EP05, EP14 and EP18** require faithful treatment of controlling requirements. Missing, ambiguous, unsupported or stale prerequisites must not quietly become approval or not-applicable. Fail closed according to the applicable contract without inventing a policy, grant, reason, deadline or default. Protect mandatory governance invariants through the mechanisms appropriate to the system's risk.

Where policy and rules are configurable, their governing authority, scope, versions, provenance, applicability and change process must remain explicit. Policy changes, evaluator changes and configuration updates cannot silently waive binding checks or create a competing, unaccountable route to decision authority. Implementations may use authenticated files, registries, typed evaluators, deterministic software or other adequate forms; **no particular rules engine, storage technology or canonical kernel is constitutionally required**. If data and evaluator logic are separated, preserve completeness, authenticity, unambiguous applicability, defined failure treatment and authorized activation.

Historical decisions retain their original governing rule/configuration identities and observed outcomes. Evaluation under changed policy is a new, distinct event, not retroactive amendment. Material governance-rule changes require source-based impact assessment, relevant adverse and negative controls, and independent assessment where warranted. Likewise, source inspection, green CI and local simulation are not substitutes for enabled-path security assurance.

### 4. Evidence, qualification and accountable certification

**EP04, EP06–EP08, EP16 and EP23** require that consequential claims follow the evidence rather than the other way around. Preserve original findings, failed runs, material alternatives, decisions and supersession paths. Reproduce exact behavior where feasible; for nondeterministic systems, preserve the governing context and attributable transitions needed for bounded reconstruction.

Independent expectations should be recorded before candidate acceptance. Implementation does not grade itself, and a qualifier cannot adjust frozen expected results to make a candidate pass. Qualification, responsible certification and technical integration are distinct functions. Machine generation and nominal human review alone establish neither competence nor authority.

Keep lifecycle states distinct: proposed, documented, implemented, developer-tested, independently qualified, integrated, deployed and production-qualified. A result transfers only to the exact sources, profiles and conditions actually evaluated. Measure the time to independently accepted outcomes where observable; code volume, elapsed commit intervals and the number of workers are not substitutes for measured effort or value.

### 5. External commitments, measurements and risk

**EP12, EP13 and EP21** prohibit claims that cheaper, faster or simplified alternatives preserve quality when mandatory governance, reliability or compatibility floors have not been demonstrated. Measure costs, latency, refusals, failures, retries, resources and acceptance before making optimization claims. An internal technical improvement is not justified by silently degrading a legitimate external commitment.

## Risk-proportionate review and allocation

Classify changes by the highest applicable risk. Review remains proportionate to consequences and does not displace governing obligations, required checks or decisions expressly reserved to competent authority.

| Tier | Scope | Required treatment |
|---|---|---|
| Tier 1 — routine | Documentation, metadata and minor nonsemantic CI. | Worker self-validation, required automated checks and orchestrator integration. No independent agent review or post-merge audit. |
| Tier 2 — bounded ordinary engineering | Ordinary bounded implementation outside Tier 3 boundaries. | Developer regressions, CI and applicable independent qualification. Add code review only for a concrete identified risk. |
| Tier 3 — critical | Admission, authority, atomic state, trust, authentication, negative-evidence custody, oracle/acceptance or security. | One focused independent verifier when needed for the identified risk; retain applicable Tier 2 gates. No blanket multiple reviewers. |

Maximize useful nonconflicting work against exact pins; serialize shared canonical mutations. Assign concrete disjoint deliverables, not status-only turns. Avoid duplicate manifests, reviews and unchanged reruns. Coordinators consolidate concise milestone reporting in designated operational records.

Enforce adopted rules through task instructions, scope/source/ownership review and evidence-stage reporting. Do not create a new automated merge blocker merely to police prose. Automated enforcement is appropriate when an adopted requirement has an objective repository-local test and a reviewed enforcement design.



## Documentation, operational records and historical custody

Engineering plans and architectural definitions should state relatively stable requirements, dependencies, intended work, acceptance conditions and completion criteria. They must not represent changing assignments, approvals, test outcomes, active blockers or progress as timeless requirements. Separate these kinds of records:

- **Normative and planned material:** controlling definitions, architecture, work programs, dependency models and acceptance requirements. Maintain these as stable, versioned statements.
- **Operational material:** current assignments, status, authorizations, reviews, check results, blockers and next actions. Keep these in designated live records.
- **Historical evidence:** dated decisions, immutable handoffs, logs, frozen expectations, qualification reports and source/configuration snapshots. Preserve them as historical observations with their original identities.

This separation must never erase inconvenient history or prohibit exact references to dated decisions, source revisions or approval prerequisites. A change in current operational status does not rewrite a frozen record. The purpose is to prevent mutable status from masquerading as enduring doctrine, not to prohibit legitimate provenance or create formalistic prose checks. Automated documentation validation is warranted only where there is an objective, reviewed rule.

## Evidence and claim discipline

Preserve original bytes and identities for failures and negative findings; use linked successors. Missing freshness evidence establishes no freshness. Required checks that are missing, disabled, unsupported or unavailable cannot become PASS or convenient non-applicability. Non-applicability requires the actual source predicate to be absent.

An ambiguous commit acknowledgment is not proof of durable storage. A receipt supplies evidence, not authority. A model's proposed action supplies neither a grant nor permission to execute. Bound historical results to exact source, profile and configuration. A bounded reconstruction result proves only that case.

Source inspection is review, not execution. Developer suites and static analysis are not independent qualification. Integration is not deployment, release or production qualification. Emulator results do not establish real-environment durability, identity or resilience. Planning completion does not establish executable readiness or authorization.

A mismatch against resolved, applicable frozen expectations is FAIL. An unresolved source/profile mapping or unavailable required evidence is BLOCKED or NOT ASSESSED; report setup and attempt status separately. Preserve independent expectations rather than changing them to make a candidate pass. Producer-supplied expected outputs are proposals, not independent certification.

Handoffs and relevant changes identify affected articles, exact evidence and bounded outcomes. Formatting-only work needs no meaningless full matrix. Adopting contexts should make these rules discoverable; applicable security and access controls remain higher priority.

