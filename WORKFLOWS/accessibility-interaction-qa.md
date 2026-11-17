# Workflow — Accessibility & Interaction QA

## Purpose
Evaluate accessibility and interaction quality across key screens, components, and user journeys.

## Inputs
- UI frames or accessible rendered interface.
- Component states and interaction flows.
- Supported devices/browsers and applicable accessibility target (for example, WCAG level).
- Existing semantic/ARIA implementation where code is available.

## Process
1. Confirm the applicable standard and test scope.
2. Review semantic structure, headings, labels, names, roles, and meaningful alt text.
3. Check keyboard access, focus order, visible focus, and escape/return behavior.
4. Assess contrast, text resizing, touch target usability, and motion considerations.
5. Test loading, empty, success, error, disabled, and confirmation states.
6. Review sensitive actions for clear intent and confirmation.
7. Record reproducible findings, severity, evidence, and remediation.
8. Retest after approved fixes.

## Outputs
Accessibility report, interaction-state matrix, issue list, and retest evidence.

## Guardrails
Do not claim formal conformance from a partial review. State which checks were manual, automated, not tested, or blocked. Code or design changes require L3 approval.
