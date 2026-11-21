# 4C AI-native Equity Intelligence — Product Architecture

Status: Concept architecture for validation; not a production specification  
Project ID: LV-2026-001

## 1. Product thesis

Build an AI-native system that helps a founding team complete the bounded task of exploring and comparing initial equity-structure scenarios. The product applies authorized and expert-validated equity-design experience assets through a controlled workflow.

It is not:
- a generic legal chatbot;
- a cap-table ledger replacement in the first release;
- a percentage calculator without professional reasoning;
- an autonomous lawyer or final legal decision-maker;
- a replica of the historical 4C service menu.

## 2. Initial job-to-be-done

"When our founding team is forming or reorganizing, help us make sense of roles, contributions, commitments, ownership scenarios and control implications, so that we can compare options and prepare a well-structured professional discussion."

### Core users
- founder / team organizer;
- co-founder or founding team member;
- authorized startup advisor.

### Buyer hypotheses
- founders / startups;
- incubators / accelerators;
- startup advisory platforms or professional partners.

Buyer and willingness-to-pay must be validated in G0 and G3.

## 3. MVP workflow

1. **Workspace setup:** jurisdiction, entity type / stage, team and intended task.
2. **Guided intake:** roles, cash contributions, non-cash contributions, time commitment, responsibilities, future milestones, existing agreements and preferences.
3. **Missing-information detection:** identify contradictions, gaps and questions that materially affect scenario construction.
4. **Experience application:** call approved experience assets and transparent rules; show which assumptions are used.
5. **Scenario generation:** create alternative scenarios for user comparison; do not present one as automatically correct.
6. **Deterministic calculations:** calculate percentages, pools, dilution and scenario arithmetic in tested functions.
7. **Impact explanation:** explain control, incentive, governance and future-event considerations within the product's approved scope.
8. **Report export:** assumptions, scenarios, unresolved questions, sensitivity and professional-review checklist.
9. **Professional escalation:** route special structures, disputes, tax, regulated securities, cross-border or high-impact legal issues to appropriate professionals.

## 4. System layers

### A. Experience Asset Layer
- Experience Profile;
- domain vocabulary and entity definitions;
- validated decision rules and heuristics;
- scenario / exception catalogue;
- permitted source references;
- test cases and evaluator rubric;
- version, contributor and license metadata.

### B. Orchestration Layer
- guided conversation and structured intake;
- workflow / state machine;
- retrieval with provenance;
- Agent task decomposition;
- rule selection and scenario orchestration;
- escalation and refusal routing.

### C. Deterministic Computation Layer
- share allocation arithmetic;
- pool sizing;
- dilution calculations;
- scenario comparison;
- validation of sums, constraints and data consistency.

All formulas must be explicit, versioned and unit-tested. LLM output may propose input assumptions but must not be the source of arithmetic truth.

### D. Product Interface
- founder/team workspace;
- member and contribution questionnaire;
- scenario comparison;
- assumptions and rationale;
- report and export;
- professional review handoff.

### E. Governance and Observability
- source citations / provenance;
- tenant and role-based access;
- consent and data-use permissions;
- audit events;
- evaluation and feedback records;
- model / prompt / rule versions;
- deletion and export;
- issue reporting and rollback.

## 5. Data objects

- Organization / Venture
- Person / Role (only necessary business data)
- Contribution / Commitment
- Equity Scenario
- Pool / Instrument
- Financing Event
- Rule / Assumption
- Evaluation Case
- Report
- Consent / Permission
- Audit Event

Do not collect sensitive personal data unless it is essential, justified and lawfully processed. Use synthetic data in development.

## 6. Boundaries and escalations

The MVP may provide decision support and scenario exploration. It must not:
- determine a single legally correct allocation;
- create or alter legal ownership records;
- execute securities issuance, transfer or repurchase;
- provide unreviewed advice on tax, securities, employment, foreign investment or complex corporate structures;
- assume equal legal treatment across jurisdictions;
- infer agreement or consent of a co-founder who has not participated.

Escalate where there is disagreement, coercion, existing dispute, complex vesting, cross-border ownership, regulated fundraising, tax consequences, employee incentive plan design or missing material information.

## 7. Quality dimensions

- intake completeness;
- consistency of facts and assumptions;
- correct calculations;
- provenance of professional rules;
- explainability of scenario differences;
- calibrated uncertainty;
- edge-case detection;
- appropriate escalation;
- privacy / permission compliance;
- task completion and user comprehension.

## 8. Architecture decisions to validate

| Question | Initial direction | Validation |
|---|---|---|
| Frontend | Lightweight responsive web app | Founder usability test |
| Backend | Simple API + relational data store | Data model and audit needs |
| LLM | Provider-agnostic model adapter | Task eval and cost comparison |
| Retrieval | Source-aware retrieval over approved assets | Grounding / citation eval |
| Calculation | Deterministic module with unit tests | Golden test set |
| Agent | Task-specific orchestrator | Task completion and safety eval |
| Auth / tenant | Role-based access and tenant isolation | Security review |
| Deployment | Staging first, production only after gate | Release checklist |

Do not over-engineer. Choose the simplest architecture that can pass the stated product and governance criteria.
