# Cognous Engineering Constitution

## Purpose and standing

Engineering is the disciplined conversion of proposals into reliable, accountable and legitimately accepted results. This constitution governs that process: what may be attempted, who may decide, how claims are supported, and how changes remain inspectable and revisable.

The constitution is **secular, static and technology-neutral**. It supplies general engineering obligations, not a project architecture, a particular software implementation or a work authorization. Its seven engineering principles and 23 constitutional articles are set out together below; the [adoption and amendment rules](ADOPTION.md) govern their applicability and evolution. The [orchestration guidance](ORCHESTRATION.md) describes coordinated practice without adding authority.

Use the exact adopted revision. Controlling law, security controls, competent authority, and valid local obligations retain their precedence. Publication, a technical merge, this text, or a worker instruction cannot confer otherwise missing access, spending, external-effect, deployment, release, certification or adoption authority.

## Engineering principles — EP1–EP7

The **engineering principles** are the memorable, decision-guiding commitments of this constitution. The **constitutional articles**, designated **CA01–CA23** below, are the more specific obligations, prohibited shortcuts and validation duties through which the principles are applied. The two levels serve different purposes: principles guide judgment when circumstances vary; articles make that judgment accountable.

The distinction between broadly distributed proposal rights and narrowly scoped canonical authority runs through all seven principles.

### EP1 — Operational legibility

Consequential engineering transitions must permit competent, authorized observers to connect intent, controlling requirements, evidence, evaluation, responsible decisions, execution and observed effect. Logs alone are insufficient when they obscure causal or authority relationships. Legibility is bounded by legitimate privacy, confidentiality and security obligations.

**Expressed through constitutional articles:** CA03, CA07, CA13, CA16.

### EP2 — Canonical integration

Proposals, branches, local results and recommendations do not acquire canonical standing merely by existing or appearing correct. The system must identify its controlling state and the authorized, traceable transition by which a candidate becomes accepted. Technical integration, formal qualification, organizational adoption and deployment are distinct transitions.

**Expressed through constitutional articles:** CA03, CA04, CA17, CA19, CA23.

### EP3 — Identity-scoped delegation

Authority attaches to an identifiable actor operating within a specific role, domain, action, context and time. Competence, reputation, capability or possession of a tool does not alone confer permission. Delegation must preserve explicit scope, limits, accountability and revocation conditions. No delegate may silently enlarge or transfer its authority.

**Expressed through constitutional articles:** CA09, CA10, CA11, CA20.

### EP4 — Lineage-preserving history

Preserve the source, ancestry, transformations, decisions, negative findings and supersession relationships needed to reconstruct consequential engineering states. A correction supplements or supersedes historical records instead of silently rewriting them. Preserve governance-relevant context even when an intrinsically nondeterministic process cannot be replayed byte-for-byte. Collection and retention remain proportionate and lawful.

**Expressed through constitutional articles:** CA06, CA07, CA15, CA22.

### EP5 — Boundary commitments

Internal implementations may evolve. Legitimate external commitments—including documented behavior, interface meanings, obligations, rights and relied-upon guarantees—must remain intact or change through an explicit, authorized and reviewable compatibility process. Stability of external commitments does not imply immutability of internal interfaces.

**Expressed through constitutional articles:** CA12, CA15, CA21.

### EP6 — Reversible possibility

Maintain lawful opportunities to inspect alternatives, challenge accepted decisions and supersede canonical states on proper grounds, without treating every alternative as an authorized reopening. Preserve material rejected proposals, dissent and uncertainty where they have legitimate review value. Reverting a governance decision does not reverse an irreversible external effect; compensation or remediation requires its own authority.

**Expressed through constitutional articles:** CA06, CA15, CA17, CA22.

### EP7 — Accountable certification

Separate contribution, inspection, independent qualification, certification and canonical integration according to their distinct purposes. Machine assistance or a passing test cannot certify itself. Human presence is not sufficient unless the certifier has appropriate authority, evidence, independence and accountability. Risk and controlling requirements determine when functions must be held by distinct actors.

**Expressed through constitutional articles:** CA04, CA08, CA16, CA23.


The principles describe enduring objectives, not a requirement to adopt any particular tool, programming language, branching method, signature format or infrastructure. A signed or hashed artifact may substantiate provenance; it does not alone establish correctness or legitimate authority.

### Principle-to-article crosswalk

| Engineering principle | Primary constitutional articles |
|---|---|
| EP1 — Operational legibility | CA03, CA07, CA13, CA16 |
| EP2 — Canonical integration | CA03, CA04, CA17, CA19, CA23 |
| EP3 — Identity-scoped delegation | CA09, CA10, CA11, CA20 |
| EP4 — Lineage-preserving history | CA06, CA07, CA15, CA22 |
| EP5 — Boundary commitments | CA12, CA15, CA21 |
| EP6 — Reversible possibility | CA06, CA15, CA17, CA22 |
| EP7 — Accountable certification | CA04, CA08, CA16, CA23 |

## Responsibilities and boundaries

**Contributors and implementation owners** reconcile obligations, design and build changes, validate their own work, and deliver a source-identifiable candidate. **Independent qualification** establishes and applies expectations that are not retrofitted to a candidate's observed behavior. **Certifiers and adopting authorities** make their respective decisions only where their identity, scope and governing rules permit. **Integrators** establish canonical technical state only within their delegated power.

These functions can sometimes be performed by the same actor, but only where the controlling requirements and risk permit. Assigning a title to a person, agent or service does not manufacture independence or authority. Coordination of work is different from inspection, certification, adoption and deployment.

Every substantive assertion must distinguish authoritative source, relayed source, direct observation, interpretation and inference. Preserve exact source and configuration identities and do not collapse distinct identifier namespaces. An unavailable controlling text cannot be replaced by a plausible summary.

## Constitutional articles — CA01–CA23

The constitutional articles translate the seven principles into specific obligations, prohibited shortcuts and validation expectations. Their substance and order are retained; **CA** distinguishes operationally testable articles from the seven **EP** principles. Historic references to article numbers CA01–CA23 refer to the corresponding CA01–CA23 under this revision.

| Article | Required behavior | Prohibited shortcut | Validation |
|---|---|---|---|
| CA01 — Reuse Before Build | Inspect and reuse qualified, versioned components. | Duplicate an owned capability for convenience. | Reuse/source crosswalk. |
| CA02 — Minimum Sufficient Implementation | Deliver the smallest complete authorized capability. | Speculative architecture, infrastructure, dependencies or scope expansion. | Authorization-to-diff review. |
| CA03 — Contract Before Code | Identify the controlling source, external reliance boundary, duties, expected acceptance and the authority by which a proposed change may acquire canonical standing. | Start against an unnamed or mutable contract. | Entry prerequisites. |
| CA04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. | Independent pre-acceptance source/pin record. |
| CA05 — Fail Closed Without Inventing Policy | Apply specified conservative treatment and expose missing semantics. | Invent a cause, grant, floor, deadline, mapping or default. | Negative controls and source audit. |
| CA06 — Preserve Original Evidence | Retain consequential decision ancestry, rejected alternatives, objections, adverse findings and supersession where legitimately relevant, subject to privacy and retention limits. | Delete, relabel, overwrite or silently rescore failures. | Immutable predecessor evidence. |
| CA07 — Exact-Source Reproducibility | Bind claims to exact source, configuration, governing context and transition evidence; reconstruct authoritative pathways when deterministic execution replay is impossible. | Transfer a pass across revisions. | Exact-head manifest and review. |
| CA08 — Independently Qualified Delivery | Optimize authorization-to-independently-qualified outcome; distinguish lifecycle evidence. | Treat PR counts, green CI or documents as delivery or qualification. | Honest PASS/FAIL/BLOCKED and stage timing; active hours remain unknown unless measured. |
| CA09 — Safe Parallelism | Parallelize independent work against pins; serialize conflicting canonical contract, state, schema, admission and integration changes. | Concurrent conflicting authority mutations. | Ownership, pin and dependency review. |
| CA10 — Autonomous Within Authority | Finish routine authorized work and eligible corrections and merges. | Assume new architectural, financial, security or release authority. | Authorization and merge audit. |
| CA11 — Proactive Blocker Management | Check dependencies, resolve routine issues, redirect useful work and isolate one decision package. | Repeat planning loops or wait for routine continuation. | Designated blocker and next-action record. |
| CA12 — No Unqualified Degradation | Protect mandatory floors and legitimate external commitments during internal evolution; use explicit authorized compatibility transitions for justified changes. | Treat lower cost or fallback as equivalent. | Floor and negative-control evidence. |
| CA13 — Observability Before Optimization | Measure baseline cost, latency, refusal, failure, retry, resources and acceptance. | Claim improvement from projection. | Reproducible measurement protocol. |
| CA14 — Secure by Construction | Use least privilege, bounded environments and risk-proportionate assurance. | Treat CI or speculative counts as security qualification. | Enabled-path security review. |
| CA15 — Bounded Changes and Reversible Integration | Keep changes reviewable with migration/rollback and recorded irreversible authority. | Bundle unrelated architecture or erase history. | Scope and migration review. |
| CA16 — No Silent Claim Promotion | Separate proposed, documented, implemented, developer-tested, independently qualified, deployed and production-qualified. | Promote lifecycle labels or substitute them for project-defined claim statuses. | Claim/evidence review. |
| CA17 — Decision Finality and Controlled Reopening | Preserve canonical decision finality while allowing bounded, reasoned challenge and authorized supersession without erasing alternative or adverse evidence. | Reopen from preference or use finality to suppress a defect. | Decision record and reopening assessment. |
| CA18 — Governed Policy and Protected Invariants | Version, authenticate and review governance-critical policy and rule changes; protect established mandatory invariants against configuration override. | Treat unreviewed settings or evaluator changes as governing authority, weaken mandatory checks or introduce an unaccountable decision path. | Policy lineage, completeness, negative tests and proportionate independent review. |
| CA19 — Canonical Integration | Distinguish proposal, inspection, acceptance and integration; only competent authority confers canonical standing. | Treat local success, generated output or merge mechanics as organizational adoption. | Traceable adoption and integration identity. |
| CA20 — Scoped Delegation | Bind delegated work to actor, role, domain, action, context, time, limits and accountable issuer. | Treat technical capability or a subordinate assignment as general transferable authority. | Scope, expiry and revocation audit. |
| CA21 — Boundary Commitments | Preserve relied-upon external semantics or obtain an explicit authorized compatibility transition. | Introduce silent contract, rights, evidence or interface regressions through internal refactoring. | Boundary-focused regression and migration review. |
| CA22 — Reversible Possibility | Preserve proportionate lawful alternatives and permit justified challenge and supersession with ancestry. | Erase dissent or confuse decision rollback with reversal of a committed external effect. | Lineage and recovery review. |
| CA23 — Accountable Certification | Separate contribution, inspection, qualification, certification and integration according to risk and governing independence requirements. | Self-certify generated work or treat nominal human involvement as sufficient authority. | Competence, identity, independence and accountability review. |

## How the articles work together

### 1. Proposals, contracts and canonical change

**CA01–CA03 and CA19** require reuse before invention, the minimum sufficient intervention, and contracts before implementation. A proposal must identify its controlling source, intended effect, legitimate reliance boundary, acceptance criteria and integration authority. A local demonstration, signed artifact or successful merge does not itself establish organizational adoption. The right to generate an alternative is broader than the right to make it canonical.

**CA15, CA17, CA21 and CA22** balance decisiveness with evolution. Work should be small enough to inspect, integrate and where possible reverse; changes must not silently violate obligations on which others legitimately rely. Internal architecture may change freely inside those commitments. Otherwise, an authorized compatibility or migration decision is required.

A canonical decision remains operative until lawfully superseded. Reopening requires an identified authority, controlling source, reasons, scope, version and qualification implications. Material new evidence, demonstrated inconsistency, a security or constitutional defect, or explicit competent instruction can justify reconsideration. Mere preference does not. Preserve material alternatives, objections and adverse records proportionately and lawfully. Reversal of a decision or configuration cannot undo an already committed external effect; any compensation needs distinct authority.

### 2. Delegation, coordinated work and accountability

**CA09–CA11 and CA20** support productive parallel engineering without distributing canonical authority indiscriminately. Delegate concrete, bounded work to identifiable actors by role, domain, action, context, time and limits. Serialize conflicting changes to canonical contracts, shared schemas, admission conditions or mutable state; parallelize independent investigations and implementation tasks against fixed inputs.

Workers and coordinators should resolve routine authorized issues, manage dependencies and surface genuine decision points, but cannot infer permission for an architectural change, additional expense, security exception or release from their technical capacity. Delegation does not permit a subordinate to enlarge its authority or transfer it onward silently. Track revocation and expiry where applicable.

### 3. Policy integrity, failure semantics and security

**CA05, CA14 and CA18** require faithful treatment of controlling requirements. Missing, ambiguous, unsupported or stale prerequisites must not quietly become approval or not-applicable. Fail closed according to the applicable contract without inventing a policy, grant, reason, deadline or default. Protect mandatory governance invariants through the mechanisms appropriate to the system's risk.

Where policy and rules are configurable, their governing authority, scope, versions, provenance, applicability and change process must remain explicit. Policy changes, evaluator changes and configuration updates cannot silently waive binding checks or create a competing, unaccountable route to decision authority. Implementations may use authenticated files, registries, typed evaluators, deterministic software or other adequate forms; **no particular rules engine, storage technology or canonical kernel is constitutionally required**. If data and evaluator logic are separated, preserve completeness, authenticity, unambiguous applicability, defined failure treatment and authorized activation.

Historical decisions retain their original governing rule/configuration identities and observed outcomes. Evaluation under changed policy is a new, distinct event, not retroactive amendment. Material governance-rule changes require source-based impact assessment, relevant adverse and negative controls, and independent assessment where warranted. Likewise, source inspection, green CI and local simulation are not substitutes for enabled-path security assurance.

### 4. Evidence, qualification and accountable certification

**CA04, CA06–CA08, CA16 and CA23** require that consequential claims follow the evidence rather than the other way around. Preserve original findings, failed runs, material alternatives, decisions and supersession paths. Reproduce exact behavior where feasible; for nondeterministic systems, preserve the governing context and attributable transitions needed for bounded reconstruction.

Independent expectations should be recorded before candidate acceptance. Implementation does not grade itself, and a qualifier cannot adjust frozen expected results to make a candidate pass. Qualification, responsible certification and technical integration are distinct functions. Machine generation and nominal human review alone establish neither competence nor authority.

Keep lifecycle states distinct: proposed, documented, implemented, developer-tested, independently qualified, integrated, deployed and production-qualified. A result transfers only to the exact sources, profiles and conditions actually evaluated. Measure the time to independently accepted outcomes where observable; code volume, elapsed commit intervals and the number of workers are not substitutes for measured effort or value.

### 5. External commitments, measurements and risk

**CA12, CA13 and CA21** prohibit claims that cheaper, faster or simplified alternatives preserve quality when mandatory governance, reliability or compatibility floors have not been demonstrated. Measure costs, latency, refusals, failures, retries, resources and acceptance before making optimization claims. An internal technical improvement is not justified by silently degrading a legitimate external commitment.

## Risk-proportionate review and allocation

**Tier 1 is highest criticality; Tier 3 is lowest.** These are assurance and review classifications, **not a remediation queue**. A critical defect usually demands urgent containment, but scheduling must account for exploitability, consequences, affected users, dependencies, available mitigations and competent direction. Do not automatically fix Tier 3 items first simply because they are numbered third. Classify changes by the most consequential applicable risk. Review remains proportionate to consequences and does not displace governing obligations, required checks or decisions expressly reserved to competent authority.

| Tier | Scope | Required treatment |
|---|---|---|
| Tier 1 — critical | Authority, admission, security, trust, authentication, irreversible effects, atomic state, negative-evidence custody, or independent acceptance logic. | All applicable Tier 2 and Tier 3 controls, with focused independent review proportionate to the identified critical risk. Preserve explicitly reserved approval and authority boundaries. |
| Tier 2 — substantive | Bounded implementation or behavior-changing engineering outside Tier 1 critical boundaries. | Developer regression tests, required automation, and independent qualification where applicable. Use additional code review where concrete risks warrant it. |
| Tier 3 — routine | Documentation, metadata, formatting, and objectively nonsemantic changes. | Author self-validation and required automated checks. Independent review is not required unless a specific risk or governing rule demands it. |

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

