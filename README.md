# rapid-ai-builder

`rapid-ai-builder` is a lightweight AI development framework for going from idea to a working localhost application in 1-2 hours. It is designed for a builder and an AI coding assistant to move quickly, lock scope early, and iterate from working software instead of abstract plans.

## Core Philosophy
- Working localhost application over perfect architecture.
- Simple first build over complex infrastructure.
- Mock external services first.
- Fast iteration over premature optimization.
- One application per project.

## Default Stack
The default recommendation is:
- Frontend: Angular
- Backend: FastAPI
- Database: SQLite
- Styling: Tailwind CSS

During discussion, the AI should ask whether to use this default stack or another stack.

## Workflow
The framework follows this sequence:
1. Idea
2. Discussion
3. Clarifying Questions
4. Requirements Summary
5. Scope Lock
6. Architecture Draft
7. Local Build Strategy
8. One-Shot Build Plan
9. Generate Application
10. Run on Localhost
11. Builder Review
12. Iteration Plan

Detailed workflow guidance lives in `workflow/`.

## Quick Start
1. Run `/idea`
2. Run `/discuss`
3. Lock scope with `/scope-lock`
4. Generate a build plan with `/build-plan`
5. Build the application with `/build-app`
6. Run the app on localhost
7. Iterate with `/iterate`

## Commands
- `/idea`: capture the initial app concept.
- `/discuss`: refine the app, users, flow, and stack.
- `/scope-lock`: freeze the first build scope.
- `/architecture`: define the simplest technical approach.
- `/build-plan`: create a one-shot implementation plan.
- `/build-app`: generate and verify the app.
- `/iterate`: plan the next improvements.

See `commands/` for command-specific guidance.

## Project Structure
```text
rapid-ai-builder/
├── workflow/
│   ├── framework_flow.md
│   └── builder_guide.md
├── prompts/
│   ├── idea_prompt.md
│   ├── discussion_prompt.md
│   ├── scope_lock_prompt.md
│   ├── architecture_prompt.md
│   ├── build_plan_prompt.md
│   ├── one_shot_build_prompt.md
│   └── iteration_prompt.md
├── templates/
│   ├── requirements_template.md
│   ├── scope_lock_template.md
│   ├── architecture_template.md
│   └── build_plan_template.md
├── commands/
│   ├── idea.md
│   ├── discuss.md
│   ├── scope_lock.md
│   ├── architecture.md
│   ├── build_plan.md
│   ├── build_app.md
│   └── iterate.md
├── skills/
│   ├── rapid_build_rules.md
│   ├── angular_patterns.md
│   ├── fastapi_patterns.md
│   ├── sql_schema_patterns.md
│   └── ui_design_patterns.md
├── mcp/
│   ├── mcp_policy.md
│   ├── local_tools.md
│   └── future_integrations.md
└── README.md
```

## How To Start A New Project
- Begin with the problem, users, and one core flow.
- Confirm the default stack or choose an override during discussion.
- Use the templates in `templates/` to keep outputs structured.
- Use the prompts in `prompts/` to guide the AI step by step.
- Do not build until scope lock is approved.

## How To Iterate
- Review the running localhost app first.
- Capture issues, missing behavior, and UX friction.
- Prioritize the next smallest useful change.
- Keep integrations mocked until core flows are stable.

## Iteration Management
The framework records development progress in `docs/iterations/`. Each iteration should leave a clear written history so the AI and builder can quickly recover project context.

New commands:
- `/status`: generate a concise dashboard of the current project state.
- `/resume`: reconstruct the project state after a long break.

Every iteration should:
1. update `docs/iterations/`
2. update `docs/project_overview.md`
3. create a git commit snapshot
