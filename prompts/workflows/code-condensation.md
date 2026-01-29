# Code Condensation (Behavior Preserving)

## Purpose
Reduce code size and complexity while maintaining current behavior, public interfaces, and side effects.

## Inputs
- Target files, modules, or directories.
- Constraints on readability, style, or performance.
- Tests or verification tools available.

## Constraints
- No behavior changes unless explicitly approved.
- Preserve public interfaces and input/output contracts.
- Avoid cleverness that reduces readability.

## Steps
1. Establish invariants
   - List behaviors that must not change.
   - Identify public APIs and side effects.
2. Identify condensation opportunities
   - Remove unnecessary repetition.
   - Simplify control flow without changing logic.
3. Propose changes
   - Provide a concise list of edits with rationale.
   - Call out any risks to clarity or behavior.
4. Apply minimal edits
   - Keep diffs small and localized.
   - Validate against invariants.
5. Verify
   - Run available tests or checks.
   - If tests are unavailable, document the gap.

## Output format
- Invariants and interfaces.
- Proposed condensation changes.
- Verification plan.
- Results and open risks.

## Completion criteria
- Code is smaller or simpler with preserved behavior.
- Interfaces and side effects remain unchanged.
- Verification results are recorded.
