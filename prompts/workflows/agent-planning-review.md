# Agent and Planning Review

## Purpose
Rapidly understand the current state of work by reviewing `agent.md` and `planning.md`, then correlate that context with the most recent Git activity. This provides a high-level project understanding without deep code spelunking.

## Inputs
- `agent.md` and `planning.md` in the repository root (if present).
- Latest commit history across all branches.

## Constraints
- Do not modify code during this review.
- Prefer read-only inspection and summary.
- If `agent.md` or `planning.md` is missing, report it and continue with available context.

## Steps
1. Read `agent.md`
   - Extract constraints, assumptions, and decision rules.
   - Note any explicit boundaries or prohibited actions.
2. Read `planning.md`
   - Summarize goals, observations, and planned actions.
   - Identify any open questions or unresolved risks.
3. Review recent Git activity
   - Use: `git log --all -10 --oneline --decorate`
   - Summarize the themes of recent changes and what they imply.
4. Synthesize current state
   - Combine plan intent with recent commits to infer current direction.
   - Flag mismatches between plan and actual changes.

## Output format
- Constraints and assumptions (from `agent.md`).
- Current plan summary (from `planning.md`).
- Recent Git activity summary (latest 10 commits across all branches).
- Inferred current state and open questions.

## Completion criteria
- `agent.md` and `planning.md` are reviewed and summarized.
- Recent commit history is summarized.
- A concise picture of the current state of work is produced.
