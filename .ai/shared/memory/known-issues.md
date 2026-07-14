# SAI — Known issues and recurring failures

> Record verified, recurring problems and their workarounds. Remove entries
> when fixed at the source (rules, contracts, tests, or references).

## Open

- **Slack MCP delivery from cloud agents can fail silently** (observed
  2026-07-14): `slack_send_message` returned `no_text` and the message did
  not appear in #agentupdates. Workaround: verify delivery by reading the
  channel after posting; on failure, queue the event under
  `.git/agent-events/queue/` via `scripts/agent-report` and flush later.
- **No Google Drive credentials in cloud-agent VMs** (observed 2026-07-14):
  `scripts/agent-sync-drive` records status `pending` when
  `SAI_DRIVE_REMOTE` is unset. Drive mirroring must be run from a machine
  with a configured rclone remote.

## Resolved

(none yet)
