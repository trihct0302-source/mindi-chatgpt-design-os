# Workflow — Frontend Design & Builder

## Purpose
Translate an approved design specification into a frontend implementation plan and, when explicitly authorized, code and test artifacts.

## Inputs
- Approved Figma node/frame and design specification.
- Existing repository and relevant source files.
- Framework, build commands, dependencies, and coding conventions.
- Responsive, accessibility, and acceptance requirements.

## Process
1. Confirm repository, branch, stack, and implementation scope.
2. Inspect existing architecture and reuse patterns before proposing new ones.
3. Map frames/components/tokens to frontend structure.
4. Define responsive behavior, states, semantics, and interaction logic.
5. Present implementation plan and affected-file list.
6. Obtain L3 approval before writing code.
7. Implement only the approved scope.
8. Run available lint, build, unit, visual, and interaction checks.
9. Report evidence, deviations, and remaining risks.

## Outputs
Implementation plan, file-change proposal, code changes when authorized, preview/test evidence, and implementation report.

## Guardrails
- No source-code writes under L0–L2.
- No dependency installation, secrets handling, production data access, merge, or deploy without explicit scope approval.
- Do not claim tests passed unless they were actually run.
