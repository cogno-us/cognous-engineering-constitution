# Task-Scoped Engineering Compliance Injection — v1.0

**Status:** Proposed normative orchestration addendum, subject to competent adoption under [ADOPTION.md](ADOPTION.md). **Scope:** engineering assignment generation, not a new constitutional article or automatic adoption. **Source of clauses:** [ENGINEERING_CONSTITUTION.md](ENGINEERING_CONSTITUTION.md), CA01–CA23. **Companion:** [TESTING_POLICY.md](TESTING_POLICY.md). The exact article text below was copied from the existing constitutional article table; inspect against the selected revision before expanding a packet.

## 1. Requirement and boundary

For each bounded assignment, select the **role** and the **primary task archetype**, then include its canonical constitutional slice in the eight-field assignment packet's Governance field. Supply a short **task-specific binding**, without altering or paraphrasing the normative source text. The Acceptance field declares risk tier, exact evidence sources and sufficient tests. Always include the *exact full governing revision identity* and links to the complete Constitution, orchestration guidance and testing policy, so the slice does not replace governing requirements.

This is a **fixed lookup and mechanical text expansion** where supported, not a request for an LLM to freely summarize, reconstruct or choose constitutional wording from memory. For all contexts, verify source exactness. If the selected revision lacks the slice text, **stop and reconcile**; do not silently substitute remembered wording. A prompt alone does not establish cryptographic or programmatic determinism; a renderer should verify template IDs, canonical bytes and fillable slots before dispatch.

## 2. Routing axes and deterministic selection

**Role axis:** `implementation_owner`, `independent_qualification_owner`, `orchestrator`, or other explicitly authorized local role. The role supplies authority and independence bounds. Role alone does not authorize execution or change an assignment's archetype. An `independent_qualification_owner` performing qualification uses **D**; an implementation owner cannot claim D's independent standing by selecting D. No archetype expands scope.

**Task axis:** exactly one primary archetype A–D, with secondary applicable constraints explicitly added. If the work combines incompatible archetypes (for example design plus qualification or schema freeze plus rule migration), split into separate work packages where possible. The mapping is a **minimum default slice**, not a cap on relevant controlling clauses. If other articles, requirements, local adoption rules or security holds apply, include them via exact reference and explicit bind, adding verbatim text if indispensable. Do not omit law, adopted project controls or constitutional obligations merely to meet a word count.

| Archetype | Trigger | Canonical default article IDs | Risk routing |
|---|---|---|---|
| **A** | Contract/schema/registry/shared-boundary design; interface, policy representation or canonical state boundary changes | CA01, CA03, CA04, CA18, CA21 | T2/T3 based on changed boundary |
| **B** | Scoped feature/leaf migration against reviewed frozen interface; reclassify if authority or execution is affected | CA02, CA04, CA05, CA09, CA15 | T1–T3 based on reachable effects |
| **C** | Bug, failing CI, regression or build repair; risk from impacted path | CA02, CA04, CA06, CA07 | Impact-dependent T0–T3 |
| **D** | Independent qualification specification, execution or verdict by qualified owner | CA04, CA06, CA07, CA08, CA23 | T4 for prescribed qualification; protocol changes may be T3 |

## 3. Canonical clause slices — verbatim table cells

The following **Required behavior** and **Prohibited shortcut** entries are verbatim copies from the source's CA table. Heading labels are aids, not rewritten requirements. A compliant generator copies the displayed source cells exactly and separately appends a task-specific binding; it does not silently edit the quoted normative text.

### Archetype A

| Article | Required behavior — exact source | Prohibited shortcut — exact source |
|---|---|---|
| CA01 — Reuse Before Build | Inspect and reuse qualified, versioned components. | Duplicate an owned capability for convenience. |
| CA03 — Contract Before Code | Identify the controlling source, external reliance boundary, duties, expected acceptance and the authority by which a proposed change may acquire canonical standing. | Start against an unnamed or mutable contract. |
| CA04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. |
| CA18 — Governed Policy and Protected Invariants | Version, authenticate and review governance-critical policy and rule changes; protect established mandatory invariants against configuration override. | Treat unreviewed settings or evaluator changes as governing authority, weaken mandatory checks or introduce an unaccountable decision path. |
| CA21 — Boundary Commitments | Preserve relied-upon external semantics or obtain an explicit authorized compatibility transition. | Introduce silent contract, rights, evidence or interface regressions through internal refactoring. |

### Archetype B

| Article | Required behavior — exact source | Prohibited shortcut — exact source |
|---|---|---|
| CA02 — Minimum Sufficient Implementation | Deliver the smallest complete authorized capability. | Speculative architecture, infrastructure, dependencies or scope expansion. |
| CA04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. |
| CA05 — Fail Closed Without Inventing Policy | Apply specified conservative treatment and expose missing semantics. | Invent a cause, grant, floor, deadline, mapping or default. |
| CA09 — Safe Parallelism | Parallelize independent work against pins; serialize conflicting canonical contract, state, schema, admission and integration changes. | Concurrent conflicting authority mutations. |
| CA15 — Bounded Changes and Reversible Integration | Keep changes reviewable with migration/rollback and recorded irreversible authority. | Bundle unrelated architecture or erase history. |

### Archetype C

| Article | Required behavior — exact source | Prohibited shortcut — exact source |
|---|---|---|
| CA02 — Minimum Sufficient Implementation | Deliver the smallest complete authorized capability. | Speculative architecture, infrastructure, dependencies or scope expansion. |
| CA04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. |
| CA06 — Preserve Original Evidence | Retain consequential decision ancestry, rejected alternatives, objections, adverse findings and supersession where legitimately relevant, subject to privacy and retention limits. | Delete, relabel, overwrite or silently rescore failures. |
| CA07 — Exact-Source Reproducibility | Bind claims to exact source, configuration, governing context and transition evidence; reconstruct authoritative pathways when deterministic execution replay is impossible. | Transfer a pass across revisions. |

### Archetype D

| Article | Required behavior — exact source | Prohibited shortcut — exact source |
|---|---|---|
| CA04 — Qualification Designed Before Acceptance | Distinguish implementation inspection, independent qualification, competent certification and final integration; preserve independence wherever required. | Fit an oracle to implementation or substitute developer tests. |
| CA06 — Preserve Original Evidence | Retain consequential decision ancestry, rejected alternatives, objections, adverse findings and supersession where legitimately relevant, subject to privacy and retention limits. | Delete, relabel, overwrite or silently rescore failures. |
| CA07 — Exact-Source Reproducibility | Bind claims to exact source, configuration, governing context and transition evidence; reconstruct authoritative pathways when deterministic execution replay is impossible. | Transfer a pass across revisions. |
| CA08 — Independently Qualified Delivery | Optimize authorization-to-independently-qualified outcome; distinguish lifecycle evidence. | Treat PR counts, green CI or documents as delivery or qualification. |
| CA23 — Accountable Certification | Separate contribution, inspection, qualification, certification and integration according to risk and governing independence requirements. | Self-certify generated work or treat nominal human involvement as sufficient authority. |

## 4. Binding and assignment compilation protocol

The canonical eight fields remain: **Identity, Authority, Ownership, Inputs, Acceptance, Delivery, Boundaries, Governance**. Do not invent a ninth mandatory field or omit one. Fill these documented slots with values verified from the current repository, not example values:

- `{ROLE}`, `{ARCHETYPE}`, `{CONSTITUTION_REF}`, `{TESTING_POLICY_REF}`
- `{REPOSITORY}`, `{BASE_SHA}`, `{ALLOWED_PATHS}`, `{READ_ONLY_PINS}`, `{FROZEN_CONTRACT_SHA}`
- `{PROHIBITED_ORACLE_PATHS}`, `{ADOPTED_REFUSAL_SEMANTICS}`, `{KNOWN_OUT_OF_SCOPE}`
- `{RISK_TIER}`, `{TARGETED_TEST_COMMANDS}`, `{REUSED_EVIDENCE_SHA}`, `{EVIDENCE_APPLICABILITY}`, `{ESCALATION_GATE}`.

For **each** canonical article row included, provide a separate task-specific **Binding:** with the exact applicable code path, commit/pin, operator authority, refusal or negative control. If unknown, state `UNVERIFIED` and block the dependency; never invent a path, checksum, test, or approval. Distinguish a hard file lock from a suggested code-location bound. A path not listed as writable remains read-only unless permission is explicitly expanded.

**Acceptance rules:** select testing scope from actual reachability, not solely archetype. Provide executable focused commands when verified; otherwise require discovery and recording of exact commands as a preparatory step. Prior evidence may be reused only with exact source/dependency/configuration applicability and affected-path regression proof; byte-identical evaluator/schema alone does not prove unchanged behavior after callers, registry data or hardcoded branches change. Do not promise one refusal test suffices for all T3 cases.

**Governance stays source-accurate:** never paraphrase the copied Required behavior/Prohibited shortcut cells. Local implementation constraints belong in separate Binding text. A generic citation without substantive task-specific binding is inadequate; a curated slice is not a substitute for the full constitution. Deterministic compilation is a target for mechanical generators and should be validated as such before claiming zero drift.

## 5. Failure and escalation behavior

Before issuing a packet, validate archetype/role, 8-field completeness, source-revision and article-text fidelity, live file/commit pins, permitted ownership, risk-tier rationale and required evidence gate. Missing source/contract facts => STOP/UNVERIFIED, then one concise blocker packet under CA11: (1) exact missing fact/counterexample, (2) source and affected scope, (3) alternatives, (4) risk/evidence impact, (5) requested decision. Do not add speculative fallbacks or weaken prior compatibility. Historical contract freezes and independent qualification remain in force.

**Example-only placeholders are never executable instructions:** any displayed SHA, test command or path in examples must be read from an actual repository before dispatch. Maintain refusal of authorization/merge/deployment claims not supported by project-specific authority.
