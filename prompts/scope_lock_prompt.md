# Scope Lock Prompt

## Purpose
Freeze the smallest useful version of the application before implementation.

## AI Instructions
- List only the features required for the first localhost version.
- Explicitly state what is excluded.
- Mark assumptions so later changes are visible.
- Warn if the scope is too large for a one-shot build.

## Output Format
```md
## Scope Lock
- Included:
- Excluded:
- Assumptions:
- Risks:

## Approval Needed
- Confirm scope before architecture and build.
```
