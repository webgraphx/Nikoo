# WGX Nikoo Dashboard UI — Agent Harness

**Version:** 0.1.0  
**Repository:** [webgraphx/Nikoo](https://github.com/webgraphx/Nikoo)  
**Status:** Portable, approval-gated harness specification — ready for use across AI environments.

## Purpose
A portable, approval-gated harness for planning, building, testing, and packaging the **Nikoo Dashboard UI MVP** (Persian-first, RTL, HTML5 + Tailwind CSS + Vanilla JS).

## Important limitations
- This repository is the **harness specification**, not the product source code.
- No backend, production authentication, payment, real AI API, or production database in the baseline MVP.
- All demo data and AI responses must be clearly labelled as sample/mock (`نمونه آزمایشی`).
- Platform compatibility claims remain **UNVERIFIED** until tested in the target environment.
- Human approval is required before any publish, deploy, or destructive Git action.

## Contents
| Path | Description |
|------|-------------|
| `AGENTS.md` | Global non-negotiable rules (read first) |
| `harness/` | Architecture, permissions, workflow gates, acceptance policy |
| `agents/` | Role prompts (Controller, Auditor, Spec Analyst, …) |
| `workflows/` | Gated workflow steps (G0 → G7) |
| `skills/` | Portable task playbooks |
| `adapters/` | Platform-specific packs (Grok Web, …) |
| `tests/` | Acceptance checklist |
| `templates/` | Audit, change-request, QA and release report templates |
| `docs/` | MVP scope, design-system notes, compatibility matrix |

## Recommended use
1. Read `AGENTS.md` and `harness/permissions.md`.
2. Start at **G0** using `workflows/00-read-only-audit.md`.
3. Do **not** edit product files or install dependencies until explicit approval for the relevant scope is given.
4. Keep generated output and test evidence in a reviewable branch or isolated working copy.
5. Require human approval before publication, deployment, or any action outside the approved scope.

## MVP scope summary
Fully Persian RTL dashboard, mobile-first.  
Modules (demo only): Dashboard, Projects/Tasks, AI Mock Chat, Users, CRM, Store, Finance, Settings.  
Local preferences may use browser `localStorage` after implementation approval.  
This is a front-end demo, **not** production CRM / e-commerce / accounting software.

## License
Documentation and prompts in this repository are provided for use with the Nikoo project.  
No secrets, tokens, or personal data are included.
