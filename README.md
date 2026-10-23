# WGX Nikoo Dashboard UI

**Version:** 0.1.0  
**Official Repository:** [webgraphx/Nikoo](https://github.com/webgraphx/Nikoo)  
**Status:** Official project repository — contains the Agent Harness (active) and is the designated home for the Nikoo Dashboard UI MVP source (not yet implemented).

## Purpose
This is the **official repository** for the Nikoo Dashboard UI MVP (Persian-first, RTL, HTML5 + Tailwind CSS + Vanilla JS) and its approval-gated Agent Harness.

## Current state
- **Harness**: Fully installed and active (G0 completed).
- **Product source code**: Not yet present. Implementation begins only after G1–G3 approvals.
- No backend, production authentication, payment, real AI API, or production database in the baseline MVP.
- All demo data and AI responses must be labelled as sample/mock (`نمونه آزمایشی`).

## Contents (current)
| Path | Description |
|------|-------------|
| `AGENTS.md` | Global non-negotiable rules (read first) |
| `harness/` | Architecture, permissions, workflow gates, acceptance policy |
| `agents/` | Role prompts (Controller, Auditor, …) |
| `workflows/` | Gated workflow steps (G0 → G7) |
| `skills/` | Portable task playbooks |
| `adapters/` | Platform-specific packs (Grok Web, …) |
| `tests/` | Acceptance checklist |
| `templates/` | Task / audit / QA report templates |
| `docs/` | MVP scope, compatibility matrix |

Future product areas (to be created only after explicit G3 approval):
- `src/` — UI source, modules, styles
- `public/` — static assets
- `dist/` — build output (generated)

## Recommended use
1. Read `AGENTS.md` and `harness/permissions.md`.
2. Start at **G0** using `workflows/00-read-only-audit.md`.
3. Do **not** edit product files or install dependencies until explicit approval for the relevant scope is given.
4. Keep generated output and test evidence reviewable.
5. Human approval is required before publication, deployment, or any action outside approved scope.

## MVP scope summary
Fully Persian RTL dashboard, mobile-first.  
Modules (demo only): Dashboard, Projects/Tasks, AI Mock Chat, Users, CRM, Store, Finance, Settings.  
Local preferences may use browser `localStorage` after implementation approval.  
This is a front-end demo, **not** production CRM / e-commerce / accounting software.

## License
Documentation and prompts in this repository are provided for the Nikoo project.  
No secrets, tokens, or personal data are included.
