# Prompt Library

This directory contains prompt templates grouped by type. Each prompt is written to be copied directly into an agent session.

## Workflows
### Context
- `workflows/context/agent-planning-review.md` - Review `agent.md`, `planning.md`, and recent commits.
- `workflows/context/create-codebase-context.md` - Build high-fidelity context before edits.
- `workflows/context/create-codebase-context-lite.md` - Gather task-scoped context with minimal token use.
- `workflows/context/mimic-code-architecture.md` - Match an existing codebase's architecture and style.
- `workflows/context/reestablish-context.md` - Rebuild session context after chat condensation using Git and artifacts.

### Setup
- `workflows/setup/branch-setup.md` - Initialize a branch session and local planning files.

### Execution
- `workflows/execution/agent-execution.md` - Execute a plan from `agent.md` and `planning.md` safely.

### Merge
- `workflows/merge/merge-branch-to-main.md` - Analyze branch vs main and design a merge plan.

### Quality
- `workflows/quality/bug-hunt.md` - Reproduce, isolate, and explain a bug before fixing.
- `workflows/quality/release-readiness.md` - Evaluate release readiness and decide go or no-go.
- `workflows/quality/code-cleanup.md` - Remove redundant or unnecessary code safely.
- `workflows/quality/code-condensation.md` - Condense code while preserving behavior.
- `workflows/quality/codebase-efficacy-review.md` - Evaluate codebase efficacy and improvements.

## Batch
- `batch/agent-initialization-bundle.md` - Condensed onboarding workflow for context, style, and execution.

## Experimental
- Add experimental prompts here.

## Planning
- `planning/migration-plan.md` - Plan a safe, reversible migration.
- `planning/refactor-plan.md` - Plan a behavior-preserving refactor.
- `planning/mvp-plan.md` - Define a minimum viable product for a specific task.
