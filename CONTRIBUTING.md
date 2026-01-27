# Contributing

Thanks for helping expand the prompt library. This repo is optimized for clarity, safety, and long-term growth.

## Before you add a prompt
- Check `docs/STYLE_GUIDE.md` for formatting and naming rules.
- Search `prompts/` to avoid duplicates.
- Decide the right category under `prompts/`.

## Adding a new prompt
1. Create a new markdown file under `prompts/` using kebab-case.
2. Follow the template in `docs/STYLE_GUIDE.md`.
3. Add the prompt to `docs/INDEX.md` and `prompts/README.md`.
4. Update `docs/STRUCTURE.md` if you introduce a new category.

## Updating an existing prompt
- Preserve intent unless explicitly changing behavior.
- Document major changes in the prompt itself when appropriate.

## General guidelines
- Use ASCII-only text.
- Keep prompts self-contained and executable in a single session.
- Avoid hidden assumptions; make constraints explicit.
