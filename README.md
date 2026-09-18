# FileTemplates

A personal, public library of reusable project templates and repository tooling.

## Overview

This repository keeps Gale's commonly used templates independent from the
Socket skills that originally packaged many of them. The initial collection is
a curated snapshot: files are copied here so they can evolve as personal
templates without changing Socket's product behavior.

See [CATALOG.md](./CATALOG.md) for the complete source-to-destination inventory.

## Repository Structure

```text
templates/
├── agent-workflows/          # Agent automation and evaluation plans
├── apple-workspace/          # Swift package, XcodeGen, and Xcode workspace scaffolding
├── cloud-deployment/         # Container release and deployment contracts
├── github/                   # Reusable GitHub repository configuration
├── licenses/                 # Apache-2.0 and MIT license text
├── model-lab/                # Experiment, evaluation, comparison, and dataset records
├── repository-documents/     # README, CONTRIBUTING, AGENTS, and ROADMAP templates
├── repository-maintenance/   # FSX runtime, profiles, and GitHub validation
└── swift-support/            # Focused Swift inventory and exception records
```

## Provenance

Most files in the initial snapshot come from authored assets in the local
`gaelic-ghost/socket` source repository. Generated Socket exports and installed
plugin caches are intentionally excluded. The MIT license sample comes from a
Gale-owned MIT-licensed repository because Socket does not currently ship an
MIT license template.

The .NET Socket plugin currently contains workflow guidance but no reusable
template or script assets. No .NET project files were invented for this
snapshot. The F# scripts included here are the real repository and Apple
workspace tooling owned by the relevant Socket skills.

## Using the Templates

Copy the smallest relevant directory into a new project, then replace project
specific names, identifiers, versions, and policy text. Treat scripts as source
material until their relative paths and dependencies have been reviewed for the
target repository.

## License

This repository is licensed under the [Apache License 2.0](./LICENSE). Individual
license samples under `templates/licenses/` are provided as reusable license
texts and retain the terms written in those files.
