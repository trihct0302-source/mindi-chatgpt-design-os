# Approval Policy

## Operating levels
| Level | Name | Allowed activity | Default |
|---|---|---|---|
| L0 | Read | Read accessible sources, collect metadata, summarize structure | Allowed |
| L1 | Analyze | Compare, audit, diagnose, calculate, and identify risks | Allowed |
| L2 | Propose | Draft recommendations, specifications, diffs, plans, and test cases without applying them | Allowed |
| L3 | Execute | Write or modify Figma/code/design-system artifacts, commit, merge, publish, or deploy | Explicit approval required |

## Approval gate
**Review → Approve → Execute → Verify → Version**

An approval must specify:
- Target artifact/repository/project.
- Exact scope and intended outcome.
- Permitted operations.
- Excluded operations.
- Acceptance criteria.
- Whether commit, merge, publish, or deploy is included.

Approval for one artifact or task does not authorize unrelated changes.

## Execution controls
1. Present the proposed change and expected impact.
2. Obtain explicit approval for L3.
3. Execute only the approved scope.
4. Verify the result against acceptance criteria.
5. Record changed files, commit/PR references, test evidence, and unresolved issues.

## Actions requiring separate approval
- Editing or publishing Figma source files.
- Editing product source code beyond an approved implementation task.
- Changing shared design tokens or component libraries.
- Committing to protected/default branches, merging PRs, or deploying.
- Destructive operations, data migrations, or permission changes.

## Stop conditions
Stop and ask for clarification when scope is ambiguous, sources conflict, access is insufficient, a destructive side effect is possible, or acceptance criteria cannot be verified.
