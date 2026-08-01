# CLAUDE.md

Personal recipe collection. Markdown files organized by protein/category.

## Layout

- Top-level `.md` files for standalone recipes (e.g. `lasagna.md`, `turkey.md`).
- Subdirectories group by protein or category: `beef/`, `chicken/`, `fish/`, `pork/`, `soup/`, `smoothies/`, `sides/`, etc.
- New recipes go in the matching subdirectory when one exists; otherwise create the directory (singular, lowercase).
- Filenames are lowercase kebab-case: `french-onion.md`, `bacon-wrapped-chicken-breast.md`.

## Recipe format

Preferred structure (see `beef/`, `soup/french-onion.md` for examples):

```markdown
# Recipe Name

## Ingredients

- item with quantity

## Instructions

1. Step one.
2. Step two.

## References

- [Source description](https://...)
```

Older files use looser formats — don't retrofit unless the user asks.

## Commits

Conventional Commits, always `chore` scope for recipe adds:

```
chore: add french onion soup recipe
```

One recipe per commit. Branch name mirrors the commit: `chore/add-<recipe>-recipe`.

## Scope

This is a personal repo with no code, no tests, no CI. Skip the tooling/architecture reflexes — the only task is capturing recipes cleanly.
