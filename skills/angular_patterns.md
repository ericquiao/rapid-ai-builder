# Angular Patterns

## Purpose
Provide simple Angular conventions for the first build.

## Recommended Patterns
- Use standalone components unless the project already uses another pattern.
- Keep feature folders shallow.
- Create a small service layer for API calls.
- Use route-based pages and simple presentational components.
- Keep shared UI minimal.
- Prefer reactive forms for non-trivial input.
- Avoid state libraries unless local component state becomes unmanageable.

## Suggested Structure
```text
src/app/
  core/
  features/
  shared/
```
