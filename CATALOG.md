# Template Catalog

This catalog records the initial template snapshot and its exact authored
source. Source paths are relative to the local `gaelic-ghost/socket` repository
unless another repository is named explicitly.

## Repository Documents

These pairs stay together: each Markdown scaffold is governed by its adjacent
JSON contract.

| Destination | Source skill asset |
| --- | --- |
| `templates/repository-documents/readme/README.template.md` | `plugins/repository-skills/skills/maintain-project-readme/assets/README.template.md` |
| `templates/repository-documents/readme/document.contract.json` | `plugins/repository-skills/skills/maintain-project-readme/assets/document.contract.json` |
| `templates/repository-documents/contributing/CONTRIBUTING.template.md` | `plugins/repository-skills/skills/maintain-project-contributing/assets/CONTRIBUTING.template.md` |
| `templates/repository-documents/contributing/document.contract.json` | `plugins/repository-skills/skills/maintain-project-contributing/assets/document.contract.json` |
| `templates/repository-documents/agents/AGENTS.template.md` | `plugins/repository-skills/skills/maintain-project-agents/assets/AGENTS.template.md` |
| `templates/repository-documents/agents/document.contract.json` | `plugins/repository-skills/skills/maintain-project-agents/assets/document.contract.json` |
| `templates/repository-documents/roadmap/ROADMAP.template.md` | `plugins/repository-skills/skills/maintain-project-roadmap/assets/ROADMAP.template.md` |
| `templates/repository-documents/roadmap/document.contract.json` | `plugins/repository-skills/skills/maintain-project-roadmap/assets/document.contract.json` |

## Repository Maintenance

The `installer/` directory is the skill-facing entrypoint. `shared/`, `runtime/`,
`profiles/`, and `github/` contain the files it installs or uses.

| Destination | Source skill asset |
| --- | --- |
| `templates/repository-maintenance/installer/maintain-project-repo.fsx` | `plugins/repository-skills/skills/maintain-project-repo/scripts/maintain-project-repo.fsx` |
| `templates/repository-maintenance/installer/maintain-project-docs.fsx` | `plugins/repository-skills/skills/maintain-project-repo/scripts/maintain-project-docs.fsx` |
| `templates/repository-maintenance/shared/ProjectDocs.fsx` | `plugins/repository-skills/shared/project-docs/ProjectDocs.fsx` |
| `templates/repository-maintenance/shared/DocsCoordinator.fsx` | `plugins/repository-skills/shared/project-docs/DocsCoordinator.fsx` |
| `templates/repository-maintenance/managed-assets.json` | `plugins/repository-skills/skills/maintain-project-repo/assets/managed-assets.json` |
| `templates/repository-maintenance/github/validate-repo-maintenance.yml` | `plugins/repository-skills/skills/maintain-project-repo/assets/github/validate-repo-maintenance.yml` |
| `templates/repository-maintenance/runtime/maintain-project-docs.fsx` | `plugins/repository-skills/skills/maintain-project-repo/assets/repo-maintenance/maintain-project-docs.fsx` |
| `templates/repository-maintenance/runtime/repo-maintenance.fsx` | `plugins/repository-skills/skills/maintain-project-repo/assets/repo-maintenance/repo-maintenance.fsx` |
| `templates/repository-maintenance/runtime/repo-maintenance.just` | `plugins/repository-skills/skills/maintain-project-repo/assets/repo-maintenance/repo-maintenance.just` |
| `templates/repository-maintenance/runtime/syncing/README.md` | `plugins/repository-skills/skills/maintain-project-repo/assets/repo-maintenance/syncing/README.md` |
| `templates/repository-maintenance/profiles/apple/.swiftformat` | `plugins/repository-skills/skills/maintain-project-repo/assets/profiles/apple/repo-maintenance/.swiftformat` |
| `templates/repository-maintenance/profiles/apple/.swiftlint.yml` | `plugins/repository-skills/skills/maintain-project-repo/assets/profiles/apple/repo-maintenance/.swiftlint.yml` |
| `templates/repository-maintenance/profiles/xcode-workspace/validations/40-xcode-workspace-layout.fsx` | `plugins/repository-skills/skills/maintain-project-repo/assets/profiles/xcode-workspace/repo-maintenance/validations/40-xcode-workspace-layout.fsx` |
| `templates/repository-maintenance/profiles/xcode-workspace/workspace/validate-components.fsx` | `plugins/repository-skills/skills/maintain-project-repo/assets/profiles/xcode-workspace/repo-maintenance/workspace/validate-components.fsx` |

## Apple Workspace and Swift Package Scaffolding

Socket's Xcode workspace and `Package.swift` templates are embedded in
`run-workflow.fsx`; there are no separate canonical scaffold files to copy.
Keeping the generator intact preserves those templates exactly.

| Destination | Source skill asset |
| --- | --- |
| `templates/apple-workspace/scripts/run-workflow.fsx` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/scripts/run-workflow.fsx` |
| `templates/apple-workspace/managed-guidance/AGENTS-root.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-root.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-apps.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-apps.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-packages.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-packages.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-services.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-services.md` |
| `templates/apple-workspace/managed-guidance/CONTRIBUTING.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/CONTRIBUTING.md` |
| `templates/apple-workspace/managed-guidance/pre-commit` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/pre-commit` |

## Licenses

| Destination | Source |
| --- | --- |
| `templates/licenses/apache-2.0/LICENSE` | Socket root `LICENSE` |
| `templates/licenses/mit/LICENSE` | `gaelic-ghost/NyextStepOfficeTower/LICENSE` |

## Deliberate Exclusions and Gaps

- Installed plugin caches, generated Socket root exports, `.DS_Store` files,
  and test caches are not source templates and are excluded.
- The `dotnet-skills` plugin has no `assets/` or `scripts/` payloads. Its
  examples are workflow documentation, not standalone templates.
- Specialized templates outside the requested scope, such as agent automation,
  model evaluation, Motion, and server-side Swift exception templates, remain
  in their owning skills.
