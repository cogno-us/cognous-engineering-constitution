# Testing Addendum — Risk-Based Development Testing and Milestone Qualification

**Classification:** Interpretive and operational guidance supporting the existing constitution; **not a new constitutional article**, not a waiver, and not a retroactive amendment to adopted or frozen revisions.  
**Proposed:** 2026-10-25. **Scope:** Cognous engineering workstreams, subject to project-specific adoption and controlling contracts.  
**Constitutional basis:** [ENGINEERING_CONSTITUTION.md](../ENGINEERING_CONSTITUTION.md), especially CA01–CA08, CA12–CA16, CA18, CA21, CA23, and EP1, EP4, EP7; [ADOPTION.md](../ADOPTION.md).  
**Precedence:** Controlling law, project safety/security rules, pinned contractual acceptance obligations, independent qualification, branch protections, and release holds override this scheduling guidance. An addendum cannot itself confer adoption, spending, integration, deployment, certification or release authority.

## Principle

**Test continuously; qualify comprehensively at defined milestones—not automatically after every incremental change.**

Allocate verification effort according to *risk, affected boundaries, and actual changed behavior*. Keep fast development feedback distinct from independently qualified evidence. Reuse already-working test infrastructure; do not make repeated full-battery executions, redundant manual evidence reviews, or speculative qualification frameworks routine prerequisites to each small feature.

This changes **testing cadence**, not mandatory assurances, acceptance criteria, protected invariants, or required independence.

## Three complementary levels

### Level 1 — Implementation feedback (bounded spot checks)

For ordinary development changes:
1. Build and typecheck affected modules.
2. Run targeted unit and component tests relevant to the change.
3. Exercise a small representative set—typically **2–5 behavioral spot checks**—including applicable negative paths; this is a heuristic, **not a maximum or required substitute** for mandated tests.
4. Check affected safety invariants; repair verified defects and rerun the tests that demonstrate the fix.
5. Retain material failures, limitations and exact candidate identity. Do not delete, silently relabel or rescore adverse evidence.

Existing unattended CI may continue, including broad suites if already inexpensive and required. Avoid **redundant manual reruns and full evidence-pack preparation** when exact-head evidence already answers the development question.

**Claim boundary:** A working demo and developer tests support `IMPLEMENTED / DEVELOPER-TESTED`, not independent qualification, deployment approval or production readiness.

### Level 2 — Sprint integration and PR gate

Before integrating a sprint candidate:
1. Show the authorized end-to-end behavior.
2. Run affected regressions, interface/contract checks and critical negative controls.
3. Verify the consequences of changes to authority, policy, canonical state, custody, refusal, persistence, recovery and external effects where applicable.
4. Complete required code review, protected CI/security checks and documented acceptance criteria.
5. Identify exact source/configuration/head, unresolved risks and supported nonclaims; preserve negative observations.

**Do not replace a mandatory independently qualified gate with developer testing.** If the controlling project contract requires full-battery or independent checks before a particular merge, those checks remain required unless competent authority explicitly changes the contract.

### Level 3 — Freeze, qualification and release decisions

At a designated MVP freeze, integrated candidate milestone, security gate or release qualification:
1. Freeze candidate, dependencies, profiles, inputs, clock/environment as applicable, and **independent expectations/oracles before execution**.
2. Run full **applicable** regression and integration coverage, bounded adversarial/security and fault/recovery scenarios as risk requires.
3. Preserve raw attempts, negative results, artifacts, custody/identity, configuration and reproduction instructions.
4. Report **PASS / FAIL / BLOCKED / NOT EXECUTED** separately (and N/A where supported); no green-workflow promotion to qualification.
5. Remediate and requalify affected scope, maintaining predecessor results and exact revision lineage.

Independent qualification, authorized certification, canonical integration, organizational adoption and production deployment are **separate decisions**. Existing holds remain effective until lifted by competent authority.

## Escalation rule — change impact outranks code size

Expand immediate pre-merge testing beyond routine spot checks if a change could:
- Permit, dispatch or fail to reconcile an unauthorized **external effect**.
- Alter grant, identity, delegation, admission, revocation, policy or protected invariant semantics.
- Affect canonical state integrity, negative-record custody, evidence preservation, persistence, concurrency, crash recovery or irreversible migration.
- Change shared contracts, protocol compatibility or security-relevant dependencies.
- Repair a historical material defect or invalidate prior qualification evidence.

Run the **necessary affected negative, integration, failure-injection and adversarial controls now** rather than postponing high-consequence evidence to the final milestone. A seemingly one-line change may demand extensive tests; a large non-effecting internal change may not.

## Distinct application profiles

**Governed Cognition Runtime (GCR).** GCR denotes the generic architectural role of a governed cognitive runtime, not a particular proprietary implementation, repository, or qualification program. During implementation, emphasize eligible versus invalid evidence, authority/policy refusal, source and lineage preservation, canonical transitions, and fresh-process recovery. Independent cognitive preservation, compression, answer-quality and conformance testing belongs to the designated profile/milestone. Do not transfer a qualification pass between distinct GCR implementations or revisions, or confuse emulator recovery with cloud durability.

**Cognous OCS / Stack Qualification.** During implementation exercise the impacted authorization-to-effect boundary, dispatch, revocation/race behavior, idempotency, refusal and reconciliation. Higher-consequence effects may require broader immediate regression and adversarial testing. Existing OCS security, publication and production holds, candidate-freeze requirements, and independent qualification obligations are unchanged.

The programs may harmonize generic manifests, digests, evidence conventions and telemetry *without conflating their domain-specific assertions or independent oracles* or creating cross-repository runtime dependencies.

## Anti-patterns

- Re-running thousands of unrelated tests as a manual ritual after every small edit.
- Using passing developer CI to self-issue qualification or certification.
- Deferring serious authority/effect or integrity risks to milestone freeze.
- Creating a second verifier, runner, dashboard or evidence platform absent a specific demonstrated gap.
- Editing frozen expectations after observing candidate output; hiding failures, BLOCKED cases or attempts.
- Confusing cost reduction, spot-check counts or rapid PR merges with verified reliability.
- Treating this guidance as an override of pinned project-specific duties.

## Operating loop and records

**Implement → targeted spot-check → repair → affected integration gate → milestone qualification.**

Record only the proportionate evidence needed for each stage: exact candidate, changed boundaries, focused cases and outcomes, material failures, known limitations, reviewer disposition and next action. Reserve full independently reviewable evidence packs for mandated gates and defined freeze/qualification milestones.

**Adoption note:** This document supplies a consistent interpretation and reusable operating policy. Each project owner/adopting authority must identify its applicable revision, scope and any needed contract amendments under [ADOPTION.md](../ADOPTION.md). Frozen past qualifications and explicitly pinned constitution revisions are not silently changed by publication of this addendum.
