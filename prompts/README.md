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
- `workflows/execution/confirm-implementation.md` - Verify implementation matches the plan and task goals.

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

## Git
### Branches
- `git/branches/add-remote-branch.md` - Push a local branch to a remote and set upstream.
- `git/branches/link-remote-branch.md` - Link a local branch to an existing remote branch.
- `git/branches/remove-remote-branch.md` - Delete a remote branch safely with confirmation.

### History
- `git/history/rebase-branch.md` - Rebase a current branch onto a target branch with verification.

### Sync
- `git/sync/pull-with-logging.md` - Pull changes while capturing issues, warnings, and errors.

### Tags
- `git/tags/create-tag.md` - Create a Git tag with explicit target and metadata.

### Merge
- `git/merge/merge-branch-to-main.md` - Analyze branch vs main and design a merge plan.

## Planning
- `planning/migration-plan.md` - Plan a safe, reversible migration.
- `planning/refactor-plan.md` - Plan a behavior-preserving refactor.
- `planning/mvp-plan.md` - Define a minimum viable product for a specific task.
