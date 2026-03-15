# Framework Flow

## Purpose
Define the required end-to-end workflow for rapid local AI builds.

## Workflow
1. Idea
   Capture the app concept in one paragraph.
2. Discussion
   Review the problem, target users, and success outcome.
3. Clarifying Questions
   Ask only the minimum questions needed to remove ambiguity.
4. Requirements Summary
   Write a concise requirements draft using the template.
5. Scope Lock
   Freeze the first build to a small, local, testable feature set.
6. Architecture Draft
   Pick the stack, app shape, and mocked integration points.
7. Local Build Strategy
   Decide how the app will run on localhost with minimal setup.
8. One-Shot Build Plan
   List files, components, endpoints, schema, and run steps.
9. Generate Application
   Build the app in one focused implementation pass.
10. Run on Localhost
    Start frontend and backend locally and confirm the happy path.
11. Builder Review
    Gather feedback on gaps, UX issues, and missing flows.
12. Iteration Plan
    Turn feedback into the next small scoped build.

## Rules
- Prioritize a running localhost app over ideal architecture.
- Use one application per project.
- Mock external services first.
- Avoid infrastructure that slows down the first build.
- Stop expanding scope after scope lock unless the builder explicitly changes it.

## Expected AI Behavior
- Move one step at a time.
- Show the current step before asking for input.
- Keep outputs short and structured.
- Push toward implementation once scope is locked.
