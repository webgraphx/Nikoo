# Architecture and Execution Specification

## Repository
This harness repository: `webgraphx/Nikoo`  
Product target (when authorized): separate product repository (not modified by this package).

## Harness model
User → Controller → Project State & Policies → Permission Gate → Spec Analyst → Design System → Module Agents → AI Mock Adapter → QA/Security → Build & Package → Clean extraction test → Human release approval.

The controller coordinates work and preserves state. Specialist roles may be separate agents only if the selected platform supports them; otherwise use sequential role prompts in one conversation.

## Roles
- Controller: scope, state, gates, evidence, delegation.
- Auditor: read-only inventory and compatibility checks.
- Spec Analyst: convert approved scope into testable requirements.
- UI Designer: design tokens, layout rules, responsive/RTL specifications.
- Frontend Developer: implement approved files only.
- Module Developer: implement one bounded module per task.
- AI Interface Developer: mock adapter and future provider interface, no live provider in MVP.
- QA Agent: execute approved automated tests and record output.
- Security Reviewer: review secrets, dependencies, unsafe DOM handling and storage.
- Release Agent: build archive, inspect contents and validate clean extraction; no publishing.

## Project-state lifecycle
`DRAFT → AUDIT_READY → AUDIT_REPORTED → SPEC_REVIEW → SPEC_APPROVED → DESIGN_REVIEW → DESIGN_APPROVED → DEV_AUTHORIZED → IMPLEMENTING → QA → PACKAGE_REVIEW → RELEASE_APPROVED`

A state transition requires its gate's evidence and approval. No agent may self-approve a human gate. Failure transitions to `BLOCKED` with a reason and recovery action.

## Baseline technical target
- HTML5
- Tailwind CSS using a build process; exact version to be chosen after read-only audit and dependency proposal
- Vanilla JavaScript, modularized by feature
- npm scripts for build/test/lint only after dependency approval
- RTL and Persian text from the start
- Demo data and optional localStorage
- Mock AI adapter with explicit “نمونه آزمایشی” indication
- No backend or real API keys in source

## Proposed project areas
Confirm actual repository structure during G0 before mapping these to paths:
- `src/` source UI, styles, modules and data adapters
- `public/` static assets
- `tests/` automated acceptance checks
- `dist/` build output, generated only when authorized
- `docs/` product requirements, design system and test reports

## Output deliverables
1. Source files.
2. Built static output.
3. Reproducible setup/build instructions.
4. ZIP package and clean-extraction test report.
5. README, architecture and module scope.
6. Test report with commands, environment, results, failures and limitations.
7. Dependency/license inventory.
8. Separate adapter packs for Grok Web, ChatGPT Projects, Codex and Hermes Agent.
