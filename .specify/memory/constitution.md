# SDD Constitution

## Core Principles

### I. Spec-First Development
Every non-trivial feature must start from a written specification in `specs/<feature-id>/spec.md`.
Implementation starts only after the specification is reviewed and clarified.

### II. Plan Before Code
Each approved specification must produce a technical plan in `specs/<feature-id>/plan.md`.
The plan must define architecture, data flow, risks, and testing strategy before coding tasks begin.

### III. Testability Is Mandatory
Every feature plan must include verifiable acceptance criteria and test cases.
Code changes without a matching test strategy are considered incomplete.

### IV. Traceability From Spec to Task to Code
All implementation tasks in `specs/<feature-id>/tasks.md` must map back to requirements in `spec.md`.
Pull requests must reference related spec and task entries.

### V. Small, Reversible Changes
Work is delivered in small commits with clear intent and minimal blast radius.
Large rewrites require explicit rationale and rollback strategy in the plan.

## Technical Constraints

- Keep toolchain and dependencies minimal unless justified by the feature plan.
- Prefer clarity and maintainability over framework complexity.
- Security and data handling decisions must be documented in the plan for affected features.

## Workflow And Quality Gates

1. Run `$speckit-constitution` to maintain project principles.
2. Run `$speckit-specify` for feature requirements.
3. Run `$speckit-clarify` when requirements are ambiguous.
4. Run `$speckit-plan` for technical design.
5. Run `$speckit-tasks` to generate executable work items.
6. Run `$speckit-analyze` and `$speckit-checklist` before implementation.
7. Run `$speckit-implement` and validate against acceptance criteria.

## Governance

This constitution is the source of truth for project delivery standards.
Changes to this constitution require:
- A documented reason.
- A version update.
- A ratification date update.

**Version**: 1.0.0 | **Ratified**: 2026-04-09 | **Last Amended**: 2026-04-09
