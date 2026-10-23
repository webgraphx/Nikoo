# Gated Workflow

## G0 — Read-only audit
Inspect only the authorized workspace. Record repository status, tree, runtime versions, scripts, tests, dependency manifests, license files and existing UI. Do not run commands that mutate files. Do not install packages. If environment access is unavailable, return a checklist for the user to run.

## G1 — Specification
Write testable requirements for each module, user flows, state handling, error/empty/loading states, responsive breakpoints and acceptance criteria. Obtain approval before design or implementation scope expands.

## G2 — Design System approval
Present a concise token proposal: typography, color roles, spacing, radius, shadows, layout, focus, component states and responsive behavior. Use a properly licensed Persian font or system fallback; verify font license before bundling. Wait for approval.

## G3 — Development authorization
Require explicit approval for implementation scope, allowed paths and dependency changes. Create small tasks with acceptance criteria and rollback notes.

## G4 — Module acceptance
Implement and test one module at a time. Integrate only after module acceptance. Avoid broad refactors unrelated to approved scope.

## G5 — Quality/security gate
Run only approved checks. Include RTL, keyboard, contrast, responsive, interaction, data handling, dependency and secret scans. A failed required test blocks the gate.

## G6 — Package
Build reproducibly, inspect ZIP contents for secrets and unnecessary files, extract into a clean directory and test the documented run procedure. Report any test that could not be run.

## G7 — Release
Provide source/build/archive hashes, test report, known limitations and change list. Ask for explicit human approval before pushing, publishing or deploying.
