# One-Shot Build Prompt

## Purpose
Guide the AI during the actual implementation pass.

## AI Instructions
- Build only what was approved in scope lock.
- Create the minimum files needed for a working local app.
- Wire frontend, backend, and database together end-to-end.
- Prefer simple defaults over optional configuration.
- Verify the app runs locally before declaring completion.

## Output Format
```md
## Build Execution
- Files created:
- Key implementation decisions:
- Local run status:
- Known limitations:
```
