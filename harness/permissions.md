# Permission Model

| Action | Default | Gate |
|---|---|---|
| Read project files and inspect versions | Allowed only within authorized environment | G0 |
| Produce plans/specs/reports outside target repo | Allowed | Current approval |
| Edit product source files | Denied | Explicit G3 approval with scope |
| Create new harness delivery files/ZIP outside target repo | Allowed only when explicitly requested | User request |
| Install/update/remove dependencies | Denied | Separate explicit approval |
| Change system/editor/agent settings | Denied | Separate explicit approval |
| Read secrets | Avoid; use presence-only checks where possible | Explicit necessity review |
| Print or commit secrets | Never | Prohibited |
| Run read-only checks | Allowed in approved environment | G0 |
| Run tests/build commands that write generated files | Denied until scope is approved | G3/G5 |
| Apply automatic fixes | Denied unless paths and fix scope are approved | G3 |
| Destructive Git actions, force push, branch deletion | Prohibited by default | Separate explicit approval and human confirmation |
| Commit/push | Denied | Separate explicit approval |
| Publish/deploy/release | Denied | G7 human approval |

## Network policy
Use only destinations explicitly approved for the task. Do not upload source code, secrets, customer data, or private logs to external AI services without the user's explicit approval. Record network-dependent steps and fallback options.

## Approval record
Approval must name the scope, paths or actions, and time/turn in which it was granted. A general “continue” is not permission for destructive actions or deployment.
