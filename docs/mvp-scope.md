# Nikoo Dashboard UI — MVP Scope

## Shared UI requirements
Persian-first and RTL from the beginning; responsive/mobile-first; consistent Design System; semantic HTML; keyboard support and visible focus; empty/loading/success/error states where relevant; demo data only.

## Modules
1. Dashboard: KPI cards, charts/visual summaries, recent activity.
2. Projects and tasks: list, search/filter, status, demo create/edit.
3. AI assistant: chat, submit message, mock response, loading/error; provider adapter interface only.
4. Users/data: sample users, search/filter, detail/status/form interactions; no real authentication.
5. CRM demo: contacts, companies, opportunities, pipeline stages, tasks/reminders and summary reports.
6. Store demo: products, categories, orders, inventory, discounts, shipping/returns and sales summary.
7. Finance demo: revenue/expenses, transactions, budgets, invoices, receivables/liabilities and summary reports.
8. Settings: theme and UI preferences, local demo-data controls and explicit reset.

## Non-goals
Backend, server database, production auth, real payments, live AI provider calls, real accounting, real inventory/orders, customer data, or production-grade CRM. “Complete demo” means coherent front-end demonstrations, not production readiness.

## Persistence
Browser localStorage may hold demo data/preferences after implementation is authorized. It is not secure storage and must not hold secrets, credentials or sensitive personal data. Provide a clear reset path and explain persistence is local to that browser.

## Proposed acceptance
- Main interactions work on all modules.
- Responsive widths tested at 360, 768 and 1440 px.
- RTL and mixed-direction content reviewed.
- Mock AI is visibly labelled.
- Build and archive instructions are reproducible.
- All required tests report PASS/FAIL/BLOCKED/NOT RUN.
