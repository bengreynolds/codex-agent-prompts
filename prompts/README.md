# Prompt Library

This directory contains prompt templates grouped by type. Each prompt is written to be copied directly into an agent session.

## Workflows
- `workflows/agent-execution.md` - Execute a plan from `agent.md` and `planning.md` safely.
- `workflows/branch-setup.md` - Initialize a branch session and local planning files.
- `workflows/create-codebase-context.md` - Build high-fidelity context before edits.
- `workflows/create-codebase-context-lite.md` - Gather task-scoped context with minimal token use.
- `workflows/merge-branch-to-main.md` - Analyze branch vs main and design a merge plan.
- `workflows/bug-hunt.md` - Reproduce, isolate, and explain a bug before fixing.
- `workflows/release-readiness.md` - Evaluate release readiness and decide go or no-go.
- `workflows/agent-planning-review.md` - Review `agent.md`, `planning.md`, and recent commits.
- `workflows/mimic-code-architecture.md` - Match an existing codebase's architecture and style.

## Planning
- `planning/migration-plan.md` - Plan a safe, reversible migration.
- `planning/refactor-plan.md` - Plan a behavior-preserving refactor.
