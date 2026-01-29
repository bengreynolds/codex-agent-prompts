# Reestablish Session Context After Chat Condensation

## Purpose
Rebuild working context when prior chat history has been condensed to save tokens. Use repository signals (Git history) and any available user-provided summaries to recover intent, constraints, and current state.

## Inputs
- Branch name or target working branch.
- Any user-provided summaries, notes, or artifacts from the prior chat.
- Repository state and Git history.

## Constraints
- Accuracy, precision, and safety take precedence over speed.
- Do not invent missing context; request it explicitly.
- Prefer primary sources (repo files, commit history) over assumptions.

## Steps
1. Confirm the scope
   - Ask for the branch name and the current task goal.
   - Ask for any available chat summary, notes, or key decisions.
2. Recover plan artifacts
   - Look for `agent.md` and `planning.md` in the repo.
   - If missing, ask the user to provide prior content or recreate them.
3. Review recent Git history
   - Inspect recent commits on the target branch.
   - If the branch history is insufficient, expand to other branches for context.
4. Reconstruct intent
   - Align recent commits with any plan artifacts and user notes.
   - Identify probable goals, constraints, and in-progress work.
5. Validate with the user
   - Present a concise reconstructed summary.
   - Ask for confirmation or corrections before proceeding.

## Output format
- Branch and task scope.
- Recovered constraints and plan summary.
- Recent Git activity summary.
- Reconstructed current state.
- Clarifications needed.

## Completion criteria
- A validated, user-confirmed context summary exists, or
- Missing information is explicitly requested with next steps.
