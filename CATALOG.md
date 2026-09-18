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

Socket's canonical multi-component Xcode workspace and `Package.swift`
templates are embedded in `run-workflow.fsx`. Apple Dev Skills also ships a
separate standalone XcodeGen SwiftUI app scaffold and Codex local-environment
configurations. Both source shapes are preserved here.

| Destination | Source skill asset |
| --- | --- |
| `templates/apple-workspace/scripts/run-workflow.fsx` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/scripts/run-workflow.fsx` |
| `templates/apple-workspace/managed-guidance/AGENTS-root.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-root.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-apps.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-apps.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-packages.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-packages.md` |
| `templates/apple-workspace/managed-guidance/AGENTS-services.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/AGENTS-services.md` |
| `templates/apple-workspace/managed-guidance/CONTRIBUTING.md` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/CONTRIBUTING.md` |
| `templates/apple-workspace/managed-guidance/pre-commit` | `plugins/apple-dev-skills/skills/bootstrap-xcode-workspace/assets/managed-guidance/pre-commit` |
| `templates/apple-workspace/codex-local-environments/swift-package.toml` | `plugins/apple-dev-skills/templates/codex-local-environments/swift-package.toml` |
| `templates/apple-workspace/codex-local-environments/xcode-project.toml` | `plugins/apple-dev-skills/templates/codex-local-environments/xcode-project.toml`, adapted to use configured build locations |
| `templates/apple-workspace/xcodegen/swiftui-app/project.yml.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/project.yml.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/App-Debug.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/App-Debug.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/App-Release.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/App-Release.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/App.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/App.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/Shared.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/Shared.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/Tests-Debug.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/Tests-Debug.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/Tests-Release.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/Tests-Release.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Configurations/Tests.xcconfig.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Configurations/Tests.xcconfig.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/AccentColor.colorset/Contents.json.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/AccentColor.colorset/Contents.json.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/AppIcon.appiconset/Contents.json.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/AppIcon.appiconset/Contents.json.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/Contents.json.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Sources/Resources/Assets.xcassets/Contents.json.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Sources/Resources/Localizable.xcstrings.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Sources/Resources/Localizable.xcstrings.tmpl` |
| `templates/apple-workspace/xcodegen/swiftui-app/Sources/Support/App.entitlements.tmpl` | `plugins/apple-dev-skills/templates/xcodegen/swiftui-app/Sources/Support/App.entitlements.tmpl` |

## Cloud Deployment

These five files form one fail-closed release and deployment contract. The
shell adapters intentionally refuse to run until their project-specific seams
are implemented.

| Destination | Source skill asset |
| --- | --- |
| `templates/cloud-deployment/dockerized-service-release/release-container.yml.tmpl` | `plugins/cloud-deployment-skills/skills/dockerized-service-release-deployment-workflow/assets/release-container.yml.tmpl` |
| `templates/cloud-deployment/dockerized-service-release/deploy-production.yml.tmpl` | `plugins/cloud-deployment-skills/skills/dockerized-service-release-deployment-workflow/assets/deploy-production.yml.tmpl` |
| `templates/cloud-deployment/dockerized-service-release/release-manifest.json.tmpl` | `plugins/cloud-deployment-skills/skills/dockerized-service-release-deployment-workflow/assets/release-manifest.json.tmpl` |
| `templates/cloud-deployment/dockerized-service-release/deploy-production-image.sh.tmpl` | `plugins/cloud-deployment-skills/skills/dockerized-service-release-deployment-workflow/assets/deploy-production-image.sh.tmpl` |
| `templates/cloud-deployment/dockerized-service-release/verify-production-health.sh.tmpl` | `plugins/cloud-deployment-skills/skills/dockerized-service-release-deployment-workflow/assets/verify-production-health.sh.tmpl` |

## Agent Workflow Documents

| Destination | Source skill asset |
| --- | --- |
| `templates/agent-workflows/automation-plan.template.md` | `plugins/agent-engineering-skills/skills/design-agent-automation-workflow/references/automation-plan-template.md` |
| `templates/agent-workflows/eval-plan.template.md` | `plugins/agent-engineering-skills/skills/design-agent-eval-workflow/references/eval-plan-template.md` |

## Model Lab

| Destination | Source skill asset |
| --- | --- |
| `templates/model-lab/compare-model-checkpoints/model-comparison-report.template.md` | `plugins/model-lab-skills/skills/compare-model-checkpoints/assets/model-comparison-report.md` |
| `templates/model-lab/design-model-experiment/experiment-manifest.template.json` | `plugins/model-lab-skills/skills/design-model-experiment/assets/experiment-manifest.json` |
| `templates/model-lab/evaluate-language-model/eval-cases.template.jsonl` | `plugins/model-lab-skills/skills/evaluate-language-model/assets/eval-cases.jsonl` |
| `templates/model-lab/evaluate-language-model/evaluation-report.template.md` | `plugins/model-lab-skills/skills/evaluate-language-model/assets/evaluation-report.md` |
| `templates/model-lab/prepare-language-model-dataset/dataset-card.template.md` | `plugins/model-lab-skills/skills/prepare-language-model-dataset/assets/dataset-card.md` |

## Swift Support Documents

| Destination | Source skill asset |
| --- | --- |
| `templates/swift-support/file-header-inventory.template.yaml` | `plugins/apple-dev-skills/skills/structure-swift-sources/references/file-header-inventory.template.yaml` |
| `templates/swift-support/official-sdk-exception.template.md` | `plugins/server-side-swift/skills/soto-aws-workflow/references/official-sdk-exception.template.md` |

## GitHub Configuration

The funding template is intentionally adapted from its Socket source: inactive
provider placeholders were removed, while Gale's active usernames were kept.

| Destination | Source |
| --- | --- |
| `templates/github/FUNDING.yml` | `plugins/apple-dev-skills/.github/FUNDING.yml`, adapted for reuse |

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
- Worked examples, example prompts, diagnostic references, and plugin artwork
  remain in their owning skills because they are not blank reusable templates.
- The Motion project/template/render contract remains in its owning skill
  because it is an operational safety checklist rather than a project file.
- Socket-coupled agent-plugin maintenance assets and generator/exporter scripts
  remain in their owning skills pending a deliberate generic-tooling design.
