# Create Tag

## Purpose
Create a Git tag for a specific commit or the current HEAD with clear metadata.

## Inputs
- Current branch name (if tagging HEAD).
- Tag name.
- Tag type (annotated or lightweight).
- Tag message (for annotated tags).
- Target commit SHA (optional).

## Constraints
- Use all available context from the current chat before acting.
- If tag name or target is missing, ask the user for it.
- If context is unclear, gather more from the repo (recent commits, existing tags) before proceeding.

## Steps
1. Confirm scope
   - Restate tag name, target commit/branch, and tag type.
   - Ask for missing inputs.
2. Inspect repository state
   - Verify target commit exists.
   - Check for tag name collisions.
3. Create tag
   - Create the tag with the requested type and message.
4. Verify
   - List the tag and confirm it points to the intended commit.
5. Report
   - Summarize the tag details and any issues.

## Output format
- Tag details (name, type, target).
- Verification outcome.
- Next steps (e.g., push tag) if requested.

## Completion criteria
- Tag is created and verified, or
- Blocking issues are documented with a clear next action.
