# Operating Doctrine Review

- Doctrine path: /Users/pranay/Projects/trucking/products/product-09-storage-leasing/OPERATING_DOCTRINE.md
- SHA-256: e14bab7b1964d8b755c9e6c7f5b1c2b44e1d726033fa23aeaee6ce921e271a75
- Generated: 2026-11-05T16:23:10Z
- This is a generated review artifact, not an instruction source.

## SECTION_0

- Label: §0 Start from live truth
- Reviewed: True
- Evidence: Live-truth inspection of staged diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): fixed P09 build break in GST invoice UI (removed nonexistent RentLedgerEntry.lateFee; uses calculateLateFee). Added optional facility GSTIN capture (types/facilityModel/createFacility/registration UI) and passes entered GSTIN/state into invoice generation (no fabricated values). Evidence tier 2: npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green; npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_00_INTEGRATED

- Label: Full doctrine integrated audit
- Reviewed: True
- Evidence: Integrated: P09 GST invoice UI fixed and coherent (computed late fee, optional facility GSTIN capture/additive model+test, entered values only). Diff: docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts. Tests: npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green. Build: npm run build exit 0 (Vite; chunk-size warning only). Residual: estimate-only invoicing, outbox not wired to full-state storageClient, mobile/capture/e-NWR/cold-chain hooks pending.

## SECTION_1

- Label: §1 Outcomes and retained value
- Reviewed: True
- Evidence: Goal for this diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): complete GST/India invoice slice coherently and production-honest. No hardcoded demo/fabricated GSTIN; invoice is an estimate requiring verification. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green. npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_10

- Label: §10 Parallel work and contested state
- Reviewed: True
- Evidence: Performance in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): local computations only; no new network dependencies. npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_11

- Label: §11 Engineering and data integrity
- Reviewed: True
- Evidence: Security/data in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): no secrets; user-entered tax identifiers only; no fabricated GSTIN. docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts.

## SECTION_12

- Label: §12 AI output boundary
- Reviewed: True
- Evidence: Observability in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): deterministic invoice rendering; existing flash/validation patterns preserved. docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts.

## SECTION_13

- Label: §13 Product, operator, and claim reality
- Reviewed: True
- Evidence: Blast radius for diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts) limited to P09. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green.

## SECTION_14

- Label: §14 Documentation and decisions
- Reviewed: True
- Evidence: Documentation/decisions in diff: docs/DECISION_RECORD_UI_OVERHAUL.md updated; docs/reviews/motto_review.md updated by gate flow. Durable audit-plan/persona evidence updates follow in the same workstream. docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green. npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_15

- Label: §15 Completion contract
- Reviewed: True
- Evidence: Preservation in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): no valuable behavior removed; additive optional GSTIN fields and UI fix. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green.

## SECTION_16

- Label: §16 Specialist doctrine routing
- Reviewed: True
- Evidence: Migration/compat for diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): optional GSTIN fields; ledger schema unchanged. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green.

## SECTION_17

- Label: §17 Propagation contract
- Reviewed: True
- Evidence: Readiness for diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): tests/build green; runtime uses local dev services; GST invoice is estimate-only (not filing/legal advice). Residual risks: outbox not wired to full-state storageClient, mobile/capture/e-NWR/cold-chain hooks pending. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green. npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_2

- Label: §2 Truth taxonomy
- Reviewed: True
- Evidence: Canonical ownership preserved in this diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): engine + UI paths only; gstInvoice/offlineOutbox remain canonical modules; no parallel ledger/invoice system added.

## SECTION_3

- Label: §3 Proportional rigor and evidence
- Reviewed: True
- Evidence: Scope bounded to P09 diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): GST invoicing/late-fee estimate UI, facility GSTIN, additive facility model/test. No unrelated products.

## SECTION_4

- Label: §4 Authorization and side effects
- Reviewed: True
- Evidence: Safety/correctness in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): build fixed; late fee computed from real dueDate/principal/asOf; GSTIN/place-of-supply derived from entered values. UI labels estimate/verify. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green. npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_5

- Label: §5 Canonical paths and ownership
- Reviewed: True
- Evidence: Architecture in diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): additive optional fields; pure invoice/late-fee functions; outbox remains separate (not wired into full-state storageClient, avoiding risky parallel persistence).

## SECTION_6

- Label: §6 Semantic salvage and supersession
- Reviewed: True
- Evidence: Testing for diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): full regression 83 tests pass, including facility GSTIN regression (tests/facilityModel.test.ts) and existing gstInvoice/offlineOutbox coverage. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green.

## SECTION_7

- Label: §7 Capability routing
- Reviewed: True
- Evidence: Build/type for diff (docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts): npm run build exit 0 (Vite; chunk-size warning only).

## SECTION_8

- Label: §8 Skills lifecycle
- Reviewed: True
- Evidence: Skills/lifecycle: followed established P09/trucking patterns (canonical engine/UI separation, additive changes, regression tests) and local project instructions/AGENTS; no new skill installed. Diff paths: docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts. npm test -> 10 files, 83 tests passed (incl. facility GSTIN regression); full suite green.

## SECTION_9

- Label: §9 Exploration and durable knowledge
- Reviewed: True
- Evidence: Exploration/durable knowledge: implementation aligns with warehouse/storage audit findings (GST invoicing, facility identity, honest estimates). Audit plan/checklist update with persona reviews 0205/0206/0207 is a follow-up in this session; this diff recorded in docs/DECISION_RECORD_UI_OVERHAUL.md and commit evidence. docs/DECISION_RECORD_UI_OVERHAUL.md, docs/reviews/motto_review.md, src/engine/facilityModel.ts, src/engine/types.ts, src/ui/App.tsx, tests/facilityModel.test.ts.
