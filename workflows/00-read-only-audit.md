# G0 — Read-only Audit

## Entry conditions
- User has authorized inspection of a specific workspace or provided the file tree/contents.
- Agent is operating under `AGENTS.md` and `harness/permissions.md`.

## Allowed actions
- List files and directories.
- Read source, config, package manifests, license files, existing docs.
- Record runtime/tool versions if observable.
- Produce an inventory report.

## Forbidden actions
- Any write, delete, rename, install, commit, push, deploy.
- Running commands that mutate the filesystem or install packages.

## Required output
- Task report in the standard format (Task ID, Goal, Allowed paths, …).
- Inventory of observed structure, key files, and versions.
- List of missing evidence or blocked checks.
- Explicit statement of what was **not** verified.

## Stop conditions
- Any request that would require mutation → stop and request explicit G3/G7 approval.
- Environment access unavailable → return a checklist for the user to run.
