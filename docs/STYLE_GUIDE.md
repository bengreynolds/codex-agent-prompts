# Prompt Style Guide

## Goals
Make prompts readable, copyable, and safe to execute in an interpreter or agent session.

## Formatting
- Use clear, short headings and consistent section ordering.
- Prefer bullet lists for steps, constraints, and checklists.
- Keep paragraphs short and avoid dense blocks of text.
- Use inline code for file paths, command names, and literal tokens.
- Stick to ASCII characters to avoid encoding issues.

## Suggested prompt template
```
# Title

## Purpose

## Inputs

## Constraints

## Steps

## Completion criteria
```

## Naming
- Use kebab-case filenames.
- Be explicit in the filename about the action or scope.
- Avoid abbreviations unless they are standard.

## Content rules
- Prefer explicit over implicit instructions.
- Document safety constraints and ambiguity handling.
- Avoid mixing planning and execution instructions in the same prompt.
