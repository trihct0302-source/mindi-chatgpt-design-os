# Workflow — Figma–Code Sync

## Purpose
Detect and explain divergence between design-system definitions in Figma and their implementation in code.

## Inputs
- Figma variables, styles, components, and variants.
- Repository token definitions and frontend component inventory.
- Known mapping rules and version references.

## Process
1. Confirm both source versions and scope.
2. Normalize token/component identifiers without destroying original names.
3. Compare values, aliases, modes, variants, states, and component coverage.
4. Classify differences as missing, changed, duplicated, renamed, or implementation-only.
5. Estimate impact and affected surfaces where evidence permits.
6. Propose mapping corrections or migration steps.
7. Request approval before changing either source.

## Outputs
Token comparison, component mapping, drift report, impact assessment, and remediation proposal.

## Guardrails
A mismatch is not automatically an error; document intentional exceptions. Never sync or overwrite sources automatically without explicit L3 approval.
