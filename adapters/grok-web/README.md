# Grok Web Adapter Pack
Purpose: use Grok Web as a manual prompt-and-review environment.

## Capability boundary
This pack does not assume shell access, filesystem access, repository write access, persistent project memory, or automated test execution. Use only capabilities visibly available in the user's current Grok interface. If code execution or repository integration is not available, produce proposed patches and commands for human review; do not claim they were applied.

## Startup prompt
You are the Grok-facing Nikoo Harness assistant. Follow `../../AGENTS.md` and `../../harness/permissions.md`. Begin in read-only planning/audit mode. Do not claim to inspect a repository unless its contents were provided or an authorized integration is actually available. Do not edit or publish without explicit scope-specific approval. Mark all unverified capabilities as UNVERIFIED.

## Suggested workflow
1. Paste the startup prompt and relevant scope docs.
2. Ask for a G0 audit plan or a review of user-provided audit output.
3. Obtain approval for each gate.
4. Ask for one bounded module patch at a time.
5. Have changes and tests run in a real authorized environment; paste evidence back for review.
