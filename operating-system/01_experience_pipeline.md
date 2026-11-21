# Legal Experience Investment Pipeline

Version: 1.0  
Applies to: Every LegalVC experience opportunity  
Owner: Human Organizer

## Purpose

This pipeline prevents LegalVC-OPC from drifting into general legal-tech dealflow. Every opportunity must be anchored to a specific item of legal professional experience and a task where that experience matters.

## Stage map

| Stage | Name | Core question | Exit decision |
|---|---|---|---|
| L0 | Opportunity | What professional experience and task have been observed? | Profile or close |
| L1 | Experience Profile | What is the expert actually doing and judging? | Research, merge or close |
| L2 | Value & Demand | Why is this experience valuable and who needs it? | Rights review, reframe or stop |
| L3 | Rights & Provenance | Can it lawfully be used for this purpose? | Authorized scope, redesign or stop |
| L4 | Experience Engineering | Can the judgment be represented and tested? | Asset pack, further research or stop |
| L5 | AI-native Product & Customer | Can a product complete the target task and obtain real usage/payment? | Scale, iterate, partner or stop |
| L6 | Investment & Return | What resources, rights and returns should LegalVC commit to? | Invest, license, incubate, monitor or exit |

## L0 — Opportunity

### Required information
- Project ID and short title.
- Source and date of discovery.
- Legal task / customer problem.
- Experience holder / contributor, if known.
- Why expertise rather than generic legal information may matter.
- Initial customer / buyer hypothesis.
- Known rights, confidentiality or data constraints.
- Next smallest validation action.

### Pass condition
The opportunity describes a concrete task, a plausible experience source and an observable problem. A broad label such as “AI for law firms” is insufficient.

### Stop / hold
Close or park if no specific task or experience can be identified after initial screening.

## L1 — Experience Profile

Interview or observe the professional work. Separate:
- inputs and factual context;
- issue spotting;
- professional judgment;
- decision options and trade-offs;
- action sequence;
- outputs and quality criteria;
- exceptions and escalation points;
- evidence of outcomes.

Do not infer rights from an expert's possession of a document or involvement in a matter.

**Exit artifact:** completed Experience Profile (template 03).

## L2 — Value & Demand

### Experience value
- Importance and consequence of the task.
- Frequency and repeatability.
- Scarcity and difficulty of acquiring the judgment.
- Outcomes attributable to the experience.
- Transferability to other similar situations.
- Change rate / obsolescence risk.
- Error cost and feasible human controls.

### Customer demand
- User, buyer, budget holder and procurement route.
- Existing alternative and its total cost.
- Task frequency, time and failure costs.
- Evidence of actual workarounds, purchasing or willingness to pay.
- Product adoption barriers and integration needs.

### Required evidence labels
Mark every important statement as one of:
- **F — Fact:** supported by a verifiable primary source.
- **P — Party claim:** reported by a project, expert, customer or partner.
- **H — Hypothesis:** not yet tested.
- **I — Inference:** analytical conclusion derived from other evidence.
- **R — Result:** verified behavior or measurable outcome.

**Exit artifact:** Value & Demand Assessment.

## L3 — Rights & Provenance

Complete the Rights & Provenance Matrix before using source material in a product, model, retrieval system, test dataset, marketing asset or customer deliverable.

Minimum checks:
- identity and authority of each rights holder;
- pre-existing know-how vs institution-owned work product;
- client/matter confidentiality and professional duties;
- copyright, database rights, trade secrets and third-party materials;
- personal data and lawful processing basis;
- permitted purposes: interview, internal research, retrieval, inference, evaluation, model training, product delivery, demonstration, marketing, sublicensing;
- territory, term, customer segment, retention, deletion, revocation and derivative work;
- ownership and licensing of newly developed assets.

**Hard gate:** If required rights cannot be established, do not ingest or use the restricted material. Redesign the work using public, synthetic or independently created material only where that clean-room route is itself lawful and properly documented.

## L4 — Experience Engineering

Define the customer task before selecting the model or tool.

### Experience Asset Pack
1. Task definition and boundaries.
2. Experience Profile and source references.
3. Domain concepts and entities.
4. Judgment points and decision rules.
5. Input requirements and data schema.
6. Workflow / state transitions.
7. Output schema and quality rubric.
8. Exceptions, refusal and escalation rules.
9. Test cases, expected results and evaluator notes.
10. Version, rights and maintenance record.

### Engineering principles
- Deterministic computations must use tested code.
- LLMs may interpret context, ask questions, explain and draft within their scope.
- Every material output should retain provenance to permitted sources.
- Use least privilege, tenant separation and data minimization.
- Build evals before broadening product scope.
- A demo is not proof of reliability.

**Exit artifact:** Experience Asset Pack, prototype and evaluation baseline.

## L5 — AI-native Product & Customer Validation

Test three things independently:
1. **Professional validity:** Does the system reflect the expert's validated approach within the stated scope?
2. **Task utility:** Can the intended customer complete a real task with acceptable effort and outcome?
3. **Commercial behavior:** Does the customer use, pay, reuse, renew or expand?

### Product release criteria
- documented target task and prohibited use;
- acceptable performance on representative and edge-case evals;
- no unresolved critical failure in the intended use scope;
- functional human escalation;
- privacy, security and access control review;
- cost and latency measured per task;
- customer-facing limitations and support route;
- versioned release and rollback path.

### Commercial evidence hierarchy
Intent → scheduled pilot → completed use → signed paid scope → cash collected → repeat usage → renewal / expansion.

Do not report intent or a free demo as revenue validation.

**Exit artifact:** Product Evaluation Record + Pilot Report.

## L6 — Investment & Return

The Human Organizer prepares an Investment Memo covering:
- core experience being invested in;
- evidence and remaining unknowns;
- rights acquired or still required;
- product and customer evidence;
- cash, time, technology and external resources to be committed;
- legal vehicle / contract structure;
- revenue and rights allocation;
- milestones, stop conditions and exit / data disposition.

### Available decisions
- Invest / incubate.
- License / co-develop.
- Paid research or engineering project.
- Commercial partnership.
- Continue validation without new capital.
- Monitor / hold.
- Stop / exit.

Not every form of resource allocation is a financial investment. The legal nature and consideration must be recorded accurately.

## Gate decision record

For each stage transition, record:
- Project ID and stage.
- Date and decision owner.
- Evidence reviewed.
- Decision: Pass / Conditional Pass / Hold / Stop.
- Unresolved conditions.
- Budget released and cost code, if any.
- Next owner, deliverable and due date.
- Reason for decision and dissenting view, if any.

## Universal stop conditions

Stop or suspend the affected activity if:
- core rights / authority cannot be established;
- confidential or personal data is being used outside its permitted scope;
- there is no defensible professional quality standard;
- serious or repeated high-impact errors remain uncontrolled;
- customer demand is not evidenced after the agreed test;
- unit economics cannot plausibly improve within a defined iteration budget;
- project rights, liabilities or revenue allocation cannot be clearly contracted.
