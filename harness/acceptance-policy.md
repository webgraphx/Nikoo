# Acceptance Policy

A gate passes only when all mandatory criteria have evidence. An agent's assertion alone is not evidence.

## Harness acceptance
- H-01 Required docs and role prompts exist.
- H-02 Permission boundaries are explicit and internally consistent.
- H-03 Every workflow has entry conditions, actions, outputs and stop conditions.
- H-04 Tasks define allowed paths and measurable acceptance criteria.
- H-05 Platform compatibility claims cite tested versions and observed evidence; otherwise label them “unverified”.
- H-06 No secret values appear in files, logs or archives.
- H-07 Blocked tasks preserve status and explain the missing prerequisite.
- H-08 Archive can be extracted and inspected without corrupt paths or accidental secret files.
- H-09 No target repository changes occur without G3 authorization.
- H-10 No publish/deploy occurs without G7 human approval.

## Nikoo UI acceptance (for future implementation)
- N-01 Main modules render with no console-breaking errors.
- N-02 All primary UI is Persian and RTL, including forms, tables, menus and dialogs.
- N-03 Layout checked at 360px, 768px and 1440px.
- N-04 Keyboard focus is visible and primary flows are keyboard-operable.
- N-05 Empty, loading, success and error states are present where relevant.
- N-06 Search, filters, demo create/edit/status actions behave as specified.
- N-07 Mock AI responses are labelled and do not imply live AI.
- N-08 localStorage behavior is documented; reset is explicit and safe.
- N-09 No production credentials, real customer records or secret values.
- N-10 License inventory covers runtime dependencies, icons and fonts.
- N-11 ZIP extracts cleanly and follows README on a fresh environment.
- N-12 All required test outcomes are reported; unrun tests are not marked as passed.
