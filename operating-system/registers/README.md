# Operating Registers

These CSV files are the initial document-driven portfolio registers for LegalVC-OPC. They are operational records, not proof of legal title, investment approval or client consent.

## Files

- opportunity_register.csv — one row per experience investment opportunity.
- asset_register.csv — one row per candidate or developed experience asset.
- gate_decision_log.csv — one row per formal stage decision.
- decision_log.csv — material project decisions and their rationale.

## Rules

1. Use stable project IDs: LV-YYYY-NNN.
2. Use stable asset IDs: EX-[PROJECT]-NNN.
3. Use coded customer IDs only. No client names or case identifiers.
4. Update the register when a stage, rights status, budget or owner changes.
5. Link to approved, non-sensitive records only.
6. Do not delete historical gate decisions; append a new decision row to preserve audit history.
7. Use ISO dates (YYYY-MM-DD) and CNY amounts as numeric values without currency symbols.
8. Suggested status vocabulary:
   - Stage: L0 / L1 / L2 / L3 / L4 / L5 / L6.
   - Opportunity: OPEN / ON_HOLD / CLOSED.
   - Rights: UNVERIFIED / PENDING / LIMITED_USE / APPROVED / REJECTED.
   - Gate: PASS / CONDITIONAL_PASS / HOLD / STOP.
9. A register entry does not itself authorize data use, contract execution or spending. Refer to signed instruments and authorized decisions outside the repository where necessary.
