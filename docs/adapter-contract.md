# Runtime adapter contract

An adapter translates portable role cards into a bot network. It documents how
to provide these capabilities and marks unsupported ones:

| Capability | Required behavior |
| --- | --- |
| Named profiles | Durable identity and instructions per role |
| Shared context | Read-only access to brief and linked records |
| Messaging | Direct handoffs and optional group coordination |
| Scheduling | Recurring reports or scans; no destructive defaults |
| Tools/connectors | Explicit allowlist with least privilege |
| Workspace | Isolated branch, worktree, or draft area |
| Review | Evidence, human approval, and PR/merge boundary |

An adapter must not invent vendor features. If a capability is missing, keep the
workflow manual and say so.
