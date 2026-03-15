# FastAPI Patterns

## Purpose
Provide straightforward backend conventions for local-first applications.

## Recommended Patterns
- Use a single FastAPI app.
- Group endpoints by feature.
- Keep business logic in small service modules when needed.
- Use Pydantic models for request and response schemas.
- Use SQLite for the first build.
- Seed sample data when it helps demo the happy path.
- Mock external APIs behind simple adapter functions.

## Suggested Structure
```text
backend/
  app/
    main.py
    api/
    models/
    schemas/
    services/
```
