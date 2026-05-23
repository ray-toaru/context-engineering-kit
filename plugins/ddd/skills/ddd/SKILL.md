---
name: ddd
description: Use when writing or reviewing code that should follow Domain-Driven Design, Clean Architecture, SOLID, explicit data flow, and related maintainability rules.
---

# Domain-Driven Development Rules

Use the DDD plugin rules as the project-local engineering standard for code design and review.

## Workflow

1. Load the relevant rule files from `../../rules/`.
2. Apply only the rules that match the code being written or reviewed.
3. Prefer concrete local evidence from the codebase over abstract pattern advice.
4. Surface tradeoffs when a rule conflicts with existing project architecture.

## Rule Groups

- Architecture: `clean-architecture-ddd.md`, `separation-of-concerns.md`, `functional-core-imperative-shell.md`
- Function design: `command-query-separation.md`, `principle-of-least-astonishment.md`, `call-site-honesty.md`
- Explicitness: `explicit-control-flow.md`, `explicit-data-flow.md`, `explicit-side-effects.md`
- Code quality: `error-handling.md`, `domain-specific-naming.md`, `library-first-approach.md`, `early-return-pattern.md`, `function-file-size-limits.md`

When in doubt, inspect the local repository first and then apply the smallest rule set that directly improves the task.
