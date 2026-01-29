# Documentation Index

## Overview
- `README.md` - Repository overview and quick start.
- `docs/STRUCTURE.md` - Directory layout, naming conventions, and how prompts are organized for long-term growth.
- `docs/STYLE_GUIDE.md` - Markdown formatting rules and prompt-writing standards to keep prompts readable and consistent.
- `CONTRIBUTING.md` - Step-by-step guidance for adding, updating, and maintaining prompts in this library.

## Prompt catalog
### Workflows
#### Context
- `prompts/workflows/context/agent-planning-review.md` - Summarize `agent.md`, `planning.md`, and the latest commits to establish current project state.
- `prompts/workflows/context/create-codebase-context.md` - Build comprehensive, high-fidelity codebase context before any edits or decisions.
- `prompts/workflows/context/create-codebase-context-lite.md` - Gather only task-scoped context with minimal token usage while preserving accuracy and safety.
- `prompts/workflows/context/mimic-code-architecture.md` - Align new work with existing architecture, naming, structure, and formatting conventions.
- `prompts/workflows/context/reestablish-context.md` - Rebuild session context after chat condensation using Git history and plan artifacts.

#### Setup
- `prompts/workflows/setup/branch-setup.md` - Initialize a branch session, set up `.gitignore`, and create local `agent.md` and `planning.md` working files.

#### Execution
- `prompts/workflows/execution/agent-execution.md` - Execute a plan from `agent.md` and `planning.md` safely.
- `prompts/workflows/execution/confirm-implementation.md` - Verify implementation matches the plan and task goals.

#### Quality
- `prompts/workflows/quality/bug-hunt.md` - Systematically reproduce, minimize, and explain a bug before proposing fixes.
- `prompts/workflows/quality/release-readiness.md` - Assess release quality gates, operational readiness, and make a clear go or no-go decision.
- `prompts/workflows/quality/code-cleanup.md` - Identify and remove patch debt, duplicate logic, and unnecessary code without changing behavior.
- `prompts/workflows/quality/code-condensation.md` - Reduce code size and complexity while preserving current behavior and interfaces.
- `prompts/workflows/quality/codebase-efficacy-review.md` - Evaluate codebase effectiveness and surface prioritized improvement opportunities.

### Batch
- `prompts/batch/agent-initialization-bundle.md` - Condensed onboarding workflow for context, style, and execution.

### Experimental
- Add experimental prompts here.

### Git
#### Branches
- `prompts/git/branches/add-remote-branch.md` - Push a local branch to a remote and set upstream.
- `prompts/git/branches/link-remote-branch.md` - Link a local branch to an existing remote branch.
- `prompts/git/branches/remove-remote-branch.md` - Delete a remote branch safely with confirmation.

#### History
- `prompts/git/history/rebase-branch.md` - Rebase a current branch onto a target branch with verification.

#### Sync
- `prompts/git/sync/pull-with-logging.md` - Pull changes while capturing issues, warnings, and errors.

#### Tags
- `prompts/git/tags/create-tag.md` - Create a Git tag with explicit target and metadata.

#### Merge
- `prompts/git/merge/merge-branch-to-main.md` - Analyze differences between a branch and `main`, document risks, and plan a low-risk merge.

### Planning
- `prompts/planning/migration-plan.md` - Plan a safe, reversible migration.
- `prompts/planning/refactor-plan.md` - Plan a behavior-preserving refactor with explicit invariants, checkpoints, and rollback.
- `prompts/planning/mvp-plan.md` - Define the smallest viable scope, acceptance criteria, and validation plan for a specific task.
