# Workflow — Design System Manager

## Purpose
Create and maintain an inspectable map of design tokens, components, variants, ownership, and versioning across design and implementation sources.

## Inputs
- Figma variables/styles and component libraries.
- Code token files and component inventory, when available.
- Approved brand guidelines and design-system conventions.

## Process
1. Inventory available design and code sources with versions.
2. Extract token names, values, modes, aliases, and usage.
3. Inventory components, variants, states, and documented behaviors.
4. Map design tokens/components to implementation equivalents.
5. Identify duplicates, naming mismatches, missing mappings, and deprecated items.
6. Propose canonical naming, ownership, versioning, and migration notes.
7. Prepare a change proposal for approval where edits are required.

## Outputs
- Token map.
- Component inventory and variant matrix.
- Design-to-code mapping.
- Drift/duplication/deprecation report.
- Proposed changelog and governance actions.

## Guardrails
- Never overwrite source-of-truth tokens or libraries without L3 approval.
- Preserve version, date, owner, rationale, and affected pages/components.
- Deprecated assets must be marked and archived according to the approved governance process, not silently deleted.
