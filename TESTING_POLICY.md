# Cognous Risk-Tiered Testing and Evidence Policy — v1.0

**Status:** Normative engineering practice, subject to competent adoption under [ADOPTION.md](ADOPTION.md). **Classification:** new normative implementation guidance; does not amend EP1–EP7 or CA01–CA23. **Applies to:** software, models, datasets, configuration, governance controls, documentation and automated workflows where adopted. **Effective adoption:** requires an exact-revision, scope-specific adoption record. Merging this document alone is not project adoption.

## 1. Controlling principle

**Every change must produce the minimum sufficient *new* evidence to substantiate that its risk-relevant invariants and external commitments still hold.** Test scope scales with consequences, reachability and uncertainty of failure, not diff length, number of files or the number of available tests. Reuse existing evidence only where exact source, dependency, contract, configuration and execution-environment applicability is demonstrated.

This policy operationalizes CA02, CA04, CA06–CA08, CA12–CA16, CA18 and CA23. It does not reduce controlling regulatory, security, contractual, branch protection, independent-qualification or adopted project requirements. If two rules apply, follow the stronger applicable obligation; record unresolved conflicts.

## 2. Mandatory risk classification

Assess the **highest consequential impact** of any reachable changed path, including transitive dependencies, data, state, policy or CI configuration. Do not classify based on lines changed.

| Tier | Illustrative scope | Minimum ordinary engineering evidence |
|---|---|---|
| **T0 — Editorial** | Comments, prose, metadata, non-executable documentation, with no contract, governance, generated artifacts or CI semantics changed | Relevant formatting, links, document/claim consistency; confirm change is truly non-executable. Full component regressions ordinarily unnecessary. |
| **T1 — Isolated low consequence** | Non-authorizing utilities, presentation, bounded mocks and local tooling | Focused unit test and representative positive, negative and error cases, with static checks where relevant. A single mocked case is sufficient only if it covers the bounded claim and no material alternative path is reachable. |
| **T2 — Interface or composition** | Public API, data/contract schema, policy representation, cross-component wiring, version pin, migration or effective-policy composition | Exact schema/compatibility, representative boundary and negative tests, affected integration/regression paths and pin/consumer checks. |
| **T3 — Governance or safety critical** | Authority, trust, canonical state, persistence, approval commitment, revocation, security controls, execution boundary, external effects, rollback/replay or production behavior | Broad **affected** regression, adverse/negative and boundary tests, security and failure-path checks, compatibility, recovery where applicable, and qualified change-specific evidence. Unrelated repository-wide tests are not automatic unless risk or controlling gates require them. |
| **T4 — Acceptance milestone** | Release candidate, engineering freeze, certification, mandated independent qualification | The complete prescribed qualification campaign at exact frozen heads, with required independence and adverse evidence; cannot be replaced by T0–T3 developer results. |

A documentation edit changing a governing requirement, security procedure, API contract or release claim is not automatically T0. A one-line authorization change can be T3. Classify a change with multiple aspects at the highest relevant tier, and cite the rationale.

## 3. Scope selection and test sufficiency

1. Identify controlling source and accepted baseline, changed paths, consumers, affected invariants, external obligations and plausible failure modes.
2. Select the smallest suite that can *falsify* each material claim. Include positive, negative, boundary, refusal and adversarial cases where their risk is material. For governance-critical changes, one happy-path case is insufficient.
3. Prefer focused compile/type/lint checks and deterministic mocked fixtures during iterative development; run real integration tests where a mock cannot establish the relevant boundary.
4. Escalate when security/authority/persistence/external effects are reachable, a dependency or contract changes, behavior differs from baseline, coverage is uncertain, a failure indicates wider reachability, or an independently qualified gate demands it.
5. Keep full-cohort, paid-provider, production-system and expensive cross-repository campaigns off by default. Require explicit authorization for paid calls, billable environments or real external effects and respect any already approved cap.
6. Never disable a needed test, adjust an oracle to match implementation, hide failure logs, loosen a check or call a workflow skip a PASS.

## 4. Evidence reuse and CI optimization

Reuse a prior pass only when the claimant records exact tested source head, relevant dependencies/contract versions, inputs, environment, test identifier, result and why the changed system remains within that evidence's applicability. A passing test on a different revision is not automatically transferable (CA07). Re-run targeted tests when the evidence cannot cover a changed failure mode.

CI should be change-sensitive where repository policy permits: editorial-only checks for T0; focused suites for T1; contract and affected integration tests for T2; broad affected regression and security tests for T3. T4 follows its independent acceptance plan. Preserve branch protection, required named checks and review rules; if a required workflow has no applicable executable tests, report an honest explicitly **not-applicable/skipped-by-scope** status using a branch-protection-compatible design. Avoid unnecessary duplicate workflows, repeated full-cohort replays and rerunning the same frozen suite merely to reproduce unchanged results. Skip rationale must be auditable.

CI optimization itself is a workflow/security change: assess its reachability and prove that branch protection, mandatory checks and relevant tests cannot be bypassed by misclassification, path filters, changed workflow files, renames or generated artifacts.

### Shared-boundary evidence reuse for multi-item migrations

When multiple migrations use a common evaluator/schema/contract, test and pin the common boundary before migrating individual items where feasible. A subsequent item may reuse prior *boundary* tests only after recording (1) the exact tested evaluator and contract identities and all relevant dependencies and environment, (2) byte or semantically justified identity of those boundary inputs at the new head, and (3) absence of new reachable interactions outside the earlier test scope. A zero diff in evaluator and contract files is **necessary in simple cases but not sufficient**: changed data, callers, dispatch, runtime wiring, authority state or configuration may invalidate the earlier evidence.

Each migrated item still requires source-to-registered-data equivalence and refusal/negative tests, plus affected integration tests that establish the removal or replacement of its legacy hardcoded path did not alter externally observable decisions. Removing a hardcoded branch is a code and possibly execution-boundary change, **not automatically data-only or T1/T2**. Reclassify at T3 whenever authority, canonical state or enforcement reachability makes that appropriate; use T4 for any independently prescribed final qualification. An unforeseen schema incompatibility must use an explicit change-control gate rather than a hidden in-item schema amendment. Refer to [batch architecture and evidence invariant](ORCHESTRATION.md#batch-architecture-and-evidence-invariant).

## 5. PR evidence declaration

Every substantive candidate includes a compact **CI Scope Declaration**, embedded in the PR or a linked durable record:

- **Risk tier and justification**; exact change head and affected scope/invariants.
- **New evidence**: test names, results, environment and pins.
- **Reused evidence**: exact source identities and applicability argument.
- **Not run / skipped**: tests, reason, and remaining qualification obligations.
- **Failures and blockers**: unchanged baseline failures, new regressions, risk owners and disposition.
- **Authority**: explicit approval for any paid test, external effect or qualification exception.

For T0 this may be a short statement. Do not create large reports for trivial changes. Builder claims of `TESTED`, `QUALIFIED`, `ACCEPTED`, `RELEASED` and `DEPLOYED` remain distinct.

## 6. Autonomous engineering and escalation

Within delegated scope, builders should complete routine fixes, targeted rechecks and documentation repair in a bounded work session without unnecessary intermediate approvals. Escalate a genuine architectural, authority, security, contractual, expenditure or qualification decision. Do not merge when approval is reserved; do not bypass mandatory reviews or branch protection. Session continuity may come from pinned plans, pull requests, decision records and evidence rather than a persistent conversation.

## 7. Independent qualification, retention and exceptions

Risk-tiered developer CI is **not** independent Tier 1 qualification or certification. Preserve negative evidence, original failed outputs, qualification holds, exact-head traces and the independent oracle. The independent qualifier defines and executes the required scope rather than inheriting a builder's convenience-based test selection. Any waiver or policy exception requires competent authority, explicit scope, duration, rationale, mitigating controls and immutable evidence; this policy does not itself confer waiver authority.

**Normative precedence and amendment:** The constitutional principles, articles and [ADOPTION.md](ADOPTION.md) control. This companion may be amended with its own versioned lineage and competent adoption. It cannot silently alter the obligations or adopted revision of any engineering project.
