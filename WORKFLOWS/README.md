# Workflows

Six workflows are coordinated by the central orchestrator. Each workflow follows the shared lifecycle and approval policy in `00_CORE`.

| Workflow | Input | Output |
|---|---|---|
| Figma Design Assistant | Figma URL, brief, target frames | Design report, UX/UI findings, proposals |
| Design System Manager | Figma variables/components, code tokens | Token map, component inventory, governance actions |
| Design QA & Audit | Frames, screenshots, design specs | Severity-ranked issue list and QA report |
| Frontend Design & Builder | Approved Figma node/spec, source code, stack | Implementation proposal, code/preview/tests when approved |
| Figma–Code Sync | Design tokens/components, repository | Mapping and drift report |
| Accessibility & Interaction QA | UI, component states, flows, test environment | Accessibility and interaction report |

No workflow may bypass L3 approval for execution. Workflow definitions specify purpose, prerequisites, steps, outputs, and stop conditions.
