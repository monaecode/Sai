# SAI — Repository map

> Verified 2026-07-14 against commit `34827e7` on `Dezocode/Sai:main`.
> Keep current when top-level structure changes.

| Path | Purpose |
|---|---|
| `README.md` | Product description |
| `Team.md` | Team page (currently empty) |
| `.ai/` | ICM agent workspace — see `.ai/CONTEXT.md` |
| `.ai/_config/` | Repository, reporting, sync, security policy |
| `.ai/agents/` | CEO and secretary charters |
| `.ai/shared/memory/` | Durable memory (this folder) |
| `.ai/shared/schemas/` | JSON Schemas for events and stage outputs |
| `.ai/shared/references/` | Git workflow, testing, release policy |
| `.ai/stages/` | Six ICM stage contracts |
| `.ai/runs/` | Per-task working artifacts (Layer 4) |
| `.ai/audit/` | Audit trail documentation |
| `.cursor/rules/` | Shared Cursor operating rules |
| `.githooks/` | Reporting git hooks |
| `scripts/` | agent-report, agent-sync-drive, install-agent-hooks, verify-agent-audit |
| `.github/workflows/` | CI audit verification |

## Remotes and fork topology

- `Dezocode/Sai` — canonical, not a fork, default branch `main`.
- `monaecode/Sai` — fork of `Dezocode/Sai`, default branch `main`.
- Existing remote branches at time of writing: `main`,
  `cursor/cloud-env-setup-532b`, `cursor/sai-agent-framework-30d8`.
