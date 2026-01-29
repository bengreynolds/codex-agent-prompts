# Remove Remote Branch

## Purpose
Delete a remote branch safely, with explicit confirmation and verification.

## Inputs
- Remote name (default `origin` if not specified).
- Remote branch name.
- Confirmation that deletion is intended.

## Constraints
- Use all available context from the current chat before acting.
- If remote branch or confirmation is missing, ask the user for it.
- If context is unclear, gather more from the repo (remote branches, protections) before proceeding.
- Do not delete protected or default branches without explicit approval.

## Steps
1. Confirm scope
   - Restate remote and branch to delete.
   - Request explicit confirmation.
2. Inspect repository state
   - Verify the remote branch exists.
   - Check for protections or default branch status.
3. Delete
   - Delete the remote branch.
4. Verify
   - Prune remotes and confirm deletion.
5. Report
   - Summarize deletion and verification outcome.

## Output format
- Remote and branch confirmed.
- Deletion action and verification.
- Any errors or blockers.

## Completion criteria
- Remote branch is deleted and verified, or
- Blocking issues are documented with a clear next action.
