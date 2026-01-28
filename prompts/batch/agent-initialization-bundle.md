# Agent Initialization Bundle

## Purpose
Run a single, condensed workflow that covers: targeted context building, architecture mimicry, plan review, and safe execution. This is intended for consistent agent onboarding at the start of a task while still prioritizing accuracy, precision, and safety.

## Inputs
- Task goal and desired outcome (explicitly stated).
- Reference code or directories to model (examples of existing style and structure).
- `agent.md` and `planning.md` (if present).
- Constraints and preferences (time, scope, risk tolerance, tooling restrictions).
- Environment details if relevant (languages, frameworks, versions).

## Constraints
- Prefer accuracy, precision, and safety over speed.
- Keep context gathering scoped to the task, but do not skip needed context.
- Do not introduce new patterns or dependencies without approval.
- If required inputs are missing, ask the user before proceeding.
- Do not execute changes without understanding the current plan and constraints.
- Use summaries instead of long excerpts unless details are required for correctness.

## Steps
1. Confirm the goal
   - Restate the task in one sentence.
   - Define success criteria and explicit boundaries (what is in and out of scope).
   - Ask for any missing required inputs before proceeding.
2. Gather targeted context
   - Identify the most relevant files, directories, and modules.
   - Read only the sections needed to understand the task and risks.
   - Summarize intent, inputs/outputs, dependencies, and sharp edges.
3. Mimic existing architecture
   - Extract naming conventions, structure, and formatting from reference code.
   - Confirm architectural boundaries (layers, modules, ownership).
   - Align any planned changes with existing patterns.
4. Review plan state
   - Summarize `agent.md` and `planning.md` if present.
   - Note constraints, assumptions, risks, and open questions.
   - Identify any mismatch between plans and current codebase reality.
5. Execute safely
   - Follow the plan and constraints without shortcuts.
   - If blocked by missing context, pause and gather only what is required.
   - If uncertainty remains, request clarification before proceeding.

## Output format
- Goal and success criteria.
- Context summary.
- Architecture and style conventions.
- Plan and constraint summary.
- Actions taken or next actions.
- Clarifications needed.

## Completion criteria
- The agent can proceed safely with aligned context and conventions, or
- The agent requests the minimum needed clarification to proceed.
