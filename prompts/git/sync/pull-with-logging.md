# Pull With Issue and Error Logging

## Purpose
Pull the latest changes for a branch while capturing issues, warnings, and errors for traceability.

## Inputs
- Current branch name.
- Remote name (default `origin` if not specified).
- Any constraints (timebox, risk tolerance, testing expectations).

## Constraints
- Use all available context from the current chat before acting.
- If current branch is missing, ask the user for it.
- If context is unclear, gather more from the repo (status, branches, recent commits) before proceeding.
- Do not proceed with a dirty working tree without explicit approval.

## Steps
1. Confirm scope
   - Restate the current branch and remote.
   - Ask for missing inputs.
2. Inspect repository state
   - Check working tree cleanliness and current branch.
   - Fetch remote updates if needed.
3. Pull with logging
   - Run pull and capture output.
   - Record warnings, conflicts, or errors verbatim where relevant.
4. Verify
   - Run required tests or checks if requested.
5. Report
   - Summarize the pull result and any issues.

## Output format
- Confirmed branch and remote.
- Pull output summary and any errors.
- Conflicts or warnings (if any).
- Verification results.
- Next steps or required approvals.

## Completion criteria
- Pull completes and issues are documented, or
- Blocking errors are reported with a clear next action.
