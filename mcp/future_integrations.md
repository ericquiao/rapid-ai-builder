# Future Integrations

## Purpose
Document how external services should be introduced after the local version works.

## Later-Phase Guidance
- Add cloud services only after the local flow is stable.
- Replace mocks one integration at a time.
- Keep an adapter boundary between app logic and external services.
- Re-test the local app after each real integration is introduced.

## Typical Upgrade Path
1. Keep the existing local app working.
2. Swap one mock for one real integration.
3. Add minimal configuration and secrets handling.
4. Validate failure handling before expanding further.
