# Code Cleanup (Redundancy and Patch Debt)

## Purpose
Identify and remove leftover artifacts from previous patches, duplicate logic, and unnecessary code without changing behavior.

## Inputs
- Target files, modules, or directories.
- Known areas of patch debt or duplication (if any).
- Test or verification tools available.

## Constraints
- Preserve existing behavior unless explicitly approved.
- Avoid large refactors; prefer small, safe cleanups.
- If uncertainty exists, document it and ask for guidance before changes.

## Steps
1. Locate candidates
   - Scan for duplicated logic, dead code, commented-out blocks, or obsolete paths.
2. Validate relevance
   - Confirm whether code is still used or required.
   - Check call sites and tests for dependencies.
3. Propose cleanup
   - List specific removals or consolidations.
   - Provide the safety rationale for each change.
4. Execute safely
   - Make minimal edits and keep diffs small.
   - Run verification steps if available.
5. Report results
   - Summarize what was removed or consolidated.
   - Note any residual risks or follow-ups.

## Output format
- Targets and rationale.
- Proposed cleanup items.
- Verification plan.
- Results and remaining risks.

## Completion criteria
- Redundant or unnecessary code is removed or consolidated.
- Behavior is preserved and verified where possible.
- Any risky or uncertain items are explicitly documented.
