# Bug Hunt Workflow

## Purpose
Systematically reproduce, isolate, and explain a bug before making any fix. This workflow emphasizes evidence, minimal reproduction, and risk-aware analysis.

## Inputs
- Reported symptoms and environment details.
- Steps to reproduce (if available).
- Logs, traces, or screenshots (if available).

## Constraints
- Do not propose fixes until the bug is reproducible.
- Do not change code during investigation unless explicitly requested.
- Prefer read-only inspection and logging.

## Steps
1. Clarify the bug
   - Restate the symptom in one sentence.
   - Capture environment and version details.
   - Confirm expected vs actual behavior.
2. Reproduce
   - Attempt to reproduce in a clean environment.
   - If reproduction fails, enumerate possible missing conditions.
3. Minimize
   - Reduce to the smallest reproducible case.
   - Identify inputs, state, or timing that are necessary.
4. Localize
   - Trace the path from input to failure.
   - Identify suspicious modules or functions.
5. Hypothesize
   - List 2-3 plausible root causes.
   - Note what evidence would confirm or reject each.
6. Validate
   - Gather the evidence needed to confirm the most likely cause.
   - If evidence is insufficient, stop and report gaps.

## Output format
- Reproduction steps (minimal).
- Environment and assumptions.
- Likely root cause(s) with supporting evidence.
- Open questions or missing data.

## Completion criteria
- A minimal, repeatable reproduction exists.
- The likely root cause is documented with evidence.
- No code changes have been made unless explicitly approved.
