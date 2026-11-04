---
name: cognous-engineering-governance
description: Apply the Cognous Engineering Constitution to authorized software engineering, architecture, orchestration, PR review, defect remediation, CI test scoping, independent qualification, release assessments, adoption and amendment decisions. Use when drafting builder/orchestrator assignments, auditing compliance with EP1–EP7 or CA01–CA23, selecting risk-tiered evidence, controlling parallel work or preparing governance decisions for a Cognous project. Require verified project adoption and source pins; the skill itself never grants authority.
---

# Cognous Engineering Governance

This skill is an operational interpretation of `cogno-us/cognous-engineering-constitution` as inspected on 2026-11-04 at default-branch tree `dcdbe3b76843d672ca3cfb1f000124ecd78ed03c`. It is **not an adoption act, license to act, replacement for the exact locally adopted revision or independent certification**. For any binding compliance assertion, fetch the adopted exact revision from GitHub and compare original bytes. Repository HEAD may have changed. The locally bundled reference material provides a self-contained operational guide but source documents prevail on a conflict.

## Non-negotiable decision hierarchy

1. Respect applicable law, security controls, valid contracts, reserved decisions, and project-specific instructions.
2. Identify the project's authorized **exact constitutional revision**, adoption scope, effective time, exceptions and controlling source/configuration pins under `ADOPTION.md`. Publication or merge alone does not adopt a constitution or addendum. If unavailable, classify **UNVERIFIED** and refuse the affected authority-sensitive action.
3. Follow EP1–EP7 and CA01–CA23 for the applicable adopted revision. Adopted project controls and stronger required checks remain effective.
4. Apply risk-tiered testing `TESTING_POLICY.md`, orchestration `ORCHESTRATION.md` and task-scoped compliance `ENGINEERING_COMPLIANCE_ADDENDUM.md` **only within their applicable adoption status**. `ORCHESTRATOR_PROMPT_ENGINEERING_ADDENDUM.md` expressly describes itself as a proposal, not automatically adopted.
5. Never conflate a contribution, inspection, developer test, independent qualification, certification, canonical integration, organizational adoption, release, deployment and production qualification. None implies the next.

Read these bundled references as needed:
- [Constitutional article catalog and exact text](references/constitutional-articles.md): exact CA table; EP crosswalk; hard constraints.
- [Assignment and orchestration](references/orchestration-assignments.md): eight-field packet, role/archetype routing, parallelism, blockers, batch migrations, merge controls, telemetry.
- [Testing, evidence and qualification](references/testing-qualification.md): T0–T4, three testing levels, evidence reuse, CI Scope Declaration, acceptance states.
- [Adoption, amendments and provenance](references/adoption-authority.md): who may adopt, revision selection, amendments, source provenance and retained negatives.
- [Operational templates and gates](references/templates.md): copyable assignment, review, decision, handoff and blocker formats.
- [Source manifest](references/source-manifest.md): exact repository paths, observed tree, statuses and hyperlinks.

## Default working procedure

1. **Discover** actual repo/project, branch/head, adopted constitution, governing project plan, legitimate authority, task and prior decisions. Use a connected GitHub tool if available; otherwise identify missing evidence, never fabricate SHAs, decisions, access or a pass.
2. **Classify** role, primary task archetype A–D (if compiling an assignment), independently assess highest reachable testing tier T0–T4, and identify impacted EP/CA clauses. Article slices are a minimum, not a limit.
3. **Reconcile before implementation**: reuse qualified components (CA01); identify fixed source/contract/external commitments and intended acceptance (CA03); implement only smallest complete authorized scope (CA02); freeze shared contracts before parallel migrations when applicable.
4. **Enforce authority**: actor/role/domain/action/context/time/limits/issuer, ownership, expiry and revocation. No technical capability, model suggestion, signature, receipt, merge button, coordination role or worker title creates authority. No unapproved spending, production calls, releases, security exceptions or governance changes.
5. **Plan falsifiable evidence** before coding or acceptance. Preserve independent oracles and original adverse evidence. Test current affected paths, negatives and failures based on actual reachability; do not substitute one mocked happy path for critical behavior.
6. **Perform only authorized work**. Parallelize disjoint pinned inputs, serialize canonical/shared mutations, keep PRs reviewable. Resolve routine blockers and corrections autonomously when delegated. Do not manufacture code changes where the reported defect is already fixed.
7. **Report accurately**: cite exact source, configuration, environment and observed results. Identify FAILED, BLOCKED, NOT EXECUTED, NOT APPLICABLE distinctly. Prior PASS is reusable only with established applicability. State unknowns explicitly.
8. **Gate handoff and integration**: verify exact final head, required checks, reviews, independently qualified obligations, and reservation of merge authority immediately before merging. Verify post-merge identity. Integration is neither acceptance nor deployment by itself.

## Assignment compilation

When asked to instruct a builder or orchestrator, return one **self-contained eight-field packet**, with headings in this exact order: `Identity`, `Authority`, `Ownership`, `Inputs`, `Acceptance`, `Delivery`, `Boundaries`, `Governance`. Define the operational meaning of the selected archetype in Identity. Include source-backed exact pins and task-specific article bindings in Governance. Read [orchestration-assignments](references/orchestration-assignments.md) and [constitutional-articles](references/constitutional-articles.md). If formal structured data is requested, validate to the repository's `schemas/orchestrator-assignment-v1.schema.json` and separately check source fidelity, cross-field consistency, real existence and adoption. Schema validation alone proves neither authority nor semantic compliance. Do not claim mechanical clause validation unless performed.

For user-requested builder instructions, output instructions in a **single code block**, include references to the governing static project plan and Engineering Constitution, and begin with `Put the maximum number of parallel agents to work within authorized, nonconflicting scopes.` This is presentation preference only; it does not create worker/spend authority.

## Risk and claims

Use T0 editorial; T1 isolated low consequence; T2 interface/composition; T3 governance/safety-critical reachable change; T4 prescribed acceptance milestone. The constitution also includes **Tier 1–3 review classifications**, which are not the T0–T4 testing taxonomy. Never conflate them. Change consequence and transitive reachability, not lines of code or archetype, set testing tier. Risk-tiered developer CI does not replace prescribed independent qualification. Keep paid/production/full-cohort campaigns OFF unless specifically authorized.

Use `PROPOSED`, `DOCUMENTED`, `IMPLEMENTED`, `DEVELOPER-TESTED`, `INDEPENDENTLY QUALIFIED`, `INTEGRATED`, `DEPLOYED`, `PRODUCTION-QUALIFIED` only for evidence supporting that exact stage. Distinguish `PASS`, `FAIL`, `BLOCKED`, `NOT ASSESSED/NOT EXECUTED`, and evidenced `N/A` at test-case level. Never revise a frozen oracle to fit output, erase failure evidence, or label skipped required checks PASS.

## Stop/escalate conditions

Escalate one actionable, source-backed decision packet for missing controlling contract, unresolved architecture, governance invariant, security/identity grant, external-effects authority, qualification-rule changes, contract migration, spending beyond an approved cap, release/deployment approval or required independence. Include missing fact, exact source, affected scope, supported alternatives, risk/evidence impacts and decision requested. Continue other independent authorized work. No repeated planning loops or fabricated policy defaults. A missing source is not permission.

## Source discipline

The full repository files, including proposed addenda, are authoritative only to the extent the adopting context selects them. Retain exact references and predecessor evidence. Never treat copied normative article text in this package as automatically synchronized with later repo revisions. Check [source-manifest](references/source-manifest.md) when assessing source freshness. If an adopted text differs, use that exact text rather than this snapshot and disclose the divergence.


---
To read any file's contents, use `functions.exec` to run `text(await tools.skills__read({"uri": "skills://cognous-engineering-governance/<relative_file_path>"}))`.
Read once per file. Available relative file paths:

SKILL.md
agents/openai.yaml
assets/icon.svg
references/adoption-authority.md
references/constitutional-articles.md
references/orchestration-assignments.md
references/source-manifest.md
references/templates.md
references/testing-qualification.md