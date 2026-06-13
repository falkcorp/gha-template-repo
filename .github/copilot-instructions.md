<!-- file: .github/copilot-instructions.md -->
<!-- version: 2.4.0 -->
<!-- guid: 4d5e6f7a-8b9c-0d1e-2f3a-4b5c6d7e8f9a -->
<!-- last-edited: 2026-06-13 -->

# gha-template-repo — Additional Context

Org-wide coding standards (file headers, language rules, commit format) are at
**https://github.com/falkcorp/.github** and apply automatically to this repo.

For full project context: **CLAUDE.md** at the repo root.

## Project overview

Template repository — single source of truth for all GHA action repos. Language: YAML.

## Key directories

- `.github/workflows/` — Reusable workflows called by other repositories
- `.github/instructions/` — Modular AI agent rules with language targeting
- `scripts/` — Python automation tools for cross-repo operations

## Critical constraints

- All commits MUST use conventional commit format: `type(scope): description`.
- Sync changes to target repos using `scripts/intelligent_sync_to_repos.py`.
- This repo manages configurations propagated across the falkcorp org.
