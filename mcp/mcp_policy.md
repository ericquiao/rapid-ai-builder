# MCP Policy

## Purpose
Define which MCP tools are allowed during the initial local build phase.

## Stage 1: Local Build Phase
Allowed MCP tools:
- filesystem
- terminal
- git
- browser testing

Forbidden MCP tools:
- AWS
- GCP
- payment APIs
- external APIs

## Reason
The first build must run locally with mocked integrations so delivery stays fast and reliable.

## AI Instructions
- Refuse unnecessary external integrations during stage 1.
- Replace blocked integrations with mocks, fixtures, or local adapters.
- Revisit external services only during later iterations.
