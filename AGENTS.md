# AGENTS.md

## Repository Scope

This repository owns Gale's personal, reusable file templates. It is distinct
from Socket: copied files may intentionally diverge after their provenance is
recorded in `CATALOG.md`.

## Source of Truth

- `CATALOG.md` owns the source-to-destination inventory.
- `templates/` owns the reusable copies.
- Socket paths named in the catalog are provenance, not live dependencies.

## Working Rules

- Preserve template placeholders and reusable wording unless a change is meant
  to specialize a template.
- Keep related templates and their contracts together.
- Record newly imported files and their provenance in `CATALOG.md`.
- Do not silently resynchronize a personal template from Socket over local
  divergence.

## Validation

Verify that every file below `templates/` is represented in `CATALOG.md`, links
resolve, and copied scripts retain their executable bit when applicable.

## Safety Boundaries

Ask before publishing changes that replace intentionally diverged personal
templates with newer Socket versions or that change this repository's license.
