# Contributing to FileTemplates

## Overview

This repository is a personal template library. Contributions should make a
template easier to reuse, add a clearly owned template, or improve provenance
and discoverability.

## Contribution Workflow

Keep each change focused on one template family. When importing a file, add its
exact origin to `CATALOG.md`. When changing a copied file, state whether the
change is a deliberate personal divergence or a refresh from its source.

## Verification

Before review:

1. Confirm every file under `templates/` appears in `CATALOG.md`.
2. Check Markdown links and JSON syntax.
3. Review scripts for source-relative paths before treating them as runnable in
   this repository.
4. Confirm no generated caches, credentials, or machine-local state were added.

## License and Contribution Terms

Contributions are licensed under the repository's Apache License 2.0. License
samples under `templates/licenses/` retain the terms written in those files.
