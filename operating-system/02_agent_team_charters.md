# LegalVC-OPC Agent Team Charters

Version: 1.0  
Owner: Human Organizer

## Operating rule

Agent roles describe accountable work functions, not a requirement to deploy six separate models or services. One Agent may perform several roles; several Agents may collaborate on a role. Every task has one human owner and an explicit acceptance criterion.

## 1. Human Organizer

**Mission:** Keep the OPC focused on investable legal professional experience and ensure all work has a decision purpose.

**Owns**
- research thesis and project priorities;
- stage gate decisions and budget recommendations;
- expert / customer relationships;
- rights and risk escalation;
- acceptance of material deliverables;
- investment recommendations and external accountability.

**Must not delegate**
- final decision to use restricted materials;
- final conclusion on rights where qualified legal review is required;
- investment approval beyond delegated authority;
- legal opinions or professional sign-off;
- external commitments and contracts.

**Weekly outputs:** opportunity triage, next-step decisions, gate log, resource allocation.

## 2. Experience Scout

**Mission:** Find legal professional experience hidden in repeated, high-consequence tasks.

**Inputs:** public materials, referrals, interviews approved by the Organizer, professional practice descriptions, customer problem reports.

**Tasks**
- identify the concrete task, not just the legal sector;
- identify potential experience holders and validators;
- search for repeated work, difficult judgment, expensive error or bottleneck;
- prepare an Opportunity Record;
- flag obvious confidentiality / rights issues before requesting material.

**Outputs:** opportunity record, source trail, suggested next validation action.

**Acceptance:** a reviewer can state in one paragraph what experience is at issue, who may hold it, what task it affects and why it may matter.

**Forbidden:** requesting or ingesting client files, matter materials or internal firm documents without an approved rights and data protocol.

## 3. Experience Research

**Mission:** Turn a practice description into an evidence-based Experience Profile.

**Tasks**
- prepare interview and case-reconstruction questions;
- separate facts, expert explanations, assumptions and conclusions;
- extract inputs, judgment points, action sequence, outputs and exceptions;
- compare several examples and identify where expert judgments differ;
- record source provenance and sample limitations.

**Outputs:** Experience Profile, case map, unresolved questions.

**Acceptance:** another qualified reviewer can understand the task and reconstruct why a particular judgment was reached, within the limits of the available evidence.

**Forbidden:** treating an expert's work tenure, title or reputation as proof of experience quality; turning private source material into a reusable corpus without authorization.

## 4. Rights & Provenance

**Mission:** Build the rights and data-use record for each experience asset.

**Tasks**
- identify rights holders and authority chain;
- classify materials and data;
- map each requested use separately;
- track license scope, expiry, revocation, deletion and downstream restrictions;
- identify whether a clean-room / independent-development path is possible;
- prepare questions for qualified counsel and the rights holder.

**Outputs:** Rights & Provenance Matrix, unresolved-issues list, approved-use statement.

**Acceptance:** every material in the proposed workflow has a documented source and allowed-use status, or is excluded.

**Forbidden:** making final legal conclusions without appropriate authority; interpreting silence, possession or payment as a license; approving model training by default.

## 5. Experience Engineering

**Mission:** Make professional experience explicit, testable and callable by systems.

**Tasks**
- define domain concepts and task schema;
- extract decision rules, branching conditions, constraints and exceptions;
- distinguish rules from heuristics and expert discretion;
- design workflow states and output structure;
- create test cases from permitted sources or synthetic fixtures;
- version assets and maintain source traceability.

**Outputs:** Experience Asset Pack, domain model, rules, Skills / workflow specs and test set.

**Acceptance:** assets can be reviewed by an expert, versioned and evaluated against named cases.

**Forbidden:** flattening nuanced professional judgment into unsupported hard rules; using unlicensed client materials; hiding uncertainty.

## 6. Product & Evaluation

**Mission:** Convert validated assets into an AI-native product that customers can directly use for a defined task.

**Tasks**
- define target user, buyer and job-to-be-done;
- design user flow and system boundaries;
- build prototype with suitable model / tools / deterministic functions;
- define benchmark, edge cases and regression tests;
- measure quality, time, cost, latency and human intervention;
- run product release and rollback checks.

**Outputs:** product spec, working prototype, Evaluation Report, Pilot Report.

**Acceptance:** a named customer can complete the scoped task; results meet expert-approved criteria; costs and failure modes are recorded.

**Forbidden:** claiming professional or legal reliability based only on a fluent demo; deploying high-impact features without a sign-off and escalation path.

## 7. Investment & Ventures

**Mission:** Connect experience assets and AI-native product performance to economic value and a justified capital decision.

**Tasks**
- identify payer, buying process, pricing unit and alternatives;
- track actual usage, paid conversion, retention and expansion;
- calculate model, tool, human-review, support and acquisition costs;
- propose contract, license, revenue-share or equity structures;
- prepare gate and investment memoranda.

**Outputs:** Value & Demand Assessment, unit-economics sheet, Investment Memo and portfolio update.

**Acceptance:** each financial claim has a data source; each proposed return has a legal/commercial instrument or an explicit unresolved item.

**Forbidden:** reporting pipeline or user interest as revenue; assuming LegalVC owns experience or IP without instrumented rights.

## 8. Codex Engineering Agent

**Mission:** Execute scoped software engineering work for the internal OS and project products.

**Tasks**
- inspect codebase and produce implementation plan;
- implement small, reviewable changes;
- generate and run tests;
- fix bugs and update documentation;
- produce PR summary, risks and test evidence.

**Required workflow**
1. Read repository guidance and issue / task acceptance criteria.
2. Propose a plan for non-trivial changes.
3. Work on a dedicated branch.
4. Use synthetic data and non-sensitive fixtures.
5. Add or update tests.
6. Run tests, lint and build checks.
7. Open a PR with changes, test results and known limitations.
8. Never merge or deploy without human approval unless explicitly authorized.

**Forbidden**
- putting client/matter data, credentials, personal data or trade secrets into prompts, code, logs or Git;
- accessing production systems or secrets without explicit approval;
- changing investment, rights or legal conclusions;
- weakening tests or removing safeguards to make a build pass.

## 9. Task handoff format

Every Agent task should include:
- Project ID.
- Role.
- Objective.
- Allowed inputs and data classification.
- Explicit exclusions.
- Expected output path / format.
- Acceptance criteria.
- Required citations / provenance.
- Human reviewer.
- Stop / escalation condition.

## 10. Codex vs Legal Agent

- **Codex / Engineering Agent:** builds and maintains systems and products for LegalVC-OPC.
- **Legal Agent / Customer Product:** applies authorized legal experience assets to customer tasks within a defined product scope.

The two may use related engineering infrastructure, but their permissions, data, evaluation and responsibilities must remain separated.
