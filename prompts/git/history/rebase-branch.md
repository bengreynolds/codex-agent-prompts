# Rebase Branch

## Purpose
Rebase a current branch onto a target branch as a one-time task while preserving intent, recording conflicts, and keeping the result stable.

## Inputs
- Current branch name.
- Target branch name.
- Any constraints (risk tolerance, timebox, testing expectations).

## Constraints
- Use all available context from the current chat before acting.
- If current or target branch is missing, ask the user for it.
- If context is unclear, gather more from the repo (status, branches, recent commits) before proceeding.
- Do not proceed if the working tree has uncommitted changes without explicit approval.

## Steps
1. Confirm scope
   - Restate current and target branch.
   - Ask for missing inputs.
2. Inspect repository state
   - Check working tree cleanliness and current branch.
   - Fetch latest remote refs if needed.
3. Perform rebase
   - Rebase current branch onto target.
   - Capture conflicts and resolution notes.
4. Verify
   - Run required tests or checks.
   - Record outcomes and any regressions.
5. Report
   - Summarize changes, conflicts, and verification results.

## Output format
- Confirmed branches and constraints.
- Rebase actions taken.
- Conflicts and resolutions (if any).
- Verification results.
- Next steps or required approvals.

## Completion criteria
- Rebase completes cleanly with verification results, or
- Blocking issues are documented with a clear next action.
