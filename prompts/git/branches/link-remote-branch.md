# Link Existing Branch to Remote

## Purpose
Link a local branch to an existing remote branch by setting the upstream.

## Inputs
- Local branch name.
- Remote name (default `origin` if not specified).
- Remote branch name.

## Constraints
- Use all available context from the current chat before acting.
- If local or remote branch is missing, ask the user for it.
- If context is unclear, gather more from the repo (branch list, remotes) before proceeding.

## Steps
1. Confirm scope
   - Restate local branch, remote, and remote branch name.
   - Ask for missing inputs.
2. Inspect repository state
   - Verify local branch exists.
   - Verify remote branch exists.
3. Link
   - Set upstream tracking to the remote branch.
4. Verify
   - Confirm tracking status.
5. Report
   - Summarize actions and tracking result.

## Output format
- Confirmed branches and remote.
- Upstream link result.
- Errors or blockers.

## Completion criteria
- Upstream is configured and verified, or
- Blocking issues are documented with a clear next action.
