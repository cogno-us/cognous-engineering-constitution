# Orchestrator Prompt Engineering Addendum — v1.0 (proposal)

**Classification:** Proposed normative implementation guidance. **Status:** NOT ADOPTED by publication or merge. Applies only following competent, exact-revision, scope-specific adoption under [ADOPTION.md](ADOPTION.md). It does not change EP1–EP7, CA01–CA23, existing project adoptions, frozen contracts or reserved authority.

**Companion sources:** [Engineering Constitution](ENGINEERING_CONSTITUTION.md), [Orchestration](ORCHESTRATION.md), [Task-Scoped Compliance Injection](ENGINEERING_COMPLIANCE_ADDENDUM.md), [Risk-Tiered Testing](TESTING_POLICY.md). The companion addendum controls exact clause lookup; this document controls *assignment compilation and presentation* only when adopted. Use the **same adopted exact constitutional source** for normative clause text. Never replace controlling project pins with the repository's latest revision silently.

## 1. Problem and design goal

A builder should not have to guess what “Archetype C” means or navigate a large constitutional corpus to learn its immediate work. Prior orchestrator prompts showed complementary defects: (a) correct verbatim clause injection but too much repeated governance text and too little operational direction, and (b) clear execution phases but an Archetype C repair section that delegated exact clause injection to later subassignments rather than injecting it in the active packet. Both can lead to drift. The required output is **one self-contained, executable eight-field assignment**, not a general-purpose constitution recap.

**Optimization objective:** minimum total engineering effort per independently accepted, reliable deliverable. Reduce repeated contract mutations, generic test campaigns, incidental workflows and intermediate handoffs without weakening qualification, security, provenance or authority.

## 2. Three distinct decisions before drafting

1. **Authority and adoption resolution.** Identify the receiving project, competent decision, exact base/head, local adopted constitutional revision, governing source pins, permissions and known holds. New constitutional publication is not local adoption. If a relevant source, decision or adoption is **UNVERIFIED**, do not invent it: discover it or issue a single source-backed blocker for the affected operation.
2. **Primary archetype.** Select exactly one A–D based on the immediate deliverable, not every activity in a larger program. Role and archetype are independent axes; archetype never confers authority. If design and implementation need separate contract-freeze authority or qualification independence, issue separate packets with explicit gates.
3. **Risk tier.** Independently select T0–T4 based on highest reachable consequence, including data, workflow, caller and transitive changes. Archetype does **not** determine tier. T3 execution-boundary repair may require more than one mocked case; T4 independent qualification is separately owned.

### Operational archetype definitions

| Code | Builder's immediate job | Entry gate | Exit evidence |
|---|---|---|---|
| **A — Architecture/contract** | Inventory related items; reconcile shared invariants, interfaces, versioning, failure semantics; select one canonical writer; freeze the common contract **before** migration. | Controlling sources, scope, affected consumers, architecture authority identified. | Versioned contract and decision record, compatibility/refusal plan, approved freeze or explicit blocker. |
| **B — Scoped implementation/migration** | Implement the smallest authorized change **against a frozen contract**; preserve legitimate compatibility and negative evidence. | Contract/version, writable ownership, acceptance path and required predecessor gate satisfied. | Exact implementation head, changed paths, affected tests, migration/rollback facts and honest status. |
| **C — Defect/CI/regression repair** | Confirm the reported failure is still present; preserve original evidence; identify source-backed cause; make the **smallest** correction; test affected behavior at final head. **If already fixed/mergeable, do not manufacture a code change.** | Exact failing evidence or current counterexample, relevant baseline/head and authority. | Fixed or no-op disposition with precise evidence, affected positive/negative checks, regressions distinguished from baseline. |
| **D — Independent qualification** | Apply an independently controlled oracle/protocol to frozen exact subjects; retain raw results, adverse findings and qualified verdict boundaries. | Independent owner, frozen subject, protocol/oracle and required separation verified. | Bounded independent verdict plus failures, exclusions and acceptance authority left explicit. |

For composite programs, show work-package phases and dependencies, but **each dispatched builder work package has one primary archetype**. An orchestrator may reference a future archetype without pretending its clauses were injected into an active subassignment.

## 3. Canonical packet: eight fields, no ninth

Use **exactly** these eight top-level fields, in this order. The formal structure is [schemas/orchestrator-assignment-v1.schema.json](schemas/orchestrator-assignment-v1.schema.json). This is a contract for structured packet data; the builder-facing rendered prompt may use compact numbered headings instead of raw JSON.

1. **Identity:** work package, actual role, primary archetype **and its operational meaning**, repository, exact base SHA and target.
2. **Authority:** authorized outcome and originating decision, eligible actions, restrictions, finance, merge/deployment permission.
3. **Ownership:** designated writer, exact writable paths, protected paths, parallel ownership if any. Absence from writable set means read-only.
4. **Inputs:** controlling project plan, frozen contracts/SHAs, interfaces, dependent projects, original failures and artifact identities.
5. **Acceptance:** risk tier + reachable rationale, falsifiable success and negative/boundary controls, exact focused commands or **DISCOVER BEFORE EXECUTION**, prior evidence + applicability, skips, independent qualification boundary, concise CI Scope Declaration.
6. **Delivery:** PR/branch, exact final SHA, observable result, evidence/negative findings, one bounded handoff.
7. **Boundaries:** prohibited scope, refusal/stop triggers, architectural decision escalation, operator contact only for genuinely reserved decisions.
8. **Governance:** exact project-adopted source, addendum/policy revision identities and **verbatim** Required behavior + Prohibited shortcut cells for the selected canonical archetype, each followed by an **independent task-specific Binding**.

**Presentation rule:** Begin with an imperative, concrete objective and no more than a short paragraph of context, then render the eight fields. Put the operational definition in Identity, execution sequencing and tests in Authority/Acceptance as relevant, and normative verbatim clauses in Governance. Avoid restating the same prohibition under three different headings. Keep packet compact proportional to risk and scope; completeness does not require verbose repetition.

## 4. Typed compilation, canonical clause injection and validation

A machine-readable packet MUST validate against the companion JSON Schema. Schema validation is **necessary but not sufficient**. A compiler/inspector MUST additionally enforce these cross-field and repository-dependent checks:

- **Source/adoption:** full SHA must exist; project adoption revision and scope must be verified; amendment revisions are not silently substituted. Incomplete adoption may be reported as UNVERIFIED with a blocker, not as established authorization.
- **Archetype fidelity:** select from the applicable *exact-revision* Compliance Addendum: A = CA01/03/04/18/21; B = CA02/04/05/09/15; C = CA02/04/06/07; D = CA04/06/07/08/23. Compare article ID, **Required behavior** and **Prohibited shortcut** against canonical source text, not a memorized paraphrase. Missing applicable mandatory clauses or a mismatched byte sequence is a compilation FAIL. Extra relevant articles may be included when justified. Each row has a separate actual file/pin/decision/refusal **Binding**; do not embed task-specific edits in normative text.
- **Role/independence:** an implementation owner cannot declare independent qualification merely by choosing D. Any D verdict requires actual qualification authority and independence. A single assignment with incompatible design and qualification authority must be split.
- **Identity/ownership:** resolve current repository and PR heads before action; ensure writable and protected paths do not overlap, except explicitly documented and separately authorized protected edits; parallel workers must have nonoverlapping canonical-write domains.
- **Authority consistency:** paid execution is OFF unless separately authorized with a nonzero ceiling and evidence; positive `mergeAuthorized` or `deploymentAuthorized` values require independently grounded decisions. Never infer authority from tool access.
- **Evidence/testing:** classify by reachability, not diff size; do not promise one mocked case suffices for T3. Exact previous source/dependency/config/environment applicability is required to reuse a PASS. Separate workflow success, implementation testing, independent qualification, integration, release and deployment.
- **Completeness:** no placeholders such as `<SHA>`, `TBD` or `UNVERIFIED` are silently treated as passed requirements. Missing blocking inputs generate a concise blocker packet rather than a fabricated executable assignment.
- **Documentation:** every substantive PR gets a concise CI Scope Declaration: tier/rationale, tested exact head, new and reused evidence, skipped work, failures, required qualification and explicit paid-effect authority if relevant.

Do not claim a mechanically checked prompt unless canonical text equality and source identities were actually checked by a validator. The JSON Schema checks shape and types; it does **not** prove file existence, adopted authority, cross-repository lineage, clause fidelity or evidence applicability.

## 5. Assignment compiler stages and refusal

```text
DISCOVER current refs, adoption, applicable source and decision
  -> CLASSIFY role / one primary archetype / independent risk tier
  -> RECONCILE shared architecture where needed (A -> gate -> B)
  -> RESOLVE frozen inputs, owners, authorization and evidence
  -> INJECT exact canonical normative cells + task bindings
  -> VALIDATE JSON Schema + cross-field/source/policy checks
  -> RENDER concise eight-field builder assignment
  -> DISPATCH only within authorization
  -> COLLECT exact-head results and statuses
```

If a hard prerequisite is absent, return one bounded CA11 blocker: **missing fact; controlling source; affected scope; alternatives; risk/evidence impact; precise Architect decision**. Ordinary syntax, test, packaging and integration errors are builder-owned; they are not operator escalation triggers. No speculative adapter or policy default may conceal an actual incompatibility.

## 6. Worked shape — defect repair (illustrative, not executable)

**Identity:** `WP-REPAIR-EXAMPLE`, role `implementation_owner`, archetype **C**, operational meaning “confirm current defect, preserve observed failure, minimally fix or no-op, recheck affected behavior”; repo/base `DISCOVER AND PIN`.

**Authority:** fix an already-authorized defect; no paid calls, merge or deployment grant.

**Ownership:** single writer of affected implementation path; frozen schema/oracles protected.

**Inputs:** cited failed check, exact tested source, current head, adopted contract.

**Acceptance:** tier based on *reachable consequences*; targeted positive/negative/boundary controls; previous results reused only if applicable; CI Scope Declaration.

**Delivery:** one PR and exact head; distinguish developer-tested from independently qualified.

**Boundaries:** no refactoring, new policy, security weakening or extra authority.

**Governance:** inject the **entire** current-revision Archetype C verbatim slice (CA02, CA04, CA06, CA07), each with source-backed Binding. Do **not** merely write “follow CA02–CA07” or ask the receiving builder to perform its own injection. The orchestrator is responsible for compiling it.

The illustrative `DISCOVER AND PIN` placeholder is intentionally **not dispatchable**. Replace it with retrieved identities before execution.

## 7. Adoption, backward compatibility and acceptance of this proposal

This document is a **normative orchestration-process proposal**, not a constitutional article amendment. Prior assignment records and old project adoptions remain unchanged. If adopted, apply prospectively at the next safe assignment boundary; no speculative retroactive refactoring.

**Acceptance checks for adopting the addendum:**
- JSON Schema draft 2020-12 parses, and positive/negative fixture packets validate as expected.
- A complete Archetype C sample with exact clauses, pins and bindings passes the *source-fidelity checker*, whereas a paraphrased or missing clause fails.
- Invalid role D claiming independent qualification, conflicting ownership, unknown current head, unapproved paid spend and unsupported evidence transfer are refused by cross-field/source validation.
- A current existing mergeable PR emits a no-op repair option rather than forced reconciliation.
- A multi-item migration produces A (contract freeze), then B (bounded migration), and keeps D with a genuinely independent owner.
- The governance adoption decision records exact source SHA, scope, effective point and reserved powers; PR merge alone is not adoption.

**CI Scope Declaration:** T2 proposed process/schema addition; source/doc consistency and JSON Schema syntax/fixture contract checks are required. No paid tests, independent software qualification, production or workflow activation is authorized. Any needed compiler/validator implementation is a **separate authorized work package**; this document does not claim a working generator merely because it specifies one.
