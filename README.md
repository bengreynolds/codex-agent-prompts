# Codex Agent Prompts

A curated set of prompt templates for OpenAI Codex (VS Code integrated) to run structured, safe agent workflows. The focus is on planning, execution protocols, and codebase context building.

## What is this repository?
This repo is a growing library of reusable prompts that standardize how an agent should gather context, plan, and execute code changes. Each prompt is written as a self-contained workflow you can drop into an agent session.

## Quick start
1. Pick a workflow from `prompts/workflows/`.
2. Copy the prompt into your agent session (or reference the file).
3. Fill in any placeholders like repository paths or filenames.

## Repository layout
- `prompts/` Prompt library grouped by type.
- `docs/` Documentation for structure and writing standards.
- `CONTRIBUTING.md` Guidelines for expanding the library.

## About agent.md and planning.md
Some workflows in this repo assume two local, session-specific files:

- `agent.md` records the agent's constraints, assumptions, decision rules, and boundaries of autonomy.
- `planning.md` records observations, intent, risks, and a step-by-step plan.

These files are typically created at the start of a task (see `prompts/workflows/branch-setup.md` and `prompts/workflows/agent-planning-review.md`). They are meant to be temporary working artifacts for a single task or branch session, not permanent documentation.

Use cases:
- `agent.md` anchors safety and decision constraints before any edits.
- `planning.md` provides traceability from intent to action and is referenced during execution.

## Index
See `docs/INDEX.md` for the full prompt catalog.
