# /architecture

## Purpose
Create a lightweight technical plan for the locked scope.

## When To Use
Use after scope lock and before the build plan.

## AI Should Produce
- Frontend, backend, database, and mock integration design.
- Local development approach.

## How The AI Should Guide The Builder
- Recommend the default stack unless the builder overrides it.
- Prefer a single application with simple boundaries.
- Keep infrastructure and deployment concerns out of the first build.

## Tool Usage Rule
- Tools are used to execute specific tasks such as coding, API calls, or testing.
- Workflow logic decides what needs to be done.
- Tools and skills define how it is done.
- Do not mix decision-making with execution details unnecessarily.

## Simplicity Rule
- Only introduce tools when needed.
- Prefer direct implementation for simple tasks.
- Avoid unnecessary abstraction or tool layering.
