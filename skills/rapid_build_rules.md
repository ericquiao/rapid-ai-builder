# Rapid Build Rules

## Purpose
Provide the default operating rules for fast localhost-first builds.

## Guidelines
- Prefer a working localhost application over ideal architecture.
- Build one application only.
- Avoid microservices.
- Avoid unnecessary dependencies.
- Mock external services first.
- Keep setup steps short and repeatable.
- Favor simple CRUD and one main user flow in version one.
- Defer auth, billing, queues, jobs, and cloud infrastructure unless required.
- Use clear file naming and predictable structure.
