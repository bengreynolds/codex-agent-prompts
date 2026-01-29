# Add Remote Branch and Link

## Purpose
Create a remote branch from a local branch and link it as the upstream.

## Inputs
- Local branch name.
- Remote name (default `origin` if not specified).
- Remote branch name (optional; defaults to local name).

## Constraints
- Use all available context from the current chat before acting.
- If local branch is missing, ask the user for it.
- If context is unclear, gather more from the repo (branch list, remotes) before proceeding.

## Steps
1. Confirm scope
   - Restate local branch, remote, and remote branch name.
   - Ask for missing inputs.
2. Inspect repository state
   - Verify local branch exists and is checked out.
   - Verify remote exists.
3. Push and link
   - Push local branch to the remote.
   - Set upstream tracking to the remote branch.
4. Verify
   - Confirm upstream is configured.
5. Report
   - Summarize actions and current tracking status.

## Output format
- Confirmed branches and remote.
- Actions taken.
- Upstream verification result.
- Next steps or approvals needed.

## Completion criteria
- Remote branch exists and upstream is linked, or
- Blocking issues are documented with a clear next action.
