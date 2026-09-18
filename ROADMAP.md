# FileTemplates Roadmap

## Vision

Maintain one easy-to-browse home for Gale's reusable project files while
allowing personal conventions to evolve independently from Socket products.

## Product Principles

- Prefer useful standalone files over skill packaging.
- Preserve provenance without requiring the source repository at runtime.
- Keep template families small, explicit, and easy to copy.

## Milestone 0: Foundation

### Status

Complete

### Scope

- [x] Define the initial template taxonomy.
- [x] Inventory the relevant Socket-authored assets.
- [x] Copy repository documents, FSX maintenance tooling, Apple workspace
  scaffolding, and common licenses.
- [x] Publish the initial snapshot to the public GitHub repository.

### Exit Criteria

- [x] The public remote contains the cataloged initial snapshot.
- [x] Repository identity, public visibility, and the `main` default branch are
  verified through GitHub.

## Backlog Candidates

- Extract the Swift/Xcode scaffold fragments from the FSX generator into
  independently reusable templates if Socket adopts the same source split.
- Add first-party .NET project templates when Gale chooses concrete F# and C#
  shapes; do not derive them silently from guidance examples.
- Add a deliberate refresh/diff workflow for comparing personal copies with
  newer Socket sources.
- Decide whether to align optional GitHub settings such as projects, wiki,
  Dependabot security updates, private vulnerability reporting, and branch
  protection with the maintained public-repository baseline.

## History

- 2026-09-18: Created the initial catalog and personal template taxonomy.
