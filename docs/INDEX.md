# Documentation Index

## Overview
- `README.md` - Repository overview and quick start.
- `docs/STRUCTURE.md` - Directory layout, naming conventions, and how prompts are organized for long-term growth.
- `docs/STYLE_GUIDE.md` - Markdown formatting rules and prompt-writing standards to keep prompts readable and consistent.
- `CONTRIBUTING.md` - Step-by-step guidance for adding, updating, and maintaining prompts in this library.

## Prompt catalog
### Workflows
- `prompts/workflows/agent-execution.md` - Execute a plan from `agent.md` and `planning.md` safely.
- `prompts/workflows/branch-setup.md` - Initialize a branch session, set up `.gitignore`, and create local `agent.md` and `planning.md` working files.
- `prompts/workflows/create-codebase-context.md` - Build comprehensive, high-fidelity codebase context before any edits or decisions.
- `prompts/workflows/create-codebase-context-lite.md` - Gather only task-scoped context with minimal token usage while preserving accuracy and safety.
- `prompts/workflows/merge-branch-to-main.md` - Analyze differences between a branch and `main`, document risks, and plan a low-risk merge.
- `prompts/workflows/bug-hunt.md` - Systematically reproduce, minimize, and explain a bug before proposing fixes.
- `prompts/workflows/release-readiness.md` - Assess release quality gates, operational readiness, and make a clear go or no-go decision.
- `prompts/workflows/agent-planning-review.md` - Summarize `agent.md`, `planning.md`, and the latest commits to establish current project state.
- `prompts/workflows/mimic-code-architecture.md` - Align new work with existing architecture, naming, structure, and formatting conventions.
- `prompts/workflows/code-cleanup.md` - Identify and remove patch debt, duplicate logic, and unnecessary code without changing behavior.
- `prompts/workflows/code-condensation.md` - Reduce code size and complexity while preserving current behavior and interfaces.
- `prompts/workflows/codebase-efficacy-review.md` - Evaluate codebase effectiveness and surface prioritized improvement opportunities.

### Batch
- `prompts/batch/agent-initialization-bundle.md` - Condensed onboarding workflow for context, style, and execution.

### Experimental
- Add experimental prompts here.

### Planning
- `prompts/planning/migration-plan.md` - Plan a safe, reversible migration.
- `prompts/planning/refactor-plan.md` - Plan a behavior-preserving refactor with explicit invariants, checkpoints, and rollback.
- `prompts/planning/mvp-plan.md` - Define the smallest viable scope, acceptance criteria, and validation plan for a specific task.
