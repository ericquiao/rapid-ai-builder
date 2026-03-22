# rapid-ai-builder

`rapid-ai-builder` is a lightweight reusable software and AI development framework for going from idea to a working localhost application quickly. It is designed for a builder and an AI coding assistant to move fast, lock scope early, and iterate from working software instead of abstract plans.

## Core Philosophy
- Working software over perfect architecture.
- Simple first build over complex infrastructure.
- Explicit validation before scale-up.
- Fast iteration over premature optimization.
- Reusable across software products, internal tools, automations, and AI systems.

## Engineering Framework
The framework uses a staged progression that keeps validation explicit while preserving momentum:

Mock / Concept -> Core POC -> Integration POCs -> System Integration -> MVP -> Beta -> Production

Important rule:
The framework should remain stable and only be modified when a real project reveals a structural limitation.

### Stage 1: Mock / Concept
**Purpose**

Define the problem, target users, core workflow, and the simplest believable version of the solution. This stage validates what should be built before validating how it should be built.

**Typical Activities**
- Clarify the product concept, users, constraints, and success signals.
- Sketch user journeys, sample inputs and outputs, or mocked system behavior.
- Create low-fidelity mock flows, static screens, stub APIs, or deterministic AI responses.
- Identify the smallest useful scope for the first build.

**Deliverables**
- Problem statement and target user summary.
- Core workflow definition.
- Mocked UX, sample outputs, or concept demo.
- Initial scope boundary and assumptions list.

**Exit Criteria**
- The team agrees on the problem, user, and primary use case.
- The target workflow is understandable without real integrations.
- The first validation questions are clear enough to test in a POC.

**Next Stage**

Core POC

### Stage 2: Core POC
**Purpose**

Validate the core technical feasibility of the product's hardest or riskiest capability in isolation. This stage proves that the essential engine can work before surrounding it with external dependencies.

**Typical Activities**
- Test the core algorithm, AI workflow, model behavior, or backend logic.
- Run focused technical experiments against the highest-risk assumption.
- Measure baseline feasibility, performance, quality, or reliability.
- Document technical constraints, failure modes, and design implications.

**Deliverables**
- Core feasibility prototype.
- Experiment notes and results.
- List of validated and invalidated assumptions.
- Recommendation for what needs external integration testing next.

**Exit Criteria**
- The central technical hypothesis is proven viable or clearly rejected.
- The main technical risks are understood well enough to proceed.
- The project has enough evidence to begin integration-specific experiments.

**Next Stage**

Integration POCs

### Stage 3: Integration POCs
**Purpose**

Validate external dependencies one by one before attempting full system assembly. This stage isolates integration risk so teams can confirm each required service, API, data source, model provider, or platform dependency independently.

**Typical Activities**
- Build targeted experiments for third-party APIs, auth flows, databases, queues, model providers, sensors, or enterprise systems.
- Verify data contracts, latency, error handling, throughput, and operational limits.
- Test connectivity, credentials, permissions, and environment assumptions.
- Compare alternative integrations when needed.

**Deliverables**
- Integration test prototypes or reference implementations.
- Integration risk log with known constraints and workarounds.
- Confirmed contracts for external systems.
- Shortlist of approved integration approaches.

**Exit Criteria**
- Each required integration has been validated enough to reduce unknowns.
- Blocking limitations, rate limits, security constraints, and contract mismatches are known.
- The team can integrate the validated components into one working system with manageable risk.

**Next Stage**

System Integration

### Stage 4: System Integration
**Purpose**

Combine the validated core capability and validated integrations into a coherent end-to-end system. This stage proves that the pieces work together as one product, not just as separate experiments.

**Typical Activities**
- Connect core logic with selected integrations in a unified architecture.
- Validate end-to-end workflows, orchestration, data flow, and error paths.
- Resolve interface mismatches, state handling issues, and system-level failures.
- Establish basic deployment, configuration, and observability patterns for a working integrated build.

**Deliverables**
- End-to-end integrated system prototype.
- System architecture and interface decisions.
- Known gaps and stabilization backlog.
- Evidence that the primary workflow works across real system boundaries.

**Exit Criteria**
- The primary end-to-end workflow operates across the full system.
- Major component interactions are stable enough for productization work.
- Remaining work is primarily about usability, completeness, and hardening rather than basic feasibility.

**Next Stage**

MVP

### Stage 5: MVP
**Purpose**

Turn the integrated system into a usable product with the minimum feature set required for real users or stakeholders. This stage focuses on usefulness, repeatability, and product readiness at small scale.

**Typical Activities**
- Build the minimum set of production-intent features around the validated system.
- Improve UX, workflows, state management, and operational consistency.
- Add essential persistence, security controls, configuration handling, and test coverage.
- Prepare onboarding, usage guidance, and basic support processes.

**Deliverables**
- Functional minimum viable product.
- Core user-facing workflows with real integrations.
- Basic documentation, test coverage, and deployment instructions.
- Prioritized backlog for beta feedback and stabilization.

**Exit Criteria**
- Real users can complete the primary workflow without manual intervention from builders.
- The product delivers repeatable value in a limited real-world setting.
- The team is ready to broaden usage and collect structured feedback.

**Next Stage**

Beta

### Stage 6: Beta
**Purpose**

Validate the MVP with broader real-world usage, uncover operational issues, and refine the product before general release. This stage focuses on confidence, learning, and controlled expansion.

**Typical Activities**
- Release to a limited but real user group.
- Gather feedback, usage patterns, defects, and support needs.
- Improve stability, onboarding, performance, and usability.
- Add monitoring, alerting, and release management discipline.

**Deliverables**
- Beta release used by real testers or customers.
- Feedback log and prioritized improvement plan.
- Reliability and usage insights.
- Release-readiness assessment.

**Exit Criteria**
- The product performs reliably for the intended beta audience.
- Key usability and operational issues are resolved or clearly understood.
- The system is ready for broader release with acceptable support burden.

**Next Stage**

Production

### Stage 7: Production
**Purpose**

Operate the product as a dependable real-world system with appropriate reliability, security, scalability, and governance for its context.

**Typical Activities**
- Harden infrastructure, security, monitoring, backup, and recovery processes.
- Improve scalability, maintainability, and incident response readiness.
- Formalize deployment, support, change management, and operational ownership.
- Continue iterative product improvement based on live usage.

**Deliverables**
- Production-ready system and operating model.
- Operational runbooks and support processes.
- Monitoring, alerting, and incident response standards.
- Roadmap for continued optimization and expansion.

**Exit Criteria**
- The product can be operated and supported reliably in its intended environment.
- Key business, technical, and operational controls are in place.
- The team can scale usage without re-entering feasibility validation work.

**Next Stage**

Ongoing iteration and optimization

## Project Stage Identification
Every project using this framework must declare its current stage explicitly so humans and AI agents can determine appropriate next actions.

Required declaration:

`Current Stage: <stage name>`

Allowed stage names:
- Mock / Concept
- Core POC
- Integration POCs
- System Integration
- MVP
- Beta
- Production

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
├── docs/
│   ├── mock_design.md
│   ├── poc_analysis.md
│   └── project_overview.md
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
- Record the current project `Current Stage` in `docs/project_overview.md`.
- Confirm the default stack or choose an override during discussion.
- Use the templates in `templates/` to keep outputs structured.
- Use the prompts in `prompts/` to guide the AI step by step.
- Do not build until scope lock is approved.

## How To Iterate
- Review the running localhost app first.
- Capture issues, missing behavior, and UX friction.
- Prioritize the next smallest useful change.
- Move through stages intentionally: Mock / Concept clarifies the solution, Core POC validates the hardest technical assumption, Integration POCs validate dependencies, System Integration proves end-to-end behavior, MVP makes it usable, Beta broadens validation, and Production hardens operations.
- Keep integration scope narrow until the project is ready for system-level assembly.

## Iteration Management
The framework records development progress in `docs/iterations/`. Each iteration should leave a clear written history so the AI and builder can quickly recover project context.

New commands:
- `/status`: generate a concise dashboard of the current project state.
- `/resume`: reconstruct the project state after a long break.

Every iteration should:
1. update `docs/iterations/`
2. update `docs/project_overview.md`
3. create a git commit snapshot
