# /status

## Command
`/status`

## Purpose
Provide a concise dashboard view of the current project state.

## Instructions For AI Execution
1. Read the following project documentation:
   - `docs/project_overview.md`
   - `docs/project_memory.json`
   - `docs/scope_lock.md`
   - `docs/architecture.md`
   - `docs/build_plan.md`
   - `docs/iterations/`
2. Identify:
   - latest iteration
   - current stage from `docs/project_memory.json` if available
   - active tasks from `docs/project_memory.json`
   - recent decisions from `docs/project_memory.json`
   - known risks from `docs/project_memory.json`
   - working features
   - known issues
   - next planned improvements
   - next action from `docs/project_memory.json`
3. Generate a clean summary including:
   - Project Name
   - Goal
   - Current Stage
   - Latest Iteration
   - Active Tasks
   - Key Decisions
   - Risks
   - Working Features
   - Known Issues
   - Next Action
   - Next Suggested Iteration
4. If `docs/project_memory.json` is missing, suggest creating it with only:
   - `current_stage`
   - `active_tasks`
   - `decisions`
   - `risks`
   - `next_action`
5. If the `docs/iterations/` folder is missing or empty, suggest creating the first iteration record.
