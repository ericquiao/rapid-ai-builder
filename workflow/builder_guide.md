# Builder Guide

## Purpose
Help the builder use `rapid-ai-builder` with an AI coding assistant from idea to local app.

## How To Work With The AI
- Start with `/idea` to describe the app.
- Use `/discuss` to refine the problem, users, and preferred stack.
- Confirm whether to use the default stack:
  Angular, FastAPI, SQLite, Tailwind CSS.
- Answer clarifying questions briefly.
- Approve the requirements summary and scope lock before building.
- Review the architecture and build plan.
- Run `/build-app` only after scope is locked.
- Use `/iterate` after testing the local app.

## Builder Rules
- Keep the first version narrow.
- Choose one core user journey.
- Defer integrations, auth complexity, billing, and cloud setup unless essential.
- Prefer mock data over blocked progress.
- Ask for changes in small batches after the first build works.

## Recommended Builder Inputs
- Problem: what needs to be solved.
- Users: who will use the app.
- Main flow: what a user should do end-to-end.
- Constraints: time, stack, design, or offline requirements.
- Success: what must work on localhost today.
