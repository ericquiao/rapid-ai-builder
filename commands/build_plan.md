# /build-plan

## Purpose
Convert the approved architecture into clear, minimal implementation steps while staying stage-aware and execution-safe.

## When To Use
Use once architecture is approved.

## Core Objective
- File list.
- API endpoints.
- UI components.
- Database tables.
- Run and verification steps.
- Keep the plan specific enough for one-shot implementation.
- Focus on the happy path first.
- Call out mocks and shortcuts clearly.
- Suggested skills when clearly helpful.
- Parallel task notes only when tasks are clearly independent.

## Execution Approach
- Always plan sequentially first.
- Only introduce parallel tasks when there is clear independence and speed benefit.
- Keep the plan simple and specific enough for one-shot implementation.

## Parallel Guidance
- Only recommend parallel work when tasks are clearly independent and can be split safely with little coordination.
- Only mark tasks as parallel if they do not modify the same files, data, or components.
- If unsure, default to sequential execution.
- Keep parallel execution optional, not required.

## Skills Usage
- Suggest relevant skills from `skills/` as optional references, not automatic steps.
- Only suggest a skill if it clearly reduces effort or improves reliability, and do not suggest multiple skills unnecessarily.
- Do not use skills for simple or obvious tasks.
- Only use a skill when the task is repeated, has known complexity, or benefits from a structured pattern.

## Workflow Consistency
- A workflow is the logical sequence of steps needed to achieve a goal.
- Keep workflows simple, stage-aware, and aligned with the current command.
- Each command should produce outputs that naturally feed the next command.
- Avoid jumping steps or skipping stages, and maintain continuity between planning, building, and iteration.

## Tool Usage
- Tools are used to execute specific tasks such as coding, API calls, or testing.
- Workflow logic decides what needs to be done; tools and skills define how it is done.
- Only introduce tools when needed, prefer direct implementation for simple tasks, and avoid unnecessary abstraction or tool layering.
- Do not mix decision-making with execution details unnecessarily.

## Generality Rule
- Keep build plans reusable across different application types.
- Avoid introducing patterns or structure that only apply to a specific app unless explicitly required.
