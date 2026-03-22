# Name
`api_integration_validation`

## Purpose
Check whether an external API integration is simple enough, feasible enough, and well understood before it is included in the build plan.

## Inputs
- API name or provider
- Intended use case
- Required endpoints or actions
- Known auth and data requirements

## Outputs
- Integration feasibility summary
- Key assumptions to validate
- Known risks or blockers
- Recommendation to mock, defer, or proceed

## When To Use
- During Core POC or Integration POCs
- When a build depends on an external API
- Before committing an integration to the main implementation plan
