# /iterate

## Purpose
Plan and implement the next round of improvements after review.

## When To Use
Use after the builder has seen the local app.

## AI Should Produce
- Feedback summary.
- Prioritized next changes.
- A tight next-step iteration plan.
- Updates for `docs/project_memory.json` covering:
  - `decisions`
  - `risks`
  - `next_action`

## How The AI Should Guide The Builder
- Separate bugs from new features.
- Recommend the smallest valuable next step.
- Keep future integrations deferred until core flows are stable.
- Refresh `docs/project_memory.json` after each iteration review.
- Keep memory updates minimal and limited to:
  - decisions made in the iteration
  - risks now known
  - the single next recommended action

## Workflow Thinking Rule
- A workflow is the logical sequence of steps needed to achieve a goal.
- Keep workflows simple.
- Keep workflows stage-aware.
- Keep workflows aligned with the current command.
- Do not create separate workflow files or systems.

## Workflow Consistency Rule
- Each command should produce outputs that naturally feed the next command.
- Avoid jumping steps or skipping stages.
- Maintain continuity between planning, building, and iteration.

## Parallel Re-evaluation Rule
- During iteration, reassess current and upcoming tasks.
- Identify whether any tasks have become independent and can now be executed in parallel.
- Only recommend parallel execution if tasks do not share dependencies.
- Only recommend parallel execution if tasks do not modify the same components.
- If conditions are unclear, remain sequential.

## Generality Check
- Ensure recommendations remain applicable across different project types.
- Avoid drifting into app-specific assumptions unless required by scope.
