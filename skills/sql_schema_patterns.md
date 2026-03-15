# SQL Schema Patterns

## Purpose
Provide simple relational design guidance for first-version schemas.

## Recommended Patterns
- Start with the fewest tables possible.
- Use integer primary keys unless there is a strong reason not to.
- Add timestamps only when useful.
- Normalize obvious repeated entities, but do not over-model.
- Design around the main user flow.
- Keep foreign keys explicit.
- Avoid premature optimization and advanced database features.

## Basic Checklist
- What core records exist?
- What relationships are required?
- What data is only mock or seed data for now?
