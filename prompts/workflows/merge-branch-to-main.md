# Merge Branch to Main (Analysis and Plan)

## Objective
Identify and reason about all differences between the current branch and `main`, at both the file and line level, to design a low-risk merge strategy.

## Scope
This includes:
- Which files differ.
- Which specific lines or regions differ.
- Why those differences exist.
- How they affect behavior, functionality, performance, or correctness.

## Autonomy and freedom (explicitly allowed)
You are allowed to:
- Choose any appropriate Git tooling (`git diff`, `git range-diff`, `git log`, `git blame`, etc.).
- Traverse the repository freely to understand context.
- Infer intent from commit history, naming, or code structure.
- Categorize changes using your own taxonomy if helpful.
- Propose alternative merge strategies (rebase-like, selective cherry-pick, manual reconciliation).
- Flag uncertainty and suggest follow-ups when intent is ambiguous.

You do not need permission to:
- Inspect files.
- Compare branches.
- Analyze historical context.
- Document hypotheses.

## Constraints (hard rules)
You must not:
- Modify functional code before a plan is documented.
- Assume `main` is correct by default.
- Resolve conflicts implicitly or silently.
- Perform refactors "while you are there."
- Optimize or clean code unless required for behavioral parity.

All changes must be intentional, justified, and planned.

## Required analysis dimensions
For every difference relative to `main`, explicitly assess:
- Type
  - New feature
  - Behavioral change
  - Bug fix
  - Refactor (no behavior change)
  - Accidental divergence
- Risk
  - Merge conflict risk
  - Behavioral regression risk
- Dependency
  - Does this change depend on other changes?
  - Is ordering important?

## Planning output requirements (`planning.md`)
Your plan must include:
- A file-by-file summary of differences vs `main`.
- Line- or block-level descriptions of key changes.
- Rationale for keeping, modifying, or discarding each change.
- A proposed merge sequence that minimizes risk.
- Notes on any unresolved ambiguity or decisions requiring human input.

No code edits may proceed unless they are:
- Referenced in `planning.md`.
- Justified by documented intent.
- Necessary to preserve current-branch behavior.

## Success criteria
This task is successful when:
- The full behavioral delta vs `main` is understood and documented.
- A merge can be executed confidently with no surprises.
- The current branch's functionality is preserved or intentionally improved.
- Future reviewers can understand why each merge decision was made.
