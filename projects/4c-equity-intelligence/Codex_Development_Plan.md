# 4C AI-native Equity Intelligence — Codex Development Plan

Project ID: LV-2026-001  
Status: Planning only; development start requires L3/L4 rights and experience gates.

## 1. Engineering objective

Use Codex as the primary software engineering execution layer to build a small, testable MVP around a bounded founder-team equity scenario workflow.

Codex reduces repetitive engineering effort; it does not remove the need for product decisions, architecture review, professional evaluation, security controls or customer validation.

## 2. Repository rules

- Work on a dedicated project branch.
- Keep each change small and reviewable.
- Every task has acceptance criteria.
- Tests are required for calculations, rules and material workflows.
- Use synthetic fixtures by default.
- No client names, case materials, personal data, confidential contracts, secrets or API keys in prompts, code, tests, logs or Git.
- Never put production credentials in repository files.
- No direct production deployment from an unreviewed branch.
- Human approval required before merge, release and deployment.
- Preserve auditability of rule, prompt, model and product versions.

## 3. Suggested initial application structure

This is a proposal, not a mandated stack. Select the simplest implementation that meets product requirements.

- app / frontend: responsive guided intake and scenario comparison;
- api: project, user, scenario and report endpoints;
- domain: versioned entities and validation;
- experience-assets: approved rules, source references and content metadata;
- calculation: deterministic allocation, pool and dilution functions;
- agent: intake assistance, missing-information detection and explanation;
- evaluation: golden cases, property tests, edge cases and regression suite;
- security: auth, tenancy, consent, audit and data retention;
- docs: product spec, threat model, deployment and support runbook.

## 4. Work packages

### WP0 — Repository and security foundation
Acceptance:
- README and contribution guide;
- environment-variable handling;
- synthetic fixtures only;
- lint / build / test checks;
- secrets scanning and dependency review;
- branch and PR workflow.

### WP1 — Domain model and intake
Acceptance:
- entity / person / role / contribution / scenario model;
- required-field validation;
- missing-information prompts;
- no hidden defaults for material facts.

### WP2 — Deterministic calculation engine
Acceptance:
- explicit formula specification;
- unit tests for sums, rounding, dilution and invalid inputs;
- property-based tests where appropriate;
- golden test cases reviewed by a domain expert;
- version and assumptions recorded in each result.

### WP3 — Experience and rule orchestration
Acceptance:
- every rule has asset ID, source, version and permission status;
- rules distinguish hard constraints, heuristics and expert discretion;
- unknown / unsupported scenarios trigger hold or escalation.

### WP4 — Scenario comparison and explanations
Acceptance:
- at least two alternative scenarios where suitable;
- assumptions and trade-offs visible;
- explanation cites the relevant approved experience assets;
- no claim that a generated option is the legally correct answer.

### WP5 — Report export and review handoff
Acceptance:
- structured report with assumptions, outputs and unresolved questions;
- review checklist;
- exportable audit summary;
- no direct modification of legal ownership records.

### WP6 — Evaluation, security and pilot readiness
Acceptance:
- evaluation record complete;
- critical scenarios pass;
- privacy / data-flow / access review;
- failure and rollback path;
- pilot agreement and consent process approved.

## 5. Definition of done

A feature is done only when:
- acceptance criteria pass;
- automated tests pass;
- code and dependencies are reviewed;
- UI behavior and failure states are checked;
- source / rule provenance is preserved;
- logs do not leak sensitive data;
- documentation is updated;
- known limitations are disclosed;
- a human reviewer approves the PR.

## 6. Engineering cost discipline

- Prefer existing managed infrastructure over custom platform building.
- Avoid multi-agent orchestration unless a measured task requires it.
- Use one model interface with provider abstraction only where it prevents real lock-in cost.
- Cache safe, non-sensitive computations.
- Measure cost per completed customer task, not just token cost.
- Do not add features without a customer task, acceptance test and owner.
- Stop building after the agreed MVP scope; use pilot evidence to decide what to build next.

## 7. Required Codex task prompt

Each Codex task should provide:
- project goal and task context;
- repository guidance to read;
- files in scope;
- expected behavior;
- acceptance criteria;
- test commands;
- security / data constraints;
- prohibited changes;
- required PR summary.

Codex must report what it changed, tests run, tests not run, known risks and follow-up work. It must not claim tests passed if they were not executed.
