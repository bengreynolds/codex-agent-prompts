# Create Codebase Context (Low Profile)

## Purpose
Gain just enough context to execute a specific goal or task without excessive token usage. This prompt prioritizes targeted discovery over exhaustive codebase review.

## Inputs
- A clear goal or task statement.
- Optional constraints (time, scope, risk tolerance).

## Constraints
- Keep context collection minimal and task-scoped.
- Avoid full-file dumps unless strictly necessary.
- Prefer summaries over long excerpts.
- If context is insufficient during planning or execution, pause and gather only the missing context.
- If a required input (goal/task statement) is missing, ask the user for it before proceeding.
- Accuracy, precision, and safety take precedence over speed or token reduction.

## Steps
1. Confirm the goal
   - If the goal or task is not provided, ask the user for it.
   - Restate the task in one sentence.
   - Identify success criteria and boundaries.
2. Map the likely area
   - List the most relevant directories, files, or modules.
   - Use lightweight discovery (file tree, grep, or file headers).
3. Collect minimal context
   - Read only the sections needed to understand the task.
   - Summarize in short bullets: intent, inputs/outputs, and risks.
4. Plan with limited context
   - Draft a plan using only the gathered information.
   - Explicitly call out unknowns that might block execution.
5. On-demand context expansion
   - If a step cannot proceed, stop and gather just enough context for that step.
   - Repeat until the next step is unblocked.

## Output format
- Goal and success criteria.
- Current context summary (short bullets).
- Known unknowns.
- Plan or next action.

## Completion criteria
- The task can proceed with the current context, or
- The missing context is identified with a targeted next step to obtain it.
