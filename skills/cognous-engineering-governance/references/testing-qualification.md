# Risk-tiered testing and qualification

Sources: `TESTING_POLICY.md` (v1.0 normative practice requiring local adoption), `addenda/RISK_BASED_TESTING.md` (interpretive/proposed guidance); Constitution CA02, CA04, CA06–CA08, CA12–CA16, CA18, CA23. Stronger adopted or contractual controls take precedence.

## Risk T0–T4: highest reachable consequence

| Tier | Typical material change | Minimum ordinary new evidence |
|---|---|---|
| T0 editorial | Non-executable prose/comment/metadata; no governance, contract, generated content or CI semantics | Validate actual nonsemantic nature, links, consistency/formatting; not automatic full regressions |
| T1 isolated low consequence | Non-authorizing utilities, bounded mock/tooling, presentation | Focused unit test plus positive/negative/error/boundary as applicable, static checks |
| T2 interface/composition | API, schema, policy representation, inter-component wiring, effective config, version pins, migration | Exact contract/schema/compatibility, affected consumers, integration and negative tests |
| T3 governance/safety critical | Authority, trust, security, revocation, approval, canonical state, persistence, external effects, crash recovery, rollback, acceptance boundary | Broad **affected** regression; adverse/negative/security/failure/recovery, compatibility and change-specific qualified evidence |
| T4 acceptance milestone | Frozen release candidate, certification, required independent campaign | Full **prescribed applicable** independent qualification at exact frozen heads, independently owned oracle and raw negative evidence |

A one-line authority change can be T3. A doc change to a governing contract is not T0. Include transitive reachability: callers, data, policy, CI workflow changes, generated artifacts, state, effective configuration. A T3 change does not automatically require *unrelated* full-repository suites; obey mandatory named checks and risk coverage. T4 is a distinct milestone rather than a size-of-diff tier.

## Three-level operating cadence

**Level 1 — iterative feedback:** build/typecheck affected modules, focused unit/component tests, a few representative behavioral spot checks (often 2–5, **heuristic only**, never a cap), critical negative checks, preserve failures. Developer-tested ≠ independently qualified.

**Level 2 — sprint/PR integration:** authorized end-to-end behavior; affected regressions, interface/contract/critical negative controls; verify policy, security, custody, external effects, refusal, recovery when reachable; protected checks and review; exact final head/limitations. Do not skip mandatory pre-merge independent gate.

**Level 3 — frozen milestone:** exact subject, dependencies, profile, environment and independent expectations frozen **before** evaluation; complete applicable campaign with adverse/negative/recovery/security checks; raw attempts/custody preserved; independent PASS/FAIL/BLOCKED/NOT EXECUTED; successor requalification retains failures. Release and deployment remain reserved separate decisions.

## Falsifiability and test selection

Select smallest suite able to **falsify each material claim**, including positives, negatives, boundary, refusal, adversarial, interruption and recovery where relevant. Use deterministic fixtures for early iteration; exercise real boundary when mocks cannot substantiate identity, durability, effects, integration or environment. Expand when authority/persistence/security/external effects reachable, contract changes, baseline anomaly, uncertainty, wider failure or prescribed independent gate. Avoid repeated full battery without changed input or a protocol requirement. Never alter oracle to match implementation, disable required checks, hide errors or call skip PASS.

## Exact-head evidence reuse

Reuse only after recording tested source and changed head, dependencies/contracts, input and environment identities, test ID/result and reason all affected reachable paths remain covered. A zero diff in an evaluator/schema is not sufficient when callers, data, dispatch, runtime wiring or authority state changes. Each migrated item needs source-to-data equivalence, negative/refusal and affected integration tests. If a hardcoded branch was removed, do not pretend it was a data-only change. Unforeseen schema changes require contract change-control. An emulator pass proves its tested emulator profile, not real cloud durability or production identity.

## CI optimization and branch protection

Path-sensitive workflows may reduce unrelated work if repository policy allows. Protect mandatory named checks, branch protection, workflow-file edits, changed-path classification, renames and generated artifacts from bypass. An applicable empty suite may report `SKIPPED BY SCOPE / N/A` accurately via branch-compatible design, never PASS. Changing CI selectors itself deserves reachability/security analysis. Avoid duplicate harnesses and duplicate manual runs.

## Compact PR CI Scope Declaration

For each substantive candidate, state: (1) T-tier, rationale and exact final head; (2) changed scope/invariants/consumers; (3) **new evidence** tests, execution environment, pins and results; (4) **reused evidence** exact IDs and applicability; (5) not run/skipped and remaining qualification obligations; (6) baseline/new failures and BLOCKED owners; (7) authority for paid providers, external effects or exceptions. Keep T0 proportionate, not a bureaucratic matrix.

## Qualification chain and verdict distinctions

**Independent specification → Configuration → Frozen invocation → Observation → Independent oracle → Evidence record.** Independent qualifier owns the expectation before candidate observation, not retrofit. Record exact fixture/spec/hash, expected predicate or bytes, effective-enabled config, authority/policy identities, invocation and environment, raw outputs, negative results, checksums, transition/receipt/recovery, resource metrics, reviewer and verdict. Test standalone and affected interactions, disabled/unavailable states and refusal. Independence is a real separation of duties; a different agent that shares builder-controlled oracle is not automatically independent. Human signoff without competence, evidence and scoped authority does not certify.

Case classifications: **PASS** matches resolved applicable frozen expectation; **FAIL** is observed mismatch; **BLOCKED** is unresolved source/profile mapping or required evidence/precondition preventing verdict; **NOT ASSESSED/NOT EXECUTED** means no qualifying run; **N/A** only if actual governing applicability predicate is absent. Keep attempted execution separate from environment setup. Preserve historic negatives and original scoring, publish successor correction separately. An ambiguous ack is not durable custody; receipts do not establish grants.

## Risk-specific negative cases

- Authority/delegation: unauthorized actor, expired/revoked scope, crossed domain/context, denied approval, conflicting canonical writers.
- Policy: malformed/unknown version, disabled rule, overlapping or missing applicability, unreviewed evaluator, fail-closed refusal, invariant tamper.
- Persistence: interrupted commit/ack, fresh-process replay, wrong-owner recovery, partial writes, lineage integrity, no silent deletion.
- External effects: duplicate/race dispatch, idempotency, lost ack/reconciliation, revocation between approval and execution, irreversible compensation authority.
- Contract/migration: old legitimate inputs, invalid schemas, version drift, consumer compatibility, no hidden fallback, exact baseline comparisons.
- CI: skipped/missing mandated check, altered path filter, renamed file, generated-artifact effects, frozen oracle edits.

## Cost and spending boundaries

Keep expensive complete batteries, real provider calls, billable cloud and actual external effects OFF unless explicitly scoped, budgeted and authorized. A planned budget is not approval. Account for real unit prices, observed calls/retries, refusal rate, acceptable quality floor and cost **per independently accepted deliverable**. Never label estimated savings measured.
