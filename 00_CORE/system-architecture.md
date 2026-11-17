# System Architecture

## Purpose
MINDI ChatGPT Design OS is an integrated, approval-governed operating model for design discovery, design-system management, design QA, frontend translation, Figma–code alignment, and accessibility QA.

## V1 boundary
- Pilot: `mindi-landing`.
- Deliverables in this repository: documentation, Skills, and Workflows only.
- No direct edits to Figma files, product source code, production data, or deployment targets in V1 setup.
- No Figma URL has been supplied yet; Figma-dependent tasks must remain in intake/discovery until a valid source is provided.

## Operating model
A central orchestrator receives a request, classifies the work, selects one or more specialist workflows, maintains task context, enforces approval gates, and consolidates evidence into a final report.

### Six specialist workflows
1. **Figma Design Assistant** — inspect design sources, interpret briefs, review UX/UI, and propose design directions.
2. **Design System Manager** — inventory tokens/components, map design-to-code conventions, and govern versions.
3. **Design QA & Audit** — inspect frames/screenshots for layout, hierarchy, consistency, and visual defects.
4. **Frontend Design & Builder** — translate approved design specifications into implementation plans, code proposals, previews, and tests.
5. **Figma–Code Sync** — compare design tokens/components with repository implementation and report drift.
6. **Accessibility & Interaction QA** — assess semantics, keyboard operation, contrast, focus, states, and interaction feedback.

## Shared lifecycle
Intake → Discovery → Analysis → Proposal → Approval → Execution (only when authorized) → QA → Release recommendation → Version record.

## Sources of truth
- Figma: design artifacts, frames, variables, and component-library references.
- GitHub: versioned source code, Skills, Workflows, technical documentation, and change history.
- Approved project brief: product intent, audience, scope, constraints, and acceptance criteria.
- QA evidence: screenshots, test results, issue lists, and verification records.

When sources conflict, do not silently choose. Record the conflict, identify the authoritative owner, and request a decision.

## System outputs
Every completed task should produce: request summary, source inventory, findings, assumptions/unknowns, recommendations, approval state, QA evidence, and version/change record where applicable.
