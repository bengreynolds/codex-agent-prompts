# Refactor Plan

## Purpose
Plan a refactor that preserves behavior while improving structure, readability, or maintainability.

## Inputs
- Target modules or files.
- Known pain points or code smells.
- Tests or verification tools available.

## Constraints
- No behavior changes unless explicitly approved.
- Protect critical paths with tests or checks.
- Prefer small, reviewable steps.

## Steps
1. Define intent
   - What the refactor will and will not change.
   - Behavioral invariants to preserve.
2. Identify risk areas
   - Tight coupling, side effects, and hidden dependencies.
3. Propose sequence
   - Ordered steps with clear checkpoints.
   - Opportunities to validate at each step.
4. Safeguards
   - Tests to add or run before and after.
   - Metrics or diffs to confirm no regressions.
5. Rollback strategy
   - How to revert if behavior changes are detected.

## Output format
- Scope and invariants.
- Step-by-step plan with checkpoints.
- Safeguards and verification steps.
- Rollback approach.

## Completion criteria
- The plan is detailed enough to execute without improvisation.
- Invariants and verification steps are explicit.
- Risk and rollback are addressed.
