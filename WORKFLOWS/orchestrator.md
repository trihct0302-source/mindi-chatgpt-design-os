# Workflow — Central Orchestrator

## Purpose
Coordinate the six specialist workflows, preserve shared task context, and enforce governance from intake through verification.

## Intake contract
Capture:
- Request and intended outcome.
- Project/page/component scope.
- Source links and identifiers.
- Deadline/priority and named PIC/approver.
- Constraints, exclusions, and acceptance criteria.
- Requested operating level (default L0–L2).

## Routing
| Request type | Primary workflow | Optional handoff |
|---|---|---|
| Inspect Figma / interpret brief | Figma Design Assistant | Design QA |
| Define or audit tokens/components | Design System Manager | Figma–Code Sync |
| Review visual/layout quality | Design QA & Audit | Accessibility QA |
| Implement approved design | Frontend Design & Builder | Accessibility QA |
| Compare design and code | Figma–Code Sync | Design System Manager |
| Keyboard, semantics, WCAG, UI states | Accessibility & Interaction QA | Design QA |

## Shared execution sequence
1. **Intake:** confirm request, outcome, scope, urgency, PIC, stakeholders, and constraints.
2. **Discovery:** inspect only accessible and authorized sources; list missing inputs.
3. **Analysis:** produce evidence-based findings and classify observed/inferred/assumed/unknown.
4. **Proposal:** recommend a bounded change, affected artifacts, risks, acceptance criteria, and rollback considerations.
5. **Approval:** require explicit L3 authorization before any write or external side effect.
6. **Execution:** perform only the approved operation and report deviations immediately.
7. **QA:** verify against acceptance criteria and record test evidence.
8. **Release recommendation:** summarize readiness; merge/publish/deploy remain separate approval decisions.
9. **Version:** record PR/commit, artifacts, date, owner, and unresolved issues.

## Handoff contract
Every specialist handoff includes: task ID/title, objective, source references, scope, findings, assumptions/unknowns, proposed action, approval state, dependencies, owner, and expected output.

## Stop and escalate
Stop if a source is missing, access is denied, requirements conflict, scope expands, an action is destructive, or the task would exceed the approved L3 boundary. Ask one precise question identifying the blocker.

## Completion report
Return: objective, work completed, evidence, decisions required, remaining risks, next action, PIC, and approval/release state.
