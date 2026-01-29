# Repository Structure

## Goals
- Keep prompts discoverable as the library grows.
- Separate prompt content from documentation and meta files.
- Maintain consistent naming and predictable paths.

## Directory layout
```
.
|-- docs/
|   |-- INDEX.md
|   |-- STRUCTURE.md
|   `-- STYLE_GUIDE.md
|-- prompts/
|   |-- README.md
|   |-- batch/
|   |   `-- agent-initialization-bundle.md
|   |-- experimental/
|   |-- planning/
|   |   |-- migration-plan.md
|   |   |-- refactor-plan.md
|   |   `-- mvp-plan.md
|   `-- workflows/
|       |-- context/
|       |   |-- agent-planning-review.md
|       |   |-- create-codebase-context-lite.md
|       |   |-- create-codebase-context.md
|       |   |-- mimic-code-architecture.md
|       |   `-- reestablish-context.md
|       |-- execution/
|       |   `-- agent-execution.md
|       |-- merge/
|       |   `-- merge-branch-to-main.md
|       |-- quality/
|       |   |-- bug-hunt.md
|       |   |-- code-cleanup.md
|       |   |-- code-condensation.md
|       |   |-- codebase-efficacy-review.md
|       |   `-- release-readiness.md
|       `-- setup/
|           `-- branch-setup.md
|-- CONTRIBUTING.md
`-- README.md
```

## Conventions
- Prompt files use kebab-case names (example: `merge-branch-to-main.md`).
- Group prompts by type under `prompts/` as the collection expands.
- Keep docs in `docs/` and link them from `docs/INDEX.md`.
- Prefer ASCII-only text for maximum portability.
