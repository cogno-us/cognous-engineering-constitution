# Constitution: exact table and operational interpretations

Source: `ENGINEERING_CONSTITUTION.md`, main tree `dcdbe3b76843d672ca3cfb1f000124ecd78ed03c` observed 2026-11-04. **These cells are verbatim from the observed article table, not a claim about any project's adopted revision.** Before injecting legally/operationally binding text, compare source for exact selected SHA.

## Seven engineering principles

- **EP1 Operational legibility (CA03, CA07, CA13, CA16):** permit accountable observers to trace intent, requirements, evidence, assessment, decision, execution and effects with privacy/security bounds.
- **EP2 Canonical integration (CA03, CA04, CA17, CA19, CA23):** proposals and successes are not canonical until an identified competent authority effects a traceable integration; qualification, adoption and deployment are distinct.
- **EP3 Identity-scoped delegation (CA09, CA10, CA11, CA20):** actor, role, domain, action, context, time, limits, accountability, expiry/revocation; capability does not confer authority.
- **EP4 Lineage-preserving history (CA06, CA07, CA15, CA22):** preserve source ancestry, negative findings, supersession and reconstructable transitions subject to lawful retention.
- **EP5 Boundary commitments (CA12, CA15, CA21):** internal design can change but external relied-upon semantics require preservation or authorized compatibility transition.
- **EP6 Reversible possibility (CA06, CA15, CA17, CA22):** preserve justified challenges and alternatives, control reopening, acknowledge irreversible external effects.
- **EP7 Accountable certification (CA04, CA08, CA16, CA23):** distinguish author, inspector, independent qualifier, certifier and integrator, requiring real competence, authority and independence.

## Exact constitutional table cells

| ID / title | Required behavior (verbatim) | Prohibited shortcut (verbatim) | Validation (verbatim) |
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

## Interpretive boundary notes

- Historical labels `EP01–EP23` correspond to CA01–CA23 in this revision; EP1–EP7 now name the seven broad principles.
- No specific programming language, rules engine, storage, kernel, branch method or signature technology is mandated. A receipt/hash may prove identity or provenance, not correctness or authority.
- Canonical decisions are final unless competent, sourced, scoped reopening; genuine defects and new material evidence can justify reopening. Preserve prior decision lineage.
- An ambiguous commit acknowledgment does not prove durable custody. Missing freshness evidence does not prove freshness. Required checks disabled/unavailable do not PASS.
- Substantive documentation and governance-policy changes are not automatically routine. Qualify them by their impact.
- **Constitution review Tier 1–3**: Tier 1 routine/nonsemantic; Tier 2 substantive bounded implementation; Tier 3 critical authority/security/state/trust/effects/acceptance. This **differs** from TESTING_POLICY testing tiers T0–T4.
