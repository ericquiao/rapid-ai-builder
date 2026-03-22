# /resume

## Command
`/resume`

## Purpose
Reconstruct the project state when returning after a long break.

## Instructions For AI Execution
1. Read these documents:
   - `docs/project_overview.md`
   - `docs/project_memory.json`
   - `docs/scope_lock.md`
   - `docs/architecture.md`
   - `docs/build_plan.md`
   - `docs/iterations/`
2. Determine:
   - the current stage from `docs/project_memory.json` if available
   - active tasks from `docs/project_memory.json`
   - the latest completed iteration
   - features currently implemented
   - recent decisions from `docs/project_memory.json`
   - known risks from `docs/project_memory.json`
   - recommended next development step from `docs/project_memory.json` when present
3. Produce a short summary titled:

```md
## Project Resume Summary
```

Including:
- Current Project Status
- Current Stage
- Active Tasks
- Latest Iteration
- Completed Features
- Key Decisions
- Risks
- Known Issues
- Next Development Step
4. If `docs/project_memory.json` is missing, suggest creating it with only:
   - `current_stage`
   - `active_tasks`
   - `decisions`
   - `risks`
   - `next_action`
